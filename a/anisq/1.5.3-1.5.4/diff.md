# Comparing `tmp/anisq-1.5.3.tar.gz` & `tmp/anisq-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anisq-1.5.3.tar", last modified: Mon Apr  3 20:50:09 2023, max compression
+gzip compressed data, was "anisq-1.5.4.tar", last modified: Wed May 10 17:09:04 2023, max compression
```

## Comparing `anisq-1.5.3.tar` & `anisq-1.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0 denis     (1000) denis     (1000)        0 2023-04-03 20:50:09.483422 anisq-1.5.3/
--rwxrwxrwx   0 denis     (1000) denis     (1000)      596 2023-04-03 20:50:09.479423 anisq-1.5.3/PKG-INFO
--rwxrwxrwx   0 denis     (1000) denis     (1000)     2346 2023-03-18 12:11:07.000000 anisq-1.5.3/README.md
-drwxrwxrwx   0 denis     (1000) denis     (1000)        0 2023-04-03 20:50:09.276524 anisq-1.5.3/anisq/
--rwxrwxrwx   0 denis     (1000) denis     (1000)        0 2023-03-18 12:11:07.000000 anisq-1.5.3/anisq/__init__.py
--rwxrwxrwx   0 denis     (1000) denis     (1000)    14338 2023-04-03 20:49:25.000000 anisq-1.5.3/anisq/anisq.py
-drwxrwxrwx   0 denis     (1000) denis     (1000)        0 2023-04-03 20:50:09.447357 anisq-1.5.3/anisq.egg-info/
--rwxrwxrwx   0 denis     (1000) denis     (1000)      596 2023-04-03 20:50:09.000000 anisq-1.5.3/anisq.egg-info/PKG-INFO
--rwxrwxrwx   0 denis     (1000) denis     (1000)      227 2023-04-03 20:50:09.000000 anisq-1.5.3/anisq.egg-info/SOURCES.txt
--rwxrwxrwx   0 denis     (1000) denis     (1000)        1 2023-04-03 20:50:09.000000 anisq-1.5.3/anisq.egg-info/dependency_links.txt
--rwxrwxrwx   0 denis     (1000) denis     (1000)       44 2023-04-03 20:50:09.000000 anisq-1.5.3/anisq.egg-info/entry_points.txt
--rwxrwxrwx   0 denis     (1000) denis     (1000)       31 2023-04-03 20:50:09.000000 anisq-1.5.3/anisq.egg-info/requires.txt
--rwxrwxrwx   0 denis     (1000) denis     (1000)        6 2023-04-03 20:50:09.000000 anisq-1.5.3/anisq.egg-info/top_level.txt
--rwxrwxrwx   0 denis     (1000) denis     (1000)       38 2023-04-03 20:50:09.485482 anisq-1.5.3/setup.cfg
--rwxrwxrwx   0 denis     (1000) denis     (1000)     1122 2023-04-03 20:50:00.000000 anisq-1.5.3/setup.py
+drwxrwxrwx   0 denis     (1000) denis     (1000)        0 2023-05-10 17:09:04.575316 anisq-1.5.4/
+-rwxrwxrwx   0 denis     (1000) denis     (1000)      596 2023-05-10 17:09:04.569786 anisq-1.5.4/PKG-INFO
+-rwxrwxrwx   0 denis     (1000) denis     (1000)     2346 2023-03-18 12:11:07.000000 anisq-1.5.4/README.md
+drwxrwxrwx   0 denis     (1000) denis     (1000)        0 2023-05-10 17:09:04.330355 anisq-1.5.4/anisq/
+-rwxrwxrwx   0 denis     (1000) denis     (1000)        0 2023-03-18 12:11:07.000000 anisq-1.5.4/anisq/__init__.py
+-rwxrwxrwx   0 denis     (1000) denis     (1000)    14415 2023-05-10 16:59:21.000000 anisq-1.5.4/anisq/anisq.py
+drwxrwxrwx   0 denis     (1000) denis     (1000)        0 2023-05-10 17:09:04.529655 anisq-1.5.4/anisq.egg-info/
+-rwxrwxrwx   0 denis     (1000) denis     (1000)      596 2023-05-10 17:09:04.000000 anisq-1.5.4/anisq.egg-info/PKG-INFO
+-rwxrwxrwx   0 denis     (1000) denis     (1000)      227 2023-05-10 17:09:04.000000 anisq-1.5.4/anisq.egg-info/SOURCES.txt
+-rwxrwxrwx   0 denis     (1000) denis     (1000)        1 2023-05-10 17:09:04.000000 anisq-1.5.4/anisq.egg-info/dependency_links.txt
+-rwxrwxrwx   0 denis     (1000) denis     (1000)       44 2023-05-10 17:09:04.000000 anisq-1.5.4/anisq.egg-info/entry_points.txt
+-rwxrwxrwx   0 denis     (1000) denis     (1000)       31 2023-05-10 17:09:04.000000 anisq-1.5.4/anisq.egg-info/requires.txt
+-rwxrwxrwx   0 denis     (1000) denis     (1000)        6 2023-05-10 17:09:04.000000 anisq-1.5.4/anisq.egg-info/top_level.txt
+-rwxrwxrwx   0 denis     (1000) denis     (1000)       38 2023-05-10 17:09:04.577316 anisq-1.5.4/setup.cfg
+-rwxrwxrwx   0 denis     (1000) denis     (1000)     1122 2023-05-10 17:06:54.000000 anisq-1.5.4/setup.py
```

### Comparing `anisq-1.5.3/PKG-INFO` & `anisq-1.5.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anisq
-Version: 1.5.3
+Version: 1.5.4
 Summary: Streaming / Downloading Albanian Subtitled Anime
 Home-page: UNKNOWN
 Author: deniscerri (Denis Çerri)
 Author-email: 64997243+deniscerri@users.noreply.github.com
 License: UNKNOWN
 Keywords: python,video,stream,anime,albanian
 Platform: UNKNOWN
