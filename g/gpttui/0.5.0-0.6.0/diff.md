# Comparing `tmp/gpttui-0.5.0.tar.gz` & `tmp/gpttui-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpttui-0.5.0.tar", last modified: Mon Apr 24 21:41:15 2023, max compression
+gzip compressed data, was "gpttui-0.6.0.tar", last modified: Wed May 10 16:52:53 2023, max compression
```

## Comparing `gpttui-0.5.0.tar` & `gpttui-0.6.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      123 2023-04-07 23:28:42.202644 gpttui-0.5.0/.gitignore
--rw-r--r--   0        0        0      185 2023-04-24 20:21:25.237725 gpttui-0.5.0/Makefile
--rw-r--r--   0        0        0     2164 2023-04-21 22:33:55.636511 gpttui-0.5.0/README.md
--rw-r--r--   0        0        0   999692 2023-04-21 22:33:55.649844 gpttui-0.5.0/docs/img/example.gif
--rw-r--r--   0        0        0      594 2023-04-24 21:41:09.499816 gpttui-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/database/__init__.py
--rw-r--r--   0        0        0     2937 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/database/base.py
--rw-r--r--   0        0        0     4103 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/database/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/models/__init__.py
--rw-r--r--   0        0        0     2819 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/models/base.py
--rw-r--r--   0        0        0     3728 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/models/chatsonic.py
--rw-r--r--   0        0        0     4171 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/models/colossal.py
--rw-r--r--   0        0        0     3054 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/models/openai.py
--rw-r--r--   0        0        0        0 2023-04-11 01:50:25.100205 gpttui-0.5.0/src/gpttui/tui/__init__.py
--rw-r--r--   0        0        0     7384 2023-04-21 22:33:55.649844 gpttui-0.5.0/src/gpttui/tui/app.py
--rw-r--r--   0        0        0     3328 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/tui/config.py
--rw-r--r--   0        0        0     3004 2023-04-24 21:41:09.503150 gpttui-0.5.0/src/gpttui/tui/front.py
--rw-r--r--   0        0        0      210 2023-04-11 01:50:25.103539 gpttui-0.5.0/src/gpttui/tui/main.py
--rwxr-xr-x   0        0        0      140 2023-04-11 01:50:25.103539 gpttui-0.5.0/test/main.sh
--rw-r--r--   0        0        0     1983 2023-04-11 01:50:25.103539 gpttui-0.5.0/test/test_db.py
--rw-r--r--   0        0        0     1582 2023-04-11 01:50:25.103539 gpttui-0.5.0/test/test_model.py
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 gpttui-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      123 2023-04-14 21:25:28.979290 gpttui-0.6.0/.gitignore
+-rw-r--r--   0        0        0      176 2023-05-10 14:55:58.792046 gpttui-0.6.0/Makefile
+-rw-r--r--   0        0        0     5941 2023-05-10 16:51:37.160788 gpttui-0.6.0/README.md
+-rw-r--r--   0        0        0   999692 2023-05-10 16:51:37.177455 gpttui-0.6.0/docs/img/example.gif
+-rw-r--r--   0        0        0      549 2023-05-10 16:51:37.177455 gpttui-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-14 21:25:28.979290 gpttui-0.6.0/src/gpttui/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:25:28.979290 gpttui-0.6.0/src/gpttui/database/__init__.py
+-rw-r--r--   0        0        0     2947 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/database/base.py
+-rw-r--r--   0        0        0     4046 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/database/sqlite.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:25:28.979290 gpttui-0.6.0/src/gpttui/models/__init__.py
+-rw-r--r--   0        0        0     2822 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/models/base.py
+-rw-r--r--   0        0        0     3627 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/models/chatsonic.py
+-rw-r--r--   0        0        0     4111 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/models/colossal.py
+-rw-r--r--   0        0        0     2997 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/models/openai.py
+-rw-r--r--   0        0        0        0 2023-04-14 21:25:28.979290 gpttui-0.6.0/src/gpttui/tui/__init__.py
+-rw-r--r--   0        0        0     7462 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/tui/app.py
+-rw-r--r--   0        0        0     3139 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/tui/config.py
+-rw-r--r--   0        0        0     3203 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/tui/front.py
+-rw-r--r--   0        0        0     1478 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/tui/init.py
+-rw-r--r--   0        0        0      216 2023-05-10 16:51:37.177455 gpttui-0.6.0/src/gpttui/tui/main.py
+-rwxr-xr-x   0        0        0      140 2023-04-14 21:25:28.979290 gpttui-0.6.0/test/main.sh
+-rw-r--r--   0        0        0     1989 2023-05-10 16:51:37.177455 gpttui-0.6.0/test/test_db.py
+-rw-r--r--   0        0        0     1446 2023-05-10 16:51:37.177455 gpttui-0.6.0/test/test_model.py
+-rw-r--r--   0        0        0      473 1970-01-01 00:00:00.000000 gpttui-0.6.0/PKG-INFO
```

### Comparing `gpttui-0.5.0/docs/img/example.gif` & `gpttui-0.6.0/docs/img/example.gif`

 * *Files identical despite different names*

### Comparing `gpttui-0.5.0/src/gpttui/database/base.py` & `gpttui-0.6.0/src/gpttui/database/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,68 +3,78 @@
 """
 
 from abc import ABC, abstractmethod
 from typing import List, Any
 from pydantic import BaseModel
 from enum import Enum
 
+
 class DatabasesEnum(Enum):
     """
     Enum that specifies the supported databases.
     """
+
     SQLITE = "SQLITE"
 
+
 class Message(BaseModel):
     """
     Dataclass that contains a single message.
 
     Attributes
     ----------
     role : str
         Who wrote the message.
     content : str
         Message content.
     """
+
     role: str
     content: str
 
+
 class Messages(BaseModel):
     """
     Dataclass that represents multiple messages.
 
     Attributes
     ----------
     values : List[Message]
         List of messages.
     """
+
     values: List[Message]
 
+
 class MessageWithTime(BaseModel):
     """
     Dataclass that represents a message and its timestamp.
 
     Attributes
     ----------
     message : Message
         A message instance.
     timestamp : int
         Unix time.
     """
+
     message: Message
     timestamp: int
 
+
 class AbstractDB(ABC):
     """
     Abstract class that represents any compatible database.
 
     Attributes
     ----------
     connection : Any
         Connection with any database.
     """
+
     connection: Any
 
     @abstractmethod
     def setup(self, **kwargs: str) -> "AbstractDB":
         """
         This method must be used to setup the database. For instance, to add connection strings, clients, among others.
