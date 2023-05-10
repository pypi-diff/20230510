# Comparing `tmp/weesocket-1.0.1.tar.gz` & `tmp/weesocket-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weesocket-1.0.1.tar", last modified: Sat Aug 20 15:47:55 2022, max compression
+gzip compressed data, was "weesocket-2.0.0.tar", last modified: Wed May 10 12:10:37 2023, max compression
```

## Comparing `weesocket-1.0.1.tar` & `weesocket-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2022-08-20 15:47:55.885277 weesocket-1.0.1/
--rw-r--r--   0 katry     (1000) katry     (1001)    34701 2022-08-20 12:34:44.000000 weesocket-1.0.1/LICENSE
--rw-r--r--   0 katry     (1000) katry     (1001)      943 2022-08-20 15:47:55.885277 weesocket-1.0.1/PKG-INFO
--rw-r--r--   0 katry     (1000) katry     (1001)      392 2022-08-20 13:48:08.000000 weesocket-1.0.1/README.md
--rw-r--r--   0 katry     (1000) katry     (1001)       38 2022-08-20 15:47:55.885277 weesocket-1.0.1/setup.cfg
--rw-r--r--   0 katry     (1000) katry     (1001)      800 2022-08-20 14:36:26.000000 weesocket-1.0.1/setup.py
-drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2022-08-20 15:47:55.875277 weesocket-1.0.1/weesocket/
--rw-r--r--   0 katry     (1000) katry     (1001)       77 2022-08-20 15:47:01.000000 weesocket-1.0.1/weesocket/__init__.py
--rw-r--r--   0 katry     (1000) katry     (1001)     3480 2022-08-20 13:27:39.000000 weesocket-1.0.1/weesocket/abstract.py
--rw-r--r--   0 katry     (1000) katry     (1001)     3376 2022-08-20 15:47:45.000000 weesocket-1.0.1/weesocket/client.py
--rw-r--r--   0 katry     (1000) katry     (1001)     5478 2022-08-20 15:47:51.000000 weesocket-1.0.1/weesocket/server.py
-drwxr-xr-x   0 katry     (1000) katry     (1001)        0 2022-08-20 15:47:55.885277 weesocket-1.0.1/weesocket.egg-info/
--rw-r--r--   0 katry     (1000) katry     (1001)      943 2022-08-20 15:47:55.000000 weesocket-1.0.1/weesocket.egg-info/PKG-INFO
--rw-r--r--   0 katry     (1000) katry     (1001)      274 2022-08-20 15:47:55.000000 weesocket-1.0.1/weesocket.egg-info/SOURCES.txt
--rw-r--r--   0 katry     (1000) katry     (1001)        1 2022-08-20 15:47:55.000000 weesocket-1.0.1/weesocket.egg-info/dependency_links.txt
--rw-r--r--   0 katry     (1000) katry     (1001)       69 2022-08-20 15:47:55.000000 weesocket-1.0.1/weesocket.egg-info/requires.txt
--rw-r--r--   0 katry     (1000) katry     (1001)       10 2022-08-20 15:47:55.000000 weesocket-1.0.1/weesocket.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:10:37.607843 weesocket-2.0.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34701 2023-05-07 19:09:58.000000 weesocket-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5687 2023-05-10 12:10:37.603843 weesocket-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5179 2023-05-08 12:49:59.000000 weesocket-2.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-10 12:10:37.607843 weesocket-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1120 2023-05-07 19:09:58.000000 weesocket-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:10:37.603843 weesocket-2.0.0/src/
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-05-10 12:10:35.000000 weesocket-2.0.0/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2023-05-07 22:25:35.000000 weesocket-2.0.0/src/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)     2824 2023-05-07 23:29:30.000000 weesocket-2.0.0/src/client.py
+-rw-rw-rw-   0 root         (0) root         (0)     5303 2023-05-08 09:44:03.000000 weesocket-2.0.0/src/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 12:10:37.603843 weesocket-2.0.0/weesocket.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5687 2023-05-10 12:10:37.000000 weesocket-2.0.0/weesocket.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-10 12:10:37.000000 weesocket-2.0.0/weesocket.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 12:10:37.000000 weesocket-2.0.0/weesocket.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-10 12:10:37.000000 weesocket-2.0.0/weesocket.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-10 12:10:37.000000 weesocket-2.0.0/weesocket.egg-info/top_level.txt
```

### Comparing `weesocket-1.0.1/LICENSE` & `weesocket-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weesocket-1.0.1/setup.py` & `weesocket-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 import setuptools
-from weesocket import __version__
+from src import __version__
+
+try:
+	from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
+
+	class bdist_wheel(_bdist_wheel):
+		def finalize_options(self):
+			_bdist_wheel.finalize_options(self)
+			self.root_is_pure = False
+except ImportError:
+	bdist_wheel = None  # type: ignore
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
+with open("requirements.txt") as rq:
+	required = rq.read().splitlines()
+
 setuptools.setup(
 	name="weesocket",
 	version=__version__,
 	author="Patrik Katrenak",
 	author_email="patrik@katryapps.com",
 	description="Tiny socket wrapper",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	url="https://gitlab.com/katry/weesocket",
-	packages=["weesocket"],
-	install_requires=["rsa"],
-	extras_require={
-		"orjson": ["orjson"],
-		"ujson": ["ujson"],
-		"dev": ["orjson", "pytest", "wheel", "twine"]
-	},
+
+	package_dir={"weesocket": "src"},
+	include_package_data=True,
+	install_requires=required,
+
 	classifiers=[
 		"Programming Language :: Python :: 3",
 		"License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
 		"Operating System :: OS Independent",
+		"Natural Language :: English",
 	],
+	cmdclass={"bdist_wheel": bdist_wheel},
 	platforms=["any"],
-	python_requires=">=3.9",
+	python_requires=">=3.10",
 )
