# Comparing `tmp/useragents_me_scraper-0.1.0.tar.gz` & `tmp/useragents_me_scraper-0.1.1.tar.gz`

## Comparing `useragents_me_scraper-0.1.0.tar` & `useragents_me_scraper-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/.pytest_cache/README.md
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     5534 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/src/useragents_me_scraper/useragents.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/src/useragents_me_scraper/utils.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/tests/test_useragents.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/tests/test_utils.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/LICENSE
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/README.md
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/src/useragents_me_scraper/useragents.py
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/src/useragents_me_scraper/utils.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/tests/test_useragents.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/tests/test_utils.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/LICENSE
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 useragents_me_scraper-0.1.1/PKG-INFO
```

### Comparing `useragents_me_scraper-0.1.0/.pytest_cache/v/cache/nodeids` & `useragents_me_scraper-0.1.1/.pytest_cache/v/cache/nodeids`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,44 @@
-00000000: 5b0d 0a20 2022 7465 7374 732f 7465 7374  [..  "tests/test
-00000010: 5f75 7365 7261 6765 6e74 732e 7079 3a3a  _useragents.py::
-00000020: 7465 7374 5f63 6f6e 7461 696e 735f 7661  test_contains_va
-00000030: 6c69 645f 7375 6273 7472 696e 675f 656d  lid_substring_em
-00000040: 7074 7922 2c0d 0a20 2022 7465 7374 732f  pty",..  "tests/
-00000050: 7465 7374 5f75 7365 7261 6765 6e74 732e  test_useragents.
-00000060: 7079 3a3a 7465 7374 5f63 6f6e 7461 696e  py::test_contain
-00000070: 735f 7661 6c69 645f 7375 6273 7472 696e  s_valid_substrin
-00000080: 675f 6661 6c73 6522 2c0d 0a20 2022 7465  g_false",..  "te
-00000090: 7374 732f 7465 7374 5f75 7365 7261 6765  sts/test_userage
-000000a0: 6e74 732e 7079 3a3a 7465 7374 5f63 6f6e  nts.py::test_con
-000000b0: 7461 696e 735f 7661 6c69 645f 7375 6273  tains_valid_subs
-000000c0: 7472 696e 675f 7472 7565 5f6d 756c 7469  tring_true_multi
-000000d0: 706c 6522 2c0d 0a20 2022 7465 7374 732f  ple",..  "tests/
-000000e0: 7465 7374 5f75 7365 7261 6765 6e74 732e  test_useragents.
-000000f0: 7079 3a3a 7465 7374 5f63 6f6e 7461 696e  py::test_contain
-00000100: 735f 7661 6c69 645f 7375 6273 7472 696e  s_valid_substrin
-00000110: 675f 7472 7565 5f73 696e 676c 6522 2c0d  g_true_single",.
-00000120: 0a20 2022 7465 7374 732f 7465 7374 5f75  .  "tests/test_u
-00000130: 7365 7261 6765 6e74 732e 7079 3a3a 7465  seragents.py::te
-00000140: 7374 5f69 735f 6e6f 745f 7661 6c69 645f  st_is_not_valid_
-00000150: 7063 745f 666c 6f61 7422 2c0d 0a20 2022  pct_float",..  "
-00000160: 7465 7374 732f 7465 7374 5f75 7365 7261  tests/test_usera
-00000170: 6765 6e74 732e 7079 3a3a 7465 7374 5f69  gents.py::test_i
-00000180: 735f 6e6f 745f 7661 6c69 645f 7063 745f  s_not_valid_pct_
-00000190: 696e 7422 2c0d 0a20 2022 7465 7374 732f  int",..  "tests/
-000001a0: 7465 7374 5f75 7365 7261 6765 6e74 732e  test_useragents.
-000001b0: 7079 3a3a 7465 7374 5f69 735f 7661 6c69  py::test_is_vali
-000001c0: 645f 7063 745f 666c 6f61 7422 2c0d 0a20  d_pct_float",.. 
-000001d0: 2022 7465 7374 732f 7465 7374 5f75 7365   "tests/test_use
-000001e0: 7261 6765 6e74 732e 7079 3a3a 7465 7374  ragents.py::test
-000001f0: 5f69 735f 7661 6c69 645f 7063 745f 696e  _is_valid_pct_in
-00000200: 7422 2c0d 0a20 2022 7465 7374 732f 7465  t",..  "tests/te
-00000210: 7374 5f75 7365 7261 6765 6e74 732e 7079  st_useragents.py
-00000220: 3a3a 7465 7374 5f70 726f 6365 7373 5f75  ::test_process_u
-00000230: 6122 2c0d 0a20 2022 7465 7374 732f 7465  a",..  "tests/te
-00000240: 7374 5f75 7469 6c73 2e70 793a 3a74 6573  st_utils.py::tes
-00000250: 745f 636f 6e76 6572 745f 746f 5f64 6174  t_convert_to_dat
-00000260: 6522 2c0d 0a20 2022 7465 7374 732f 7465  e",..  "tests/te
-00000270: 7374 5f75 7469 6c73 2e70 793a 3a74 6573  st_utils.py::tes
-00000280: 745f 6973 5f6e 6f74 5f6f 7574 6461 7465  t_is_not_outdate
-00000290: 6422 2c0d 0a20 2022 7465 7374 732f 7465  d",..  "tests/te
-000002a0: 7374 5f75 7469 6c73 2e70 793a 3a74 6573  st_utils.py::tes
-000002b0: 745f 6973 5f6f 7574 6461 7465 6422 0d0a  t_is_outdated"..
-000002c0: 5d                                       ]
+00000000: 5b0a 2020 2274 6573 7473 2f74 6573 745f  [.  "tests/test_
+00000010: 7573 6572 6167 656e 7473 2e70 793a 3a74  useragents.py::t
+00000020: 6573 745f 636f 6e74 6169 6e73 5f76 616c  est_contains_val
+00000030: 6964 5f73 7562 7374 7269 6e67 5f65 6d70  id_substring_emp
+00000040: 7479 222c 0a20 2022 7465 7374 732f 7465  ty",.  "tests/te
+00000050: 7374 5f75 7365 7261 6765 6e74 732e 7079  st_useragents.py
+00000060: 3a3a 7465 7374 5f63 6f6e 7461 696e 735f  ::test_contains_
+00000070: 7661 6c69 645f 7375 6273 7472 696e 675f  valid_substring_
+00000080: 6661 6c73 6522 2c0a 2020 2274 6573 7473  false",.  "tests
+00000090: 2f74 6573 745f 7573 6572 6167 656e 7473  /test_useragents
+000000a0: 2e70 793a 3a74 6573 745f 636f 6e74 6169  .py::test_contai
+000000b0: 6e73 5f76 616c 6964 5f73 7562 7374 7269  ns_valid_substri
+000000c0: 6e67 5f74 7275 655f 6d75 6c74 6970 6c65  ng_true_multiple
+000000d0: 222c 0a20 2022 7465 7374 732f 7465 7374  ",.  "tests/test
+000000e0: 5f75 7365 7261 6765 6e74 732e 7079 3a3a  _useragents.py::
+000000f0: 7465 7374 5f63 6f6e 7461 696e 735f 7661  test_contains_va
+00000100: 6c69 645f 7375 6273 7472 696e 675f 7472  lid_substring_tr
+00000110: 7565 5f73 696e 676c 6522 2c0a 2020 2274  ue_single",.  "t
+00000120: 6573 7473 2f74 6573 745f 7573 6572 6167  ests/test_userag
+00000130: 656e 7473 2e70 793a 3a74 6573 745f 6973  ents.py::test_is
+00000140: 5f6e 6f74 5f76 616c 6964 5f70 6374 5f66  _not_valid_pct_f
+00000150: 6c6f 6174 222c 0a20 2022 7465 7374 732f  loat",.  "tests/
+00000160: 7465 7374 5f75 7365 7261 6765 6e74 732e  test_useragents.
+00000170: 7079 3a3a 7465 7374 5f69 735f 6e6f 745f  py::test_is_not_
+00000180: 7661 6c69 645f 7063 745f 696e 7422 2c0a  valid_pct_int",.
+00000190: 2020 2274 6573 7473 2f74 6573 745f 7573    "tests/test_us
+000001a0: 6572 6167 656e 7473 2e70 793a 3a74 6573  eragents.py::tes
+000001b0: 745f 6973 5f76 616c 6964 5f70 6374 5f66  t_is_valid_pct_f
+000001c0: 6c6f 6174 222c 0a20 2022 7465 7374 732f  loat",.  "tests/
+000001d0: 7465 7374 5f75 7365 7261 6765 6e74 732e  test_useragents.
+000001e0: 7079 3a3a 7465 7374 5f69 735f 7661 6c69  py::test_is_vali
+000001f0: 645f 7063 745f 696e 7422 2c0a 2020 2274  d_pct_int",.  "t
+00000200: 6573 7473 2f74 6573 745f 7573 6572 6167  ests/test_userag
+00000210: 656e 7473 2e70 793a 3a74 6573 745f 7072  ents.py::test_pr
+00000220: 6f63 6573 735f 7561 222c 0a20 2022 7465  ocess_ua",.  "te
+00000230: 7374 732f 7465 7374 5f75 7469 6c73 2e70  sts/test_utils.p
+00000240: 793a 3a74 6573 745f 636f 6e76 6572 745f  y::test_convert_
+00000250: 746f 5f64 6174 6522 2c0a 2020 2274 6573  to_date",.  "tes
+00000260: 7473 2f74 6573 745f 7574 696c 732e 7079  ts/test_utils.py
+00000270: 3a3a 7465 7374 5f69 735f 6e6f 745f 6f75  ::test_is_not_ou
+00000280: 7464 6174 6564 222c 0a20 2022 7465 7374  tdated",.  "test
+00000290: 732f 7465 7374 5f75 7469 6c73 2e70 793a  s/test_utils.py:
+000002a0: 3a74 6573 745f 6973 5f6f 7574 6461 7465  :test_is_outdate
+000002b0: 6422 0a5d                                d".]
```