```

### Comparing `gpttui-0.5.0/src/gpttui/database/sqlite.py` & `gpttui-0.6.0/src/gpttui/database/sqlite.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 """
 This file defines the required elements to use sqlite as a database.
 """
 import sqlite3
 from gpttui.database.base import AbstractDB, MessageWithTime, Messages, Message
 from typing import Callable, List
 
+
 class SqliteDB(AbstractDB):
     """
     This class represents a database based on SQLITE.
 
     Attributes
     ----------
     connection : sqlite3.Connection
         Connection with a sqlite database.
     """
+
     connection: sqlite3.Connection
 
     def setup(self, **kwargs: str) -> "AbstractDB":
         """
         This method allows creating a connection with the database.
 
         Parameters
@@ -66,83 +68,83 @@
 
         Parameters
         ----------
         session_name : str
             Session name.
         """
         f = lambda cursor: cursor.execute(
-                f"""
+            f"""
                 CREATE TABLE IF NOT EXISTS {session_name}(
                     id INTEGER PRIMARY KEY AUTOINCREMENT,
                     role TEXT,
                     content TEXT,
                     timestamp INT
                     );
                 """
-                )
+        )
         self.__write_with_connection(f)
 
     def delete_session(self, session_name: str):
         """
         Deletes a session (table) in sqlite.
-        
+
         Parameters
         ----------
         session_name : str
             Session name.
         """
         f = lambda cursor: cursor.execute(
-                f"""
+            f"""
                 DROP TABLE {session_name};
                 """
-                )
+        )
         self.__write_with_connection(f)
 
     def add_message(self, msg: MessageWithTime, session_name: str):
         """
         Saves a message (row) in the database.
 
         Parameters
         ----------
         msg : MessageWithTime
             Message to store.
         session_name : str
             Session name.
         """
         f = lambda cursor: cursor.execute(
-                f"""
+            f"""
                 INSERT INTO {session_name} (
                     role, content, timestamp
                     )
                 VALUES (?, ?, ?);
                 """,
-                (msg.message.role, msg.message.content, msg.timestamp)
-                )
+            (msg.message.role, msg.message.content, msg.timestamp),
+        )
         self.__write_with_connection(f)
 
     def get_messages(self, session_name: str) -> Messages:
         """
         Extracts the most recent messages from the database.
 
         Parameters
         ----------
         session_name : str
             Session name.
         """
         f = lambda cursor: cursor.execute(
-                f"""
+            f"""
                 SELECT
                     role, content
                 FROM
                     {session_name}
                 ORDER BY
                     timestamp ASC
                 ;
                 """
-                )
+        )
         result = self.__read_with_connection(f)
         messages = Messages(values=[Message(role=x[0], content=x[1]) for x in result])
         return messages
 
     def close(self):
         """
         Closes the connection with the database.
```

### Comparing `gpttui-0.5.0/src/gpttui/models/base.py` & `gpttui-0.6.0/src/gpttui/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 """
 import time
 from abc import ABC, abstractmethod
 from pydantic import BaseModel
 from gpttui.database.base import AbstractDB, Messages, Message, MessageWithTime
 from enum import Enum
 
+
 class ModelsEnum(Enum):
     """
     This enum defines the available models.
     """
+
     OPENAI = "OPENAI"
     CHATSONIC = "CHATSONIC"
     COLOSSAL = "COLOSSAL"
 
