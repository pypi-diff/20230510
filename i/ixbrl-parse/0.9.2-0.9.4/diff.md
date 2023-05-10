# Comparing `tmp/ixbrl-parse-0.9.2.tar.gz` & `tmp/ixbrl-parse-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ixbrl-parse-0.9.2.tar", last modified: Wed May 19 12:59:10 2021, max compression
+gzip compressed data, was "ixbrl-parse-0.9.4.tar", last modified: Mon Oct 24 12:26:47 2022, max compression
```

## Comparing `ixbrl-parse-0.9.2.tar` & `ixbrl-parse-0.9.4.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2021-05-19 12:59:10.533225 ixbrl-parse-0.9.2/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4083 2021-05-19 12:59:10.533225 ixbrl-parse-0.9.2/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     2629 2021-05-19 12:57:30.000000 ixbrl-parse-0.9.2/README.md
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2021-05-19 12:59:10.532225 ixbrl-parse-0.9.2/ixbrl_parse/
--rw-rw-r--   0 mark      (1000) mark      (1000)      249 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.2/ixbrl_parse/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     1368 2021-05-19 10:28:06.000000 ixbrl-parse-0.9.2/ixbrl_parse/dataframe.py
--rw-rw-r--   0 mark      (1000) mark      (1000)    29144 2021-05-19 12:42:06.000000 ixbrl-parse-0.9.2/ixbrl_parse/ixbrl.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     4911 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.2/ixbrl_parse/schema.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     9433 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.2/ixbrl_parse/transform.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     2713 2021-05-19 12:52:09.000000 ixbrl-parse-0.9.2/ixbrl_parse/value.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2021-05-19 12:59:10.532225 ixbrl-parse-0.9.2/ixbrl_parse.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4083 2021-05-19 12:59:10.000000 ixbrl-parse-0.9.2/ixbrl_parse.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      528 2021-05-19 12:59:10.000000 ixbrl-parse-0.9.2/ixbrl_parse.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2021-05-19 12:59:10.000000 ixbrl-parse-0.9.2/ixbrl_parse.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       28 2021-05-19 12:59:10.000000 ixbrl-parse-0.9.2/ixbrl_parse.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)       12 2021-05-19 12:59:10.000000 ixbrl-parse-0.9.2/ixbrl_parse.egg-info/top_level.txt
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2021-05-19 12:59:10.533225 ixbrl-parse-0.9.2/scripts/
--rwxrwxr-x   0 mark      (1000) mark      (1000)     3529 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.2/scripts/ixbrl-diff
--rwxrwxr-x   0 mark      (1000) mark      (1000)     3705 2021-05-19 11:03:44.000000 ixbrl-parse-0.9.2/scripts/ixbrl-dump
--rwxr-xr-x   0 mark      (1000) mark      (1000)     2756 2021-05-19 09:30:13.000000 ixbrl-parse-0.9.2/scripts/ixbrl-markdown
--rwxrwxr-x   0 mark      (1000) mark      (1000)     4652 2021-05-19 11:02:54.000000 ixbrl-parse-0.9.2/scripts/ixbrl-report
--rwxrwxr-x   0 mark      (1000) mark      (1000)     1847 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.2/scripts/ixbrl-to-csv
--rwxrwxr-x   0 mark      (1000) mark      (1000)     1270 2021-05-19 12:54:05.000000 ixbrl-parse-0.9.2/scripts/ixbrl-to-json
--rwxrwxr-x   0 mark      (1000) mark      (1000)      950 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.2/scripts/ixbrl-to-kv
--rwxrwxr-x   0 mark      (1000) mark      (1000)      993 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.2/scripts/ixbrl-to-rdf
--rwxrwxr-x   0 mark      (1000) mark      (1000)     4613 2021-05-19 10:59:30.000000 ixbrl-parse-0.9.2/scripts/ixbrl-to-xbrl
--rw-rw-r--   0 mark      (1000) mark      (1000)       79 2021-05-19 12:59:10.534225 ixbrl-parse-0.9.2/setup.cfg
--rw-rw-r--   0 mark      (1000) mark      (1000)     1200 2021-05-19 12:58:37.000000 ixbrl-parse-0.9.2/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-24 12:26:47.853050 ixbrl-parse-0.9.4/
+-rw-rw-r--   0 mark      (1000) mark      (1000)    11357 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.4/LICENSE
+-rw-r--r--   0 mark      (1000) mark      (1000)     3246 2022-10-24 12:26:47.853050 ixbrl-parse-0.9.4/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2629 2021-05-19 12:57:30.000000 ixbrl-parse-0.9.4/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-24 12:26:47.851050 ixbrl-parse-0.9.4/ixbrl_parse/
+-rw-rw-r--   0 mark      (1000) mark      (1000)      249 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.4/ixbrl_parse/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1368 2021-05-19 10:28:06.000000 ixbrl-parse-0.9.4/ixbrl_parse/dataframe.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)    29968 2022-08-23 08:40:37.000000 ixbrl-parse-0.9.4/ixbrl_parse/ixbrl.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4911 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.4/ixbrl_parse/schema.py
+-rw-r--r--   0 mark      (1000) mark      (1000)    29616 2022-10-24 12:24:53.000000 ixbrl-parse-0.9.4/ixbrl_parse/transform.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     2713 2021-05-19 12:52:09.000000 ixbrl-parse-0.9.4/ixbrl_parse/value.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-24 12:26:47.852050 ixbrl-parse-0.9.4/ixbrl_parse.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     3246 2022-10-24 12:26:47.000000 ixbrl-parse-0.9.4/ixbrl_parse.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      536 2022-10-24 12:26:47.000000 ixbrl-parse-0.9.4/ixbrl_parse.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2022-10-24 12:26:47.000000 ixbrl-parse-0.9.4/ixbrl_parse.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       42 2022-10-24 12:26:47.000000 ixbrl-parse-0.9.4/ixbrl_parse.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)       12 2022-10-24 12:26:47.000000 ixbrl-parse-0.9.4/ixbrl_parse.egg-info/top_level.txt
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2022-10-24 12:26:47.853050 ixbrl-parse-0.9.4/scripts/
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     3529 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.4/scripts/ixbrl-diff
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     3705 2021-05-19 11:03:44.000000 ixbrl-parse-0.9.4/scripts/ixbrl-dump
+-rwxr-xr-x   0 mark      (1000) mark      (1000)     2756 2021-05-19 09:30:13.000000 ixbrl-parse-0.9.4/scripts/ixbrl-markdown
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     4652 2021-05-19 11:02:54.000000 ixbrl-parse-0.9.4/scripts/ixbrl-report
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     1847 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.4/scripts/ixbrl-to-csv
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     1270 2021-05-19 12:54:05.000000 ixbrl-parse-0.9.4/scripts/ixbrl-to-json
+-rwxrwxr-x   0 mark      (1000) mark      (1000)      950 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.4/scripts/ixbrl-to-kv
+-rwxrwxr-x   0 mark      (1000) mark      (1000)      993 2021-05-18 12:21:05.000000 ixbrl-parse-0.9.4/scripts/ixbrl-to-rdf
+-rwxrwxr-x   0 mark      (1000) mark      (1000)     4613 2021-05-19 10:59:30.000000 ixbrl-parse-0.9.4/scripts/ixbrl-to-xbrl
+-rw-rw-r--   0 mark      (1000) mark      (1000)       79 2022-10-24 12:26:47.853050 ixbrl-parse-0.9.4/setup.cfg
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1222 2022-10-24 12:26:13.000000 ixbrl-parse-0.9.4/setup.py
```

### Comparing `ixbrl-parse-0.9.2/README.md` & `ixbrl-parse-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/ixbrl_parse/dataframe.py` & `ixbrl-parse-0.9.4/ixbrl_parse/dataframe.py`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/ixbrl_parse/ixbrl.py` & `ixbrl-parse-0.9.4/ixbrl_parse/ixbrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -491,15 +491,17 @@
         if self.value:
             print("  Value:", self.value)
 
     @staticmethod
     def recurse_elts(elt, lower=False):
         a = ""
         if elt.text:
-            a += elt.text + " "
+            # This is probably right, but causes some things to appear wrong.
+            a += elt.text 
+#            a += elt.text + " "
         for s in elt:
             a += Value.recurse_elts(s, True)
         if lower and elt.tail:
             a += elt.tail
         return a
 
     def get_raw(self):
@@ -555,16 +557,17 @@
 
     def to_value(self):
         raw = self.get_raw()
         if hasattr(self, "format") and self.format:
             value = transform.transform(self, raw)
         else:
             if raw in { "nil", "None", "none", "", "no", "No" }: raw = 0
-            value = Float(float(raw) * self.scale, self.unit)
+            value = Float(float(raw) * self.scale * self.sign, self.unit)
         return value
+
     def to_dict(self, schema=None):
         ret = {
             "value": self.to_value().get_value()
         }
         if schema: ret["label"] = schema.get_label(self.name)
         if self.unit: ret["unit"] = str(self.unit)
         return ret
@@ -879,14 +882,36 @@
                 units[id] = unit
 
                 continue
 
             except:
                 pass
 
+            try:
+                div_elt = unit_elt.find("xbrli:divide", ns)
+                num_elt = div_elt.find(
+                    "./xbrli:unitnumerator/xbrli:measure", ns
+                )
+                den_elt = div_elt.find(
+                    "./xbrli:unitdenominator/xbrli:measure", ns
+                )
+
+                unit = Divide(
+                    Measure(to_qname(num_elt, num_elt.text)),
+                    Measure(to_qname(den_elt, den_elt.text))
+                )
+                unit.id = id
+
+                units[id] = unit
+
+                continue
+
+            except:
+                pass
+
             meas_elt = unit_elt.find("xbrli:measure", ns)
             units[id] = Measure(to_qname(meas_elt, meas_elt.text))
             units[id].id = id
 
         contexts = {}
 
         for ctxt_elt in doc.findall(".//xbrli:context", ns):
@@ -952,16 +977,15 @@
                 v.format = to_qname(elt, format)
 
             ctxt.values[name] = v
             values[key] = v
 
             while cont != None:
                 contelt = continuation[cont]
-                for s in contelt:
-                    v.elements.append(s)
+                v.elements.append(contelt)
                 cont = contelt.get("continuedAt")
 
         for elt in doc.findall(".//ix:nonFraction", ns):
             name = to_qname(elt, elt.get("name"))
             ctxt = contexts[elt.get("contextRef")]
             cont = elt.get("continuedAt")
             key = (ctxt, name)
@@ -974,14 +998,19 @@
 
             v = NonFraction()
             v.name = name
             v.context = ctxt
 
             v.decimals = elt.get("decimals")
 
+            if elt.get("sign") == "-":
+                v.sign = -1
+            else:
+                v.sign = 1
+
             format = elt.get("format")
             if format:
                 v.format = to_qname(elt, format)
             else:
                 v.format = None
 
             v.scale = scale
```

