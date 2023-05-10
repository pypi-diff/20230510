# Comparing `tmp/autonity-0.2.0.tar.gz` & `tmp/autonity-0.2.dev1.tar.gz`

## Comparing `autonity-0.2.0.tar` & `autonity-0.2.dev1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/__init__.py
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi_manager.py
--rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi_parser.py
--rw-r--r--   0        0        0    12895 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/autonity.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/committee_member.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/config.py
--rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/erc20.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/liquid_newton.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/py.typed
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/tendermint.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/validator.py
--rw-r--r--   0        0        0    26355 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/Autonity.abi
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/BytesLib.abi
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/Helpers.abi
--rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/IERC20.abi
--rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/Liquid.abi
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/Precompiled.abi
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/Upgradeable.abi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/autonity-commit.txt
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/abi/solc-version.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/utils/__init__.py
--rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/utils/denominations.py
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/utils/keyfile.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/utils/tx.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 autonity-0.2.0/autonity/utils/web3.py
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 autonity-0.2.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 autonity-0.2.0/LICENSE
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 autonity-0.2.0/README.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 autonity-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6928 2020-02-02 00:00:00.000000 autonity-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/__init__.py
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi_manager.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi_parser.py
+-rw-r--r--   0        0        0    12895 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/autonity.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/committee_member.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/config.py
+-rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/erc20.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/liquid_newton.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/py.typed
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/tendermint.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/validator.py
+-rw-r--r--   0        0        0    26355 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/Autonity.abi
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/BytesLib.abi
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/Helpers.abi
+-rw-r--r--   0        0        0     3401 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/IERC20.abi
+-rw-r--r--   0        0        0     6739 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/Liquid.abi
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/Precompiled.abi
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/Upgradeable.abi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/autonity-commit.txt
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/abi/solc-version.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/utils/__init__.py
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/utils/denominations.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/utils/keyfile.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/utils/tx.py
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 autonity-0.2.dev1/autonity/utils/web3.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 autonity-0.2.dev1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 autonity-0.2.dev1/LICENSE
+-rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 autonity-0.2.dev1/README.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 autonity-0.2.dev1/pyproject.toml
+-rw-r--r--   0        0        0     6931 2020-02-02 00:00:00.000000 autonity-0.2.dev1/PKG-INFO
```

### Comparing `autonity-0.2.0/autonity/abi_manager.py` & `autonity-0.2.dev1/autonity/abi_manager.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/abi_parser.py` & `autonity-0.2.dev1/autonity/abi_parser.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/autonity.py` & `autonity-0.2.dev1/autonity/autonity.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/committee_member.py` & `autonity-0.2.dev1/autonity/committee_member.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/config.py` & `autonity-0.2.dev1/autonity/config.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/erc20.py` & `autonity-0.2.dev1/autonity/erc20.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/liquid_newton.py` & `autonity-0.2.dev1/autonity/liquid_newton.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/tendermint.py` & `autonity-0.2.dev1/autonity/tendermint.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/validator.py` & `autonity-0.2.dev1/autonity/validator.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/abi/Autonity.abi` & `autonity-0.2.dev1/autonity/abi/Autonity.abi`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/abi/IERC20.abi` & `autonity-0.2.dev1/autonity/abi/IERC20.abi`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/abi/Liquid.abi` & `autonity-0.2.dev1/autonity/abi/Liquid.abi`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/abi/Upgradeable.abi` & `autonity-0.2.dev1/autonity/abi/Upgradeable.abi`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/utils/denominations.py` & `autonity-0.2.dev1/autonity/utils/denominations.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/utils/keyfile.py` & `autonity-0.2.dev1/autonity/utils/keyfile.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/utils/tx.py` & `autonity-0.2.dev1/autonity/utils/tx.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/autonity/utils/web3.py` & `autonity-0.2.dev1/autonity/utils/web3.py`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/LICENSE` & `autonity-0.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/README.md` & `autonity-0.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/pyproject.toml` & `autonity-0.2.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonity-0.2.0/PKG-INFO` & `autonity-0.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonity
-Version: 0.2.0
+Version: 0.2.dev1
 Summary: Python library for interacting with Autonity
 License-Expression: MIT
 License-File: LICENSE
 Keywords: autonity,client,library,rpc,web3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