+
 class AbstractModel(ABC):
     """
     This abstract class defines any generative model.
 
     Attributes
     ----------
     model_name : str
@@ -26,14 +29,15 @@
     session_name : str
         Session name.
     context : str
         Context given to the model.
     database : AbstractDB
         Database to store the messages.
     """
+
     config: BaseModel
     session_name: str
     context: str
     database: AbstractDB
 
     def add_context(self, context: str) -> "AbstractModel":
         """
@@ -61,23 +65,25 @@
         Messages
             Most recent messages.
         """
         self.database.create_session(session_name=self.session_name)
         last_msgs = self.database.get_messages(session_name=self.session_name)
         if not len(last_msgs.values):
             msg = MessageWithTime(
-                    message=Message(role="system", content=self.context),
-                    timestamp=int(time.time())
-                    )
+                message=Message(role="system", content=self.context),
+                timestamp=int(time.time()),
+            )
             self.database.add_message(msg=msg, session_name=self.session_name)
             return self.last_messages()
         return last_msgs
 
     @abstractmethod
-    def setup(self, config: BaseModel, session_name: str, database: AbstractDB) -> "AbstractModel":
+    def setup(
+        self, config: BaseModel, session_name: str, database: AbstractDB
+    ) -> "AbstractModel":
         """
         This method is used to setup any model.
 
         Parameters
         ----------
         config : BaseModel
             Dataclass with the model's config options.
```

### Comparing `gpttui-0.5.0/src/gpttui/models/chatsonic.py` & `gpttui-0.6.0/src/gpttui/models/chatsonic.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,39 +2,49 @@
 This module contains the integration with ChatSonic.
 """
 import time
 from typing import List
 from pydantic import BaseModel
 from gpttui.models.base import AbstractModel
 from gpttui.database.base import Messages, Message, MessageWithTime, AbstractDB
+
 try:
     import httpx
 except ImportError:
-    raise ImportError("Could not import chatsonic dependencies, please install it with:\n\tpip install gpttui[chatsonic]")
+    raise ImportError(
+        "Could not import chatsonic dependencies, please install it with:\n\tpip install gpttui[chatsonic]"
+    )
+
 
 class ChatSonicConf(BaseModel):
-    url : str = "https://api.writesonic.com/v2/business/content/chatsonic?engine=premium"
-    api_key : str = ""
+    url: str = "https://api.writesonic.com/v2/business/content/chatsonic?engine=premium"
+    api_key: str = ""
     enable_memory: bool = True
     enable_google_results: bool = True
 
+
 class ChatSonicMessage(BaseModel):
-    is_sent : bool
-    message : str
+    is_sent: bool
+    message: str
+
 
 class ChatSonicMessages(BaseModel):
-    values : List[ChatSonicMessage]
+    values: List[ChatSonicMessage]
+
 
 class ChatSonicModel(AbstractModel):
     """
     This class allows loading and interacting with any openai model through its API.
     """
-    config : ChatSonicConf
 
-    def setup(self, config: ChatSonicConf, session_name: str, database: AbstractDB) -> "ChatSonicModel":
+    config: ChatSonicConf
+
+    def setup(
+        self, config: ChatSonicConf, session_name: str, database: AbstractDB
+    ) -> "ChatSonicModel":
         """
         Initializes the model and collects credentials for OpenAI.
 
         Parameters
         ----------
         url : str
             Chatsonic URL.
@@ -59,23 +69,21 @@
         msgs : Messages
             Input messages.
 
         Returns
         -------
         ChatSonicMessages
             Parsed messages.
-        """ 
+        """
         parsed_msgs = []
         for msg in msgs.values:
             if msg.role not in ["assistant", "user"]:
                 continue
             is_sent = msg.role == "user"
-            parsed_msgs.append(
-                    ChatSonicMessage(is_sent=is_sent, message=msg.content)
-                    )
+            parsed_msgs.append(ChatSonicMessage(is_sent=is_sent, message=msg.content))
         return ChatSonicMessages(values=parsed_msgs)
 
     async def get_answer(self, message: str) -> str:
         """
         Obtains an answer form any message.
 
         Parameters
@@ -86,33 +94,32 @@
         Returns
         -------
         str
             Generated response.
         """
         last_msgs = self.last_messages()
         new_msg = MessageWithTime(
-                message=Message(role="user", content=message),
-                timestamp=int(time.time())
-                )
+            message=Message(role="user", content=message), timestamp=int(time.time())
+        )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         last_msgs = self.last_messages()
         payload = {
-                "enable_memory": self.config.enable_memory,
-                "enable_google_results": self.config.enable_google_results,
-                "input_text": self.context,
-                "history_data": ChatSonicModel.parse_messages(last_msgs).dict()["values"]
-                } 
+            "enable_memory": self.config.enable_memory,
+            "enable_google_results": self.config.enable_google_results,
+            "input_text": self.context,
+            "history_data": ChatSonicModel.parse_messages(last_msgs).dict()["values"],
+        }
         headers = {
-                "accept": "application/json",
-                "content-type": "application/json",
-                "X-API-KEY": self.config.api_key
-                }
+            "accept": "application/json",
+            "content-type": "application/json",
+            "X-API-KEY": self.config.api_key,
+        }
         async with httpx.AsyncClient() as client:
             r = await client.post(self.config.url, json=payload, headers=headers)
             response = r.json()["message"]
 
         new_msg = MessageWithTime(
-                message=Message(role="assistant", content=response),
-                timestamp=int(time.time())
-                )
+            message=Message(role="assistant", content=response),
+            timestamp=int(time.time()),
+        )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         return response
```

### Comparing `gpttui-0.5.0/src/gpttui/models/colossal.py` & `gpttui-0.6.0/src/gpttui/models/colossal.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,51 +2,64 @@
 This module contains the integration with ChatSonic.
 """
 import time
 from typing import List
 from pydantic import BaseModel
 from gpttui.models.base import AbstractModel
 from gpttui.database.base import Messages, Message, MessageWithTime, AbstractDB