```

### Comparing `weesocket-1.0.1/weesocket/client.py` & `weesocket-2.0.0/src/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,133 +1,110 @@
-from socket import socket, AF_UNIX, AF_INET, SOCK_STREAM
-from threading import Thread
 from rsa import PublicKey
+from .abstract import SocketAbstract
+from socket import (
+	socket,
+	AF_UNIX, AF_INET,
+	SOCK_STREAM, SHUT_RDWR
+)
 
-from .abstract import Socket, logger
 
-
-class Client(Socket):
+class Client(SocketAbstract):
 	def __init__(
-		self, trigger=None, alias=None, file=None, host="0.0.0.0",
-		port=6666, secret=None, server_secret=None, default_target=None
+		self, socket_file: str = "", host: str = "", port: int = 0,
+		encrypt: bool = True, secret: bytes = b"", remote_secret: bytes = b"",
+		buffer_size: int = 4096, public_key="", private_key="",
+		rsa_length: int = 2048, daemon: bool = True, logger=None
 	):
-		self._name = None
-		self._alias = alias
-		self._default_target = default_target
-		self._remotekey = None
-		self._authorized = True
-		self._thread = None
-
-		self.__enabled = False
-		self.__queue = []
-		self._secret = secret
-		if server_secret:
-			self._authorized = False
-			self._server_secret = server_secret
-		super().__init__(trigger=trigger, file=file, host=host, port=port, secrets=[secret], server_secret=server_secret)
+		if not socket_file and (not host or port < 1 or port > 65535):
+			raise OSError("Invalid connection settings")
+		self._socket = socket()
+		self._id = None
+		self._file = socket_file
+		self._host = host
+		self._port = port
+		self._buffer_size = buffer_size
+		self._remote_secret = remote_secret
+		self._open = False
+		self._queue = []
+		super().__init__(
+			encrypt=encrypt, secret=secret, logger=logger,
+			public_key=public_key, private_key=private_key,
+			rsa_length=rsa_length, daemon=daemon
+		)
 
-	def start(self):
-		self.__enabled = True
+	def run(self):
 		if self._file:
 			self._socket = socket(AF_UNIX, SOCK_STREAM)
 			self._socket.connect(self._file)
 		else:
 			self._socket = socket(AF_INET, SOCK_STREAM)
 			self._socket.connect((self._host, self._port))
-		self._thread = Thread(target=self.__on_message, args=())
-		self._thread.start()
+		self._socket.settimeout(2)
+		self._listen()
 
