# Comparing `tmp/gandai-1.1.1.tar.gz` & `tmp/gandai-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gandai-1.1.1.tar", last modified: Tue May  9 22:18:20 2023, max compression
+gzip compressed data, was "gandai-1.1.2.tar", last modified: Wed May 10 05:24:57 2023, max compression
```

## Comparing `gandai-1.1.1.tar` & `gandai-1.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:18:20.205299 gandai-1.1.1/
--rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.1/MANIFEST.in
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-09 22:18:20.205170 gandai-1.1.1/PKG-INFO
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:18:20.199256 gandai-1.1.1/gandai/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-02 13:58:25.000000 gandai-1.1.1/gandai/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:18:20.202495 gandai-1.1.1/gandai/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      179 2023-04-07 16:05:45.000000 gandai-1.1.1/gandai/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.1/gandai/__pycache__/adapters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.1/gandai/__pycache__/auth.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     4152 2023-04-12 13:11:27.000000 gandai-1.1.1/gandai/__pycache__/datastore.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.1/gandai/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3736 2023-05-09 18:28:28.000000 gandai-1.1.1/gandai/__pycache__/main.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     5999 2023-05-09 18:36:56.000000 gandai-1.1.1/gandai/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    16707 2023-05-09 22:17:10.000000 gandai-1.1.1/gandai/__pycache__/query.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.1/gandai/__pycache__/services.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     7725 2023-05-09 18:21:29.000000 gandai-1.1.1/gandai/__pycache__/sources.cpython-311.pyc
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:18:20.203330 gandai-1.1.1/gandai/adapters/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-03 12:29:00.000000 gandai-1.1.1/gandai/adapters/__init__.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:18:20.204310 gandai-1.1.1/gandai/adapters/__pycache__/
--rw-r--r--   0 parker     (501) staff       (20)      188 2023-04-07 16:05:45.000000 gandai-1.1.1/gandai/adapters/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1875 2023-04-10 12:31:26.000000 gandai-1.1.1/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)      924 2023-04-07 16:06:33.000000 gandai-1.1.1/gandai/adapters/__pycache__/filters.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)    14686 2023-04-14 19:20:28.000000 gandai-1.1.1/gandai/adapters/__pycache__/grata.cpython-311.pyc
--rw-r--r--   0 parker     (501) staff       (20)     1223 2023-05-05 19:45:58.000000 gandai-1.1.1/gandai/adapters/dealcloud.py
--rw-r--r--   0 parker     (501) staff       (20)     1824 2023-03-18 19:53:14.000000 gandai-1.1.1/gandai/adapters/filters.py
--rw-r--r--   0 parker     (501) staff       (20)    10094 2023-05-04 03:54:50.000000 gandai-1.1.1/gandai/adapters/grata.py
--rw-r--r--   0 parker     (501) staff       (20)     1704 2023-03-30 16:03:27.000000 gandai-1.1.1/gandai/auth.py
--rw-r--r--   0 parker     (501) staff       (20)     1578 2023-04-12 13:11:26.000000 gandai-1.1.1/gandai/datastore.py
--rw-r--r--   0 parker     (501) staff       (20)     3089 2023-05-09 18:28:27.000000 gandai-1.1.1/gandai/main.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:18:20.204909 gandai-1.1.1/gandai/migrations/
--rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.1/gandai/migrations/__init__.py
--rw-r--r--   0 parker     (501) staff       (20)     2536 2023-05-09 21:46:03.000000 gandai-1.1.1/gandai/migrations/create_db.sql
--rw-r--r--   0 parker     (501) staff       (20)     1764 2023-04-12 12:53:47.000000 gandai-1.1.1/gandai/migrations/dealcloud_to_gandai.py
--rw-r--r--   0 parker     (501) staff       (20)     2560 2023-05-09 18:36:54.000000 gandai-1.1.1/gandai/models.py
--rw-r--r--   0 parker     (501) staff       (20)    17540 2023-05-09 22:17:08.000000 gandai-1.1.1/gandai/query.py
--rw-r--r--   0 parker     (501) staff       (20)     5348 2023-05-09 18:21:27.000000 gandai-1.1.1/gandai/sources.py
-drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-09 22:18:20.199853 gandai-1.1.1/gandai.egg-info/
--rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-09 22:18:20.000000 gandai-1.1.1/gandai.egg-info/PKG-INFO
--rw-r--r--   0 parker     (501) staff       (20)     1120 2023-05-09 22:18:20.000000 gandai-1.1.1/gandai.egg-info/SOURCES.txt
--rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-09 22:18:20.000000 gandai-1.1.1/gandai.egg-info/dependency_links.txt
--rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-09 22:18:20.000000 gandai-1.1.1/gandai.egg-info/top_level.txt
--rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-09 22:18:05.000000 gandai-1.1.1/pyproject.toml
--rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-09 22:18:20.205330 gandai-1.1.1/setup.cfg
--rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.1/setup.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.152320 gandai-1.1.2/
+-rw-r--r--   0 parker     (501) staff       (20)       26 2023-05-09 22:04:17.000000 gandai-1.1.2/MANIFEST.in
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-10 05:24:57.151903 gandai-1.1.2/PKG-INFO
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.147821 gandai-1.1.2/gandai/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-02 13:58:25.000000 gandai-1.1.2/gandai/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.150184 gandai-1.1.2/gandai/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      179 2023-04-07 16:05:45.000000 gandai-1.1.2/gandai/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7464 2023-05-09 01:55:35.000000 gandai-1.1.2/gandai/__pycache__/adapters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4191 2023-05-02 14:03:52.000000 gandai-1.1.2/gandai/__pycache__/auth.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     4152 2023-04-12 13:11:27.000000 gandai-1.1.2/gandai/__pycache__/datastore.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5979 2023-05-05 21:52:33.000000 gandai-1.1.2/gandai/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3736 2023-05-09 18:28:28.000000 gandai-1.1.2/gandai/__pycache__/main.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     5999 2023-05-09 18:36:56.000000 gandai-1.1.2/gandai/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    16707 2023-05-10 05:05:31.000000 gandai-1.1.2/gandai/__pycache__/query.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     3403 2023-05-01 00:06:24.000000 gandai-1.1.2/gandai/__pycache__/services.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     7725 2023-05-09 18:21:29.000000 gandai-1.1.2/gandai/__pycache__/sources.cpython-311.pyc
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.150894 gandai-1.1.2/gandai/adapters/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-03-03 12:29:00.000000 gandai-1.1.2/gandai/adapters/__init__.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.151387 gandai-1.1.2/gandai/adapters/__pycache__/
+-rw-r--r--   0 parker     (501) staff       (20)      188 2023-04-07 16:05:45.000000 gandai-1.1.2/gandai/adapters/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1875 2023-04-10 12:31:26.000000 gandai-1.1.2/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)      924 2023-04-07 16:06:33.000000 gandai-1.1.2/gandai/adapters/__pycache__/filters.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)    14686 2023-04-14 19:20:28.000000 gandai-1.1.2/gandai/adapters/__pycache__/grata.cpython-311.pyc
+-rw-r--r--   0 parker     (501) staff       (20)     1223 2023-05-05 19:45:58.000000 gandai-1.1.2/gandai/adapters/dealcloud.py
+-rw-r--r--   0 parker     (501) staff       (20)     1824 2023-03-18 19:53:14.000000 gandai-1.1.2/gandai/adapters/filters.py
+-rw-r--r--   0 parker     (501) staff       (20)    10094 2023-05-04 03:54:50.000000 gandai-1.1.2/gandai/adapters/grata.py
+-rw-r--r--   0 parker     (501) staff       (20)     1704 2023-03-30 16:03:27.000000 gandai-1.1.2/gandai/auth.py
+-rw-r--r--   0 parker     (501) staff       (20)     1578 2023-04-12 13:11:26.000000 gandai-1.1.2/gandai/datastore.py
+-rw-r--r--   0 parker     (501) staff       (20)     3089 2023-05-09 18:28:27.000000 gandai-1.1.2/gandai/main.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.151733 gandai-1.1.2/gandai/migrations/
+-rw-r--r--   0 parker     (501) staff       (20)        0 2023-04-10 12:18:33.000000 gandai-1.1.2/gandai/migrations/__init__.py
+-rw-r--r--   0 parker     (501) staff       (20)     2536 2023-05-09 21:46:03.000000 gandai-1.1.2/gandai/migrations/create_db.sql
+-rw-r--r--   0 parker     (501) staff       (20)     1764 2023-04-12 12:53:47.000000 gandai-1.1.2/gandai/migrations/dealcloud_to_gandai.py
+-rw-r--r--   0 parker     (501) staff       (20)     2560 2023-05-09 18:36:54.000000 gandai-1.1.2/gandai/models.py
+-rw-r--r--   0 parker     (501) staff       (20)    17549 2023-05-10 03:03:20.000000 gandai-1.1.2/gandai/query.py
+-rw-r--r--   0 parker     (501) staff       (20)     5348 2023-05-09 18:21:27.000000 gandai-1.1.2/gandai/sources.py
+drwxr-xr-x   0 parker     (501) staff       (20)        0 2023-05-10 05:24:57.148270 gandai-1.1.2/gandai.egg-info/
+-rw-r--r--   0 parker     (501) staff       (20)      215 2023-05-10 05:24:57.000000 gandai-1.1.2/gandai.egg-info/PKG-INFO
+-rw-r--r--   0 parker     (501) staff       (20)     1120 2023-05-10 05:24:57.000000 gandai-1.1.2/gandai.egg-info/SOURCES.txt
+-rw-r--r--   0 parker     (501) staff       (20)        1 2023-05-10 05:24:57.000000 gandai-1.1.2/gandai.egg-info/dependency_links.txt
+-rw-r--r--   0 parker     (501) staff       (20)        7 2023-05-10 05:24:57.000000 gandai-1.1.2/gandai.egg-info/top_level.txt
+-rw-r--r--   0 parker     (501) staff       (20)      370 2023-05-10 05:24:38.000000 gandai-1.1.2/pyproject.toml
+-rw-r--r--   0 parker     (501) staff       (20)       38 2023-05-10 05:24:57.152363 gandai-1.1.2/setup.cfg
+-rw-r--r--   0 parker     (501) staff       (20)      159 2023-03-06 14:38:11.000000 gandai-1.1.2/setup.py
```

### Comparing `gandai-1.1.1/gandai/__pycache__/adapters.cpython-311.pyc` & `gandai-1.1.2/gandai/__pycache__/adapters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/__pycache__/auth.cpython-311.pyc` & `gandai-1.1.2/gandai/__pycache__/auth.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/__pycache__/datastore.cpython-311.pyc` & `gandai-1.1.2/gandai/__pycache__/datastore.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.2/gandai/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/__pycache__/main.cpython-311.pyc` & `gandai-1.1.2/gandai/__pycache__/main.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/__pycache__/models.cpython-311.pyc` & `gandai-1.1.2/gandai/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/__pycache__/query.cpython-311.pyc` & `gandai-1.1.2/gandai/__pycache__/query.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x64c65a64 (Tue May  9 22:17:08 2023 UTC)
-files sz: 17540
+moddate:  0x78095b64 (Wed May 10 03:03:20 2023 UTC)
+files sz: 17549
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a02640064026c036d045a0401
@@ -102,148 +102,148 @@
                134 CALL                     0
                144 POP_TOP
    
     24         146 LOAD_CONST               8 (<code object get_engine, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 24>)
                148 MAKE_FUNCTION            0
                150 STORE_NAME              21 (get_engine)
    
