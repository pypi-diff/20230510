# Comparing `tmp/zep_python-0.1.10.tar.gz` & `tmp/zep_python-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zep_python-0.1.10.tar", max compression
+gzip compressed data, was "zep_python-0.2.tar", max compression
```

## Comparing `zep_python-0.1.10.tar` & `zep_python-0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-05-09 06:06:56.672383 zep_python-0.1.10/LICENSE
--rw-r--r--   0        0        0       12 2023-05-09 06:06:56.672383 zep_python-0.1.10/README.md
--rw-r--r--   0        0        0      549 2023-05-09 06:06:56.672383 zep_python-0.1.10/pyproject.toml
--rw-r--r--   0        0        0      158 2023-05-09 06:06:56.672383 zep_python-0.1.10/zep_python/__init__.py
--rw-r--r--   0        0        0     1026 2023-05-09 06:06:56.672383 zep_python-0.1.10/zep_python/exceptions.py
--rw-r--r--   0        0        0     6590 2023-05-09 06:06:56.672383 zep_python-0.1.10/zep_python/models.py
--rw-r--r--   0        0        0      605 2023-05-09 06:06:56.672383 zep_python-0.1.10/zep_python/utils.py
--rw-r--r--   0        0        0    10865 2023-05-09 06:06:56.672383 zep_python-0.1.10/zep_python/zep_client.py
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 zep_python-0.1.10/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-10 02:08:40.024333 zep_python-0.2/LICENSE
+-rw-r--r--   0        0        0    10553 2023-05-10 02:08:40.024333 zep_python-0.2/README.md
+-rw-r--r--   0        0        0      620 2023-05-10 02:08:40.024333 zep_python-0.2/pyproject.toml
+-rw-r--r--   0        0        0      282 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/exceptions.py
+-rw-r--r--   0        0        0     6823 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/models.py
+-rw-r--r--   0        0        0      670 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/utils.py
+-rw-r--r--   0        0        0    10971 2023-05-10 02:08:40.024333 zep_python-0.2/zep_python/zep_client.py
+-rw-r--r--   0        0        0    11180 1970-01-01 00:00:00.000000 zep_python-0.2/PKG-INFO
```

### Comparing `zep_python-0.1.10/LICENSE` & `zep_python-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zep_python-0.1.10/zep_python/exceptions.py` & `zep_python-0.2/zep_python/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,16 +25,27 @@
     def __init__(
         self, message: str, response_data: Optional[Dict[Any, Any]] = None
     ) -> None:
         super().__init__(message)
         self.response_data = response_data
 
 
-class UnexpectedResponseError(ZepClientError):
+class APIError(ZepClientError):
     """
     Raised when the API response format is unexpected.
 
     Inherits from ZepClientError.
     """
 
     def __init__(self, message: str) -> None:
         super().__init__(message)
+
+
+class NotFoundError(ZepClientError):
+    """
+    Raised when the API response contains no results.
+
+    Inherits from ZepClientError.
+    """
+
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
```

### Comparing `zep_python-0.1.10/zep_python/models.py` & `zep_python-0.2/zep_python/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from __future__ import annotations
 
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional, Sequence
 
 
 class Memory:
     """
     Represents a memory object with messages, metadata, and other attributes.
 
-    :param messages: A list of message objects, where each message contains a role and content.
+    :param messages: A list of message objects, where each message contains a role and
+                     content.
     :type messages: Optional[List[Dict[str, Any]]]
     :param metadata: A dictionary containing metadata associated with the memory.
     :type metadata: Optional[Dict[str, Any]]
     :param summary: A dictionary containing a summary of the memory.
     :type summary: Optional[Dict[str, Any]]
     :param uuid: A unique identifier for the memory.
     :type uuid: Optional[str]
@@ -19,23 +20,30 @@
     :type created_at: Optional[str]
     :param token_count: The token count of the memory.
     :type token_count: Optional[int]
     """
 
     def __init__(
         self,
-        messages: Optional[List[Dict[str, Any]]] = None,
+        messages: Optional[Sequence[Dict[str, Any] | Message]] = None,
         metadata: Optional[Dict[str, Any]] = None,
         summary: Optional[Dict[str, Any]] = None,
         uuid: Optional[str] = None,
         created_at: Optional[str] = None,
         token_count: Optional[int] = None,
-    ):
+    ) -> None:
         if messages is not None:
-            self.messages = [Message(**message_data) for message_data in messages]
+            self.messages = [
+                (
+                    Message(**message_data)
+                    if isinstance(message_data, dict)
+                    else message_data
+                )
+                for message_data in messages
+            ]
         else:
             self.messages = []
         self.metadata = metadata if metadata is not None else {}
         self.summary = Summary(**summary) if summary else None
         self.uuid = uuid
         self.created_at = created_at
         self.token_count = token_count
@@ -201,15 +209,15 @@
         message: Optional[Dict[str, Any]] = None,
         meta: Optional[
             Dict[str, Any]
         ] = None,  # Add the 'meta' argument with a default value
         score: Optional[float] = None,
         summary: Optional[str] = None,
         dist: Optional[float] = None,
