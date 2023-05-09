# Comparing `tmp/run_rx-0.0.2.tar.gz` & `tmp/run_rx-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "run_rx-0.0.2.tar", max compression
+gzip compressed data, was "run_rx-0.0.3.tar", max compression
```

## Comparing `run_rx-0.0.2.tar` & `run_rx-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,25 @@
--rw-r--r--   0        0        0     1069 2023-05-04 19:54:40.231125 run_rx-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      897 2023-05-06 18:24:26.470100 run_rx-0.0.2/README.md
--rw-r--r--   0        0        0      721 2023-05-05 22:21:30.732209 run_rx-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      300 2023-05-03 20:39:38.474682 run_rx-0.0.2/rx/__main__.py
--rw-r--r--   0        0        0     2406 2023-05-06 18:41:24.564694 run_rx-0.0.2/rx/client/commands/exec.py
--rw-r--r--   0        0        0      989 2023-04-22 21:27:00.833838 run_rx-0.0.2/rx/client/commands/init.py
--rw-r--r--   0        0        0     1970 2023-04-10 18:30:14.435321 run_rx-0.0.2/rx/client/configuration/config_base.py
--rw-r--r--   0        0        0     6945 2023-05-06 18:38:30.014044 run_rx-0.0.2/rx/client/configuration/local.py
--rw-r--r--   0        0        0      481 2023-03-29 19:30:38.625814 run_rx-0.0.2/rx/client/configuration/remote.py
--rw-r--r--   0        0        0     2811 2023-05-05 22:11:45.982253 run_rx-0.0.2/rx/client/executor.py
--rw-r--r--   0        0        0      256 2023-04-10 18:50:33.017005 run_rx-0.0.2/rx/client/grpc_helper.py
--rw-r--r--   0        0        0     5202 2023-05-05 22:12:00.605647 run_rx-0.0.2/rx/client/init_client.py
--rw-r--r--   0        0        0     9492 2023-05-05 21:12:58.788558 run_rx-0.0.2/rx/client/login.py
--rw-r--r--   0        0        0     2029 2023-03-25 18:11:12.345418 run_rx-0.0.2/rx/client/menu.py
--rw-r--r--   0        0        0     1029 2023-05-03 20:09:57.609097 run_rx-0.0.2/rx/client/output_handler.py
--rw-r--r--   0        0        0     2303 2023-05-05 22:11:20.469353 run_rx-0.0.2/rx/client/rsync.py
--rw-r--r--   0        0        0     1579 2023-03-29 19:53:44.892412 run_rx-0.0.2/rx/client/user.py
--rw-r--r--   0        0        0     5624 2023-04-23 18:22:17.589816 run_rx-0.0.2/rx/proto/rx_pb2.py
--rw-r--r--   0        0        0     7378 2023-04-23 18:22:17.589919 run_rx-0.0.2/rx/proto/rx_pb2.pyi
--rw-r--r--   0        0        0    11070 2023-04-23 18:22:17.590590 run_rx-0.0.2/rx/proto/rx_pb2_grpc.py
--rw-r--r--   0        0        0     1815 1970-01-01 00:00:00.000000 run_rx-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 19:54:40.231125 run_rx-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0      901 2023-05-09 22:23:59.643229 run_rx-0.0.3/README.md
+-rw-r--r--   0        0        0      298 2023-04-28 22:39:27.166689 run_rx-0.0.3/install/.rxignore
+-rw-r--r--   0        0        0      588 2023-03-14 00:53:59.323287 run_rx-0.0.3/install/README.md
+-rw-r--r--   0        0        0       98 2023-04-01 19:04:24.721429 run_rx-0.0.3/install/python-cpu
+-rw-r--r--   0        0        0       98 2023-04-01 19:04:30.545846 run_rx-0.0.3/install/python-gpu
+-rw-r--r--   0        0        0      735 2023-05-09 22:32:52.383525 run_rx-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-05-03 20:39:38.474682 run_rx-0.0.3/rx/__main__.py
+-rw-r--r--   0        0        0     2406 2023-05-09 22:23:45.102644 run_rx-0.0.3/rx/client/commands/exec.py
+-rw-r--r--   0        0        0      989 2023-05-09 22:23:45.103045 run_rx-0.0.3/rx/client/commands/init.py
+-rw-r--r--   0        0        0     1970 2023-04-10 18:30:14.435321 run_rx-0.0.3/rx/client/configuration/config_base.py
+-rw-r--r--   0        0        0     6945 2023-05-09 22:30:04.869127 run_rx-0.0.3/rx/client/configuration/local.py
+-rw-r--r--   0        0        0      481 2023-03-29 19:30:38.625814 run_rx-0.0.3/rx/client/configuration/remote.py
+-rw-r--r--   0        0        0     2811 2023-05-09 22:23:45.103366 run_rx-0.0.3/rx/client/executor.py
+-rw-r--r--   0        0        0      256 2023-04-10 18:50:33.017005 run_rx-0.0.3/rx/client/grpc_helper.py
+-rw-r--r--   0        0        0     5202 2023-05-09 22:23:45.104121 run_rx-0.0.3/rx/client/init_client.py
+-rw-r--r--   0        0        0     9492 2023-05-05 21:12:58.788558 run_rx-0.0.3/rx/client/login.py
+-rw-r--r--   0        0        0     2029 2023-03-25 18:11:12.345418 run_rx-0.0.3/rx/client/menu.py
+-rw-r--r--   0        0        0     1029 2023-05-03 20:09:57.609097 run_rx-0.0.3/rx/client/output_handler.py
+-rw-r--r--   0        0        0     2303 2023-05-05 22:11:20.469353 run_rx-0.0.3/rx/client/rsync.py
+-rw-r--r--   0        0        0     1579 2023-03-29 19:53:44.892412 run_rx-0.0.3/rx/client/user.py
+-rw-r--r--   0        0        0     5866 2023-05-09 18:41:10.568989 run_rx-0.0.3/rx/proto/rx_pb2.py
+-rw-r--r--   0        0        0     7595 2023-05-09 18:41:10.570471 run_rx-0.0.3/rx/proto/rx_pb2.pyi
+-rw-r--r--   0        0        0    12663 2023-05-09 18:41:10.570796 run_rx-0.0.3/rx/proto/rx_pb2_grpc.py
+-rw-r--r--   0        0        0     1819 1970-01-01 00:00:00.000000 run_rx-0.0.3/PKG-INFO
```

### Comparing `run_rx-0.0.2/LICENSE.txt` & `run_rx-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/README.md` & `run_rx-0.0.3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Remote execution made easy.
 
 ## Installation
 
 Install the latest release from pip:
 
