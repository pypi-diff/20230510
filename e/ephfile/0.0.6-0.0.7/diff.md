# Comparing `tmp/ephfile-0.0.6.tar.gz` & `tmp/ephfile-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ephfile-0.0.6.tar", last modified: Thu Mar 23 21:33:27 2023, max compression
+gzip compressed data, was "ephfile-0.0.7.tar", last modified: Wed May 10 13:05:07 2023, max compression
```

## Comparing `ephfile-0.0.6.tar` & `ephfile-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:33:27.975126 ephfile-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-23 21:33:22.000000 ephfile-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-23 21:33:27.975126 ephfile-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-23 21:33:22.000000 ephfile-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:33:27.971126 ephfile-0.0.6/ephfile/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2907 2023-03-23 21:33:22.000000 ephfile-0.0.6/ephfile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 21:33:27.975126 ephfile-0.0.6/ephfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-23 21:33:27.000000 ephfile-0.0.6/ephfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-23 21:33:27.000000 ephfile-0.0.6/ephfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 21:33:27.000000 ephfile-0.0.6/ephfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-23 21:33:27.000000 ephfile-0.0.6/ephfile.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 21:33:27.975126 ephfile-0.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3149 2023-03-23 21:33:22.000000 ephfile-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:05:07.032236 ephfile-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 13:05:02.000000 ephfile-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 13:05:07.032236 ephfile-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-10 13:05:02.000000 ephfile-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:05:07.032236 ephfile-0.0.7/ephfile/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-05-10 13:05:02.000000 ephfile-0.0.7/ephfile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:05:07.032236 ephfile-0.0.7/ephfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-10 13:05:06.000000 ephfile-0.0.7/ephfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-10 13:05:07.000000 ephfile-0.0.7/ephfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:05:06.000000 ephfile-0.0.7/ephfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 13:05:06.000000 ephfile-0.0.7/ephfile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 13:05:07.032236 ephfile-0.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3149 2023-05-10 13:05:02.000000 ephfile-0.0.7/setup.py
```

### Comparing `ephfile-0.0.6/LICENSE` & `ephfile-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ephfile-0.0.6/ephfile/__init__.py` & `ephfile-0.0.7/ephfile/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 					import pathlib
 					pathlib.Path(foil).touch()
 				except Exception as  e:
 					pass
 			self.foil = foil
 		self.contents_lambda = contents_lambda or to_str
 
-		if contents:
-			if not isinstance(contents,list):
-				contents = [contents]
-		elif isinstance(contents,str):
+		if isinstance(contents,list):
+			contents = "\n".join(contents)
+
+		if isinstance(contents,str):
 			contents = contents.split('\n')
 			for cont in contents:
 				contz = self.contents_lambda(cont)
 				if self.named:
 					self.named.write(str.encode(contz + "\n"))
 				else:
 					with open(self.foil,"a+") as writer:
@@ -89,17 +89,15 @@
 		if newpathwithin != '':
 			print(self.dir)
 			newpath = self()+"/"+newpathwithin
 			print(newpath)
 			os.system("mkdir -p {0}".format(newpath))
 		else:
 			newpath = self()
-		print("before")
 		shutil.copyfile(ephfile,str(newpath)+"/"+str(ephfile))
-		print("after")
 
 	def __iadd__(self,contentobj):
 		if isinstance(contentobj,ephdir):
 			newpath = self()+"/"+currentobj()
 			os.system("mkdir -p {0}".format(newpath))
 			for foil in currentobj.files:
 				self.addephfileto(ephfile(),newpath)
@@ -112,14 +110,15 @@
 		return self.dir
 
 	def __enter__(self):
 		return self
 
 	def close(self):
 		try:
+			print("yes|rm -r " + str(self.dir))
 			os.system("yes|rm -r " + str(self.dir))
 		except Exception as e:
 			pass
 	
 	def __exit__(self, exc_type, exc_val, exc_tb):
 		self.close()
 		return self
```

### Comparing `ephfile-0.0.6/setup.py` & `ephfile-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.6"
+VERSION = "0.0.7"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

