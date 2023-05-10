# Comparing `tmp/markdowntodocx-0.1.3.8.tar.gz` & `tmp/markdowntodocx-0.1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdowntodocx-0.1.3.8.tar", last modified: Wed Feb 15 09:55:03 2023, max compression
+gzip compressed data, was "markdowntodocx-0.1.3.9.tar", last modified: Wed May 10 12:53:26 2023, max compression
```

## Comparing `markdowntodocx-0.1.3.8.tar` & `markdowntodocx-0.1.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2023-02-15 09:55:03.916799 markdowntodocx-0.1.3.8/
--rw-r--r--   0 barre     (1000) barre     (1000)     1064 2021-12-08 19:41:49.000000 markdowntodocx-0.1.3.8/LICENSE
--rw-r--r--   0 barre     (1000) barre     (1000)     4737 2023-02-15 09:55:03.916799 markdowntodocx-0.1.3.8/PKG-INFO
--rw-r--r--   0 barre     (1000) barre     (1000)     4468 2023-02-09 08:39:57.000000 markdowntodocx-0.1.3.8/README.md
-drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2023-02-15 09:55:03.916799 markdowntodocx-0.1.3.8/markdowntodocx/
--rw-r--r--   0 barre     (1000) barre     (1000)        0 2021-12-08 19:43:39.000000 markdowntodocx-0.1.3.8/markdowntodocx/__init__.py
--rw-r--r--   0 barre     (1000) barre     (1000)    27764 2023-02-15 09:52:55.000000 markdowntodocx-0.1.3.8/markdowntodocx/markdownconverter.py
-drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2023-02-15 09:55:03.916799 markdowntodocx-0.1.3.8/markdowntodocx.egg-info/
--rw-r--r--   0 barre     (1000) barre     (1000)     4737 2023-02-15 09:55:03.000000 markdowntodocx-0.1.3.8/markdowntodocx.egg-info/PKG-INFO
--rw-r--r--   0 barre     (1000) barre     (1000)      241 2023-02-15 09:55:03.000000 markdowntodocx-0.1.3.8/markdowntodocx.egg-info/SOURCES.txt
--rw-r--r--   0 barre     (1000) barre     (1000)        1 2023-02-15 09:55:03.000000 markdowntodocx-0.1.3.8/markdowntodocx.egg-info/dependency_links.txt
--rw-r--r--   0 barre     (1000) barre     (1000)       15 2023-02-15 09:55:03.000000 markdowntodocx-0.1.3.8/markdowntodocx.egg-info/top_level.txt
--rw-r--r--   0 barre     (1000) barre     (1000)       38 2023-02-15 09:55:03.920132 markdowntodocx-0.1.3.8/setup.cfg
--rw-r--r--   0 barre     (1000) barre     (1000)      618 2023-02-15 09:54:51.000000 markdowntodocx-0.1.3.8/setup.py
+drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2023-05-10 12:53:26.194735 markdowntodocx-0.1.3.9/
+-rw-r--r--   0 barre     (1000) barre     (1000)     1064 2021-12-08 19:41:49.000000 markdowntodocx-0.1.3.9/LICENSE
+-rw-r--r--   0 barre     (1000) barre     (1000)     4737 2023-05-10 12:53:26.194735 markdowntodocx-0.1.3.9/PKG-INFO
+-rw-r--r--   0 barre     (1000) barre     (1000)     4468 2023-02-09 08:39:57.000000 markdowntodocx-0.1.3.9/README.md
+drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2023-05-10 12:53:26.194735 markdowntodocx-0.1.3.9/markdowntodocx/
+-rw-r--r--   0 barre     (1000) barre     (1000)        0 2021-12-08 19:43:39.000000 markdowntodocx-0.1.3.9/markdowntodocx/__init__.py
+-rw-r--r--   0 barre     (1000) barre     (1000)    28451 2023-05-10 12:50:18.000000 markdowntodocx-0.1.3.9/markdowntodocx/markdownconverter.py
+drwxr-xr-x   0 barre     (1000) barre     (1000)        0 2023-05-10 12:53:26.194735 markdowntodocx-0.1.3.9/markdowntodocx.egg-info/
+-rw-r--r--   0 barre     (1000) barre     (1000)     4737 2023-05-10 12:53:26.000000 markdowntodocx-0.1.3.9/markdowntodocx.egg-info/PKG-INFO
+-rw-r--r--   0 barre     (1000) barre     (1000)      241 2023-05-10 12:53:26.000000 markdowntodocx-0.1.3.9/markdowntodocx.egg-info/SOURCES.txt
+-rw-r--r--   0 barre     (1000) barre     (1000)        1 2023-05-10 12:53:26.000000 markdowntodocx-0.1.3.9/markdowntodocx.egg-info/dependency_links.txt
+-rw-r--r--   0 barre     (1000) barre     (1000)       15 2023-05-10 12:53:26.000000 markdowntodocx-0.1.3.9/markdowntodocx.egg-info/top_level.txt
+-rw-r--r--   0 barre     (1000) barre     (1000)       38 2023-05-10 12:53:26.194735 markdowntodocx-0.1.3.9/setup.cfg
+-rw-r--r--   0 barre     (1000) barre     (1000)      618 2023-05-10 12:30:45.000000 markdowntodocx-0.1.3.9/setup.py
```

### Comparing `markdowntodocx-0.1.3.8/LICENSE` & `markdowntodocx-0.1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `markdowntodocx-0.1.3.8/PKG-INFO` & `markdowntodocx-0.1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdowntodocx
-Version: 0.1.3.8
+Version: 0.1.3.9
 Summary: Convert markdown inside Docx to docx styles
 Home-page: https://github.com/fbarre96/MarkDownToDocxStyle
 Author: Fabien Barre
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `markdowntodocx-0.1.3.8/README.md` & `markdowntodocx-0.1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `markdowntodocx-0.1.3.8/markdowntodocx/markdownconverter.py` & `markdowntodocx-0.1.3.9/markdowntodocx/markdownconverter.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,20 +95,23 @@
 
     def _add_p_with_paragraph(self, para):
         _p = para._p
         # paragraph footnote style
         pPr = _p.get_or_add_pPr()
         rstyle = pPr.get_or_add_pStyle()
         rstyle.val = 'FootnoteText'
+        para.style = styles["footnote text"]
         # run style (with id of run)
         new_run_element = _p._new_r()
         para.runs[0]._element.addprevious(new_run_element)
         rPr = new_run_element.get_or_add_rPr()
         rstyle = rPr.get_or_add_rStyle()
         rstyle.val = 'FootnoteReference'
+        r = Run(new_run_element, para)
+        r.style = styles["footnote reference"]
         ref = OxmlElement('w:footnoteRef')
         new_run_element.append(ref)
         self._insert_p(_p)
         return _p
     
     @property
     def paragraph(self):
@@ -362,14 +365,15 @@
             state = "normal"
         else:
             footnote_id = state.split(":")[1]
             footnote = footnotes[footnote_id]
             pPr = paragraph._p.get_or_add_pPr()
             rstyle = pPr.get_or_add_pStyle()
             rstyle.val = 'FootnoteText'
+            paragraph.style = styles["footnote text"]
             footnote._fn._insert_p(paragraph._p)
     else:
         state = transform_regex(paragraph, r"^(\[\^)([^\]\n]*)(\]:)(?!\w)(.+(?:\n[ \t]+.+)*)", (delCar, delCar, delCar, defineFootnote))
     transform_regex(paragraph, r"(https?:\/\/(?:www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b(?:[-a-zA-Z0-9()@:%_\+.~#?&//=]*[-a-zA-Z0-9@:%_\+.~#?&//=]))", (setHyperlink,))
     
     return state
 
@@ -405,35 +409,39 @@
     _footnotes_part = document._part.part_related_by(RT.FOOTNOTES)
     footnotes_part = _footnotes_part.element
     footnote = footnotes_part.add_footnote()
 
     footnote = Footnote(footnote, document._part)
     return footnote
 
-def add_footnote_reference(run, footnote):
+def add_footnote_reference(run, footnote_element):
     rPr = run._r.get_or_add_rPr()
     rstyle = rPr.get_or_add_rStyle()
     rstyle.val = 'FootnoteReference'
+    run.style = styles["footnote reference"]
     reference = OxmlElement('w:footnoteReference')
-    reference._id = footnote._id
+    reference._id = footnote_element._id
     run._r.append(reference)
 
 def setInlineFootnote(document, paragraph, run, match):
+    """Set the inline footnote.
+    run: document run that will be transformed to a footnote."""
     deletedCars = len(run.text)
-    run.text= ""
+    run.text= "" # Run text is removed to be placed inside the footnote paragraph
     #footnotes
-    footnote = add_footnote(document)
+    footnote = add_footnote(document) # create the footnote section for the document (empty)
     gr = re.search(r"(https?:\/\/(?:www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b(?:[-a-zA-Z0-9()@:%_\+.~#?&//=]*[-a-zA-Z0-9@:%_\+.~#?&//=]))", match.group(2))
-    
-    if gr is not None:
-        _p = footnote._fn._add_p(str(match.group(2)))
-        para = Paragraph(_p, footnote)
-        h_deletedCars, h_deletedRun, h_state = setHyperlink(para, para.runs[-1], gr, text=" "+str(match.group(2)), is_footnote=True, document=document)
-    else:
-        _p = footnote._fn._add_p(" " + str(match.group(2)))
+    _p = footnote._fn._add_p(" ") # create a paragraph with a run containing a space to separate the footnote id from the text
+    para = Paragraph(_p, footnote)
+    para.style = styles["footnote text"] # set footnote style
+    para.add_run(str(match.group(2)))   # put match text inside the footnotes
+    if gr is not None: # is link
+        h_deletedCars, h_deletedRun, h_state = setHyperlink(para, para.runs[-1], gr, text=str(match.group(2)), is_footnote=True, document=document)
+
+    para.runs[0].style = styles["footnote reference"] # set footnote id style
     # footnotes reference
     add_footnote_reference(run, footnote._fn)
     
     return deletedCars, False, "normal"
 
 def declareFootnote(document, paragraph, run, match):
     deletedCars = len(run.text)
@@ -447,14 +455,15 @@
 
     return deletedCars, False, "normal"
 
 def defineFootnote(paragraph, run, match):
     #footnotes
     footnote_id = match.group(2)
     footnote = footnotes[footnote_id]
+    
     _p = footnote._fn._add_p_with_paragraph(paragraph)
     return 0, False, "inFootnoteDefinition:"+str(footnote_id)
 
 
 def setBookmark(document, paragraph, run, match):
     """Set the bookmark
     function adapted from https://stackoverflow.com/questions/57586400/how-to-create-bookmarks-in-a-word-document-then-create-internal-hyperlinks-to-t
```

### Comparing `markdowntodocx-0.1.3.8/markdowntodocx.egg-info/PKG-INFO` & `markdowntodocx-0.1.3.9/markdowntodocx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdowntodocx
-Version: 0.1.3.8
+Version: 0.1.3.9
 Summary: Convert markdown inside Docx to docx styles
 Home-page: https://github.com/fbarre96/MarkDownToDocxStyle
 Author: Fabien Barre
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `markdowntodocx-0.1.3.8/setup.py` & `markdowntodocx-0.1.3.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name='markdowntodocx',
     packages=find_packages(include=['markdowntodocx']),
-    version='0.1.3.8',
+    version='0.1.3.9',
     url="https://github.com/fbarre96/MarkDownToDocxStyle",
     description='Convert markdown inside Docx to docx styles',
     long_description=README,
     long_description_content_type="text/markdown",
     author='Fabien Barre',
     license='MIT',
     setup_requires=['python-docx',"requests"],
```

