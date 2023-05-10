# Comparing `tmp/oc_sql_helpers-1.0.0-py3-none-any.whl.zip` & `tmp/oc_sql_helpers-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 20017 bytes, number of entries: 9
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-14 09:28 oc_sql_helpers/__init__.py
--rw-r--r--  2.0 unx    34422 b- defN 23-Apr-14 09:28 oc_sql_helpers/normalizer.py
--rw-r--r--  2.0 unx     2802 b- defN 23-Apr-14 09:28 oc_sql_helpers/str_decoder.py
--rw-r--r--  2.0 unx    18181 b- defN 23-Apr-14 09:28 oc_sql_helpers/wrapper.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Apr-14 09:28 oc_sql_helpers-1.0.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      243 b- defN 23-Apr-14 09:28 oc_sql_helpers-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 09:28 oc_sql_helpers-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Apr-14 09:28 oc_sql_helpers-1.0.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      756 b- defN 23-Apr-14 09:28 oc_sql_helpers-1.0.0.dist-info/RECORD
-9 files, 67868 bytes uncompressed, 18707 bytes compressed:  72.4%
+Zip file size: 20127 bytes, number of entries: 9
+-rw-r--r--  2.0 unx        0 b- defN 23-May-10 11:47 oc_sql_helpers/__init__.py
+-rw-r--r--  2.0 unx    34675 b- defN 23-May-10 11:47 oc_sql_helpers/normalizer.py
+-rw-r--r--  2.0 unx     2802 b- defN 23-May-10 11:47 oc_sql_helpers/str_decoder.py
+-rw-r--r--  2.0 unx    18181 b- defN 23-May-10 11:47 oc_sql_helpers/wrapper.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-10 11:47 oc_sql_helpers-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx      243 b- defN 23-May-10 11:47 oc_sql_helpers-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-10 11:47 oc_sql_helpers-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-10 11:47 oc_sql_helpers-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      756 b- defN 23-May-10 11:47 oc_sql_helpers-1.0.1.dist-info/RECORD
+9 files, 68121 bytes uncompressed, 18817 bytes compressed:  72.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: oc_sql_helpers/str_decoder.py
 Comment: 
 
 Filename: oc_sql_helpers/wrapper.py
 Comment: 
 
-Filename: oc_sql_helpers-1.0.0.dist-info/LICENSE
+Filename: oc_sql_helpers-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: oc_sql_helpers-1.0.0.dist-info/METADATA
+Filename: oc_sql_helpers-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: oc_sql_helpers-1.0.0.dist-info/WHEEL
+Filename: oc_sql_helpers-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: oc_sql_helpers-1.0.0.dist-info/top_level.txt
+Filename: oc_sql_helpers-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: oc_sql_helpers-1.0.0.dist-info/RECORD
+Filename: oc_sql_helpers-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oc_sql_helpers/normalizer.py

```diff
@@ -67,15 +67,16 @@
             "wrapped": [{"start": re.compile(b'(\s|^)wrapped(\s|$)', flags=re.I)}]}
     # these objects are legal in any part of file
     # NOTE: national charset literals may be supported in wrong way by this implementation
     _re_objects_body={
             "object_name": [{"start": re.compile(b'"'), "end": re.compile(b'"')}],
             "literal":[
                 {"start": re.compile(b"q'(.)", flags=re.I), "end": b"%s'", 
-                    "substitutes": {b"[": b"\]", b"{": b"\}", b"<": b"\>", b"(": b"\)"}},
+                    "substitutes": {b"[": b"\]", b"{": b"\}", b"<": b"\>", b"(": b"\)", b"?": b"\?", b".": b"\.", b"^": b"\^", b"$": b"\$", b"\\": b"\\\\", b"*": b"\*",
+                        b"+": b"\+", b"|": b"\|"}},
                 {"start": re.compile(b"'", flags=re.I), "end": re.compile(b"'")}],
             "comment":[
                 {"start": re.compile(b'(\s|^)\-\-'), "end": re.compile(b'\n')},
                 {"start": re.compile(b'\/\*'), "end": re.compile(b'\*\/')}]}
 
     def _fl_full(self):
         """
@@ -754,16 +755,17 @@
         """
         General part of 'is_sql', 'is_wrapped', 'is_wrappable' methods
         """
         # create temporary file for normalization output
         _tmp = tempfile.NamedTemporaryFile(suffix='.tmpsql', mode='w+b')
         try:
             self.normalize(fl, self._fl_full() + [PLSQLNormalizationFlags.no_literals], write_to=_tmp)
-        except PLSQLNormalizationError as _e:
-            logging.exception(_e)
+        except (PLSQLNormalizationError, RecursionError) as _e:
+            # we do not need log these exceptions as exceptions - it is OK for all use cases
+            logging.debug(_e, exc_info=True)
             self._reset()
 
         _tmp.close()
 
     def is_wrapped_path(self, path):
         """
         Check if a file on given path is wrapped or not
```

## Comparing `oc_sql_helpers-1.0.0.dist-info/LICENSE` & `oc_sql_helpers-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `oc_sql_helpers-1.0.0.dist-info/RECORD` & `oc_sql_helpers-1.0.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 oc_sql_helpers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-oc_sql_helpers/normalizer.py,sha256=OECCJ6EdkF2THxREA0P7e7tO31jqgepAPh9APc3b93o,34422
+oc_sql_helpers/normalizer.py,sha256=yT7Rbe-vl0ec4oHQ6-oazv-41R5x1IIGfdhcZR41OL4,34675
 oc_sql_helpers/str_decoder.py,sha256=zt1fN07fkW55TmLm7Inb-5RTab7UaXiAjxBd-f5vMeU,2802
 oc_sql_helpers/wrapper.py,sha256=GJcu_iS7o9fjBLECv17U1IPecPVt9fy0m89KXWJKywQ,18181
-oc_sql_helpers-1.0.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-oc_sql_helpers-1.0.0.dist-info/METADATA,sha256=yaqy9ttmUJMG5IT__b74Kz-yTpC-Tgo9RznT4UHeXgM,243
-oc_sql_helpers-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-oc_sql_helpers-1.0.0.dist-info/top_level.txt,sha256=pKp8OXzXLdlZecL-DuIWqY8U4tr1bMLDqK4MOtMdMTU,15
-oc_sql_helpers-1.0.0.dist-info/RECORD,,
+oc_sql_helpers-1.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+oc_sql_helpers-1.0.1.dist-info/METADATA,sha256=uXzT57AO1IbYZeI0141EFf_Y3egkqGjlmqOFGQQArpg,243
+oc_sql_helpers-1.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+oc_sql_helpers-1.0.1.dist-info/top_level.txt,sha256=pKp8OXzXLdlZecL-DuIWqY8U4tr1bMLDqK4MOtMdMTU,15
+oc_sql_helpers-1.0.1.dist-info/RECORD,,
```

