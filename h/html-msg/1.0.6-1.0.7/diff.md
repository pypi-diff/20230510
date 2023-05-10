# Comparing `tmp/html_msg-1.0.6.tar.gz` & `tmp/html_msg-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_msg-1.0.6.tar", last modified: Tue May  9 19:48:37 2023, max compression
+gzip compressed data, was "html_msg-1.0.7.tar", last modified: Wed May 10 21:48:51 2023, max compression
```

## Comparing `html_msg-1.0.6.tar` & `html_msg-1.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 19:48:37.768655 html_msg-1.0.6/
--rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0     3963 2023-05-09 19:48:37.767658 html_msg-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 19:48:37.756013 html_msg-1.0.6/html_msg/
--rw-rw-rw-   0        0        0      115 2023-05-09 19:47:47.000000 html_msg-1.0.6/html_msg/__init__.py
--rw-rw-rw-   0        0        0    12111 2023-05-09 17:31:43.000000 html_msg-1.0.6/html_msg/html_message.py
--rw-rw-rw-   0        0        0    14517 2023-05-09 19:00:47.000000 html_msg-1.0.6/html_msg/html_table.py
-drwxrwxrwx   0        0        0        0 2023-05-09 19:48:37.767658 html_msg-1.0.6/html_msg.egg-info/
--rw-rw-rw-   0        0        0     3963 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-09 19:48:37.000000 html_msg-1.0.6/html_msg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 19:48:37.768655 html_msg-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      824 2023-05-09 19:47:55.000000 html_msg-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:48:51.769281 html_msg-1.0.7/
+-rw-rw-rw-   0        0        0     1095 2023-05-06 11:32:57.000000 html_msg-1.0.7/LICENSE.txt
+-rw-rw-rw-   0        0        0     3965 2023-05-10 21:48:51.768284 html_msg-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3383 2023-05-09 19:29:44.000000 html_msg-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 21:48:51.756312 html_msg-1.0.7/html_msg/
+-rw-rw-rw-   0        0        0      115 2023-05-10 21:46:23.000000 html_msg-1.0.7/html_msg/__init__.py
+-rw-rw-rw-   0        0        0    12111 2023-05-09 17:31:43.000000 html_msg-1.0.7/html_msg/html_message.py
+-rw-rw-rw-   0        0        0    14803 2023-05-10 21:46:14.000000 html_msg-1.0.7/html_msg/html_table.py
+drwxrwxrwx   0        0        0        0 2023-05-10 21:48:51.768284 html_msg-1.0.7/html_msg.egg-info/
+-rw-rw-rw-   0        0        0     3965 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-10 21:48:51.000000 html_msg-1.0.7/html_msg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 21:48:51.769281 html_msg-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      823 2023-05-10 21:48:46.000000 html_msg-1.0.7/setup.py
```

### Comparing `html_msg-1.0.6/LICENSE.txt` & `html_msg-1.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.6/PKG-INFO` & `html_msg-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: html_msg
-Version: 1.0.6
-Summary: This tool allows to create HTML message via simple methods,      without the need to write HTML code manually.
+Version: 1.0.7
+Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
 Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Keywords: HTML,Message
 Description-Content-Type: text/markdown
```

### Comparing `html_msg-1.0.6/README.md` & `html_msg-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.6/html_msg/html_message.py` & `html_msg-1.0.7/html_msg/html_message.py`

 * *Files identical despite different names*

### Comparing `html_msg-1.0.6/html_msg/html_table.py` & `html_msg-1.0.7/html_msg/html_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         '''
         Sets the CSS style of the table.
         
         Note: Please note that this method sets the style of rows. 
               In order to set the style of headers, use method 'set_header_style'
 
         Args:
-            style (str): a string representing the CSS style.
+            style (str): a dictionary or a string representing the CSS style.
 
         Example:
             table = HTMLTable()
             table.set_table_style("border-collapse: collapse; padding: 5pt 5pt 5pt;")
         '''
         if type(style) == dict:
             self.table_style = self.generate_css_style(style)
@@ -206,22 +206,27 @@
     
     def set_header_style(self, style):
         
         '''
         Sets the CSS style of the table header.
 
         Args:
-            style (str): a string representing the CSS style.
+            style (dict or str): a dictionary or a string representing the CSS style.
 
         Example:
             table = HTMLTable()
             table.set_header_style("border: solid #E0E0E0 1.0pt; padding: 5pt 5pt 5pt;")
         '''
+        if type(style) == dict:
+            self.header_style = self.generate_css_style(style)
+        elif type(style) == str:
+            self.header_style = style
+        else:
+            raise ValueError(f'Parameter <style> must be either dictionary or string.')       
         
-        self.header_style = style
     
     def apply_design_preset(self, preset_name):
         
         '''
         Applies a pre-defined design preset to the table.
 
         Args:
```

### Comparing `html_msg-1.0.6/html_msg.egg-info/PKG-INFO` & `html_msg-1.0.7/html_msg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: html-msg
-Version: 1.0.6
-Summary: This tool allows to create HTML message via simple methods,      without the need to write HTML code manually.
+Version: 1.0.7
+Summary: This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.
 Home-page: https://github.com/Sirakan-B/html_msg/
 Download-URL: https://pypi.org/project/html-msg/
 Author: Sirakan Bagdasarian
 Author-email: bsirak@bk.ru
 License: MIT
 Keywords: HTML,Message
 Description-Content-Type: text/markdown
```

### Comparing `html_msg-1.0.6/setup.py` & `html_msg-1.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 
 
 setup_args = dict(
     name='html_msg',
-    version='1.0.6',
-    description='This tool allows to create HTML message via simple methods, \
-     without the need to write HTML code manually.',
+    version='1.0.7',
+    description='This tool allows you to create HTML messages using simple methods, without the need to write HTML code manually.',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n',
     license='MIT',
     packages=find_packages(),
     author='Sirakan Bagdasarian',
     author_email='bsirak@bk.ru',
     keywords=['HTML', 'Message'],
```