+
 try:
     import httpx, ssl
 except ImportError:
-    raise ImportError("Could not import colossal dependencies, please install it with:\n\tpip install gpttui[colossal]")
+    raise ImportError(
+        "Could not import colossal dependencies, please install it with:\n\tpip install gpttui[colossal]"
+    )
+
 
 class ColossalConf(BaseModel):
     """
     Dataclass with the config for the colossal model.
     """
-    url : str = "https://service.colossalai.org/generate"
+
+    url: str = "https://service.colossalai.org/generate"
     repetition_penalty: float = 1.2
-    top_k : int = 40
-    top_p : float = 0.5
-    temperature : float = 0.7
-    max_new_tokens : int = 512
+    top_k: int = 40
+    top_p: float = 0.5
+    temperature: float = 0.7
+    max_new_tokens: int = 512
     timeout: float = 30
 
+
 class ColossalMessage(BaseModel):
     """
     Represents a single message.
     """
-    instruction : str
-    response : str
+
+    instruction: str
+    response: str
+
 
 class ColossalMessages(BaseModel):
     """
     Represents the history of messages.
     """
-    values : List[ColossalMessage]
+
+    values: List[ColossalMessage]
+
 
 class ColossalModel(AbstractModel):
     """
     This class allows loading and interacting with colossal model.
     """
-    config : ColossalConf
 
-    def setup(self, config: ColossalConf, session_name: str, database: AbstractDB) -> "ColossalModel":
+    config: ColossalConf
+
+    def setup(
+        self, config: ColossalConf, session_name: str, database: AbstractDB
+    ) -> "ColossalModel":
         """
         Initializes the model.
 
         Parameters
         ----------
         config : ColossalConf
             Configuration options.
@@ -75,22 +88,22 @@
         msgs : Messages
             Input messages.
 
         Returns
         -------
         ChatSonicMessages
             Parsed messages.
-        """ 
+        """
         parsed_msgs = []
         user = filter(lambda x: x.role == "user", msgs.values)
         assistant = filter(lambda x: x.role == "assistant", msgs.values)
         for umsg, amsg in zip(user, assistant):
             parsed_msgs.append(
-                    ColossalMessage(instruction=umsg.content, response=amsg.content)
-                    )
+                ColossalMessage(instruction=umsg.content, response=amsg.content)
+            )
         return ColossalMessages(values=parsed_msgs)
 
     async def get_answer(self, message: str) -> str:
         """
         Obtains an answer form any message.
 
         Parameters
@@ -101,34 +114,33 @@
         Returns
         -------
         str
             Generated response.
         """
         last_msgs = self.last_messages()
         new_msg = MessageWithTime(
-                message=Message(role="user", content=message),
-                timestamp=int(time.time())
-                )
+            message=Message(role="user", content=message), timestamp=int(time.time())
+        )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         last_msgs = self.last_messages()
         history = ColossalModel.parse_messages(last_msgs)
         history.values.append(ColossalMessage(instruction=message, response=""))
         payload = {
-                "repetition_penalty": self.config.repetition_penalty,
-                "top_k": self.config.top_k,
-                "top_p": self.config.top_p,
-                "temperature": self.config.temperature,
-                "max_new_tokens": self.config.max_new_tokens,
-                "history": history.dict()["values"]
-                } 
+            "repetition_penalty": self.config.repetition_penalty,
+            "top_k": self.config.top_k,
+            "top_p": self.config.top_p,
+            "temperature": self.config.temperature,
+            "max_new_tokens": self.config.max_new_tokens,
+            "history": history.dict()["values"],
+        }
         context = ssl._create_unverified_context()
         timeout = httpx.Timeout(self.config.timeout)
         async with httpx.AsyncClient(verify=context, timeout=timeout) as client:
             r = await client.post(self.config.url, json=payload)
             response = r.text
 
         new_msg = MessageWithTime(
-                message=Message(role="assistant", content=response),
-                timestamp=int(time.time())
-                )
+            message=Message(role="assistant", content=response),
+            timestamp=int(time.time()),
+        )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         return response
```

### Comparing `gpttui-0.5.0/src/gpttui/models/openai.py` & `gpttui-0.6.0/src/gpttui/models/openai.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 """
 This module contains the integration with OpenAI models.
 """
 try:
     import openai, time
     from openai.error import Timeout
 except ImportError:
-    raise ImportError("Could not import openai library, please install it with:\n\tpip install gpttui[openai]")
+    raise ImportError(
+        "Could not import openai library, please install it with:\n\tpip install gpttui[openai]"
+    )
 from pydantic import BaseModel
 from gpttui.models.base import AbstractModel
 from gpttui.database.base import AbstractDB, Message, MessageWithTime
 
+
 class OpenAIConf(BaseModel):
     """
     Dataclass to setup OpenAI models.
     """
-    timeout : int = 30
-    max_retries : int = 3
-    model_name : str = "gpt-3.5-turbo"
-    organization : str = ""
-    api_key : str = ""
+
+    timeout: int = 30
+    max_retries: int = 3
+    model_name: str = "gpt-3.5-turbo"
+    organization: str = ""
+    api_key: str = ""
+
 
 class OpenAIModel(AbstractModel):
     """
     This class allows loading and interacting with any openai model through its API.
     """
-    config : OpenAIConf
 
-    def setup(self, config: OpenAIConf, session_name: str, database: AbstractDB) -> "OpenAIModel":
+    config: OpenAIConf
+
+    def setup(
+        self, config: OpenAIConf, session_name: str, database: AbstractDB
+    ) -> "OpenAIModel":
         """
         Initializes the model and collects credentials for OpenAI.
 
         Parameters
         ----------
         model_name : str
             Model name.
