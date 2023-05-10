# Comparing `tmp/microsoft-kiota-serialization-json-0.3.2.tar.gz` & `tmp/microsoft-kiota-serialization-json-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft-kiota-serialization-json-0.3.2.tar", last modified: Thu Apr 27 15:39:12 2023, max compression
+gzip compressed data, was "microsoft-kiota-serialization-json-0.3.3.tar", last modified: Wed May 10 20:23:50 2023, max compression
```

## Comparing `microsoft-kiota-serialization-json-0.3.2.tar` & `microsoft-kiota-serialization-json-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
--rw-r--r--   0        0        0       82 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/CODEOWNERS
--rw-r--r--   0        0        0      240 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/dependabot.yml
--rw-r--r--   0        0        0      792 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1870 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/workflows/build_publish.yml
--rw-r--r--   0        0        0     2538 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1270 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1799 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.gitignore
--rw-r--r--   0        0        0    15976 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/.pylintrc
--rw-r--r--   0        0        0      775 2023-04-27 15:39:03.224829 microsoft-kiota-serialization-json-0.3.2/CHANGELOG.md
--rw-r--r--   0        0        0      444 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/LICENSE
--rw-r--r--   0        0        0      350 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/Pipfile
--rw-r--r--   0        0        0    35877 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/Pipfile.lock
--rw-r--r--   0        0        0     2545 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/README.md
--rw-r--r--   0        0        0     2757 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/SECURITY.md
--rw-r--r--   0        0        0     1244 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/SUPPORT.md
--rw-r--r--   0        0        0      119 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/__init__.py
--rw-r--r--   0        0        0       23 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/_version.py
--rw-r--r--   0        0        0    10526 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_parse_node.py
--rw-r--r--   0        0        0     1433 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_parse_node_factory.py
--rw-r--r--   0        0        0    17554 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_serialization_writer.py
--rw-r--r--   0        0        0     1297 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_serialization_writer_factory.py
--rw-r--r--   0        0        0     1344 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/__init__.py
--rw-r--r--   0        0        0       94 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/helpers/__init__.py
--rw-r--r--   0        0        0     1710 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/helpers/entity.py
--rw-r--r--   0        0        0      105 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/helpers/office_location.py
--rw-r--r--   0        0        0     5687 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/helpers/user.py
--rw-r--r--   0        0        0        0 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/__init__.py
--rw-r--r--   0        0        0     5926 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_parse_node.py
--rw-r--r--   0        0        0     1678 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_parse_node_factory.py
--rw-r--r--   0        0        0     6947 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_serialization_writer.py
--rw-r--r--   0        0        0     1101 2023-04-27 15:39:03.228829 microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_serialization_writer_factory.py
--rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft-kiota-serialization-json-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       82 2023-05-10 20:23:45.894541 microsoft-kiota-serialization-json-0.3.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      240 2023-05-10 20:23:45.894541 microsoft-kiota-serialization-json-0.3.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      792 2023-05-10 20:23:45.894541 microsoft-kiota-serialization-json-0.3.3/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1870 2023-05-10 20:23:45.894541 microsoft-kiota-serialization-json-0.3.3/.github/workflows/build_publish.yml
+-rw-r--r--   0        0        0     2538 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1270 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1799 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/.gitignore
+-rw-r--r--   0        0        0    15976 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/.pylintrc
+-rw-r--r--   0        0        0      885 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/LICENSE
+-rw-r--r--   0        0        0      350 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/Pipfile
+-rw-r--r--   0        0        0    35817 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/Pipfile.lock
+-rw-r--r--   0        0        0     2545 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/README.md
+-rw-r--r--   0        0        0     2757 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/SECURITY.md
+-rw-r--r--   0        0        0     1244 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/SUPPORT.md
+-rw-r--r--   0        0        0      119 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/_version.py
+-rw-r--r--   0        0        0    10604 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_parse_node.py
+-rw-r--r--   0        0        0     1445 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_parse_node_factory.py
+-rw-r--r--   0        0        0    17554 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_serialization_writer.py
+-rw-r--r--   0        0        0     1297 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     1344 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      221 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/__init__.py
+-rw-r--r--   0        0        0       94 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/helpers/__init__.py
+-rw-r--r--   0        0        0     1710 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/helpers/entity.py
+-rw-r--r--   0        0        0      105 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/helpers/office_location.py
+-rw-r--r--   0        0        0     5687 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/helpers/user.py
+-rw-r--r--   0        0        0        0 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/__init__.py
+-rw-r--r--   0        0        0     5930 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_parse_node.py
+-rw-r--r--   0        0        0     1747 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_parse_node_factory.py
+-rw-r--r--   0        0        0     6947 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_serialization_writer.py
+-rw-r--r--   0        0        0     1101 2023-05-10 20:23:45.898541 microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_serialization_writer_factory.py
+-rw-r--r--   0        0        0     3534 1970-01-01 00:00:00.000000 microsoft-kiota-serialization-json-0.3.3/PKG-INFO
```

### Comparing `microsoft-kiota-serialization-json-0.3.2/.github/workflows/auto-merge-dependabot.yml` & `microsoft-kiota-serialization-json-0.3.3/.github/workflows/auto-merge-dependabot.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/.github/workflows/build_publish.yml` & `microsoft-kiota-serialization-json-0.3.3/.github/workflows/build_publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/.github/workflows/codeql-analysis.yml` & `microsoft-kiota-serialization-json-0.3.3/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/.github/workflows/conflicting-pr-label.yml` & `microsoft-kiota-serialization-json-0.3.3/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/.gitignore` & `microsoft-kiota-serialization-json-0.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/.pylintrc` & `microsoft-kiota-serialization-json-0.3.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/CHANGELOG.md` & `microsoft-kiota-serialization-json-0.3.3/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,22 @@
 
 ## [0.3.2] - 2023-04-27
 
 ### Added
 
 ### Changed
 
