# Comparing `tmp/pip_fluigio-0.2.2.tar.gz` & `tmp/pip_fluigio-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip_fluigio-0.2.2.tar", max compression
+gzip compressed data, was "pip_fluigio-0.2.3.tar", max compression
```

## Comparing `pip_fluigio-0.2.2.tar` & `pip_fluigio-0.2.3.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0        0 2022-10-07 16:30:04.011506 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/__init__.py
--rw-r--r--   0        0        0      552 2023-01-04 19:40:47.391773 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/card.py
--rw-r--r--   0        0        0        0 2022-10-07 16:30:04.011506 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/colleague_group.py
--rw-r--r--   0        0        0     1032 2022-12-22 19:41:01.422070 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/dataset.py
--rw-r--r--   0        0        0        0 2022-10-07 16:30:04.011506 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/document.py
--rw-r--r--   0        0        0        0 2022-10-07 16:38:18.668330 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/factories.py
--rw-r--r--   0        0        0        0 2022-10-07 16:30:04.011506 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/interfaces/__init__.py
--rw-r--r--   0        0        0      198 2022-12-22 19:41:01.415403 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/interfaces/card.py
--rw-r--r--   0        0        0     1092 2022-11-13 01:39:00.756100 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/interfaces/dataset.py
--rw-r--r--   0        0        0      750 2023-01-04 19:46:09.249807 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/interfaces/workflow_engine.py
--rw-r--r--   0        0        0      712 2022-11-13 03:09:01.520455 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/token.py
--rw-r--r--   0        0        0      837 2023-01-04 19:41:27.511529 pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/workflow_engine.py
--rw-r--r--   0        0        0        0 2022-11-10 14:41:22.896622 pip_fluigio-0.2.2/pip_fluigio/__init__.py
--rw-r--r--   0        0        0        0 2022-11-10 22:06:33.147094 pip_fluigio-0.2.2/pip_fluigio/adapters/__init__.py
--rw-r--r--   0        0        0      301 2022-12-22 19:45:39.284634 pip_fluigio-0.2.2/pip_fluigio/adapters/card.py
--rw-r--r--   0        0        0      459 2022-12-22 19:41:01.422070 pip_fluigio-0.2.2/pip_fluigio/adapters/dataset.py
--rw-r--r--   0        0        0     1483 2023-01-04 19:46:20.313073 pip_fluigio-0.2.2/pip_fluigio/adapters/workflow_engine.py
--rw-r--r--   0        0        0        0 2022-10-07 16:30:04.448170 pip_fluigio-0.2.2/pip_fluigio/fluig_services/__init__.py
--rw-r--r--   0        0        0     1065 2023-01-04 19:28:35.336199 pip_fluigio-0.2.2/pip_fluigio/fluig_services/card.py
--rw-r--r--   0        0        0        0 2022-10-07 16:30:04.448170 pip_fluigio-0.2.2/pip_fluigio/fluig_services/colleague_group.py
--rw-r--r--   0        0        0     5964 2023-01-03 00:41:58.095975 pip_fluigio-0.2.2/pip_fluigio/fluig_services/dataset.py
--rw-r--r--   0        0        0        0 2022-10-07 16:30:04.451503 pip_fluigio-0.2.2/pip_fluigio/fluig_services/document.py
--rw-r--r--   0        0        0        0 2022-10-07 21:05:41.263852 pip_fluigio-0.2.2/pip_fluigio/fluig_services/infraestruture/__init__.py
--rw-r--r--   0        0        0      749 2022-11-11 00:19:35.736691 pip_fluigio-0.2.2/pip_fluigio/fluig_services/infraestruture/server.py
--rw-r--r--   0        0        0     2348 2023-01-03 00:41:58.052642 pip_fluigio-0.2.2/pip_fluigio/fluig_services/token.py
--rw-r--r--   0        0        0     1989 2023-01-05 19:53:57.148140 pip_fluigio-0.2.2/pip_fluigio/fluig_services/workflow_engine.py
--rw-r--r--   0        0        0        0 2022-10-07 16:30:04.454837 pip_fluigio-0.2.2/pip_fluigio/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-12-22 19:54:45.721392 pip_fluigio-0.2.2/pip_fluigio/tests/adapters/__init__.py
--rw-r--r--   0        0        0        0 2022-10-07 16:30:04.454837 pip_fluigio-0.2.2/pip_fluigio/utils/__init__.py
--rw-r--r--   0        0        0      399 2023-01-04 19:54:58.273233 pip_fluigio-0.2.2/pip_fluigio/utils/commomns.py
--rw-r--r--   0        0        0      122 2022-11-10 10:51:50.982272 pip_fluigio-0.2.2/pip_fluigio/utils/exceptions.py
--rw-r--r--   0        0        0     1108 2022-11-15 03:53:21.464741 pip_fluigio-0.2.2/pip_fluigio/utils/logger.py
--rw-r--r--   0        0        0      559 2023-01-05 19:54:19.444683 pip_fluigio-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      963 2023-01-05 19:54:35.696460 pip_fluigio-0.2.2/setup.py
--rw-r--r--   0        0        0      474 2023-01-05 19:54:35.696868 pip_fluigio-0.2.2/PKG-INFO
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:30:04.011506 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/__init__.py
+-rwxr-xr-x   0        0        0      552 2023-01-04 19:40:47.391773 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/card.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:30:04.011506 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/colleague_group.py
+-rwxr-xr-x   0        0        0     1032 2022-12-22 19:41:01.422070 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/dataset.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:30:04.011506 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/document.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:38:18.668330 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/factories.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:30:04.011506 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/interfaces/__init__.py
+-rwxr-xr-x   0        0        0      198 2022-12-22 19:41:01.415403 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/interfaces/card.py
+-rwxr-xr-x   0        0        0     1092 2022-11-13 01:39:00.756099 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/interfaces/dataset.py
+-rwxr-xr-x   0        0        0      750 2023-01-04 19:46:09.249807 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/interfaces/workflow_engine.py
+-rwxr-xr-x   0        0        0      712 2022-11-13 03:09:01.520455 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/token.py
+-rwxr-xr-x   0        0        0     1431 2023-01-09 17:38:13.730882 pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/workflow_engine.py
+-rwxr-xr-x   0        0        0        0 2022-11-10 14:41:22.896622 pip_fluigio-0.2.3/pip_fluigio/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-11-10 22:06:33.147094 pip_fluigio-0.2.3/pip_fluigio/adapters/__init__.py
+-rwxr-xr-x   0        0        0      301 2022-12-22 19:45:39.284634 pip_fluigio-0.2.3/pip_fluigio/adapters/card.py
+-rwxr-xr-x   0        0        0      459 2022-12-22 19:41:01.422070 pip_fluigio-0.2.3/pip_fluigio/adapters/dataset.py
+-rwxr-xr-x   0        0        0     1483 2023-01-04 19:46:20.313072 pip_fluigio-0.2.3/pip_fluigio/adapters/workflow_engine.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:30:04.448170 pip_fluigio-0.2.3/pip_fluigio/fluig_services/__init__.py
+-rwxr-xr-x   0        0        0     1065 2023-01-04 19:28:35.336199 pip_fluigio-0.2.3/pip_fluigio/fluig_services/card.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:30:04.448170 pip_fluigio-0.2.3/pip_fluigio/fluig_services/colleague_group.py
+-rwxr-xr-x   0        0        0     5964 2023-01-03 00:41:58.095975 pip_fluigio-0.2.3/pip_fluigio/fluig_services/dataset.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:30:04.451503 pip_fluigio-0.2.3/pip_fluigio/fluig_services/document.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 21:05:41.263852 pip_fluigio-0.2.3/pip_fluigio/fluig_services/infraestruture/__init__.py
+-rwxr-xr-x   0        0        0      749 2022-11-11 00:19:35.736691 pip_fluigio-0.2.3/pip_fluigio/fluig_services/infraestruture/server.py
+-rwxr-xr-x   0        0        0     2348 2023-01-03 00:41:58.052642 pip_fluigio-0.2.3/pip_fluigio/fluig_services/token.py
+-rwxr-xr-x   0        0        0     1989 2023-01-05 19:53:57.148140 pip_fluigio-0.2.3/pip_fluigio/fluig_services/workflow_engine.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:30:04.454837 pip_fluigio-0.2.3/pip_fluigio/tests/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-12-22 19:54:45.721391 pip_fluigio-0.2.3/pip_fluigio/tests/adapters/__init__.py
+-rwxr-xr-x   0        0        0        0 2022-10-07 16:30:04.454837 pip_fluigio-0.2.3/pip_fluigio/utils/__init__.py
+-rwxr-xr-x   0        0        0      399 2023-01-04 19:54:58.273233 pip_fluigio-0.2.3/pip_fluigio/utils/commomns.py
+-rwxr-xr-x   0        0        0      122 2022-11-10 10:51:50.982272 pip_fluigio-0.2.3/pip_fluigio/utils/exceptions.py
+-rwxr-xr-x   0        0        0     1108 2022-11-15 03:53:21.464740 pip_fluigio-0.2.3/pip_fluigio/utils/logger.py
+-rwxr-xr-x   0        0        0      559 2023-05-10 17:56:59.949826 pip_fluigio-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      525 1970-01-01 00:00:00.000000 pip_fluigio-0.2.3/PKG-INFO
```

### Comparing `pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/card.py` & `pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/card.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/dataset.py` & `pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/dataset.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/interfaces/dataset.py` & `pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/interfaces/dataset.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/interfaces/workflow_engine.py` & `pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/interfaces/workflow_engine.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/token.py` & `pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/token.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/__fluig_services_base/workflow_engine.py` & `pip_fluigio-0.2.3/pip_fluigio/__fluig_services_base/workflow_engine.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,7 +29,31 @@
             thread_sequence: Optional[str]
 
         Raises:
 
         """
 
         return
+
+    def start_process(self) -> None:
+
+        """
+        Descriptions: Abstrat method start process with fluig service WSDL
+
+        Args:
+            company_id:str
+            username: str
+            password: str
+            process_id: int
+            choosed_state: int
+            colleague_id: List of Colleagues
+            comments: str
+            user_id:str
+            complete_task:str
+            attachments: List of ItemAttachments
+            items: List of Item
+            appoitments: Optional[str]
+            manager_mode: Optional[str]
+
+        Raises:
+
+        """
```

### Comparing `pip_fluigio-0.2.2/pip_fluigio/adapters/workflow_engine.py` & `pip_fluigio-0.2.3/pip_fluigio/adapters/workflow_engine.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/fluig_services/card.py` & `pip_fluigio-0.2.3/pip_fluigio/fluig_services/card.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/fluig_services/dataset.py` & `pip_fluigio-0.2.3/pip_fluigio/fluig_services/dataset.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/fluig_services/infraestruture/server.py` & `pip_fluigio-0.2.3/pip_fluigio/fluig_services/infraestruture/server.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/fluig_services/token.py` & `pip_fluigio-0.2.3/pip_fluigio/fluig_services/token.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/fluig_services/workflow_engine.py` & `pip_fluigio-0.2.3/pip_fluigio/fluig_services/workflow_engine.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pip_fluigio/utils/logger.py` & `pip_fluigio-0.2.3/pip_fluigio/utils/logger.py`

 * *Files identical despite different names*

### Comparing `pip_fluigio-0.2.2/pyproject.toml` & `pip_fluigio-0.2.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pip_fluigio"
-version = "0.2.2"
+version = "0.2.3"
 description = "abstratct library  services soap plataform fluig"
 authors = ["Rodrigo Becker <rodrigo.beckermore@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydantic = "^1.10.2"
 loguru = "^0.6.0"
```