-	def connect(self):
-		self.start()
+	def send(self, data: dict, target=""):
+		if self._open:
+			self._send(data, target)
+		else:
+			self._queue.append((data, target))
 
 	def disconnect(self):
-		self.__enabled = False
-		self._authorized = False if self._server_secret else True
-		self._remotekey = None
-		self._send_data(
-			self._socket,
-			self._prepare_data(
-				"disconnect",
-				self._name,
-				socket_action="disconnect",
-				key=self._remotekey,
-				secret=self._secret
-			)
-		)
+		if self.enabled:
+			self._socket.shutdown(SHUT_RDWR)
+			self._socket.close()
+			self._open = False
 
-	def send(self, data, target=None, target_id=None):
-		target = target or self._default_target
-		if self._name:
-			data = Socket._prepare_data(
-				data, self._name, target, target_id, self._remotekey,
-				alias=self._alias, secret=self._secret
-			)
-			Socket._send_data(
-				self._socket,
-				data
-			)
-		else:
-			self.__queue.append((data, target, target_id))
-
-	def __on_message(self):
+	def _listen(self):
 		data = None
 		bytes = b""
-		while self.__enabled:
+		while self.enabled:
 			try:
-				bytes += self._socket.recv(1024)
+				bytes += self._socket.recv(self._buffer_size)
 			except Exception:
-				logger.warning("Connection reset by peer - client")
-				break
+				continue
 			if not bytes:
 				break
-			data, bytes = Socket._process_stream(bytes)
-			secret = self._server_secret and [self._server_secret]
-			for item in data:
-				json = Socket._load_data(item, self._key)
-				self._process_data(json, None, secret)
-				data = None
-		self._socket.close()
-
-	def _socket_trigger(self, data, connection):
-		actions = {
-			"prepare": self._prepare,
-			"server-auth": self._auth,
-		}
-		action = actions.get(data["socket-action"])
-		if action:
-			action(data)
-
-	def _prepare(self, data):
-		self._name = data["name"]
-		if data.get("key"):
-			self._remotekey = PublicKey.load_pkcs1(data["key"])
-			self.authorize()
-		else:
-			self.__send_queue()
-		if self._alias:
-			alias = {"set-alias": self._alias}
-			self._send_data(
-				self._socket, self._prepare_data(
-					alias, self._name, socket_action="set-alias",
-					key=self._remotekey, secret=self._secret
-				)
-			)
-
-	def authorize(self):
-		data = {
-			"key": self._publickey.decode(),
-		}
-		self._send_data(self._socket, self._prepare_data(
-			data, self._name, socket_action="auth", secret=self._secret
-		))
-		if not self._server_secret:
-			self.__send_queue()
-
-	def _auth(self, data):
-		if data["server-secret"] == self._server_secret:
-			self._authorized = True
-			self.__send_queue()
-
-	def __send_queue(self):
-		for item in self.__queue:
-			self.send(item[0], item[1], item[2])
-		self.__queue = []
+			data, overload = self._check(bytes)
+			try:
+				parsed = self._load(data, self._remote_secret)
+			except Exception as e:
+				self._log("ParseError: invalid network data\n%s" % str(e), level=30)
+				parsed = {}
+			if "payload" in parsed:
+				self._trigger(parsed["payload"], parsed.get("sender"))
+			elif "client_id" in parsed:
+				self._id = parsed["client_id"]
+				key = parsed.get("key")
+				if key:
+					self._remote_key = PublicKey.load_pkcs1(key)
+				self._socket.sendall(self._dump({
+					"secret": self.secret.decode(),
+					"key": self._public_key,
+					"sender": self._id
+				}))
+				if not self._remote_secret:
+					self._ready()
+			elif not self._open and "secret" in parsed:
+				if parsed["secret"].encode() == self._remote_secret:
+					self._ready()
+			bytes = overload
+		self.disconnect()
+
+	def _send(self, data: dict, target: str):
+		self._socket.sendall(self._dump({
+			"payload": data,
+			"target": target,
+			"sender": self._id
+		}))
+
+	def _ready(self):
+		while len(self._queue):
+			self._send(*self._queue.pop(0))
+		self._open = True
+
+	@property
+	def id(self):
+		return self._id
+
+	@property
+	def enabled(self):
+		return not self._socket._closed
```