-    pip install rx
+    pip install run-rx
 
 rx uses rsync for downloads, so make sure rsync is installed on your
 system:
 
     which rsync
 
 If it isn't, install it with your favorite package manager:
```

### Comparing `run_rx-0.0.2/pyproject.toml` & `run_rx-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "run-rx"
-version = "0.0.2"
+version = "0.0.3"
 description = "A tool to simplify remote execution"
 authors = ["Kris Chodorow <k.chodorow@gmail.com>"]
 license = "LICENSE.txt"
 readme = "README.md"
 homepage = "https://www.run-rx.com"
 repository = "https://github.com/run-rx/rx"
 packages = [
     { include = "rx" },
 ]
 include = [
   "rx/proto/*.py",
   "rx/proto/*.pyi",
+  "install/*"
 ]
 exclude = [
   "**/*_test.py",
   "rx/proto/*.proto",
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `run_rx-0.0.2/rx/client/commands/exec.py` & `run_rx-0.0.3/rx/client/commands/exec.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/client/commands/init.py` & `run_rx-0.0.3/rx/client/commands/init.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/client/configuration/config_base.py` & `run_rx-0.0.3/rx/client/configuration/config_base.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/client/configuration/local.py` & `run_rx-0.0.3/rx/client/configuration/local.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from absl import flags
 from absl import logging
 import sty
 
 from rx.client.configuration import config_base
 from rx.proto import rx_pb2
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 IGNORE = pathlib.Path('.rxignore')
 
 _REMOTE = flags.DEFINE_string(
   'remote', 'default',
   'The remote configuration file to use (see .rx/README.md).')
 _RSYNC_PATH = flags.DEFINE_string('rsync_path', None, 'Path to rsync binary')
```

### Comparing `run_rx-0.0.2/rx/client/executor.py` & `run_rx-0.0.3/rx/client/executor.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/client/init_client.py` & `run_rx-0.0.3/rx/client/init_client.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/client/login.py` & `run_rx-0.0.3/rx/client/login.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/client/menu.py` & `run_rx-0.0.3/rx/client/menu.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/client/output_handler.py` & `run_rx-0.0.3/rx/client/output_handler.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/client/rsync.py` & `run_rx-0.0.3/rx/client/rsync.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/client/user.py` & `run_rx-0.0.3/rx/client/user.py`

 * *Files identical despite different names*

### Comparing `run_rx-0.0.2/rx/proto/rx_pb2.py` & `run_rx-0.0.3/rx/proto/rx_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11rx/proto/rx.proto\x12\x02rx\x1a\x1bgoogle/protobuf/empty.proto\"\x95\x01\n\x06Remote\x12\x1f\n\x05image\x18\x01 \x01(\x0b\x32\x10.rx.Remote.Image\x12%\n\x08hardware\x18\x02 \x01(\x0b\x32\x13.rx.Remote.Hardware\x1a$\n\x05Image\x12\x0e\n\x06\x64ocker\x18\x01 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x1a\x1d\n\x08Hardware\x12\x11\n\tprocessor\x18\x01 \x01(\t\"\x08\n\x06Python\"D\n\x0b\x45nvironment\x12\x19\n\x05\x61lloc\x18\x01 \x01(\x0b\x32\n.rx.Remote\x12\x1a\n\x06python\x18\x02 \x01(\x0b\x32\n.rx.Python\"?\n\x05\x44\x65lta\x12\x10\n\x08\x61\x64\x64_path\x18\x01 \x03(\t\x12\x0f\n\x07\x61\x64\x64_dir\x18\x02 \x03(\t\x12\x13\n\x0bremove_path\x18\x03 \x03(\t\"7\n\x06Result\x12\x1c\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0e.rx.StatusCode\x12\x0f\n\x07message\x18\x02 \x01(\t\"H\n\x0bRsyncSource\x12\x12\n\nmachine_id\x18\x01 \x01(\x03\x12\x11\n\tdirectory\x18\x02 \x01(\t\x12\x12\n\npublic_key\x18\x03 \x01(\x0c\")\n\x10RsyncDestination\x12\x15\n\rdaemon_module\x18\x01 \x01(\t\"X\n\x0b\x45xecRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x0c\n\x04\x61rgv\x18\x02 \x03(\t\x12%\n\x0crsync_source\x18\x03 \x01(\x0b\x32\x0f.rx.RsyncSource\"v\n\x0c\x45xecResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x0e\n\x06stdout\x18\x03 \x01(\x0c\x12\x0e\n\x06stderr\x18\x04 \x01(\x0c\x12\x14\n\x0coutput_files\x18\x05 \x03(\t\"?\n\x0fGetUserResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x10\n\x08username\x18\x02 \x01(\t\"o\n\x0bInitRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12%\n\x0crsync_source\x18\x02 \x01(\x0b\x32\x0f.rx.RsyncSource\x12#\n\ntarget_env\x18\x03 \x01(\x0b\x32\x0f.rx.Environment\"\x7f\n\x0cInitResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12(\n\nrsync_dest\x18\x02 \x01(\x0b\x32\x14.rx.RsyncDestination\x12\x13\n\x0bworker_addr\x18\x03 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x04 \x01(\t\"*\n\x12InstallDepsRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"A\n\x13InstallDepsResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x0e\n\x06stdout\x18\x02 \x01(\x0c\"9\n\x0bKillRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\"&\n\x12SetUsernameRequest\x12\x10\n\x08username\x18\x01 \x01(\t\"1\n\x13SetUsernameResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result*O\n\nStatusCode\x12\x06\n\x02OK\x10\x00\x12\x0b\n\x07UNKNOWN\x10\x01\x12\x0b\n\x07INVALID\x10\x02\x12\r\n\tNOT_FOUND\x10\x03\x12\x10\n\x0cUNAUTHORIZED\x10\x04\x32\xb8\x01\n\x10\x45xecutionService\x12\x42\n\x0bInstallDeps\x12\x16.rx.InstallDepsRequest\x1a\x17.rx.InstallDepsResponse\"\x00\x30\x01\x12-\n\x04\x45xec\x12\x0f.rx.ExecRequest\x1a\x10.rx.ExecResponse\"\x00\x30\x01\x12\x31\n\x04Kill\x12\x0f.rx.KillRequest\x1a\x16.google.protobuf.Empty\"\x00\x32\xb7\x01\n\x0cSetupService\x12\x38\n\x07GetUser\x12\x16.google.protobuf.Empty\x1a\x13.rx.GetUserResponse\"\x00\x12+\n\x04Init\x12\x0f.rx.InitRequest\x1a\x10.rx.InitResponse\"\x00\x12@\n\x0bSetUsername\x12\x16.rx.SetUsernameRequest\x1a\x17.rx.SetUsernameResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11rx/proto/rx.proto\x12\x02rx\x1a\x1bgoogle/protobuf/empty.proto\"\x95\x01\n\x06Remote\x12\x1f\n\x05image\x18\x01 \x01(\x0b\x32\x10.rx.Remote.Image\x12%\n\x08hardware\x18\x02 \x01(\x0b\x32\x13.rx.Remote.Hardware\x1a$\n\x05Image\x12\x0e\n\x06\x64ocker\x18\x01 \x01(\t\x12\x0b\n\x03tag\x18\x02 \x01(\t\x1a\x1d\n\x08Hardware\x12\x11\n\tprocessor\x18\x01 \x01(\t\"\x08\n\x06Python\"D\n\x0b\x45nvironment\x12\x19\n\x05\x61lloc\x18\x01 \x01(\x0b\x32\n.rx.Remote\x12\x1a\n\x06python\x18\x02 \x01(\x0b\x32\n.rx.Python\"?\n\x05\x44\x65lta\x12\x10\n\x08\x61\x64\x64_path\x18\x01 \x03(\t\x12\x0f\n\x07\x61\x64\x64_dir\x18\x02 \x03(\t\x12\x13\n\x0bremove_path\x18\x03 \x03(\t\"7\n\x06Result\x12\x1c\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x0e.rx.StatusCode\x12\x0f\n\x07message\x18\x02 \x01(\t\"H\n\x0bRsyncSource\x12\x12\n\nmachine_id\x18\x01 \x01(\x03\x12\x11\n\tdirectory\x18\x02 \x01(\t\x12\x12\n\npublic_key\x18\x03 \x01(\x0c\")\n\x10RsyncDestination\x12\x15\n\rdaemon_module\x18\x01 \x01(\t\")\n\x11\x41llocNewWorkerReq\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"X\n\x0b\x45xecRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x0c\n\x04\x61rgv\x18\x02 \x03(\t\x12%\n\x0crsync_source\x18\x03 \x01(\x0b\x32\x0f.rx.RsyncSource\"v\n\x0c\x45xecResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\x12\x0e\n\x06stdout\x18\x03 \x01(\x0c\x12\x0e\n\x06stderr\x18\x04 \x01(\x0c\x12\x14\n\x0coutput_files\x18\x05 \x03(\t\"?\n\x0fGetUserResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x10\n\x08username\x18\x02 \x01(\t\"o\n\x0bInitRequest\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12%\n\x0crsync_source\x18\x02 \x01(\x0b\x32\x0f.rx.RsyncSource\x12#\n\ntarget_env\x18\x03 \x01(\x0b\x32\x0f.rx.Environment\"\x7f\n\x0cInitResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12(\n\nrsync_dest\x18\x02 \x01(\x0b\x32\x14.rx.RsyncDestination\x12\x13\n\x0bworker_addr\x18\x03 \x01(\t\x12\x14\n\x0cworkspace_id\x18\x04 \x01(\t\"*\n\x12InstallDepsRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\"A\n\x13InstallDepsResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result\x12\x0e\n\x06stdout\x18\x02 \x01(\x0c\"9\n\x0bKillRequest\x12\x14\n\x0cworkspace_id\x18\x01 \x01(\t\x12\x14\n\x0c\x65xecution_id\x18\x02 \x01(\t\"&\n\x12SetUsernameRequest\x12\x10\n\x08username\x18\x01 \x01(\t\"1\n\x13SetUsernameResponse\x12\x1a\n\x06result\x18\x01 \x01(\x0b\x32\n.rx.Result*O\n\nStatusCode\x12\x06\n\x02OK\x10\x00\x12\x0b\n\x07UNKNOWN\x10\x01\x12\x0b\n\x07INVALID\x10\x02\x12\r\n\tNOT_FOUND\x10\x03\x12\x10\n\x0cUNAUTHORIZED\x10\x04\x32\xb8\x01\n\x10\x45xecutionService\x12\x42\n\x0bInstallDeps\x12\x16.rx.InstallDepsRequest\x1a\x17.rx.InstallDepsResponse\"\x00\x30\x01\x12-\n\x04\x45xec\x12\x0f.rx.ExecRequest\x1a\x10.rx.ExecResponse\"\x00\x30\x01\x12\x31\n\x04Kill\x12\x0f.rx.KillRequest\x1a\x16.google.protobuf.Empty\"\x00\x32\xf4\x01\n\x0cSetupService\x12;\n\x0e\x41llocNewWorker\x12\x15.rx.AllocNewWorkerReq\x1a\x10.rx.InitResponse\"\x00\x12\x38\n\x07GetUser\x12\x16.google.protobuf.Empty\x1a\x13.rx.GetUserResponse\"\x00\x12+\n\x04Init\x12\x0f.rx.InitRequest\x1a\x10.rx.InitResponse\"\x00\x12@\n\x0bSetUsername\x12\x16.rx.SetUsernameRequest\x1a\x17.rx.SetUsernameResponse\"\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'rx.proto.rx_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _STATUSCODE._serialized_start=1303
-  _STATUSCODE._serialized_end=1382
+  _STATUSCODE._serialized_start=1346
+  _STATUSCODE._serialized_end=1425
   _REMOTE._serialized_start=55
   _REMOTE._serialized_end=204
   _REMOTE_IMAGE._serialized_start=137
   _REMOTE_IMAGE._serialized_end=173
   _REMOTE_HARDWARE._serialized_start=175
   _REMOTE_HARDWARE._serialized_end=204
   _PYTHON._serialized_start=206
@@ -37,32 +37,34 @@
   _DELTA._serialized_end=349
   _RESULT._serialized_start=351
   _RESULT._serialized_end=406
   _RSYNCSOURCE._serialized_start=408
   _RSYNCSOURCE._serialized_end=480
   _RSYNCDESTINATION._serialized_start=482
   _RSYNCDESTINATION._serialized_end=523
-  _EXECREQUEST._serialized_start=525
-  _EXECREQUEST._serialized_end=613
-  _EXECRESPONSE._serialized_start=615
-  _EXECRESPONSE._serialized_end=733
-  _GETUSERRESPONSE._serialized_start=735
-  _GETUSERRESPONSE._serialized_end=798
-  _INITREQUEST._serialized_start=800
-  _INITREQUEST._serialized_end=911
-  _INITRESPONSE._serialized_start=913
-  _INITRESPONSE._serialized_end=1040
-  _INSTALLDEPSREQUEST._serialized_start=1042
-  _INSTALLDEPSREQUEST._serialized_end=1084
-  _INSTALLDEPSRESPONSE._serialized_start=1086
-  _INSTALLDEPSRESPONSE._serialized_end=1151
-  _KILLREQUEST._serialized_start=1153
-  _KILLREQUEST._serialized_end=1210
-  _SETUSERNAMEREQUEST._serialized_start=1212
-  _SETUSERNAMEREQUEST._serialized_end=1250
-  _SETUSERNAMERESPONSE._serialized_start=1252
-  _SETUSERNAMERESPONSE._serialized_end=1301
-  _EXECUTIONSERVICE._serialized_start=1385
-  _EXECUTIONSERVICE._serialized_end=1569
-  _SETUPSERVICE._serialized_start=1572
-  _SETUPSERVICE._serialized_end=1755
+  _ALLOCNEWWORKERREQ._serialized_start=525
+  _ALLOCNEWWORKERREQ._serialized_end=566
+  _EXECREQUEST._serialized_start=568
+  _EXECREQUEST._serialized_end=656
+  _EXECRESPONSE._serialized_start=658
+  _EXECRESPONSE._serialized_end=776
+  _GETUSERRESPONSE._serialized_start=778
+  _GETUSERRESPONSE._serialized_end=841
+  _INITREQUEST._serialized_start=843
+  _INITREQUEST._serialized_end=954
+  _INITRESPONSE._serialized_start=956
+  _INITRESPONSE._serialized_end=1083
+  _INSTALLDEPSREQUEST._serialized_start=1085
+  _INSTALLDEPSREQUEST._serialized_end=1127
+  _INSTALLDEPSRESPONSE._serialized_start=1129
+  _INSTALLDEPSRESPONSE._serialized_end=1194
+  _KILLREQUEST._serialized_start=1196
+  _KILLREQUEST._serialized_end=1253
+  _SETUSERNAMEREQUEST._serialized_start=1255
+  _SETUSERNAMEREQUEST._serialized_end=1293
+  _SETUSERNAMERESPONSE._serialized_start=1295
+  _SETUSERNAMERESPONSE._serialized_end=1344
+  _EXECUTIONSERVICE._serialized_start=1428
+  _EXECUTIONSERVICE._serialized_end=1612
+  _SETUPSERVICE._serialized_start=1615
+  _SETUPSERVICE._serialized_end=1859
 # @@protoc_insertion_point(module_scope)
```

### Comparing `run_rx-0.0.2/rx/proto/rx_pb2.pyi` & `run_rx-0.0.3/rx/proto/rx_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,20 @@
 DESCRIPTOR: _descriptor.FileDescriptor
 INVALID: StatusCode
 NOT_FOUND: StatusCode
 OK: StatusCode
 UNAUTHORIZED: StatusCode
 UNKNOWN: StatusCode
 
+class AllocNewWorkerReq(_message.Message):
+    __slots__ = ["workspace_id"]
+    WORKSPACE_ID_FIELD_NUMBER: _ClassVar[int]
+    workspace_id: str
+    def __init__(self, workspace_id: _Optional[str] = ...) -> None: ...
+
 class Delta(_message.Message):
     __slots__ = ["add_dir", "add_path", "remove_path"]
     ADD_DIR_FIELD_NUMBER: _ClassVar[int]
     ADD_PATH_FIELD_NUMBER: _ClassVar[int]
     REMOVE_PATH_FIELD_NUMBER: _ClassVar[int]
     add_dir: _containers.RepeatedScalarFieldContainer[str]
     add_path: _containers.RepeatedScalarFieldContainer[str]
```

### Comparing `run_rx-0.0.2/rx/proto/rx_pb2_grpc.py` & `run_rx-0.0.3/rx/proto/rx_pb2_grpc.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,14 +138,19 @@
 
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
+        self.AllocNewWorker = channel.unary_unary(
+                '/rx.SetupService/AllocNewWorker',
+                request_serializer=rx_dot_proto_dot_rx__pb2.AllocNewWorkerReq.SerializeToString,
+                response_deserializer=rx_dot_proto_dot_rx__pb2.InitResponse.FromString,
+                )
         self.GetUser = channel.unary_unary(
                 '/rx.SetupService/GetUser',
                 request_serializer=google_dot_protobuf_dot_empty__pb2.Empty.SerializeToString,
                 response_deserializer=rx_dot_proto_dot_rx__pb2.GetUserResponse.FromString,
                 )
         self.Init = channel.unary_unary(
                 '/rx.SetupService/Init',
@@ -158,14 +163,21 @@
                 response_deserializer=rx_dot_proto_dot_rx__pb2.SetUsernameResponse.FromString,
                 )
 
 
 class SetupServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
+    def AllocNewWorker(self, request, context):
+        """Creates a new worker for an existing workspace.
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def GetUser(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def Init(self, request, context):
@@ -179,14 +191,19 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_SetupServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
+            'AllocNewWorker': grpc.unary_unary_rpc_method_handler(
+                    servicer.AllocNewWorker,
+                    request_deserializer=rx_dot_proto_dot_rx__pb2.AllocNewWorkerReq.FromString,
+                    response_serializer=rx_dot_proto_dot_rx__pb2.InitResponse.SerializeToString,
+            ),
             'GetUser': grpc.unary_unary_rpc_method_handler(
                     servicer.GetUser,
                     request_deserializer=google_dot_protobuf_dot_empty__pb2.Empty.FromString,
                     response_serializer=rx_dot_proto_dot_rx__pb2.GetUserResponse.SerializeToString,
             ),
             'Init': grpc.unary_unary_rpc_method_handler(
                     servicer.Init,
@@ -205,14 +222,31 @@
 
 
  # This class is part of an EXPERIMENTAL API.
 class SetupService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
+    def AllocNewWorker(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/rx.SetupService/AllocNewWorker',
+            rx_dot_proto_dot_rx__pb2.AllocNewWorkerReq.SerializeToString,
+            rx_dot_proto_dot_rx__pb2.InitResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def GetUser(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `run_rx-0.0.2/PKG-INFO` & `run_rx-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: run-rx
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool to simplify remote execution
 Home-page: https://www.run-rx.com
 License: LICENSE.txt
 Author: Kris Chodorow
 Author-email: k.chodorow@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
@@ -27,15 +27,15 @@
 
 Remote execution made easy.
 
 ## Installation
 
 Install the latest release from pip:
 
-    pip install rx
+    pip install run-rx
 
 rx uses rsync for downloads, so make sure rsync is installed on your
 system:
 
     which rsync
 
 If it isn't, install it with your favorite package manager:
```

