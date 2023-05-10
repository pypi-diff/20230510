# Comparing `tmp/psytricks-1.1.0.tar.gz` & `tmp/psytricks-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psytricks-1.1.0.tar", max compression
+gzip compressed data, was "psytricks-2.0.0.tar", max compression
```

## Comparing `psytricks-1.1.0.tar` & `psytricks-2.0.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-1.1.0/LICENSE
--rw-r--r--   0        0        0     3557 2023-04-25 12:23:05.630073 psytricks-1.1.0/README.md
--rw-r--r--   0        0        0      973 2023-04-27 10:15:37.642659 psytricks-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       93 2023-04-27 10:15:37.642659 psytricks-1.1.0/src/psytricks/__init__.py
--rw-r--r--   0        0        0     5145 2023-04-25 11:22:59.630911 psytricks-1.1.0/src/psytricks/cli.py
--rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-1.1.0/src/psytricks/decoder.py
--rw-r--r--   0        0        0     2265 2023-04-27 09:43:59.712708 psytricks-1.1.0/src/psytricks/mappings.py
--rw-r--r--   0        0        0     3014 2023-04-13 12:38:57.964112 psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json
--rw-r--r--   0        0        0    18009 2023-04-25 07:07:36.345357 psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json
--rw-r--r--   0        0        0     4623 2023-04-25 07:59:35.398779 psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetSessions.json
--rw-r--r--   0        0        0    11759 2023-04-25 11:05:43.569742 psytricks-1.1.0/src/psytricks/ps1scripts/psytricks-wrapper.ps1
--rw-r--r--   0        0        0    11067 2023-04-25 11:09:47.919739 psytricks-1.1.0/src/psytricks/wrapper.py
--rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 psytricks-1.1.0/setup.py
--rw-r--r--   0        0        0     4325 1970-01-01 00:00:00.000000 psytricks-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35059 2022-12-20 15:40:57.930292 psytricks-2.0.0/LICENSE
+-rw-r--r--   0        0        0     6284 2023-05-10 19:08:40.522092 psytricks-2.0.0/README.md
+-rw-r--r--   0        0        0     1045 2023-05-10 19:13:07.196941 psytricks-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-05-10 19:13:07.200941 psytricks-2.0.0/src/psytricks/__init__.py
+-rw-r--r--   0        0        0     6146 2023-05-10 19:13:07.200941 psytricks-2.0.0/src/psytricks/__ps1__/psytricks-lib.ps1
+-rw-r--r--   0        0        0     6392 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/psytricks-wrapper.ps1
+-rw-r--r--   0        0        0     1961 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/restricks-server.example.xml
+-rw-r--r--   0        0        0    14826 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/restricks-server.ps1
+-rw-r--r--   0        0        0     3014 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json
+-rw-r--r--   0        0        0    18009 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json
+-rw-r--r--   0        0        0     4623 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetSessions.json
+-rw-r--r--   0        0        0     6043 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/cli.py
+-rw-r--r--   0        0        0     1880 2023-04-27 09:47:02.646410 psytricks-2.0.0/src/psytricks/decoder.py
+-rw-r--r--   0        0        0      671 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/literals.py
+-rw-r--r--   0        0        0     3516 2023-04-27 10:47:48.965859 psytricks-2.0.0/src/psytricks/mappings.py
+-rw-r--r--   0        0        0    21031 2023-05-10 19:08:40.530093 psytricks-2.0.0/src/psytricks/wrapper.py
+-rw-r--r--   0        0        0     7094 1970-01-01 00:00:00.000000 psytricks-2.0.0/PKG-INFO
```

### Comparing `psytricks-1.1.0/LICENSE` & `psytricks-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psytricks-1.1.0/pyproject.toml` & `psytricks-2.0.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 [tool.poetry]
 authors = ["Niko Ehrenfeuchter <nikolaus.ehrenfeuchter@unibas.ch>"]
 description = "PowerShell Python Citrix Tricks."
 license = "GPL-3.0-or-later"
 name = "psytricks"
 readme = "README.md"
-version = "1.1.0"
+version = "2.0.0"
 
 [tool.poetry.urls]
 "Changelog" = "https://github.com/imcf/psytricks/blob/main/CHANGELOG.md"
 "Organisation Homepage" = "https://imcf.one/"
 "Twitter" = "https://twitter.com/imcf_basel"
 
 [tool.poetry.dependencies]
 click = "^8.1.3"
 loguru = "^0.6.0"
 python = "^3.10"
+requests = "^2.30.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
+ipython = "^8.13.2"
 pylint = "^2.16.2"
 
 [tool.poetry.scripts]
 psytricks = "psytricks.cli:run_cli"
 
 [tool.poetry-dynamic-versioning]
 enable = false