@@ -63,32 +71,31 @@
         Returns
         -------
         str
             Generated response.
         """
         last_msgs = self.last_messages()
         new_msg = MessageWithTime(
-                message=Message(role="user", content=message),
-                timestamp=int(time.time())
-                )
+            message=Message(role="user", content=message), timestamp=int(time.time())
+        )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         last_msgs = self.last_messages()
         response = ""
         retries = 0
         while not response and retries < self.config.max_retries:
             try:
                 response = await openai.ChatCompletion.acreate(
-                            model = self.config.model_name,
-                            messages = last_msgs.dict()["values"],
-                            request_timeout = self.config.timeout
-                            )
+                    model=self.config.model_name,
+                    messages=last_msgs.dict()["values"],
+                    request_timeout=self.config.timeout,
+                )
             except Timeout:
                 retries += 1
         if retries == self.config.max_retries:
             raise Timeout("Maximum number of retries achieved.")
-        response = str(response.choices[0].message.content) # type: ignore
+        response = str(response.choices[0].message.content)  # type: ignore
         new_msg = MessageWithTime(
-                message=Message(role="assistant", content=response),
-                timestamp=int(time.time())
-                )
+            message=Message(role="assistant", content=response),
+            timestamp=int(time.time()),
+        )
         self.database.add_message(msg=new_msg, session_name=self.session_name)
         return response
```

### Comparing `gpttui-0.5.0/src/gpttui/tui/app.py` & `gpttui-0.6.0/src/gpttui/tui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,75 +1,87 @@
 """
 This file defines the main TUI App.
 """
-import os, re
 import pyperclip
 from pathlib import Path
 from enum import Enum, auto
-from typing import Any
+from typing import Any, Type
 from textual.app import App, ComposeResult
 from textual.widgets import Input, Markdown, Static
 from textual.containers import Container
 from textual.events import Key
 from gpttui.models.base import AbstractModel
-from gpttui.tui.config import KeyBindings, keybindings_config
+from gpttui.tui.config import KeyBindings
+
 
 class ModeEnum(Enum):
     """
     This enum represents the possible modes of the application.
     """
+
     INSERT = auto()
     NORMAL = auto()
 
+
 class NormalIndicator(Static):
     """
     Static container for the normal mode.
     """
+
     ...
 
+
 class InsertIndicator(Static):
     """
     Static container for the insert mode.
     """
+
     ...
 
+
 class UserInput(Input):
     """
     Represents the text input.
     """
+
     ...
 
+
 class Prompt(Static):
     """
     The prompt contains the mode indicators and the text input.
     """
+
     def compose(self) -> ComposeResult:
         yield NormalIndicator("NORMAL", id="normal-indicator")
         yield InsertIndicator("INSERT", id="insert-indicator")
         yield Input(placeholder="Enter some text...")
 
+
 class UserText(Static):
     """
     Static container to display the sender.
     """
+
     ...
 
+
 class Message(Static):
     """
     A message contains the the sender and its text.
 
     Parameters
     ----------
     user : str
         Sender.
     message : str
         Text of the message.
     """
 
-    def __init__(self, user:str, message: str, *args: Any, **kwargs: Any):
+    def __init__(self, user: str, message: str, *args: Any, **kwargs: Any):
         super(Message, self).__init__(*args, **kwargs)
         self.user = user
         self.message = message
 
     def compose(self) -> ComposeResult:
         """
         Generator with the message components.
@@ -85,14 +97,15 @@
         try:
             md = Markdown()
             md.update(self.message)
         except:
             md = Static(self.message)
         yield md
 