-    48         152 PUSH_NULL
+    49         152 PUSH_NULL
                154 LOAD_NAME               21 (get_engine)
                156 PRECALL                  0
                160 CALL                     0
                170 STORE_NAME              22 (engine)
    
-    54         172 LOAD_CONST               9 ('company')
+    55         172 LOAD_CONST               9 ('company')
                174 LOAD_NAME                9 (Company)
                176 BUILD_TUPLE              2
-               178 LOAD_CONST              10 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 54>)
+               178 LOAD_CONST              10 (<code object insert_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 55>)
                180 MAKE_FUNCTION            4 (annotations)
                182 STORE_NAME              23 (insert_company)
    
-    68         184 LOAD_CONST              11 ('event')
+    69         184 LOAD_CONST              11 ('event')
                186 LOAD_NAME                8 (Event)
                188 LOAD_CONST              12 ('return')
                190 LOAD_NAME                8 (Event)
                192 BUILD_TUPLE              4
-               194 LOAD_CONST              13 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 68>)
+               194 LOAD_CONST              13 (<code object insert_event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 69>)
                196 MAKE_FUNCTION            4 (annotations)
                198 STORE_NAME              24 (insert_event)
    
-    89         200 LOAD_CONST              14 ('actor')
+    90         200 LOAD_CONST              14 ('actor')
                202 LOAD_NAME               11 (Actor)
                204 LOAD_CONST              12 ('return')
                206 LOAD_NAME               11 (Actor)
                208 BUILD_TUPLE              4
-               210 LOAD_CONST              15 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 89>)
+               210 LOAD_CONST              15 (<code object insert_actor, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 90>)
                212 MAKE_FUNCTION            4 (annotations)
                214 STORE_NAME              25 (insert_actor)
    
-   104         216 LOAD_CONST              16 ('search')
+   105         216 LOAD_CONST              16 ('search')
                218 LOAD_NAME               12 (Search)
                220 LOAD_CONST              12 ('return')
                222 LOAD_NAME               12 (Search)
                224 BUILD_TUPLE              4
-               226 LOAD_CONST              17 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 104>)
+               226 LOAD_CONST              17 (<code object insert_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 105>)
                228 MAKE_FUNCTION            4 (annotations)
                230 STORE_NAME              26 (insert_search)
    
-   123         232 LOAD_CONST              18 ('checkpoint')
+   124         232 LOAD_CONST              18 ('checkpoint')
                234 LOAD_NAME               13 (Checkpoint)
                236 LOAD_CONST              12 ('return')
                238 LOAD_NAME               13 (Checkpoint)
                240 BUILD_TUPLE              4
-               242 LOAD_CONST              19 (<code object insert_checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 123>)
+               242 LOAD_CONST              19 (<code object insert_checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 124>)
                244 MAKE_FUNCTION            4 (annotations)
                246 STORE_NAME              27 (insert_checkpoint)
    
-   139         248 LOAD_CONST              20 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 139>)
+   140         248 LOAD_CONST              20 (<code object search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 140>)
                250 MAKE_FUNCTION            0
                252 STORE_NAME              28 (search)
    
-   146         254 LOAD_CONST              34 (('advance',))
+   147         254 LOAD_CONST              34 (('advance',))
                256 LOAD_CONST              22 ('search_uid')
                258 LOAD_NAME               29 (int)
                260 LOAD_CONST              23 ('last_event_type')
                262 LOAD_NAME               30 (str)
                264 BUILD_TUPLE              4
-               266 LOAD_CONST              24 (<code object target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 146>)
+               266 LOAD_CONST              24 (<code object target, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 147>)
                268 MAKE_FUNCTION            5 (defaults, annotations)
                270 STORE_NAME              31 (target)
    
-   170         272 LOAD_CONST              22 ('search_uid')
+   171         272 LOAD_CONST              22 ('search_uid')
                274 LOAD_NAME               29 (int)
                276 LOAD_CONST              12 ('return')
                278 LOAD_NAME                2 (pd)
                280 LOAD_ATTR               32 (DataFrame)
                290 BUILD_TUPLE              4
-               292 LOAD_CONST              25 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 170>)
+               292 LOAD_CONST              25 (<code object target_count, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 171>)
                294 MAKE_FUNCTION            4 (annotations)
                296 STORE_NAME              33 (target_count)
    
-   186         298 LOAD_CONST              22 ('search_uid')
+   187         298 LOAD_CONST              22 ('search_uid')
                300 LOAD_NAME               29 (int)
                302 LOAD_CONST              12 ('return')
                304 LOAD_NAME                2 (pd)
                306 LOAD_ATTR               32 (DataFrame)
                316 BUILD_TUPLE              4
-               318 LOAD_CONST              26 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 186>)
+               318 LOAD_CONST              26 (<code object event, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 187>)
                320 MAKE_FUNCTION            4 (annotations)
                322 STORE_NAME              34 (event)
    
-   198         324 LOAD_CONST              12 ('return')
+   199         324 LOAD_CONST              12 ('return')
                326 LOAD_NAME                2 (pd)
                328 LOAD_ATTR               32 (DataFrame)
                338 BUILD_TUPLE              2
-               340 LOAD_CONST              27 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 198>)
+               340 LOAD_CONST              27 (<code object checkpoint, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 199>)
                342 MAKE_FUNCTION            4 (annotations)
                344 STORE_NAME              35 (checkpoint)
    
-   209         346 LOAD_CONST              22 ('search_uid')
+   210         346 LOAD_CONST              22 ('search_uid')
                348 LOAD_NAME               29 (int)
                350 LOAD_CONST              12 ('return')
                352 LOAD_NAME                2 (pd)
                354 LOAD_ATTR               32 (DataFrame)
                364 BUILD_TUPLE              4
-               366 LOAD_CONST              28 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 209>)
+               366 LOAD_CONST              28 (<code object comment_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 210>)
                368 MAKE_FUNCTION            4 (annotations)
                370 STORE_NAME              36 (comment_by_domain)
    
-   230         372 LOAD_CONST              22 ('search_uid')
+   231         372 LOAD_CONST              22 ('search_uid')
                374 LOAD_NAME               29 (int)
                376 LOAD_CONST              12 ('return')
                378 LOAD_NAME               12 (Search)
                380 BUILD_TUPLE              4
-               382 LOAD_CONST              29 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 230>)
+               382 LOAD_CONST              29 (<code object find_search_by_uid, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 231>)
                384 MAKE_FUNCTION            4 (annotations)
                386 STORE_NAME              37 (find_search_by_uid)
    
-   246         388 LOAD_CONST              30 ('domain')
+   247         388 LOAD_CONST              30 ('domain')
                390 LOAD_NAME               30 (str)
                392 LOAD_CONST              12 ('return')
                394 LOAD_NAME                9 (Company)
                396 BUILD_TUPLE              4
-               398 LOAD_CONST              31 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 246>)
+               398 LOAD_CONST              31 (<code object find_company_by_domain, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 247>)
                400 MAKE_FUNCTION            4 (annotations)
                402 STORE_NAME              38 (find_company_by_domain)
    
-   265         404 LOAD_CONST               9 ('company')
+   266         404 LOAD_CONST               9 ('company')
                406 LOAD_NAME                9 (Company)
                408 LOAD_CONST              12 ('return')
                410 LOAD_CONST               1 (None)
                412 BUILD_TUPLE              4
-               414 LOAD_CONST              32 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 265>)
+               414 LOAD_CONST              32 (<code object update_company, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 266>)
                416 MAKE_FUNCTION            4 (annotations)
                418 STORE_NAME              39 (update_company)
    
-   289         420 LOAD_CONST              16 ('search')
+   290         420 LOAD_CONST              16 ('search')
                422 LOAD_NAME               12 (Search)
                424 LOAD_CONST              12 ('return')
                426 LOAD_CONST               1 (None)
                428 BUILD_TUPLE              4
-               430 LOAD_CONST              33 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 289>)
+               430 LOAD_CONST              33 (<code object update_search, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 290>)
                432 MAKE_FUNCTION            4 (annotations)
                434 STORE_NAME              40 (update_search)
                436 LOAD_CONST               1 (None)
                438 RETURN_VALUE
    consts
       0
       None
@@ -313,33 +313,33 @@
                      208 POP_JUMP_FORWARD_IF_FALSE    43 (to 296)
          
           31         210 LOAD_GLOBAL             11 (NULL + Connector)
                      222 PRECALL                  0
                      226 CALL                     0
                      236 STORE_DEREF              3 (connector)
          
-          32         238 LOAD_CLOSURE             3 (connector)
+          33         238 LOAD_CLOSURE             3 (connector)
                      240 BUILD_TUPLE              1
-                     242 LOAD_CONST               5 (<code object getconn, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 32>)
+                     242 LOAD_CONST               5 (<code object getconn, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 33>)
                      244 MAKE_FUNCTION            8 (closure)
                      246 STORE_FAST               1 (getconn)
          
-          41         248 LOAD_GLOBAL              7 (NULL + sqlalchemy)
+          42         248 LOAD_GLOBAL              7 (NULL + sqlalchemy)
                      260 LOAD_ATTR                4 (create_engine)
          
-          42         270 LOAD_CONST               6 ('postgresql+pg8000://')
+          43         270 LOAD_CONST               6 ('postgresql+pg8000://')
          
-          43         272 LOAD_FAST                1 (getconn)
+          44         272 LOAD_FAST                1 (getconn)
          
-          41         274 KW_NAMES                 7
+          42         274 KW_NAMES                 7
                      276 PRECALL                  2
                      280 CALL                     2
                      290 STORE_FAST               2 (pool)
          
-          45         292 LOAD_FAST                2 (pool)
+          46         292 LOAD_FAST                2 (pool)
                      294 RETURN_VALUE
          
           29     >>  296 LOAD_CONST               0 (None)
                      298 RETURN_VALUE
          consts
             None
             'ENV_STAGE'
@@ -357,51 +357,51 @@
                   0000000000000064027403000000000000000000006a0200000000000000
                   006403a6010000ab0100000000000000007403000000000000000000006a
                   0200000000000000006404a6010000ab0100000000000000007403000000
                   000000000000006a0200000000000000006405a6010000ab010000000000
                   000000ac06a6050000ab0500000000000000007d007c005300
                              0 COPY_FREE_VARS           1
                