-# pattern = "^psytricks-((?P<epoch>\\d+)!)?(?P<base>\\d+(\\.\\d+)*)"
 style = "semver"
 vcs = "git"
 
 [tool.poetry-dynamic-versioning.substitution]
 folders = [
   {path = "src"},
+  {path = "src/psytricks/__ps1__", files = ["*.ps1"], patterns = ['(^\$Version = ["])[^"]*(["])']},
 ]
 
 [build-system]
 build-backend = "poetry_dynamic_versioning.backend"
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
```

### Comparing `psytricks-1.1.0/src/psytricks/cli.py` & `psytricks-2.0.0/src/psytricks/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -88,16 +88,34 @@
         ]
     ),
     required=False,
     help="The power action to perform on a machine. [required for: 'poweraction']",
 )
 @click.option(
     "--message",
-    type=click.Path(exists=True),
-    help="A JSON file containing the message details (style, title, body).",
+    type=str,
+    help="The body of a pop-up message to be sent. [required for: 'sendmessage']",
+)
+@click.option(
+    "--title",
+    type=str,
+    help="The title of a pop-up message to be sent. [required for: 'sendmessage']",
+)
+@click.option(
+    "--style",
+    type=click.Choice(
+        [
+            "information",
+            "exclamation",
+            "critical",
+            "question",
+        ]
+    ),
+    default="information",
+    help="The icon-style of a pop-up message to be sent. [required for: 'sendmessage']",
 )
 @click.option(
     "--users",
     help=(
         "One or more usernames, enclosed in quotes, separated by comma but without "
         "space, e.g. 'alice,bob'. [required for: 'setaccess']"
     ),
@@ -112,64 +130,87 @@
 )
 @click.option(
     "--outfile",
     type=click.Path(dir_okay=False, writable=True),
     help="The path to a file to write the output into (default=stdout).",
 )
 def run_cli(
-    cdc, verbose, command, machine, group, action, message, users, disable, outfile
+    cdc,
+    verbose,
+    command,
+    machine,
+    group,
+    action,
+    message,
+    title,
+    style,
+    users,
+    disable,
+    outfile,
 ):
     """Create a wrapper object and call the method requested on the command line.
 
     Parameters
     ----------
     cdc : str
         The address of the Citrix Delivery Controller (CDC) to connect to.
     verbose : int
         The logging verbosity.
     command : str
         The command indicating which wrapper method to call.
     """
+    # FIXME: adapt for "kwargs" being dropped in PSyTricksWrapper
     configure_logging(verbose)
     wrapper = PSyTricksWrapper(deliverycontroller=cdc)
-    call_method = {
-        "disconnect": wrapper.disconnect_session,
-        "getaccess": wrapper.get_access_users,
-        "machines": wrapper.get_machine_status,
-        "maintenance": wrapper.set_maintenance,
-        "poweraction": wrapper.perform_poweraction,
-        "sendmessage": wrapper.send_message,
-        "sessions": wrapper.get_sessions,
-        "setaccess": wrapper.set_access_users,
-    }
-    call_kwargs = {
-        "machine": machine,
-        "group": group,
-        "action": action,
-        "message": message,
-        "users": users,
-        "disable": disable,
-    }
-
-    if command == "disconnect" and machine is None:
-        raise click.UsageError("Command 'disconnect' requires --machine!")
-    if command in ["getaccess", "setaccess"] and group is None:
-        raise click.UsageError("Commands 'getaccess'/'setaccess' require --group!")
-    if command == "setaccess" and users is None:
-        raise click.UsageError("Command 'setaccess' requires --users!")
-    if command == "poweraction" and action is None:
-        raise click.UsageError("Command 'poweraction' requires --action!")
-    if command == "sendmessage" and message is None:
-        raise click.UsageError("Command 'sendmessage' requires --message!")
-    if command in ["maintenance", "poweraction"] and machine is None:
-        raise click.UsageError(
-            "Commands 'maintenance'/'poweraction' require --machine!"
-        )
+    details = ""
+
+    if command == "machines":
+        details = wrapper.get_machine_status()
+
+    if command == "sessions":
+        details = wrapper.get_sessions()
+
+    elif command == "disconnect":
+        if machine is None:
+            raise click.UsageError("Command 'disconnect' requires --machine!")
+        details = wrapper.disconnect_session(machine)
+
+    elif command == "getaccess":
+        if group is None:
+            raise click.UsageError("Command 'getaccess' requires --group!")
+        details = wrapper.get_access_users(group)
+
+    elif command == "setaccess":
+        if users is None:
+            raise click.UsageError("Command 'setaccess' requires --users!")
+        if group is None:
+            raise click.UsageError("Command 'setaccess' requires --group!")
+        details = wrapper.set_access_users(group, users, disable)
+
+    elif command == "poweraction":
+        if machine is None:
+            raise click.UsageError("Command 'poweraction' requires --machine!")
+        if action is None:
+            raise click.UsageError("Command 'poweraction' requires --action!")
+        details = wrapper.perform_poweraction(machine, action)
+
+    elif command == "sendmessage":
+        style = style[0].upper() + style[1:]
+        if machine is None:
+            raise click.UsageError("Command 'sendmessage' requires --machine!")
+        if message is None:
+            raise click.UsageError("Command 'sendmessage' requires --message!")
+        if title is None:
+            raise click.UsageError("Command 'sendmessage' requires --title!")
+        wrapper.send_message(machine, message, title, style)
 
-    details = call_method[command](**call_kwargs)
+    elif command == "maintenance":
+        if machine is None:
+            raise click.UsageError("Command 'maintenance' requires --machine!")
+        details = wrapper.set_maintenance(machine, disable)
 
     if outfile:
         with open(outfile, "a", encoding="utf-8") as fh:
             fh.writelines(pformat(details))
         log.success(f"Done writing output into [{outfile}].")
     else:
         pprint(details)
```

### Comparing `psytricks-1.1.0/src/psytricks/decoder.py` & `psytricks-2.0.0/src/psytricks/decoder.py`

 * *Files identical despite different names*

### Comparing `psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetAccessUsers.json` & `psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetAccessUsers.json`

 * *Files identical despite different names*

### Comparing `psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetMachineStatus.json` & `psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetMachineStatus.json`

 * *Files identical despite different names*

### Comparing `psytricks-1.1.0/src/psytricks/ps1scripts/dummydata/GetSessions.json` & `psytricks-2.0.0/src/psytricks/__ps1__/sampledata/GetSessions.json`

 * *Files identical despite different names*

