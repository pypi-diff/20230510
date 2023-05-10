# Comparing `tmp/ntdsdotsqlite-0.9.4.tar.gz` & `tmp/ntdsdotsqlite-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntdsdotsqlite-0.9.4.tar", max compression
+gzip compressed data, was "ntdsdotsqlite-0.9.5.tar", max compression
```

## Comparing `ntdsdotsqlite-0.9.4.tar` & `ntdsdotsqlite-0.9.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-0.9.4/ntdsdotsqlite/__init__.py
--rw-r--r--   0        0        0      854 2023-05-08 16:23:21.892529 ntdsdotsqlite-0.9.4/ntdsdotsqlite/__main__.py
--rw-r--r--   0        0        0     4795 2023-05-09 17:02:10.560346 ntdsdotsqlite-0.9.4/ntdsdotsqlite/accounts.py
--rw-r--r--   0        0        0     1454 2023-05-08 09:43:59.572323 ntdsdotsqlite-0.9.4/ntdsdotsqlite/containers.py
--rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-0.9.4/ntdsdotsqlite/decrypt.py
--rw-r--r--   0        0        0     3089 2023-05-08 21:09:08.053917 ntdsdotsqlite-0.9.4/ntdsdotsqlite/domain.py
--rw-r--r--   0        0        0      905 2023-05-08 13:52:27.251046 ntdsdotsqlite-0.9.4/ntdsdotsqlite/groups.py
--rw-r--r--   0        0        0      320 2023-05-08 21:09:14.178994 ntdsdotsqlite-0.9.4/ntdsdotsqlite/links.py
--rw-r--r--   0        0        0     2726 2023-05-08 15:41:39.616697 ntdsdotsqlite-0.9.4/ntdsdotsqlite/model.sql
--rw-r--r--   0        0        0     4615 2023-05-09 20:33:04.646232 ntdsdotsqlite-0.9.4/ntdsdotsqlite/ntdsdotsqlite.py
--rw-r--r--   0        0        0     1595 2023-05-08 09:44:10.802061 ntdsdotsqlite-0.9.4/ntdsdotsqlite/orga_units.py
--rw-r--r--   0        0        0    26966 2023-05-09 20:30:13.020077 ntdsdotsqlite-0.9.4/ntdsdotsqlite/secretsdump.py
--rw-r--r--   0        0        0     5851 2023-05-09 20:32:50.342772 ntdsdotsqlite-0.9.4/ntdsdotsqlite/utils.py
--rw-r--r--   0        0        0      695 2023-05-09 20:49:32.596269 ntdsdotsqlite-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-0.9.4/README.md
--rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 ntdsdotsqlite-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-24 19:34:15.811658 ntdsdotsqlite-0.9.5/ntdsdotsqlite/__init__.py
+-rw-r--r--   0        0        0      854 2023-05-08 16:23:21.892529 ntdsdotsqlite-0.9.5/ntdsdotsqlite/__main__.py
+-rw-r--r--   0        0        0     5134 2023-05-10 17:20:33.263014 ntdsdotsqlite-0.9.5/ntdsdotsqlite/accounts.py
+-rw-r--r--   0        0        0     1454 2023-05-08 09:43:59.572323 ntdsdotsqlite-0.9.5/ntdsdotsqlite/containers.py
+-rw-r--r--   0        0        0     4145 2023-05-06 15:44:55.688794 ntdsdotsqlite-0.9.5/ntdsdotsqlite/decrypt.py
+-rw-r--r--   0        0        0     3089 2023-05-08 21:09:08.053917 ntdsdotsqlite-0.9.5/ntdsdotsqlite/domain.py
+-rw-r--r--   0        0        0      905 2023-05-08 13:52:27.251046 ntdsdotsqlite-0.9.5/ntdsdotsqlite/groups.py
+-rw-r--r--   0        0        0      320 2023-05-08 21:09:14.178994 ntdsdotsqlite-0.9.5/ntdsdotsqlite/links.py
+-rw-r--r--   0        0        0     2726 2023-05-08 15:41:39.616697 ntdsdotsqlite-0.9.5/ntdsdotsqlite/model.sql
+-rw-r--r--   0        0        0     4644 2023-05-10 17:08:18.055714 ntdsdotsqlite-0.9.5/ntdsdotsqlite/ntdsdotsqlite.py
+-rw-r--r--   0        0        0     1595 2023-05-08 09:44:10.802061 ntdsdotsqlite-0.9.5/ntdsdotsqlite/orga_units.py
+-rw-r--r--   0        0        0    26966 2023-05-09 20:30:13.020077 ntdsdotsqlite-0.9.5/ntdsdotsqlite/secretsdump.py
+-rw-r--r--   0        0        0     5851 2023-05-09 20:32:50.342772 ntdsdotsqlite-0.9.5/ntdsdotsqlite/utils.py
+-rw-r--r--   0        0        0      695 2023-05-10 17:21:14.997394 ntdsdotsqlite-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     2005 2023-05-08 16:12:51.277756 ntdsdotsqlite-0.9.5/README.md
+-rw-r--r--   0        0        0     2775 1970-01-01 00:00:00.000000 ntdsdotsqlite-0.9.5/PKG-INFO
```

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/__main__.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/__main__.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/accounts.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/accounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,26 @@
         accountExpires = a.get(ese_db.column_names["accountExpires"])
         if accountExpires:
             if accountExpires and accountExpires == 0 or accountExpires == 0x7FFFFFFFFFFFFFFF:
                 accountExpires = 0
             else:
                 accountExpires = hundredns_to_datetime(accountExpires)
         uac = a.get(ese_db.column_names["userAccountControl"])
+        sid = a.get(ese_db.column_names["objectSid"])
+        guid = a.get(ese_db.column_names["objectGUID"])
         account = {
             "id": a.get("DNT_col"), "description": a.get(ese_db.column_names["description"]),
             "UAC": uac,
-            "SID": raw_to_sid(a.get(ese_db.column_names["objectSid"])),
+            "SID": raw_to_sid(sid) if sid else None,
             "samaccountname": a.get(ese_db.column_names["sAMAccountName"]),
             # unix epoch or NULL if password never set
             "pwdLastSet": pwdlastset,
             "nthash": a.get(ese_db.column_names["unicodePwd"]),
             "commonname": a.get(ese_db.column_names["cn"]),
-            "GUID": raw_to_guid(a.get(ese_db.column_names["objectGUID"])),
+            "GUID": raw_to_guid(guid) if guid else None,
             "adminCount": admincount,
             "displayName": a.get(ese_db.column_names["displayName"]),
             "UPN": a.get(ese_db.column_names["userPrincipalName"]),
             "supplementalCredentials": a.get(ese_db.column_names["supplementalCredentials"]),
             # unix epoch
             "lastLogonTimestamp": lastLogonTimestamp,
             "lmPwdHistory": a.get(ese_db.column_names["lmPwdHistory"]),
@@ -63,33 +65,41 @@
         if (spn := account["SPN"]):
             if type(spn) is str:
                 account["SPN"] = json.dumps([spn])
             elif type(spn) is list:
                 account["SPN"] = json.dumps(spn)
             else:
                 print(f"SPN type unknown : {spn} - {type(spn)}")
+                print(account)
                 exit(1)
-        uac_flags = {
-            k.name: True if uac & k.value else False for k in UAC_FLAGS
-        }
-        account["uac_flags"] = json.dumps(uac_flags)
-        account["isDisabled"] = uac_flags["ACCOUNTDISABLE"]
+        if uac:
+            uac_flags = {
+                k.name: True if uac & k.value else False for k in UAC_FLAGS
+            }
+            account["uac_flags"] = json.dumps(uac_flags)
+            account["isDisabled"] = uac_flags["ACCOUNTDISABLE"]
+        else:
+            account["uac_flags"] = None
+            account["isDisabled"] = None
         # Generate Distinguished Name
         cur = sqlite_db.cursor()
         parent_dnt = a.get("PDNT_col")
         res = cur.execute(f"SELECT dn FROM organizational_units WHERE id={parent_dnt}")
         res = res.fetchone()
         if res is None:
             res = cur.execute(f"SELECT dn FROM containers WHERE id={parent_dnt}")
             res = res.fetchone()
         account["dn"] = "CN=" + escape_dn_chars(account["commonname"]) + "," + res[0]
         primaryGroup = a.get(ese_db.column_names["primaryGroupID"])
-        res = cur.execute(f"SELECT id, SID from groups WHERE SID LIKE '%-{primaryGroup}'")
-        res = res.fetchone()
-        account["primaryGroup"] = res[0]
+        if primaryGroup:
+            res = cur.execute(f"SELECT id, SID from groups WHERE SID LIKE '%-{primaryGroup}'")
+            res = res.fetchone()
+            account["primaryGroup"] = res[0]
+        else:
+            account["primaryGroup"] = None
         # manage groups membership
         links_list = relations[account["id"]]
         account["links"] = json.dumps(links_list)
         account["memberOf"] = []
         for link in links_list:
             res = cur.execute(f"SELECT id FROM groups WHERE id={link}")
             res = res.fetchone()
```

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/containers.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/containers.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/decrypt.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/decrypt.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/domain.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/domain.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/groups.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/groups.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/model.sql` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/model.sql`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/ntdsdotsqlite.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/ntdsdotsqlite.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 import sqlite3
 import json
 
 
 def run(ese_path, outpath, system_path):
     create_database(outpath)
     sqlite_db = sqlite3.connect(outpath)