-                32           2 RESUME                   0
+                33           2 RESUME                   0
                
-                33           4 LOAD_DEREF               1 (connector)
+                34           4 LOAD_DEREF               1 (connector)
                              6 LOAD_METHOD              0 (connect)
                
-                34          28 LOAD_GLOBAL              3 (NULL + os)
+                35          28 LOAD_GLOBAL              3 (NULL + os)
                             40 LOAD_ATTR                2 (getenv)
                             50 LOAD_CONST               1 ('INSTANCE_CONNECTION_NAME')
                             52 PRECALL                  1
                             56 CALL                     1
                
-                35          66 LOAD_CONST               2 ('pg8000')
+                36          66 LOAD_CONST               2 ('pg8000')
                
-                36          68 LOAD_GLOBAL              3 (NULL + os)
+                37          68 LOAD_GLOBAL              3 (NULL + os)
                             80 LOAD_ATTR                2 (getenv)
                             90 LOAD_CONST               3 ('DB_USER')
                             92 PRECALL                  1
                             96 CALL                     1
                
-                37         106 LOAD_GLOBAL              3 (NULL + os)
+                38         106 LOAD_GLOBAL              3 (NULL + os)
                            118 LOAD_ATTR                2 (getenv)
                            128 LOAD_CONST               4 ('DB_PASS')
                            130 PRECALL                  1
                            134 CALL                     1
                
-                38         144 LOAD_GLOBAL              3 (NULL + os)
+                39         144 LOAD_GLOBAL              3 (NULL + os)
                            156 LOAD_ATTR                2 (getenv)
                            166 LOAD_CONST               5 ('DB_NAME')
                            168 PRECALL                  1
                            172 CALL                     1
                
-                33         182 KW_NAMES                 6
+                34         182 KW_NAMES                 6
                            184 PRECALL                  5
                            188 CALL                     5
                            198 STORE_FAST               0 (conn)
                
-                40         200 LOAD_FAST                0 (conn)
+                41         200 LOAD_FAST                0 (conn)
                            202 RETURN_VALUE
                consts
                   None
                   'INSTANCE_CONNECTION_NAME'
                   'pg8000'
                   'DB_USER'
                   'DB_PASS'
@@ -409,26 +409,26 @@
                   ('user', 'password', 'db')
                names      ('connect', 'os', 'getenv')
                varnames   ('conn',)
                freevars   ('connector',)
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       'getconn'
-               firstlineno 32
+               firstlineno 33
                lnotab 0x04011801260102012601260126fb1207
             'postgresql+pg8000://'
             ('creator',)
          names      ('print', 'os', 'getenv', 'sqlalchemy', 'create_engine', 'Connector')
          varnames   ('DB_URI', 'getconn', 'pool')
          freevars   ()
          cellvars   ('connector',)
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'get_engine'
          firstlineno 24
-         lnotab 0x0401420130010401280130021c010a091601020102fe120404f0
+         lnotab 0x0401420130010401280130021c020a091601020102fe120404ef
       'company'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
          code
@@ -437,49 +437,49 @@
             000000000000006401a6010000ab0100000000000000007d027c01a00300
             000000000000000000000000000000000000007c02740900000000000000
             0000007c00a6010000ab010000000000000000a6020000ab020000000000
             00000001007c01a0050000000000000000000000000000000000000000a6
             000000ab0000000000000000000100640064006400a6020000ab02000000
             000000000001006e0b230031007304770278035900770101005900010001
             007c005300
-          54           0 RESUME                   0
+          55           0 RESUME                   0
          
-          55           2 LOAD_GLOBAL              0 (engine)
+          56           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          56          54 LOAD_GLOBAL              5 (NULL + text)
+          57          54 LOAD_GLOBAL              5 (NULL + text)
          
-          57          66 LOAD_CONST               1 ('\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            ')
+          58          66 LOAD_CONST               1 ('\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            ')
          
-          56          68 PRECALL                  1
+          57          68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               2 (statement)
          
-          63          84 LOAD_FAST                1 (con)
+          64          84 LOAD_FAST                1 (con)
                       86 LOAD_METHOD              3 (execute)
                      108 LOAD_FAST                2 (statement)
                      110 LOAD_GLOBAL              9 (NULL + asdict)
                      122 LOAD_FAST                0 (company)
                      124 PRECALL                  1
                      128 CALL                     1
                      138 PRECALL                  2
                      142 CALL                     2
                      152 POP_TOP
          
-          64         154 LOAD_FAST                1 (con)
+          65         154 LOAD_FAST                1 (con)
                      156 LOAD_METHOD              5 (commit)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 POP_TOP
          
-          55         194 LOAD_CONST               0 (None)
+          56         194 LOAD_CONST               0 (None)
                      196 LOAD_CONST               0 (None)
                      198 LOAD_CONST               0 (None)
                      200 PRECALL                  2
                      204 CALL                     2
                      214 POP_TOP
                      216 JUMP_FORWARD            11 (to 240)
                  >>  218 PUSH_EXC_INFO
@@ -490,30 +490,30 @@
                      228 POP_EXCEPT
                      230 RERAISE                  1
                  >>  232 POP_TOP
                      234 POP_EXCEPT
                      236 POP_TOP
                      238 POP_TOP
          