-    ):
+    ) -> None:
         self.message = message
         self.meta = (
             meta if meta is not None else {}
         )  # Use the provided value or an empty dictionary
         self.score = score
         self.summary = summary
         self.dist = dist
```

### Comparing `zep_python-0.1.10/zep_python/zep_client.py` & `zep_python-0.2/zep_python/zep_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
 from types import TracebackType
 from typing import List, Optional, Type
 
 import httpx
 
-from exceptions import UnexpectedResponseError
-from models import Memory, SearchPayload, SearchResult
-from utils import sync
+from zep_python.exceptions import APIError, NotFoundError
+from zep_python.models import Memory, SearchPayload, SearchResult
+from zep_python.utils import sync
 
 API_BASEURL = "/api/v1"
 
 
 class ZepClient:
     """
     ZepClient class implementation.
@@ -27,15 +27,16 @@
     -------
     get_memory(session_id: str, lastn: Optional[int] = None) -> List[Memory]:
         Retrieve memory for the specified session.
     add_memory(session_id: str, memory_messages: Memory) -> str:
         Add memory to the specified session.
     delete_memory(session_id: str) -> str:
         Delete memory for the specified session.
-    search_memory(session_id: str, search_payload: SearchPayload, limit: Optional[int] = None) -> List[SearchResult]:
+    search_memory(session_id: str, search_payload: SearchPayload,
+                  limit: Optional[int] = None) -> List[SearchResult]:
         Search memory for the specified session.
     close() -> None:
         Close the HTTP client.
     """
 
     def __init__(self, base_url: str) -> None:
         """
@@ -59,33 +60,37 @@
         exc_type: Type[Exception],
         exc_val: Exception,
         exc_tb: TracebackType,
     ) -> None:
         await self.close()
 
     @sync
-    def get_memory(self, session_id: str, lastn: Optional[int] = None) -> List[Memory]:
+    def get_memory(
+        self, session_id: str, lastn: Optional[int] = None
+    ) -> List[Memory]:
         """
-        Retrieve memory for the specified session. This method is a synchronous wrapper for the asynchronous method `aget_memory`.
+        Retrieve memory for the specified session. This method is a synchronous wrapper
+        for the asynchronous method `aget_memory`.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which to retrieve memory.
         lastn : Optional[int], optional
-            The number of most recent memory entries to retrieve. Defaults to None (all entries).
+            The number of most recent memory entries to retrieve. Defaults to None (all
+            entries).
 
         Returns
         -------
         List[Memory]
             A list of Memory objects representing the retrieved memory entries.
 
         Raises
         ------
-        UnexpectedResponseError
+        APIError
             If the API response format is unexpected.
         """
         # we've wrapped the function in a decorator that will run it synchronously.
         # ignore the type error.
         return self.aget_memory(session_id, lastn)  # type: ignore
 
     async def aget_memory(
@@ -95,58 +100,63 @@
         Asynchronously retrieve memory for the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which to retrieve memory.
         lastn : Optional[int], optional
-            The number of most recent memory entries to retrieve. Defaults to None (all entries).
+            The number of most recent memory entries to retrieve. Defaults to None (all
+            entries).
 
         Returns
         -------
         List[Memory]
             A list of Memory objects representing the retrieved memory entries.
 
         Raises
         ------
-        UnexpectedResponseError
+        APIError
             If the API response format is unexpected.
         """
         url = f"{self.base_url}{API_BASEURL}/sessions/{session_id}/memory"
         params = (
             {"lastn": lastn} if lastn is not None else {}
         )  # Include 'lastn' as a query parameter if provided
         response = await self.client.get(url, params=params)
-        response_data = response.json()
+
+        if response.status_code == 404:
+            raise NotFoundError(f"No memory found for session {session_id}")
 
         if response.status_code != 200:
-            raise UnexpectedResponseError(
-                f"Unexpected status code: {response.status_code}"
-            )
+            raise APIError(f"Unexpected status code: {response.status_code}")
+
+        response_data = response.json()
 
         # Check if the response contains the expected field 'messages'.
         if "messages" in response_data:
             # If 'messages' is None, return an empty list.
             if response_data["messages"] is None:
                 return []
             # Create a Memory instance using the 'messages' field from the response.
             memory = Memory(
                 messages=response_data["messages"],
                 # Add the 'summary' field if it is present in the response.
                 summary=response_data.get("summary", None),
-                # Add any other fields from the response that are relevant to the Memory class.
+                # Add any other fields from the response that are relevant to the
+                # Memory class.
             )
             return [memory]
         else:
-            raise UnexpectedResponseError("Unexpected response format from the API")
+            raise APIError("Unexpected response format from the API")
 
     @sync
     def add_memory(self, session_id: str, memory_messages: Memory) -> str:
         """
-        Add memory to the specified session. This method is a synchronous wrapper for the asynchronous method `aadd_memory`.
+        Add memory to the specified session. This method is a synchronous wrapper for
+        the asynchronous method `aadd_memory`.
 
         Parameters
         ----------
         session_id : str
             The ID of the session to which memory should be added.
         memory_messages : Memory
             A Memory object representing the memory messages to be added.
@@ -154,22 +164,24 @@
         Returns
         -------
         str
             The response text from the API.
 
         Raises
         ------
-        UnexpectedResponseError
+        APIError
             If the API response format is unexpected.
         """
         # we've wrapped the function in a decorator that will run it synchronously.
         # ignore the type error.
         return self.aadd_memory(session_id, memory_messages)  # type: ignore
 
-    async def aadd_memory(self, session_id: str, memory_messages: Memory) -> str:
+    async def aadd_memory(
+        self, session_id: str, memory_messages: Memory
+    ) -> str:
         """
         Asynchronously add memory to the specified session.
 
         Parameters
         ----------
         session_id : str
             The ID of the session to which memory should be added.
@@ -179,46 +191,45 @@
         Returns
         -------
         str
             The response text from the API.
 
         Raises
         ------
-        UnexpectedResponseError
+        APIError
             If the API response format is unexpected.
         """
         response = await self.client.post(
             f"{self.base_url}{API_BASEURL}/sessions/{session_id}/memory",
             json=memory_messages.to_dict(),
         )
         if response.status_code != 200:
-            raise UnexpectedResponseError(
-                f"Unexpected status code: {response.status_code}"
-            )
+            raise APIError(f"Unexpected status code: {response.status_code}")
 
         return response.text
 
     @sync
     def delete_memory(self, session_id: str) -> str:
         """
-        Delete memory for the specified session. This method is a synchronous wrapper for the asynchronous method `adelete_memory`.
+        Delete memory for the specified session. This method is a synchronous wrapper
+        for the asynchronous method `adelete_memory`.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which memory should be deleted.
 
         Returns
         -------
         str
             The response text from the API.
 
         Raises
         ------
-        UnexpectedResponseError
+        APIError
             If the API response format is unexpected.
         """
         # we've wrapped the function in a decorator that will run it synchronously.
         # ignore the type error.
         return self.adelete_memory(session_id)  # type: ignore
 
     async def adelete_memory(self, session_id: str) -> str:
@@ -233,35 +244,37 @@
         Returns
         -------
         str
             The response text from the API.
 
         Raises
         ------
-        UnexpectedResponseError
+        APIError
             If the API response format is unexpected.
         """
         response = await self.client.delete(
             f"{self.base_url}{API_BASEURL}/sessions/{session_id}/memory"
         )
+        if response.status_code == 404:
+            raise NotFoundError(f"No session found for session {session_id}")
+
         if response.status_code != 200:
-            raise UnexpectedResponseError(
-                f"Unexpected status code: {response.status_code}"
-            )
+            raise APIError(f"Unexpected status code: {response.status_code}")
         return response.text
 
     @sync
     def search_memory(
         self,
         session_id: str,
         search_payload: SearchPayload,
         limit: Optional[int] = None,
     ) -> List[SearchResult]:
         """
-        Search memory for the specified session. This method is a synchronous wrapper for the asynchronous method `asearch_memory`.
+        Search memory for the specified session. This method is a synchronous wrapper
+        for the asynchronous method `asearch_memory`.
 
         Parameters
         ----------
         session_id : str
             The ID of the session for which memory should be searched.
         search_payload : SearchPayload
             A SearchPayload object representing the search query.
@@ -271,15 +284,15 @@
         Returns
         -------
         List[SearchResult]
             A list of SearchResult objects representing the search results.
 
         Raises
         ------
-        UnexpectedResponseError
+        APIError
             If the API response format is unexpected.
         """
         # we've wrapped the function in a decorator that will run it synchronously.
         # ignore the type error.
         return self.asearch_memory(session_id, search_payload, limit)  # type: ignore
 
     async def asearch_memory(
@@ -303,29 +316,30 @@
         Returns
         -------
         List[SearchResult]
             A list of SearchResult objects representing the search results.
 
         Raises
         ------
-        UnexpectedResponseError
+        APIError
             If the API response format is unexpected.
         """
         params = {"limit": limit} if limit is not None else {}
         response = await self.client.post(
             f"{self.base_url}{API_BASEURL}/sessions/{session_id}/search",
             json=search_payload.__dict__,
             params=params,
         )
         if response.status_code != 200:
-            raise UnexpectedResponseError(
-                f"Unexpected status code: {response.status_code}"
-            )
-        return [SearchResult(**search_result) for search_result in response.json()]
+            raise APIError(f"Unexpected status code: {response.status_code}")
+        return [
+            SearchResult(**search_result) for search_result in response.json()
+        ]
 
     async def close(self) -> None:
         """
         Asynchronously close the HTTP client.
 
-        [Optional] This method may be called when the ZepClient is no longer needed to release resources.
+        [Optional] This method may be called when the ZepClient is no longer needed to
+        release resources.
         """
         await self.client.aclose()
```