### Comparing `ixbrl-parse-0.9.2/ixbrl_parse/schema.py` & `ixbrl-parse-0.9.4/ixbrl_parse/schema.py`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/ixbrl_parse/value.py` & `ixbrl-parse-0.9.4/ixbrl_parse/value.py`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/ixbrl_parse.egg-info/SOURCES.txt` & `ixbrl-parse-0.9.4/ixbrl_parse.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 ixbrl_parse/__init__.py
 ixbrl_parse/dataframe.py
 ixbrl_parse/ixbrl.py
 ixbrl_parse/schema.py
```

### Comparing `ixbrl-parse-0.9.2/scripts/ixbrl-diff` & `ixbrl-parse-0.9.4/scripts/ixbrl-diff`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/scripts/ixbrl-dump` & `ixbrl-parse-0.9.4/scripts/ixbrl-dump`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/scripts/ixbrl-markdown` & `ixbrl-parse-0.9.4/scripts/ixbrl-markdown`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/scripts/ixbrl-report` & `ixbrl-parse-0.9.4/scripts/ixbrl-report`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/scripts/ixbrl-to-csv` & `ixbrl-parse-0.9.4/scripts/ixbrl-to-csv`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/scripts/ixbrl-to-json` & `ixbrl-parse-0.9.4/scripts/ixbrl-to-json`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/scripts/ixbrl-to-kv` & `ixbrl-parse-0.9.4/scripts/ixbrl-to-kv`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/scripts/ixbrl-to-rdf` & `ixbrl-parse-0.9.4/scripts/ixbrl-to-rdf`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/scripts/ixbrl-to-xbrl` & `ixbrl-parse-0.9.4/scripts/ixbrl-to-xbrl`

 * *Files identical despite different names*

### Comparing `ixbrl-parse-0.9.2/setup.py` & `ixbrl-parse-0.9.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ixbrl-parse",
-    version="0.9.2",
+    version="0.9.4",
     author="Cybermaggedon",
     author_email="mark@cyberapocalypse.co.uk",
     description="Parse iXBRL files, can present in RDF",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cybermaggedon/ixbrl-parse",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    download_url = "https://github.com/cybermaggedon/ixbrl-parse/archive/refs/tags/v0.9.2.tar.gz",
+    download_url = "https://github.com/cybermaggedon/ixbrl-parse/archive/refs/tags/v0.9.4.tar.gz",
     install_requires=[
         "number_parser",
         "requests",
-        "lxml"
+        "lxml",
+	"rdflib",
+	"pandas"
     ],
     scripts=[
         "scripts/ixbrl-dump",
         "scripts/ixbrl-report",
         "scripts/ixbrl-markdown",
         "scripts/ixbrl-to-rdf",
         "scripts/ixbrl-to-csv",
```

