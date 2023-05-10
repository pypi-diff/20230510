# Comparing `tmp/rwpp-0.1.1.tar.gz` & `tmp/rwpp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwpp-0.1.1.tar", max compression
+gzip compressed data, was "rwpp-0.1.2.tar", max compression
```

## Comparing `rwpp-0.1.1.tar` & `rwpp-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1036 2023-04-23 17:24:52.284417 rwpp-0.1.1/LICENSE
--rw-r--r--   0        0        0     4091 2023-04-30 18:16:20.252021 rwpp-0.1.1/README.md
--rw-r--r--   0        0        0      458 2023-04-30 18:20:58.860055 rwpp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-23 17:24:52.284417 rwpp-0.1.1/rwpp/__init__.py
--rw-r--r--   0        0        0     3230 2023-04-30 17:27:19.744237 rwpp-0.1.1/rwpp/main.py
--rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 rwpp-0.1.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1036 2023-05-04 15:24:54.106930 rwpp-0.1.2/LICENSE
+-rwxr-xr-x   0        0        0     4091 2023-05-04 15:24:54.106930 rwpp-0.1.2/README.md
+-rwxr-xr-x   0        0        0      458 2023-05-10 05:38:14.705489 rwpp-0.1.2/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2023-05-04 15:24:54.110263 rwpp-0.1.2/rwpp/__init__.py
+-rwxr-xr-x   0        0        0     3256 2023-05-10 04:57:26.244100 rwpp-0.1.2/rwpp/main.py
+-rw-r--r--   0        0        0     4711 1970-01-01 00:00:00.000000 rwpp-0.1.2/PKG-INFO
```

### Comparing `rwpp-0.1.1/LICENSE` & `rwpp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rwpp-0.1.1/README.md` & `rwpp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rwpp-0.1.1/rwpp/main.py` & `rwpp-0.1.2/rwpp/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,33 +19,35 @@
     downloaded_images = os.listdir(f"{download_path}/{subreddit}")
 
     accepted_formats = [".jpg", ".jpeg", ".png"]
 
     if sort_by:
         client = redditwarp.SYNC.Client()
         method = getattr(client.p.subreddit.pull, sort_by)
-        if time and callable(getattr(method, '__call__')) and len(inspect.signature(method).parameters) == 2:
+        if (
+            time
+            and callable(getattr(method, "__call__"))
+            and len(inspect.signature(method).parameters) == 2
+        ):
             # The method doesn't accept any parameters, so don't pass `time`
-            raise ValueError(
-                f"Method '{sort_by}' doesn't accept any parameters.")
+            raise ValueError(f"Method '{sort_by}' doesn't accept any parameters.")
         elif time:
             # The method accepts a `time` parameter, so pass it
             posts = method(subreddit, amount=limit, time=time)
         else:
             # The method doesn't accept a `time` parameter, so call it without the `time` argument
             posts = method(subreddit, amount=limit)
     else:
         raise ValueError("sort_by parameter is missing or invalid.")
 
     for post in posts:
         if not isinstance(post, LinkPost):
             continue
         if post.link.split("/")[-1] not in downloaded_images:
             if post.link.endswith(tuple(accepted_formats)):
-
                 # Retrive the image
                 r = requests.get(post.link)
 
                 # Save image to file
                 with open(
                     f"{download_path}/{subreddit}/{post.link.split('/')[-1]}", "wb"
                 ) as f:
@@ -59,38 +61,39 @@
         else:
             typer.echo("Image already downloaded...")
 
 
 # @app.callback()
 def main(
     subreddit: str = typer.Argument(
-        ...,
-        help="The given subreddit(s) to pull images from"
+        ..., help="The given subreddit(s) to pull images from"
     ),
     limit: int = typer.Option(
         10,
         help="The amount of posts to pull from subreddit(s)",
-        prompt="How many images would you like to download? "
+        prompt="How many images would you like to download? ",
     ),
     download_path: str = typer.Option(
         "./downloads",
         help="The path where you would like to save images",
-        prompt="Where would you like to save the images? "
+        prompt="Where would you like to save the images? ",
     ),
     sort_by: str = typer.Option(
         "hot",
         help="The sort order to pull images by",
-        prompt="Sort order for images?: [hot, new, top, rising] "
+        prompt="Sort order for images?: [hot, new, top, rising] ",
     ),
-    time: str = typer.Option(
-        "",
-        help="The time period to pull images from, only needed for top posts",
-        prompt="Time period for images? (Only needed for top posts): [hour, day, week, month, year, all] "
-    )
 ):
+    # Prompt for time option only if sort_by is top
+    if sort_by == "top":
+        time = typer.prompt(
+            "Time period would you like to sort top by? [hour, day, week, month, year] "
+        )
+    else:
+        time = None
     download(subreddit, limit, download_path, time, sort_by)
 
 
 # Main function to be called from terminal
 @app.callback()
 def cli():
     typer.run(main)
```

### Comparing `rwpp-0.1.1/PKG-INFO` & `rwpp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwpp
-Version: 0.1.1
+Version: 0.1.2
 Summary: Reddit Wallpaper Puller, a simple CLI to pull wallpapers from Reddit.
 Author: Ducky
 Author-email: duckbox007@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

