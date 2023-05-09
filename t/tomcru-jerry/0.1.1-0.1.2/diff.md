# Comparing `tmp/tomcru_jerry-0.1.1.tar.gz` & `tmp/tomcru_jerry-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomcru_jerry-0.1.1.tar", max compression
+gzip compressed data, was "tomcru_jerry-0.1.2.tar", max compression
```

## Comparing `tomcru_jerry-0.1.1.tar` & `tomcru_jerry-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.1/LICENSE
--rw-r--r--   0        0        0      124 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.1/README.md
--rw-r--r--   0        0        0      391 2023-04-27 01:02:40.831876 tomcru_jerry-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1978 2023-04-17 23:54:18.705910 tomcru_jerry-0.1.1/tomcru_jerry/__init__.py
--rw-r--r--   0        0        0     3084 2023-04-25 23:25:52.640719 tomcru_jerry-0.1.1/tomcru_jerry/cli.py
--rw-r--r--   0        0        0     3859 2023-04-23 14:49:50.811637 tomcru_jerry-0.1.1/tomcru_jerry/controllers.py
--rw-r--r--   0        0        0     2422 2023-04-17 23:28:38.922059 tomcru_jerry-0.1.1/tomcru_jerry/flask_jerry.py
--rw-r--r--   0        0        0     3617 2023-04-17 23:34:56.509211 tomcru_jerry-0.1.1/tomcru_jerry/mockapi.py
--rw-r--r--   0        0        0     5494 2023-04-18 00:07:35.193927 tomcru_jerry-0.1.1/tomcru_jerry/static.py
--rw-r--r--   0        0        0     2268 2023-04-24 16:07:40.404928 tomcru_jerry-0.1.1/tomcru_jerry/utils.py
--rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 tomcru_jerry-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.2/LICENSE
+-rw-r--r--   0        0        0      124 2023-04-09 00:51:18.750203 tomcru_jerry-0.1.2/README.md
+-rw-r--r--   0        0        0      391 2023-05-09 23:35:50.014590 tomcru_jerry-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1978 2023-04-17 23:54:18.705910 tomcru_jerry-0.1.2/tomcru_jerry/__init__.py
+-rw-r--r--   0        0        0     3084 2023-04-25 23:25:52.640719 tomcru_jerry-0.1.2/tomcru_jerry/cli.py
+-rw-r--r--   0        0        0     3859 2023-04-23 14:49:50.811637 tomcru_jerry-0.1.2/tomcru_jerry/controllers.py
+-rw-r--r--   0        0        0     2422 2023-04-17 23:28:38.922059 tomcru_jerry-0.1.2/tomcru_jerry/flask_jerry.py
+-rw-r--r--   0        0        0     3874 2023-04-29 02:48:29.775134 tomcru_jerry-0.1.2/tomcru_jerry/mockapi.py
+-rw-r--r--   0        0        0     5556 2023-04-29 16:36:50.609598 tomcru_jerry-0.1.2/tomcru_jerry/static.py
+-rw-r--r--   0        0        0     2268 2023-04-24 16:07:40.404928 tomcru_jerry-0.1.2/tomcru_jerry/utils.py
+-rw-r--r--   0        0        0      576 1970-01-01 00:00:00.000000 tomcru_jerry-0.1.2/PKG-INFO
```

### Comparing `tomcru_jerry-0.1.1/LICENSE` & `tomcru_jerry-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.1/tomcru_jerry/__init__.py` & `tomcru_jerry-0.1.2/tomcru_jerry/__init__.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.1/tomcru_jerry/cli.py` & `tomcru_jerry-0.1.2/tomcru_jerry/cli.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.1/tomcru_jerry/controllers.py` & `tomcru_jerry-0.1.2/tomcru_jerry/controllers.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.1/tomcru_jerry/flask_jerry.py` & `tomcru_jerry-0.1.2/tomcru_jerry/flask_jerry.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.1/tomcru_jerry/mockapi.py` & `tomcru_jerry-0.1.2/tomcru_jerry/mockapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,51 +57,56 @@
         }
     if 'headers' not in resp:
         resp['headers'] = {'Content-Type': 'application/json'}
 
     p = re.compile(r'\{([^}]*)}')
 
     for container in ['body', 'headers']:
-        for key, transform in resp_tpl[container].items():
-            if isinstance(transform, str):
-                # subtitute request -> response transformations
-                groups = p.findall(transform)
-
-                if groups:
-                    res = transform
-
-                    for group in groups:
-                        to_find = str(group)
-                        if 'headers' == to_find.split('.')[0]:
-                            to_find = to_find.lower()
-
-                        if 'access_token' == to_find:
-                            try:
-                                _bearer, token = req['headers']['authorization'].split(' ')
-
-                                assert _bearer.lower() == 'bearer'
-                                if not token:
-                                    raise Exception("")
-                            except:
-                                return {"body": {}}, 403
-
-                            substitute = token
-                        elif 'url' == to_find:
-                            substitute = str(request.url_root)
-                        else:
-                            substitute = get_dict_hierarchy(req, to_find)
-                            #substitute = req.get(to_find)
-
-                        if f'{{{group}}}' == transform:
-                            # replace as-is (keeps type)
-                            if substitute is not None:
-                                res = substitute
-                                break
-                        else:
-                            # string template replace
-                            if substitute is not None:
-                                res = res.replace(f'{{{group}}}', str(substitute))
+        content = resp_tpl[container]
 