-          65     >>  240 LOAD_FAST                0 (company)
+          66     >>  240 LOAD_FAST                0 (company)
                      242 RETURN_VALUE
          ExceptionTable:
            52 to 192 -> 218 [1] lasti
            218 to 224 -> 226 [3] lasti
            232 to 232 -> 226 [3] lasti
          consts
             None
             '\n                INSERT INTO company (domain, name, description) \n                VALUES(:domain, :name, :description)\n                ON CONFLICT DO NOTHING\n            '
          names      ('engine', 'connect', 'text', 'execute', 'asdict', 'commit')
          varnames   ('company', 'con', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_company'
-         firstlineno 54
+         firstlineno 55
          lnotab 0x020134010c0102ff1007460128f72e0a
       'event'
       'return'
       code
          argcount  : 1
          nlocals   : 6
          stacksize : 6
@@ -530,89 +530,89 @@
             00a6000000ab0000000000000000007d057c0572087c0564031900000000
             00000000006e0164007c005f0800000000000000007c01a0060000000000
             0000000000000000000000000000007405000000000000000000006404a6
             010000ab010000000000000000a6010000ab01000000000000000001007c
             01a0090000000000000000000000000000000000000000a6000000ab0000
             000000000000000100640064006400a6020000ab02000000000000000001
             006e0b230031007304770278035900770101005900010001007c005300
-          68           0 RESUME                   0
+          69           0 RESUME                   0
          
-          69           2 LOAD_GLOBAL              0 (engine)
+          70           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          70          54 LOAD_GLOBAL              5 (NULL + text)
+          71          54 LOAD_GLOBAL              5 (NULL + text)
          
-          71          66 LOAD_CONST               1 ('\n                INSERT INTO event (search_uid, domain, actor_key, type, data) \n                VALUES(:search_uid, :domain, :actor_key, :type, :data)\n                ON CONFLICT DO NOTHING\n                RETURNING id\n            ')
+          72          66 LOAD_CONST               1 ('\n                INSERT INTO event (search_uid, domain, actor_key, type, data) \n                VALUES(:search_uid, :domain, :actor_key, :type, :data)\n                ON CONFLICT DO NOTHING\n                RETURNING id\n            ')
          
-          70          68 PRECALL                  1
+          71          68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               2 (statement)
          
-          78          84 LOAD_GLOBAL              7 (NULL + asdict)
+          79          84 LOAD_GLOBAL              7 (NULL + asdict)
                       96 LOAD_FAST                0 (event)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_FAST               3 (obj)
          
-          79         114 LOAD_GLOBAL              9 (NULL + json)
+          80         114 LOAD_GLOBAL              9 (NULL + json)
                      126 LOAD_ATTR                5 (dumps)
                      136 LOAD_FAST                3 (obj)
                      138 LOAD_CONST               2 ('data')
                      140 BINARY_SUBSCR
                      150 PRECALL                  1
                      154 CALL                     1
                      164 LOAD_FAST                3 (obj)
                      166 LOAD_CONST               2 ('data')
                      168 STORE_SUBSCR
          
-          80         172 LOAD_FAST                1 (con)
+          81         172 LOAD_FAST                1 (con)
                      174 LOAD_METHOD              6 (execute)
                      196 LOAD_FAST                2 (statement)
                      198 LOAD_FAST                3 (obj)
                      200 PRECALL                  2
                      204 CALL                     2
                      214 STORE_FAST               4 (result)
          
-          82         216 LOAD_FAST                4 (result)
+          83         216 LOAD_FAST                4 (result)
                      218 LOAD_METHOD              7 (first)
                      240 PRECALL                  0
                      244 CALL                     0
                      254 STORE_FAST               5 (_id)
          
-          83         256 LOAD_FAST                5 (_id)
+          84         256 LOAD_FAST                5 (_id)
                      258 POP_JUMP_FORWARD_IF_FALSE     8 (to 276)
                      260 LOAD_FAST                5 (_id)
                      262 LOAD_CONST               3 (0)
                      264 BINARY_SUBSCR
                      274 JUMP_FORWARD             1 (to 278)
                  >>  276 LOAD_CONST               0 (None)
                  >>  278 LOAD_FAST                0 (event)
                      280 STORE_ATTR               8 (id)
          
-          84         290 LOAD_FAST                1 (con)
+          85         290 LOAD_FAST                1 (con)
                      292 LOAD_METHOD              6 (execute)
                      314 LOAD_GLOBAL              5 (NULL + text)
                      326 LOAD_CONST               4 ('REFRESH MATERIALIZED VIEW target')
                      328 PRECALL                  1
                      332 CALL                     1
                      342 PRECALL                  1
                      346 CALL                     1
                      356 POP_TOP
          
-          85         358 LOAD_FAST                1 (con)
+          86         358 LOAD_FAST                1 (con)
                      360 LOAD_METHOD              9 (commit)
                      382 PRECALL                  0
                      386 CALL                     0
                      396 POP_TOP
          
-          69         398 LOAD_CONST               0 (None)
+          70         398 LOAD_CONST               0 (None)
                      400 LOAD_CONST               0 (None)
                      402 LOAD_CONST               0 (None)
                      404 PRECALL                  2
                      408 CALL                     2
                      418 POP_TOP
                      420 JUMP_FORWARD            11 (to 444)
                  >>  422 PUSH_EXC_INFO
@@ -623,15 +623,15 @@
                      432 POP_EXCEPT
                      434 RERAISE                  1
                  >>  436 POP_TOP
                      438 POP_EXCEPT
                      440 POP_TOP
                      442 POP_TOP
          
-          86     >>  444 LOAD_FAST                0 (event)
+          87     >>  444 LOAD_FAST                0 (event)
                      446 RETURN_VALUE
          ExceptionTable:
            52 to 396 -> 422 [1] lasti
            422 to 428 -> 430 [3] lasti
            436 to 436 -> 430 [3] lasti
          consts
             None
@@ -641,15 +641,15 @@
             'REFRESH MATERIALIZED VIEW target'
          names      ('engine', 'connect', 'text', 'asdict', 'json', 'dumps', 'execute', 'first', 'id', 'commit')
          varnames   ('event', 'con', 'statement', 'obj', 'result', '_id')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_event'
-         firstlineno 68
+         firstlineno 69
          lnotab 0x020134010c0102ff10081e013a012c0228012201440128f02e11
       'actor'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
@@ -659,52 +659,52 @@
             000000000000006401a6010000ab0100000000000000007d027407000000
             000000000000007c00a6010000ab0100000000000000007d037c01a00400
             000000000000000000000000000000000000007c027c03a6020000ab0200
             0000000000000001007c01a0050000000000000000000000000000000000
             000000a6000000ab0000000000000000000100640064006400a6020000ab
             02000000000000000001006e0b2300310073047702780359007701010059
             00010001007c005300
-          89           0 RESUME                   0
+          90           0 RESUME                   0
          
-          90           2 LOAD_GLOBAL              0 (engine)
+          91           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-          91          54 LOAD_GLOBAL              5 (NULL + text)
+          92          54 LOAD_GLOBAL              5 (NULL + text)
          
-          92          66 LOAD_CONST               1 ('\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            ')
+          93          66 LOAD_CONST               1 ('\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            ')
          
-          91          68 PRECALL                  1
+          92          68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               2 (statement)
          
-          98          84 LOAD_GLOBAL              7 (NULL + asdict)
+          99          84 LOAD_GLOBAL              7 (NULL + asdict)
                       96 LOAD_FAST                0 (actor)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_FAST               3 (obj)
          
-          99         114 LOAD_FAST                1 (con)
+         100         114 LOAD_FAST                1 (con)
                      116 LOAD_METHOD              4 (execute)
                      138 LOAD_FAST                2 (statement)
                      140 LOAD_FAST                3 (obj)
                      142 PRECALL                  2
                      146 CALL                     2
                      156 POP_TOP
          
-         100         158 LOAD_FAST                1 (con)
+         101         158 LOAD_FAST                1 (con)
                      160 LOAD_METHOD              5 (commit)
                      182 PRECALL                  0
                      186 CALL                     0
                      196 POP_TOP
          
-          90         198 LOAD_CONST               0 (None)
+          91         198 LOAD_CONST               0 (None)
                      200 LOAD_CONST               0 (None)
                      202 LOAD_CONST               0 (None)
                      204 PRECALL                  2
                      208 CALL                     2
                      218 POP_TOP
                      220 JUMP_FORWARD            11 (to 244)
                  >>  222 PUSH_EXC_INFO
@@ -715,30 +715,30 @@
                      232 POP_EXCEPT
                      234 RERAISE                  1
                  >>  236 POP_TOP
                      238 POP_EXCEPT
                      240 POP_TOP
                      242 POP_TOP
          
-         101     >>  244 LOAD_FAST                0 (actor)
+         102     >>  244 LOAD_FAST                0 (actor)
                      246 RETURN_VALUE
          ExceptionTable:
            52 to 196 -> 222 [1] lasti
            222 to 228 -> 230 [3] lasti
            236 to 236 -> 230 [3] lasti
          consts
             None
             '\n                INSERT INTO actor (key, type, name) \n                VALUES(:key, :type, :name)\n                ON CONFLICT DO NOTHING\n            '
          names      ('engine', 'connect', 'text', 'asdict', 'execute', 'commit')
          varnames   ('actor', 'con', 'statement', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_actor'
-         firstlineno 89
+         firstlineno 90
          lnotab 0x020134010c0102ff10071e012c0128f62e0b
       'search'
       code
          argcount  : 1
          nlocals   : 4
          stacksize : 6
          flags     : 3
@@ -756,96 +756,96 @@
             006a0500000000000000007c03640519000000000000000000a6010000ab
             0100000000000000007c0364053c0000007c01a006000000000000000000
             00000000000000000000007c027c03a6020000ab02000000000000000001
             007c01a0070000000000000000000000000000000000000000a6000000ab
             0000000000000000000100640064006400a6020000ab0200000000000000
             0001006e0b230031007304770278035900770101005900010001007c0053
             00
-         104           0 RESUME                   0
+         105           0 RESUME                   0
          
-         105           2 LOAD_GLOBAL              0 (engine)
+         106           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-         106          54 LOAD_GLOBAL              5 (NULL + text)
+         107          54 LOAD_GLOBAL              5 (NULL + text)
          
-         107          66 LOAD_CONST               1 ('\n                INSERT INTO search (uid, client_domain, label, meta, inclusion, exclusion, sort) \n                VALUES(:uid, :client_domain, :label, :meta, :inclusion, :exclusion, :sort)\n                ON CONFLICT DO NOTHING\n            ')
+         108          66 LOAD_CONST               1 ('\n                INSERT INTO search (uid, client_domain, label, meta, inclusion, exclusion, sort) \n                VALUES(:uid, :client_domain, :label, :meta, :inclusion, :exclusion, :sort)\n                ON CONFLICT DO NOTHING\n            ')
          
-         106          68 PRECALL                  1
+         107          68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               2 (statement)
          
-         113          84 LOAD_GLOBAL              7 (NULL + asdict)
+         114          84 LOAD_GLOBAL              7 (NULL + asdict)
                       96 LOAD_FAST                0 (search)
                       98 PRECALL                  1
                      102 CALL                     1
                      112 STORE_FAST               3 (obj)
          
-         114         114 LOAD_GLOBAL              9 (NULL + json)
+         115         114 LOAD_GLOBAL              9 (NULL + json)
                      126 LOAD_ATTR                5 (dumps)
                      136 LOAD_FAST                3 (obj)
                      138 LOAD_CONST               2 ('meta')
                      140 BINARY_SUBSCR
                      150 PRECALL                  1
                      154 CALL                     1
                      164 LOAD_FAST                3 (obj)
                      166 LOAD_CONST               2 ('meta')
                      168 STORE_SUBSCR
          
-         115         172 LOAD_GLOBAL              9 (NULL + json)
+         116         172 LOAD_GLOBAL              9 (NULL + json)
                      184 LOAD_ATTR                5 (dumps)
                      194 LOAD_FAST                3 (obj)
                      196 LOAD_CONST               3 ('inclusion')
                      198 BINARY_SUBSCR
                      208 PRECALL                  1
                      212 CALL                     1
                      222 LOAD_FAST                3 (obj)
                      224 LOAD_CONST               3 ('inclusion')
                      226 STORE_SUBSCR
          
-         116         230 LOAD_GLOBAL              9 (NULL + json)
+         117         230 LOAD_GLOBAL              9 (NULL + json)
                      242 LOAD_ATTR                5 (dumps)
                      252 LOAD_FAST                3 (obj)
                      254 LOAD_CONST               4 ('exclusion')
                      256 BINARY_SUBSCR
                      266 PRECALL                  1
                      270 CALL                     1
                      280 LOAD_FAST                3 (obj)
                      282 LOAD_CONST               4 ('exclusion')
                      284 STORE_SUBSCR
          
-         117         288 LOAD_GLOBAL              9 (NULL + json)
+         118         288 LOAD_GLOBAL              9 (NULL + json)
                      300 LOAD_ATTR                5 (dumps)
                      310 LOAD_FAST                3 (obj)
                      312 LOAD_CONST               5 ('sort')
                      314 BINARY_SUBSCR
                      324 PRECALL                  1
                      328 CALL                     1
                      338 LOAD_FAST                3 (obj)
                      340 LOAD_CONST               5 ('sort')
                      342 STORE_SUBSCR
          
-         118         346 LOAD_FAST                1 (con)
+         119         346 LOAD_FAST                1 (con)
                      348 LOAD_METHOD              6 (execute)
                      370 LOAD_FAST                2 (statement)
                      372 LOAD_FAST                3 (obj)
                      374 PRECALL                  2
                      378 CALL                     2
                      388 POP_TOP
          
-         119         390 LOAD_FAST                1 (con)
+         120         390 LOAD_FAST                1 (con)
                      392 LOAD_METHOD              7 (commit)
                      414 PRECALL                  0
                      418 CALL                     0
                      428 POP_TOP
          
-         105         430 LOAD_CONST               0 (None)
+         106         430 LOAD_CONST               0 (None)
                      432 LOAD_CONST               0 (None)
                      434 LOAD_CONST               0 (None)
                      436 PRECALL                  2
                      440 CALL                     2
                      450 POP_TOP
                      452 JUMP_FORWARD            11 (to 476)
                  >>  454 PUSH_EXC_INFO
@@ -856,15 +856,15 @@
                      464 POP_EXCEPT
                      466 RERAISE                  1
                  >>  468 POP_TOP
                      470 POP_EXCEPT
                      472 POP_TOP
                      474 POP_TOP
          
-         120     >>  476 LOAD_FAST                0 (search)
+         121     >>  476 LOAD_FAST                0 (search)
                      478 RETURN_VALUE
          ExceptionTable:
            52 to 428 -> 454 [1] lasti
            454 to 460 -> 462 [3] lasti
            468 to 468 -> 462 [3] lasti
          consts
             None
@@ -875,15 +875,15 @@
             'sort'
          names      ('engine', 'connect', 'text', 'asdict', 'json', 'dumps', 'execute', 'commit')
          varnames   ('search', 'con', 'statement', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_search'
-         firstlineno 104
+         firstlineno 105
          lnotab 0x020134010c0102ff10071e013a013a013a013a012c0128f22e0f
       'checkpoint'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 7
          flags     : 3
@@ -893,49 +893,49 @@
             000000000000006401a6010000ab0100000000000000007d027c01a00300
             000000000000000000000000000000000000007c02740900000000000000
             0000007c00a6010000ab010000000000000000a6020000ab020000000000
             00000001007c01a0050000000000000000000000000000000000000000a6
             000000ab0000000000000000000100640064006400a6020000ab02000000
             000000000001006e0b230031007304770278035900770101005900010001
             007c005300
-         123           0 RESUME                   0
+         124           0 RESUME                   0
          
-         124           2 LOAD_GLOBAL              0 (engine)
+         125           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (con)
          
-         125          54 LOAD_GLOBAL              5 (NULL + text)
+         126          54 LOAD_GLOBAL              5 (NULL + text)
          
-         126          66 LOAD_CONST               1 ('\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            ')
+         127          66 LOAD_CONST               1 ('\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            ')
          
-         125          68 PRECALL                  1
+         126          68 PRECALL                  1
                       72 CALL                     1
                       82 STORE_FAST               2 (statement)
          
-         131          84 LOAD_FAST                1 (con)
+         132          84 LOAD_FAST                1 (con)
                       86 LOAD_METHOD              3 (execute)
                      108 LOAD_FAST                2 (statement)
                      110 LOAD_GLOBAL              9 (NULL + asdict)
                      122 LOAD_FAST                0 (checkpoint)
                      124 PRECALL                  1
                      128 CALL                     1
                      138 PRECALL                  2
                      142 CALL                     2
                      152 POP_TOP
          
-         132         154 LOAD_FAST                1 (con)
+         133         154 LOAD_FAST                1 (con)
                      156 LOAD_METHOD              5 (commit)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 POP_TOP
          
-         124         194 LOAD_CONST               0 (None)
+         125         194 LOAD_CONST               0 (None)
                      196 LOAD_CONST               0 (None)
                      198 LOAD_CONST               0 (None)
                      200 PRECALL                  2
                      204 CALL                     2
                      214 POP_TOP
                      216 JUMP_FORWARD            11 (to 240)
                  >>  218 PUSH_EXC_INFO
@@ -946,30 +946,30 @@
                      228 POP_EXCEPT
                      230 RERAISE                  1
                  >>  232 POP_TOP
                      234 POP_EXCEPT
                      236 POP_TOP
                      238 POP_TOP
          
-         133     >>  240 LOAD_FAST                0 (checkpoint)
+         134     >>  240 LOAD_FAST                0 (checkpoint)
                      242 RETURN_VALUE
          ExceptionTable:
            52 to 192 -> 218 [1] lasti
            218 to 224 -> 226 [3] lasti
            232 to 232 -> 226 [3] lasti
          consts
             None
             '\n                INSERT INTO checkpoint (event_id) \n                VALUES(:event_id)\n            '
          names      ('engine', 'connect', 'text', 'execute', 'asdict', 'commit')
          varnames   ('checkpoint', 'con', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'insert_checkpoint'
-         firstlineno 123
+         firstlineno 124
          lnotab 0x020134010c0102ff1006460128f82e09
       code
          argcount  : 0
          nlocals   : 3
          stacksize : 6
          flags     : 3
          code
@@ -979,49 +979,49 @@
             006401a6010000ab010000000000000000a6010000ab0100000000000000
             007d017409000000000000000000006a0500000000000000007c01a00600
             00000000000000000000000000000000000000a6000000ab000000000000
             0000007c01a0070000000000000000000000000000000000000000a60000
             00ab000000000000000000ac02a6020000ab0200000000000000007d0264
             0064006400a6020000ab02000000000000000001006e0b23003100730477
             0278035900770101005900010001007c025300
-         139           0 RESUME                   0
+         140           0 RESUME                   0
          
-         140           2 LOAD_GLOBAL              0 (engine)
+         141           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         141          54 LOAD_FAST                0 (conn)
+         142          54 LOAD_FAST                0 (conn)
                       56 LOAD_METHOD              2 (execute)
                       78 LOAD_GLOBAL              7 (NULL + text)
                       90 LOAD_CONST               1 ("SELECT *, meta->>'group' as group FROM search")
                       92 PRECALL                  1
                       96 CALL                     1
                      106 PRECALL                  1
                      110 CALL                     1
                      120 STORE_FAST               1 (result)
          
-         142         122 LOAD_GLOBAL              9 (NULL + pd)
+         143         122 LOAD_GLOBAL              9 (NULL + pd)
                      134 LOAD_ATTR                5 (DataFrame)
                      144 LOAD_FAST                1 (result)
                      146 LOAD_METHOD              6 (fetchall)
                      168 PRECALL                  0
                      172 CALL                     0
                      182 LOAD_FAST                1 (result)
                      184 LOAD_METHOD              7 (keys)
                      206 PRECALL                  0
                      210 CALL                     0
                      220 KW_NAMES                 2
                      222 PRECALL                  2
                      226 CALL                     2
                      236 STORE_FAST               2 (df)
          
-         140         238 LOAD_CONST               0 (None)
+         141         238 LOAD_CONST               0 (None)
                      240 LOAD_CONST               0 (None)
                      242 LOAD_CONST               0 (None)
                      244 PRECALL                  2
                      248 CALL                     2
                      258 POP_TOP
                      260 JUMP_FORWARD            11 (to 284)
                  >>  262 PUSH_EXC_INFO
@@ -1032,15 +1032,15 @@
                      272 POP_EXCEPT
                      274 RERAISE                  1
                  >>  276 POP_TOP
                      278 POP_EXCEPT
                      280 POP_TOP
                      282 POP_TOP
          
-         143     >>  284 LOAD_FAST                2 (df)
+         144     >>  284 LOAD_FAST                2 (df)
                      286 RETURN_VALUE
          ExceptionTable:
            52 to 236 -> 262 [1] lasti
            262 to 268 -> 270 [3] lasti
            276 to 276 -> 270 [3] lasti
          consts
             None
@@ -1048,15 +1048,15 @@
             ('columns',)
          names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'search'
-         firstlineno 139
+         firstlineno 140
          lnotab 0x02013401440174fe2e03
       'advance'
       'search_uid'
       'last_event_type'
       code
          argcount  : 2
          nlocals   : 8
@@ -1078,59 +1078,59 @@
             030000ab0300000000000000007d057415000000000000000000007c00a6
             010000ab0100000000000000007d077c05a00b0000000000000000000000
             0000000000000000007c076a0c0000000000000000a00d00000000000000
             0000000000000000000000000064076404a6020000ab0200000000000000
             007c076a0c0000000000000000a00d000000000000000000000000000000
             00000000006408a6010000ab01000000000000000064096b0200000000ac
             0aa6020000ab0200000000000000007d057c055300
-         146           0 RESUME                   0
+         147           0 RESUME                   0
          
-         147           2 LOAD_GLOBAL              0 (engine)
+         148           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               2 (conn)
          
-         148          54 LOAD_CONST               1 ('SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type')
+         149          54 LOAD_CONST               1 ('SELECT * FROM target WHERE search_uid = :search_uid AND last_event_type = :last_event_type')
                       56 STORE_FAST               3 (statement)
          
-         149          58 LOAD_FAST                2 (conn)
+         150          58 LOAD_FAST                2 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         150          82 LOAD_GLOBAL              7 (NULL + text)
+         151          82 LOAD_GLOBAL              7 (NULL + text)
                       94 LOAD_FAST                3 (statement)
                       96 PRECALL                  1
                      100 CALL                     1
          
-         151         110 LOAD_FAST                0 (search_uid)
+         152         110 LOAD_FAST                0 (search_uid)
                      112 LOAD_FAST                1 (last_event_type)
                      114 LOAD_CONST               2 (('search_uid', 'last_event_type'))
                      116 BUILD_CONST_KEY_MAP      2
          
-         149         118 PRECALL                  2
+         150         118 PRECALL                  2
                      122 CALL                     2
                      132 STORE_FAST               4 (result)
          
-         153         134 LOAD_GLOBAL              9 (NULL + pd)
+         154         134 LOAD_GLOBAL              9 (NULL + pd)
                      146 LOAD_ATTR                5 (DataFrame)
                      156 LOAD_FAST                4 (result)
                      158 LOAD_METHOD              6 (fetchall)
                      180 PRECALL                  0
                      184 CALL                     0
                      194 LOAD_FAST                4 (result)
                      196 LOAD_METHOD              7 (keys)
                      218 PRECALL                  0
                      222 CALL                     0
                      232 KW_NAMES                 3
                      234 PRECALL                  2
                      238 CALL                     2
                      248 STORE_FAST               5 (targets)
          
-         147         250 LOAD_CONST               0 (None)
+         148         250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 LOAD_CONST               0 (None)
                      256 PRECALL                  2
                      260 CALL                     2
                      270 POP_TOP
                      272 JUMP_FORWARD            11 (to 296)
                  >>  274 PUSH_EXC_INFO
@@ -1141,62 +1141,62 @@
                      284 POP_EXCEPT
                      286 RERAISE                  1
                  >>  288 POP_TOP
                      290 POP_EXCEPT
                      292 POP_TOP
                      294 POP_TOP
          
-         155     >>  296 LOAD_GLOBAL             17 (NULL + comment_by_domain)
+         156     >>  296 LOAD_GLOBAL             17 (NULL + comment_by_domain)
                      308 LOAD_FAST                0 (search_uid)
                      310 PRECALL                  1
                      314 CALL                     1
                      324 STORE_FAST               6 (comments)
          
-         156         326 LOAD_FAST                5 (targets)
+         157         326 LOAD_FAST                5 (targets)
                      328 LOAD_METHOD              9 (merge)
                      350 LOAD_FAST                6 (comments)
                      352 LOAD_CONST               4 ('domain')
                      354 LOAD_CONST               5 ('left')
                      356 KW_NAMES                 6
                      358 PRECALL                  3
                      362 CALL                     3
                      372 STORE_FAST               5 (targets)
          
-         160         374 LOAD_GLOBAL             21 (NULL + find_search_by_uid)
+         161         374 LOAD_GLOBAL             21 (NULL + find_search_by_uid)
                      386 LOAD_FAST                0 (search_uid)
                      388 PRECALL                  1
                      392 CALL                     1
                      402 STORE_FAST               7 (search)
          
-         161         404 LOAD_FAST                5 (targets)
+         162         404 LOAD_FAST                5 (targets)
                      406 LOAD_METHOD             11 (sort_values)
          
-         162         428 LOAD_FAST                7 (search)
+         163         428 LOAD_FAST                7 (search)
                      430 LOAD_ATTR               12 (sort)
                      440 LOAD_METHOD             13 (get)
                      462 LOAD_CONST               7 ('field')
                      464 LOAD_CONST               4 ('domain')
                      466 PRECALL                  2
                      470 CALL                     2
          
-         163         480 LOAD_FAST                7 (search)
+         164         480 LOAD_FAST                7 (search)
                      482 LOAD_ATTR               12 (sort)
                      492 LOAD_METHOD             13 (get)
                      514 LOAD_CONST               8 ('order')
                      516 PRECALL                  1
                      520 CALL                     1
                      530 LOAD_CONST               9 ('asc')
                      532 COMPARE_OP               2 (==)
          
-         161         538 KW_NAMES                10
+         162         538 KW_NAMES                10
                      540 PRECALL                  2
                      544 CALL                     2
                      554 STORE_FAST               5 (targets)
          
-         167         556 LOAD_FAST                5 (targets)
+         168         556 LOAD_FAST                5 (targets)
                      558 RETURN_VALUE
          ExceptionTable:
            52 to 248 -> 274 [1] lasti
            274 to 280 -> 282 [3] lasti
            288 to 288 -> 282 [3] lasti
          consts
             None
@@ -1212,15 +1212,15 @@
             ('by', 'ascending')
          names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'comment_by_domain', 'merge', 'find_search_by_uid', 'sort_values', 'sort', 'get')
          varnames   ('search_uid', 'last_event_type', 'conn', 'statement', 'result', 'targets', 'comments', 'search')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target'
-         firstlineno 146
+         firstlineno 147
          lnotab
             0x02013401040118011c0108fe100474fa2e081e0130041e01180134013a
             fe1206
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
@@ -1232,58 +1232,58 @@
             00000000007c02a6010000ab01000000000000000064027c006901a60200
             00ab0200000000000000007d037409000000000000000000006a05000000
             00000000007c03a0060000000000000000000000000000000000000000a6
             000000ab0000000000000000007c03a00700000000000000000000000000
             00000000000000a6000000ab000000000000000000ac03a6020000ab0200
             000000000000007d04640064006400a6020000ab02000000000000000001
             006e0b230031007304770278035900770101005900010001007c045300
-         170           0 RESUME                   0
+         171           0 RESUME                   0
          
-         171           2 LOAD_GLOBAL              0 (engine)
+         172           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         172          54 LOAD_CONST               1 ('\n                SELECT last_event_type, count(*)\n                FROM target\n                WHERE search_uid = :search_uid\n                GROUP BY last_event_type\n            ')
+         173          54 LOAD_CONST               1 ('\n                SELECT last_event_type, count(*)\n                FROM target\n                WHERE search_uid = :search_uid\n                GROUP BY last_event_type\n            ')
                       56 STORE_FAST               2 (statement)
          
-         178          58 LOAD_FAST                1 (conn)
+         179          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         179          82 LOAD_GLOBAL              7 (NULL + text)
+         180          82 LOAD_GLOBAL              7 (NULL + text)
                       94 LOAD_FAST                2 (statement)
                       96 PRECALL                  1
                      100 CALL                     1
          
-         180         110 LOAD_CONST               2 ('search_uid')
+         181         110 LOAD_CONST               2 ('search_uid')
                      112 LOAD_FAST                0 (search_uid)
                      114 BUILD_MAP                1
          
-         178         116 PRECALL                  2
+         179         116 PRECALL                  2
                      120 CALL                     2
                      130 STORE_FAST               3 (result)
          
-         182         132 LOAD_GLOBAL              9 (NULL + pd)
+         183         132 LOAD_GLOBAL              9 (NULL + pd)
                      144 LOAD_ATTR                5 (DataFrame)
                      154 LOAD_FAST                3 (result)
                      156 LOAD_METHOD              6 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                3 (result)
                      194 LOAD_METHOD              7 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 3
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               4 (df)
          
-         171         248 LOAD_CONST               0 (None)
+         172         248 LOAD_CONST               0 (None)
                      250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 PRECALL                  2
                      258 CALL                     2
                      268 POP_TOP
                      270 JUMP_FORWARD            11 (to 294)
                  >>  272 PUSH_EXC_INFO
@@ -1294,15 +1294,15 @@
                      282 POP_EXCEPT
                      284 RERAISE                  1
                  >>  286 POP_TOP
                      288 POP_EXCEPT
                      290 POP_TOP
                      292 POP_TOP
          
-         183     >>  294 LOAD_FAST                4 (df)
+         184     >>  294 LOAD_FAST                4 (df)
                      296 RETURN_VALUE
          ExceptionTable:
            52 to 246 -> 272 [1] lasti
            272 to 278 -> 280 [3] lasti
            286 to 286 -> 280 [3] lasti
          consts
             None
@@ -1311,15 +1311,15 @@
             ('columns',)
          names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'target_count'
-         firstlineno 170
+         firstlineno 171
          lnotab 0x02013401040618011c0106fe100474f52e0c
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -1329,55 +1329,55 @@
             00000000007c02a6010000ab01000000000000000064027c006901a60200
             00ab0200000000000000007d037409000000000000000000006a05000000
             00000000007c03a0060000000000000000000000000000000000000000a6
             000000ab0000000000000000007c03a00700000000000000000000000000
             00000000000000a6000000ab000000000000000000ac03a6020000ab0200
             000000000000007d04640064006400a6020000ab02000000000000000001
             006e0b230031007304770278035900770101005900010001007c045300
-         186           0 RESUME                   0
+         187           0 RESUME                   0
          
-         187           2 LOAD_GLOBAL              0 (engine)
+         188           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         188          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
+         189          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM event\n                WHERE search_uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         193          58 LOAD_FAST                1 (conn)
+         194          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + text)
                       94 LOAD_FAST                2 (statement)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 LOAD_CONST               2 ('search_uid')
                      112 LOAD_FAST                0 (search_uid)
                      114 BUILD_MAP                1
                      116 PRECALL                  2
                      120 CALL                     2
                      130 STORE_FAST               3 (result)
          
-         194         132 LOAD_GLOBAL              9 (NULL + pd)
+         195         132 LOAD_GLOBAL              9 (NULL + pd)
                      144 LOAD_ATTR                5 (DataFrame)
                      154 LOAD_FAST                3 (result)
                      156 LOAD_METHOD              6 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                3 (result)
                      194 LOAD_METHOD              7 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 3
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               4 (df)
          
-         187         248 LOAD_CONST               0 (None)
+         188         248 LOAD_CONST               0 (None)
                      250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 PRECALL                  2
                      258 CALL                     2
                      268 POP_TOP
                      270 JUMP_FORWARD            11 (to 294)
                  >>  272 PUSH_EXC_INFO
@@ -1388,15 +1388,15 @@
                      282 POP_EXCEPT
                      284 RERAISE                  1
                  >>  286 POP_TOP
                      288 POP_EXCEPT
                      290 POP_TOP
                      292 POP_TOP
          
-         195     >>  294 LOAD_FAST                4 (df)
+         196     >>  294 LOAD_FAST                4 (df)
                      296 RETURN_VALUE
          ExceptionTable:
            52 to 246 -> 272 [1] lasti
            272 to 278 -> 280 [3] lasti
            286 to 286 -> 280 [3] lasti
          consts
             None
@@ -1405,15 +1405,15 @@
             ('columns',)
          names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'event'
-         firstlineno 186
+         firstlineno 187
          lnotab 0x0201340104054a0174f92e08
       code
          argcount  : 0
          nlocals   : 4
          stacksize : 6
          flags     : 3
          code
@@ -1423,52 +1423,52 @@
             00000000007c01a6010000ab010000000000000000a6010000ab01000000
             00000000007d027409000000000000000000006a0500000000000000007c
             02a0060000000000000000000000000000000000000000a6000000ab0000
             000000000000007c02a00700000000000000000000000000000000000000
             00a6000000ab000000000000000000ac02a6020000ab0200000000000000
             007d03640064006400a6020000ab02000000000000000001006e0b230031
             007304770278035900770101005900010001007c035300
-         198           0 RESUME                   0
+         199           0 RESUME                   0
          
-         199           2 LOAD_GLOBAL              0 (engine)
+         200           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               0 (conn)
          
-         200          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n            ')
+         201          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM checkpoint\n            ')
                       56 STORE_FAST               1 (statement)
          
-         204          58 LOAD_FAST                0 (conn)
+         205          58 LOAD_FAST                0 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + text)
                       94 LOAD_FAST                1 (statement)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 PRECALL                  1
                      114 CALL                     1
                      124 STORE_FAST               2 (result)
          
-         205         126 LOAD_GLOBAL              9 (NULL + pd)
+         206         126 LOAD_GLOBAL              9 (NULL + pd)
                      138 LOAD_ATTR                5 (DataFrame)
                      148 LOAD_FAST                2 (result)
                      150 LOAD_METHOD              6 (fetchall)
                      172 PRECALL                  0
                      176 CALL                     0
                      186 LOAD_FAST                2 (result)
                      188 LOAD_METHOD              7 (keys)
                      210 PRECALL                  0
                      214 CALL                     0
                      224 KW_NAMES                 2
                      226 PRECALL                  2
                      230 CALL                     2
                      240 STORE_FAST               3 (df)
          
-         199         242 LOAD_CONST               0 (None)
+         200         242 LOAD_CONST               0 (None)
                      244 LOAD_CONST               0 (None)
                      246 LOAD_CONST               0 (None)
                      248 PRECALL                  2
                      252 CALL                     2
                      262 POP_TOP
                      264 JUMP_FORWARD            11 (to 288)
                  >>  266 PUSH_EXC_INFO
@@ -1479,15 +1479,15 @@
                      276 POP_EXCEPT
                      278 RERAISE                  1
                  >>  280 POP_TOP
                      282 POP_EXCEPT
                      284 POP_TOP
                      286 POP_TOP
          
-         206     >>  288 LOAD_FAST                3 (df)
+         207     >>  288 LOAD_FAST                3 (df)
                      290 RETURN_VALUE
          ExceptionTable:
            52 to 240 -> 266 [1] lasti
            266 to 272 -> 274 [3] lasti
            280 to 280 -> 274 [3] lasti
          consts
             None
@@ -1495,15 +1495,15 @@
             ('columns',)
          names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys')
          varnames   ('conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'checkpoint'
-         firstlineno 198
+         firstlineno 199
          lnotab 0x020134010404440174fa2e07
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 6
          flags     : 3
          code
@@ -1517,58 +1517,58 @@
             00000000000000a6000000ab000000000000000000ac03a6020000ab0200
             000000000000007d04640064006400a6020000ab02000000000000000001
             006e0b230031007304770278035900770101005900010001007c04a00800
             000000000000000000000000000000000000006404a6010000ab01000000
             0000000000a0090000000000000000000000000000000000000000640564
             0684006901a6010000ab010000000000000000a00a000000000000000000
             0000000000000000000000a6000000ab0000000000000000005300
-         209           0 RESUME                   0
+         210           0 RESUME                   0
          
-         210           2 LOAD_GLOBAL              0 (engine)
+         211           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         211          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
+         212          54 LOAD_CONST               1 ("\n                SELECT *, data->>'comment' AS comment\n                FROM event e\n                WHERE \n                    search_uid = :search_uid AND\n                    type = 'comment'\n            ")
                       56 STORE_FAST               2 (statement)
          
-         218          58 LOAD_FAST                1 (conn)
+         219          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         219          82 LOAD_GLOBAL              7 (NULL + text)
+         220          82 LOAD_GLOBAL              7 (NULL + text)
                       94 LOAD_FAST                2 (statement)
                       96 PRECALL                  1
                      100 CALL                     1
          
-         220         110 LOAD_CONST               2 ('search_uid')
+         221         110 LOAD_CONST               2 ('search_uid')
                      112 LOAD_FAST                0 (search_uid)
                      114 BUILD_MAP                1
          
-         218         116 PRECALL                  2
+         219         116 PRECALL                  2
                      120 CALL                     2
                      130 STORE_FAST               3 (result)
          
-         222         132 LOAD_GLOBAL              9 (NULL + pd)
+         223         132 LOAD_GLOBAL              9 (NULL + pd)
                      144 LOAD_ATTR                5 (DataFrame)
                      154 LOAD_FAST                3 (result)
                      156 LOAD_METHOD              6 (fetchall)
                      178 PRECALL                  0
                      182 CALL                     0
                      192 LOAD_FAST                3 (result)
                      194 LOAD_METHOD              7 (keys)
                      216 PRECALL                  0
                      220 CALL                     0
                      230 KW_NAMES                 3
                      232 PRECALL                  2
                      236 CALL                     2
                      246 STORE_FAST               4 (df)
          
-         210         248 LOAD_CONST               0 (None)
+         211         248 LOAD_CONST               0 (None)
                      250 LOAD_CONST               0 (None)
                      252 LOAD_CONST               0 (None)
                      254 PRECALL                  2
                      258 CALL                     2
                      268 POP_TOP
                      270 JUMP_FORWARD            11 (to 294)
                  >>  272 PUSH_EXC_INFO
@@ -1579,22 +1579,22 @@
                      282 POP_EXCEPT
                      284 RERAISE                  1
                  >>  286 POP_TOP
                      288 POP_EXCEPT
                      290 POP_TOP
                      292 POP_TOP
          
-         224     >>  294 LOAD_FAST                4 (df)
+         225     >>  294 LOAD_FAST                4 (df)
                      296 LOAD_METHOD              8 (groupby)
                      318 LOAD_CONST               4 ('domain')
                      320 PRECALL                  1
                      324 CALL                     1
                      334 LOAD_METHOD              9 (agg)
                      356 LOAD_CONST               5 ('comment')
-                     358 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 224>)
+                     358 LOAD_CONST               6 (<code object <lambda>, file "/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py", line 225>)
                      360 MAKE_FUNCTION            0
                      362 BUILD_MAP                1
                      364 PRECALL                  1
                      368 CALL                     1
                      378 LOAD_METHOD             10 (reset_index)
                      400 PRECALL                  0
                      404 CALL                     0
@@ -1614,37 +1614,37 @@
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 19
                code
                   0x97007401000000000000000000007c00a6010000ab0100000000000000
                   005300
-               224           0 RESUME                   0
+               225           0 RESUME                   0
                              2 LOAD_GLOBAL              1 (NULL + list)
                             14 LOAD_FAST                0 (x)
                             16 PRECALL                  1
                             20 CALL                     1
                             30 RETURN_VALUE
                consts
                   None
                names      ('list',)
                varnames   ('x',)
                freevars   ()
                cellvars   ()
                filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
                name       '<lambda>'
-               firstlineno 224
+               firstlineno 225
                lnotab 0x
          names      ('engine', 'connect', 'execute', 'text', 'pd', 'DataFrame', 'fetchall', 'keys', 'groupby', 'agg', 'reset_index')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'df')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'comment_by_domain'
