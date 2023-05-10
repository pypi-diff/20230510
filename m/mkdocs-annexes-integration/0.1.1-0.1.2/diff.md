# Comparing `tmp/mkdocs-annexes-integration-0.1.1.tar.gz` & `tmp/mkdocs-annexes-integration-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-annexes-integration-0.1.1.tar", last modified: Tue May  9 06:34:13 2023, max compression
+gzip compressed data, was "mkdocs-annexes-integration-0.1.2.tar", last modified: Tue May  9 09:39:50 2023, max compression
```

## Comparing `mkdocs-annexes-integration-0.1.1.tar` & `mkdocs-annexes-integration-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 06:34:13.591688 mkdocs-annexes-integration-0.1.1/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     3871 2023-05-09 06:34:13.589691 mkdocs-annexes-integration-0.1.1/PKG-INFO
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 06:34:13.490625 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-02 06:14:09.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration/__init__.py
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     6454 2023-05-09 06:32:03.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration/plugin.py
-drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 06:34:13.574636 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     3871 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/PKG-INFO
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      386 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/SOURCES.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/dependency_links.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       93 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/entry_points.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       32 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/requires.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       27 2023-05-09 06:34:13.000000 mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/top_level.txt
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2023-05-09 06:34:13.592692 mkdocs-annexes-integration-0.1.1/setup.cfg
--rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1169 2023-05-09 06:33:50.000000 mkdocs-annexes-integration-0.1.1/setup.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 09:39:50.766554 mkdocs-annexes-integration-0.1.2/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       77 2023-05-09 09:20:19.000000 mkdocs-annexes-integration-0.1.2/MANIFEST.in
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4620 2023-05-09 09:39:50.764555 mkdocs-annexes-integration-0.1.2/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      782 2023-05-09 09:36:24.000000 mkdocs-annexes-integration-0.1.2/changelog.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1075 2023-04-28 08:21:37.000000 mkdocs-annexes-integration-0.1.2/license
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 09:39:50.666955 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-02 06:14:09.000000 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration/__init__.py
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     8295 2023-05-09 09:25:59.000000 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration/plugin.py
+drwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        0 2023-05-09 09:39:50.749557 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration.egg-info/
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     4620 2023-05-09 09:39:50.000000 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration.egg-info/PKG-INFO
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)      441 2023-05-09 09:39:50.000000 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration.egg-info/SOURCES.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)        1 2023-05-09 09:39:50.000000 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration.egg-info/dependency_links.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       93 2023-05-09 09:39:50.000000 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration.egg-info/entry_points.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       32 2023-05-09 09:39:50.000000 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration.egg-info/requires.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       27 2023-05-09 09:39:50.000000 mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration.egg-info/top_level.txt
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     3258 2023-05-09 09:31:00.000000 mkdocs-annexes-integration-0.1.2/readme.md
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)       38 2023-05-09 09:39:50.766554 mkdocs-annexes-integration-0.1.2/setup.cfg
+-rwxrwxrwx   0 thibaud-brrd  (1001) thibaud-brrd  (1001)     1201 2023-05-09 09:16:52.000000 mkdocs-annexes-integration-0.1.2/setup.py
```

### Comparing `mkdocs-annexes-integration-0.1.1/PKG-INFO` & `mkdocs-annexes-integration-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-annexes-integration
-Version: 0.1.1
+Version: 0.1.2
 Summary: A MkDocs plugin transforming annexes files into images to be integrated in markdown pages
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-annexes-integration
         
@@ -36,50 +36,72 @@
         
         #### Install on Windows :
         
         On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
         
         ### Installing using pip:
         
-        `pip install mkdocs-annexes-integrations`
+        `pip install mkdocs-annexes-integration`
         
         ## Config
         
         You need to activate the plugin in `mkdocs.yml`:
         
         ```yaml
         plugins:
-          - annexes-integrations:
-            - annexes: # Required (at least 1)
-              - Title of the annex A1: path/A/to/an/annex1.pdf # An path to an annex with it's title
-              - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
-              - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
-              - Title of the annex C1:
-                  src: ../src/path/C/to/an/annex1.pdf
-                  dest: dest/path/C/to/an/annex1.pdf
-              # ...
-            - temp_dir: "folder_name" # Optional --> Default : temp_annexes
+          - annexes-integration:
+              annexes: # Required (at least 1)
+                - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
+                - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
+                - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
+                - Title of the code file annex:
+                    src: ../src/path/to/a/code/file1.py
+                    dest: dest/path/to/a/code/file1.py
+                # others annexes...
+              temp_dir: "folder_name" # Optional --> Default : temp_annexes
         ```
         