### Comparing `useragents_me_scraper-0.1.0/src/useragents_me_scraper/useragents.py` & `useragents_me_scraper-0.1.1/src/useragents_me_scraper/useragents.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-import json
-import requests
-import utils
-from bs4 import BeautifulSoup
-
-FILENAME = 'ua_cache.json'
-URL = "https://www.useragents.me/"
-
-
-def _save_ua_cache(ua_processed_json):
-    """ Saves the UA data into a json file.
-
-    Parameters
-    ----------
-    ua_processed_json : dict 
-      Processed ua containing start_date, end_date, and content (list of uas, pcts).
-    """
-    with open(FILENAME, 'w') as outfile:
-        json.dump(ua_processed_json, outfile)
-
-
-def _is_existing_ua_cache():
-    """ Returns true or false depending on whether a ua_cache.json exists in the local space or not.
-
-    Returns
-    -------
-    boolean
-      True if the ua_cache.json exists. False if the ua_cache.json does not exist.
-    """
-    existing_flag = False
-
-    try:
-        f = open('ua_cache.json')
-    except:
-        existing_flag = False
-    finally:
-        f.close()
-
-    return existing_flag
-
-
-def _is_outdated_ua_cache():
-    """ Returns true or false depending on whether the date today is past beyond the end_date in ua_cache.json.
-
-    Returns
-    -------
-    boolean
-      True if the ua_cache is outdated. False if the ua_cache is not outdated.
-    """
-    outdated_flag = True
-
-    with open(FILENAME, 'r') as f:
-        ua_data = json.load(f)
-        outdated_flag = utils.is_outdated(ua_data['end_date'])
-
-    return outdated_flag
-
-
-def _scrape_ua_me():
-    """ Returns true or false depending on whether the date today is past the end date argument or not.
-
-    Returns
-    -------
-    list
-      List of the raw scraped ua-pct dictionary key-value pairs scraped from useragents.me.
-    """
-    r = requests.get(URL)
-
-    content = BeautifulSoup(r.content, 'html5lib')
-
-    common_div = content.find(id="most-common-desktop-useragents-json-csv")
-    common_user_agents = common_div.div.textarea.string
-    ua_raw_json = json.loads(common_user_agents)
-
-    return ua_raw_json
-
-
-def _process_ua(ua_raw_json):
-    """ Processes ua_raw_json by adding start_date, end_date, and nesting raw ua data inside the list content key.
-
-    Parameters
-    ----------
-    ua_raw_json : 
-      List of the raw scraped ua-pct dictionary key-value pairs scraped from useragents.me.
-
-    Returns
-    -------
-    dict
-        A dictionary with start_date, end_date, and content with ua-pct key-value pairs. 
-    """
-    start_date = utils.date.today()
-    end_date = start_date + utils.timedelta(days=7)
-
-    ua_processed_json = {
-        "start_date": str(start_date),
-        "end_date": str(end_date),
-        "content": ua_raw_json
-    }
-
-    return ua_processed_json
-
-
-def _is_valid_pct(pct, min_pct, max_pct):
-    """ Returns true or false on whether the pct is within the min_pct and max_pct valid range.
-
-    Parameters
-    ----------
-    pct : float
-      The pct of a given useragent.
-    min_pct: float
-      Min range for the pct.
-    max_pct: float
-      Max range for the pct.
-
-    Returns
-    -------
-    boolean
-      True if pct is within the range. False if pct is outside the range.
-    """
-    return pct >= min_pct and pct <= max_pct
-
-
-def _contains_valid_substring(substring_list, ua_string):
-    """ Returns true or false depending on whether no substring_list was specified or any keyword inside substring_list is found within the ua_string.
-
-    Parameters
-    ----------
-    substring_list : list
-      A list containing all keywords to be searched.
-    ua_string : string
-      A useragent string to be searched with keywords for.
-
-    Returns
-    -------
-    boolean
-      True if no substring_list specified or a keyword matched within ua_string. False no keyword matched the ua_string.
-    """
-    return len(substring_list) == 0 or any(keyword in ua_string for keyword in substring_list)
-
-
-def get_uas(head=None, min_pct=0.0, max_pct=100.0, substring_list=[], cache=True):
-    """ Returns true or false depending on whether the date today is past the end date argument or not.
-
-    Parameters
-    ----------
-    head : int
-      The date that the date today is going to be compared to
-    min_pct: float
-      Min range for the pct.
-    max_pct: float
-      Max range for the pct.
-    substring_list : list
-      A list containing all keywords to be searched and matched on useragents.
-    cache : boolean
-      A flag for either caching the scraped to a ua_cache.json file that has a weeklong lifetime, or directly scraping the site. 
-
-    Returns
-    -------
-    list
-      The list of useragents filtered according to the specifications passed.
-    """
-    retrieved_uas = []
-
-    # If cache does not exist or is outdated
-    if not _is_existing_ua_cache() or _is_outdated_ua_cache():
-        # Process/Format
-        ua_raw_json = _scrape_ua_me()
-        ua_processed_json = _process_ua(ua_raw_json)
-        # Save
-        if cache:
-            _save_ua_cache(ua_processed_json)
-        else:
-            ua_data = ua_processed_json
-
-    # Loading the data
-    if cache:
-        with open('ua_cache.json', 'r') as f:
-            ua_data = json.load(f)
-
-    for ua in ua_data['content']:
-        # Filter according to pct and substring
-        if _is_valid_pct(ua['pct'], min_pct, max_pct) and _contains_valid_substring(substring_list, ua['ua']):
-            retrieved_uas.append(ua['ua'])
-        # Filter according to head
-        if head != None and len(retrieved_uas) == head:
-            break
-
-    return retrieved_uas
+import json
+import requests
+import utils
+from bs4 import BeautifulSoup
+
+FILENAME = 'ua_cache.json'
+URL = "https://www.useragents.me/"
+
+
+def _save_ua_cache(ua_processed_json):
+    """ Saves the UA data into a json file.
+
+    Parameters
+    ----------
+    ua_processed_json : dict 
+      Processed ua containing start_date, end_date, and content (list of uas, pcts).
+    """
+    with open(FILENAME, 'w') as outfile:
+        json.dump(ua_processed_json, outfile)
+
+
+def _is_existing_ua_cache():
+    """ Returns true or false depending on whether a ua_cache.json exists in the local space or not.
+
+    Returns
+    -------
+    boolean
+      True if the ua_cache.json exists. False if the ua_cache.json does not exist.
+    """
+    existing_flag = False
+
+    try:
+        f = open('ua_cache.json')
+    except:
+        existing_flag = False
+    finally:
+        f.close()
+
+    return existing_flag
+
+
+def _is_outdated_ua_cache():
+    """ Returns true or false depending on whether the date today is past beyond the end_date in ua_cache.json.
+
+    Returns
+    -------
+    boolean
+      True if the ua_cache is outdated. False if the ua_cache is not outdated.
+    """
+    outdated_flag = True
+
+    with open(FILENAME, 'r') as f:
+        ua_data = json.load(f)
+        outdated_flag = utils.is_outdated(ua_data['end_date'])
+
+    return outdated_flag
+
+
+def _scrape_ua_me():
+    """ Returns true or false depending on whether the date today is past the end date argument or not.
+
+    Returns
+    -------
+    list
+      List of the raw scraped ua-pct dictionary key-value pairs scraped from useragents.me.
+    """
+    r = requests.get(URL)
+
+    content = BeautifulSoup(r.content, 'html5lib')
+
+    common_div = content.find(id="most-common-desktop-useragents-json-csv")
+    common_user_agents = common_div.div.textarea.string
+    ua_raw_json = json.loads(common_user_agents)
+
+    return ua_raw_json
+
+
+def _process_ua(ua_raw_json):
+    """ Processes ua_raw_json by adding start_date, end_date, and nesting raw ua data inside the list content key.
+
+    Parameters
+    ----------
+    ua_raw_json : 
+      List of the raw scraped ua-pct dictionary key-value pairs scraped from useragents.me.
+
+    Returns
+    -------
+    dict
+        A dictionary with start_date, end_date, and content with ua-pct key-value pairs. 
+    """
+    start_date = utils.date.today()
+    end_date = start_date + utils.timedelta(days=7)
+
+    ua_processed_json = {
+        "start_date": str(start_date),
+        "end_date": str(end_date),
+        "content": ua_raw_json
+    }
+
+    return ua_processed_json
+
+
+def _is_valid_pct(pct, min_pct, max_pct):
+    """ Returns true or false on whether the pct is within the min_pct and max_pct valid range.
+
+    Parameters
+    ----------
+    pct : float
+      The pct of a given useragent.
+    min_pct: float
+      Min range for the pct.
+    max_pct: float
+      Max range for the pct.
+
+    Returns
+    -------
+    boolean
+      True if pct is within the range. False if pct is outside the range.
+    """
+    return pct >= min_pct and pct <= max_pct
+
+
+def _contains_valid_substring(substring_list, ua_string):
+    """ Returns true or false depending on whether no substring_list was specified or any keyword inside substring_list is found within the ua_string.
+
+    Parameters
+    ----------
+    substring_list : list
+      A list containing all keywords to be searched.
+    ua_string : string
+      A useragent string to be searched with keywords for.
+
+    Returns
+    -------
+    boolean
+      True if no substring_list specified or a keyword matched within ua_string. False no keyword matched the ua_string.
+    """
+    return len(substring_list) == 0 or any(keyword in ua_string for keyword in substring_list)
+
+
+def get_uas(head=None, min_pct=0.0, max_pct=100.0, substring_list=[], cache=True):
+    """ Returns true or false depending on whether the date today is past the end date argument or not.
+
+    Parameters
+    ----------
+    head : int
+      The date that the date today is going to be compared to
+    min_pct: float
+      Min range for the pct.
+    max_pct: float
+      Max range for the pct.
+    substring_list : list
+      A list containing all keywords to be searched and matched on useragents.
+    cache : boolean
+      A flag for either caching the scraped to a ua_cache.json file that has a weeklong lifetime, or directly scraping the site. 
+
+    Returns
+    -------
+    list
+      The list of useragents filtered according to the specifications passed.
+    """
+    retrieved_uas = []
+
+    # If cache does not exist or is outdated
+    if not _is_existing_ua_cache() or _is_outdated_ua_cache():
+        # Process/Format
+        ua_raw_json = _scrape_ua_me()
+        ua_processed_json = _process_ua(ua_raw_json)
+        # Save
+        if cache:
+            _save_ua_cache(ua_processed_json)
+        else:
+            ua_data = ua_processed_json
+
+    # Loading the data
+    if cache:
+        with open('ua_cache.json', 'r') as f:
+            ua_data = json.load(f)
+
+    for ua in ua_data['content']:
+        # Filter according to pct and substring
+        if _is_valid_pct(ua['pct'], min_pct, max_pct) and _contains_valid_substring(substring_list, ua['ua']):
+            retrieved_uas.append(ua['ua'])
+        # Filter according to head
+        if head != None and len(retrieved_uas) == head:
+            break
+
+    return retrieved_uas
```

### Comparing `useragents_me_scraper-0.1.0/src/useragents_me_scraper/utils.py` & `useragents_me_scraper-0.1.1/src/useragents_me_scraper/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from datetime import datetime, date, timedelta
-
-
-def convert_str_to_date(str_date):
-    """ Converts a string to a _Date object and returns it
-
-    Returns
-    -------
-    _Date 
-      Formatted date to YYYY-MM-DD format
-    """
-    return datetime.strptime(str_date, '%Y-%m-%d').date()
-
-
-def get_week_timeframe():
-    """ Returns two _Date values - start_date (today) and end_date (date 7 days after start_date)
-
-    Returns
-    -------
-    _Date 
-      The date today.
-    _Date
-      The date excatly 7 days after today.
-    """
-    start_date = date.today()
-    end_date = start_date + timedelta(days=7)
-    return start_date, end_date
-
-
-def is_outdated(end_date):
-    """ Returns true or false depending on whether the date today is past the end date argument or not.
-
-    Parameters
-    ----------
-    end_date : str
-      The date that the date today is going to be compared to
-
-    Returns
-    -------
-    boolean
-      True if the date is outdated. False if the date is not outdated.
-    """
-
-    end_date = convert_str_to_date(end_date)
-    return date.today() > end_date
+from datetime import datetime, date, timedelta
+
+
+def convert_str_to_date(str_date):
+    """ Converts a string to a _Date object and returns it
+
+    Returns
+    -------
+    _Date 
+      Formatted date to YYYY-MM-DD format
+    """
+    return datetime.strptime(str_date, '%Y-%m-%d').date()
+
+
+def get_week_timeframe():
+    """ Returns two _Date values - start_date (today) and end_date (date 7 days after start_date)
+
+    Returns
+    -------
+    _Date 
+      The date today.
+    _Date
+      The date excatly 7 days after today.
+    """
+    start_date = date.today()
+    end_date = start_date + timedelta(days=7)
+    return start_date, end_date
+
+
+def is_outdated(end_date):
+    """ Returns true or false depending on whether the date today is past the end date argument or not.
+
+    Parameters
+    ----------
+    end_date : str
+      The date that the date today is going to be compared to
+
+    Returns
+    -------
+    boolean
+      True if the date is outdated. False if the date is not outdated.
+    """
+
+    end_date = convert_str_to_date(end_date)
+    return date.today() > end_date
```

### Comparing `useragents_me_scraper-0.1.0/tests/test_useragents.py` & `useragents_me_scraper-0.1.1/tests/test_useragents.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-from useragents_me_scraper import useragents as ua
-
-
-def test_process_ua():
-    test_ua_json = '[{"ua":"Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36","pct":36.47},{"ua":"Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/112.0.0.0 Safari\/537.36","pct":24.17},{"ua":"Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/109.0.0.0 Safari\/537.36","pct":5.47}]'
-    test_processed_ua = ua._process_ua(test_ua_json)
-    test_content = test_ua_json
-    test_start_date, test_end_date = ua.utils.get_week_timeframe()
-
-    assert(ua.utils.convert_str_to_date(test_processed_ua['start_date']) == test_start_date and
-           ua.utils.convert_str_to_date(test_processed_ua['end_date']) == test_end_date and
-           test_processed_ua['content'] == test_content)
-
-
-def test_is_valid_pct_int():
-    assert ua._is_valid_pct(50, 0, 100) == True
-
-
-def test_is_not_valid_pct_int():
-    assert ua._is_valid_pct(0, 50, 100) == False
-
-
-def test_is_valid_pct_float():
-    assert ua._is_valid_pct(50.5, 50.0, 50.9) == True
-
-
-def test_is_not_valid_pct_float():
-    assert ua._is_valid_pct(50.0, 60.9, 70.9) == False
-
-
-def test_contains_valid_substring_empty():
-    test_ua = 'Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36'
-    substring_list = []
-    assert ua._contains_valid_substring(substring_list, test_ua) == True
-
-
-def test_contains_valid_substring_true_single():
-    test_ua = 'Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36'
-    substring_list = ['AppleWebKit']
-    assert ua._contains_valid_substring(substring_list, test_ua) == True
-
-
-def test_contains_valid_substring_true_multiple():
-    test_ua = 'Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36'
-    substring_list = ['10.0', 'Windows', 'Safari', '537.36']
-    assert ua._contains_valid_substring(substring_list, test_ua) == True
-
-
-def test_contains_valid_substring_false():
-    test_ua = 'Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36'
-    substring_list = ['5347']
-    assert ua._contains_valid_substring(substring_list, test_ua) == False
+from useragents_me_scraper import useragents as ua
+
+
+def test_process_ua():
+    test_ua_json = '[{"ua":"Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36","pct":36.47},{"ua":"Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/112.0.0.0 Safari\/537.36","pct":24.17},{"ua":"Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/109.0.0.0 Safari\/537.36","pct":5.47}]'
+    test_processed_ua = ua._process_ua(test_ua_json)
+    test_content = test_ua_json
+    test_start_date, test_end_date = ua.utils.get_week_timeframe()
+
+    assert(ua.utils.convert_str_to_date(test_processed_ua['start_date']) == test_start_date and
+           ua.utils.convert_str_to_date(test_processed_ua['end_date']) == test_end_date and
+           test_processed_ua['content'] == test_content)
+
+
+def test_is_valid_pct_int():
+    assert ua._is_valid_pct(50, 0, 100) == True
+
+
+def test_is_not_valid_pct_int():
+    assert ua._is_valid_pct(0, 50, 100) == False
+
+
+def test_is_valid_pct_float():
+    assert ua._is_valid_pct(50.5, 50.0, 50.9) == True
+
+
+def test_is_not_valid_pct_float():
+    assert ua._is_valid_pct(50.0, 60.9, 70.9) == False
+
+
+def test_contains_valid_substring_empty():
+    test_ua = 'Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36'
+    substring_list = []
+    assert ua._contains_valid_substring(substring_list, test_ua) == True
+
+
+def test_contains_valid_substring_true_single():
+    test_ua = 'Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36'
+    substring_list = ['AppleWebKit']
+    assert ua._contains_valid_substring(substring_list, test_ua) == True
+
+
+def test_contains_valid_substring_true_multiple():
+    test_ua = 'Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36'
+    substring_list = ['10.0', 'Windows', 'Safari', '537.36']
+    assert ua._contains_valid_substring(substring_list, test_ua) == True
+
+
+def test_contains_valid_substring_false():
+    test_ua = 'Mozilla\/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit\/537.36 (KHTML, like Gecko) Chrome\/111.0.0.0 Safari\/537.36'
+    substring_list = ['5347']
+    assert ua._contains_valid_substring(substring_list, test_ua) == False
```

### Comparing `useragents_me_scraper-0.1.0/pyproject.toml` & `useragents_me_scraper-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "useragents_me_scraper"
-version = "0.1.0"
-authors = [
-  { name="iDLEWINK", email="jak.uson11@yahoo.com" },
-]
-description = "An ease-of-access and non-intrusive Python web scraper using beautifulsoup to easily fetch and filter through the latest user agents found in useragents.me"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
-dependencies = [
-  "pytest",
-  "json",
-  "bs4",
-  "requests"
-]
-
-[tool.pytest.ini_options]
-pythonpath = [
-  "src", "src/useragents_me_scraper", 
-]
-
-[project.urls]
-"Homepage" = "https://github.com/iDLEWINK/useragents-me-scraper"
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "useragents_me_scraper"
+version = "0.1.1"
+authors = [
+  { name="iDLEWINK", email="jak.uson11@yahoo.com" },
+]
+description = "An ease-of-access and non-intrusive Python web scraper using beautifulsoup to easily fetch and filter through the latest user agents found in useragents.me"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = [
+    "Programming Language :: Python :: 3",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+]
+dependencies = [
+  "pytest",
+  "bs4",
+  "requests"
+]
+
+[tool.pytest.ini_options]
+pythonpath = [
+  ".", "src", "src/useragents_me_scraper", 
+]
+
+[project.urls]
+"Homepage" = "https://github.com/iDLEWINK/useragents-me-scraper"
 "Bug Tracker" = "https://github.com/iDLEWINK/useragents-me-scraper/issues"
```

### Comparing `useragents_me_scraper-0.1.0/PKG-INFO` & `useragents_me_scraper-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: useragents_me_scraper
-Version: 0.1.0
+Version: 0.1.1
 Summary: An ease-of-access and non-intrusive Python web scraper using beautifulsoup to easily fetch and filter through the latest user agents found in useragents.me
 Project-URL: Homepage, https://github.com/iDLEWINK/useragents-me-scraper
 Project-URL: Bug Tracker, https://github.com/iDLEWINK/useragents-me-scraper/issues
 Author-email: iDLEWINK <jak.uson11@yahoo.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: bs4
-Requires-Dist: json
 Requires-Dist: pytest
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 # useragents-me-scraper
```