-         firstlineno 209
+         firstlineno 210
          lnotab 0x02013401040718011c0106fe100474f42e0e
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
          code
@@ -1657,40 +1657,40 @@
             036a04000000000000000064036b0200000000720264005300740b000000
             00000000000000740d000000000000000000007c03a00700000000000000
             00000000000000000000000000a6000000ab0000000000000000007c03a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000a6020000ab020000000000000000a6010000ab010000000000
             0000007d047413000000000000000000007414000000000000000000007c
             04a6020000ab0200000000000000005300
-         230           0 RESUME                   0
+         231           0 RESUME                   0
          
-         231           2 LOAD_GLOBAL              0 (engine)
+         232           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         232          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
+         233          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM search\n                WHERE uid = :search_uid\n            ')
                       56 STORE_FAST               2 (statement)
          
-         237          58 LOAD_FAST                1 (conn)
+         238          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + text)
                       94 LOAD_FAST                2 (statement)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 LOAD_CONST               2 ('search_uid')
                      112 LOAD_FAST                0 (search_uid)
                      114 BUILD_MAP                1
                      116 PRECALL                  2
                      120 CALL                     2
                      130 STORE_FAST               3 (result)
          
-         231         132 LOAD_CONST               0 (None)
+         232         132 LOAD_CONST               0 (None)
                      134 LOAD_CONST               0 (None)
                      136 LOAD_CONST               0 (None)
                      138 PRECALL                  2
                      142 CALL                     2
                      152 POP_TOP
                      154 JUMP_FORWARD            11 (to 178)
                  >>  156 PUSH_EXC_INFO