```

### Comparing `anisq-1.5.3/README.md` & `anisq-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `anisq-1.5.3/anisq/anisq.py` & `anisq-1.5.4/anisq/anisq.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,31 +57,34 @@
 	try:
 		return BeautifulSoup(scraper.post(URL).text, "html.parser")
 	except:
 		return ""
 
 
 def mp4_upload(URL):
-	URL=URL.replace("embed-","").replace(".html","")
-	html=requests.get(URL).text
-	soup=BeautifulSoup(html,'html.parser')
-	
-	params=dict()
-	inputs=soup.find_all('input')
-	for item in inputs:
-		params.update({item['name']:item['value']})
-	response=requests.post(URL,data=params).text
-
-	soup=BeautifulSoup(response, 'html.parser')
-	params=dict()
-	inputs=soup.find_all('input')
-	for item in inputs:
-		params.update({item['name']:item['value']})
-	response=requests.post(URL,data=params,verify=False,allow_redirects=False).headers['Location']
-	return response
+	try:
+		URL=URL.replace("embed-","").replace(".html","")
+		html=requests.get(URL).text
+		soup=BeautifulSoup(html,'html.parser')
+		
+		params=dict()
+		inputs=soup.find_all('input')
+		for item in inputs:
+			params.update({item['name']:item['value']})
+		response=requests.post(URL,data=params).text
+
+		soup=BeautifulSoup(response, 'html.parser')
+		params=dict()
+		inputs=soup.find_all('input')
+		for item in inputs:
+			params.update({item['name']:item['value']})
+		response=requests.post(URL,data=params,verify=False,allow_redirects=False).headers['Location']
+		return response
+	except:
+		return ""
 
 def help_text():
 	print("""
 Usage:
 	anisq [options] [input title or file]
 Options:
 	-h show this page
@@ -216,15 +219,15 @@
 
 	if not Config.watch:
 		if (Config.title == ''):
 			Config.title = page.xpath('//*[@id="info"]/h1/text()')[0]
 			fix_title()
 
 		if Config.media_type == 'seriale':
-			split_title = str(embed_title).split(" ")
+			split_title = [x.replace(' ', '') for x in str(embed_title).split(":")]
 			season_nr = split_title[len(split_title)-1].split("x")[0]
 			episode_nr = split_title[len(split_title)-1].split("x")[1]
 			Config.output_path = f"{Config.root_path}/{Config.title}/{Config.title} - S{season_nr}E{episode_nr}.mkv"
 		
 			if os.path.exists(str(Config.output_path)):
 				if is_file_incomplete():
 					print(f"{Green}Episode is Downloaded. {White}")
@@ -242,18 +245,18 @@
 	video = ''
 	for referer in referers:
 		if 'fembed' in referer or 'suzihaza' in referer or 'femax' in referer:
 			print(f"{LYellow}Trying to download from stream: {referer}{White}")
 			referer = re.sub("/v/", '/f/', referer)
 			videoid = re.sub(".*/f/", '', referer)
 			res = str(post_request(f'https://vanfem.com/api/source/{videoid}'))
-			res = json.loads(res)
 
 			
 			try:
+				res = json.loads(res)
 				video = res['data'][len(res['data'])-1]['file']
 			except:
 				video = ''
 			res = download(referer, video)
 			if (res == 0):
 				break
```

### Comparing `anisq-1.5.3/anisq.egg-info/PKG-INFO` & `anisq-1.5.4/anisq.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anisq
-Version: 1.5.3
+Version: 1.5.4
 Summary: Streaming / Downloading Albanian Subtitled Anime
 Home-page: UNKNOWN
 Author: deniscerri (Denis Çerri)
 Author-email: 64997243+deniscerri@users.noreply.github.com
 License: UNKNOWN
 Keywords: python,video,stream,anime,albanian
 Platform: UNKNOWN
```

### Comparing `anisq-1.5.3/setup.py` & `anisq-1.5.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.5.3'
+VERSION = '1.5.4'
 DESCRIPTION = 'Streaming / Downloading Albanian Subtitled Anime'
 
 # Setting up
 setup(
     name="anisq",
     version=VERSION,
     author="deniscerri (Denis Çerri)",
```

