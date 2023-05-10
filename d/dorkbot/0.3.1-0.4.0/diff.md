# Comparing `tmp/dorkbot-0.3.1.tar.gz` & `tmp/dorkbot-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorkbot-0.3.1.tar", last modified: Tue Apr 25 21:22:20 2023, max compression
+gzip compressed data, was "dorkbot-0.4.0.tar", last modified: Wed May 10 00:12:43 2023, max compression
```

## Comparing `dorkbot-0.3.1.tar` & `dorkbot-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:20.005293 dorkbot-0.3.1/
--rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.3.1/LICENSE
--rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.3.1/MANIFEST.in
--rw-r--r--   0 jgor       (501) staff       (20)    10550 2023-04-25 21:22:20.005400 dorkbot-0.3.1/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)    10148 2023-04-25 17:56:00.000000 dorkbot-0.3.1/README.md
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:19.976103 dorkbot-0.3.1/dorkbot/
--rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)       22 2023-04-25 21:22:09.000000 dorkbot-0.3.1/dorkbot/_version.py
--rwxr-xr-x   0 jgor       (501) staff       (20)    28397 2023-04-25 21:19:09.000000 dorkbot-0.3.1/dorkbot/dorkbot.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:19.999926 dorkbot-0.3.1/dorkbot/indexers/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     1714 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/bing_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     5474 2023-04-25 17:09:52.000000 dorkbot-0.3.1/dorkbot/indexers/commoncrawl.py
--rw-r--r--   0 jgor       (501) staff       (20)      329 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/google.js
--rw-r--r--   0 jgor       (501) staff       (20)     1910 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/google.py
--rw-r--r--   0 jgor       (501) staff       (20)     2630 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/google_api.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     5643 2023-04-25 17:59:04.000000 dorkbot-0.3.1/dorkbot/indexers/pywb.py
--rw-r--r--   0 jgor       (501) staff       (20)      412 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/stdin.py
--rwxr-xr-x   0 jgor       (501) staff       (20)     4131 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/indexers/wayback.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:20.004790 dorkbot-0.3.1/dorkbot/scanners/
--rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/scanners/__init__.py
--rw-r--r--   0 jgor       (501) staff       (20)     2733 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/scanners/arachni.py
--rw-r--r--   0 jgor       (501) staff       (20)      673 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/scanners/example.py
--rw-r--r--   0 jgor       (501) staff       (20)     2524 2023-04-19 17:48:56.000000 dorkbot-0.3.1/dorkbot/scanners/wapiti.py
-drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-04-25 21:22:19.978465 dorkbot-0.3.1/dorkbot.egg-info/
--rw-r--r--   0 jgor       (501) staff       (20)    10550 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/PKG-INFO
--rw-r--r--   0 jgor       (501) staff       (20)      659 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/SOURCES.txt
--rw-r--r--   0 jgor       (501) staff       (20)        1 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/dependency_links.txt
--rw-r--r--   0 jgor       (501) staff       (20)       49 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/entry_points.txt
--rw-r--r--   0 jgor       (501) staff       (20)        8 2023-04-25 21:22:19.000000 dorkbot-0.3.1/dorkbot.egg-info/top_level.txt
--rw-r--r--   0 jgor       (501) staff       (20)       74 2023-04-25 21:22:20.006638 dorkbot-0.3.1/setup.cfg
--rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.3.1/setup.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.852147 dorkbot-0.4.0/
+-rw-r--r--   0 jgor       (501) staff       (20)    10596 2023-04-19 17:48:56.000000 dorkbot-0.4.0/LICENSE
+-rw-r--r--   0 jgor       (501) staff       (20)       35 2023-04-19 17:48:56.000000 dorkbot-0.4.0/MANIFEST.in
+-rw-r--r--   0 jgor       (501) staff       (20)    11006 2023-05-10 00:12:43.852231 dorkbot-0.4.0/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)    10604 2023-05-09 23:21:26.000000 dorkbot-0.4.0/README.md
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.797481 dorkbot-0.4.0/dorkbot/
+-rw-r--r--   0 jgor       (501) staff       (20)       34 2023-04-19 17:48:56.000000 dorkbot-0.4.0/dorkbot/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)       22 2023-05-10 00:12:10.000000 dorkbot-0.4.0/dorkbot/_version.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)    32189 2023-05-09 22:36:28.000000 dorkbot-0.4.0/dorkbot/dorkbot.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.839483 dorkbot-0.4.0/dorkbot/indexers/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.0/dorkbot/indexers/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     1870 2023-05-09 22:35:43.000000 dorkbot-0.4.0/dorkbot/indexers/bing_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     6022 2023-05-09 19:41:07.000000 dorkbot-0.4.0/dorkbot/indexers/commoncrawl.py
+-rw-r--r--   0 jgor       (501) staff       (20)      479 2023-05-09 19:40:01.000000 dorkbot-0.4.0/dorkbot/indexers/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3131 2023-04-27 19:42:53.000000 dorkbot-0.4.0/dorkbot/indexers/google.js
+-rw-r--r--   0 jgor       (501) staff       (20)     2221 2023-05-09 19:40:36.000000 dorkbot-0.4.0/dorkbot/indexers/google.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3008 2023-05-09 19:40:46.000000 dorkbot-0.4.0/dorkbot/indexers/google_api.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     6279 2023-05-09 19:41:26.000000 dorkbot-0.4.0/dorkbot/indexers/pywb.py
+-rw-r--r--   0 jgor       (501) staff       (20)      562 2023-05-09 19:40:11.000000 dorkbot-0.4.0/dorkbot/indexers/stdin.py
+-rwxr-xr-x   0 jgor       (501) staff       (20)     4674 2023-05-09 21:01:22.000000 dorkbot-0.4.0/dorkbot/indexers/wayback.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.851677 dorkbot-0.4.0/dorkbot/scanners/
+-rw-r--r--   0 jgor       (501) staff       (20)        0 2023-04-19 17:48:56.000000 dorkbot-0.4.0/dorkbot/scanners/__init__.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3397 2023-05-09 21:38:35.000000 dorkbot-0.4.0/dorkbot/scanners/arachni.py
+-rw-r--r--   0 jgor       (501) staff       (20)      913 2023-05-08 20:47:36.000000 dorkbot-0.4.0/dorkbot/scanners/example.py
+-rw-r--r--   0 jgor       (501) staff       (20)     3160 2023-05-09 21:38:21.000000 dorkbot-0.4.0/dorkbot/scanners/wapiti.py
+drwxr-xr-x   0 jgor       (501) staff       (20)        0 2023-05-10 00:12:43.807522 dorkbot-0.4.0/dorkbot.egg-info/
+-rw-r--r--   0 jgor       (501) staff       (20)    11006 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/PKG-INFO
+-rw-r--r--   0 jgor       (501) staff       (20)      659 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/SOURCES.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        1 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/dependency_links.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       49 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/entry_points.txt
+-rw-r--r--   0 jgor       (501) staff       (20)        8 2023-05-10 00:12:43.000000 dorkbot-0.4.0/dorkbot.egg-info/top_level.txt
+-rw-r--r--   0 jgor       (501) staff       (20)       74 2023-05-10 00:12:43.852897 dorkbot-0.4.0/setup.cfg
+-rw-r--r--   0 jgor       (501) staff       (20)      950 2023-04-19 17:48:56.000000 dorkbot-0.4.0/setup.py
```

### Comparing `dorkbot-0.3.1/LICENSE` & `dorkbot-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.1/PKG-INFO` & `dorkbot-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.3.1
+Version: 0.4.0
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
@@ -29,87 +29,100 @@
 ==========
 * Create a Google API credential via the [Developer Console](https://console.developers.google.com)
 * Create a Google [Custom Search Engine](https://www.google.com/cse/) and note the search engine ID, e.g. 012345678901234567891:abc12defg3h
 <pre>$ pip3 install dorkbot wapiti3</pre>
 <pre>$ dorkbot -i google_api -o key=your_api_credential_here -o engine=your_engine_id_here -o query="filetype:php inurl:id"</pre>
 <pre>$ dorkbot -s wapiti</pre>
 
+Help
+====
+<pre>
+ -h, --help            Show program (or specified module) help
+</pre>
+<pre>
+  --show-defaults       Show default values in help output
+</pre>
+
 Usage
 =====
 <pre>
-usage: dorkbot [-h] [-c CONFIG] [-r DIRECTORY] [--log LOG] [-v] [-V]
-                  [-d DATABASE] [-u] [-l] [--list-unscanned]
-                  [--add-target TARGET] [--delete-target TARGET]
-                  [--flush-targets] [-i INDEXER] [-o INDEXER_OPTION]
-                  [-s SCANNER] [-p SCANNER_OPTION] [-f] [-b BLACKLIST]
-                  [--list-blacklist] [--add-blacklist-item ITEM]
-                  [--delete-blacklist-item ITEM] [--flush-blacklist]
+usage: dorkbot.py [-c CONFIG] [-r DIRECTORY] [--source [SOURCE]]
+                  [--show-defaults] [--count COUNT] [--random] [-h]
+                  [--log LOG] [-v] [-V] [-d DATABASE] [-u] [-l]
+                  [--list-unscanned] [--add-target TARGET]
+                  [--delete-target TARGET] [--flush-targets] [-i INDEXER]
+                  [-o INDEXER_ARG] [-s SCANNER] [-p SCANNER_ARG] [-f]
+                  [-b BLOCKLIST] [--list-blocklist]
+                  [--add-blocklist-item ITEM] [--delete-blocklist-item ITEM]
+                  [--flush-blocklist]
 
-optional arguments:
-  -h, --help            show this help message and exit
+options:
   -c CONFIG, --config CONFIG
                         Configuration file
   -r DIRECTORY, --directory DIRECTORY
                         Dorkbot directory (default location of db, tools,
                         reports)
+  --source [SOURCE]     Label associated with targets
+  --show-defaults       Show default values in help output
+  -h, --help            Show program (or specified module) help
   --log LOG             Path to log file
   -v, --verbose         Enable verbose logging (DEBUG output)
   -V, --version         Print version
 
+global scanner options:
+  --count COUNT         number of urls to scan, or -1 to scan all urls
+  --random              retrieve urls in random order
+
 database:
   -d DATABASE, --database DATABASE
                         Database file/uri
-  -u, --prune           Apply fingerprinting and blacklist without scanning
+  -u, --prune           Apply fingerprinting and blocklist without scanning
 
 targets:
   -l, --list-targets    List targets in database
   --list-unscanned      List unscanned targets in database
   --add-target TARGET   Add a url to the target database
   --delete-target TARGET
                         Delete a url from the target database
   --flush-targets       Delete all targets
 
 indexing:
   -i INDEXER, --indexer INDEXER
                         Indexer module to use
-  -o INDEXER_OPTION, --indexer-option INDEXER_OPTION
-                        Pass an option to the indexer (can be used multiple
-                        times)
+  -o INDEXER_ARG, --indexer-arg INDEXER_ARG
+                        Pass an argument to the indexer module (can be used
+                        multiple times)
 
 scanning:
   -s SCANNER, --scanner SCANNER
                         Scanner module to use
-  -p SCANNER_OPTION, --scanner-option SCANNER_OPTION
-                        Pass an option to the scanner (can be used multiple
-                        times)
+  -p SCANNER_ARG, --scanner-arg SCANNER_ARG
+                        Pass an argument to the scanner module (can be used
+                        multiple times)
 
 fingerprints:
   -f, --flush-fingerprints
                         Delete all fingerprints of previously-scanned items
 
-blacklist:
-  -b BLACKLIST, --blacklist BLACKLIST
-                        Blacklist file/uri
-  --list-blacklist      List blacklist entries
-  --add-blacklist-item ITEM
-                        Add an ip/host/regex pattern to the blacklist
-  --delete-blacklist-item ITEM
-                        Delete an item from the blacklist
-  --flush-blacklist     Delete all blacklist items
+blocklist:
+  -b BLOCKLIST, --blocklist BLOCKLIST
+                        Blocklist file/uri
+  --list-blocklist      List blocklist entries
+  --add-blocklist-item ITEM
+                        Add an ip/host/regex pattern to the blocklist
+  --delete-blocklist-item ITEM
+                        Delete an item from the blocklist
+  --flush-blocklist     Delete all blocklist items
 </pre>
 
-Requirements
-============
-* Python 3.x (cross-platform)
+Tools / Dependencies
+=====
 * [psycopg2-binary](https://pypi.org/project/psycopg2-binary/) or [psycopg2](https://pypi.org/project/psycopg2/) (if using PostgreSQL)
 * [phoenixdb](https://pypi.org/project/phoenixdb/) (if using PhoenixDB)
-
-Tools
-=====
-* [PhantomJS](http://phantomjs.org/)
+* [PhantomJS](http://phantomjs.org/) (if using non-api google indexer)
 * [Arachni](http://www.arachni-scanner.com/)
 * [Wapiti](http://wapiti.sourceforge.net/)
 
 As needed, dorkbot will search for tools in the following order:
 * Directory specified via relevant module option
 * Located in *tools* directory (within current directory, by default), with the subdirectory named after the tool
 * Available in the user's PATH (e.g. installed system-wide)
@@ -130,146 +143,148 @@
 ===========
 The configuration file (dorkbot.ini) can be used to prepopulate certain command-line flags.
 
 Example dorkbot.ini:
 <pre>
 [dorkbot]
 database=/opt/dorkbot/dorkbot.db
+[indexers.wayback]
+domain=example.com
+from=2022
+[scanners.arachni]
+arachni_dir=/opt/arachni
+report_dir=/tmp/reports
 </pre>
 
-Blacklist
+Blocklist
 =========
-The blacklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. By default the blacklist is stored in the dorkbot database, but a separate database or file can be specified by passing the appropriate connection uri or file path to --blacklist. Note: --add-blacklist-item / --delete-blacklist-item are not implemented for file-based blacklists, and --flush-blacklist deletes the file.
+The blocklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. By default the blocklist is stored in the dorkbot database, but a separate database or file can be specified by passing the appropriate connection uri or file path to --blocklist. Note: --add-blocklist-item / --delete-blocklist-item are not implemented for file-based blocklists, and --flush-blocklist deletes the file.
 
-Supported external blacklists:
+Supported external blocklists:
 * postgresql://[server info]
 * phoenixdb://[server info]
-* sqlite3:///path/to/blacklist.db
-* /path/to/blacklist.txt
+* sqlite3:///path/to/blocklist.db
+* /path/to/blocklist.txt
 
-Example blacklist items:
+Example blocklist items:
 <pre>
 regex:^[^\?]+$
 regex:.*login.*
 regex:^https?://[^.]*.example.com/.*
 host:www.google.com
 ip:127.0.0.1
 </pre>
 
-The first item will remove any target that doesn't contain a question mark, in other words any url that doesn't contain any GET parameters to test. The second attempts to avoid login functions, and the third blacklists all target urls on example.com. The fourth excludes targets with a hostname of www.google.com and the fifth excludes targets whose host resolves to 127.0.0.1.
+The first item will remove any target that doesn't contain a question mark, in other words any url that doesn't contain any GET parameters to test. The second attempts to avoid login functions, and the third blocklists all target urls on example.com. The fourth excludes targets with a hostname of www.google.com and the fifth excludes targets whose host resolves to 127.0.0.1.
 
-Indexer Modules
-===============
-### (general options) ###
-These options are applicable regardless of module chosen
+Prune
+=====
+The prune flag iterates through all targets, computes the fingerprints in memory, and marks subsequent matching targets as scanned. Additionally it deletes any target matching a blocklist item. The result is a database where --list-unscanned returns only scannable urls. It honors the **random** flag to compute fingerprints in random order.
 
-* source - label stored in source field for target, overrides label provided by module (if present and without a value during list operations, source field will be printed along with url)
+General Options
+===============
+These options are applicable regardless of module chosen:
+<pre>
+  --source [SOURCE]     Label associated with targets
+  --count COUNT         number of urls to scan, or -1 to scan all urls
+  --random              retrieve urls in random order
+</pre>
 
+Indexer Modules
+===============
 ### google ###
-Search for targets in a Google Custom Search Engine (CSE) via custom search element.
-
-Requirements: [PhantomJS](http://phantomjs.org/)
+<pre>
+  Searches google.com via scraping
 
-Options:
-* **engine** - CSE id
-* **query** - search query
-* phantomjs_dir - phantomjs base directory containing bin/phantomjs (default: tools/phantomjs/)
-* domain - limit searches to specified domain
+  --engine ENGINE       CSE id
+  --query QUERY         search query
+  --phantomjs-dir PHANTOMJS_DIR
+                        phantomjs base dir containing bin/phantomjs
+  --domain DOMAIN       limit searches to specified domain
+</pre>
 
 ### google_api ###
-Search for targets in a Google Custom Search Engine (CSE) via JSON API.
-
-Requirements: none
+<pre>
+  Searches google.com
 
-Options:
-* **key** - API key
-* **engine** - CSE id
-* **query** - search query
-* domain - limit searches to specified domain
+  --key KEY             API key
+  --engine ENGINE       CSE id
+  --query QUERY         search query
+  --domain DOMAIN       limit searches to specified domain
+</pre>
 
 ### pywb ###
-Search for targets within a pywb instance's indexed results.
-
-Requirements: none
+<pre>
+  Searches a given pywb server's crawl data
 
-Options:
-* **server** - pywb server url
-* **domain** - pull all results for given domain or subdomain
-* cdx_api_suffix - suffix after index for index api (default: /cdx)
-* index - search a specific index (default: first fixed index, or first dynamic index)
-* filter - query filter to apply to the search
-* retries - number of times to retry fetching results on error (default: 10)
-* threads - number concurrent requests to pywb server (default: 10)
+  --server SERVER       pywb server url
+  --domain DOMAIN       pull all results for given domain or subdomain
+  --cdx-api-suffix CDX_API_SUFFIX
+                        suffix after index for index api
+  --index INDEX         search a specific index
+  --filter FILTER       query filter to apply to the search
+  --retries RETRIES     number of times to retry fetching results on error
+  --threads THREADS     number of concurrent requests to wayback.org
+</pre>
 
 ### commoncrawl ###
-Search for targets within commoncrawl.org results.
-
-Requirements: none
+<pre>
+  Searches commoncrawl.org crawl data
 
-Options:
-* **domain** - pull all results for given domain or subdomain
-* index - search a specific index, e.g. CC-MAIN-2019-22 (default: latest)
-* filter - query filter to apply to the search
-* retries - number of times to retry fetching results on error (default: 10)
-* threads - number concurrent requests to commoncrawl.org (default: 10)
+  --domain DOMAIN       pull all results for given domain or subdomain
+  --index INDEX         search a specific index, e.g. CC-MAIN-2019-22 (default: latest)
+  --filter FILTER       query filter to apply to the search
+  --retries RETRIES     number of times to retry fetching results on error
+  --threads THREADS     number of concurrent requests to commoncrawl.org
+</pre>
 
 ### wayback ###
-Search for targets within archive.org results.
-
-Requirements: none
+<pre>
+  Searches archive.org crawl data
 
-Options:
-* **domain** - pull all results for given domain or subdomain
-* filter - query filter to apply to the search
-* from - beginning timestamp
-* to - end timestamp
+  --domain DOMAIN       pull all results for given domain or subdomain
+  --filter FILTER       query filter to apply to the search
+  --from FROM           beginning timestamp
+  --to TO               end timestamp
+  --retries RETRIES     number of times to retry fetching results on error
+  --threads THREADS     number of concurrent requests to wayback.org
+</pre>
 
 ### bing_api ###
-Search for targets via Bing Web Search API.
-
-Requirements: none
+<pre>
+  Searches bing.com
 
-Options:
-* **key** - API key
-* **query** - search query
+  --key KEY             API key
+  --query QUERY         search query
+</pre>
 
 ### stdin ###
-Read targets from standard input, one per line.
-
-Requirements: none
-
-Options: none
+<pre>
+  Accepts urls from stdin, one per line
+</pre>
 
 Scanner Modules
 ===============
-### (general options) ###
-These options are applicable regardless of module chosen
-
-* report_dir - directory to save vulnerability report (default: reports/)
-* label - friendly name field to include in vulnerability report
-* count - number of urls to scan, or -1 to scan all urls (default: -1)
-* random - scan urls in random order
-
 ### arachni ###
-Scan targets with Arachni command-line scanner.
-
-Requirements: [Arachni](http://www.arachni-scanner.com/)
+<pre>
+  Scans with the arachni command-line scanner
 
-Options:
-* arachni_dir - arachni base directory containing bin/arachni and bin/arachni_reporter (default: tools/arachni/)
-* args - space-delimited list of additional arguments, e.g. args="--http-user-agent Dorkbot/1.0 --timeout 00:15:00"
+  --arachni-dir ARACHNI_DIR
+                        arachni base dir containing bin/arachni and bin/arachni_reporter
+  --args ARGS           space-delimited list of additional arguments
+  --report-dir REPORT_DIR
+                        directory to save vulnerability report
+  --label LABEL         friendly name field to include in vulnerability report
+</pre>
 
 ### wapiti ###
-Scan targets with Wapiti command-line scanner.
-
-Requirements: [Wapiti](http://wapiti.sourceforge.net/)
-
-Options:
-* wapiti_dir - wapiti base directory containing bin/wapiti (default: tools/wapiti/)
-* args - space-delimited list of additional arguments
-
-Prune
-=====
-The prune flag iterates through all targets, computes the fingerprints in memory, and marks subsequent matching targets as scanned. Additionally it deletes any target matching a blacklist item. The result is a database where --list-unscanned returns only scannable urls. It honors (a subset of) the options specified in SCANNER_OPTIONS as follows:
+<pre>
+  Scans with the wapiti3 command-line scanner
 
-* random - evaluate urls in random order when computing fingerprints
+  --wapiti-dir WAPITI_DIR
+                        wapiti base dir containing bin/wapiti
+  --args ARGS           space-delimited list of additional arguments
+  --report-dir REPORT_DIR
+                        directory to save vulnerability report
+  --label LABEL         friendly name field to include in vulnerability report
+</pre>
```

### Comparing `dorkbot-0.3.1/README.md` & `dorkbot-0.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -16,87 +16,100 @@
 ==========
 * Create a Google API credential via the [Developer Console](https://console.developers.google.com)
 * Create a Google [Custom Search Engine](https://www.google.com/cse/) and note the search engine ID, e.g. 012345678901234567891:abc12defg3h
 <pre>$ pip3 install dorkbot wapiti3</pre>
 <pre>$ dorkbot -i google_api -o key=your_api_credential_here -o engine=your_engine_id_here -o query="filetype:php inurl:id"</pre>
 <pre>$ dorkbot -s wapiti</pre>
 
+Help
+====
+<pre>
+ -h, --help            Show program (or specified module) help
+</pre>
+<pre>
+  --show-defaults       Show default values in help output
+</pre>
+
 Usage
 =====
 <pre>
-usage: dorkbot [-h] [-c CONFIG] [-r DIRECTORY] [--log LOG] [-v] [-V]
-                  [-d DATABASE] [-u] [-l] [--list-unscanned]
-                  [--add-target TARGET] [--delete-target TARGET]
-                  [--flush-targets] [-i INDEXER] [-o INDEXER_OPTION]
-                  [-s SCANNER] [-p SCANNER_OPTION] [-f] [-b BLACKLIST]
-                  [--list-blacklist] [--add-blacklist-item ITEM]
-                  [--delete-blacklist-item ITEM] [--flush-blacklist]
+usage: dorkbot.py [-c CONFIG] [-r DIRECTORY] [--source [SOURCE]]
+                  [--show-defaults] [--count COUNT] [--random] [-h]
+                  [--log LOG] [-v] [-V] [-d DATABASE] [-u] [-l]
+                  [--list-unscanned] [--add-target TARGET]
+                  [--delete-target TARGET] [--flush-targets] [-i INDEXER]
+                  [-o INDEXER_ARG] [-s SCANNER] [-p SCANNER_ARG] [-f]
+                  [-b BLOCKLIST] [--list-blocklist]
+                  [--add-blocklist-item ITEM] [--delete-blocklist-item ITEM]
+                  [--flush-blocklist]
 
-optional arguments:
-  -h, --help            show this help message and exit
+options:
   -c CONFIG, --config CONFIG
                         Configuration file
   -r DIRECTORY, --directory DIRECTORY
                         Dorkbot directory (default location of db, tools,
                         reports)
+  --source [SOURCE]     Label associated with targets
+  --show-defaults       Show default values in help output
+  -h, --help            Show program (or specified module) help
   --log LOG             Path to log file
   -v, --verbose         Enable verbose logging (DEBUG output)
   -V, --version         Print version
 
+global scanner options:
+  --count COUNT         number of urls to scan, or -1 to scan all urls
+  --random              retrieve urls in random order
+
 database:
   -d DATABASE, --database DATABASE
                         Database file/uri
-  -u, --prune           Apply fingerprinting and blacklist without scanning
+  -u, --prune           Apply fingerprinting and blocklist without scanning
 
 targets:
   -l, --list-targets    List targets in database
   --list-unscanned      List unscanned targets in database
   --add-target TARGET   Add a url to the target database
   --delete-target TARGET
                         Delete a url from the target database
   --flush-targets       Delete all targets
 
 indexing:
   -i INDEXER, --indexer INDEXER
                         Indexer module to use
-  -o INDEXER_OPTION, --indexer-option INDEXER_OPTION
-                        Pass an option to the indexer (can be used multiple
-                        times)
+  -o INDEXER_ARG, --indexer-arg INDEXER_ARG
+                        Pass an argument to the indexer module (can be used
+                        multiple times)
 
 scanning:
   -s SCANNER, --scanner SCANNER
                         Scanner module to use
-  -p SCANNER_OPTION, --scanner-option SCANNER_OPTION
-                        Pass an option to the scanner (can be used multiple
-                        times)
+  -p SCANNER_ARG, --scanner-arg SCANNER_ARG
+                        Pass an argument to the scanner module (can be used
+                        multiple times)
 
 fingerprints:
   -f, --flush-fingerprints
                         Delete all fingerprints of previously-scanned items
 
-blacklist:
-  -b BLACKLIST, --blacklist BLACKLIST
-                        Blacklist file/uri
-  --list-blacklist      List blacklist entries
-  --add-blacklist-item ITEM
-                        Add an ip/host/regex pattern to the blacklist
-  --delete-blacklist-item ITEM
-                        Delete an item from the blacklist
-  --flush-blacklist     Delete all blacklist items
+blocklist:
+  -b BLOCKLIST, --blocklist BLOCKLIST
+                        Blocklist file/uri
+  --list-blocklist      List blocklist entries
+  --add-blocklist-item ITEM
+                        Add an ip/host/regex pattern to the blocklist
+  --delete-blocklist-item ITEM
+                        Delete an item from the blocklist
+  --flush-blocklist     Delete all blocklist items
 </pre>
 
-Requirements
-============
-* Python 3.x (cross-platform)
+Tools / Dependencies
+=====
 * [psycopg2-binary](https://pypi.org/project/psycopg2-binary/) or [psycopg2](https://pypi.org/project/psycopg2/) (if using PostgreSQL)
 * [phoenixdb](https://pypi.org/project/phoenixdb/) (if using PhoenixDB)
-
-Tools
-=====
-* [PhantomJS](http://phantomjs.org/)
+* [PhantomJS](http://phantomjs.org/) (if using non-api google indexer)
 * [Arachni](http://www.arachni-scanner.com/)
 * [Wapiti](http://wapiti.sourceforge.net/)
 
 As needed, dorkbot will search for tools in the following order:
 * Directory specified via relevant module option
 * Located in *tools* directory (within current directory, by default), with the subdirectory named after the tool
 * Available in the user's PATH (e.g. installed system-wide)
@@ -117,146 +130,148 @@
 ===========
 The configuration file (dorkbot.ini) can be used to prepopulate certain command-line flags.
 
 Example dorkbot.ini:
 <pre>
 [dorkbot]
 database=/opt/dorkbot/dorkbot.db
+[indexers.wayback]
+domain=example.com
+from=2022
+[scanners.arachni]
+arachni_dir=/opt/arachni
+report_dir=/tmp/reports
 </pre>
 
-Blacklist
+Blocklist
 =========
-The blacklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. By default the blacklist is stored in the dorkbot database, but a separate database or file can be specified by passing the appropriate connection uri or file path to --blacklist. Note: --add-blacklist-item / --delete-blacklist-item are not implemented for file-based blacklists, and --flush-blacklist deletes the file.
+The blocklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. By default the blocklist is stored in the dorkbot database, but a separate database or file can be specified by passing the appropriate connection uri or file path to --blocklist. Note: --add-blocklist-item / --delete-blocklist-item are not implemented for file-based blocklists, and --flush-blocklist deletes the file.
 
-Supported external blacklists:
+Supported external blocklists:
 * postgresql://[server info]
 * phoenixdb://[server info]
-* sqlite3:///path/to/blacklist.db
-* /path/to/blacklist.txt
+* sqlite3:///path/to/blocklist.db
+* /path/to/blocklist.txt
 
-Example blacklist items:
+Example blocklist items:
 <pre>
 regex:^[^\?]+$
 regex:.*login.*
 regex:^https?://[^.]*.example.com/.*
 host:www.google.com
 ip:127.0.0.1
 </pre>
 
-The first item will remove any target that doesn't contain a question mark, in other words any url that doesn't contain any GET parameters to test. The second attempts to avoid login functions, and the third blacklists all target urls on example.com. The fourth excludes targets with a hostname of www.google.com and the fifth excludes targets whose host resolves to 127.0.0.1.
+The first item will remove any target that doesn't contain a question mark, in other words any url that doesn't contain any GET parameters to test. The second attempts to avoid login functions, and the third blocklists all target urls on example.com. The fourth excludes targets with a hostname of www.google.com and the fifth excludes targets whose host resolves to 127.0.0.1.
 
-Indexer Modules
-===============
-### (general options) ###
-These options are applicable regardless of module chosen
+Prune
+=====
+The prune flag iterates through all targets, computes the fingerprints in memory, and marks subsequent matching targets as scanned. Additionally it deletes any target matching a blocklist item. The result is a database where --list-unscanned returns only scannable urls. It honors the **random** flag to compute fingerprints in random order.
 
-* source - label stored in source field for target, overrides label provided by module (if present and without a value during list operations, source field will be printed along with url)
+General Options
+===============
+These options are applicable regardless of module chosen:
+<pre>
+  --source [SOURCE]     Label associated with targets
+  --count COUNT         number of urls to scan, or -1 to scan all urls
+  --random              retrieve urls in random order
+</pre>
 
+Indexer Modules
+===============
 ### google ###
-Search for targets in a Google Custom Search Engine (CSE) via custom search element.
-
-Requirements: [PhantomJS](http://phantomjs.org/)
+<pre>
+  Searches google.com via scraping
 
-Options:
-* **engine** - CSE id
-* **query** - search query
-* phantomjs_dir - phantomjs base directory containing bin/phantomjs (default: tools/phantomjs/)
-* domain - limit searches to specified domain
+  --engine ENGINE       CSE id
+  --query QUERY         search query
+  --phantomjs-dir PHANTOMJS_DIR
+                        phantomjs base dir containing bin/phantomjs
+  --domain DOMAIN       limit searches to specified domain
+</pre>
 
 ### google_api ###
-Search for targets in a Google Custom Search Engine (CSE) via JSON API.
-
-Requirements: none
+<pre>
+  Searches google.com
 
-Options:
-* **key** - API key
-* **engine** - CSE id
-* **query** - search query
-* domain - limit searches to specified domain
+  --key KEY             API key
+  --engine ENGINE       CSE id
+  --query QUERY         search query
+  --domain DOMAIN       limit searches to specified domain
+</pre>
 
 ### pywb ###
-Search for targets within a pywb instance's indexed results.
-
-Requirements: none
+<pre>
+  Searches a given pywb server's crawl data
 
-Options:
-* **server** - pywb server url
-* **domain** - pull all results for given domain or subdomain
-* cdx_api_suffix - suffix after index for index api (default: /cdx)
-* index - search a specific index (default: first fixed index, or first dynamic index)
-* filter - query filter to apply to the search
-* retries - number of times to retry fetching results on error (default: 10)
-* threads - number concurrent requests to pywb server (default: 10)
+  --server SERVER       pywb server url
+  --domain DOMAIN       pull all results for given domain or subdomain
+  --cdx-api-suffix CDX_API_SUFFIX
+                        suffix after index for index api
+  --index INDEX         search a specific index
+  --filter FILTER       query filter to apply to the search
+  --retries RETRIES     number of times to retry fetching results on error
+  --threads THREADS     number of concurrent requests to wayback.org
+</pre>
 
 ### commoncrawl ###
-Search for targets within commoncrawl.org results.
-
-Requirements: none
+<pre>
+  Searches commoncrawl.org crawl data
 
-Options:
-* **domain** - pull all results for given domain or subdomain
-* index - search a specific index, e.g. CC-MAIN-2019-22 (default: latest)
-* filter - query filter to apply to the search
-* retries - number of times to retry fetching results on error (default: 10)
-* threads - number concurrent requests to commoncrawl.org (default: 10)
+  --domain DOMAIN       pull all results for given domain or subdomain
+  --index INDEX         search a specific index, e.g. CC-MAIN-2019-22 (default: latest)
+  --filter FILTER       query filter to apply to the search
+  --retries RETRIES     number of times to retry fetching results on error
+  --threads THREADS     number of concurrent requests to commoncrawl.org
+</pre>
 
 ### wayback ###
-Search for targets within archive.org results.
-
-Requirements: none
+<pre>
+  Searches archive.org crawl data
 
-Options:
-* **domain** - pull all results for given domain or subdomain
-* filter - query filter to apply to the search
-* from - beginning timestamp
-* to - end timestamp
+  --domain DOMAIN       pull all results for given domain or subdomain
+  --filter FILTER       query filter to apply to the search
+  --from FROM           beginning timestamp
+  --to TO               end timestamp
+  --retries RETRIES     number of times to retry fetching results on error
+  --threads THREADS     number of concurrent requests to wayback.org
+</pre>
 
 ### bing_api ###
-Search for targets via Bing Web Search API.
-
-Requirements: none
+<pre>
+  Searches bing.com
 
-Options:
-* **key** - API key
-* **query** - search query
+  --key KEY             API key
+  --query QUERY         search query
+</pre>
 
 ### stdin ###
-Read targets from standard input, one per line.
-
-Requirements: none
-
-Options: none
+<pre>
+  Accepts urls from stdin, one per line
+</pre>
 
 Scanner Modules
 ===============
-### (general options) ###
-These options are applicable regardless of module chosen
-
-* report_dir - directory to save vulnerability report (default: reports/)
-* label - friendly name field to include in vulnerability report
-* count - number of urls to scan, or -1 to scan all urls (default: -1)
-* random - scan urls in random order
-
 ### arachni ###
-Scan targets with Arachni command-line scanner.
-
-Requirements: [Arachni](http://www.arachni-scanner.com/)
+<pre>
+  Scans with the arachni command-line scanner
 
-Options:
-* arachni_dir - arachni base directory containing bin/arachni and bin/arachni_reporter (default: tools/arachni/)
-* args - space-delimited list of additional arguments, e.g. args="--http-user-agent Dorkbot/1.0 --timeout 00:15:00"
+  --arachni-dir ARACHNI_DIR
+                        arachni base dir containing bin/arachni and bin/arachni_reporter
+  --args ARGS           space-delimited list of additional arguments
+  --report-dir REPORT_DIR
+                        directory to save vulnerability report
+  --label LABEL         friendly name field to include in vulnerability report
+</pre>
 
 ### wapiti ###
-Scan targets with Wapiti command-line scanner.
-
-Requirements: [Wapiti](http://wapiti.sourceforge.net/)
-
-Options:
-* wapiti_dir - wapiti base directory containing bin/wapiti (default: tools/wapiti/)
-* args - space-delimited list of additional arguments
-
-Prune
-=====
-The prune flag iterates through all targets, computes the fingerprints in memory, and marks subsequent matching targets as scanned. Additionally it deletes any target matching a blacklist item. The result is a database where --list-unscanned returns only scannable urls. It honors (a subset of) the options specified in SCANNER_OPTIONS as follows:
+<pre>
+  Scans with the wapiti3 command-line scanner
 
-* random - evaluate urls in random order when computing fingerprints
+  --wapiti-dir WAPITI_DIR
+                        wapiti base dir containing bin/wapiti
+  --args ARGS           space-delimited list of additional arguments
+  --report-dir REPORT_DIR
+                        directory to save vulnerability report
+  --label LABEL         friendly name field to include in vulnerability report
+</pre>
```

### Comparing `dorkbot-0.3.1/dorkbot/dorkbot.py` & `dorkbot-0.4.0/dorkbot/dorkbot.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,73 +18,103 @@
 import sys
 from contextlib import closing
 from logging.handlers import WatchedFileHandler
 from urllib.parse import urlparse
 
 
 def main():
-    args, parser = get_args_parser()
+    args, parser = get_main_args_parser()
     initialize_logger(args.log, args.verbose)
-    indexer_options = parse_options(args.indexer_option)
-    scanner_options = parse_options(args.scanner_option)
 
     if args.directory and not os.path.isdir(args.directory):
         logging.debug("Creating directory - %s", args.directory)
         try:
             os.makedirs(args.directory)
         except OSError as e:
             logging.error("Failed to create directory - %s", str(e))
             sys.exit(1)
 
+    if args.help:
+        indexer_parser = None
+        if args.indexer:
+            indexer_parser, other_args = get_module_parser(load_module("indexers", args.indexer))
+            if not args.scanner:
+                indexer_parser.print_help()
+        if args.scanner:
+            scanner_parser, other_args = get_module_parser(load_module("scanners", args.scanner), parent_parser=indexer_parser)
+            scanner_parser.print_help()
+        if not args.indexer and not args.scanner:
+            parser.print_help()
+        sys.exit(0)
+
     if args.indexer or args.prune or args.scanner \
             or args.list_targets or args.flush_targets \
             or args.add_target or args.delete_target \
-            or args.list_blacklist or args.flush_blacklist \
-            or args.add_blacklist_item or args.delete_blacklist_item \
+            or args.list_blocklist or args.flush_blocklist \
+            or args.add_blocklist_item or args.delete_blocklist_item \
             or args.flush_fingerprints or args.list_unscanned:
 
         db = TargetDatabase(args.database)
-        if args.blacklist:
-            blacklist = Blacklist(args.blacklist)
+        if args.blocklist:
+            blocklist = Blocklist(args.blocklist)
         else:
             pattern = "^[^:]+://.*$"
             regex = re.compile(pattern)
             if (regex.match(args.database)):
-                blacklist = Blacklist(args.database)
+                blocklist = Blocklist(args.database)
             else:
-                blacklist = Blacklist("sqlite3://" + args.database)
+                blocklist = Blocklist("sqlite3://" + args.database)
+
+        if args.flush_blocklist: blocklist.flush()
+        if args.add_blocklist_item: blocklist.add(args.add_blocklist_item)
+        if args.delete_blocklist_item: blocklist.delete(args.delete_blocklist_item)
+        if args.list_blocklist:
+            for item in blocklist.get_parsed_items(): print(item)
 
-        if args.flush_targets: db.flush_targets()
-        if args.flush_blacklist: blacklist.flush()
         if args.flush_fingerprints: db.flush_fingerprints()
-        if args.add_target: db.add_target(args.add_target, indexer_options.get("source"))
+
+        if args.flush_targets: db.flush_targets()
+        if args.add_target: db.add_target(args.add_target, args.source)
         if args.delete_target: db.delete_target(args.delete_target)
-        if args.list_targets or args.list_unscanned:
-            try:
-                for url in db.get_urls(unscanned_only=args.list_unscanned, source=indexer_options.get("source")): print(url)
-            except BrokenPipeError:
-                devnull = os.open(os.devnull, os.O_WRONLY)
-                os.dup2(devnull, sys.stdout.fileno())
-                sys.exit(1)
         db.close()
 
-        if args.add_blacklist_item: blacklist.add(args.add_blacklist_item)
-        if args.delete_blacklist_item: blacklist.delete(args.delete_blacklist_item)
-        if args.list_blacklist:
-            for item in blacklist.get_parsed_items(): print(item)
-
         if args.indexer:
-            index(db, blacklist, load_module("indexers", args.indexer), args, indexer_options)
+            indexer_module = load_module("indexers", args.indexer)
+            indexer_parser, other_args = get_module_parser(indexer_module)
+            indexer_args = indexer_parser.parse_args(format_module_args(args.indexer_arg))
+            try:
+                index(db, blocklist, indexer_module, args, indexer_args)
+            except KeyboardInterrupt:
+                sys.exit(1)
 
         if args.prune:
-            prune(db, blacklist, args, scanner_options)
+            prune(db, blocklist, args)
 
         if args.scanner:
-            scan(db, blacklist, load_module("scanners", args.scanner), args, scanner_options)
+            scanner_module = load_module("scanners", args.scanner)
+            scanner_parser, other_args = get_module_parser(scanner_module)
+            scanner_args = scanner_parser.parse_args(format_module_args(args.scanner_arg))
+            try:
+                scan(db, blocklist, scanner_module, args, scanner_args)
+            except KeyboardInterrupt:
+                sys.exit(1)
 
+        db = TargetDatabase(args.database)
+        if args.list_targets or args.list_unscanned:
+            try:
+                urls = db.get_urls(unscanned_only=args.list_unscanned, source=args.source, randomize=args.random)
+                if args.count > 0:
+                    urls = urls[:args.count]
+                for url in urls:
+                    print(url)
+            except BrokenPipeError:
+                devnull = os.open(os.devnull, os.O_WRONLY)
+                os.dup2(devnull, sys.stdout.fileno())
+                sys.exit(1)
+        db.close()
     else:
         parser.print_usage()
 
     logging.shutdown()
 
 
 def initialize_logger(log_file, verbose):
@@ -116,55 +146,82 @@
     except ImportError:
         logging.error("Module not found")
         sys.exit(1)
 
     return module
 
 
-def get_args_parser():
+def get_initial_args_parser():
     config_dir = os.path.abspath(os.path.expanduser(
         os.environ.get("XDG_CONFIG_HOME") or
         os.environ.get("APPDATA") or
         os.path.join(os.environ["HOME"], ".config")
     ))
 
     initial_parser = argparse.ArgumentParser(
         description="dorkbot", add_help=False)
     initial_parser.add_argument("-c", "--config", \
                                 default=os.path.join(config_dir, "dorkbot", "dorkbot.ini"), \
                                 help="Configuration file")
     initial_parser.add_argument("-r", "--directory", \
                                 default=os.getcwd(), \
                                 help="Dorkbot directory (default location of db, tools, reports)")
+    initial_parser.add_argument("--source", nargs="?", const=True, default=False, \
+                                help="Label associated with targets")
+    initial_parser.add_argument("--show-defaults", action="store_true", \
+                                help="Show default values in help output")
+    global_scanner_options = initial_parser.add_argument_group("global scanner options")
+    global_scanner_options.add_argument("--count", type=int, default=-1, \
+                          help="number of urls to scan, or -1 to scan all urls")
+    global_scanner_options.add_argument("--random", action="store_true", \
+                          help="retrieve urls in random order")
     initial_args, other_args = initial_parser.parse_known_args()
 
+    return initial_args, other_args, initial_parser
+
+
+def get_main_args_parser():
+    initial_args, other_args, initial_parser = get_initial_args_parser()
+
     defaults = {
         "database": os.path.join(initial_args.directory, "dorkbot.db"),
     }
 
     if os.path.isfile(initial_args.config):
-        config = configparser.SafeConfigParser()
+        config = configparser.ConfigParser()
         config.read(initial_args.config)
-        options = config.items("dorkbot")
-        defaults.update(dict(options))
+        try:
+            config_items = config.items("dorkbot")
+            defaults.update(dict(config_items))
+        except KeyError:
+            pass
+        except configparser.NoSectionError as e:
+            logging.debug(e)
+
+    if initial_args.show_defaults:
+        parser = argparse.ArgumentParser(parents=[initial_parser], add_help=False, \
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    else:
+        parser = argparse.ArgumentParser(parents=[initial_parser], add_help=False)
 
-    parser = argparse.ArgumentParser(parents=[initial_parser])
     parser.set_defaults(**defaults)
+    parser.add_argument("-h", "--help", action="store_true", \
+                        help="Show program (or specified module) help")
     parser.add_argument("--log", \
                         help="Path to log file")
     parser.add_argument("-v", "--verbose", action="store_true", \
                         help="Enable verbose logging (DEBUG output)")
     parser.add_argument("-V", "--version", action="version", \
                         version="%(prog)s " + __version__, help="Print version")
 
     database = parser.add_argument_group('database')
     database.add_argument("-d", "--database", \
                           help="Database file/uri")
     database.add_argument("-u", "--prune", action="store_true", \
-                          help="Apply fingerprinting and blacklist without scanning")
+                          help="Apply fingerprinting and blocklist without scanning")
 
     targets = parser.add_argument_group('targets')
     targets.add_argument("-l", "--list-targets", action="store_true", \
                          help="List targets in database")
     targets.add_argument("--list-unscanned", action="store_true", \
                          help="List unscanned targets in database")
     targets.add_argument("--add-target", metavar="TARGET", \
@@ -173,111 +230,160 @@
                          help="Delete a url from the target database")
     targets.add_argument("--flush-targets", action="store_true", \
                          help="Delete all targets")
 
     indexing = parser.add_argument_group('indexing')
     indexing.add_argument("-i", "--indexer", \
                           help="Indexer module to use")
-    indexing.add_argument("-o", "--indexer-option", action="append", \
-                          help="Pass an option to the indexer (can be used multiple times)")
+    indexing.add_argument("-o", "--indexer-arg", action="append", \
+                          help="Pass an argument to the indexer module (can be used multiple times)")
 
     scanning = parser.add_argument_group('scanning')
     scanning.add_argument("-s", "--scanner", \
                           help="Scanner module to use")
-    scanning.add_argument("-p", "--scanner-option", action="append", \
-                          help="Pass an option to the scanner (can be used multiple times)")
+    scanning.add_argument("-p", "--scanner-arg", action="append", \
+                          help="Pass an argument to the scanner module (can be used multiple times)")
 
     fingerprints = parser.add_argument_group('fingerprints')
     fingerprints.add_argument("-f", "--flush-fingerprints", action="store_true", \
                               help="Delete all fingerprints of previously-scanned items")
 
-    blacklist = parser.add_argument_group('blacklist')
-    blacklist.add_argument("-b", "--blacklist", \
-                           help="Blacklist file/uri")
-    blacklist.add_argument("--list-blacklist", action="store_true", \
-                           help="List blacklist entries")
-    blacklist.add_argument("--add-blacklist-item", metavar="ITEM", \
-                           help="Add an ip/host/regex pattern to the blacklist")
-    blacklist.add_argument("--delete-blacklist-item", metavar="ITEM", \
-                           help="Delete an item from the blacklist")
-    blacklist.add_argument("--flush-blacklist", action="store_true", \
-                           help="Delete all blacklist items")
+    blocklist = parser.add_argument_group('blocklist')
+    blocklist.add_argument("-b", "--blocklist", \
+                           help="Blocklist file/uri")
+    blocklist.add_argument("--list-blocklist", action="store_true", \
+                           help="List blocklist entries")
+    blocklist.add_argument("--add-blocklist-item", metavar="ITEM", \
+                           help="Add an ip/host/regex pattern to the blocklist")
+    blocklist.add_argument("--delete-blocklist-item", metavar="ITEM", \
+                           help="Delete an item from the blocklist")
+    blocklist.add_argument("--flush-blocklist", action="store_true", \
+                           help="Delete all blocklist items")
 
-    args = parser.parse_args(other_args)
-    args.directory = initial_args.directory
+    args = parser.parse_args(other_args, namespace=initial_args)
     return args, parser
 
 
-def index(db, blacklist, indexer, args, options):
+def get_module_parser(module, parent_parser=None):
+    initial_args, other_args, initial_parser = get_initial_args_parser()
+
+    defaults = {}
+    module_defaults = {}
+
+    if os.path.isfile(initial_args.config):
+        config = configparser.ConfigParser()
+        config.read(initial_args.config)
+
+        try:
+            config_items = config.items("dorkbot")
+            defaults.update(dict(config_items))
+        except KeyError:
+            pass
+        except configparser.NoSectionError as e:
+            logging.debug(e)
+
+        try:
+            module_config_items = config.items(module.__name__)
+            module_defaults.update(dict(module_config_items))
+        except KeyError:
+            pass
+        except configparser.NoSectionError as e:
+            logging.debug(e)
+
+    if parent_parser:
+        initial_parser = parent_parser
+
+    usage="%(prog)s [args] -i/-s [module] -o/-p [module_arg[=value]] ..."
+    epilog="NOTE: module args are passed via -o/-p as key=value and do not themselves require hyphens"
+
+    if initial_args.show_defaults:
+        parser = argparse.ArgumentParser(parents=[initial_parser], usage=usage, epilog=epilog, add_help=False, \
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    else:
+        parser = argparse.ArgumentParser(parents=[initial_parser], usage=usage, epilog=epilog, add_help=False)
+
+    parser.set_defaults(**defaults)
+    module.populate_parser(initial_args, parser)
+    parser.set_defaults(**module_defaults)
+
+    return parser, other_args
+
+
+def format_module_args(args_list):
+    args = []
+
+    if args_list:
+        for arg in args_list:
+            if arg.startswith("--"):
+                args.add(arg)
+            else:
+                args.append("--" + arg)
+
+    return args
+
+
+def index(db, blocklist, indexer, args, indexer_args):
     indexer_name = indexer.__name__.split(".")[-1]
-    indexer_options = ",".join(["%s=%s" % (key, val) for key, val in options.items()])
-    logging.info("Indexing: %s %s", indexer_name, indexer_options)
-    options["directory"] = args.directory
-    urls, module_source = indexer.run(options)
-    source = options.get("source", module_source)
+    logging.info("Indexing: %s %s", indexer_name, vars(indexer_args))
+    setattr(indexer_args, "directory", args.directory)
+    urls, module_source = indexer.run(indexer_args)
+    if args.source:
+        source = args.source
+    else:
+        source = module_source
 
     targets = []
     for url in urls:
-        if not blacklist.match(Target(url)): targets.append(url)
+        if not blocklist.match(Target(url)): targets.append(url)
 
     db.connect()
     db.add_targets(targets, source)
     db.close()
 
 
-def prune(db, blacklist, args, options):
-    if "random" in options:
-        randomize = True
-    else:
-        randomize = False
-
+def prune(db, blocklist, args):
     logging.info("Pruning database")
 
     db.connect()
-    db.prune(blacklist, randomize)
+    db.prune(blocklist, args.random)
     db.close()
 
 
-def scan(db, blacklist, scanner, args, options):
-    options["directory"] = args.directory
-    report_dir = options.get("reports", os.path.join(args.directory, "reports"))
-    if not os.path.isdir(report_dir):
+def scan(db, blocklist, scanner, args, scanner_args):
+    if not os.path.isdir(scanner_args.report_dir):
         try:
-            os.makedirs(report_dir)
+            os.makedirs(scanner_args.report_dir)
         except OSError as e:
             logging.error("Failed to create report directory - %s", str(e))
             sys.exit(1)
 
-    count = int(options.get("count", "-1"))
-    label = options.get("label", "")
-
     scanned = 0
-    while scanned < count or count == -1:
+    while scanned < args.count or args.count == -1:
         db.connect()
-        target = db.get_next_target(random=options.get("random", False))
+        target = db.get_next_target(random=args.random)
         if not target:
             break
 
-        if blacklist.match(target):
-            logging.debug("Deleting (matches blacklist pattern): %s", target.url)
+        if blocklist.match(target):
+            logging.debug("Deleting (matches blocklist pattern): %s", target.url)
             db.delete_target(target.url)
             continue
 
         db.close()
 
         logging.info("Scanning: %s", target.url)
-        results = scanner.run(options, target)
+        results = scanner.run(scanner_args, target)
         scanned += 1
 
         if results == False:
             logging.error("Scan failed: %s", target.url)
             continue
 
         target.endtime = generate_timestamp()
-        target.write_report(report_dir, label, results)
+        target.write_report(scanner_args.report_dir, scanner_args.label, results)
 
 
 def generate_fingerprint(target):
     url_parts = urlparse(target.url)
     netloc = url_parts.netloc
     depth = str(url_parts.path.count("/"))
     page = url_parts.path.split("/")[-1]
@@ -294,28 +400,14 @@
     return datetime.datetime.now().astimezone().isoformat()
 
 
 def generate_hash(url):
     return hashlib.md5(url.encode("utf-8")).hexdigest()
 
 
-def parse_options(options_list):
-    options = dict()
-
-    if options_list:
-        for option in options_list:
-            if "=" in option:
-                key, value = option.split("=", 1)
-            else:
-                key, value = option, True
-            options.update({key: value})
-
-    return options
-
-
 class TargetDatabase:
     def __init__(self, database):
         self.connect_kwargs = {}
         if database.startswith("postgresql://"):
             self.database = database
             module_name = "psycopg2"
             self.insert = "INSERT"
@@ -355,30 +447,30 @@
                     sys.exit(1)
 
         self.connect()
         try:
             with self.db, closing(self.db.cursor()) as c:
                 c.execute("CREATE TABLE IF NOT EXISTS targets (url VARCHAR PRIMARY KEY, source VARCHAR, scanned INTEGER DEFAULT 0)")
                 c.execute("CREATE TABLE IF NOT EXISTS fingerprints (fingerprint VARCHAR PRIMARY KEY)")
-                c.execute("CREATE TABLE IF NOT EXISTS blacklist (item VARCHAR PRIMARY KEY)")
+                c.execute("CREATE TABLE IF NOT EXISTS blocklist (item VARCHAR PRIMARY KEY)")
         except self.module.Error as e:
             logging.error("Failed to load database - %s", str(e))
             sys.exit(1)
 
     def connect(self):
         try:
             self.db = self.module.connect(self.database, **self.connect_kwargs)
         except self.module.Error as e:
             logging.error("Error loading database - %s", str(e))
             sys.exit(1)
 
     def close(self):
         self.db.close()
 
-    def get_urls(self, unscanned_only=False, source=False):
+    def get_urls(self, unscanned_only=False, source=False, randomize=False):
         fields = "url"
         if source is True:
             fields += ",source"
 
         sql = f"SELECT {fields} FROM targets"
         if unscanned_only:
             sql += " WHERE scanned != 1"
@@ -395,14 +487,17 @@
                 else:
                     c.execute(sql)
                 urls = [" | ".join(row) for row in c.fetchall()]
         except self.module.Error as e:
             logging.error("Failed to get targets - %s", str(e))
             sys.exit(1)
 
+        if randomize:
+            random.shuffle(urls)
+
         return urls
 
     def get_next_target(self, random=False):
         sql = "SELECT url FROM targets WHERE scanned != 1"
         if random:
             sql += " ORDER BY RANDOM()"
 
@@ -503,15 +598,15 @@
         try:
             with self.db, closing(self.db.cursor()) as c:
                 c.execute("DELETE FROM targets")
         except self.module.Error as e:
             logging.error("Failed to flush targets - %s", str(e))
             sys.exit(1)
 
-    def prune(self, blacklist, randomize=False):
+    def prune(self, blocklist, randomize=False):
         fingerprints = set()
 
         urls = self.get_urls()
 
         if randomize:
             random.shuffle(urls)
 
@@ -521,16 +616,16 @@
             fingerprint = generate_fingerprint(target)
             with self.db, closing(self.db.cursor()) as c:
                 if fingerprint in fingerprints or self.get_scanned(fingerprint, c):
                     logging.debug("Marking scanned (matches fingerprint of another target): %s", target.url)
                     self.mark_scanned(target.url, c)
                     continue
 
-            if blacklist.match(target):
-                logging.debug("Deleting (matches blacklist pattern): %s", target.url)
+            if blocklist.match(target):
+                logging.debug("Deleting (matches blocklist pattern): %s", target.url)
                 self.delete_target(target.url)
                 continue
 
             fingerprints.add(fingerprint)
 
 
 class Target:
@@ -567,106 +662,106 @@
         filename = os.path.join(report_dir, self.get_hash() + ".json")
 
         with open(filename, "w") as outfile:
             json.dump(vulns, outfile, indent=4, sort_keys=True)
             print("Report saved to: %s" % outfile.name)
 
 
-class Blacklist:
-    def __init__(self, blacklist):
+class Blocklist:
+    def __init__(self, blocklist):
         self.connect_kwargs = {}
         self.ip_set = set()
         self.host_set = set()
         self.regex_set = set()
 
-        if blacklist.startswith("postgresql://"):
-            self.database = blacklist
+        if blocklist.startswith("postgresql://"):
+            self.database = blocklist
             module_name = "psycopg2"
             self.insert = "INSERT"
             self.conflict = "ON CONFLICT DO NOTHING"
-        elif blacklist.startswith("phoenixdb://"):
-            self.database = blacklist[12:]
+        elif blocklist.startswith("phoenixdb://"):
+            self.database = blocklist[12:]
             module_name = "phoenixdb"
             self.insert = "UPSERT"
             self.conflict = ""
             self.connect_kwargs["autocommit"] = True
-        elif blacklist.startswith("sqlite3://"):
-            self.database = os.path.expanduser(blacklist[10:])
+        elif blocklist.startswith("sqlite3://"):
+            self.database = os.path.expanduser(blocklist[10:])
             module_name = "sqlite3"
             database_dir = os.path.dirname(self.database)
             self.insert = "INSERT OR REPLACE"
             self.conflict = ""
             if database_dir and not os.path.isdir(database_dir):
                 try:
                     os.makedirs(database_dir)
                 except OSError as e:
                     logging.error("Failed to create directory - %s", str(e))
                     sys.exit(1)
         else:
             self.database = False
-            self.filename = blacklist
+            self.filename = blocklist
             try:
-                self.blacklist_file = open(self.filename, "r")
+                self.blocklist_file = open(self.filename, "r")
             except Exception as e:
-                logging.error("Failed to read blacklist file - %s", str(e))
+                logging.error("Failed to read blocklist file - %s", str(e))
                 sys.exit(1)
 
         if self.database:
             self.module = importlib.import_module(module_name, package=None)
 
             if self.module.paramstyle == "qmark":
                 self.param = "?"
             else:
                 self.param = "%s"
 
             self.connect()
             try:
                 with self.db, closing(self.db.cursor()) as c:
-                    c.execute("CREATE TABLE IF NOT EXISTS blacklist (item VARCHAR PRIMARY KEY)")
+                    c.execute("CREATE TABLE IF NOT EXISTS blocklist (item VARCHAR PRIMARY KEY)")
             except self.module.Error as e:
-                logging.error("Failed to load blacklist database - %s", str(e))
+                logging.error("Failed to load blocklist database - %s", str(e))
                 sys.exit(1)
 
         self.parse_list(self.read_items())
 
     def connect(self):
         if self.database:
             try:
                 self.db = self.module.connect(self.database, **self.connect_kwargs)
             except self.module.Error as e:
                 logging.error("Error loading database - %s", str(e))
                 sys.exit(1)
         else:
             try:
-                self.blacklist_file = open(self.filename, "a")
+                self.blocklist_file = open(self.filename, "a")
             except Exception as e:
-                logging.error("Failed to read blacklist file - %s", str(e))
+                logging.error("Failed to read blocklist file - %s", str(e))
                 sys.exit(1)
 
     def close(self):
         if self.database:
             self.db.close()
         else:
-            self.blacklist_file.close()
+            self.blocklist_file.close()
 
     def parse_list(self, items):
         for item in items:
             if item.startswith("ip:"):
                 ip = item.split(":")[1]
                 try:
                     ip_net = ipaddress.ip_network(ip)
                 except ValueError as e:
-                    logging.error("Could not parse blacklist item as ip - %s", str(e))
+                    logging.error("Could not parse blocklist item as ip - %s", str(e))
                 self.ip_set.add(ip_net)
             elif item.startswith("host:"):
                 self.host_set.add(item.split(":")[1])
             elif item.startswith("regex:"):
                 self.regex_set.add(item.split(":")[1])
             else:
-                logging.warning("Could not parse blacklist item - %s", item)
+                logging.warning("Could not parse blocklist item - %s", item)
 
         pattern = "|".join(self.regex_set)
         if pattern:
             self.regex = re.compile(pattern)
         else:
             self.regex = None
 
@@ -682,67 +777,67 @@
                ["host:" + item for item in self.host_set] + \
                ["regex:" + item for item in self.regex_set]
 
     def read_items(self):
         if self.database:
             try:
                 with self.db, closing(self.db.cursor()) as c:
-                    c.execute("SELECT item FROM blacklist")
+                    c.execute("SELECT item FROM blocklist")
                     items = [row[0] for row in c.fetchall()]
             except self.module.Error as e:
                 logging.error("Failed to get targets - %s", str(e))
                 sys.exit(1)
         else:
-            items = self.blacklist_file.read().splitlines()
+            items = self.blocklist_file.read().splitlines()
 
         return items
 
     def add(self, item):
         self.connect()
 
         if item.startswith("ip:"):
             ip = item.split(":")[1]
             try:
                 ip_net = ipaddress.ip_network(ip)
             except ValueError as e:
-                logging.error("Could not parse blacklist item as ip - %s", str(e))
+                logging.error("Could not parse blocklist item as ip - %s", str(e))
                 sys.exit(1)
             self.ip_set.add(ip_net)
         elif item.startswith("host:"):
             self.host_set.add(item.split(":")[1])
         elif item.startswith("regex:"):
             self.regex_set.add(item.split(":")[1])
         else:
-            logging.error("Could not parse blacklist item - %s", item)
+            logging.error("Could not parse blocklist item - %s", item)
             sys.exit(1)
 
         if self.database:
             try:
                 with self.db, closing(self.db.cursor()) as c:
-                    c.execute("%s INTO blacklist VALUES (%s)" % (self.insert, self.param), (item,))
+                    c.execute("%s INTO blocklist VALUES (%s)" % (self.insert, self.param), (item,))
             except self.module.Error as e:
-                logging.error("Failed to add blacklist item - %s", str(e))
+                logging.error("Failed to add blocklist item - %s", str(e))
                 sys.exit(1)
         else:
-            logging.warning("Add ignored (not implemented for file-based blacklist)")
+            logging.warning("Add ignored (not implemented for file-based blocklist)")
 
         self.close()
 
     def delete(self, item):
         self.connect()
 
         if self.database:
             try:
                 with self.db, closing(self.db.cursor()) as c:
-                    c.execute("DELETE FROM blacklist WHERE item=(%s)" % self.param, (item,))
+                    c.execute("DELETE FROM blocklist WHERE item=(%s)" % self.param, (item,))
             except self.module.Error as e:
-                logging.error("Failed to delete blacklist item - %s", str(e))
+                logging.error("Failed to delete blocklist item - %s", str(e))
                 sys.exit(1)
         else:
-            logging.warning("Delete ignored (not implemented for file-based blacklist)")
+            logging.warning("Delete ignored (not implemented for file-based blocklist)")
 
         self.close()
 
     def match(self, target):
         if self.regex and self.regex.match(target.url):
             return True
 
@@ -752,27 +847,27 @@
         for ip_net in self.ip_set:
             if target.ip and target.ip in ip_net:
                 return True
 
         return False
 
     def flush(self):
-        logging.info("Flushing blacklist")
+        logging.info("Flushing blocklist")
         if self.database:
             try:
                 with self.db, closing(self.db.cursor()) as c:
-                    c.execute("DELETE FROM blacklist")
+                    c.execute("DELETE FROM blocklist")
             except self.module.Error as e:
-                logging.error("Failed to flush blacklist - %s", str(e))
+                logging.error("Failed to flush blocklist - %s", str(e))
                 sys.exit(1)
         else:
             try:
                 os.unlink(self.filename)
             except OSError as e:
-                logging.error("Failed to delete blacklist file - %s", str(e))
+                logging.error("Failed to delete blocklist file - %s", str(e))
                 sys.exit(1)
 
         self.regex = None
         self.regex_set = set()
         self.ip_set = set()
         self.host_set = set()
```

### Comparing `dorkbot-0.3.1/dorkbot/indexers/commoncrawl.py` & `dorkbot-0.4.0/dorkbot/indexers/commoncrawl.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,52 @@
+import argparse
 import json
 import logging
 import random
 import re
 import sys
 import time
 from concurrent.futures import ThreadPoolExecutor
 from http.client import IncompleteRead
 from itertools import repeat
 from urllib.error import HTTPError
 from urllib.parse import urlencode, urlparse
 from urllib.request import urlopen
 
 
-def run(options):
-    required = ["domain"]
-    for r in required:
-        if r not in options:
-            logging.error("%s must be set", r)
-            sys.exit(1)
+def populate_parser(args, parser):
+    module_group = parser.add_argument_group(__name__, "Searches commoncrawl.org crawl data")
+    module_group.add_argument("--domain", required=True, \
+                          help="pull all results for given domain or subdomain")
+    module_group.add_argument("--index", \
+                          help="search a specific index, e.g. CC-MAIN-2019-22 (default: latest)")
+    module_group.add_argument("--filter", \
+                          help="query filter to apply to the search")
+    module_group.add_argument("--retries", type=int, default=10, \
+                          help="number of times to retry fetching results on error")
+    module_group.add_argument("--threads", type=int, default=1, \
+                          help="number of concurrent requests to commoncrawl.org")
 
-    source = __name__.split(".")[-1]
-
-    retries = int(options.get("retries", "10"))
-    threads = int(options.get("threads", "10"))
-    domain = options["domain"]
-    index = options.get("index", "")
-    url_filter = options.get("filter", "")
 
+def run(args):
+    source = __name__.split(".")[-1]
     data = {}
-    data["url"] = "*.%s" % domain
+    data["url"] = "*.%s" % args.domain
     data["fl"] = "url"
     data["output"] = "json"
-    if url_filter:
-        data["filter"] = url_filter
+    if args.filter:
+        data["filter"] = args.filter
 
-    if not index:
-        index = get_latest_index(retries)
-    num_pages = get_num_pages(index, data, retries)
+    if not args.index:
+        args.index = get_latest_index(int(args.retries))
+    num_pages = get_num_pages(args.index, data, int(args.retries))
 
-    source += f",index:{index}"
+    source += f",index:{args.index}"
 
-    results = get_results(domain, index, data, num_pages, threads, retries)
+    results = get_results(args.domain, args.index, data, num_pages, args.threads, args.retries)
     for result in results:
         logging.debug(result)
     logging.info("Fetched %d results", len(results))
     return results, source
 
 
 def get_latest_index(retries):
```

### Comparing `dorkbot-0.3.1/dorkbot/indexers/google.js` & `dorkbot-0.4.0/dorkbot/indexers/google.js`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.1/dorkbot/indexers/google_api.py` & `dorkbot-0.4.0/dorkbot/indexers/google_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,45 @@
+import argparse
 import json
 import logging
 import sys
 import time
 from urllib.error import HTTPError
 from urllib.parse import urlencode, urlparse
 from urllib.request import urlopen
 
 
-def run(options):
-    required = ["key", "engine", "query"]
-    for r in required:
-        if r not in options:
-            logging.error("%s must be set", r)
-            sys.exit(1)
+def populate_parser(args, parser):
+    module_group = parser.add_argument_group(__name__, "Searches google.com")
+    module_group.add_argument("--key", required=True, \
+                          help="API key")
+    module_group.add_argument("--engine", required=True, \
+                          help="CSE id")
+    module_group.add_argument("--query", required=True, \
+                          help="search query")
+    module_group.add_argument("--domain", \
+                          help="limit searches to specified domain")
 
-    source = __name__.split(".")[-1]
 
-    results = get_results(options)
+def run(args):
+    source = __name__.split(".")[-1]
+    results = get_results(args.key, args.engine, args.query, args.domain)
     return results, source
 
 
-def get_results(options):
+def get_results(key, engine, query, domain):
     data = {}
-    data["key"] = options["key"]
-    data["cx"] = options["engine"]
-    data["q"] = options["query"]
+    data["key"] = key
+    data["cx"] = engine
+    data["q"] = query
     data["num"] = 10
     data["start"] = 0
 
-    if "domain" in options:
-        data["siteSearch"] = options["domain"]
+    if domain:
+        data["siteSearch"] = domain
 
     results = []
     while True:
         items = issue_request(data)
         data["start"] += data["num"]
         if not items:
             break
```

### Comparing `dorkbot-0.3.1/dorkbot/indexers/pywb.py` & `dorkbot-0.4.0/dorkbot/indexers/pywb.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,53 +1,56 @@
+import argparse
 import json
 import logging
 import random
 import re
 import sys
 import time
 from concurrent.futures import ThreadPoolExecutor
 from http.client import IncompleteRead
 from itertools import repeat
 from urllib.error import HTTPError
 from urllib.parse import urlencode, urlparse
 from urllib.request import urlopen
 
 
-def run(options):
-    required = ["server", "domain"]
-    for r in required:
-        if r not in options:
-            logging.error("%s must be set", r)
-            sys.exit(1)
+def populate_parser(args, parser):
+    module_group = parser.add_argument_group(__name__, "Searches a given pywb server's crawl data")
+    module_group.add_argument("--server", required=True, \
+                          help="pywb server url")
+    module_group.add_argument("--domain", required=True, \
+                          help="pull all results for given domain or subdomain")
+    module_group.add_argument("--cdx-api-suffix", default="/cdx", \
+                          help="suffix after index for index api")
+    module_group.add_argument("--index", \
+                          help="search a specific index")
+    module_group.add_argument("--filter", \
+                          help="query filter to apply to the search")
+    module_group.add_argument("--retries", type=int, default=10, \
+                          help="number of times to retry fetching results on error")
+    module_group.add_argument("--threads", type=int, default=1, \
+                          help="number of concurrent requests to wayback.org")
 
-    source = __name__.split(".")[-1]
-
-    retries = int(options.get("retries", "10"))
-    threads = int(options.get("threads", "10"))
-    server = options["server"]
-    domain = options["domain"]
-    index = options.get("index", "")
-    url_filter = options.get("filter", "")
-    cdx_api_suffix = options.get("cdx_api_suffix", "/cdx")
 
+def run(args):
+    source = __name__.split(".")[-1]
     data = {}
-    data["url"] = "*.%s" % domain
-    data["fl"] = "url"
+    data["url"] = "*.%s" % args.domain
     data["output"] = "json"
-    if url_filter:
-        data["filter"] = url_filter
+    if args.filter:
+        data["filter"] = args.filter
 
-    if not index:
-        index = get_latest_index(server, retries)
-    base_url = f"{server}/{index}{cdx_api_suffix}"
-    num_pages = get_num_pages(base_url, data, retries)
+    if not args.index:
+        index = get_latest_index(args.server, int(args.retries))
+    base_url = f"{args.server}/{args.index}{args.cdx_api_suffix}"
+    num_pages = get_num_pages(base_url, data, int(args.retries))
 
-    source += f",index:{index}"
+    source += f",index:{args.index}"
 
-    results = get_results(base_url, data, retries, num_pages, threads, domain)
+    results = get_results(base_url, data, args.retries, num_pages, args.threads, args.domain)
     for result in results:
         logging.debug(result)
     logging.info("Fetched %d results", len(results))
     return results, source
 
 
 def get_latest_index(server, retries):
```

### Comparing `dorkbot-0.3.1/dorkbot/indexers/wayback.py` & `dorkbot-0.4.0/dorkbot/indexers/wayback.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,56 @@
+import argparse
 import json
 import logging
 import random
 import re
 import sys
 import time
 from concurrent.futures import ThreadPoolExecutor
 from http.client import IncompleteRead
 from itertools import repeat
 from urllib.error import HTTPError
 from urllib.parse import urlencode, urlparse
 from urllib.request import urlopen
 
 
-def run(options):
-    required = ["domain"]
-    for r in required:
-        if r not in options:
-            logging.error("%s must be set", r)
-            sys.exit(1)
+def populate_parser(args, parser):
+    module_group = parser.add_argument_group(__name__, "Searches archive.org crawl data")
+    module_group.add_argument("--domain", required=True, \
+                          help="pull all results for given domain or subdomain")
+    module_group.add_argument("--filter", \
+                          help="query filter to apply to the search")
+    module_group.add_argument("--from", dest="from_", metavar="FROM", \
+                          help="beginning timestamp")
+    module_group.add_argument("--to", \
+                          help="end timestamp")
+    module_group.add_argument("--retries", type=int, default=10, \
+                          help="number of times to retry fetching results on error")
+    module_group.add_argument("--threads", type=int, default=1, \
+                          help="number of concurrent requests to wayback.org")
 
-    source = __name__.split(".")[-1]
-
-    retries = int(options.get("retries", "10"))
-    threads = int(options.get("threads", "1"))
-    domain = options["domain"]
-    time_from = options.get("from", "")
-    time_to = options.get("to", "")
-    url_filter = options.get("filter", "")
 
+def run(args):
+    source = __name__.split(".")[-1]
     data = {}
-    data["url"] = "*.%s" % domain
+    data["url"] = "*.%s" % args.domain
     data["fl"] = "original"
     data["output"] = "json"
-    if url_filter:
-        data["filter"] = url_filter
-    if time_from:
-        data["from"] = time_from
-        source += f",from:{time_from}"
-    if time_to:
-        data["to"] = time_to
-        source += f",to:{time_to}"
+    if args.filter:
+        data["filter"] = args.filter
+    if args.from_:
+        data["from"] = args.from_
+        source += f",from:{args.from_}"
+    if args.to:
+        data["to"] = args.to
+        source += f",to:{args.to}"
 
-    num_pages = get_num_pages(data, retries)
+    num_pages = get_num_pages(data, int(args.retries))
 
-    results = get_results(domain, data, num_pages, threads, retries)
+    results = get_results(args.domain, data, num_pages, args.threads, args.retries)
     for result in results:
         logging.debug(result)
     logging.info("Fetched %d results", len(results))
     return results, source
 
 
 def get_num_pages(data, retries):
```

### Comparing `dorkbot-0.3.1/dorkbot/scanners/arachni.py` & `dorkbot-0.4.0/dorkbot/scanners/arachni.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,49 @@
+import argparse
 import io
 import json
 import logging
 import os
 import platform
 import subprocess
 import sys
 import tempfile
 
 
-def run(options, target):
-    default_arachni_path = os.path.join(options["directory"], "tools", "arachni", "bin")
-    if not os.path.isdir(default_arachni_path): default_arachni_path = ""
+def populate_parser(args, parser):
+    module_group = parser.add_argument_group(__name__, "Scans with the arachni command-line scanner")
+    module_group.add_argument("--arachni-dir", default=os.path.join(args.directory, "tools", "arachni"), \
+                          help="arachni base dir containing bin/arachni and bin/arachni_reporter")
+    module_group.add_argument("--args", \
+                          help="space-delimited list of additional arguments")
+    module_group.add_argument("--report-dir", default=os.path.join(args.directory, "reports"), \
+                          help="directory to save vulnerability report")
+    module_group.add_argument("--label", default="", \
+                          help="friendly name field to include in vulnerability report")
 
-    if "arachni_dir" in options:
-        arachni_path = os.path.join(os.path.abspath(options["arachni_dir"]), "bin")
+
+def run(args, target):
+    if not os.path.isdir(args.arachni_dir): args.arachni_dir = ""
+
+    if args.arachni_dir:
+        arachni_path = os.path.join(os.path.abspath(args.arachni_dir), "bin")
     else:
-        arachni_path = default_arachni_path
+        arachni_path = args.arachni_dir
 
     report = os.path.join(tempfile.gettempdir(), target.get_hash() + ".afr")
 
     scan_cmd = [os.path.join(arachni_path, "arachni")]
     if platform.system() == "Windows":
         scan_cmd[0] = scan_cmd[0] + ".bat"
     scan_cmd += ["--report-save-path", report]
     scan_cmd += ["--output-only-positives"]
     scan_cmd += ["--scope-page-limit", "1"]
     scan_cmd += ["--scope-include-pattern", target.url.split("?", 1)[0]]
-    if "args" in options:
-        scan_cmd += options["args"].split()
+    if args.args:
+        scan_cmd += args.args.split()
     scan_cmd += [target.url]
 
     report_cmd = [os.path.join(arachni_path, "arachni_reporter")]
     if platform.system() == "Windows":
         report_cmd[0] = report_cmd[0] + ".bat"
     report_cmd += ["--reporter", "json:outfile=" + report + ".json"]
     report_cmd += [report]
```

### Comparing `dorkbot-0.3.1/dorkbot/scanners/wapiti.py` & `dorkbot-0.4.0/dorkbot/scanners/wapiti.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,51 @@
+import argparse
 import io
 import json
 import logging
 import os
 import platform
 import subprocess
 import sys
 import tempfile
 from urllib.parse import urlparse, urlunparse, urljoin
 
 
-def run(options, target):
-    default_wapiti_path = os.path.join(options["directory"], "tools", "wapiti", "bin")
-    if not os.path.isdir(default_wapiti_path): default_wapiti_path = ""
+def populate_parser(args, parser):
+    module_group = parser.add_argument_group(__name__, "Scans with the wapiti3 command-line scanner")
+    module_group.add_argument("--wapiti-dir", default=os.path.join(args.directory, "tools", "wapiti"), \
+                          help="wapiti base dir containing bin/wapiti")
+    module_group.add_argument("--args", \
+                          help="space-delimited list of additional arguments")
+    module_group.add_argument("--report-dir", default=os.path.join(args.directory, "reports"),\
+                          help="directory to save vulnerability report")
+    module_group.add_argument("--label", default="", \
+                          help="friendly name field to include in vulnerability report")
 
-    if "wapiti_dir" in options:
-        wapiti_path = os.path.join(os.path.abspath(options["wapiti_dir"]), "bin")
+
+def run(args, target):
+    if not os.path.isdir(args.wapiti_dir): args.wapiti_dir = ""
+
+    if args.wapiti_dir:
+        wapiti_path = os.path.join(os.path.abspath(args.wapiti_dir), "bin")
     else:
-        wapiti_path = default_wapiti_path
+        wapiti_path = args.wapiti_dir
 
     report = os.path.join(tempfile.gettempdir(), target.get_hash() + ".json")
 
     cmd = [os.path.join(wapiti_path, "wapiti")]
     if platform.system() == "Windows" and wapiti_path != "":
         cmd.insert(0, sys.executable)
     cmd += ["--url", target.url]
     cmd += ["--scope", "page"]
     cmd += ["--flush-session"]
     cmd += ["--format", "json"]
     cmd += ["--output", report]
-    if "args" in options:
-        cmd += options["args"].split()
+    if args.args:
+        cmd += args.args.split()
 
     try:
         subprocess.run(cmd, check=True)
     except OSError as e:
         if "No such file or directory" in str(e) or "The system cannot find the file specified" in str(e):
             logging.critical(
                 "Could not find wapiti. If not in PATH, extract or symlink as [directory]/tools/wapiti or set wapiti_dir option to correct directory.")
```

### Comparing `dorkbot-0.3.1/dorkbot.egg-info/PKG-INFO` & `dorkbot-0.4.0/dorkbot.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorkbot
-Version: 0.3.1
+Version: 0.4.0
 Summary: Command-line tool to scan search results for vulnerabilities
 Home-page: http://dorkbot.io
 Author: jgor
 Author-email: jgor@utexas.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
@@ -29,87 +29,100 @@
 ==========
 * Create a Google API credential via the [Developer Console](https://console.developers.google.com)
 * Create a Google [Custom Search Engine](https://www.google.com/cse/) and note the search engine ID, e.g. 012345678901234567891:abc12defg3h
 <pre>$ pip3 install dorkbot wapiti3</pre>
 <pre>$ dorkbot -i google_api -o key=your_api_credential_here -o engine=your_engine_id_here -o query="filetype:php inurl:id"</pre>
 <pre>$ dorkbot -s wapiti</pre>
 
+Help
+====
+<pre>
+ -h, --help            Show program (or specified module) help
+</pre>
+<pre>
+  --show-defaults       Show default values in help output
+</pre>
+
 Usage
 =====
 <pre>
-usage: dorkbot [-h] [-c CONFIG] [-r DIRECTORY] [--log LOG] [-v] [-V]
-                  [-d DATABASE] [-u] [-l] [--list-unscanned]
-                  [--add-target TARGET] [--delete-target TARGET]
-                  [--flush-targets] [-i INDEXER] [-o INDEXER_OPTION]
-                  [-s SCANNER] [-p SCANNER_OPTION] [-f] [-b BLACKLIST]
-                  [--list-blacklist] [--add-blacklist-item ITEM]
-                  [--delete-blacklist-item ITEM] [--flush-blacklist]
+usage: dorkbot.py [-c CONFIG] [-r DIRECTORY] [--source [SOURCE]]
+                  [--show-defaults] [--count COUNT] [--random] [-h]
+                  [--log LOG] [-v] [-V] [-d DATABASE] [-u] [-l]
+                  [--list-unscanned] [--add-target TARGET]
+                  [--delete-target TARGET] [--flush-targets] [-i INDEXER]
+                  [-o INDEXER_ARG] [-s SCANNER] [-p SCANNER_ARG] [-f]
+                  [-b BLOCKLIST] [--list-blocklist]
+                  [--add-blocklist-item ITEM] [--delete-blocklist-item ITEM]
+                  [--flush-blocklist]
 
-optional arguments:
-  -h, --help            show this help message and exit
+options:
   -c CONFIG, --config CONFIG
                         Configuration file
   -r DIRECTORY, --directory DIRECTORY
                         Dorkbot directory (default location of db, tools,
                         reports)
+  --source [SOURCE]     Label associated with targets
+  --show-defaults       Show default values in help output
+  -h, --help            Show program (or specified module) help
   --log LOG             Path to log file
   -v, --verbose         Enable verbose logging (DEBUG output)
   -V, --version         Print version
 
+global scanner options:
+  --count COUNT         number of urls to scan, or -1 to scan all urls
+  --random              retrieve urls in random order
+
 database:
   -d DATABASE, --database DATABASE
                         Database file/uri
-  -u, --prune           Apply fingerprinting and blacklist without scanning
+  -u, --prune           Apply fingerprinting and blocklist without scanning
 
 targets:
   -l, --list-targets    List targets in database
   --list-unscanned      List unscanned targets in database
   --add-target TARGET   Add a url to the target database
   --delete-target TARGET
                         Delete a url from the target database
   --flush-targets       Delete all targets
 
 indexing:
   -i INDEXER, --indexer INDEXER
                         Indexer module to use
-  -o INDEXER_OPTION, --indexer-option INDEXER_OPTION
-                        Pass an option to the indexer (can be used multiple
-                        times)
+  -o INDEXER_ARG, --indexer-arg INDEXER_ARG
+                        Pass an argument to the indexer module (can be used
+                        multiple times)
 
 scanning:
   -s SCANNER, --scanner SCANNER
                         Scanner module to use
-  -p SCANNER_OPTION, --scanner-option SCANNER_OPTION
-                        Pass an option to the scanner (can be used multiple
-                        times)
+  -p SCANNER_ARG, --scanner-arg SCANNER_ARG
+                        Pass an argument to the scanner module (can be used
+                        multiple times)
 
 fingerprints:
   -f, --flush-fingerprints
                         Delete all fingerprints of previously-scanned items
 
-blacklist:
-  -b BLACKLIST, --blacklist BLACKLIST
-                        Blacklist file/uri
-  --list-blacklist      List blacklist entries
-  --add-blacklist-item ITEM
-                        Add an ip/host/regex pattern to the blacklist
-  --delete-blacklist-item ITEM
-                        Delete an item from the blacklist
-  --flush-blacklist     Delete all blacklist items
+blocklist:
+  -b BLOCKLIST, --blocklist BLOCKLIST
+                        Blocklist file/uri
+  --list-blocklist      List blocklist entries
+  --add-blocklist-item ITEM
+                        Add an ip/host/regex pattern to the blocklist
+  --delete-blocklist-item ITEM
+                        Delete an item from the blocklist
+  --flush-blocklist     Delete all blocklist items
 </pre>
 
-Requirements
-============
-* Python 3.x (cross-platform)
+Tools / Dependencies
+=====
 * [psycopg2-binary](https://pypi.org/project/psycopg2-binary/) or [psycopg2](https://pypi.org/project/psycopg2/) (if using PostgreSQL)
 * [phoenixdb](https://pypi.org/project/phoenixdb/) (if using PhoenixDB)
-
-Tools
-=====
-* [PhantomJS](http://phantomjs.org/)
+* [PhantomJS](http://phantomjs.org/) (if using non-api google indexer)
 * [Arachni](http://www.arachni-scanner.com/)
 * [Wapiti](http://wapiti.sourceforge.net/)
 
 As needed, dorkbot will search for tools in the following order:
 * Directory specified via relevant module option
 * Located in *tools* directory (within current directory, by default), with the subdirectory named after the tool
 * Available in the user's PATH (e.g. installed system-wide)
@@ -130,146 +143,148 @@
 ===========
 The configuration file (dorkbot.ini) can be used to prepopulate certain command-line flags.
 
 Example dorkbot.ini:
 <pre>
 [dorkbot]
 database=/opt/dorkbot/dorkbot.db
+[indexers.wayback]
+domain=example.com
+from=2022
+[scanners.arachni]
+arachni_dir=/opt/arachni
+report_dir=/tmp/reports
 </pre>
 
-Blacklist
+Blocklist
 =========
-The blacklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. By default the blacklist is stored in the dorkbot database, but a separate database or file can be specified by passing the appropriate connection uri or file path to --blacklist. Note: --add-blacklist-item / --delete-blacklist-item are not implemented for file-based blacklists, and --flush-blacklist deletes the file.
+The blocklist is a list of ip addresses, hostnames, or regular expressions of url patterns that should *not* be scanned. If a target url matches any item in this list it will be skipped and removed from the database. By default the blocklist is stored in the dorkbot database, but a separate database or file can be specified by passing the appropriate connection uri or file path to --blocklist. Note: --add-blocklist-item / --delete-blocklist-item are not implemented for file-based blocklists, and --flush-blocklist deletes the file.
 
-Supported external blacklists:
+Supported external blocklists:
 * postgresql://[server info]
 * phoenixdb://[server info]
-* sqlite3:///path/to/blacklist.db
-* /path/to/blacklist.txt
+* sqlite3:///path/to/blocklist.db
+* /path/to/blocklist.txt
 
-Example blacklist items:
+Example blocklist items:
 <pre>
 regex:^[^\?]+$
 regex:.*login.*
 regex:^https?://[^.]*.example.com/.*
 host:www.google.com
 ip:127.0.0.1
 </pre>
 
-The first item will remove any target that doesn't contain a question mark, in other words any url that doesn't contain any GET parameters to test. The second attempts to avoid login functions, and the third blacklists all target urls on example.com. The fourth excludes targets with a hostname of www.google.com and the fifth excludes targets whose host resolves to 127.0.0.1.
+The first item will remove any target that doesn't contain a question mark, in other words any url that doesn't contain any GET parameters to test. The second attempts to avoid login functions, and the third blocklists all target urls on example.com. The fourth excludes targets with a hostname of www.google.com and the fifth excludes targets whose host resolves to 127.0.0.1.
 
-Indexer Modules
-===============
-### (general options) ###
-These options are applicable regardless of module chosen
+Prune
+=====
+The prune flag iterates through all targets, computes the fingerprints in memory, and marks subsequent matching targets as scanned. Additionally it deletes any target matching a blocklist item. The result is a database where --list-unscanned returns only scannable urls. It honors the **random** flag to compute fingerprints in random order.
 
-* source - label stored in source field for target, overrides label provided by module (if present and without a value during list operations, source field will be printed along with url)
+General Options
+===============
+These options are applicable regardless of module chosen:
+<pre>
+  --source [SOURCE]     Label associated with targets
+  --count COUNT         number of urls to scan, or -1 to scan all urls
+  --random              retrieve urls in random order
+</pre>
 
+Indexer Modules
+===============
 ### google ###
-Search for targets in a Google Custom Search Engine (CSE) via custom search element.
-
-Requirements: [PhantomJS](http://phantomjs.org/)
+<pre>
+  Searches google.com via scraping
 
-Options:
-* **engine** - CSE id
-* **query** - search query
-* phantomjs_dir - phantomjs base directory containing bin/phantomjs (default: tools/phantomjs/)
-* domain - limit searches to specified domain
+  --engine ENGINE       CSE id
+  --query QUERY         search query
+  --phantomjs-dir PHANTOMJS_DIR
+                        phantomjs base dir containing bin/phantomjs
+  --domain DOMAIN       limit searches to specified domain
+</pre>
 
 ### google_api ###
-Search for targets in a Google Custom Search Engine (CSE) via JSON API.
-
-Requirements: none
+<pre>
+  Searches google.com
 
-Options:
-* **key** - API key
-* **engine** - CSE id
-* **query** - search query
-* domain - limit searches to specified domain
+  --key KEY             API key
+  --engine ENGINE       CSE id
+  --query QUERY         search query
+  --domain DOMAIN       limit searches to specified domain
+</pre>
 
 ### pywb ###
-Search for targets within a pywb instance's indexed results.
-
-Requirements: none
+<pre>
+  Searches a given pywb server's crawl data
 
-Options:
-* **server** - pywb server url
-* **domain** - pull all results for given domain or subdomain
-* cdx_api_suffix - suffix after index for index api (default: /cdx)
-* index - search a specific index (default: first fixed index, or first dynamic index)
-* filter - query filter to apply to the search
-* retries - number of times to retry fetching results on error (default: 10)
-* threads - number concurrent requests to pywb server (default: 10)
+  --server SERVER       pywb server url
+  --domain DOMAIN       pull all results for given domain or subdomain
+  --cdx-api-suffix CDX_API_SUFFIX
+                        suffix after index for index api
+  --index INDEX         search a specific index
+  --filter FILTER       query filter to apply to the search
+  --retries RETRIES     number of times to retry fetching results on error
+  --threads THREADS     number of concurrent requests to wayback.org
+</pre>
 
 ### commoncrawl ###
-Search for targets within commoncrawl.org results.
-
-Requirements: none
+<pre>
+  Searches commoncrawl.org crawl data
 
-Options:
-* **domain** - pull all results for given domain or subdomain
-* index - search a specific index, e.g. CC-MAIN-2019-22 (default: latest)
-* filter - query filter to apply to the search
-* retries - number of times to retry fetching results on error (default: 10)
-* threads - number concurrent requests to commoncrawl.org (default: 10)
+  --domain DOMAIN       pull all results for given domain or subdomain
+  --index INDEX         search a specific index, e.g. CC-MAIN-2019-22 (default: latest)
+  --filter FILTER       query filter to apply to the search
+  --retries RETRIES     number of times to retry fetching results on error
+  --threads THREADS     number of concurrent requests to commoncrawl.org
+</pre>
 
 ### wayback ###
-Search for targets within archive.org results.
-
-Requirements: none
+<pre>
+  Searches archive.org crawl data
 
-Options:
-* **domain** - pull all results for given domain or subdomain
-* filter - query filter to apply to the search
-* from - beginning timestamp
-* to - end timestamp
+  --domain DOMAIN       pull all results for given domain or subdomain
+  --filter FILTER       query filter to apply to the search
+  --from FROM           beginning timestamp
+  --to TO               end timestamp
+  --retries RETRIES     number of times to retry fetching results on error
+  --threads THREADS     number of concurrent requests to wayback.org
+</pre>
 
 ### bing_api ###
-Search for targets via Bing Web Search API.
-
-Requirements: none
+<pre>
+  Searches bing.com
 
-Options:
-* **key** - API key
-* **query** - search query
+  --key KEY             API key
+  --query QUERY         search query
+</pre>
 
 ### stdin ###
-Read targets from standard input, one per line.
-
-Requirements: none
-
-Options: none
+<pre>
+  Accepts urls from stdin, one per line
+</pre>
 
 Scanner Modules
 ===============
-### (general options) ###
-These options are applicable regardless of module chosen
-
-* report_dir - directory to save vulnerability report (default: reports/)
-* label - friendly name field to include in vulnerability report
-* count - number of urls to scan, or -1 to scan all urls (default: -1)
-* random - scan urls in random order
-
 ### arachni ###
-Scan targets with Arachni command-line scanner.
-
-Requirements: [Arachni](http://www.arachni-scanner.com/)
+<pre>
+  Scans with the arachni command-line scanner
 
-Options:
-* arachni_dir - arachni base directory containing bin/arachni and bin/arachni_reporter (default: tools/arachni/)
-* args - space-delimited list of additional arguments, e.g. args="--http-user-agent Dorkbot/1.0 --timeout 00:15:00"
+  --arachni-dir ARACHNI_DIR
+                        arachni base dir containing bin/arachni and bin/arachni_reporter
+  --args ARGS           space-delimited list of additional arguments
+  --report-dir REPORT_DIR
+                        directory to save vulnerability report
+  --label LABEL         friendly name field to include in vulnerability report
+</pre>
 
 ### wapiti ###
-Scan targets with Wapiti command-line scanner.
-
-Requirements: [Wapiti](http://wapiti.sourceforge.net/)
-
-Options:
-* wapiti_dir - wapiti base directory containing bin/wapiti (default: tools/wapiti/)
-* args - space-delimited list of additional arguments
-
-Prune
-=====
-The prune flag iterates through all targets, computes the fingerprints in memory, and marks subsequent matching targets as scanned. Additionally it deletes any target matching a blacklist item. The result is a database where --list-unscanned returns only scannable urls. It honors (a subset of) the options specified in SCANNER_OPTIONS as follows:
+<pre>
+  Scans with the wapiti3 command-line scanner
 
-* random - evaluate urls in random order when computing fingerprints
+  --wapiti-dir WAPITI_DIR
+                        wapiti base dir containing bin/wapiti
+  --args ARGS           space-delimited list of additional arguments
+  --report-dir REPORT_DIR
+                        directory to save vulnerability report
+  --label LABEL         friendly name field to include in vulnerability report
+</pre>
```

### Comparing `dorkbot-0.3.1/dorkbot.egg-info/SOURCES.txt` & `dorkbot-0.4.0/dorkbot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dorkbot-0.3.1/setup.py` & `dorkbot-0.4.0/setup.py`

 * *Files identical despite different names*