@@ -1701,24 +1701,24 @@
                      166 POP_EXCEPT
                      168 RERAISE                  1
                  >>  170 POP_TOP
                      172 POP_EXCEPT
                      174 POP_TOP
                      176 POP_TOP
          
-         239     >>  178 LOAD_FAST                3 (result)
+         240     >>  178 LOAD_FAST                3 (result)
                      180 LOAD_ATTR                4 (rowcount)
                      190 LOAD_CONST               3 (0)
                      192 COMPARE_OP               2 (==)
                      198 POP_JUMP_FORWARD_IF_FALSE     2 (to 204)
          
-         240         200 LOAD_CONST               0 (None)
+         241         200 LOAD_CONST               0 (None)
                      202 RETURN_VALUE
          
-         242     >>  204 LOAD_GLOBAL             11 (NULL + dict)
+         243     >>  204 LOAD_GLOBAL             11 (NULL + dict)
                      216 LOAD_GLOBAL             13 (NULL + zip)
                      228 LOAD_FAST                3 (result)
                      230 LOAD_METHOD              7 (keys)
                      252 PRECALL                  0
                      256 CALL                     0
                      266 LOAD_FAST                3 (result)
                      268 LOAD_METHOD              8 (fetchone)
@@ -1726,15 +1726,15 @@
                      294 CALL                     0
                      304 PRECALL                  2
                      308 CALL                     2
                      318 PRECALL                  1
                      322 CALL                     1
                      332 STORE_FAST               4 (obj)
          
