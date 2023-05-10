# Comparing `tmp/eternalegypt-0.0.8.tar.gz` & `tmp/eternalegypt-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eternalegypt-0.0.8.tar", last modified: Sun Jul 28 11:11:09 2019, max compression
+gzip compressed data, was "dist/eternalegypt-0.0.9.tar", last modified: Thu Aug 15 17:10:42 2019, max compression
```

## Comparing `eternalegypt-0.0.8.tar` & `eternalegypt-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 am         (501) staff       (20)        0 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/
--rw-r--r--   0 am         (501) staff       (20)      439 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/PKG-INFO
-drwxr-xr-x   0 am         (501) staff       (20)        0 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/eternalegypt.egg-info/
--rw-r--r--   0 am         (501) staff       (20)      439 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/eternalegypt.egg-info/PKG-INFO
--rw-r--r--   0 am         (501) staff       (20)      285 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/eternalegypt.egg-info/SOURCES.txt
--rw-r--r--   0 am         (501) staff       (20)       21 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/eternalegypt.egg-info/requires.txt
--rw-r--r--   0 am         (501) staff       (20)       13 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/eternalegypt.egg-info/top_level.txt
--rw-r--r--   0 am         (501) staff       (20)        1 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/eternalegypt.egg-info/dependency_links.txt
--rw-r--r--   0 am         (501) staff       (20)       68 2017-06-22 21:18:06.000000 eternalegypt-0.0.8/MANIFEST.in
--rw-r--r--   0 am         (501) staff       (20)      409 2018-08-27 19:59:44.000000 eternalegypt-0.0.8/README.md
--rw-r--r--   0 am         (501) staff       (20)      591 2019-07-28 11:06:57.000000 eternalegypt-0.0.8/setup.py
--rw-r--r--   0 am         (501) staff       (20)       79 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/setup.cfg
-drwxr-xr-x   0 am         (501) staff       (20)        0 2019-07-28 11:11:09.000000 eternalegypt-0.0.8/eternalegypt/
--rw-r--r--   0 am         (501) staff       (20)     9152 2019-07-28 11:06:46.000000 eternalegypt-0.0.8/eternalegypt/eternalegypt.py
--rw-r--r--   0 am         (501) staff       (20)       39 2018-09-22 21:58:58.000000 eternalegypt-0.0.8/eternalegypt/__init__.py
--rw-r--r--   0 am         (501) staff       (20)     1081 2018-03-10 22:53:46.000000 eternalegypt-0.0.8/LICENSE.txt
+drwxr-xr-x   0 am         (501) staff       (20)        0 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/
+-rw-r--r--   0 am         (501) staff       (20)      439 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/PKG-INFO
+drwxr-xr-x   0 am         (501) staff       (20)        0 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/eternalegypt.egg-info/
+-rw-r--r--   0 am         (501) staff       (20)      439 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/eternalegypt.egg-info/PKG-INFO
+-rw-r--r--   0 am         (501) staff       (20)      285 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/eternalegypt.egg-info/SOURCES.txt
+-rw-r--r--   0 am         (501) staff       (20)       34 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/eternalegypt.egg-info/requires.txt
+-rw-r--r--   0 am         (501) staff       (20)       13 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/eternalegypt.egg-info/top_level.txt
+-rw-r--r--   0 am         (501) staff       (20)        1 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/eternalegypt.egg-info/dependency_links.txt
+-rw-r--r--   0 am         (501) staff       (20)       68 2017-06-22 21:18:06.000000 eternalegypt-0.0.9/MANIFEST.in
+-rw-r--r--   0 am         (501) staff       (20)      409 2018-08-27 19:59:44.000000 eternalegypt-0.0.9/README.md
+-rw-r--r--   0 am         (501) staff       (20)      606 2019-08-15 17:06:46.000000 eternalegypt-0.0.9/setup.py
+-rw-r--r--   0 am         (501) staff       (20)       79 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/setup.cfg
+drwxr-xr-x   0 am         (501) staff       (20)        0 2019-08-15 17:10:42.000000 eternalegypt-0.0.9/eternalegypt/
+-rw-r--r--   0 am         (501) staff       (20)     9809 2019-08-15 17:06:31.000000 eternalegypt-0.0.9/eternalegypt/eternalegypt.py
+-rw-r--r--   0 am         (501) staff       (20)       39 2018-09-22 21:58:58.000000 eternalegypt-0.0.9/eternalegypt/__init__.py
+-rw-r--r--   0 am         (501) staff       (20)     1081 2018-03-10 22:53:46.000000 eternalegypt-0.0.9/LICENSE.txt
```

### Comparing `eternalegypt-0.0.8/eternalegypt/eternalegypt.py` & `eternalegypt-0.0.9/eternalegypt/eternalegypt.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import json
 from functools import wraps
 from datetime import datetime
 import asyncio
 from aiohttp.client_exceptions import ClientError
 import async_timeout
 import attr