+
 class Messages(Container):
     """
     A container that stores all messages.
     """
 
     def add_message(self, msg: str, user: str):
         """
@@ -104,14 +117,15 @@
             Message to display.
         user : str
             Sender of the message.
         """
         self.mount(Message(user=user, message=msg))
         self.scroll_end()
 
+
 class GptApp(App):
     """
     This class defines the TUI App.
 
     Parameters
     ----------
     CSS_PATH : Path
@@ -125,33 +139,40 @@
     chat_text : str
         Visible text that is show in the chat.
     normal_commands : str
         Mapping between a keybinding and its function in normal mode.
     insert_commands : str
         Mapping between a keybinding and its function in insert mode.
     """
-    CSS_PATH : Path = Path(os.environ["HOME"]) / ".config/gpttui/style.css"
-    KEYBINDINGS : KeyBindings = keybindings_config()
+
+    CSS_PATH: Path
+    KEYBINDINGS: KeyBindings
     model: AbstractModel
 
     def __init__(self, *args: Any, **kwargs: Any):
         super(GptApp, self).__init__(*args, **kwargs)
         self.mode = ModeEnum.NORMAL
         self.normal_commands = {
-                self.KEYBINDINGS.insert: self.insert,
-                self.KEYBINDINGS.quit: self.quit,
-                self.KEYBINDINGS.yank: self.yank,
-                self.KEYBINDINGS.paste: self.paste,
-                self.KEYBINDINGS.clear: self.clear,
-                self.KEYBINDINGS.delete: self.delete
-                }
+            self.KEYBINDINGS.insert: self.insert,
+            self.KEYBINDINGS.quit: self.quit,
+            self.KEYBINDINGS.yank: self.yank,
+            self.KEYBINDINGS.paste: self.paste,
+            self.KEYBINDINGS.clear: self.clear,
+            self.KEYBINDINGS.delete: self.delete,
+        }
         self.insert_commands = {
-                self.KEYBINDINGS.normal: self.normal,
-                self.KEYBINDINGS.send: self.send,
-                }
+            self.KEYBINDINGS.normal: self.normal,
+            self.KEYBINDINGS.send: self.send,
+        }
+
+    @classmethod
+    def setup_cls(cls, css_path: Path, keybindings: KeyBindings) -> Type["GptApp"]:
+        cls.CSS_PATH = css_path
+        cls.KEYBINDINGS = keybindings
+        return cls
 
     def setup(self, model: AbstractModel) -> "GptApp":
         """
         Setups the App.
 
         Parameters
         ----------
@@ -198,41 +219,43 @@
 
         Parameters
         ----------
         event : Key
             Event related to the key that was pressed.
         """
         f = self.normal_commands.get(event.key)
-        if f is not None: await f()
+        if f is not None:
+            await f()
 
     async def handle_insert(self, event: Key) -> None:
         """
         Determines what to do in insert mode.
 
         Parameters
         ----------
         event : Key
             Event related to the key that was pressed.
         """
         f = self.insert_commands.get(event.key)
-        if f is not None: await f()
+        if f is not None:
+            await f()
 
     async def insert(self):
         """
         Changes to insert mode.
         """
         self.add_class("insert-mode")
         self.query_one(Input).focus()
         self.mode = ModeEnum.INSERT
 
     async def clear(self):
         """
         Clears the historical messages.
         """
-        self.query_one(Messages) #TODO
+        self.query_one(Messages)  # TODO
 
     async def yank(self):
         """
         Copies the last message into the clipboard.
         """
         msgs = self.model.database.get_messages(self.model.session_name)
         pyperclip.copy(msgs.values[-1].content)
```

### Comparing `gpttui-0.5.0/src/gpttui/tui/config.py` & `gpttui-0.6.0/src/gpttui/tui/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 """
 This file defines the main configuration options for the TUI.
 """
-import os
 from pathlib import Path
 from pydantic import BaseModel
-from typing import TypeVar, Type
-from gpttui.models.chatsonic import ChatSonicConf
-from gpttui.models.colossal import ColossalConf
-from gpttui.models.openai import OpenAIConf
+from typing import Type
 
 __CSS_CONFIG = """
 Prompt {
     dock: bottom;
     layout: horizontal;
     padding: 0;
     margin: 0;
@@ -76,41 +72,43 @@
     dock: right;
     width: 94%;
     padding: 0 0 0 1;
     margin: 0;
 }
 """
 
+
 class KeyBindings(BaseModel):
     """
     Dataclass that represents the possible keybindings.
     """
+
     insert: str
     normal: str
     yank: str
     paste: str
     clear: str
     quit: str
     send: str
     delete: str
 
-def config_folder() -> Path:
+
+def config_folder(config_path: Path) -> Path:
     """
     Setups the config folder and returns its path.
 
     Returns
     -------
     Path
         Configuration path.
     """