-         243         334 LOAD_GLOBAL             19 (NULL + from_dict)
+         244         334 LOAD_GLOBAL             19 (NULL + from_dict)
                      346 LOAD_GLOBAL             20 (Search)
                      358 LOAD_FAST                4 (obj)
                      360 PRECALL                  2
                      364 CALL                     2
                      374 RETURN_VALUE
          ExceptionTable:
            52 to 130 -> 156 [1] lasti
@@ -1747,15 +1747,15 @@
             0
          names      ('engine', 'connect', 'execute', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Search')
          varnames   ('search_uid', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_search_by_uid'
-         firstlineno 230
+         firstlineno 231
          lnotab 0x0201340104054afa2e08160104028201
       'domain'
       code
          argcount  : 1
          nlocals   : 5
          stacksize : 7
          flags     : 3
@@ -1769,40 +1769,40 @@
             036a04000000000000000064036b0200000000720264005300740b000000
             00000000000000740d000000000000000000007c03a00700000000000000
             00000000000000000000000000a6000000ab0000000000000000007c03a0
             080000000000000000000000000000000000000000a6000000ab00000000
             0000000000a6020000ab020000000000000000a6010000ab010000000000
             0000007d047413000000000000000000007414000000000000000000007c
             04a6020000ab0200000000000000005300
-         246           0 RESUME                   0
+         247           0 RESUME                   0
          
-         247           2 LOAD_GLOBAL              0 (engine)
+         248           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         248          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
+         249          54 LOAD_CONST               1 ('\n                SELECT *\n                FROM company\n                WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         253          58 LOAD_FAST                1 (conn)
+         254          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
                       82 LOAD_GLOBAL              7 (NULL + text)
                       94 LOAD_FAST                2 (statement)
                       96 PRECALL                  1
                      100 CALL                     1
                      110 LOAD_CONST               2 ('domain')
                      112 LOAD_FAST                0 (domain)
                      114 BUILD_MAP                1
                      116 PRECALL                  2
                      120 CALL                     2
                      130 STORE_FAST               3 (result)
          
-         247         132 LOAD_CONST               0 (None)
+         248         132 LOAD_CONST               0 (None)
                      134 LOAD_CONST               0 (None)
                      136 LOAD_CONST               0 (None)
                      138 PRECALL                  2
                      142 CALL                     2
                      152 POP_TOP
                      154 JUMP_FORWARD            11 (to 178)
                  >>  156 PUSH_EXC_INFO
@@ -1813,24 +1813,24 @@
                      166 POP_EXCEPT
                      168 RERAISE                  1
                  >>  170 POP_TOP
                      172 POP_EXCEPT
                      174 POP_TOP
                      176 POP_TOP
          
-         255     >>  178 LOAD_FAST                3 (result)
+         256     >>  178 LOAD_FAST                3 (result)
                      180 LOAD_ATTR                4 (rowcount)
                      190 LOAD_CONST               3 (0)
                      192 COMPARE_OP               2 (==)
                      198 POP_JUMP_FORWARD_IF_FALSE     2 (to 204)
          
-         256         200 LOAD_CONST               0 (None)
+         257         200 LOAD_CONST               0 (None)
                      202 RETURN_VALUE
          
-         258     >>  204 LOAD_GLOBAL             11 (NULL + dict)
+         259     >>  204 LOAD_GLOBAL             11 (NULL + dict)
                      216 LOAD_GLOBAL             13 (NULL + zip)
                      228 LOAD_FAST                3 (result)
                      230 LOAD_METHOD              7 (keys)
                      252 PRECALL                  0
                      256 CALL                     0
                      266 LOAD_FAST                3 (result)
                      268 LOAD_METHOD              8 (fetchone)
@@ -1838,15 +1838,15 @@
                      294 CALL                     0
                      304 PRECALL                  2
                      308 CALL                     2
                      318 PRECALL                  1
                      322 CALL                     1
                      332 STORE_FAST               4 (obj)
          
-         259         334 LOAD_GLOBAL             19 (NULL + from_dict)
+         260         334 LOAD_GLOBAL             19 (NULL + from_dict)
                      346 LOAD_GLOBAL             20 (Company)
                      358 LOAD_FAST                4 (obj)
                      360 PRECALL                  2
                      364 CALL                     2
                      374 RETURN_VALUE
          ExceptionTable:
            52 to 130 -> 156 [1] lasti
@@ -1859,15 +1859,15 @@
             0
          names      ('engine', 'connect', 'execute', 'text', 'rowcount', 'dict', 'zip', 'keys', 'fetchone', 'from_dict', 'Company')
          varnames   ('domain', 'conn', 'statement', 'result', 'obj')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'find_company_by_domain'
-         firstlineno 246
+         firstlineno 247
          lnotab 0x0201340104054afa2e08160104028201
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 10
          flags     : 3
          code
@@ -1880,74 +1880,74 @@
             00a6010000ab01000000000000000064029c04a6020000ab020000000000
             00000001007c01a002000000000000000000000000000000000000000074
             07000000000000000000006403a6010000ab010000000000000000a60100
             00ab01000000000000000001007c01a00a00000000000000000000000000
             00000000000000a6000000ab0000000000000000000100640064006400a6
             020000ab0200000000000000000100640053002300310073047702780359
             007701010059000100010064005300
-         265           0 RESUME                   0
+         266           0 RESUME                   0
          
-         266           2 LOAD_GLOBAL              0 (engine)
+         267           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         267          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
+         268          54 LOAD_CONST               1 ('\n            UPDATE company\n            SET\n                name = :name,\n                description = :description,\n                meta = :meta\n            WHERE domain = :domain\n            ')
                       56 STORE_FAST               2 (statement)
          
-         276          58 LOAD_FAST                1 (conn)
+         277          58 LOAD_FAST                1 (conn)
                       60 LOAD_METHOD              2 (execute)
          
-         277          82 LOAD_GLOBAL              7 (NULL + text)
+         278          82 LOAD_GLOBAL              7 (NULL + text)
                       94 LOAD_FAST                2 (statement)
                       96 PRECALL                  1
                      100 CALL                     1
          
-         279         110 LOAD_FAST                0 (company)
+         280         110 LOAD_FAST                0 (company)
                      112 LOAD_ATTR                4 (name)
          
-         280         122 LOAD_FAST                0 (company)
+         281         122 LOAD_FAST                0 (company)
                      124 LOAD_ATTR                5 (description)
          
-         281         134 LOAD_FAST                0 (company)
+         282         134 LOAD_FAST                0 (company)
                      136 LOAD_ATTR                6 (domain)
          
-         282         146 LOAD_GLOBAL             15 (NULL + json)
+         283         146 LOAD_GLOBAL             15 (NULL + json)
                      158 LOAD_ATTR                8 (dumps)
                      168 LOAD_FAST                0 (company)
                      170 LOAD_ATTR                9 (meta)
                      180 PRECALL                  1
                      184 CALL                     1
          
-         278         194 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
+         279         194 LOAD_CONST               2 (('name', 'description', 'domain', 'meta'))
                      196 BUILD_CONST_KEY_MAP      4
          
-         276         198 PRECALL                  2
+         277         198 PRECALL                  2
                      202 CALL                     2
                      212 POP_TOP
          
-         285         214 LOAD_FAST                1 (conn)
+         286         214 LOAD_FAST                1 (conn)
                      216 LOAD_METHOD              2 (execute)
                      238 LOAD_GLOBAL              7 (NULL + text)
                      250 LOAD_CONST               3 ('REFRESH MATERIALIZED VIEW target')
                      252 PRECALL                  1
                      256 CALL                     1
                      266 PRECALL                  1
                      270 CALL                     1
                      280 POP_TOP
          
-         286         282 LOAD_FAST                1 (conn)
+         287         282 LOAD_FAST                1 (conn)
                      284 LOAD_METHOD             10 (commit)
                      306 PRECALL                  0
                      310 CALL                     0
                      320 POP_TOP
          
-         266         322 LOAD_CONST               0 (None)
+         267         322 LOAD_CONST               0 (None)
                      324 LOAD_CONST               0 (None)
                      326 LOAD_CONST               0 (None)
                      328 PRECALL                  2
                      332 CALL                     2
                      342 POP_TOP
                      344 LOAD_CONST               0 (None)
                      346 RETURN_VALUE
@@ -1975,15 +1975,15 @@
             'REFRESH MATERIALIZED VIEW target'
          names      ('engine', 'connect', 'execute', 'text', 'name', 'description', 'domain', 'json', 'dumps', 'meta', 'commit')
          varnames   ('company', 'conn', 'statement')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_company'
-         firstlineno 265
+         firstlineno 266
          lnotab 0x02013401040918011c020c010c010c0130fc04fe1009440128ec
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 9
          flags     : 3
          code
@@ -1996,71 +1996,71 @@
             070000000000000000a6010000ab01000000000000000074090000000000
             00000000006a0500000000000000007c006a080000000000000000a60100
             00ab0100000000000000007c006a09000000000000000064029c04a60200
             00ab02000000000000000001007c01a00a00000000000000000000000000
             00000000000000a6000000ab0000000000000000000100640064006400a6
             020000ab0200000000000000000100640053002300310073047702780359
             007701010059000100010064005300
-         289           0 RESUME                   0
+         290           0 RESUME                   0
          
-         290           2 LOAD_GLOBAL              0 (engine)
+         291           2 LOAD_GLOBAL              0 (engine)
                       14 LOAD_METHOD              1 (connect)
                       36 PRECALL                  0
                       40 CALL                     0
                       50 BEFORE_WITH
                       52 STORE_FAST               1 (conn)
          
-         291          54 LOAD_FAST                1 (conn)
+         292          54 LOAD_FAST                1 (conn)
                       56 LOAD_METHOD              2 (execute)
          
-         292          78 LOAD_GLOBAL              7 (NULL + text)
+         293          78 LOAD_GLOBAL              7 (NULL + text)
          
-         293          90 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
+         294          90 LOAD_CONST               1 ('\n                UPDATE search\n                SET\n                    sort = :sort,\n                    inclusion = :inclusion,\n                    exclusion = :exclusion\n                WHERE uid = :uid\n                ')
          
-         292          92 PRECALL                  1
+         293          92 PRECALL                  1
                       96 CALL                     1
          
-         303         106 LOAD_GLOBAL              9 (NULL + json)
+         304         106 LOAD_GLOBAL              9 (NULL + json)
                      118 LOAD_ATTR                5 (dumps)
                      128 LOAD_FAST                0 (search)
                      130 LOAD_ATTR                6 (sort)
                      140 PRECALL                  1
                      144 CALL                     1
          
-         304         154 LOAD_GLOBAL              9 (NULL + json)
+         305         154 LOAD_GLOBAL              9 (NULL + json)
                      166 LOAD_ATTR                5 (dumps)
                      176 LOAD_FAST                0 (search)
                      178 LOAD_ATTR                7 (inclusion)
                      188 PRECALL                  1
                      192 CALL                     1
          
-         305         202 LOAD_GLOBAL              9 (NULL + json)
+         306         202 LOAD_GLOBAL              9 (NULL + json)
                      214 LOAD_ATTR                5 (dumps)
                      224 LOAD_FAST                0 (search)
                      226 LOAD_ATTR                8 (exclusion)
                      236 PRECALL                  1
                      240 CALL                     1
          
-         306         250 LOAD_FAST                0 (search)
+         307         250 LOAD_FAST                0 (search)
                      252 LOAD_ATTR                9 (uid)
          
-         302         262 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
+         303         262 LOAD_CONST               2 (('sort', 'inclusion', 'exclusion', 'uid'))
                      264 BUILD_CONST_KEY_MAP      4
          
-         291         266 PRECALL                  2
+         292         266 PRECALL                  2
                      270 CALL                     2
                      280 POP_TOP
          
-         309         282 LOAD_FAST                1 (conn)
+         310         282 LOAD_FAST                1 (conn)
                      284 LOAD_METHOD             10 (commit)
                      306 PRECALL                  0
                      310 CALL                     0
                      320 POP_TOP
          
-         290         322 LOAD_CONST               0 (None)
+         291         322 LOAD_CONST               0 (None)
                      324 LOAD_CONST               0 (None)
                      326 LOAD_CONST               0 (None)
                      328 PRECALL                  2
                      332 CALL                     2
                      342 POP_TOP
                      344 LOAD_CONST               0 (None)
                      346 RETURN_VALUE
@@ -2087,20 +2087,20 @@
             ('sort', 'inclusion', 'exclusion', 'uid')
          names      ('engine', 'connect', 'execute', 'text', 'json', 'dumps', 'sort', 'inclusion', 'exclusion', 'uid', 'commit')
          varnames   ('search', 'conn')
          freevars   ()
          cellvars   ()
          filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
          name       'update_search'
-         firstlineno 289
+         firstlineno 290
          lnotab 0x0201340118010c0102ff0e0b3001300130010cfc04f5101228ed
       ('advance',)
    names      ('json', 'pandas', 'pd', 'dataclasses', 'asdict', 'dacite', 'from_dict', 'gandai.models', 'Event', 'Company', 'EventType', 'Actor', 'Search', 'Checkpoint', 'os', 'sqlalchemy', 'text', 'google.cloud.sql.connector', 'Connector', 'dotenv', 'load_dotenv', 'get_engine', 'engine', 'insert_company', 'insert_event', 'insert_actor', 'insert_search', 'insert_checkpoint', 'search', 'int', 'str', 'target', 'DataFrame', 'target_count', 'event', 'checkpoint', 'comment_by_domain', 'find_search_by_uid', 'find_company_by_domain', 'update_company', 'update_search')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/Users/parker/Development/gandai-workspace/repo/src/gandai/query.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010c010c01200a080108010c010c010c021403061814
+      0x00ff0201080108010c010c01200a080108010c010c010c021403061914
       060c0e1015100f10131010060712181a101a0c160b1a15101010131018
```

### Comparing `gandai-1.1.1/gandai/__pycache__/services.cpython-311.pyc` & `gandai-1.1.2/gandai/__pycache__/services.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/__pycache__/sources.cpython-311.pyc` & `gandai-1.1.2/gandai/__pycache__/sources.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc` & `gandai-1.1.2/gandai/adapters/__pycache__/dealcloud.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/adapters/__pycache__/filters.cpython-311.pyc` & `gandai-1.1.2/gandai/adapters/__pycache__/filters.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/adapters/__pycache__/grata.cpython-311.pyc` & `gandai-1.1.2/gandai/adapters/__pycache__/grata.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/adapters/dealcloud.py` & `gandai-1.1.2/gandai/adapters/dealcloud.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/adapters/filters.py` & `gandai-1.1.2/gandai/adapters/filters.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/adapters/grata.py` & `gandai-1.1.2/gandai/adapters/grata.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/auth.py` & `gandai-1.1.2/gandai/auth.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/datastore.py` & `gandai-1.1.2/gandai/datastore.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/main.py` & `gandai-1.1.2/gandai/main.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/migrations/create_db.sql` & `gandai-1.1.2/gandai/migrations/create_db.sql`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/migrations/dealcloud_to_gandai.py` & `gandai-1.1.2/gandai/migrations/dealcloud_to_gandai.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/models.py` & `gandai-1.1.2/gandai/models.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai/query.py` & `gandai-1.1.2/gandai/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     print(os.getenv("ENV_STAGE"))
     if os.getenv("ENV_STAGE") == "local":
         DB_URI = "postgresql://postgres@localhost/parker"
         return sqlalchemy.create_engine(DB_URI)
     elif os.getenv("ENV_STAGE") == "dev":
         
         connector = Connector()
+        
         def getconn():
             conn = connector.connect(
                 os.getenv("INSTANCE_CONNECTION_NAME"),
                 "pg8000",
                 user=os.getenv("DB_USER"),
                 password=os.getenv("DB_PASS"),
                 db=os.getenv("DB_NAME"),
```

### Comparing `gandai-1.1.1/gandai/sources.py` & `gandai-1.1.2/gandai/sources.py`

 * *Files identical despite different names*

### Comparing `gandai-1.1.1/gandai.egg-info/SOURCES.txt` & `gandai-1.1.2/gandai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