+import flatten_json
 
 TIMEOUT = 3
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Error(Exception):
@@ -44,14 +45,15 @@
     roaming = attr.ib(default=None)
     radio_quality = attr.ib(default=None)
     rx_level = attr.ib(default=None)
     tx_level = attr.ib(default=None)
     current_band = attr.ib(default=None)
     cell_id = attr.ib(default=None)
     sms = attr.ib(factory=list)
+    everything = attr.ib(factory=dict)
 
 
 def autologin(function, timeout=TIMEOUT):
     """Decorator that will try to login and redo an action before failing."""
     @wraps(function)
     async def wrapper(self, *args, **kwargs):
         """Wrap a function with timeout."""
@@ -100,34 +102,38 @@
     async def logout(self):
         """Cleanup resources."""
         self.websession = None
         self.token = None
 
     async def login(self, password=None):
         """Create a session with the modem."""
+        # Work around missing https://github.com/aio-libs/aiohttp/pull/3576
+        try:
+            await self._login(password)
+        except (asyncio.TimeoutError, ClientError, Error):
+            await self._login(password)
+
+    async def _login(self, password=None):
+        """Create a session with the modem."""
         if password is None:
             password = self.password
         else:
             self.password = password
 
         try:
             async with async_timeout.timeout(TIMEOUT):
-                url = self._url('index.html')
+                url = self._url('model.json')
                 async with self.websession.get(url) as response:
-                    text = await response.text()
-
-                    match = re.search(r'name="token" value="(.*?)"', text)
-                    if not match:
-                        match = re.search(r'"secToken": "(.*?)"', text)
+                    data = json.loads(await response.text())
+                    self.token = data.get('session', {}).get('secToken')
 
-                    if not match:
+                    if self.token is None:
                         _LOGGER.error("No token found during login")
                         raise Error()
 
-                    self.token = match.group(1)
                     _LOGGER.debug("Token: %s", self.token)
 
                 url = self._url('Forms/config')
                 data = {
                     'session.password': password,
                     'token': self.token
                 }
@@ -162,14 +168,20 @@
             'err_redirect': '/error.json',
             'ok_redirect': '/success.json',
             'token': self.token
         }
         return self.websession.post(url, data=data)
 
     @autologin
+    async def disconnect_lte(self):
+        """Do an LTE disconnect."""
+        async with self._config_call('wwan.connect', 'Disconnect') as response:
+            _LOGGER.debug("Disconnected LTE with status %d", response.status)
+
+    @autologin
     async def connect_lte(self):
         """Do an LTE reconnect."""
         async with self._config_call('wwan.connect', 'DefaultProfile') as response:
             _LOGGER.debug("Connected to LTE with status %d", response.status)
 
     @autologin
     async def delete_sms(self, sms_id):
@@ -238,14 +250,20 @@
             # {'id': '6', 'rxTime': '11/03/18 08:18:11 PM', 'text': 'tak tik',
             #  'sender': '555-987-654', 'read': False}
             dt = datetime.strptime(msg['rxTime'], '%d/%m/%y %I:%M:%S %p')
             element = SMS(int(msg['id']), dt, not msg['read'], msg['sender'], msg['text'])
             result.sms.append(element)
         result.sms.sort(key=lambda sms: sms.id)
 
+        result.everything = {
+            key.lower(): value
+            for key, value in flatten_json.flatten(data, '.').items()
+            if value != {}
+        }
+
         return result
 
     @autologin
     async def information(self):
         """Return the current information."""
         url = self._url('model.json')
         async with self.websession.get(url) as response:
```

### Comparing `eternalegypt-0.0.8/LICENSE.txt` & `eternalegypt-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