-    home_path = os.environ["HOME"]
-    cfg_path = Path(os.path.join(home_path, ".config/gpttui"))
-    if not cfg_path.exists():
-        cfg_path.mkdir()
-    return cfg_path
+    if not config_path.exists():
+        config_path.mkdir()
+    return config_path
+
 
 def config_file(path: Path, type: Type[BaseModel]) -> BaseModel:
     """
     Setups the config file given any configuration type.
 
     Parameters
     ----------
@@ -128,40 +126,43 @@
         obj = type()
         with open(path, "w") as f:
             f.write(obj.json())
     else:
         obj = type.parse_file(path)
     return obj
 
-def css_config():
+
+def css_config(config_path: Path) -> Path:
     """
     Initializes the CSS configuration file.
     """
-    cfg_path = config_folder()
+    cfg_path = config_folder(config_path)
     filename = cfg_path / "style.css"
     if not filename.exists():
         with open(filename, "w") as f:
             f.write(__CSS_CONFIG)
+    return filename
+
 
-def keybindings_config() -> KeyBindings:
+def keybindings_config(config_path) -> KeyBindings:
     """
     Initializes the keybindings.
     """
-    cfg_path = config_folder()
+    cfg_path = config_folder(config_path)
     filename = cfg_path / "keybindings.json"
     if not filename.exists():
         filename.touch()
         keybindings = KeyBindings(
-                insert="i",
-                normal="escape",
-                yank="y",
-                paste="p",
-                clear="c",
-                quit="q",
-                send="enter",
-                delete="d",
-                )
+            insert="i",
+            normal="escape",
+            yank="y",
+            paste="p",
+            clear="c",
+            quit="q",
+            send="enter",
+            delete="d",
+        )
         with open(filename, "w") as f:
             f.write(keybindings.json())
     else:
         keybindings = KeyBindings.parse_file(filename)
     return keybindings
```

### Comparing `gpttui-0.5.0/src/gpttui/tui/front.py` & `gpttui-0.6.0/src/gpttui/tui/front.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,76 +8,74 @@
 from gpttui.database.base import AbstractDB, DatabasesEnum
 from gpttui.database.sqlite import SqliteDB
 from gpttui.models.base import AbstractModel, ModelsEnum
 from gpttui.models.chatsonic import ChatSonicConf, ChatSonicModel
 from gpttui.models.colossal import ColossalConf, ColossalModel
 from gpttui.models.openai import OpenAIModel, OpenAIConf
 from gpttui.tui.app import GptApp
-from gpttui.tui.config import config_file
+from gpttui.tui.config import config_file, css_config, keybindings_config
 from typing import Dict, Type
 
-DBS: Dict[DatabasesEnum, Type[AbstractDB]] = {
-        DatabasesEnum.SQLITE: SqliteDB
-        }
+DBS: Dict[DatabasesEnum, Type[AbstractDB]] = {DatabasesEnum.SQLITE: SqliteDB}
 MODELS: Dict[ModelsEnum, Type[AbstractModel]] = {
-        ModelsEnum.OPENAI: OpenAIModel,
-        ModelsEnum.CHATSONIC: ChatSonicModel,
-        ModelsEnum.COLOSSAL: ColossalModel
-        }
+    ModelsEnum.OPENAI: OpenAIModel,
+    ModelsEnum.CHATSONIC: ChatSonicModel,
+    ModelsEnum.COLOSSAL: ColossalModel,
+}
 CONFS: Dict[ModelsEnum, Type[BaseModel]] = {
-        ModelsEnum.OPENAI: OpenAIConf,
-        ModelsEnum.CHATSONIC: ChatSonicConf,
-        ModelsEnum.COLOSSAL: ColossalConf
-        }
+    ModelsEnum.OPENAI: OpenAIConf,
+    ModelsEnum.CHATSONIC: ChatSonicConf,
+    ModelsEnum.COLOSSAL: ColossalConf,
+}
+
 
 @command()
 @option(
     "--database_kind",
     type=DatabasesEnum,
     default=DatabasesEnum.SQLITE,
-    help="Database to store the messages."
-    )
+    help="Database to store the messages.",
+)
 @option(
     "--database_name",
     type=str,
-    default=Path(os.environ["HOME"]) / ".config/gpttui/database.sqlite",
-    help="Connection string for the database."
-    )
-@option(
-    "--session",
-    type=str,
-    default="default_session",
-    help="Session (chat) to use."
-    )
+    default="database.sqlite",
+    help="Connection string for the database.",
+)
+@option("--session", type=str, default="default_session", help="Session (chat) to use.")
 @option(
     "--model_kind",
     type=ModelsEnum,
     default=ModelsEnum.OPENAI,
-    help="Which model to use."
-    )
+    help="Which model to use.",
+)
 @option(
     "--context",
     type=str,
     default="You are an AI assistant",
-    help="Context for the model."
-    )
+    help="Context for the model.",
+)
 @option(
-    "--config",
+    "--config_path",
     type=Path,
-    default=Path(os.environ["HOME"]) / ".config/gpttui/openai.json",
-    help="Context for the model."
-    )
+    default=Path(os.environ["HOME"]) / ".config/gpttui",
+    help="Folder to save gpttui data.",
+)
+@option(
+    "--model_config", type=str, default="openai.json", help="Context for the model."
+)
 def front(
     database_kind: DatabasesEnum,
     database_name: str,
     session: str,
     model_kind: ModelsEnum,
     context: str,
-    config: Path
-    ) -> None:
+    config_path: Path,
+    model_config: str,
+) -> None:
     """
     Determines what to do when the front subcommand is launched.
 
     Parameters
     ----------
     database_kind : DatabasesEnum
         Which database to use.