-                    if res is not None:
-                        resp[container][key] = res
+        if isinstance(content, dict):
+            for key, transform in content.items():
+                if isinstance(transform, str):
+                    # subtitute request -> response transformations
+                    groups = p.findall(transform)
+
+                    if groups:
+                        res = transform
+
+                        for group in groups:
+                            to_find = str(group)
+                            if 'headers' == to_find.split('.')[0]:
+                                to_find = to_find.lower()
+
+                            if 'access_token' == to_find:
+                                try:
+                                    _bearer, token = req['headers']['authorization'].split(' ')
+
+                                    assert _bearer.lower() == 'bearer'
+                                    if not token:
+                                        raise Exception("")
+                                except:
+                                    return {"body": {}}, 403
+
+                                substitute = token
+                            elif 'url' == to_find:
+                                substitute = str(request.url_root)
+                            else:
+                                substitute = get_dict_hierarchy(req, to_find)
+                                #substitute = req.get(to_find)
+
+                            if f'{{{group}}}' == transform:
+                                # replace as-is (keeps type)
+                                if substitute is not None:
+                                    res = substitute
+                                    break
+                            else:
+                                # string template replace
+                                if substitute is not None:
+                                    res = res.replace(f'{{{group}}}', str(substitute))
+
+                        if res is not None:
+                            resp[container][key] = res
+        else:
+            resp[container] = content
 
     return resp, status
```

### Comparing `tomcru_jerry-0.1.1/tomcru_jerry/static.py` & `tomcru_jerry-0.1.2/tomcru_jerry/static.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,26 +11,27 @@
 
 class RegexConverter(BaseConverter):
     def __init__(self, url_map, *items):
         super(RegexConverter, self).__init__(url_map)
         self.regex = items[0]
 
 
-class EmeStaticWebsite:
-    def __init__(self, index, path):
+class StaticWebsite:
+    def __init__(self, index, path, static_files):
 
         template_folder, static_folder = self.get_paths(path)
 
         self.index = index if index is not None else 'index.html'
         self.template_folder = template_folder if template_folder is not None else 'templates/'
         self.static_folder = static_folder if static_folder is not None else 'public/'
         self.template: jinja2.Template = None
         self.pyl: pynliner.Pynliner = None
         self.args = {}
         self.kept_styles = defaultdict(list)
+        self.static_files = static_files
 
     def get_paths(self, path='webapp'):
         template_folder = os.path.join(path, 'templates')
         static_folder = os.path.join(path, 'public')
 
         return template_folder,static_folder
 
@@ -62,15 +63,16 @@
         with open(fileto+'.html', 'w') as fh:
             fh.write(output)
 
     def build(self, **kwargs):
         # previews email in Flask (also uses Jinja2)
         self.app = Flask('', static_folder=self.static_folder, template_folder=self.template_folder)
         #self.app.url_map.converters['regex'] = RegexConverter
-        pattern = re.compile(r'(img/|js/|css/|fonts/).*')
+
+        pattern = re.compile('('+'|'.join(self.static_files)+'/).*')
 
         @self.app.route('/', defaults={'path': ''})
         @self.app.route('/<path:path>')
         def _index(path=None):
             if re.match(pattern, path):
                 return send_from_directory(self.static_folder, path)
 
@@ -80,15 +82,16 @@
 
         self.app.config['TEMPLATES_AUTO_RELOAD'] = True
         return self.app
 
     def run(self, *args, **kwargs):
         return self.app.run(*args, **kwargs)
 
-class Ememail(EmeStaticWebsite):
+
+class Ememail(StaticWebsite):
     def __init__(self, *args, **kwargs):
         super(Ememail, self).__init__(*args, **kwargs)
 
     def _parse_head(self):
         # removes all elements from head
         self.pyl._get_soup()
         soup: BeautifulSoup = self.pyl.soup
```

### Comparing `tomcru_jerry-0.1.1/tomcru_jerry/utils.py` & `tomcru_jerry-0.1.2/tomcru_jerry/utils.py`

 * *Files identical despite different names*

### Comparing `tomcru_jerry-0.1.1/PKG-INFO` & `tomcru_jerry-0.1.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomcru-jerry
-Version: 0.1.1
+Version: 0.1.2
 Summary: General purpose web library
 Author: Rajmund Csombordi
 Author-email: rajmund.csombordi@hotmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