-    ese_db = EseDB(open(ese_path, "rb"))
+    fd = open(ese_path, "rb")
+    ese_db = EseDB(fd)
     cursor = sqlite_db.cursor()
     # Getting column names
     column_names = get_ESE_column_names(ese_db)
     ese_db.column_names = column_names
     # Compute links
     print("Retrieving and storing links information ...")
     link_relations = compute_links(ese_db)
@@ -111,7 +112,8 @@
     cursor.executemany(stmt, machines_iter)
     sqlite_db.commit()
     if system_path:
         print("Decrypting stuff with SYSTEM hive ...")
         decrypt_sqlite(sqlite_db, ese_path, system_path)
     if sqlite_db:
         sqlite_db.close()
+    fd.close()
```

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/orga_units.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/orga_units.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/secretsdump.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/secretsdump.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/ntdsdotsqlite/utils.py` & `ntdsdotsqlite-0.9.5/ntdsdotsqlite/utils.py`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/pyproject.toml` & `ntdsdotsqlite-0.9.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ntdsdotsqlite"
-version = "0.9.4"
+version = "0.9.5"
 description = "A small utility to get an SQLite  database from an NTDS.DIT file."
 authors = ["Virgile Jarry <virgile@mailbox.org>"]
 readme = "README.md"
 license = "Beerware"
 homepage = "https://github.com/almandin/ntdsdotsqlite"
 repository = "https://github.com/almandin/ntdsdotsqlite"
 documentation = "https://github.com/almandin/ntdsdotsqlite/README.md"
```

### Comparing `ntdsdotsqlite-0.9.4/README.md` & `ntdsdotsqlite-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `ntdsdotsqlite-0.9.4/PKG-INFO` & `ntdsdotsqlite-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ntdsdotsqlite
-Version: 0.9.4
+Version: 0.9.5
 Summary: A small utility to get an SQLite  database from an NTDS.DIT file.
 Home-page: https://github.com/almandin/ntdsdotsqlite
 License: Beerware
 Author: Virgile Jarry
 Author-email: virgile@mailbox.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
```

