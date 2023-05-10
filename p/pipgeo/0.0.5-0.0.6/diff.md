# Comparing `tmp/pipgeo-0.0.5.tar.gz` & `tmp/pipgeo-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pipgeo-0.0.5.tar", last modified: Tue Jan 31 04:03:59 2023, max compression
+gzip compressed data, was "pipgeo-0.0.6.tar", last modified: Wed May 10 01:19:09 2023, max compression
```

## Comparing `pipgeo-0.0.5.tar` & `pipgeo-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-31 04:03:59.290697 pipgeo-0.0.5/
--rw-rw-rw-   0        0        0     3834 2023-01-31 04:03:59.289998 pipgeo-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2493 2023-01-31 03:57:38.000000 pipgeo-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-01-31 04:03:59.279697 pipgeo-0.0.5/pipgeo/
--rw-rw-rw-   0        0        0      119 2023-01-31 03:56:15.000000 pipgeo-0.0.5/pipgeo/__init__.py
--rw-rw-rw-   0        0        0     9100 2023-01-31 03:53:06.000000 pipgeo-0.0.5/pipgeo/pipgeo.py
-drwxrwxrwx   0        0        0        0 2023-01-31 04:03:59.288696 pipgeo-0.0.5/pipgeo.egg-info/
--rw-rw-rw-   0        0        0     3834 2023-01-31 04:03:59.000000 pipgeo-0.0.5/pipgeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-01-31 04:03:59.000000 pipgeo-0.0.5/pipgeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-31 04:03:59.000000 pipgeo-0.0.5/pipgeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-01-31 04:03:59.000000 pipgeo-0.0.5/pipgeo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2023-01-31 04:03:59.000000 pipgeo-0.0.5/pipgeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-31 04:03:59.000000 pipgeo-0.0.5/pipgeo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-31 04:03:59.290697 pipgeo-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1344 2023-01-31 03:56:00.000000 pipgeo-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:19:09.339273 pipgeo-0.0.6/
+-rw-rw-rw-   0        0        0    11558 2023-01-13 05:52:28.000000 pipgeo-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3378 2023-05-10 01:19:09.332276 pipgeo-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2609 2023-05-10 01:18:13.000000 pipgeo-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 01:19:09.215614 pipgeo-0.0.6/pipgeo/
+-rw-rw-rw-   0        0        0      119 2023-05-10 01:15:21.000000 pipgeo-0.0.6/pipgeo/__init__.py
+-rw-rw-rw-   0        0        0    10231 2023-05-10 01:13:32.000000 pipgeo-0.0.6/pipgeo/pipgeo.py
+drwxrwxrwx   0        0        0        0 2023-05-10 01:19:09.326274 pipgeo-0.0.6/pipgeo.egg-info/
+-rw-rw-rw-   0        0        0     3378 2023-05-10 01:19:09.000000 pipgeo-0.0.6/pipgeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-10 01:19:09.000000 pipgeo-0.0.6/pipgeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 01:19:09.000000 pipgeo-0.0.6/pipgeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-10 01:19:09.000000 pipgeo-0.0.6/pipgeo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       88 2023-05-10 01:19:09.000000 pipgeo-0.0.6/pipgeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-10 01:19:09.000000 pipgeo-0.0.6/pipgeo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 01:19:09.340318 pipgeo-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2023-05-10 01:17:10.000000 pipgeo-0.0.6/setup.py
```

### Comparing `pipgeo-0.0.5/PKG-INFO` & `pipgeo-0.0.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,87 @@
 Metadata-Version: 2.1
 Name: pipgeo
-Version: 0.0.5
+Version: 0.0.6
 Summary: CLI for Unofficial windows Geospatial library wheels
 Home-page: https://github.com/samapriya/pipgeo
 Author: Samapriya Roy
 Author-email: samapriya.roy@gmail.com
 License: Apache 2.0
