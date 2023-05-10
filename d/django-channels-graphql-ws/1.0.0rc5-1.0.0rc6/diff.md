# Comparing `tmp/django_channels_graphql_ws-1.0.0rc5.tar.gz` & `tmp/django_channels_graphql_ws-1.0.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_channels_graphql_ws-1.0.0rc5.tar", max compression
+gzip compressed data, was "django_channels_graphql_ws-1.0.0rc6.tar", max compression
```

## Comparing `django_channels_graphql_ws-1.0.0rc5.tar` & `django_channels_graphql_ws-1.0.0rc6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-05-02 12:50:55.308791 django_channels_graphql_ws-1.0.0rc5/LICENSE
--rw-r--r--   0        0        0     1433 2023-05-02 12:50:55.309416 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/__init__.py
--rw-r--r--   0        0        0    10108 2023-05-05 11:21:54.816821 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/client.py
--rw-r--r--   0        0        0     2637 2023-05-02 12:50:55.310121 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/dict_as_object.py
--rw-r--r--   0        0        0    51298 2023-05-05 10:28:17.582938 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/graphql_ws_consumer.py
--rw-r--r--   0        0        0     3850 2023-05-02 12:50:55.310854 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/serializer.py
--rw-r--r--   0        0        0    16185 2023-05-05 10:28:17.583453 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/subscription.py
--rw-r--r--   0        0        0     4883 2023-05-05 12:36:22.593202 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/testing.py
--rw-r--r--   0        0        0     6939 2023-05-02 12:50:55.311889 django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/transport.py
--rw-r--r--   0        0        0     8470 2023-05-05 12:44:54.296330 django_channels_graphql_ws-1.0.0rc5/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-02 12:50:55.308791 django_channels_graphql_ws-1.0.0rc6/LICENSE
+-rw-r--r--   0        0        0     1433 2023-05-02 12:50:55.309416 django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/__init__.py
+-rw-r--r--   0        0        0    10108 2023-05-05 11:21:54.816821 django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/client.py
+-rw-r--r--   0        0        0     2637 2023-05-02 12:50:55.310121 django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/dict_as_object.py
+-rw-r--r--   0        0        0    51368 2023-05-10 09:43:00.753596 django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/graphql_ws_consumer.py
+-rw-r--r--   0        0        0     3850 2023-05-02 12:50:55.310854 django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/serializer.py
+-rw-r--r--   0        0        0    16209 2023-05-10 09:43:00.754112 django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/subscription.py
+-rw-r--r--   0        0        0     4883 2023-05-05 12:36:22.593202 django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/testing.py
+-rw-r--r--   0        0        0     6939 2023-05-02 12:50:55.311889 django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/transport.py
+-rw-r--r--   0        0        0     8470 2023-05-10 09:43:00.754681 django_channels_graphql_ws-1.0.0rc6/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 django_channels_graphql_ws-1.0.0rc6/PKG-INFO
```

### Comparing `django_channels_graphql_ws-1.0.0rc5/LICENSE` & `django_channels_graphql_ws-1.0.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/__init__.py` & `django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/__init__.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/client.py` & `django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/client.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/dict_as_object.py` & `django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/dict_as_object.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/graphql_ws_consumer.py` & `django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/graphql_ws_consumer.py`

 * *Files 1% similar despite different names*

```diff
@@ -731,15 +731,15 @@
             Tuple with three optional fields:
                 0: AST of parsed GraphQL document.
                 1: GraphQL operation definition.
                 2: Sequence of errors.
         """
 
         res = await channels.db.database_sync_to_async(
-            self._on_gql_start__parse_query_sync_cached
+            self._on_gql_start__parse_query_sync_cached, thread_sensitive=False
         )(op_name, query)
 
         doc_ast: Optional[graphql.DocumentNode] = res[0]
         op_ast: Optional[graphql.OperationDefinitionNode] = res[1]
         errors: Optional[Iterable[graphql.GraphQLError]] = res[2]
 
         return (doc_ast, op_ast, errors)
@@ -990,15 +990,17 @@
             sid=operation_id,
             unsubscribed_callback=unsubscribed_callback,
             enqueue_notification=enqueue_notification,
         )
         if waitlist:
             await asyncio.wait(waitlist)
 
-        _deserialize = channels.db.database_sync_to_async(Serializer.deserialize)
+        _deserialize = channels.db.database_sync_to_async(
+            Serializer.deserialize, thread_sensitive=False
+        )
 
         # For each notification (event) yielded from this function the
         # `_on_gql_start__subscribe` function will call subscription
         # resolver (`publish`) via `graphql.execute` method.
         while True:
             with notification_queue_lock:
                 payload = await notification_queue.get()
```

### Comparing `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/serializer.py` & `django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/serializer.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/subscription.py` & `django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/subscription.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
     @classmethod
     async def broadcast_async(cls, *, group=None, payload=None):
         """Broadcast, asynchronous version."""
         # Manually serialize the `payload` to allow transfer of Django
         # models inside `payload`, auto serialization does not do this.
         serialized_payload = await channels.db.database_sync_to_async(
-            Serializer.serialize
+            Serializer.serialize, thread_sensitive=False
         )(payload)
 
         # Send the message to the Channels group.
         group = cls._group_name(group)
         group_send = cls._channel_layer().group_send
         # Will result in a call of `GraphqlWsConsumer.broadcast`.
         await group_send(
```

### Comparing `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/testing.py` & `django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/testing.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc5/channels_graphql_ws/transport.py` & `django_channels_graphql_ws-1.0.0rc6/channels_graphql_ws/transport.py`

 * *Files identical despite different names*

### Comparing `django_channels_graphql_ws-1.0.0rc5/pyproject.toml` & `django_channels_graphql_ws-1.0.0rc6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 build-backend = "poetry.core.masonry.api"
 
 # --------------------------------------------------------------- POETRY
 # Python packaging and dependency management.
 # Docs: https://python-poetry.org/docs/
 [tool.poetry]
 name = "django-channels-graphql-ws"
-version = "v1.0.0rc5"
+version = "v1.0.0rc6"
 description = """Django Channels based WebSocket GraphQL server with Graphene-like subscriptions"""
 authors = ["Alexander A. Prokhorov <alexander.prokhorov@datadvance.net>"]
 homepage = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 repository = "https://github.com/datadvance/DjangoChannelsGraphqlWs"
 license = "MIT"
 packages = [
     { include = "channels_graphql_ws/" },
```

### Comparing `django_channels_graphql_ws-1.0.0rc5/PKG-INFO` & `django_channels_graphql_ws-1.0.0rc6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-channels-graphql-ws
-Version: 1.0.0rc5
+Version: 1.0.0rc6
 Summary: Django Channels based WebSocket GraphQL server with Graphene-like subscriptions
 Home-page: https://github.com/datadvance/DjangoChannelsGraphqlWs
 License: MIT
 Author: Alexander A. Prokhorov
 Author-email: alexander.prokhorov@datadvance.net
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