@@ -87,27 +85,27 @@
         Session name.
     model_kind : ModelsEnum
         Which model to use.
     model_name : str
         Model name.
     context : str
         Context for the model.
-    config : Path
-        Configuration file.
+    config_folder : Path
+        Folder to save gpttui data.
+    model_config : str
+        Json file with the model's configuration.
     """
-    db = (
-            DBS[database_kind]()
-            .setup(database=database_name)
-            )
+    css_path = css_config(config_path)
+    keybindings = keybindings_config(config_path)
+    db = DBS[database_kind]().setup(database=str(config_path / database_name))
     db.create_session(session_name=session)
-    cfg = config_file(config, CONFS[model_kind])
+    cfg = config_file(config_path / model_config, CONFS[model_kind])
 
     model = (
-            MODELS[model_kind]()
-            .add_context(context=context)
-            .setup(config=cfg, database=db, session_name=session)
-            )
-    app = (
-            GptApp()
-            .setup(model=model)
-            )
+        MODELS[model_kind]()
+        .add_context(context=context)
+        .setup(config=cfg, database=db, session_name=session)
+    )
+    app = GptApp.setup_cls(css_path=css_path, keybindings=keybindings)().setup(
+        model=model
+    )
     app.run()
```

### Comparing `gpttui-0.5.0/test/test_db.py` & `gpttui-0.6.0/test/test_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Tests for the databases integration.
 """
 import pytest, time
 from gpttui.database.sqlite import SqliteDB
 from gpttui.database.base import AbstractDB, Message, MessageWithTime
 
+
 class TestSqliteDB:
     """
     Unittests for the sqlite database.
     """
+
     @staticmethod
     def setup_db() -> AbstractDB:
         """
         Initializes the database.
 
         Returns
         -------
@@ -32,22 +34,22 @@
         session_name : str
             Session name.
         """
         db = TestSqliteDB.setup_db()
         db.create_session(session_name)
         cursor = db.connection.cursor()
         cursor.execute("SELECT name FROM sqlite_schema;")
-        *result, = map(lambda i: i[0], cursor.fetchall())
+        (*result,) = map(lambda i: i[0], cursor.fetchall())
         assert session_name in result
 
         db.delete_session(session_name)
 
         cursor = db.connection.cursor()
         cursor.execute("SELECT name FROM sqlite_schema;")
-        *result, = map(lambda i: i[0], cursor.fetchall())
+        (*result,) = map(lambda i: i[0], cursor.fetchall())
         assert session_name not in result
 
     @pytest.mark.parametrize("message", ["hello", "testing", "hi"])
     def test_message(self, message: str):
         """
         Tests the save and retrieval of messages.
```

### Comparing `gpttui-0.5.0/test/test_model.py` & `gpttui-0.6.0/test/test_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,53 +4,48 @@
 import pytest
 from gpttui.database.base import AbstractDB
 from gpttui.models.base import AbstractModel
 from gpttui.models.openai import OpenAIModel
 from gpttui.database.sqlite import SqliteDB
 from typing import Tuple
 
+
 class TestOpenAi:
     """
     Tests that are used for any OpenAI model.
     """
+
     @staticmethod
     def setup_model() -> Tuple[AbstractDB, AbstractModel]:
         """
         Initialize the model and the database.
 
         Returns
         -------
         Tuple[AbstractDB, AbstractModel]
             Initialized database and model.
         """
-        db = (
-                SqliteDB()
-                .setup(database="test.db")
-                )
+        db = SqliteDB().setup(database="test.db")
         model = (
-                OpenAIModel()
-                .add_context(context="You're an expert programmer")
-                .setup(model_name="gpt-3.5-turbo", database=db, session_name="test")
-                )
+            OpenAIModel()
+            .add_context(context="You're an expert programmer")
+            .setup(model_name="gpt-3.5-turbo", database=db, session_name="test")
+        )
         return db, model
 
-    @pytest.mark.parametrize("message", [
-        "Is Python better than JS?",
-        "How to write hello word in Python?"
-        ])
+    @pytest.mark.parametrize(
+        "message", ["Is Python better than JS?", "How to write hello word in Python?"]
+    )
     def test_generation(self, message: str):
         """
         Tests the generation from the models.
 
         Parameters
         ----------
         message : str
             Input message.
         """
-        db, model = (
-                TestOpenAi
-                .setup_model()
-                )
+        db, model = TestOpenAi.setup_model()
         db.create_session(session_name="test")
         answer = model.get_answer(message)
         db.delete_session(session_name="test")
         assert isinstance(answer, str)
```

