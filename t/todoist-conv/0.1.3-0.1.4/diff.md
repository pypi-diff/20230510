# Comparing `tmp/todoist_conv-0.1.3.tar.gz` & `tmp/todoist_conv-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todoist_conv-0.1.3.tar", max compression
+gzip compressed data, was "todoist_conv-0.1.4.tar", max compression
```

## Comparing `todoist_conv-0.1.3.tar` & `todoist_conv-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      534 2023-02-01 22:54:25.501052 todoist_conv-0.1.3/README.md
--rw-r--r--   0        0        0      643 2023-02-14 21:08:52.865783 todoist_conv-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-07-28 04:59:54.457955 todoist_conv-0.1.3/todoist_conv/__init__.py
--rw-r--r--   0        0        0     1161 2023-01-17 21:33:38.036575 todoist_conv-0.1.3/todoist_conv/cli.py
--rw-r--r--   0        0        0      389 2023-01-17 04:20:41.863036 todoist_conv-0.1.3/todoist_conv/formats/__init__.py
--rw-r--r--   0        0        0      301 2023-01-17 21:33:43.584652 todoist_conv-0.1.3/todoist_conv/formats/base.py
--rw-r--r--   0        0        0      408 2023-01-31 03:18:46.997053 todoist_conv-0.1.3/todoist_conv/formats/csv/__init__.py
--rw-r--r--   0        0        0      569 2023-01-27 05:09:00.327681 todoist_conv-0.1.3/todoist_conv/formats/csv/common.py
--rw-r--r--   0        0        0     3252 2023-01-27 05:08:56.051683 todoist_conv-0.1.3/todoist_conv/formats/csv/parser.py
--rw-r--r--   0        0        0     2008 2023-02-05 21:10:50.265162 todoist_conv-0.1.3/todoist_conv/formats/csv/serializer.py
--rw-r--r--   0        0        0      370 2023-01-17 21:39:18.152833 todoist_conv-0.1.3/todoist_conv/formats/json.py
--rw-r--r--   0        0        0      379 2023-01-17 21:35:59.618537 todoist_conv-0.1.3/todoist_conv/formats/opml/__init__.py
--rw-r--r--   0        0        0     1414 2023-01-17 21:38:15.057469 todoist_conv-0.1.3/todoist_conv/formats/opml/parser.py
--rw-r--r--   0        0        0     1599 2023-01-17 04:08:41.498577 todoist_conv-0.1.3/todoist_conv/formats/opml/serializer.py
--rw-r--r--   0        0        0      754 2023-01-31 03:16:59.727085 todoist_conv-0.1.3/todoist_conv/model.py
--rw-r--r--   0        0        0      157 2023-01-17 21:33:18.404303 todoist_conv-0.1.3/todoist_conv/text.py
--rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 todoist_conv-0.1.3/setup.py
--rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 todoist_conv-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      534 2023-02-01 22:54:25.501052 todoist_conv-0.1.4/README.md
+-rw-r--r--   0        0        0      643 2023-05-10 00:57:13.930307 todoist_conv-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-07-28 04:59:54.457955 todoist_conv-0.1.4/todoist_conv/__init__.py
+-rw-r--r--   0        0        0     1161 2023-01-17 21:33:38.036575 todoist_conv-0.1.4/todoist_conv/cli.py
+-rw-r--r--   0        0        0      389 2023-01-17 04:20:41.863036 todoist_conv-0.1.4/todoist_conv/formats/__init__.py
+-rw-r--r--   0        0        0      301 2023-01-17 21:33:43.584652 todoist_conv-0.1.4/todoist_conv/formats/base.py
+-rw-r--r--   0        0        0      408 2023-01-31 03:18:46.997053 todoist_conv-0.1.4/todoist_conv/formats/csv/__init__.py
+-rw-r--r--   0        0        0      569 2023-01-27 05:09:00.327681 todoist_conv-0.1.4/todoist_conv/formats/csv/common.py
+-rw-r--r--   0        0        0     3252 2023-01-27 05:08:56.051683 todoist_conv-0.1.4/todoist_conv/formats/csv/parser.py
+-rw-r--r--   0        0        0     2008 2023-02-05 21:10:50.265162 todoist_conv-0.1.4/todoist_conv/formats/csv/serializer.py
+-rw-r--r--   0        0        0      370 2023-01-17 21:39:18.152833 todoist_conv-0.1.4/todoist_conv/formats/json.py
+-rw-r--r--   0        0        0      379 2023-01-17 21:35:59.618537 todoist_conv-0.1.4/todoist_conv/formats/opml/__init__.py
+-rw-r--r--   0        0        0     1439 2023-05-10 00:34:45.612655 todoist_conv-0.1.4/todoist_conv/formats/opml/parser.py
+-rw-r--r--   0        0        0     1644 2023-05-09 04:17:03.009899 todoist_conv-0.1.4/todoist_conv/formats/opml/serializer.py
+-rw-r--r--   0        0        0      754 2023-01-31 03:16:59.727085 todoist_conv-0.1.4/todoist_conv/model.py
+-rw-r--r--   0        0        0      157 2023-01-17 21:33:18.404303 todoist_conv-0.1.4/todoist_conv/text.py
+-rw-r--r--   0        0        0     1447 1970-01-01 00:00:00.000000 todoist_conv-0.1.4/setup.py
+-rw-r--r--   0        0        0     1158 1970-01-01 00:00:00.000000 todoist_conv-0.1.4/PKG-INFO
```

### Comparing `todoist_conv-0.1.3/README.md` & `todoist_conv-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `todoist_conv-0.1.3/pyproject.toml` & `todoist_conv-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "todoist-conv"
-version = "0.1.3"
+version = "0.1.4"
 description = "Convert Todoist generated CSVs to/from other formats"
 authors = ["Ygor Mutti <ygormutti@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 todoist-conv = 'todoist_conv.cli:cli'
```

