# Comparing `tmp/hget-1.0.5-7-py2.py3-none-any.whl.zip` & `tmp/hget-1.0.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 14036 bytes, number of entries: 11
--rw-r--r--  2.0 unx       56 b- defN 22-Dec-16 03:17 hget/__init__.py
--rw-r--r--  2.0 unx       22 b- defN 22-Dec-16 03:17 hget/_version.py
--rw-r--r--  2.0 unx      695 b- defN 22-Dec-16 03:17 hget/main.py
--rw-r--r--  2.0 unx    18672 b- defN 23-Mar-23 09:39 hget/src.py
--rw-r--r--  2.0 unx    10088 b- defN 22-Dec-16 03:17 hget/utils.py
--rw-r--r--  2.0 unx     1094 b- defN 23-Apr-12 09:06 hget-1.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     7104 b- defN 23-Apr-12 09:06 hget-1.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx      119 b- defN 23-Apr-12 09:06 hget-1.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       40 b- defN 23-Apr-12 09:06 hget-1.0.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-12 09:06 hget-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      813 b- defN 23-Apr-12 09:06 hget-1.0.5.dist-info/RECORD
-11 files, 38708 bytes uncompressed, 12680 bytes compressed:  67.2%
+Zip file size: 14143 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       56 b- defN 23-Apr-14 02:58 hget/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 23-May-10 08:40 hget/_version.py
+-rw-r--r--  2.0 unx      713 b- defN 23-May-10 08:17 hget/main.py
+-rw-r--r--  2.0 unx    18917 b- defN 23-May-10 08:27 hget/src.py
+-rw-r--r--  2.0 unx    10293 b- defN 23-May-10 08:34 hget/utils.py
+-rw-r--r--  2.0 unx     1094 b- defN 23-May-10 09:39 hget-1.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7104 b- defN 23-May-10 09:39 hget-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-10 09:39 hget-1.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       40 b- defN 23-May-10 09:39 hget-1.0.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 23-May-10 09:39 hget-1.0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      813 b- defN 23-May-10 09:39 hget-1.0.6.dist-info/RECORD
+11 files, 39167 bytes uncompressed, 12787 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: hget/src.py
 Comment: 
 
 Filename: hget/utils.py
 Comment: 
 
-Filename: hget-1.0.5.dist-info/LICENSE
+Filename: hget-1.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: hget-1.0.5.dist-info/METADATA
+Filename: hget-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: hget-1.0.5.dist-info/WHEEL
+Filename: hget-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: hget-1.0.5.dist-info/entry_points.txt
+Filename: hget-1.0.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: hget-1.0.5.dist-info/top_level.txt
+Filename: hget-1.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: hget-1.0.5.dist-info/RECORD
+Filename: hget-1.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hget/_version.py

```diff
@@ -1 +1 @@
-__version__ = "1.0.5"
+__version__ = "1.0.6"
```

## hget/main.py

```diff
@@ -15,15 +15,15 @@
         log.setLevel(logging.DEBUG)
     outfile = args.output
     if not outfile and args.dir:
         outfile = os.path.join(args.dir, os.path.basename(args.url))
     hget(args.url, outfile, args.num, quiet=args.quiet,
          tcp_conn=args.connections, timeout=args.timeout,
          access_key=args.access_key, secrets_key=args.secrets_key,
-         max_speed=args.max_speed)
+         max_speed=args.max_speed, proxy=args.proxy)
 
 
 def main():
     args = parseArg()
     if args.use_reloader:
         autoreloader(_main, args)
     else:
```

## hget/src.py

```diff
@@ -57,15 +57,19 @@
             self.content_length = content_length
             self.loger.debug("%s of %s has download" %
                              (self.tqdm_init, self.content_length))
         else:
             req = await self.fetch(session)
             if not isinstance(req, int):
                 if 400 <= req.status < 500:
-                    raise DownloadError("ERROR %s: %s bad request" %(req.status, self.url))
+                    raise DownloadError(
+                        "Client ERROR %s: %s bad request" % (req.status, self.url))
+                elif 500 <= req.status:
+                    raise DownloadError(
+                        "Server ERROR %s: %s bad request" % (req.status, self.url))
                 content_length = int(req.headers['content-length'])
             else:
                 content_length = req
             self.content_length = content_length
             if self.content_length < 1:
                 self.offset = {}
                 self.loger.error(
@@ -101,15 +105,15 @@
                 mkfile(self.outfile, self.content_length)
             self.write_offset()
 
     async def download(self):
         self.timeout = ClientTimeout(total=60*60*24, sock_read=2400)
         self.connector = TCPConnector(
             limit=self.tcp_conn, ssl=False)
-        async with ClientSession(connector=self.connector, timeout=self.timeout) as session:
+        async with ClientSession(connector=self.connector, timeout=self.timeout, trust_env=True) as session:
             await self.get_range(session)
             _thread.start_new_thread(self.check_offset, (self.datatimeout,))
             _thread.start_new_thread(self._auto_write_offset, ())
             self.set_sem(self.threads)
             if os.getenv("RUN_HGET_FIRST") != 'false':
                 self.loger.info("File size: %s (%d bytes)",
                                 human_size(self.content_length), self.content_length)
@@ -183,15 +187,15 @@
     async def fetch(self, session, pbar=None, headers=None):
         if headers:
             async with self.sem:
                 s, e = headers["Range"]
                 headers["Range"] = 'bytes={0}-{1}'.format(s, e)
                 self.loger.debug(
                     "Start %s %s", asyncio.current_task().get_name(), headers["Range"])
-                async with session.get(self.url, headers=headers, timeout=self.timeout, params=self.extra) as req:
+                async with session.get(self.url, headers=headers, timeout=self.timeout, params=self.extra, proxy=self.extra.get("proxy")) as req:
                     with open(self.outfile, 'r+b') as f:
                         f.seek(s, os.SEEK_SET)
                         async for chunk in req.content.iter_chunked(self.chunk_size):
                             if chunk:
                                 self.rate_limiter.wait()
                                 f.write(chunk)
                                 f.flush()
```

## hget/utils.py

```diff
@@ -239,14 +239,16 @@
     parser.add_argument('-v', '--version',
                         action='version', version="v" + __version__)
     aws = parser.add_argument_group("aws arguments")
     aws.add_argument('--access-key', dest='access_key', type=str,
                      help='access key if necessary', metavar="<str>")
     aws.add_argument('--secrets-key', dest='secrets_key', type=str,
                      help='secrets key if necessary', metavar="<str>")
+    parser.add_argument('-p', '--proxy', type=str,
+                        help='proxy url, statswith http/https, HTTP_PROXY or HTTPS_PROXY environment variables will be read by default', metavar="<str>")
     parser.add_argument('--noreload', dest='use_reloader', action='store_false',
                         help='tells hget to NOT use the auto-reloader')
     parser.add_argument("url", type=str,
                         help="download url, http/https/ftp/s3 support", metavar="<url>")
     return parser.parse_args()
```

## Comparing `hget-1.0.5.dist-info/LICENSE` & `hget-1.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `hget-1.0.5.dist-info/METADATA` & `hget-1.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hget
-Version: 1.0.5
+Version: 1.0.6
 Home-page: https://github.com/yodeng/hget
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Cython
 Requires-Dist: requests
```