+- Fixed a bug with deserializing collection of enum values.
+
+## [0.3.2] - 2023-04-27
+
+### Added
+
+### Changed
+
 - Fixed a bug with deserializing models with additional data.
 
 ## [0.3.1] - 2023-03-20
 
 ### Added
 
 ### Changed
```

### Comparing `microsoft-kiota-serialization-json-0.3.2/LICENSE` & `microsoft-kiota-serialization-json-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/Pipfile.lock` & `microsoft-kiota-serialization-json-0.3.3/Pipfile.lock`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9765361952861952%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'e80eb193cf8aeb2c98926555e2e5bae634273d94b6fb009e705500b09b3d80d5'}}",*

 * * "'default'": "{'microsoft-kiota-abstractions': {'hashes': "*

 * *              "['sha256:1e9e3696b2414e6a6787e756eb69c658743f8db2b9eef8ecc415e03f6bc8b9c9', "*

 * *              "'sha256:3ff7a0ba5d0476d7b6765d71fa3153b4198cb5507d367640d20d8e5107efd64c'], "*

 * *              "'version': '==0.5.1'}}",*

 * * "'develop'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c […]*

```diff
@@ -1,30 +1,30 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "f1900de773732b7c88935c182f6612df050dab20b558bcda2311cd66c1e9bdda"
+            "sha256": "e80eb193cf8aeb2c98926555e2e5bae634273d94b6fb009e705500b09b3d80d5"
         },
         "pipfile-spec": 6,
         "requires": {},
         "sources": [
             {
                 "name": "pypi",
                 "url": "https://pypi.org/simple",
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "microsoft-kiota-abstractions": {
             "hashes": [
-                "sha256:05235ea101725d5766408fec149c04dc2e0ca71b7b31a0e920987bb97a44cf81",
-                "sha256:6a5dfbeb2d6bc6d05e79ce3cbbd487da36fc0ddf0ecbab58ca96222ff2daa39e"
+                "sha256:1e9e3696b2414e6a6787e756eb69c658743f8db2b9eef8ecc415e03f6bc8b9c9",
+                "sha256:3ff7a0ba5d0476d7b6765d71fa3153b4198cb5507d367640d20d8e5107efd64c"
             ],
             "index": "pypi",
-            "version": "==0.5.0"
+            "version": "==0.5.1"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "index": "pypi",
@@ -54,19 +54,19 @@
                 "sha256:c81e1c7fbac615037744d067a9bb5f9aeb655edf59b63ee8b59585475d6f80d8"
             ],
             "markers": "python_full_version >= '3.7.2'",
             "version": "==2.15.4"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "charset-normalizer": {
             "hashes": [
                 "sha256:04afa6387e2b282cf78ff3dbce20f0cc071c12dc8f685bd40960cc68644cfea6",
                 "sha256:04eefcee095f58eaabe6dc3cc2262f3bcd776d2c67005880894f447b3f2cb9c1",
                 "sha256:0be65ccf618c1e7ac9b849c315cc2e8a8751d9cfdaa43027d4f6624bd587ab7e",
                 "sha256:0c95f12b74681e9ae127728f7e5409cbbef9cd914d5896ef238cc779b8152373",
@@ -154,84 +154,84 @@
             "version": "==0.4.6"
         },
         "coverage": {
             "extras": [
                 "toml"
             ],
             "hashes": [
-                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
-                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
-                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
-                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
-                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
-                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
-                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
-                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
-                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
-                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
-                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
-                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
-                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
-                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
-                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
-                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
-                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
-                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
-                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
-                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
-                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
-                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
-                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
-                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
-                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
-                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
-                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
-                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
-                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
-                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
-                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
-                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
-                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
-                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
-                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
-                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
-                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
-                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
-                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
-                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
-                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
-                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
-                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
-                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
-                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
-                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
-                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
-                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
-                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
-                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
-                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
+                "sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3",
+                "sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a",
+                "sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813",
+                "sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0",
+                "sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a",
+                "sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd",
+                "sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139",
+                "sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b",
+                "sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252",
+                "sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790",
+                "sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045",
+                "sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce",
+                "sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200",
+                "sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718",
+                "sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b",
+                "sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f",
+                "sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5",
+                "sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade",
+                "sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5",
+                "sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a",
+                "sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8",
+                "sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33",
+                "sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e",
+                "sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c",
+                "sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3",
+                "sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969",
+                "sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068",
+                "sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2",
+                "sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771",
+                "sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed",
+                "sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212",
+                "sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614",
+                "sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88",
+                "sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3",
+                "sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c",
+                "sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84",
+                "sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11",
+                "sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1",
+                "sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1",
+                "sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e",
+                "sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1",
+                "sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd",
+                "sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47",
+                "sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a",
+                "sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c",
+                "sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31",
+                "sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5",
+                "sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6",
+                "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
+                "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
+                "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.2.3"
+            "version": "==7.2.5"
         },
         "dill": {
             "hashes": [
                 "sha256:a07ffd2351b8c678dfc4a856a3005f8067aea51d6ba6c700796a4d9e280f39f0",
                 "sha256:e5db55f3687856d8fbdab002ed78544e1c4559a130302693d839dfe8f93f2373"
             ],
             "markers": "python_version < '3.11'",
             "version": "==0.3.6"
         },
         "docutils": {
             "hashes": [
-                "sha256:33995a6753c30b7f577febfc2c50411fec6aac7f7ffeb7c4cfe5991072dcf9e6",
-                "sha256:5e1de4d849fee02c63b040a4a3fd567f4ab104defd8a5511fbbc24a8a017efbc"
+                "sha256:a428f10de4de4774389734c986a01b4af2d802d26717108b0f1b9356862937c5",
+                "sha256:f75a5a52fbcacd81b47e42888ad2b380748aaccfb3f13af0fe69deb759f01eb6"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==0.19"
+            "version": "==0.20"
         },
         "exceptiongroup": {
             "hashes": [
                 "sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e",
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
@@ -373,35 +373,35 @@
                 "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==23.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:01437886022decaf285d8972f9526397bfae2ac55480ed372ed6d9eca048870a",
-                "sha256:a5e1536e5ea4b1c238a1364da17ff2993d5bd28e15600c2c8224008aff6bbcad"
+                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
+                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.4.0"
+            "version": "==3.5.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.0.0"
         },
         "pylint": {
             "hashes": [
-                "sha256:761907349e699f8afdcd56c4fe02f3021ab5b3a0fc26d19a9bfdc66c7d0d5cd5",
-                "sha256:a6cbb4c6e96eab4a3c7de7c6383c512478f58f88d95764507d84c899d656a89a"
+                "sha256:5dcf1d9e19f41f38e4e85d10f511e5b9c35e1aa74251bf95cdd8cb23584e2db1",
+                "sha256:7a1145fb08c251bdb5cca11739722ce64a63db479283d10ce718b2460e54123c"
             ],
             "index": "pypi",
-            "version": "==2.17.3"
+            "version": "==2.17.4"
         },
         "pytest": {
             "hashes": [
                 "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
                 "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
@@ -413,19 +413,19 @@
                 "sha256:996b79efde6433cdbd0088872dbc5fb3ed7fe1578b68cdbba634f14bb8dd0470"
             ],
             "index": "pypi",
             "version": "==4.0.0"
         },
         "requests": {
             "hashes": [
-                "sha256:e8f3c9be120d3333921d213eef078af392fba3933ab7ed2d1cba3b56f2568c3b",
-                "sha256:f2e34a75f4749019bb0e3effb66683630e4ffeaf75819fb51bebef1bf5aef059"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.29.0"
+            "version": "==2.30.0"
         },
         "toml": {
             "hashes": [
                 "sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b",
                 "sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f"
             ],
             "index": "pypi",
@@ -469,19 +469,19 @@
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         },
         "wrapt": {
             "hashes": [
                 "sha256:02fce1852f755f44f95af51f69d22e45080102e9d00258053b79367d07af39c0",
                 "sha256:077ff0d1f9d9e4ce6476c1a924a3332452c1406e59d90a2cf24aeb29eeac9420",
                 "sha256:078e2a1a86544e644a68422f881c48b84fef6d18f8c7a957ffd3f2e0a74a0d4a",
                 "sha256:0970ddb69bba00670e58955f8019bec4a42d1785db3faa043c33d81de2bf843c",
```

### Comparing `microsoft-kiota-serialization-json-0.3.2/README.md` & `microsoft-kiota-serialization-json-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/SECURITY.md` & `microsoft-kiota-serialization-json-0.3.3/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/SUPPORT.md` & `microsoft-kiota-serialization-json-0.3.3/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_parse_node.py` & `microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_parse_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,33 +172,33 @@
         return list(map(func, list(self._json_node)))
 
     def get_collection_of_object_values(self, factory: ParsableFactory) -> List[U]:
         """Gets the collection of type U values from the json node
         Returns:
             List[U]: The collection of model object values of the node
         """
+        object_collection = self._json_node
+        if not object_collection:
+            return []
         return list(
             map(
                 lambda x: JsonParseNode(x).get_object_value(factory),  # type: ignore
-                self._json_node
+                object_collection
             )
         )
 
     def get_collection_of_enum_values(self, enum_class: K) -> List[Optional[K]]:
         """Gets the collection of enum values of the json node
         Returns:
             List[K]: The collection of enum values
         """
-        raw_values = self.get_str_value()
-        if not raw_values:
+        enum_collection = self._json_node
+        if not enum_collection:
             return []
-
-        return list(
-            map(lambda x: JsonParseNode(x).get_enum_value(enum_class), raw_values.split(","))
-        )
+        return list(map(lambda x: JsonParseNode(x).get_enum_value(enum_class), enum_collection))
 
     def get_enum_value(self, enum_class: K) -> Optional[K]:
         """Gets the enum value of the node
         Returns:
             Optional[K]: The enum value of the node
         """
         raw_key = self.get_str_value()
```

### Comparing `microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_parse_node_factory.py` & `microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_parse_node_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,9 +31,9 @@
         if valid_content_type.casefold() != content_type.casefold():
             raise TypeError(f"Expected {valid_content_type} as content type")
 
         if not content:
             raise TypeError("Content cannot be null")
 
         content_as_str = content.decode('utf-8')
-        content_dict = json.loads(content_as_str)
+        content_dict = json.loads(json.dumps(content_as_str))
         return JsonParseNode(content_dict)
```

### Comparing `microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_serialization_writer.py` & `microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/kiota_serialization_json/json_serialization_writer_factory.py` & `microsoft-kiota-serialization-json-0.3.3/kiota_serialization_json/json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/pyproject.toml` & `microsoft-kiota-serialization-json-0.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/tests/helpers/entity.py` & `microsoft-kiota-serialization-json-0.3.3/tests/helpers/entity.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/tests/helpers/user.py` & `microsoft-kiota-serialization-json-0.3.3/tests/helpers/user.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_parse_node.py` & `microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_parse_node.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 def test_get_bytes_value():
     parse_node = JsonParseNode('U2Ftd2VsIGlzIHRoZSBiZXN0')
     result = parse_node.get_bytes_value()
     assert isinstance(result, bytes)
 
 
 def test_get_collection_of_enum_values():
-    parse_node = JsonParseNode("dunhill,oval")
+    parse_node = JsonParseNode(["dunhill","oval"])
     result = parse_node.get_collection_of_enum_values(OfficeLocation)
     assert isinstance(result, list)
     assert result == [OfficeLocation.Dunhill, OfficeLocation.Oval]
 
 
 def test_get_enum_value():
     parse_node = JsonParseNode("dunhill")
```

### Comparing `microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_parse_node_factory.py` & `microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_parse_node_factory.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 def test_get_root_parse_node(sample_json_string):
     factory = JsonParseNodeFactory()
     sample_json_string_bytes = sample_json_string.encode('utf-8')
     root = factory.get_root_parse_node('application/json', sample_json_string_bytes)
     assert isinstance(root, JsonParseNode)
-
+    assert str(root.get_bytes_value(), "utf-8") == sample_json_string
 
 def test_get_root_parse_node_no_content_type(sample_json_string):
     with pytest.raises(Exception) as e_info:
         factory = JsonParseNodeFactory()
         sample_json_string_bytes = sample_json_string.encode('utf-8')
         root = factory.get_root_parse_node('', sample_json_string_bytes)
```

### Comparing `microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_serialization_writer.py` & `microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/tests/unit/test_json_serialization_writer_factory.py` & `microsoft-kiota-serialization-json-0.3.3/tests/unit/test_json_serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft-kiota-serialization-json-0.3.2/PKG-INFO` & `microsoft-kiota-serialization-json-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-serialization-json
-Version: 0.3.2
+Version: 0.3.3
 Summary: Implementation of Kiota Serialization interfaces for JSON
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