### Comparing `todoist_conv-0.1.3/todoist_conv/cli.py` & `todoist_conv-0.1.4/todoist_conv/cli.py`

 * *Files identical despite different names*

### Comparing `todoist_conv-0.1.3/todoist_conv/formats/csv/common.py` & `todoist_conv-0.1.4/todoist_conv/formats/csv/common.py`

 * *Files identical despite different names*

### Comparing `todoist_conv-0.1.3/todoist_conv/formats/csv/parser.py` & `todoist_conv-0.1.4/todoist_conv/formats/csv/parser.py`

 * *Files identical despite different names*

### Comparing `todoist_conv-0.1.3/todoist_conv/formats/csv/serializer.py` & `todoist_conv-0.1.4/todoist_conv/formats/csv/serializer.py`

 * *Files identical despite different names*

### Comparing `todoist_conv-0.1.3/todoist_conv/formats/opml/parser.py` & `todoist_conv-0.1.4/todoist_conv/formats/opml/parser.py`

 * *Files 18% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     return sections
 
 
 def parse_tasks(task_elems: list[ET.Element]) -> list[Task]:
     tasks = []
     for task_elem in task_elems:
         subtasks = parse_tasks(get_children(task_elem))
-        task_json = task_elem.get("description")
+        task_json = task_elem.get("description") or task_elem.get("note")
         task = Task.parse_raw(task_json) if task_json else Task(name="", priority=4)
 
         task.name = get_name(task_elem)
         task.subtasks.extend(subtasks)
         tasks.append(task)
 
     return tasks
```

### Comparing `todoist_conv-0.1.3/todoist_conv/formats/opml/serializer.py` & `todoist_conv-0.1.4/todoist_conv/formats/opml/serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,15 @@
             build_task_outlines(section_outline, task)
 
 
 def build_outline(parent, text, description=None):
     outline = ET.SubElement(parent, "outline", text=text)
     if description:
         outline.attrib["description"] = description
+        outline.attrib["note"] = description
     return outline
 
 
 def build_task_outlines(parent: ET.Element, task: Task):
     task_elem = build_outline(
         parent, task.name, task.copy(exclude={"subtasks"}, deep=True).json()
     )
```

### Comparing `todoist_conv-0.1.3/todoist_conv/model.py` & `todoist_conv-0.1.4/todoist_conv/model.py`

 * *Files identical despite different names*

### Comparing `todoist_conv-0.1.3/setup.py` & `todoist_conv-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['chardet>=5.1.0,<6.0.0', 'click>=8.1.3,<9.0.0', 'pydantic>=1.9.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['todoist-conv = todoist_conv.cli:cli']}
 
 setup_kwargs = {
     'name': 'todoist-conv',
-    'version': '0.1.3',
+    'version': '0.1.4',
     'description': 'Convert Todoist generated CSVs to/from other formats',
     'long_description': '# todoist-conv\n\nConverts Todoist CSVs to/from other formats to integrate with other tools, like mind mappers.\n\n## Usage\n\n```shell\n$ todoist-conv --help\nUsage: todoist-conv [OPTIONS] FILE\n\n  Converts Todoist FILE from input_format to output_format\n\nOptions:\n  -i, --input-format [csv|opml|json]\n                                  [required]\n  -f, --output-format [csv|opml|json]\n                                  [required]\n  -o, --output-file FILE          [default: -]\n  --help                          Show this message and exit.\n```',
     'author': 'Ygor Mutti',
     'author_email': 'ygormutti@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `todoist_conv-0.1.3/PKG-INFO` & `todoist_conv-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: todoist-conv
-Version: 0.1.3
+Version: 0.1.4
 Summary: Convert Todoist generated CSVs to/from other formats
 License: MIT
 Author: Ygor Mutti
 Author-email: ygormutti@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