-Description: # pipgeo: CLI for Unofficial windows Geospatial library wheels
-        
-        [![CI pipgeo](https://github.com/samapriya/pipgeo/actions/workflows/CI.yml/badge.svg)](https://github.com/samapriya/pipgeo/actions/workflows/CI.yml)
-        
-        The amazing work of [Christoph Gohlke](https://www.cgohlke.com/) is the source of all this, though the unofficial windows binaries page at lfd is no longer maintained. Christoph has created a [dedicated GitHub repository with a subset of geospatial wheel assets that have been released](https://github.com/cgohlke/geospatial.whl). This tool is a straightforward CLI that can pre-install a binary wheel from the latest release assets.
-        
-        #### Installation
-        
-        Installation is pretty simple use. The tool automatically also checks as new versions are released and informs you.
-        
-        **The precompiled wheels and as such the tool is only available for python 3.8 and higher**
-        
-        ```
-        pip install pipgeo
-        ```
-        
-        ![pipgeo-install](https://user-images.githubusercontent.com/6677629/212253241-0bed60f5-c83b-4fbb-b79d-b63d543eb928.gif)
-        
-        #### pipgeo release
-        This tool fetches release assets from the latest release and lists them to the user incase they are looking for a specific packages and or want to install a specific package.
-        
-        Example usage
-        
-        ```
-        pipgeo release
-        ```
-        
-        ![pipgeo-list](https://user-images.githubusercontent.com/6677629/212253240-1d928f64-9004-4254-b80c-0b3b08a01437.gif)
-        
-        #### pipgeo fetch
-        This tool will allow you to fetch a specific package from the latest release and install it. You can search based on the package list returned form the release tool.
-        
-        Example usage
-        
-        ```
-        pipgeo fetch --lib gdal
-        ```
-        
-        ![pipgeo-fetch](https://user-images.githubusercontent.com/6677629/212253239-9a9381e7-fe2d-4008-a4a4-8418fa687597.gif)
-        
-        #### pipgeo sys
-        This will install all packages from the release assets onto your system. It maintains prerequisite and dependency order to allow for easy installation.
-        
-        Example usage
-        
-        ```
-        pipgeo sys
-        ```
-        
-        ![pipgeo-sys](https://user-images.githubusercontent.com/6677629/212253237-9bbd32c0-3312-4a8b-8661-887f7422b45b.gif)
-        
-        ### Changelog
-        
-        #### v0.0.5
-        - release tool now print available release packages and version number
-        - improved pypi version check functionality
-        - fetch tool auto upgrades to latest version if new version is available in release
-        
-        #### v0.0.4
-        - added dependency check from dependency tree
-        - dependencies also installed using pipgeo
-        
-        #### v0.0.3
-        - updated readme with instructions
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: GIS
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pipgeo: CLI for Unofficial windows Geospatial library wheels
+
+[![CI pipgeo](https://github.com/samapriya/pipgeo/actions/workflows/CI.yml/badge.svg)](https://github.com/samapriya/pipgeo/actions/workflows/CI.yml)
+
+The amazing work of [Christoph Gohlke](https://www.cgohlke.com/) is the source of all this, though the unofficial windows binaries page at lfd is no longer maintained. Christoph has created a [dedicated GitHub repository with a subset of geospatial wheel assets that have been released](https://github.com/cgohlke/geospatial.whl). This tool is a straightforward CLI that can pre-install a binary wheel from the latest release assets.
+
+#### Installation
+
+Installation is pretty simple use. The tool automatically also checks as new versions are released and informs you.
+
+**The precompiled wheels and as such the tool is only available for python 3.8 and higher**
+
+```
+pip install pipgeo
+```
+
+![pipgeo-install](https://user-images.githubusercontent.com/6677629/212253241-0bed60f5-c83b-4fbb-b79d-b63d543eb928.gif)
+
+#### pipgeo release
+This tool fetches release assets from the latest release and lists them to the user incase they are looking for a specific packages and or want to install a specific package.
+
+Example usage
+
+```
+pipgeo release
+```
+
+![pipgeo-list](https://user-images.githubusercontent.com/6677629/212253240-1d928f64-9004-4254-b80c-0b3b08a01437.gif)
+
+#### pipgeo fetch
+This tool will allow you to fetch a specific package from the latest release and install it. You can search based on the package list returned form the release tool.
+
+Example usage
+
+```
+pipgeo fetch --lib gdal
+```
+
+![pipgeo-fetch](https://user-images.githubusercontent.com/6677629/212253239-9a9381e7-fe2d-4008-a4a4-8418fa687597.gif)
+
+#### pipgeo sys
+This will install all packages from the release assets onto your system. It maintains prerequisite and dependency order to allow for easy installation.
+
+Example usage
+
+```
+pipgeo sys
+```
+
+![pipgeo-sys](https://user-images.githubusercontent.com/6677629/212253237-9bbd32c0-3312-4a8b-8661-887f7422b45b.gif)
+
+### Changelog
+
+#### v0.0.6
+- release checker tool now checks if packages exists for installed python version in latest release
+
+#### v0.0.5
+- release tool now print available release packages and version number
+- improved pypi version check functionality
+- fetch tool auto upgrades to latest version if new version is available in release
+
+#### v0.0.4
+- added dependency check from dependency tree
+- dependencies also installed using pipgeo
+
+#### v0.0.3
+- updated readme with instructions
```

### Comparing `pipgeo-0.0.5/README.md` & `pipgeo-0.0.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,17 @@
 pipgeo sys
 ```
 
 ![pipgeo-sys](https://user-images.githubusercontent.com/6677629/212253237-9bbd32c0-3312-4a8b-8661-887f7422b45b.gif)
 
 ### Changelog
 
+#### v0.0.6
+- release checker tool now checks if packages exists for installed python version in latest release
+
 #### v0.0.5
 - release tool now print available release packages and version number
 - improved pypi version check functionality
 - fetch tool auto upgrades to latest version if new version is available in release
 
 #### v0.0.4
 - added dependency check from dependency tree
```

### Comparing `pipgeo-0.0.5/pipgeo/pipgeo.py` & `pipgeo-0.0.6/pipgeo/pipgeo.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import sys
 from collections import OrderedDict
 from os.path import expanduser
 
 import pkg_resources
 import requests
 from bs4 import BeautifulSoup
+from natsort import natsorted
 
 if not str(platform.system().lower()) == "windows":
     sys.exit('This tool is only designed to fetch binaries for windows OS')
 installed_packages = [pkg.key for pkg in pkg_resources.working_set]
 
 
 class Solution:
@@ -100,16 +101,38 @@
     ex_list = ['amd64', 'arm64']
     if not exc_name in ex_list:
         overall_sys = f'cp{version_tag}-cp{version_tag}-win{exc_name}'
     else:
         overall_sys = f'cp{version_tag}-cp{version_tag}-win_{exc_name}'
     return overall_sys
 
+def release_checker():
+    version_tag = f"{sys.version_info[0]}{sys.version_info[1]}"
+    syspy = f'cp{version_tag}'
+    response = requests.get(
+        'https://github.com/cgohlke/geospatial.whl/releases/latest')
+    if response.history:
+        tag = (response.url.split('/')[-1])
+
+    url = f"https://github.com/cgohlke/geospatial.whl/releases/expanded_assets/{tag}"
+    source = requests.get(url)
+    html_content = source.text
+    soup = BeautifulSoup(html_content, "html.parser")
+    release_package_pylist = []
+    for a in soup.find_all('a', href=True):
+        rl= a['href'].split('/')[-1].lower().split('-win')[0].split('-')[-1].split('_')[0]
+        if rl.startswith('cp'):
+            release_package_pylist.append(rl)
+    unique_pkg = list(set(release_package_pylist))
+    if not syspy in unique_pkg:
+        print('Latest package releases only support python versions'+'\n')
+        sys.exit(json.dumps(natsorted([release.split('cp')[1].replace('3','3.') for release in unique_pkg]),indent=2))
 
 def download_file(url, lib):
+    release_checker()
     home_dir = expanduser("~")
     filename = url.split('/')[-1]
     full_filename = os.path.join(home_dir, filename)
     installed_packages = [
         f'{pkg.key}-{pkg.version}' for pkg in pkg_resources.working_set]
     package_match = [x for x in installed_packages if re.search(lib, x)]
     if not package_match:
@@ -155,14 +178,15 @@
         dependency = deptree.get(lib.lower())
         if not dependency in installed_packages:
             print(f'Fetching dependency {dependency}')
             fetch_geo(dependency)
 
 
 def fetch_geo(lib):
+    release_checker()
     lib_list = []
     match_list = []
     dependency_check(lib)
     response = requests.get(
         'https://github.com/cgohlke/geospatial.whl/releases/latest')
     if response.history:
         tag = (response.url.split('/')[-1])
@@ -187,14 +211,15 @@
 def fetch_from_parser(args):
     fetch_geo(
         lib=args.lib
     )
 
 
 def release_list():
+    release_checker()
     lib_list = []
     response = requests.get(
         'https://github.com/cgohlke/geospatial.whl/releases/latest')
     if response.history:
         tag = (response.url.split('/')[-1])
 
     url = f"https://github.com/cgohlke/geospatial.whl/releases/expanded_assets/{tag}"
```

### Comparing `pipgeo-0.0.5/pipgeo.egg-info/PKG-INFO` & `pipgeo-0.0.6/pipgeo.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,85 +1,87 @@
 Metadata-Version: 2.1
 Name: pipgeo
-Version: 0.0.5
+Version: 0.0.6
 Summary: CLI for Unofficial windows Geospatial library wheels
 Home-page: https://github.com/samapriya/pipgeo
 Author: Samapriya Roy
 Author-email: samapriya.roy@gmail.com
 License: Apache 2.0
-Description: # pipgeo: CLI for Unofficial windows Geospatial library wheels
-        
-        [![CI pipgeo](https://github.com/samapriya/pipgeo/actions/workflows/CI.yml/badge.svg)](https://github.com/samapriya/pipgeo/actions/workflows/CI.yml)
-        
-        The amazing work of [Christoph Gohlke](https://www.cgohlke.com/) is the source of all this, though the unofficial windows binaries page at lfd is no longer maintained. Christoph has created a [dedicated GitHub repository with a subset of geospatial wheel assets that have been released](https://github.com/cgohlke/geospatial.whl). This tool is a straightforward CLI that can pre-install a binary wheel from the latest release assets.
-        
-        #### Installation
-        
-        Installation is pretty simple use. The tool automatically also checks as new versions are released and informs you.
-        
-        **The precompiled wheels and as such the tool is only available for python 3.8 and higher**
-        
-        ```
-        pip install pipgeo
-        ```
-        
-        ![pipgeo-install](https://user-images.githubusercontent.com/6677629/212253241-0bed60f5-c83b-4fbb-b79d-b63d543eb928.gif)
-        
-        #### pipgeo release
-        This tool fetches release assets from the latest release and lists them to the user incase they are looking for a specific packages and or want to install a specific package.
-        
-        Example usage
-        
-        ```
-        pipgeo release
-        ```
-        
-        ![pipgeo-list](https://user-images.githubusercontent.com/6677629/212253240-1d928f64-9004-4254-b80c-0b3b08a01437.gif)
-        
-        #### pipgeo fetch
-        This tool will allow you to fetch a specific package from the latest release and install it. You can search based on the package list returned form the release tool.
-        
-        Example usage
-        
-        ```
-        pipgeo fetch --lib gdal
-        ```
-        
-        ![pipgeo-fetch](https://user-images.githubusercontent.com/6677629/212253239-9a9381e7-fe2d-4008-a4a4-8418fa687597.gif)
-        
-        #### pipgeo sys
-        This will install all packages from the release assets onto your system. It maintains prerequisite and dependency order to allow for easy installation.
-        
-        Example usage
-        
-        ```
-        pipgeo sys
-        ```
-        
-        ![pipgeo-sys](https://user-images.githubusercontent.com/6677629/212253237-9bbd32c0-3312-4a8b-8661-887f7422b45b.gif)
-        
-        ### Changelog
-        
-        #### v0.0.5
-        - release tool now print available release packages and version number
-        - improved pypi version check functionality
-        - fetch tool auto upgrades to latest version if new version is available in release
-        
-        #### v0.0.4
-        - added dependency check from dependency tree
-        - dependencies also installed using pipgeo
-        
-        #### v0.0.3
-        - updated readme with instructions
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: GIS
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pipgeo: CLI for Unofficial windows Geospatial library wheels
+
+[![CI pipgeo](https://github.com/samapriya/pipgeo/actions/workflows/CI.yml/badge.svg)](https://github.com/samapriya/pipgeo/actions/workflows/CI.yml)
+
+The amazing work of [Christoph Gohlke](https://www.cgohlke.com/) is the source of all this, though the unofficial windows binaries page at lfd is no longer maintained. Christoph has created a [dedicated GitHub repository with a subset of geospatial wheel assets that have been released](https://github.com/cgohlke/geospatial.whl). This tool is a straightforward CLI that can pre-install a binary wheel from the latest release assets.
+
+#### Installation
+
+Installation is pretty simple use. The tool automatically also checks as new versions are released and informs you.
+
+**The precompiled wheels and as such the tool is only available for python 3.8 and higher**
+
+```
+pip install pipgeo
+```
+
+![pipgeo-install](https://user-images.githubusercontent.com/6677629/212253241-0bed60f5-c83b-4fbb-b79d-b63d543eb928.gif)
+
+#### pipgeo release
+This tool fetches release assets from the latest release and lists them to the user incase they are looking for a specific packages and or want to install a specific package.
+
+Example usage
+
+```
+pipgeo release
+```
+
+![pipgeo-list](https://user-images.githubusercontent.com/6677629/212253240-1d928f64-9004-4254-b80c-0b3b08a01437.gif)
+
+#### pipgeo fetch
+This tool will allow you to fetch a specific package from the latest release and install it. You can search based on the package list returned form the release tool.
+
+Example usage
+
+```
+pipgeo fetch --lib gdal
+```
+
+![pipgeo-fetch](https://user-images.githubusercontent.com/6677629/212253239-9a9381e7-fe2d-4008-a4a4-8418fa687597.gif)
+
+#### pipgeo sys
+This will install all packages from the release assets onto your system. It maintains prerequisite and dependency order to allow for easy installation.
+
+Example usage
+
+```
+pipgeo sys
+```
+
+![pipgeo-sys](https://user-images.githubusercontent.com/6677629/212253237-9bbd32c0-3312-4a8b-8661-887f7422b45b.gif)
+
+### Changelog
+
+#### v0.0.6
+- release checker tool now checks if packages exists for installed python version in latest release
+
+#### v0.0.5
+- release tool now print available release packages and version number
+- improved pypi version check functionality
+- fetch tool auto upgrades to latest version if new version is available in release
+
+#### v0.0.4
+- added dependency check from dependency tree
+- dependencies also installed using pipgeo
+
+#### v0.0.3
+- updated readme with instructions
```

### Comparing `pipgeo-0.0.5/setup.py` & `pipgeo-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setuptools.setup(
     name="pipgeo",
-    version="0.0.5",
+    version="0.0.6",
     packages=find_packages(),
     url="https://github.com/samapriya/pipgeo",
     install_requires=[
         "wheel>=0.38.4",
         "requests>=2.28.1",
         "beautifulsoup4>=4.11.1",
-        "setuptools>=41.2.0"
+        "setuptools>=41.2.0",
+        "natsort>=8.3.1"
     ],
     license="Apache 2.0",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "Natural Language :: English",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: GIS",
     ],
     author="Samapriya Roy",
```