-        As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. Both paths need to be relative to 'docs_dir', though.
+        As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
         
-        Set at least on annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
+        Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
         
-        - `annexes` - A list of all the annexes documents. The path from docs_dir to an annex file associated to it's title
+        - `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
         - `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
         
         ## Usage
         
         Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
         
         This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
         
+        ## Support
+        
+        This plugin currently support two type of files :
+        
+        - **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
+        
+        - **Code files**: The plugin will put the content of the code file into a codeblock to be integrated on a page
+        
+        Currently supported code files are :
+         - CSharp (.cs)
+         - CSS (.css)
+         - Dart (.dart)
+         - HTML (.html)
+         - Javascript (.js)
+         - JSON (.json)
+         - PHP (.php)
+         - Python (.py)
+        
+        ## License
+        
+        This project is under MIT license see: `license` file for more detail.
+        
         ## See Also
         
-        - [gitlab repo](http://www.gitlab.org/thibaud-brrd/mkdocs-annexes-integration/)
+        - [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
         - [mkdocs website](http://www.mkdocs.org/)
         - [mkdocs with-pdf plugin](https://github.com/orzih/mkdocs-with-pdf)
 Keywords: mkdocs
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration/plugin.py` & `mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,123 +1,148 @@
-import os, shutil
-import logging
-from pdf2image import convert_from_path
-
-from mkdocs.config import base, config_options as c
-from mkdocs.plugins import BasePlugin
-from mkdocs.structure.files import File
-
-# class _Annexe(base.Config):
-#     src = c.File(exists=True)
-#     dest = c.Type(str, default=src)
-#     num = c.Optional(c.Type(int))
+"""
+File: mkdocs_annexes_integration/plugin.py
+Desc: This file contain the plugin used by mkdocs to integrate annexes as markdown file
+Author: Thibaud Briard - BRT, <thibaud.brrd@eduge.ch>
+Version: 0.1.2 - 2023-05-09
+"""
+# Imports...
+import os, shutil # used to handle path, dicrectory and file creation, deletion and validation.
+import logging # used to log warning and errors for MkDocs among other things
+from pdf2image import convert_from_path # used to tranform pdf pages into images
+
+from mkdocs.config.base import Config as base_config # used to create an MkDocs config class derived from MkDocs config base
+from mkdocs.plugins import BasePlugin as base_plugin # used to create an MkDocs plugin class derived from MkDocs plugin base
+from mkdocs.config import config_options as c # used for config schema type safety
+from mkdocs.structure.files import File # used to create File in documentation
 
-class AnnexesIntegrationConfig(base.Config):
+# The plugin config options
+class AnnexesIntegrationConfig(base_config):
     temp_dir = c.Type(str, default='temp_annexes')
-    annexes = c.ListOfItems(c.Type(dict)) # c.SubConfig(_Annexe)
+    annexes = c.ListOfItems(c.Type(dict))
 
-class AnnexesIntegration(BasePlugin[AnnexesIntegrationConfig]):
+# The plugin itself
+class AnnexesIntegration(base_plugin[AnnexesIntegrationConfig]):
 
     def __init__(self):
         self._logger = logging.getLogger('mkdocs.annexes-integration')
         self._logger.setLevel(logging.INFO)
 
         self.enabled = True
         self.total_time = 0
     
     def on_config(self, config):
+        # Create temp_dir in directory of mkdocs.yml
         self.config.temp_dir = os.path.join(os.path.dirname(config.docs_dir), self.config.temp_dir)
         if not os.path.exists(self.config.temp_dir):
             os.mkdir(self.config.temp_dir)
         return config
 
     def on_files(self, files, config):
+        # Generate markdown files for each annex
         try:
             for annex in self.config.annexes:
                 title, path = list(annex.items())[0]
                 self._logger.info(f'Integrating annex "{title}"')
+                # Determine source and destination path from path option
                 src, dest = self.get_src_and_dest(path)
+                # Get extension of file
                 extension = os.path.splitext(src)[1][1:]
+                # Get absolute path to original file
                 original = os.path.join(config.docs_dir, src)
-                root = os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])
-                embedded = f'{root}.md'
+                # Get absolute path to generated markdown
+                embedded = f'{os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])}.md'
+                # skip if original file don't exist
                 if os.path.exists(original):
+                    # Check if file is code file or pdf
                     if extension in ['cs', 'css', 'dart', 'html', 'js', 'json', 'php', 'py']:
+                        # For code files content are put ina codeblock
                         self._logger.info(f'    With content as code block')
                         with open(original, 'r') as file:
                             content = file.read()
                         # Create a markdown file that take care of showing source code annex
                         if not os.path.exists(os.path.dirname(embedded)):
                             os.makedirs(os.path.dirname(embedded))
                         with open(embedded, 'w') as f:
                             # write the title and the content to the file
                             f.write(f'# {title}\n\n``` {extension}\n{content}\n```\n')
                     elif extension in ['pdf']:
+                        # For PDF files each page are transformed into images
                         self._logger.info(f'    With each pages as images')
+                        # Get absolute path for PDF directory
+                        root = os.path.join(self.config.temp_dir, os.path.splitext(dest)[0])
+                        # Get absolute path for PDF images directory
                         source = os.path.join(root, 'source')
                         # Create a root folder containing the annex
                         if not os.path.exists(root):
                             os.makedirs(root)
                         # Save pages as images in the pdf
                         images = convert_from_path(original)
                         # Create source folder to save images
                         if not os.path.exists(source):
                             os.mkdir(source)
                         # Create a markdown file that take care of showing PDF annex
                         with open(embedded, 'w') as f:
-                            # write the title to the file
+                            # Write the title to the file
                             f.write(f'# {title}\n\n')
 
                             for i in range(len(images)):
                                 # Add leading zeros to the page number
                                 filename = f'page_{i + 1:04}.jpg'
                                 images[i].save(f'{source}/{filename}', 'JPEG')
                                 files.append(File(os.path.join(os.path.splitext(dest)[0], f'source/{filename}'), src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
 
-                                # write the image link to the file
+                                # Write the image link to the file
                                 f.write(f'![Page {i+1}](./{os.path.basename(os.path.splitext(dest)[0])}/source/{filename})\n')
                     else:
                         self._logger.warning(f'file {src} extension isn\'t supported (yet) --> skipped')
-                    # removing originals files from list of mkdocs files if they were in the docs directory originaly
+                    # Removing originals files from list of mkdocs files if they were in the docs directory originaly
                     if os.path.isfile(os.path.join(config.docs_dir, dest)):
                         self._logger.info(f'    Remvoing original annex {src} from processed files list')
                         files.remove(files.get_file_from_path(src))
-                    # adding embedded files in list of mkdocs files
+                    # Adding embedded files in list of mkdocs files
                     path = f'{os.path.splitext(dest)[0]}.md'
                     self._logger.info(f'    Adding embedded annex {dest} to processed files list')
                     files.append(File(path, src_dir=self.config.temp_dir, dest_dir=config.site_dir, use_directory_urls=config.use_directory_urls))
                 else:
                     self._logger.warning(f'{src} file doesn\'t exist at {original} --> skipped')
         except Exception as e:
+            # Remove temp directory in case of any error before raising error
             self._logger.error(f'error with the annexes-integration plugin : {e}')
             if os.path.exists(self.config.temp_dir):
                 shutil.rmtree(self.config.temp_dir)
             raise e
         return files
     
     def on_post_build(self, config):
         # Removing temp_dir directory
         self._logger.info(f'Removin annexes temporary directory {self.config.temp_dir}')
         if os.path.exists(self.config.temp_dir):
             shutil.rmtree(self.config.temp_dir)
         return
     
     def get_src_and_dest(self, path):
+        # Get src and dest path from path
         if type(path) is dict:
             src = path['src']
             dest = src
+            # Remove every ../ from dest if they exist
             while (dest.startswith('../')):
                 dest = dest[3:]
+            # Get dest from dict if it as been set
             if 'dest' in path:
                 dest = path['dest']
+                
+        # Get src from path and create dest as same as src
         else:
             src = path
             dest = src
+            # Remove every ../ from dest if they exist
             while (dest.startswith('../')):
                 dest = dest[3:]
+        # add underscore if filename is index to prevent mkdocs from rendring it as an index
         if os.path.splitext(os.path.basename(dest))[0] == 'index':
             dest = os.path.join(os.path.dirname(dest), f'_{os.path.basename(dest)}')
         return src, dest
     
     def get_file_ext(self, src):
         return os.path.splitext(src)[1][1:]
```

### Comparing `mkdocs-annexes-integration-0.1.1/mkdocs_annexes_integration.egg-info/PKG-INFO` & `mkdocs-annexes-integration-0.1.2/mkdocs_annexes_integration.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-annexes-integration
-Version: 0.1.1
+Version: 0.1.2
 Summary: A MkDocs plugin transforming annexes files into images to be integrated in markdown pages
 Home-page: https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration
 Author: Thibaud Briard
 Author-email: thibaud.brrd@eduge.ch
 License: MIT
 Description: # mkdocs-annexes-integration
         
@@ -36,50 +36,72 @@
         
         #### Install on Windows :
         
         On Windows, you can download the latest binary release of Poppler from the official website and extract the files to a folder. Then, add the folder to the system's PATH environment variable.
         
         ### Installing using pip:
         
-        `pip install mkdocs-annexes-integrations`
+        `pip install mkdocs-annexes-integration`
         
         ## Config
         
         You need to activate the plugin in `mkdocs.yml`:
         
         ```yaml
         plugins:
-          - annexes-integrations:
-            - annexes: # Required (at least 1)
-              - Title of the annex A1: path/A/to/an/annex1.pdf # An path to an annex with it's title
-              - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
-              - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
-              - Title of the annex C1:
-                  src: ../src/path/C/to/an/annex1.pdf
-                  dest: dest/path/C/to/an/annex1.pdf
-              # ...
-            - temp_dir: "folder_name" # Optional --> Default : temp_annexes
+          - annexes-integration:
+              annexes: # Required (at least 1)
+                - Title of the annex A1: path/A/to/an/annex1.pdf # A path to an annex with it's title
+                - Title of the annex A2: path/A/to/an/annex2.pdf # Another path to an annex in same folder as the first
+                - Title of the annex B1: path/B/to/an/annex1.pdf # Another path to an annex but in different folder as the first two
+                - Title of the code file annex:
+                    src: ../src/path/to/a/code/file1.py
+                    dest: dest/path/to/a/code/file1.py
+                # others annexes...
+              temp_dir: "folder_name" # Optional --> Default : temp_annexes
         ```
         
-        As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. Both paths need to be relative to 'docs_dir', though.
+        As you can see, there are two possible ways to integrate an annex: using a simple path or a source path and a destination path. **Both paths need to be relative to `docs_dir`, though**.
         
-        Set at least on annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
+        Set at least one annex to use this plugin. If you don't have any annex don't add this plugin to the mkdocs plugins list in config file mkdocs.yml
         
-        - `annexes` - A list of all the annexes documents. The path from docs_dir to an annex file associated to it's title
+        - `annexes` - A list of all the annexes documents. The path from `docs_dir` to an annex file associated to it's title
         - `temp_dir` - The temp directory used to generate markdown file for each annex before rendering to HTML. Only set this option if you already have a temp_annexes folder in the root directory (same as mkdocs.yml), which, you should not normally.
         
         ## Usage
         
         Using the command `mkdocs build` or `mkdocs serve` will trigger the plugin if it as been set correctly in config file.
         
         This plugin is intended to be used with `mkdocs-with-pdf` plugin but can be used as it is.
         
+        ## Support
+        
+        This plugin currently support two type of files :
+        
+        - **PDF files**: The plugin will convert each page of the PDF into images to be integrated on a page
+        
+        - **Code files**: The plugin will put the content of the code file into a codeblock to be integrated on a page
+        
+        Currently supported code files are :
+         - CSharp (.cs)
+         - CSS (.css)
+         - Dart (.dart)
+         - HTML (.html)
+         - Javascript (.js)
+         - JSON (.json)
+         - PHP (.php)
+         - Python (.py)
+        
+        ## License
+        
+        This project is under MIT license see: `license` file for more detail.
+        
         ## See Also
         
-        - [gitlab repo](http://www.gitlab.org/thibaud-brrd/mkdocs-annexes-integration/)
+        - [gitlab repo](http://www.gitlab.org/cfpt-mkdocs-plugins/mkdocs-annexes-integration/)
         - [mkdocs website](http://www.mkdocs.org/)
         - [mkdocs with-pdf plugin](https://github.com/orzih/mkdocs-with-pdf)
 Keywords: mkdocs
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `mkdocs-annexes-integration-0.1.1/setup.py` & `mkdocs-annexes-integration-0.1.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import io
 
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-annexes-integration',
-    version='0.1.1',
+    version='0.1.2',
     description='A MkDocs plugin transforming annexes files into images to be integrated in markdown pages',
     long_description=io.open('readme.md', encoding='utf8').read(),
     long_description_content_type='text/markdown',
     keywords='mkdocs',
     url='https://gitlab.com/cfpt-mkdocs-plugins/mkdocs-annexes-integration',
     author='Thibaud Briard',
     author_email='thibaud.brrd@eduge.ch',
@@ -23,13 +23,14 @@
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3 :: Only',
     ],
     packages=find_packages(),
+    include_package_data=True,
     entry_points={
         'mkdocs.plugins': [
             'annexes-integration = mkdocs_annexes_integration.plugin:AnnexesIntegration'
         ]
     }
 )
```

