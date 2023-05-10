# Comparing `tmp/mimeograph-0.4.2.tar.gz` & `tmp/mimeograph-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mimeograph-0.4.2.tar", last modified: Thu May  4 11:24:38 2023, max compression
+gzip compressed data, was "mimeograph-0.4.3.tar", last modified: Wed May 10 10:07:29 2023, max compression
```

## Comparing `mimeograph-0.4.2.tar` & `mimeograph-0.4.3.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.4.2/LICENSE
--rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-04-24 13:03:27.000000 mimeograph-0.4.2/MANIFEST.in
--rw-rw-r--   0 tom       (1000) tom       (1000)    22824 2023-05-04 11:24:38.404713 mimeograph-0.4.2/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)    20867 2023-05-04 11:08:55.000000 mimeograph-0.4.2/README.md
--rw-rw-r--   0 tom       (1000) tom       (1000)     1712 2023-05-04 11:24:30.000000 mimeograph-0.4.2/pyproject.toml
--rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-05-04 11:24:38.404713 mimeograph-0.4.2/setup.cfg
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.396713 mimeograph-0.4.2/src/
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1251 2023-05-04 11:24:30.000000 mimeograph-0.4.2/src/mimeo/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      372 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/__main__.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/cli/
--rw-rw-r--   0 tom       (1000) tom       (1000)      757 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/cli/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1498 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/cli/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4031 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/cli/job.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    17457 2023-05-04 11:24:30.000000 mimeograph-0.4.2/src/mimeo/cli/parsers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/config/
--rw-rw-r--   0 tom       (1000) tom       (1000)      521 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/config/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2994 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/config/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    30070 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/config/mimeo_config.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/consumers/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1232 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1240 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2192 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/consumer_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2152 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/file_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2997 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/http_consumer.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      825 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/consumers/raw_consumer.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/context/
--rw-rw-r--   0 tom       (1000) tom       (1000)      932 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4047 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/decorators.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4717 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    15071 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/mimeo_context.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     4786 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/mimeo_context_manager.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2752 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/context/mimeo_iteration.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/database/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1344 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5026 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/cities.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5307 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/countries.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1966 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     5111 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/first_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2045 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/last_names.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     7578 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/database/mimeo_db.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/generators/
--rw-rw-r--   0 tom       (1000) tom       (1000)      807 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/generators/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     2810 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/generators/generator.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1653 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/generators/generator_factory.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    11599 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/generators/xml_generator.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/logging/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1264 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/logging/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1645 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/logging/filters.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.400714 mimeograph-0.4.2/src/mimeo/meta/
--rw-rw-r--   0 tom       (1000) tom       (1000)      579 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/meta/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     3760 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/meta/alive.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      585 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/meta/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1408 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/mimeo.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/src/mimeo/resources/
--rw-rw-r--   0 tom       (1000) tom       (1000)      356 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/resources/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-05-04 10:17:10.000000 mimeograph-0.4.2/src/mimeo/resources/cities.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-05-04 10:17:10.000000 mimeograph-0.4.2/src/mimeo/resources/countries.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      700 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/resources/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-05-04 10:17:11.000000 mimeograph-0.4.2/src/mimeo/resources/forenames.csv
--rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.4.2/src/mimeo/resources/logging.yaml
--rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-05-04 10:17:13.000000 mimeograph-0.4.2/src/mimeo/resources/surnames.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)     1048 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/tools.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/src/mimeo/utils/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1749 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/utils/__init__.py
--rw-rw-r--   0 tom       (1000) tom       (1000)     1326 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/utils/exc.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    23391 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/utils/mimeo_utils.py
--rw-rw-r--   0 tom       (1000) tom       (1000)    19663 2023-05-04 11:08:55.000000 mimeograph-0.4.2/src/mimeo/utils/renderers.py
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/src/mimeograph.egg-info/
--rw-rw-r--   0 tom       (1000) tom       (1000)    22824 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/PKG-INFO
--rw-rw-r--   0 tom       (1000) tom       (1000)     1826 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/SOURCES.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/dependency_links.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/entry_points.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)       98 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/requires.txt
--rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-05-04 11:24:38.000000 mimeograph-0.4.2/src/mimeograph.egg-info/top_level.txt
-drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-04 11:24:38.404713 mimeograph-0.4.2/tests/
--rw-rw-r--   0 tom       (1000) tom       (1000)     1838 2023-05-04 11:08:55.000000 mimeograph-0.4.2/tests/test_mimeograph.py
--rw-rw-r--   0 tom       (1000) tom       (1000)      465 2023-04-24 13:03:27.000000 mimeograph-0.4.2/tests/test_tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.948366 mimeograph-0.4.3/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1075 2023-03-13 05:35:12.000000 mimeograph-0.4.3/LICENSE
+-rw-rw-r--   0 tom       (1000) tom       (1000)       30 2023-04-24 13:03:27.000000 mimeograph-0.4.3/MANIFEST.in
+-rw-rw-r--   0 tom       (1000) tom       (1000)    23631 2023-05-10 10:07:29.948366 mimeograph-0.4.3/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)    21275 2023-05-10 10:02:21.000000 mimeograph-0.4.3/README.md
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3529 2023-05-10 10:07:21.000000 mimeograph-0.4.3/pyproject.toml
+-rw-rw-r--   0 tom       (1000) tom       (1000)       38 2023-05-10 10:07:29.948366 mimeograph-0.4.3/setup.cfg
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/mimeo/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1327 2023-05-10 10:07:21.000000 mimeograph-0.4.3/src/mimeo/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      408 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/__main__.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/mimeo/cli/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      761 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/cli/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1660 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/cli/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4224 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/cli/job.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    17737 2023-05-10 10:07:21.000000 mimeograph-0.4.3/src/mimeo/cli/parsers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/mimeo/config/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      589 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/config/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     3111 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/config/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    29911 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/config/mimeo_config.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.940366 mimeograph-0.4.3/src/mimeo/consumers/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1322 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1323 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2135 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/consumer_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2146 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/file_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2814 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/http_consumer.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      892 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/consumers/raw_consumer.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/context/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1001 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4261 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/decorators.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5087 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    16065 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/mimeo_context.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5091 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/mimeo_context_manager.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2888 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/context/mimeo_iteration.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/database/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1533 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5515 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/cities.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5763 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/countries.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2120 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     5479 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/first_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2192 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/last_names.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     8025 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/database/mimeo_db.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/generators/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      868 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/generators/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2685 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/generators/generator.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1640 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/generators/generator_factory.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    22917 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/generators/xml_generator.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/logging/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1364 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/logging/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1743 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/logging/filters.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/meta/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      652 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/meta/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4028 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/meta/alive.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      651 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/meta/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1474 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/mimeo.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.944366 mimeograph-0.4.3/src/mimeo/resources/
+-rw-rw-r--   0 tom       (1000) tom       (1000)      357 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/resources/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1541655 2023-05-08 08:24:08.000000 mimeograph-0.4.3/src/mimeo/resources/cities.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)     4205 2023-05-08 08:24:08.000000 mimeograph-0.4.3/src/mimeo/resources/countries.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      778 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/resources/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    66313 2023-05-08 08:24:10.000000 mimeograph-0.4.3/src/mimeo/resources/forenames.csv
+-rw-rw-r--   0 tom       (1000) tom       (1000)      719 2023-03-31 04:40:40.000000 mimeograph-0.4.3/src/mimeo/resources/logging.yaml
+-rw-rw-r--   0 tom       (1000) tom       (1000)  1197769 2023-05-08 08:24:13.000000 mimeograph-0.4.3/src/mimeo/resources/surnames.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1030 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/tools.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.948366 mimeograph-0.4.3/src/mimeo/utils/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     2063 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/utils/__init__.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1412 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/utils/exc.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    24474 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/utils/mimeo_utils.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)    20016 2023-05-10 04:50:43.000000 mimeograph-0.4.3/src/mimeo/utils/renderers.py
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.948366 mimeograph-0.4.3/src/mimeograph.egg-info/
+-rw-rw-r--   0 tom       (1000) tom       (1000)    23631 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/PKG-INFO
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1826 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/SOURCES.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        1 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/dependency_links.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)       46 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/entry_points.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)      132 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/requires.txt
+-rw-rw-r--   0 tom       (1000) tom       (1000)        6 2023-05-10 10:07:29.000000 mimeograph-0.4.3/src/mimeograph.egg-info/top_level.txt
+drwxrwxr-x   0 tom       (1000) tom       (1000)        0 2023-05-10 10:07:29.948366 mimeograph-0.4.3/tests/
+-rw-rw-r--   0 tom       (1000) tom       (1000)     1794 2023-05-10 04:50:43.000000 mimeograph-0.4.3/tests/test_mimeograph.py
+-rw-rw-r--   0 tom       (1000) tom       (1000)      514 2023-05-10 04:50:43.000000 mimeograph-0.4.3/tests/test_tools.py
```

### Comparing `mimeograph-0.4.2/LICENSE` & `mimeograph-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.2/PKG-INFO` & `mimeograph-0.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.4.2
+Version: 0.4.3
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,33 +21,45 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Keywords: mimeograph,mimeo,generate,generator
+Project-URL: GitHub, https://github.com/TomaszAniolowski/mimeo
+Keywords: mimeograph,mimeo,generate,generator,data,xml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
-
 # Mimeo (Mimeograph)
 
-**Mimeo** is a command line tool and python library generating custom data based on a template.
+[![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
+[![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)  
+[![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
+[![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
+
+[Mimeo](https://github.com/TomaszAniolowski/mimeo) is a command line tool and python library generating custom data based on a template.
 It can be used by developers, testers or even business analysts in their daily work.
 
 
 ## Installation
 
 Install Mimeo with pip
 
@@ -165,31 +177,31 @@
 
 ### Mimeo CLI
 
 #### Mimeo Configuration arguments
 
 When using Mimeo command line tool you can overwrite Mimeo Configuration properties:
 
-| Short option | Long option         | Description                                                                          |
-|:------------:|:--------------------|:-------------------------------------------------------------------------------------|
-|     `-o`     | `--output`          | overwrite the `output_details/direction` property                                    |
-|     `-x`     | `--xml-declaration` | overwrite the `output_details/xml_declaration` property                              |
-|     `-i`     | `--indent`          | overwrite the `output_details/indent` property                                       |
-|     `-d`     | `--directory`       | overwrite the `output_details/directory_path` property                               |
-|     `-f`     | `--file`            | overwrite the `output_details/file_name` property                                    |
-|     `-H`     | `--http-host`       | overwrite the `output_details/host` property                                         |
-|     `-p`     | `--http-port`       | overwrite the `output_details/port` property                                         |
-|     `-E`     | `--http-endpoint`   | overwrite the `output_details/endpoint` property                                     |
-|     `-U`     | `--http-user`       | overwrite the `output_details/username` property                                     |
-|     `-P`     | `--http-password`   | overwrite the `output_details/password` property                                     |
-|              | `--http-method`     | overwrite the `output_details/method` property                                       |
-|              | `--http-protocol`   | overwrite the `output_details/protocol` property                                     |
-|              | `--http-auth`       | overwrite the `output_details/auth` property                                         |
-|     `-e`     | `--http-env`        | overwrite the output_details http properties using a mimeo environment configuration |
-|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                         |
+| Short option | Long option         | Description                                                                  |
+|:------------:|:--------------------|:-----------------------------------------------------------------------------|
+|     `-o`     | `--output`          | overwrite the `output/direction` property                            |
+|     `-x`     | `--xml-declaration` | overwrite the `output/xml_declaration` property                      |
+|     `-i`     | `--indent`          | overwrite the `output/indent` property                               |
+|     `-d`     | `--directory`       | overwrite the `output/directory_path` property                       |
+|     `-f`     | `--file`            | overwrite the `output/file_name` property                            |
+|     `-H`     | `--http-host`       | overwrite the `output/host` property                                 |
+|     `-p`     | `--http-port`       | overwrite the `output/port` property                                 |
+|     `-E`     | `--http-endpoint`   | overwrite the `output/endpoint` property                             |
+|     `-U`     | `--http-user`       | overwrite the `output/username` property                             |
+|     `-P`     | `--http-password`   | overwrite the `output/password` property                             |
+|              | `--http-method`     | overwrite the `output/method` property                               |
+|              | `--http-protocol`   | overwrite the `output/protocol` property                             |
+|              | `--http-auth`       | overwrite the `output/auth` property                                 |
+|     `-e`     | `--http-env`        | overwrite the output http properties using a mimeo env configuration |
+|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                 |
 
 #### Logging arguments
 
 | Short option | Long option | Description       |
 |:------------:|:------------|:------------------|
 |              | `--silent`  | disable INFO logs |
 |              | `--debug`   | enable DEBUG mode |
@@ -197,29 +209,29 @@
 
 ### Mimeo Configuration
 
 Mimeo configuration is defined in a JSON file using internal settings and data templates.
 
 | Key                              |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
 |:---------------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `output_details`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
-| `output_details/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
-| `output_details/format`          |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
-| `output_details/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
-| `output_details/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
-| `output_details/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
-| `output_details/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
-| `output_details/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
-| `output_details/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
-| `output_details/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
-| `output_details/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
-| `output_details/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output_details/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
-| `output_details/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
-| `output_details/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
+| `output`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
+| `output/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
+| `output/format`          |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
+| `output/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
+| `output/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
+| `output/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
+| `output/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
+| `output/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
+| `output/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
+| `output/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
+| `output/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
+| `output/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
+| `output/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
+| `output/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
+| `output/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
 | `vars`                           |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
 | `_templates_`                    |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
 | `count`                          | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
 | `model`                          | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
 | `context`                        |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
 #### Mimeo Environment
```

### Comparing `mimeograph-0.4.2/README.md` & `mimeograph-0.4.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-
 # Mimeo (Mimeograph)
 
-**Mimeo** is a command line tool and python library generating custom data based on a template.
+[![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
+[![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)  
+[![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
+[![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
+
+[Mimeo](https://github.com/TomaszAniolowski/mimeo) is a command line tool and python library generating custom data based on a template.
 It can be used by developers, testers or even business analysts in their daily work.
 
 
 ## Installation
 
 Install Mimeo with pip
 
@@ -123,31 +127,31 @@
 
 ### Mimeo CLI
 
 #### Mimeo Configuration arguments
 
 When using Mimeo command line tool you can overwrite Mimeo Configuration properties:
 
-| Short option | Long option         | Description                                                                          |
-|:------------:|:--------------------|:-------------------------------------------------------------------------------------|
-|     `-o`     | `--output`          | overwrite the `output_details/direction` property                                    |
-|     `-x`     | `--xml-declaration` | overwrite the `output_details/xml_declaration` property                              |
-|     `-i`     | `--indent`          | overwrite the `output_details/indent` property                                       |
-|     `-d`     | `--directory`       | overwrite the `output_details/directory_path` property                               |
-|     `-f`     | `--file`            | overwrite the `output_details/file_name` property                                    |
-|     `-H`     | `--http-host`       | overwrite the `output_details/host` property                                         |
-|     `-p`     | `--http-port`       | overwrite the `output_details/port` property                                         |
-|     `-E`     | `--http-endpoint`   | overwrite the `output_details/endpoint` property                                     |
-|     `-U`     | `--http-user`       | overwrite the `output_details/username` property                                     |
-|     `-P`     | `--http-password`   | overwrite the `output_details/password` property                                     |
-|              | `--http-method`     | overwrite the `output_details/method` property                                       |
-|              | `--http-protocol`   | overwrite the `output_details/protocol` property                                     |
-|              | `--http-auth`       | overwrite the `output_details/auth` property                                         |
-|     `-e`     | `--http-env`        | overwrite the output_details http properties using a mimeo environment configuration |
-|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                         |
+| Short option | Long option         | Description                                                                  |
+|:------------:|:--------------------|:-----------------------------------------------------------------------------|
+|     `-o`     | `--output`          | overwrite the `output/direction` property                            |
+|     `-x`     | `--xml-declaration` | overwrite the `output/xml_declaration` property                      |
+|     `-i`     | `--indent`          | overwrite the `output/indent` property                               |
+|     `-d`     | `--directory`       | overwrite the `output/directory_path` property                       |
+|     `-f`     | `--file`            | overwrite the `output/file_name` property                            |
+|     `-H`     | `--http-host`       | overwrite the `output/host` property                                 |
+|     `-p`     | `--http-port`       | overwrite the `output/port` property                                 |
+|     `-E`     | `--http-endpoint`   | overwrite the `output/endpoint` property                             |
+|     `-U`     | `--http-user`       | overwrite the `output/username` property                             |
+|     `-P`     | `--http-password`   | overwrite the `output/password` property                             |
+|              | `--http-method`     | overwrite the `output/method` property                               |
+|              | `--http-protocol`   | overwrite the `output/protocol` property                             |
+|              | `--http-auth`       | overwrite the `output/auth` property                                 |
+|     `-e`     | `--http-env`        | overwrite the output http properties using a mimeo env configuration |
+|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                 |
 
 #### Logging arguments
 
 | Short option | Long option | Description       |
 |:------------:|:------------|:------------------|
 |              | `--silent`  | disable INFO logs |
 |              | `--debug`   | enable DEBUG mode |
@@ -155,29 +159,29 @@
 
 ### Mimeo Configuration
 
 Mimeo configuration is defined in a JSON file using internal settings and data templates.
 
 | Key                              |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
 |:---------------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `output_details`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
-| `output_details/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
-| `output_details/format`          |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
-| `output_details/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
-| `output_details/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
-| `output_details/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
-| `output_details/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
-| `output_details/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
-| `output_details/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
-| `output_details/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
-| `output_details/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
-| `output_details/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output_details/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
-| `output_details/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
-| `output_details/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
+| `output`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
+| `output/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
+| `output/format`          |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
+| `output/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
+| `output/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
+| `output/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
+| `output/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
+| `output/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
+| `output/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
+| `output/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
+| `output/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
+| `output/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
+| `output/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
+| `output/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
+| `output/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
 | `vars`                           |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
 | `_templates_`                    |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
 | `count`                          | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
 | `model`                          | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
 | `context`                        |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
 #### Mimeo Environment
```

### Comparing `mimeograph-0.4.2/src/mimeo/__init__.py` & `mimeograph-0.4.3/src/mimeo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,11 +39,14 @@
     The Mimeo module
 * tools
     The Mimeo Tools module
 
 To use this package, simply import the desired classes:
     from mimeo import MimeoConfig, Mimeograph
 """
+from __future__ import annotations
+
 from .config import MimeoConfig
 from .mimeo import Mimeograph
 
-__version__ = "0.4.2"
+__version__ = "0.4.3"
+__all__ = ["MimeoConfig", "Mimeograph"]
```

### Comparing `mimeograph-0.4.2/src/mimeo/cli/exc.py` & `mimeograph-0.4.3/src/mimeo/cli/exc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 """The Mimeo CLI Exceptions module.
 
 It contains all custom exceptions related to Mimeo CLI:
-    * EnvironmentNotFound
+    * EnvironmentNotFoundError
         A custom Exception class for not found environment.
-    * EnvironmentsFileNotFound
+    * EnvironmentsFileNotFoundError
         A custom Exception class for not found environments file.
 """
 
 
-class EnvironmentNotFound(Exception):
+from __future__ import annotations
+
+
+class EnvironmentNotFoundError(Exception):
     """A custom Exception class for not found environment.
 
-    Raised while attempting to access an environment that does not
-    exist.
+    Raised while attempting to access an environment that does not exist.
     """
 
-    def __init__(self, env_name: str, envs_file_path: str):
-        """Initialize EnvironmentNotFound exception with details.
+    def __init__(
+            self,
+            env_name: str,
+            envs_file_path: str,
+    ):
+        """Initialize EnvironmentNotFoundError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         env_name : str
             An environment name
         envs_file_path : str
             An environments file path
         """
-        super().__init__(f"No such env [{env_name}] in environments file [{envs_file_path}]")
+        super().__init__(f"No such env [{env_name}] "
+                         f"in environments file [{envs_file_path}]")
 
 
-class EnvironmentsFileNotFound(Exception):
+class EnvironmentsFileNotFoundError(Exception):
     """A custom Exception class for not found environments file.
 
-    Raised while attempting to access an environments file that does
-    not exist.
+    Raised while attempting to access an environments file that does not exist.
     """
 
-    def __init__(self, envs_file_path: str):
-        """Initialize EnvironmentsFileNotFound exception with details.
+    def __init__(
+            self,
+            envs_file_path: str,
+    ):
+        """Initialize EnvironmentsFileNotFoundError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         envs_file_path : str
             An environments file path
```

### Comparing `mimeograph-0.4.2/src/mimeo/cli/job.py` & `mimeograph-0.4.3/src/mimeo/cli/job.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """The Mimeo Job module.
 
 It exports a single class:
     * MimeoJob
         A class representing a single Mimeo processing job.
 """
+from __future__ import annotations
+
 import json
 import logging
 from argparse import Namespace
-from os import path, walk
+from os import walk
+from pathlib import Path
 
 from mimeo import MimeoConfig, Mimeograph
 from mimeo.cli import MimeoArgumentParser, MimeoConfigParser
 
 logger = logging.getLogger(__name__)
 
 
@@ -26,44 +29,52 @@
 
     Methods
     -------
     run()
         Executes a Mimeo Job based on the CLI arguments.
     """
 
-    def __init__(self):
+    def __init__(
+            self,
+    ):
         """Initialize MimeoJob class."""
         self._args = MimeoArgumentParser().parse_args()
 
-    def run(self):
+    def run(
+            self,
+    ):
         """Execute a Mimeo Job based on the CLI arguments.
 
         First it customizes a log level. After that all Mimeo Configs
         paths are collected. Each of them is used in the next steps,
         which are: (1) parsing the configuration and (2) processing
         it.
         """
         self._customize_log_level(self._args)
         logger.info("Starting a Mimeo job")
         for config_path in self._get_config_paths(self._args.paths):
             mimeo_config = self._get_mimeo_config(config_path, self._args)
             Mimeograph(mimeo_config).process()
 
     @staticmethod
-    def _customize_log_level(args):
+    def _customize_log_level(
+            args,
+    ):
         """Customize the log level based on command line arguments."""
         if args.silent:
             logging.getLogger("mimeo").setLevel(logging.WARNING)
         elif args.debug:
             logging.getLogger("mimeo").setLevel(logging.DEBUG)
         elif args.fine and hasattr(logging, "FINE"):
             logging.getLogger("mimeo").setLevel(logging.FINE)
 
     @staticmethod
-    def _get_config_paths(paths: list) -> list:
+    def _get_config_paths(
+            paths: list,
+    ) -> list:
         """Collect Mimeo Configuration paths.
 
         This method traverses directory paths and collects all files
         within.
 
         Parameters
         ----------
@@ -73,24 +84,28 @@
         Returns
         -------
         file_paths : list
             A list of file paths
         """
         file_paths = []
         for file_path in paths:
-            if path.isdir(file_path):
+            if Path(file_path).is_dir():
                 for dir_path, _, file_names in walk(file_path):
                     for file_name in file_names:
                         file_paths.append(f"{dir_path}/{file_name}")
-            elif path.isfile(file_path):
+            elif Path(file_path).is_file():
                 file_paths.append(file_path)
         return file_paths
 
     @classmethod
-    def _get_mimeo_config(cls, config_path: str, args: Namespace) -> MimeoConfig:
+    def _get_mimeo_config(
+            cls,
+            config_path: str,
+            args: Namespace,
+    ) -> MimeoConfig:
         """Return parsed Mimeo Configuration.
 
         This method parses a raw configuration with command line
         arguments using a MimeoConfigParser instance.
 
         Parameters
         ----------
@@ -102,23 +117,24 @@
         Returns
         -------
         MimeoConfig
             A parsed Mimeo Configuration
 
         Raises
         ------
-        EnvironmentsFileNotFound
+        EnvironmentsFileNotFoundError
             If environments file does not exist.
-        EnvironmentNotFound
+        EnvironmentNotFoundError
             If the http environment is not defined in the environments file
         """
         config = cls._get_raw_config(config_path)
         mimeo_config_parser = MimeoConfigParser(config, args)
         return mimeo_config_parser.parse_config()
 
     @staticmethod
-    def _get_raw_config(config_path: str) -> dict:
+    def _get_raw_config(
+            config_path: str,
+    ) -> dict:
         """Load configuration file to a dictionary."""
-        logger.info(f"Reading Mimeo Configuration: {config_path}")
-        with open(config_path) as config_file:
-            config = json.load(config_file)
-        return config
+        logger.info("Reading Mimeo Configuration: %s", config_path)
+        with Path(config_path).open() as config_file:
+            return json.load(config_file)
```

### Comparing `mimeograph-0.4.2/src/mimeo/cli/parsers.py` & `mimeograph-0.4.3/src/mimeo/cli/parsers.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,36 @@
 It exports two parser classes:
     * MimeoArgumentParser
         A custom ArgumentParser for the Mimeo CLI.
     * MimeoConfigParser
         A class parsing source Mimeo Configuration with Mimeo
         arguments.
 """
+from __future__ import annotations
+
 import json
 import logging
 from argparse import ArgumentParser, Namespace
-from os import path
-from typing import Union
+from pathlib import Path
 
 from mimeo import MimeoConfig
-from mimeo.cli.exc import EnvironmentNotFound, EnvironmentsFileNotFound
+from mimeo.cli.exc import (EnvironmentNotFoundError,
+                           EnvironmentsFileNotFoundError)
 
 logger = logging.getLogger(__name__)
 
-DEFAULT_ENVS_FILE_PATH = "mimeo.envs.json"
+DEFAULT_ENVS_PATH = "mimeo.envs.json"
 
 
 class MimeoArgumentParser(ArgumentParser):
     """A custom ArgumentParser for the Mimeo CLI."""
 
-    def __init__(self):
+    def __init__(
+            self,
+    ):
         """Initialize MimeoArgumentParser class.
 
         Extends ArgumentParser constructor with a Mimeo CLI details.
 
         It provides the following command line interface:
 
         usage: mimeo [OPTIONS] paths
@@ -40,160 +44,168 @@
 
         optional arguments:
           -h, --help            show this help message and exit
           -v, --version         show program's version number and exit
 
         Mimeo Configuration arguments:
           -o {file,stdout,http}, --output {file,stdout,http}
-                                overwrite the output_details/direction property
+                                overwrite the output/direction property
           -x {true,false}, --xml-declaration {true,false}
-                                overwrite the output_details/xml_declaration property
+                                overwrite the output/xml_declaration property
           -i INDENT, --indent INDENT
-                                overwrite the output_details/indent property
+                                overwrite the output/indent property
           -d DIRECTORY_PATH, --directory DIRECTORY_PATH
-                                overwrite the output_details/directory_path property
+                                overwrite the output/directory_path property
           -f FILE_NAME, --file FILE_NAME
-                                overwrite the output_details/file_name property
+                                overwrite the output/file_name property
           -H HOST, --http-host HOST
-                                overwrite the output_details/host property
+                                overwrite the output/host property
           -p PORT, --http-port PORT
-                                overwrite the output_details/port property
+                                overwrite the output/port property
           -E ENDPOINT, --http-endpoint ENDPOINT
-                                overwrite the output_details/endpoint property
+                                overwrite the output/endpoint property
           -U USERNAME, --http-user USERNAME
-                                overwrite the output_details/username property
+                                overwrite the output/username property
           -P PASSWORD, --http-password PASSWORD
-                                overwrite the output_details/password property
+                                overwrite the output/password property
           --http-method METHOD
-                                overwrite the output_details/method property
+                                overwrite the output/method property
           --http-protocol PROTOCOL
-                                overwrite the output_details/protocol property
+                                overwrite the output/protocol property
           --http-auth AUTH
-                                overwrite the output_details/auth property
+                                overwrite the output/auth property
           -e ENVIRONMENT, --http-env ENVIRONMENT
-                                overwrite the output_details http properties using a mimeo environment configuration
+                                overwrite the output http properties using a mimeo
+                                env configuration
           --http-envs-file PATH
-                                use a custom environments file (by default: mimeo.envs.json)
+                                use a custom environments file
+                                (by default: mimeo.envs.json)
 
         Logging arguments:
           --silent              disable INFO logs
           --debug               enable DEBUG mode
           --fine                enable FINE mode
         """
         super().__init__(
             prog="mimeo",
             description="Generate data based on a template",
             usage="%(prog)s [OPTIONS] paths")
         self._add_positional_arguments()
         self._add_mimeo_configuration_arguments()
         self._add_logging_arguments()
 
-    def _add_positional_arguments(self):
+    def _add_positional_arguments(
+            self,
+    ):
         """Add positional arguments."""
         self.add_argument(
             "-v",
             "--version",
             action="version",
-            version="%(prog)s v0.4.2")
+            version="%(prog)s v0.4.3")
         self.add_argument(
             "paths",
             nargs="+",
             type=str,
             help="take paths to Mimeo Configuration files")
 
-    def _add_mimeo_configuration_arguments(self):
+    def _add_mimeo_configuration_arguments(
+            self,
+    ):
         """Add arguments overwriting Mimeo Configuration."""
         mimeo_config_args = self.add_argument_group("Mimeo Configuration arguments")
         mimeo_config_args.add_argument(
             "-o",
             "--output",
             type=str,
             choices=["file", "stdout", "http"],
-            help="overwrite the output_details/direction property")
+            help="overwrite the output/direction property")
         mimeo_config_args.add_argument(
             "-x",
             "--xml-declaration",
             type=str,
             choices=["true", "false"],
-            help="overwrite the output_details/xml_declaration property")
+            help="overwrite the output/xml_declaration property")
         mimeo_config_args.add_argument(
             "-i",
             "--indent",
             type=int,
-            help="overwrite the output_details/indent property")
+            help="overwrite the output/indent property")
         mimeo_config_args.add_argument(
             "-d",
             "--directory",
             type=str,
             metavar="DIRECTORY_PATH",
-            help="overwrite the output_details/directory_path property")
+            help="overwrite the output/directory_path property")
         mimeo_config_args.add_argument(
             "-f",
             "--file",
             type=str,
             metavar="FILE_NAME",
-            help="overwrite the output_details/file_name property")
+            help="overwrite the output/file_name property")
         mimeo_config_args.add_argument(
             "-H",
             "--http-host",
             type=str,
             metavar="HOST",
-            help="overwrite the output_details/host property")
+            help="overwrite the output/host property")
         mimeo_config_args.add_argument(
             "-p",
             "--http-port",
             type=str,
             metavar="PORT",
-            help="overwrite the output_details/port property")
+            help="overwrite the output/port property")
         mimeo_config_args.add_argument(
             "-E",
             "--http-endpoint",
             type=str,
             metavar="ENDPOINT",
-            help="overwrite the output_details/endpoint property")
+            help="overwrite the output/endpoint property")
         mimeo_config_args.add_argument(
             "-U",
             "--http-user",
             type=str,
             metavar="USERNAME",
-            help="overwrite the output_details/username property")
+            help="overwrite the output/username property")
         mimeo_config_args.add_argument(
             "-P",
             "--http-password",
             type=str,
             metavar="PASSWORD",
-            help="overwrite the output_details/password property")
+            help="overwrite the output/password property")
         mimeo_config_args.add_argument(
             "--http-method",
             type=str,
             metavar="METHOD",
-            help="overwrite the output_details/method property")
+            help="overwrite the output/method property")
         mimeo_config_args.add_argument(
             "--http-protocol",
             type=str,
             metavar="PROTOCOL",
-            help="overwrite the output_details/protocol property")
+            help="overwrite the output/protocol property")
         mimeo_config_args.add_argument(
             "--http-auth",
             type=str,
             metavar="AUTH",
-            help="overwrite the output_details/auth property")
+            help="overwrite the output/auth property")
         mimeo_config_args.add_argument(
             "-e",
             "--http-env",
             type=str,
             metavar="ENVIRONMENT",
-            help="overwrite the output_details http properties using a mimeo environment configuration")
+            help="overwrite the output http properties using a mimeo env configuration")
         mimeo_config_args.add_argument(
             "--http-envs-file",
             type=str,
             metavar="PATH",
-            help=f"use a custom environments file (by default: {DEFAULT_ENVS_FILE_PATH})")
+            help=f"use a custom environments file (by default: {DEFAULT_ENVS_PATH})")
 
-    def _add_logging_arguments(self):
+    def _add_logging_arguments(
+            self,
+    ):
         """Add arguments customizing logs producing."""
         logging_args = self.add_argument_group("Logging arguments")
         logging_args_excl = logging_args.add_mutually_exclusive_group()
         logging_args_excl.add_argument(
             "--silent",
             action="store_true",
             help="disable INFO logs")
@@ -212,80 +224,99 @@
 
     Methods
     -------
     parse_config() -> MimeoConfig
         Parse a Mimeo Configuration using Mimeo arguments.
     """
 
-    _ENVIRONMENT_PROPS = [MimeoConfig.OUTPUT_DETAILS_PROTOCOL_KEY,
-                          MimeoConfig.OUTPUT_DETAILS_HOST_KEY,
-                          MimeoConfig.OUTPUT_DETAILS_PORT_KEY,
-                          MimeoConfig.OUTPUT_DETAILS_AUTH_KEY,
-                          MimeoConfig.OUTPUT_DETAILS_USERNAME_KEY,
-                          MimeoConfig.OUTPUT_DETAILS_PASSWORD_KEY]
-    
+    _ENVIRONMENT_PROPS = [MimeoConfig.OUTPUT_PROTOCOL_KEY,
+                          MimeoConfig.OUTPUT_HOST_KEY,
+                          MimeoConfig.OUTPUT_PORT_KEY,
+                          MimeoConfig.OUTPUT_AUTH_KEY,
+                          MimeoConfig.OUTPUT_USERNAME_KEY,
+                          MimeoConfig.OUTPUT_PASSWORD_KEY]
+
     _ENTRY_PATH_KEY = "entry_path"
     _GET_VALUE_KEY = "get_value"
     _ARGS_MAPPING = {
         "output": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_DIRECTION_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_DIRECTION_KEY],
         },
         "xml_declaration": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_XML_DECLARATION_KEY],
-            "get_value": lambda arg: arg.lower() == "true"
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_XML_DECLARATION_KEY],
+            "get_value": lambda arg: arg.lower() == "true",
         },
         "indent": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_INDENT_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_INDENT_KEY],
         },
         "directory": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_DIRECTORY_PATH_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_DIRECTORY_PATH_KEY],
         },
         "file": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_FILE_NAME_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_FILE_NAME_KEY],
         },
         "http_method": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_METHOD_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_METHOD_KEY],
         },
         "http_protocol": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_PROTOCOL_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_PROTOCOL_KEY],
         },
         "http_auth": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_AUTH_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_AUTH_KEY],
         },
         "http_host": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_HOST_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_HOST_KEY],
         },
         "http_port": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_PORT_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_PORT_KEY],
         },
         "http_endpoint": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_ENDPOINT_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_ENDPOINT_KEY],
         },
         "http_user": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_USERNAME_KEY]
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_USERNAME_KEY],
         },
         "http_password": {
-            "entry_path": [MimeoConfig.OUTPUT_DETAILS_KEY, MimeoConfig.OUTPUT_DETAILS_PASSWORD_KEY]
-        }
+            "entry_path": [MimeoConfig.OUTPUT_KEY,
+                           MimeoConfig.OUTPUT_PASSWORD_KEY],
+        },
     }
 
-    def __init__(self, config: dict, args: Namespace):
+    def __init__(
+            self,
+            config: dict,
+            args: Namespace,
+    ):
         """Initialize MimeoConfigParser class.
 
         Parameters
         ----------
         config:
             A source config dictionary
         args
             Arguments parsed by MimeoArgumentParser
         """
         self._raw_config = config
         self._args = args
 
-    def parse_config(self) -> MimeoConfig:
+    def parse_config(
+            self,
+    ) -> MimeoConfig:
         """Parse a Mimeo Configuration using Mimeo arguments.
 
         The parsing is made according to the following rule:
         configuration is overwritten from the most general to the most
         specific setting. It means that, whenever CLI arguments
         are overlapping (e.g. -e and -u), first the higher-level
         customization is applied (e.g. environment) and then the lower
@@ -294,28 +325,31 @@
         Returns
         -------
         mimeo_config : MimeoConfig
             A parsed Mimeo Configuration
 
         Raises
         ------
-        EnvironmentsFileNotFound
+        EnvironmentsFileNotFoundError
             If environments file does not exist.
-        EnvironmentNotFound
+        EnvironmentNotFoundError
             If the http environment is not defined in the environments file
         """
         logger.info("Parsing Mimeo Configuration")
         config = dict(self._raw_config)
         config = self._parse_with_http_environment(config)
         config = self._parse_with_specific_args(config)
         mimeo_config = MimeoConfig(config)
-        logger.fine(f"Parsed Mimeo Configuration: [{mimeo_config}]")
+        logger.fine("Parsed Mimeo Configuration: [%s]", mimeo_config)
         return mimeo_config
 
-    def _parse_with_http_environment(self, config: dict) -> dict:
+    def _parse_with_http_environment(
+            self,
+            config: dict,
+    ) -> dict:
         """Parse Mimeo Configuration with an HTTP environment.
 
         When --http-envs-file argument has not been provided, then
         the default environments path is used: mimeo.envs.json.
 
         Parameters
         ----------
@@ -327,26 +361,32 @@
         config : dict
             An overwritten Mimeo Configuration dictionary when
             --http-env argument has been provided. Otherwise,
             the source one, without any modification.
 
         Raises
         ------
-        EnvironmentsFileNotFound
+        EnvironmentsFileNotFoundError
             If environments file does not exist.
-        EnvironmentNotFound
+        EnvironmentNotFoundError
             If the http environment is not defined in the environments file
         """
-        if self._args.http_env is not None:
-            envs_file_path = self._args.http_envs_file if self._args.http_envs_file is not None else DEFAULT_ENVS_FILE_PATH
-            env = self._get_environment(envs_file_path, self._args.http_env)
-            self._overwrite_output_details_with_env(config, env)
-        return config
+        if self._args.http_env is None:
+            return config
 
-    def _parse_with_specific_args(self, config: dict) -> dict:
+        if self._args.http_envs_file is None:
+            env = self._get_environment(DEFAULT_ENVS_PATH, self._args.http_env)
+        else:
+            env = self._get_environment(self._args.http_envs_file, self._args.http_env)
+        return self._overwrite_output_with_env(config, env)
+
+    def _parse_with_specific_args(
+            self,
+            config: dict,
+    ) -> dict:
         """Parse Mimeo Configuration with Mimeo Configuration args.
 
         This method uses an internal `dict` fetching each command line
         argument with a corresponding Mimeo Configuration entry.
 
         Parameters
         ----------
@@ -357,23 +397,28 @@
         -------
         config : dict
             An overwritten Mimeo Configuration dictionary when
             some configuration arguments have been provided. Otherwise,
             the source one, without any modification.
         """
         for arg_name, mapping in self._ARGS_MAPPING.items():
-            if hasattr(self._args, arg_name) and getattr(self._args, arg_name) is not None:
+            arg = getattr(self._args, arg_name, None)
+            if arg is not None:
                 entry_path = mapping.get(self._ENTRY_PATH_KEY, arg_name)
-                get_value = mapping.get(self._GET_VALUE_KEY, lambda arg: arg)
-                value = get_value(getattr(self._args, arg_name))
+                get_value = mapping.get(self._GET_VALUE_KEY, lambda a: a)
+                value = get_value(arg)
                 config = self._overwrite_config_entry(config, entry_path, value)
         return config
 
     @classmethod
-    def _overwrite_output_details_with_env(cls, config: dict, env: dict) -> dict:
+    def _overwrite_output_with_env(
+            cls,
+            config: dict,
+            env: dict,
+    ) -> dict:
         """Overwrite Mimeo Output Details with an environment config.
 
         Parameters
         ----------
         config : dict
             A source Mimeo Configuration dictionary
         env : dict
@@ -383,56 +428,67 @@
         -------
         config : dict
             An overwritten Mimeo Configuration.
         """
         for prop in cls._ENVIRONMENT_PROPS:
             value = env.get(prop)
             if value is not None:
-                config_entry_path = [MimeoConfig.OUTPUT_DETAILS_KEY, prop]
+                config_entry_path = [MimeoConfig.OUTPUT_KEY, prop]
                 config = cls._overwrite_config_entry(config, config_entry_path, value)
         return config
 
     @classmethod
-    def _overwrite_config_entry(cls, config_entry: dict, entry_path: list, value: Union[str, int, bool]) -> dict:
+    def _overwrite_config_entry(
+            cls,
+            config_entry: dict,
+            entry_path: list,
+            value: str | int | bool,
+    ) -> dict:
         """Overwrite a Mimeo Configuration entry.
 
         Recursively finds an entry using `entry_path` list. If any of
         middle entries does not exist, it is initialized as an empty
         dictionary. Once the target entry is found, the `value` is put
         there.
 
         Parameters
         ----------
         config_entry : dict
             A Mimeo Configuration entry to get its direct child
         entry_path : list
             A list of Mimeo Configuration nested properties, e.g.
-            ['output_details', 'direction'] points to the direction
+            ['output', 'direction'] points to the direction
             property under output details entry.
         value
             An overwriting value when `entry_path` contains only one
             element.
 
         Returns
         -------
         config_entry : dict
             An overwritten Mimeo Configuration entry.
         """
         direct_entry = entry_path[0]
         if len(entry_path) > 1:
-            if config_entry.get(direct_entry) is None:
+            if direct_entry not in config_entry:
                 config_entry[direct_entry] = {}
-            config_entry[direct_entry] = cls._overwrite_config_entry(config_entry[direct_entry], entry_path[1:], value)
+            value = cls._overwrite_config_entry(
+                config_entry[direct_entry],
+                entry_path[1:],
+                value)
         else:
-            logger.fine(f"Overwriting {direct_entry} to [{value}]")
-            config_entry[direct_entry] = value
+            logger.fine("Overwriting %s to [%s]", direct_entry, value)
+        config_entry[direct_entry] = value
         return config_entry
 
     @staticmethod
-    def _get_environment(envs_path: str, env_name: str) -> dict:
+    def _get_environment(
+            envs_path: str,
+            env_name: str,
+    ) -> dict:
         """Load an HTTP environment from HTTP envs vile.
 
         Parameters
         ----------
         envs_path : str
             An HTTP envs file path
         env_name : str
@@ -441,23 +497,24 @@
         Returns
         -------
         env : dict
             An HTTP environment configuration
 
         Raises
         ------
-        EnvironmentsFileNotFound
+        EnvironmentsFileNotFoundError
             If environments file does not exist.
-        EnvironmentNotFound
+        EnvironmentNotFoundError
             If the http environment is not defined in the environments file
         """
-        if path.exists(envs_path):
-            with open(envs_path) as envs_file:
-                envs = json.load(envs_file)
-                if env_name in envs:
-                    env = envs[env_name]
-                    logger.debug(f"Using environment [{env_name}] from file [{envs_path}]: [{env}]")
-                    return env
-                else:
-                    raise EnvironmentNotFound(env_name, envs_path)
-        else:
-            raise EnvironmentsFileNotFound(envs_path)
+        if not Path(envs_path).exists():
+            raise EnvironmentsFileNotFoundError(envs_path)
+
+        with Path(envs_path).open() as envs_file:
+            envs = json.load(envs_file)
+            if env_name not in envs:
+                raise EnvironmentNotFoundError(env_name, envs_path)
+
+        env = envs[env_name]
+        logger.debug("Using environment [%s] from file [%s]: [%s]",
+                     env_name, envs_path, env)
+        return env
```

### Comparing `mimeograph-0.4.2/src/mimeo/config/__init__.py` & `mimeograph-0.4.3/src/mimeo/config/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,10 +9,14 @@
 The Mimeo Configuration package exports a class representing
 root Mimeo Configuration component:
 * MimeoConfig
     A MimeoDTO class representing Mimeo Configuration
 
 To use this package, simply import it:
     from mimeo.config import MimeoConfig
-    from mimeo.config.exc import UnsupportedPropertyValue
+    from mimeo.config.exc import UnsupportedPropertyValueError
 """
+from __future__ import annotations
+
 from .mimeo_config import MimeoConfig
+
+__all__ = ["MimeoConfig"]
```

### Comparing `mimeograph-0.4.2/src/mimeo/config/exc.py` & `mimeograph-0.4.3/src/mimeo/config/exc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 """The Mimeo Configuration Exceptions module.
 
 It contains all custom exceptions related to Mimeo Configuration:
-    * UnsupportedPropertyValue
+    * UnsupportedPropertyValueError
         A custom Exception class for unsupported properties' values.
-    * MissingRequiredProperty
+    * MissingRequiredPropertyError
         A custom Exception class for missing required properties.
-    * InvalidIndent
+    * InvalidIndentError
         A custom Exception class for invalid indent configuration.
-    * InvalidVars
+    * InvalidVarsError
         A custom Exception class for invalid vars' configuration.
-    * InvalidMimeoModel
+    * InvalidMimeoModelError
         A custom Exception class for invalid model configuration.
-    * InvalidMimeoTemplate
+    * InvalidMimeoTemplateError
         A custom Exception class for invalid template configuration.
-    * InvalidMimeoConfig
+    * InvalidMimeoConfigError
         A custom Exception class for invalid mimeo configuration.
 """
 
 
-class UnsupportedPropertyValue(Exception):
+from __future__ import annotations
+
+
+class UnsupportedPropertyValueError(Exception):
     """A custom Exception class for unsupported properties' values.
 
     Raised when a Mimeo Configuration property points to a value
     not being supported by Mimeo.
     """
 
-    def __init__(self, prop: str, val: str, supported_values: tuple):
-        """Initialize UnsupportedPropertyValue exception with details.
+    def __init__(
+            self, prop: str, val: str, supported_values: tuple,
+    ):
+        """Initialize UnsupportedPropertyValueError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         prop : str
             A property name
@@ -39,70 +44,63 @@
         supported_values : tuple
             A list of supported values for the property
         """
         super().__init__(f"Provided {prop} [{val}] is not supported! "
                          f"Supported values: [{', '.join(supported_values)}].")
 
 
-class MissingRequiredProperty(Exception):
+class MissingRequiredPropertyError(Exception):
     """A custom Exception class for missing required properties.
 
     Raised when a Mimeo Configuration does not contain a required
     property.
     """
 
-    pass
 
-
-class InvalidIndent(Exception):
+class InvalidIndentError(Exception):
     """A custom Exception class for invalid indent configuration.
 
     Raised when a configured indent is negative.
     """
 
-    def __init__(self, indent: int):
-        """Initialize InvalidIndent exception with details.
+    def __init__(
+            self,
+            indent: int,
+    ):
+        """Initialize InvalidIndentError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         indent : int
             A configured indent
         """
         super().__init__(f"Provided indent [{indent}] is negative!")
 
 
-class InvalidVars(Exception):
+class InvalidVarsError(Exception):
     """A custom Exception class for invalid vars' configuration.
 
     Raised when vars are not configured properly.
     """
 
-    pass
-
 
-class InvalidMimeoModel(Exception):
+class InvalidMimeoModelError(Exception):
     """A custom Exception class for invalid model configuration.
 
     Raised when a Mimeo Model is not configured properly.
     """
 
-    pass
 
-
-class InvalidMimeoTemplate(Exception):
+class InvalidMimeoTemplateError(Exception):
     """A custom Exception class for invalid template configuration.
 
     Raised when a Mimeo Template is not configured properly.
     """
 
-    pass
-
 
-class InvalidMimeoConfig(Exception):
+class InvalidMimeoConfigError(Exception):
     """A custom Exception class for invalid mimeo configuration.
 
     Raised when a Mimeo Configuration is not configured properly.
     """
-
-    pass
```

### Comparing `mimeograph-0.4.2/src/mimeo/consumers/__init__.py` & `mimeograph-0.4.3/src/mimeo/consumers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,7 +32,9 @@
 """
 
 from .consumer import Consumer
 from .file_consumer import FileConsumer
 from .raw_consumer import RawConsumer
 from .http_consumer import HttpConsumer
 from .consumer_factory import ConsumerFactory
+
+__all__ = ["Consumer", "FileConsumer", "RawConsumer", "HttpConsumer", "ConsumerFactory"]
```

### Comparing `mimeograph-0.4.2/src/mimeo/consumers/consumer.py` & `mimeograph-0.4.3/src/mimeo/consumers/consumer.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,34 +18,40 @@
     Methods
     -------
     consume
         Consumes data generated by Mimeo.
     """
 
     @classmethod
-    def __subclasshook__(cls, subclass: Consumer):
+    def __subclasshook__(
+            cls,
+            subclass: Consumer,
+    ):
         """Verify if a subclass implements all abstract methods.
 
         Parameters
         ----------
         subclass : Consumer
             A Consumer subclass
 
         Returns
         -------
         bool
             True if the subclass includes the consume method
         """
-        return 'consume' in subclass.__dict__ and callable(subclass.consume)
+        return "consume" in subclass.__dict__ and callable(subclass.consume)
 
     @abstractmethod
-    def consume(self, data: str):
+    def consume(
+            self,
+            data: str,
+    ):
         """Consume data generated by Mimeo.
 
         It is an abstract method to implement in subclasses
 
         Parameters
         ----------
         data : str
             Stringified data generated by Mimeo
         """
-        pass
+        raise NotImplementedError
```

### Comparing `mimeograph-0.4.2/src/mimeo/consumers/consumer_factory.py` & `mimeograph-0.4.3/src/mimeo/consumers/consumer_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """The Mimeo Consumer Factory module.
 
 It exports only one class:
     * ConsumerFactory
         A Factory class instantiating a Consumer based on Mimeo Config.
 """
-from mimeo.config.exc import UnsupportedPropertyValue
+from __future__ import annotations
+
+from mimeo.config.exc import UnsupportedPropertyValueError
 from mimeo.config.mimeo_config import MimeoConfig
 from mimeo.consumers import Consumer, FileConsumer, HttpConsumer, RawConsumer
 
 
 class ConsumerFactory:
     """A Factory class instantiating a Consumer based on Mimeo Config.
 
@@ -25,41 +27,43 @@
 
     Methods
     -------
     get_consumer(mimeo_config: MimeoConfig) -> Consumer
         Initialize a Consumer based on the Mimeo Output Direction.
     """
 
-    FILE_DIRECTION = MimeoConfig.OUTPUT_DETAILS_DIRECTION_FILE
-    STD_OUT_DIRECTION = MimeoConfig.OUTPUT_DETAILS_DIRECTION_STD_OUT
-    HTTP_DIRECTION = MimeoConfig.OUTPUT_DETAILS_DIRECTION_HTTP
+    FILE_DIRECTION = MimeoConfig.OUTPUT_DIRECTION_FILE
+    STD_OUT_DIRECTION = MimeoConfig.OUTPUT_DIRECTION_STD_OUT
+    HTTP_DIRECTION = MimeoConfig.OUTPUT_DIRECTION_HTTP
 
     @staticmethod
-    def get_consumer(mimeo_config: MimeoConfig) -> Consumer:
+    def get_consumer(
+            mimeo_config: MimeoConfig,
+    ) -> Consumer:
         """Initialize a Consumer based on the Mimeo Output Direction.
 
         Parameters
         ----------
         mimeo_config : MimeoConfig
             A Mimeo Configuration
 
         Returns
         -------
         Consumer
             A Consumer's implementation instance
 
         Raises
         ------
-        UnsupportedPropertyValue
+        UnsupportedPropertyValueError
             If the output direction is not supported
         """
-        direction = mimeo_config.output_details.direction
+        direction = mimeo_config.output.direction
         if direction == ConsumerFactory.STD_OUT_DIRECTION:
             return RawConsumer()
-        elif direction == ConsumerFactory.FILE_DIRECTION:
-            return FileConsumer(mimeo_config.output_details)
-        elif direction == ConsumerFactory.HTTP_DIRECTION:
-            return HttpConsumer(mimeo_config.output_details)
-        else:
-            raise UnsupportedPropertyValue(MimeoConfig.OUTPUT_DETAILS_DIRECTION_KEY,
-                                           direction,
-                                           MimeoConfig.SUPPORTED_OUTPUT_DIRECTIONS)
+        if direction == ConsumerFactory.FILE_DIRECTION:
+            return FileConsumer(mimeo_config.output)
+        if direction == ConsumerFactory.HTTP_DIRECTION:
+            return HttpConsumer(mimeo_config.output)
+        raise UnsupportedPropertyValueError(
+            MimeoConfig.OUTPUT_DIRECTION_KEY,
+            direction,
+            MimeoConfig.SUPPORTED_OUTPUT_DIRECTIONS)
```

### Comparing `mimeograph-0.4.2/src/mimeo/consumers/file_consumer.py` & `mimeograph-0.4.3/src/mimeo/consumers/file_consumer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """The Mimeo File Consumer module.
 
 It exports only one class:
     * FileConsumer
         A Consumer implementation saving data in the filesystem.
 """
+from __future__ import annotations
+
 import logging
 from pathlib import Path
 
-from mimeo.config.mimeo_config import MimeoOutputDetails
+from mimeo.config.mimeo_config import MimeoOutput
 from mimeo.consumers import Consumer
 
 logger = logging.getLogger(__name__)
 
 
 class FileConsumer(Consumer):
     """A Consumer implementation saving data in the filesystem.
@@ -29,42 +31,47 @@
     directory : str
         A directory path to save files within
     output_path_tmplt : str
         An output file path template
         (every file has its index inside the actual path)
     """
 
-    def __init__(self, output_details: MimeoOutputDetails):
+    def __init__(
+            self,
+            output: MimeoOutput,
+    ):
         """Initialize FileConsumer class.
 
         Parameters
         ----------
-        output_details : MimeoOutputDetails
+        output : MimeoOutput
             Configured Mimeo Output Details
         """
-        self.directory = output_details.directory_path
-        self.output_path_tmplt = f"{self.directory}/{output_details.file_name_tmplt}"
-        self.__count = 0
-
-    def consume(self, data: str) -> None:
+        self.directory = output.directory_path
+        self.output_path_tmplt = f"{self.directory}/{output.file_name}"
+        self._count = 0
+
+    def consume(
+            self,
+            data: str,
+    ) -> None:
         """Save data generated by Mimeo into a file.
 
         It is an implementation of Consumer's abstract method.
         If the output directory does not exist it is created.
         Every file name has an index inside its path.
 
         Parameters
         ----------
         data : str
             Stringified data generated by Mimeo
         """
-        logger.fine(f"Consuming data [{data}]")
+        logger.fine("Consuming data [%s]", data)
         if not Path(self.directory).exists():
-            logger.info(f"Creating output directory [{self.directory}]")
+            logger.info("Creating output directory [%s]", self.directory)
             Path(self.directory).mkdir(parents=True, exist_ok=True)
 
-        self.__count += 1
-        file_name = self.output_path_tmplt.format(self.__count)
+        self._count += 1
+        file_name = self.output_path_tmplt.format(self._count)
 
-        logger.info(f"Writing data into file [{file_name}]")
-        with open(file_name, "w") as output_file:
-            output_file.write(data)
+        logger.info("Writing data into file [%s]", file_name)
+        Path(file_name).write_text(data)
```

### Comparing `mimeograph-0.4.2/src/mimeo/consumers/http_consumer.py` & `mimeograph-0.4.3/src/mimeo/consumers/http_consumer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """The Mimeo HTTP Consumer module.
 
 It exports only one class:
     * HttpConsumer
         A Consumer implementation sending data in HTTP requests.
 """
+from __future__ import annotations
+
 import logging
 
 from requests import Response, Session
 from requests.auth import HTTPBasicAuth, HTTPDigestAuth
 
-from mimeo.config.mimeo_config import MimeoOutputDetails
+from mimeo.config.mimeo_config import MimeoOutput
 from mimeo.consumers import Consumer
 
 logger = logging.getLogger(__name__)
 
 
 class HttpConsumer(Consumer):
     """A Consumer implementation sending data in HTTP requests.
@@ -31,63 +33,69 @@
     ----------
     method : str
         An HTTP request method
     url : str
         An URL address to send the HTTP request
     """
 
-    def __init__(self, output_details: MimeoOutputDetails):
+    def __init__(
+            self,
+            output: MimeoOutput,
+    ):
         """Initialize HTTPConsumer class.
 
         Parameters
         ----------
-        output_details : MimeoOutputDetails
+        output : MimeoOutput
             Configured Mimeo Output Details
         """
-        self.method = output_details.method
-        self.url = HttpConsumer.__build_url(output_details)
-        if output_details.auth == "basic":
-            self.__auth = HTTPBasicAuth(output_details.username, output_details.password)
-        else:
-            self.__auth = HTTPDigestAuth(output_details.username, output_details.password)
-
-    def consume(self, data: str) -> Response:
+        self.method = output.method
+        self.url = HttpConsumer.__build_url(output)
+        auth_impl = HTTPBasicAuth if output.auth == "basic" else HTTPDigestAuth
+        self.__auth = auth_impl(output.username, output.password)
+
+    def consume(
+            self,
+            data: str,
+    ) -> Response:
         """Send data generated by Mimeo in an HTTP request.
 
         It is an implementation of Consumer's abstract method.
 
         Parameters
         ----------
         data : str
             Stringified data generated by Mimeo
         """
-        logger.fine(f"Consuming data [{data}]")
+        logger.fine("Consuming data [%s]", data)
         with Session() as sess:
-            logger.info(f"Sending request {self.method} {self.url}")
-            return sess.request(self.method,
-                                self.url,
-                                auth=self.__auth,
-                                data=data,
-                                headers={"Content-Type": "application/xml"})
+            logger.info("Sending request %s %s", self.method, self.url)
+            return sess.request(
+                self.method,
+                self.url,
+                auth=self.__auth,
+                data=data,
+                headers={"Content-Type": "application/xml"})
 
     @staticmethod
-    def __build_url(output_details: MimeoOutputDetails) -> str:
+    def __build_url(
+            output: MimeoOutput,
+    ) -> str:
         """Build a URL based on Mimeo Output Details.
 
         It populates a URL template using configured output details.
         When port is not configured - it uses host and endpoint values.
         Otherwise, host is followed by the colon and port.
 
         Parameters
         ----------
-        output_details : MimeoOutputDetails
+        output : MimeoOutput
             Configured Mimeo Output Details
 
         Returns
         -------
         str
             A valid URL address
         """
-        if output_details.port is None:
-            return f"{output_details.protocol}://{output_details.host}{output_details.endpoint}"
-        else:
-            return f"{output_details.protocol}://{output_details.host}:{output_details.port}{output_details.endpoint}"
+        if output.port is None:
+            return f"{output.protocol}://{output.host}{output.endpoint}"
+        return f"{output.protocol}://{output.host}:{output.port}{output.endpoint}"
```

### Comparing `mimeograph-0.4.2/src/mimeo/consumers/raw_consumer.py` & `mimeograph-0.4.3/src/mimeo/consumers/raw_consumer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """The Mimeo Raw Consumer module.
 
 It exports only one class:
     * RawConsumer
         A Consumer implementation printing data in the standard output.
 """
+from __future__ import annotations
+
 from mimeo.consumers import Consumer
 
 
 class RawConsumer(Consumer):
     """A Consumer implementation printing data in the standard output.
 
     This Consumer is instantiated for the 'stdout' output direction
@@ -15,15 +17,18 @@
 
     Methods
     -------
     consume
         Print data generated in the standard output.
     """
 
-    def consume(self, data: str) -> None:
+    def consume(
+            self,
+            data: str,
+    ) -> None:
         """Print data generated in the standard output.
 
         It is an implementation of Consumer's abstract method.
 
         Parameters
         ----------
         data : str
```

### Comparing `mimeograph-0.4.2/src/mimeo/context/__init__.py` & `mimeograph-0.4.3/src/mimeo/context/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,7 +24,9 @@
 
 To use this package, simply import the desired class:
     from mimeo.context import MimeoContextManager
 """
 from .mimeo_iteration import MimeoIteration
 from .mimeo_context import MimeoContext
 from .mimeo_context_manager import MimeoContextManager
+
+__all__ = ["MimeoIteration", "MimeoContext", "MimeoContextManager"]
```

### Comparing `mimeograph-0.4.2/src/mimeo/context/decorators.py` & `mimeograph-0.4.3/src/mimeo/context/decorators.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,22 +8,26 @@
     Decorator switching context before and after function's call
 - @mimeo_next_iteration:
     Decorator incrementing current context's iteration
 - @mimeo_clear_iterations:
     Decorator clearing iterations of the current context
 
 """
+from __future__ import annotations
+
 import functools
 from typing import Callable
 
 from mimeo.config.mimeo_config import MimeoTemplate
 from mimeo.context import MimeoContext, MimeoContextManager
 
 
-def mimeo_context(func: Callable) -> Callable:
+def mimeo_context(
+        func: Callable,
+) -> Callable:
     """Provide a 'context' parameter to a function.
 
     It can be used only for functions having defined a 'context'
     parameter. In case the function being decorated is called providing
     this param, decorator simply calls it without any modification.
     Otherwise - and this is the main purpose of the @mimeo_context
     decorator - it provides the current Mimeo Context.
@@ -36,25 +40,31 @@
     Returns
     -------
     inject_context : Callable
         The decorated function
     """
 
     @functools.wraps(func)
-    def inject_context(*args, **kwargs):
+    def inject_context(
+            *args,
+            **kwargs,
+    ):
         if any(isinstance(arg, MimeoContext) for arg in args) or "context" in kwargs:
             result = func(*args, **kwargs)
         else:
-            result = func(*args, **kwargs, context=MimeoContextManager().get_current_context())
+            current_ctx = MimeoContextManager().get_current_context()
+            result = func(*args, **kwargs, context=current_ctx)
         return result
 
     return inject_context
 
 
-def mimeo_context_switch(func: Callable) -> Callable:
+def mimeo_context_switch(
+        func: Callable,
+) -> Callable:
     """Switch context before and after function's call.
 
     It can be used only for functions having defined a MimeoTemplate
     parameter. It switches a Mimeo Context to the one defined in
     Mimeo Template, and after the function's being decorated call
     switches back to the previous one. It helps to handle nested
     Mimeo Templates. This decorator meant to be used for
@@ -68,15 +78,18 @@
     Returns
     -------
     switch_context : Callable
         The decorated function
     """
 
     @functools.wraps(func)
-    def switch_context(*args, **kwargs):
+    def switch_context(
+            *args,
+            **kwargs,
+    ):
         context_mng = MimeoContextManager()
         prev_context = context_mng.get_current_context()
 
         if "template" in kwargs:
             template = kwargs["template"]
         else:
             template = next(arg for arg in args if isinstance(arg, MimeoTemplate))
@@ -87,15 +100,17 @@
 
         context_mng.set_current_context(prev_context)
         return result
 
     return switch_context
 
 
-def mimeo_next_iteration(func):
+def mimeo_next_iteration(
+        func: Callable,
+):
     """Increment current context's iteration.
 
     It is meant to be used for Generator's function that
     generates a single data copy.
 
     Parameters
     ----------
@@ -105,23 +120,27 @@
     Returns
     -------
     next_iteration : Callable
         The decorated function
     """
 
     @functools.wraps(func)
-    def next_iteration(*args, **kwargs):
+    def next_iteration(
+            *args,
+            **kwargs,
+    ):
         MimeoContextManager().get_current_context().next_iteration()
-        result = func(*args, **kwargs)
-        return result
+        return func(*args, **kwargs)
 
     return next_iteration
 
 
-def mimeo_clear_iterations(func):
+def mimeo_clear_iterations(
+        func: Callable,
+):
     """Clear iterations of the current context.
 
     It is meant to be used for Generator's function that generates
     data from a template.
 
     Parameters
     ----------
@@ -131,13 +150,15 @@
     Returns
     -------
     clear_iterations : Callable
         The decorated function
     """
 
     @functools.wraps(func)
-    def clear_iterations(*args, **kwargs):
+    def clear_iterations(
+            *args,
+            **kwargs,
+    ):
         MimeoContextManager().get_current_context().clear_iterations()
-        result = func(*args, **kwargs)
-        return result
+        return func(*args, **kwargs)
 
     return clear_iterations
```

### Comparing `mimeograph-0.4.2/src/mimeo/context/exc.py` & `mimeograph-0.4.3/src/mimeo/context/exc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,148 +1,172 @@
 """The Mimeo Context Exceptions module.
 
 It contains all custom exceptions related to Mimeo Context:
-    * MinimumIdentifierReached
+    * MinimumIdentifierReachedError
         A custom Exception class for reaching minimum identifier.
-    * UninitializedContextIteration
+    * UninitializedContextIterationError
         A custom Exception class for uninitialized context's iteration.
-    * ContextIterationNotFound
+    * ContextIterationNotFoundError
         A custom Exception class for not found context's iteration.
-    * InvalidSpecialFieldName
+    * InvalidSpecialFieldNameError
         A custom Exception class for invalid special field's name.
-    * InvalidSpecialFieldValue
+    * InvalidSpecialFieldValueError
         A custom Exception class for invalid special field's value.
-    * SpecialFieldNotFound
+    * SpecialFieldNotFoundError
         A custom Exception class for not found special field.
-    * VarNotFound
+    * VarNotFoundError
         A custom Exception class for not found var.
 """
-from typing import Union
+from __future__ import annotations
 
 
-class MinimumIdentifierReached(Exception):
+class MinimumIdentifierReachedError(Exception):
     """A custom Exception class for reaching minimum identifier.
 
     Raised when using MimeoContext.prev_id() method and id is equal to
     0.
     """
 
-    def __init__(self):
-        """Initialize MinimumIdentifierReached exception with details.
+    def __init__(
+            self,
+    ):
+        """Initialize MinimumIdentifierReachedError exception with details.
 
         Extends Exception constructor with a constant message.
         """
         super().__init__("There's no previous ID!")
 
 
-class UninitializedContextIteration(Exception):
+class UninitializedContextIterationError(Exception):
     """A custom Exception class for uninitialized context's iteration.
 
     Raised while attempting to access the current iteration without
     prior initialization.
     """
 
-    def __init__(self, context_name: str):
-        """Initialize UninitializedContextIteration exception with details.
+    def __init__(
+            self,
+            context_name: str,
+    ):
+        """Initialize UninitializedContextIterationError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         context_name : str
             A current context name
         """
-        super().__init__(f"No iteration has been initialized for the current context [{context_name}]")
+        msg = ("No iteration has been initialized "
+               f"for the current context [{context_name}]")
+        super().__init__(msg)
 
 
-class ContextIterationNotFound(Exception):
+class ContextIterationNotFoundError(Exception):
     """A custom Exception class for not found context's iteration.
 
     Raised while attempting to access an iteration that does not exist.
     """
 
-    def __init__(self, iteration_id: int, context_name: str):
-        """Initialize ContextIterationNotFound exception with details.
+    def __init__(
+            self,
+            iteration_id: int,
+            context_name: str,
+    ):
+        """Initialize ContextIterationNotFoundError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         iteration_id : int
             A current context name
         context_name : str
             A current context name
         """
-        super().__init__(f"No iteration with id [{iteration_id}] "
-                         f"has been initialized for the current context [{context_name}]")
+        msg = (f"No iteration with id [{iteration_id}] "
+               f"has been initialized for the current context [{context_name}]")
+        super().__init__(msg)
 
 
-class InvalidSpecialFieldName(Exception):
+class InvalidSpecialFieldNameError(Exception):
     """A custom Exception class for invalid special field's name.
 
     Raised while attempting to save a special field and provided name
     is not a string value.
     """
 
-    def __init__(self):
-        """Initialize InvalidSpecialFieldName exception with details.
+    def __init__(
+            self,
+    ):
+        """Initialize InvalidSpecialFieldNameError exception with details.
 
         Extends Exception constructor with a constant message.
         """
         super().__init__("A special field name needs to be a string value!")
 
 
-class InvalidSpecialFieldValue(Exception):
+class InvalidSpecialFieldValueError(Exception):
     """A custom Exception class for invalid special field's value.
 
     Raised while attempting to save a special field and provided value
     is non-atomic one.
     """
 
-    def __init__(self, field_value: Union[dict, list]):
-        """Initialize InvalidSpecialFieldValue exception with details.
+    def __init__(
+            self,
+            field_value: dict | list,
+    ):
+        """Initialize InvalidSpecialFieldValueError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
-        field_value : Union[str, int, bool]
+        field_value : dict | list
             A special field value
         """
-        super().__init__(f"Provided field value [{field_value}] is invalid (use any atomic value)!")
+        msg = f"Provided field value [{field_value}] is invalid (use any atomic value)!"
+        super().__init__(msg)
 
 
-class SpecialFieldNotFound(Exception):
+class SpecialFieldNotFoundError(Exception):
     """A custom Exception class for not found special field.
 
     Raised while attempting to access a special field that does not
     exist.
     """
 
-    def __init__(self, field_name: str):
-        """Initialize SpecialFieldNotFound exception with details.
+    def __init__(
+            self,
+            field_name: str,
+    ):
+        """Initialize SpecialFieldNotFoundError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         field_name : str
             A special field name
         """
         super().__init__(f"Special Field [{field_name}] has not been found!")
 
 
-class VarNotFound(Exception):
+class VarNotFoundError(Exception):
     """A custom Exception class for not found var.
 
     Raised while attempting to access a variable that does not exist.
     """
 
-    def __init__(self, variable_name: str):
-        """Initialize VarNotFound exception with details.
+    def __init__(
+            self,
+            variable_name: str,
+    ):
+        """Initialize VarNotFoundError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         variable_name : str
             A variable name
```

### Comparing `mimeograph-0.4.2/src/mimeo/context/mimeo_context.py` & `mimeograph-0.4.3/src/mimeo/context/mimeo_context.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """The Mimeo Context module.
 
 It exports only one class:
     * MimeoContext
         A class managing Mimeo-Template-dependent utilities.
 """
+from __future__ import annotations
+
 import random
 
 from mimeo.context import MimeoIteration
-from mimeo.context.exc import (ContextIterationNotFound,
-                               MinimumIdentifierReached,
-                               UninitializedContextIteration)
+from mimeo.context.exc import (ContextIterationNotFoundError,
+                               MinimumIdentifierReachedError,
+                               UninitializedContextIterationError)
 from mimeo.database import MimeoDB
-from mimeo.database.exc import DataNotFound, OutOfStock
+from mimeo.database.exc import DataNotFoundError, OutOfStockError
 
 
 class MimeoContext:
     """A class managing Mimeo-Template-dependent utilities.
 
     It allows you to reach a specific iteration of a template
     generation, and ensures uniqueness of all values generated
@@ -55,15 +57,18 @@
         Provide next unique last name index.
     """
 
     _ALL = "_ALL_"
     _INITIAL_COUNT = "init-count"
     _INDEXES = "indexes"
 
-    def __init__(self, name: str):
+    def __init__(
+            self,
+            name: str,
+    ):
         """Initialize MimeoContext class.
 
         Parameters
         ----------
         name : str
             A context name
         """
@@ -71,126 +76,143 @@
         self._id = 0
         self._iterations = []
         self._countries_indexes = None
         self._cities_indexes = {}
         self._first_names_indexes = {}
         self._last_names_indexes = None
 
-    def next_id(self) -> int:
+    def next_id(
+            self,
+    ) -> int:
         """Increment an identifier and return the current (incremented) one.
 
         Identifier is used by Auto Increment Mimeo Util.
 
         Returns
         -------
         int
             A next identifier within the context
         """
         self._id += 1
         return self.curr_id()
 
-    def curr_id(self) -> int:
+    def curr_id(
+            self,
+    ) -> int:
         """Return the current identifier within the context.
 
         Identifier is used by Auto Increment Mimeo Util.
 
         Returns
         -------
         int
             The current identifier within the context
         """
         return self._id
 
-    def prev_id(self) -> int:
+    def prev_id(
+            self,
+    ) -> int:
         """Decrement an identifier and return the current (decremented) one.
 
         Identifier is used by Auto Increment Mimeo Util.
         This method is meant to be used when an error appear
         after incrementation.
 
         Returns
         -------
         int
             A previous identifier within the context
 
         Raises
         ------
-        MinimumIdentifierReached
+        MinimumIdentifierReachedError
             If the current identifier (before decrement) equals 0
         """
-        if self._id > 0:
-            self._id -= 1
-            return self.curr_id()
-        else:
-            raise MinimumIdentifierReached()
+        if self._id == 0:
+            raise MinimumIdentifierReachedError
+        self._id -= 1
+        return self.curr_id()
 
-    def next_iteration(self) -> MimeoIteration:
+    def next_iteration(
+            self,
+    ) -> MimeoIteration:
         """Initialize a next iteration within the context.
 
         To initialize the iteration, it gets the last iteration id and
         provides its incrementation.
 
         Returns
         -------
         next_iteration : MimeoIteration
             The initialized iteration
         """
-        next_iteration_id = 1 if len(self._iterations) == 0 else self._iterations[-1].id + 1
+        if len(self._iterations) == 0:
+            next_iteration_id = 1
+        else:
+            next_iteration_id = self._iterations[-1].id + 1
         next_iteration = MimeoIteration(next_iteration_id)
         self._iterations.append(next_iteration)
         return next_iteration
 
-    def curr_iteration(self) -> MimeoIteration:
+    def curr_iteration(
+            self,
+    ) -> MimeoIteration:
         """Return the current iteration within the context.
 
         Returns
         -------
         int
             The current iteration within the context
 
         Raises
         ------
-        UninitializedContextIteration
+        UninitializedContextIterationError
             If no iteration has been initialized yet for the context
         """
-        if len(self._iterations) > 0:
-            return self._iterations[-1]
-        else:
-            raise UninitializedContextIteration(self.name)
-
-    def get_iteration(self, iteration_id: int) -> MimeoIteration:
+        if len(self._iterations) == 0:
+            raise UninitializedContextIterationError(self.name)
+        return self._iterations[-1]
+
+    def get_iteration(
+            self,
+            iteration_id: int,
+    ) -> MimeoIteration:
         """Return a specific iteration from the context.
 
         Returns
         -------
         int
             A specific iteration
 
         Raises
         ------
-        ContextIterationNotFound
+        ContextIterationNotFoundError
             If the context does not have an iteration with the id
             provided
         """
         iteration = next(filter(lambda i: i.id == iteration_id, self._iterations), None)
-        if iteration is not None:
-            return iteration
-        else:
-            raise ContextIterationNotFound(iteration_id, self.name)
-
-    def clear_iterations(self):
+        if iteration is None:
+            raise ContextIterationNotFoundError(iteration_id, self.name)
+        return iteration
+
+    def clear_iterations(
+            self,
+    ):
         """Clear out all context iterations.
 
         This method is meant to be used in case of nested templates.
         Thanks to iteration reset the nested template is properly
         generated in context of the next parent template's iteration.
         """
         self._iterations = []
 
-    def next_country_index(self) -> int:
+    def next_country_index(
+            self,
+    ) -> int:
         """Provide next unique country index.
 
         When used for the first time in the specific context
         it populates internal countries' indexes list. This approach
         ensures country uniqueness without time-consuming operations.
         Each time it verifies if the internal list still contains some
         indexes.
@@ -200,23 +222,26 @@
         Returns
         -------
         int
             Next unique country identifier
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all countries' indexes have been consumed already
         """
         self._initialize_countries_indexes()
         self._validate_countries()
 
         return self._countries_indexes.pop()
 
-    def next_city_index(self, country: str = None) -> int:
+    def next_city_index(
+            self,
+            country: str = None,
+    ) -> int:
         """Provide next unique city index.
 
         When used for the first time in the specific context
         it populates internal cities' indexes map. Each `country` key
         has its own list initialized as same as country-agnostic one.
         This approach ensures city uniqueness without time-consuming
         operations. Each time it verifies if the internal list still
@@ -236,24 +261,27 @@
             Next unique city identifier
 
         Raises
         ------
         CountryNotFound
             If database does not contain any cities for the provided
             `country`
-        OutOfStock
+        OutOfStockError
             If all cities' indexes have been consumed already
         """
         country = country if country is not None else MimeoContext._ALL
         self._initialize_cities_indexes(country)
         self._validate_cities(country)
 
         return self._cities_indexes[country][MimeoContext._INDEXES].pop()
 
-    def next_first_name_index(self, sex: str = None) -> int:
+    def next_first_name_index(
+            self,
+            sex: str = None,
+    ) -> int:
         """Provide next unique first name index.
 
         When used for the first time in the specific context
         it populates internal first names' indexes map. Each `sex` key
         has its own list initialized as same as sex-agnostic one.
         This approach ensures forename uniqueness without
         time-consuming operations. Each time it verifies if the internal
@@ -270,26 +298,28 @@
         Returns
         -------
         int
             Next unique first name identifier
 
         Raises
         ------
-        InvalidSex
+        InvalidSexError
             If `sex` is not 'M' nor 'F' value
-        OutOfStock
+        OutOfStockError
             If all first names' indexes have been consumed already
         """
         sex = sex if sex is not None else MimeoContext._ALL
         self._initialize_first_names_indexes(sex)
         self._validate_first_names(sex)
 
         return self._first_names_indexes[sex][MimeoContext._INDEXES].pop()
 
-    def next_last_name_index(self) -> int:
+    def next_last_name_index(
+            self,
+    ) -> int:
         """Provide next unique last name index.
 
         When used for the first time in the specific context
         it populates internal last names' indexes list. This approach
         ensures surnames uniqueness without time-consuming operations.
         Each time it verifies if the internal list still contains some
         indexes.
@@ -299,33 +329,39 @@
         Returns
         -------
         int
             Next unique last name identifier
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all last names' indexes have been consumed already
         """
         self._initialize_last_names_indexes()
         self._validate_last_names()
 
         return self._last_names_indexes.pop()
 
-    def _initialize_countries_indexes(self):
+    def _initialize_countries_indexes(
+            self,
+    ):
         """Initialize countries' indexes with unique integers.
 
         The list length and range depends on the number of country
         records in database.
         """
         if self._countries_indexes is None:
-            countries_indexes = random.sample(range(MimeoDB.NUM_OF_COUNTRIES), MimeoDB.NUM_OF_COUNTRIES)
+            num_of_entries = MimeoDB.NUM_OF_COUNTRIES
+            countries_indexes = random.sample(range(num_of_entries), num_of_entries)
             self._countries_indexes = countries_indexes
 
-    def _initialize_cities_indexes(self, country: str):
+    def _initialize_cities_indexes(
+            self,
+            country: str,
+    ):
         """Initialize cities' indexes with unique integers.
 
         The list length and range depends on the number of city
         records in database for the `country`.
 
         Raises
         ------
@@ -336,101 +372,129 @@
         if country not in self._cities_indexes:
             if country == MimeoContext._ALL:
                 num_of_entries = MimeoDB.NUM_OF_CITIES
             else:
                 country_cities = MimeoDB().get_cities_of(country)
                 num_of_entries = len(country_cities)
                 if num_of_entries == 0:
-                    raise DataNotFound(f"Mimeo database does not contain any cities of provided country [{country}].")
+                    msg = (f"Mimeo database doesn't contain any cities "
+                           f"of provided country [{country}].")
+                    raise DataNotFoundError(msg)
 
             cities_indexes = random.sample(range(num_of_entries), num_of_entries)
             self._cities_indexes[country] = {
                 MimeoContext._INITIAL_COUNT: num_of_entries,
-                MimeoContext._INDEXES: cities_indexes
+                MimeoContext._INDEXES: cities_indexes,
             }
 
-    def _initialize_first_names_indexes(self, sex: str):
+    def _initialize_first_names_indexes(
+            self,
+            sex: str,
+    ):
         """Initialize first names' indexes with integers.
 
         The list length and range depends on the number of first name
         records in database for the `sex`.
 
         Raises
         ------
-        InvalidSex
+        InvalidSexError
             If `sex` is not 'M' nor 'F' value
         """
         if sex not in self._first_names_indexes:
             if sex == MimeoContext._ALL:
                 num_of_entries = MimeoDB.NUM_OF_FIRST_NAMES
             else:
                 first_names_for_sex = MimeoDB().get_first_names_by_sex(sex)
                 num_of_entries = len(first_names_for_sex)
 
             first_names_indexes = random.sample(range(num_of_entries), num_of_entries)
             self._first_names_indexes[sex] = {
                 MimeoContext._INITIAL_COUNT: num_of_entries,
-                MimeoContext._INDEXES: first_names_indexes
+                MimeoContext._INDEXES: first_names_indexes,
             }
 
-    def _initialize_last_names_indexes(self):
+    def _initialize_last_names_indexes(
+            self,
+    ):
         """Initialize last names' indexes with unique integers.
 
         The list length and range depends on the number of last name
         records in database.
         """
         if self._last_names_indexes is None:
-            last_names_indexes = random.sample(range(MimeoDB.NUM_OF_LAST_NAMES), MimeoDB.NUM_OF_LAST_NAMES)
+            num_of_entries = MimeoDB.NUM_OF_LAST_NAMES
+            last_names_indexes = random.sample(range(num_of_entries), num_of_entries)
             self._last_names_indexes = last_names_indexes
 
-    def _validate_countries(self):
+    def _validate_countries(
+            self,
+    ):
         """Verify if all countries' indexes have been consumed.
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all countries' indexes have been consumed already
         """
         if len(self._countries_indexes) == 0:
-            raise OutOfStock(f"No more unique values, database contain only {MimeoDB.NUM_OF_COUNTRIES} countries.")
-
-    def _validate_cities(self, country: str):
+            msg = (f"No more unique values, "
+                   f"database contain only {MimeoDB.NUM_OF_COUNTRIES} countries.")
+            raise OutOfStockError(msg)
+
+    def _validate_cities(
+            self,
+            country: str,
+    ):
         """Verify if all cities' indexes have been consumed.
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all cities' indexes have been consumed already
         """
         if len(self._cities_indexes[country][MimeoContext._INDEXES]) == 0:
             init_count = self._cities_indexes[country][MimeoContext._INITIAL_COUNT]
             if country == MimeoContext._ALL:
-                raise OutOfStock(f"No more unique values, database contain only {init_count} cities.")
+                msg = (f"No more unique values, "
+                       f"database contain only {init_count} cities.")
             else:
-                raise OutOfStock(f"No more unique values, database contain only {init_count} cities of {country}.")
-
-    def _validate_first_names(self, sex: str):
+                msg = (f"No more unique values, "
+                       f"database contain only {init_count} cities of {country}.")
+            raise OutOfStockError(msg)
+
+    def _validate_first_names(
+            self,
+            sex: str,
+    ):
         """Verify if all first names' indexes have been consumed.
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all first names' indexes have been consumed already
         """
         if len(self._first_names_indexes[sex][MimeoContext._INDEXES]) == 0:
             init_count = self._first_names_indexes[sex][MimeoContext._INITIAL_COUNT]
             if sex == MimeoContext._ALL:
-                raise OutOfStock(f"No more unique values, database contain only {init_count} first names.")
+                msg = (f"No more unique values, "
+                       f"database contain only {init_count} first names.")
             else:
-                raise OutOfStock(f"No more unique values, database contain only {init_count} "
-                                 f"{'male' if sex == 'M' else 'female'} first names.")
-
-    def _validate_last_names(self):
+                sex_info = "male" if sex == "M" else "female"
+                msg = (f"No more unique values, "
+                       f"database contain only {init_count} {sex_info} first names.")
+            raise OutOfStockError(msg)
+
+    def _validate_last_names(
+            self,
+    ):
         """Verify if all last names' indexes have been consumed.
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all last names' indexes have been consumed already
         """
         if len(self._last_names_indexes) == 0:
-            raise OutOfStock(f"No more unique values, database contain only {MimeoDB.NUM_OF_LAST_NAMES} last names.")
+            msg = (f"No more unique values, "
+                   f"database contain only {MimeoDB.NUM_OF_LAST_NAMES} last names.")
+            raise OutOfStockError(msg)
```

### Comparing `mimeograph-0.4.2/src/mimeo/context/mimeo_context_manager.py` & `mimeograph-0.4.3/src/mimeo/context/mimeo_context_manager.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 It exports only one class:
     * MimeoContextManager
         An OnlyOneAlive class managing Mimeo Contexts.
 """
 from __future__ import annotations
 
-from typing import Union
+from types import TracebackType
 
 from mimeo.config import MimeoConfig
 from mimeo.context import MimeoContext
-from mimeo.context.exc import VarNotFound
+from mimeo.context.exc import VarNotFoundError
 from mimeo.meta import Alive, OnlyOneAlive
 
 
 class MimeoContextManager(Alive, metaclass=OnlyOneAlive):
     """An OnlyOneAlive class managing Mimeo Contexts.
 
     It allows you to initialize a context, get the currently processing
@@ -32,68 +32,80 @@
         Return the current Mimeo Context.
     set_current_context(self, context: MimeoContext)
         Set the current Mimeo Context.
     get_var(self, variable_name: str)
         Return a specific Mimeo Var value.
     """
 
-    def __init__(self, mimeo_config: MimeoConfig = None):
+    def __init__(
+            self,
+            mimeo_config: MimeoConfig = None,
+    ):
         """Initialize MimeoContextManager class.
 
         Parameters
         ----------
         mimeo_config : MimeoConfig
             The Mimeo Configuration
         """
         super().__init__()
         self._mimeo_config = mimeo_config
         self._vars = {}
         self._contexts = {}
         self._current_context = None
 
-    def __enter__(self) -> MimeoContextManager:
+    def __enter__(
+            self,
+    ) -> MimeoContextManager:
         """Enter the MimeoContextManager instance.
 
         Extends Alive __enter__ function and initializes vars.
 
         Returns
         -------
         self : MimeoContextManager
             A MimeoContextManager instance
         """
         super().__enter__()
         self._vars = self._mimeo_config.vars
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(
+            self,
+            exc_type: type | None,
+            exc_val: BaseException | None,
+            exc_tb: TracebackType | None,
+    ) -> None:
         """Exit the MimeoContextManager instance.
 
         Extends Alive __enter__ function and removes internal
         attributes.
 
         Parameters
         ----------
-        exc_type
+        exc_type : type | None
             An exception's type
-        exc_val
+        exc_val : BaseException | None
             An exception's value
-        exc_tb
+        exc_tb  TracebackType | None
             An exception's traceback
 
         Returns
         -------
         None
             A None value
         """
         super().__exit__(exc_type, exc_val, exc_tb)
         self._vars = None
         self._contexts = None
-        return None
 
-    def get_context(self, context: str) -> MimeoContext:
+    def get_context(
+            self,
+            context: str,
+    ) -> MimeoContext:
         """Return a Mimeo Context with a specific name.
 
         If the context does not exist, it is initialized.
 
         Parameters
         ----------
         context : str
@@ -110,15 +122,17 @@
             If the MimeoContextManager instance is not alive
         """
         super().assert_alive()
         if context not in self._contexts:
             self._contexts[context] = MimeoContext(context)
         return self._contexts[context]
 
-    def get_current_context(self) -> MimeoContext:
+    def get_current_context(
+            self,
+    ) -> MimeoContext:
         """Return the current Mimeo Context.
 
         Returns
         -------
         MimeoContext
             The current Mimeo Context
 
@@ -126,15 +140,18 @@
         ------
         InstanceNotAlive
             If the MimeoContextManager instance is not alive
         """
         super().assert_alive()
         return self._current_context
 
-    def set_current_context(self, context: MimeoContext):
+    def set_current_context(
+            self,
+            context: MimeoContext,
+    ):
         """Set the current Mimeo Context.
 
         Parameters
         ----------
         context : MimeoContext
             A Mimeo Context to be set as the current one
 
@@ -142,34 +159,36 @@
         ------
         InstanceNotAlive
             If the MimeoContextManager instance is not alive
         """
         super().assert_alive()
         self._current_context = context
 
-    def get_var(self, variable_name: str) -> Union[str, int, bool, dict]:
+    def get_var(
+            self,
+            variable_name: str,
+    ) -> str | int | bool | dict:
         """Return a specific Mimeo Var value.
 
         Parameters
         ----------
         variable_name : str
             The Mimeo Var name
 
         Returns
         -------
-        value : Union[str, int, bool, dict]
+        value : str | int | bool | dict
             The Mimeo Var value
 
         Raises
         ------
         InstanceNotAlive
             If the MimeoContextManager instance is not alive
-        VarNotFound
+        VarNotFoundError
             If the Mimeo Var with the `variable_name` provided does not
             exist
         """
         super().assert_alive()
         value = self._vars.get(variable_name)
-        if value is not None:
-            return value
-        else:
-            raise VarNotFound(variable_name)
+        if value is None:
+            raise VarNotFoundError(variable_name)
+        return value
```

### Comparing `mimeograph-0.4.2/src/mimeo/context/mimeo_iteration.py` & `mimeograph-0.4.3/src/mimeo/context/mimeo_iteration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """The Mimeo Iteration module.
 
 It exports only one class:
     * MimeoIteration
         A class representing a single iteration in a Mimeo Template.
 """
+from __future__ import annotations
+
 import uuid
-from typing import Union
 
-from mimeo.context.exc import (InvalidSpecialFieldName,
-                               InvalidSpecialFieldValue, SpecialFieldNotFound)
+from mimeo.context.exc import (InvalidSpecialFieldNameError,
+                               InvalidSpecialFieldValueError,
+                               SpecialFieldNotFoundError)
 
 
 class MimeoIteration:
     """A class representing a single iteration in a Mimeo Template.
 
     Each iteration has its own id (an ordinal number in a context),
     a key being a unique value across all iterations, and
@@ -23,71 +25,81 @@
     id : int
         An ordinal number in a Mimeo Context
     key : str
         An UUID value unique across all templates
 
     Methods
     -------
-    add_special_field(self, field_name: str, field_value: Union[str, int, bool])
+    add_special_field(self, field_name: str, field_value: str | int | bool)
         Put a special field entry to memory.
-    get_special_field(self, field_name: str) -> Union[str, int, bool]
+    get_special_field(self, field_name: str) -> str | int | bool]
         Get a special field value from memory.
     """
 
-    def __init__(self, identifier: int):
+    def __init__(
+            self,
+            identifier: int,
+    ):
         """Initialize MimeoIteration class.
 
         Parameters
         ----------
         identifier : int
             An ordinal number in a Mimeo Context
         """
         self.id = identifier
         self.key = str(uuid.uuid4())
         self._special_fields = {}
 
-    def add_special_field(self, field_name: str, field_value: Union[str, int, bool]):
+    def add_special_field(
+            self,
+            field_name: str,
+            field_value: str | int | bool,
+    ):
         """Put a special field entry to memory.
 
         Parameters
         ----------
         field_name : str
             A special field name
-        field_value : Union[str, int, bool]
+        field_value : str | int | bool
             A special field value
 
         Raises
         ------
-        InvalidSpecialFieldName
+        InvalidSpecialFieldNameError
             If the special field name is not a string
-        InvalidSpecialFieldValue
+        InvalidSpecialFieldValueError
             If the special field value is dict or list
         """
         if not isinstance(field_name, str):
-            raise InvalidSpecialFieldName()
-        if isinstance(field_value, dict) or isinstance(field_value, list):
-            raise InvalidSpecialFieldValue(field_value)
+            raise InvalidSpecialFieldNameError
+        if isinstance(field_value, (dict, list)):
+            raise InvalidSpecialFieldValueError(field_value)
 
         self._special_fields[field_name] = field_value
 
-    def get_special_field(self, field_name: str) -> Union[str, int, bool]:
+    def get_special_field(
+            self,
+            field_name: str,
+    ) -> str | int | bool:
         """Get a special field value from memory.
 
         Parameters
         ----------
         field_name : str
             A special field name
 
         Returns
         -------
-        Union[str, int, bool]
+        str | int | bool
             A special field value
 
         Raises
         ------
-        SpecialFieldNotFound
+        SpecialFieldNotFoundError
             If the special field does not exist.
         """
         if field_name not in self._special_fields:
-            raise SpecialFieldNotFound(field_name)
+            raise SpecialFieldNotFoundError(field_name)
 
         return self._special_fields.get(field_name)
```

### Comparing `mimeograph-0.4.2/src/mimeo/database/__init__.py` & `mimeograph-0.4.3/src/mimeo/database/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,27 @@
 * Country
     DTO class representing a single row in countries CSV data.
 * FirstName
     DTO class representing a single row in forenames CSV data.
 
 To use this package, simply import the desired class:
     from mimeo.database import MimeoDB
-    from mimeo.database.exc import DataNotFound
+    from mimeo.database.exc import DataNotFoundError
 """
+from __future__ import annotations
+
 from .cities import CitiesDB, City
 from .countries import CountriesDB, Country
 from .first_names import FirstName, FirstNamesDB
 from .last_names import LastNamesDB
 from .mimeo_db import MimeoDB
+
+__all__ = [
+    "City",
+    "Country",
+    "FirstName",
+    "CitiesDB",
+    "CountriesDB",
+    "FirstNamesDB",
+    "LastNamesDB",
+    "MimeoDB",
+]
```

### Comparing `mimeograph-0.4.2/src/mimeo/database/cities.py` & `mimeograph-0.4.3/src/mimeo/database/cities.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 It exports classes related to cities CSV data:
     * City
         DTO class representing a single row in cities CSV data.
     * CitiesDB
         Class exposing READ operations on cities CSV data.
 """
-from typing import List
+from __future__ import annotations
 
 import pandas
 
 from mimeo import tools
-from mimeo.database.exc import InvalidIndex
+from mimeo.database.exc import InvalidIndexError
 
 
 class City:
     """DTO class representing a single row in cities CSV data.
 
     Attributes
     ----------
@@ -25,15 +25,21 @@
         A city name
     name_ascii : str
         A city name in ASCII encoding
     country : str
         A country of a city
     """
 
-    def __init__(self, identifier: str, name: str, name_ascii: str, country: str):
+    def __init__(
+            self,
+            identifier: str,
+            name: str,
+            name_ascii: str,
+            country: str,
+    ):
         """Initialize City class.
 
         Parameters
         ----------
         identifier : str
             An identifier
         name : str
@@ -44,152 +50,178 @@
             A country of a city
         """
         self.id = int(identifier)
         self.name = name
         self.name_ascii = name_ascii
         self.country = country
 
-    def __str__(self) -> str:
+    def __str__(
+            self,
+    ) -> str:
         """Stringify the City instance.
 
         Returns
         -------
         str
             A stringified `dict` representation of the City instance
         """
         return str({
             "id": self.id,
             "name": self.name,
             "name_ascii": self.name_ascii,
-            "country": self.country
+            "country": self.country,
         })
 
-    def __repr__(self) -> str:
+    def __repr__(
+            self,
+    ) -> str:
         """Represent the City instance.
 
         Returns
         -------
         str
             A python representation of the City instance
         """
-        return f"City('{self.id}', '{self.name}', '{self.name_ascii}', '{self.country}')"
+        return (f"City("
+                f"id='{self.id}', "
+                f"name='{self.name}', "
+                f"name_ascii='{self.name_ascii}', "
+                f"country='{self.country}')")
 
 
 class CitiesDB:
     """Class exposing READ operations on cities CSV data.
 
     Attributes
     ----------
     NUM_OF_RECORDS : int
         A number of rows in cities CSV data
 
     Methods
     -------
-    get_cities() -> List[City]
+    get_cities() -> list[City]
         Get all cities.
-    get_cities_of(country_iso3: str) -> List[City]
+    get_cities_of(country_iso3: str) -> list[City]
         Get cities of a specific country.
     get_city_at(index: int) -> City
         Get a city at `index` position.
     """
 
     NUM_OF_RECORDS = 42905
     _CITIES_DB = "cities.csv"
     _CITIES_DF = None
     _CITIES = None
     _COUNTRY_CITIES = {}
 
-    def get_city_at(self, index: int) -> City:
+    def get_city_at(
+            self,
+            index: int,
+    ) -> City:
         """Get a city at `index` position.
 
         Parameters
         ----------
         index : int
             A city row index
 
         Returns
         -------
         City
             A specific city
 
         Raises
         ------
-        InvalidIndex
+        InvalidIndexError
             If the provided `index` is out of bounds
         """
         cities = self._get_cities()
         try:
             return cities[index]
         except IndexError:
-            raise InvalidIndex(index, CitiesDB.NUM_OF_RECORDS-1)
+            last_index = CitiesDB.NUM_OF_RECORDS-1
+            raise InvalidIndexError(index, last_index) from IndexError
 
-    def get_cities_of(self, country_iso3: str) -> List[City]:
+    def get_cities_of(
+            self,
+            country_iso3: str,
+    ) -> list[City]:
         """Get cities of a specific country.
 
         Parameters
         ----------
         country_iso3 : str
             A country ISO3 code to filter cities
 
         Returns
         -------
-        List[City]
+        list[City]
             List of cities filtered by country
         """
         return self._get_country_cities(country_iso3).copy()
 
     @classmethod
-    def get_cities(cls) -> List[City]:
+    def get_cities(
+            cls,
+    ) -> list[City]:
         """Get all cities.
 
         Returns
         -------
-        List[City]
+        list[City]
             List of all cities
         """
         return cls._get_cities().copy()
 
     @classmethod
-    def _get_country_cities(cls, country_iso3: str) -> List[City]:
+    def _get_country_cities(
+            cls,
+            country_iso3: str,
+    ) -> list[City]:
         """Get cities of a specific country from cache.
 
         The country's cities list is initialized for the first time
         and cached in internal class attribute.
 
         Parameters
         ----------
         country_iso3 : str
             A country ISO3 code to filter cities
 
         Returns
         -------
-        List[City]
+        list[City]
             List of cities filtered by country
         """
         if country_iso3 not in cls._COUNTRY_CITIES:
             cities = cls._get_cities()
-            cls._COUNTRY_CITIES[country_iso3] = list(filter(lambda city: city.country == country_iso3, cities))
+            cities = filter(lambda c: c.country == country_iso3, cities)
+            cls._COUNTRY_CITIES[country_iso3] = list(cities)
         return cls._COUNTRY_CITIES[country_iso3]
 
     @classmethod
-    def _get_cities(cls) -> List[City]:
+    def _get_cities(
+            cls,
+    ) -> list[City]:
         """Get all cities from cache.
 
         The cities list is initialized for the first time and cached
         in internal class attribute.
 
         Returns
         -------
-        List[City]
+        list[City]
             List of all cities
         """
         if cls._CITIES is None:
             cls._CITIES = [City(row.ID, row.CITY, row.CITY_ASCII, row.COUNTRY)
                            for row in cls._get_cities_df().itertuples()]
         return cls._CITIES
 
     @classmethod
-    def _get_cities_df(cls) -> pandas.DataFrame:
+    def _get_cities_df(
+            cls,
+    ) -> pandas.DataFrame:
         """Load cities CSV data and save in internal class attribute."""
         if cls._CITIES_DF is None:
-            cls._CITIES_DF = pandas.read_csv(tools.get_resource(CitiesDB._CITIES_DB))
+            data = tools.get_resource(CitiesDB._CITIES_DB)
+            cls._CITIES_DF = pandas.read_csv(data)
         return cls._CITIES_DF
```

### Comparing `mimeograph-0.4.2/src/mimeo/database/countries.py` & `mimeograph-0.4.3/src/mimeo/database/countries.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 It exports classes related to countries CSV data:
     * Country
         DTO class representing a single row in countries CSV
         data.
     * CountriesDB
         Class exposing READ operations on countries CSV data.
 """
-from typing import List
+from __future__ import annotations
 
 import pandas
 
 from mimeo import tools
-from mimeo.database.exc import InvalidIndex
+from mimeo.database.exc import InvalidIndexError
 
 
 class Country:
     """DTO class representing a single row in cities CSV data.
 
     Attributes
     ----------
@@ -24,15 +24,20 @@
         A country ISO3 code
     iso_2 : str
         A country ISO2 code
     name : str
         A country name
     """
 
-    def __init__(self, iso_3: str, iso_2: str, name: str):
+    def __init__(
+            self,
+            iso_3: str,
+            iso_2: str,
+            name: str,
+    ):
         """Initialize Country class.
 
         Parameters
         ----------
         iso_3 : str
             A country ISO3 code
         iso_2 : str
@@ -40,50 +45,57 @@
         name : str
             A country name
         """
         self.iso_3 = iso_3
         self.iso_2 = iso_2
         self.name = name
 
-    def __str__(self) -> str:
+    def __str__(
+            self,
+    ) -> str:
         """Stringify the Country instance.
 
         Returns
         -------
         str
             A stringified `dict` representation of the Country instance
         """
         return str({
             "iso_3": self.iso_3,
             "iso_2": self.iso_2,
-            "name": self.name
+            "name": self.name,
         })
 
-    def __repr__(self) -> str:
+    def __repr__(
+            self,
+    ) -> str:
         """Represent the Country instance.
 
         Returns
         -------
         str
             A python representation of the Country instance
         """
-        return f"Country('{self.iso_3}', '{self.iso_2}', '{self.name}')"
+        return (f"Country("
+                f"iso_3='{self.iso_3}', "
+                f"iso_2='{self.iso_2}', "
+                f"name='{self.name}')")
 
 
 class CountriesDB:
     """Class exposing READ operations on countries CSV data.
 
     Attributes
     ----------
     NUM_OF_RECORDS : int
         A number of rows in countries CSV data
 
     Methods
     -------
-    get_countries() -> List[Country]
+    get_countries() -> list[Country]
         Get all countries.
     get_country_at(index: int) -> Country
         Get a country at `index` position.
     get_country_by_iso_3(iso_3: str) -> Country
         Get a country having a specific ISO3 code.
     get_country_by_iso_3(iso_2: str) -> Country
         Get a country having a specific ISO2 code.
@@ -92,39 +104,46 @@
     """
 
     NUM_OF_RECORDS = 239
     _COUNTRIES_DB = "countries.csv"
     _COUNTRIES_DF = None
     _COUNTRIES = None
 
-    def get_country_at(self, index: int) -> Country:
+    def get_country_at(
+            self,
+            index: int,
+    ) -> Country:
         """Get a country at `index` position.
 
         Parameters
         ----------
         index : int
             A country row index
 
         Returns
         -------
         Country
             A specific country
 
         Raises
         ------
-        InvalidIndex
+        InvalidIndexError
             If the provided `index` is out of bounds
         """
         countries = self._get_countries()
         try:
             return countries[index]
         except IndexError:
-            raise InvalidIndex(index, CountriesDB.NUM_OF_RECORDS-1)
+            last_index = CountriesDB.NUM_OF_RECORDS-1
+            raise InvalidIndexError(index, last_index) from IndexError
 
-    def get_country_by_iso_3(self, iso_3: str) -> Country:
+    def get_country_by_iso_3(
+            self,
+            iso_3: str,
+    ) -> Country:
         """Get a country having a specific ISO3 code.
 
         Parameters
         ----------
         iso_3 : str
             An ISO3 code to find a country
 
@@ -132,15 +151,18 @@
         -------
         Country
             A specific country or None
         """
         countries = self._get_countries()
         return next(filter(lambda country: country.iso_3 == iso_3, countries), None)
 
-    def get_country_by_iso_2(self, iso_2: str) -> Country:
+    def get_country_by_iso_2(
+            self,
+            iso_2: str,
+    ) -> Country:
         """Get a country having a specific ISO2 code.
 
         Parameters
         ----------
         iso_2 : str
             An ISO2 code to find a country
 
@@ -148,15 +170,18 @@
         -------
         Country
             A specific country or None
         """
         countries = self._get_countries()
         return next(filter(lambda country: country.iso_2 == iso_2, countries), None)
 
-    def get_country_by_name(self, name: str) -> Country:
+    def get_country_by_name(
+            self,
+            name: str,
+    ) -> Country:
         """Get a country having a specific name.
 
         Parameters
         ----------
         name : str
             A name to find a country
 
@@ -165,40 +190,47 @@
         Country
             A specific country or None
         """
         countries = self._get_countries()
         return next(filter(lambda country: country.name == name, countries), None)
 
     @classmethod
-    def get_countries(cls) -> List[Country]:
+    def get_countries(
+            cls,
+    ) -> list[Country]:
         """Get all countries.
 
         Returns
         -------
-        List[Country]
+        list[Country]
             List of all countries
         """
         return cls._get_countries().copy()
 
     @classmethod
-    def _get_countries(cls) -> List[Country]:
+    def _get_countries(
+            cls,
+    ) -> list[Country]:
         """Get all countries from cache.
 
         The countries list is initialized for the first time and cached
         in internal class attribute.
 
         Returns
         -------
-        List[Country]
+        list[Country]
             List of all countries
         """
         if cls._COUNTRIES is None:
             cls._COUNTRIES = [Country(row.ISO_3, row.ISO_2, row.NAME)
                               for row in cls._get_countries_df().itertuples()]
         return cls._COUNTRIES
 
     @classmethod
-    def _get_countries_df(cls) -> pandas.DataFrame:
+    def _get_countries_df(
+            cls,
+    ) -> pandas.DataFrame:
         """Load countries CSV data and save in internal class attribute."""
         if cls._COUNTRIES_DF is None:
-            cls._COUNTRIES_DF = pandas.read_csv(tools.get_resource(CountriesDB._COUNTRIES_DB))
+            data = tools.get_resource(CountriesDB._COUNTRIES_DB)
+            cls._COUNTRIES_DF = pandas.read_csv(data)
         return cls._COUNTRIES_DF
```

### Comparing `mimeograph-0.4.2/src/mimeo/database/exc.py` & `mimeograph-0.4.3/src/mimeo/utils/exc.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,52 @@
-"""The Mimeo Database Exceptions module.
+"""The Mimeo Utils Exceptions module.
 
-It contains all custom exceptions related to Mimeo Context:
-    * InvalidIndex
-        A custom Exception class for invalid row index.
-    * InvalidSex
-        A custom Exception class for uninitialized context's iteration.
-    * CountryNotFound
-        A custom Exception class for not found context's iteration.
-    * OutOfStock
-        A custom Exception class for invalid special field's name.
+It contains all custom exceptions related to Mimeo Utils:
+    * InvalidMimeoUtil
+        A custom Exception class for an invalid Mimeo Util.
+    * InvalidValue
+        A custom Exception class for an invalid value in Mimeo Util.
+    * NotASpecialField
+        A custom Exception class for a field used as a special.
 """
 
 
-class InvalidIndex(Exception):
-    """A custom Exception class for invalid row index.
+from __future__ import annotations
 
-    Raised while attempting to get data at row that does not exist.
+
+class InvalidMimeoUtilError(Exception):
+    """A custom Exception class for an invalid Mimeo Util.
+
+    Raised when Mimeo Util node has missing _name property, or it
+    does not match any Mimeo Util.
     """
 
-    def __init__(self, index: int, last_index: int):
-        """Initialize InvalidIndex exception with details.
 
-        Extends Exception constructor with a custom message.
+class InvalidValueError(Exception):
+    """A custom Exception class for an invalid value in Mimeo Util.
 
-        Parameters
-        ----------
-        index : int
-            An invalid index
-        last_index : str
-            The last existing index
-        """
-        super().__init__(f"Provided index [{index}] is out or the range: 0-{last_index}!")
+    Raised when Mimeo Util node is incorrectly parametrized.
+    """
 
 
-class InvalidSex(Exception):
-    """A custom Exception class for invalid sex.
+class NotASpecialFieldError(Exception):
+    """A custom Exception class for a field used as a special.
 
-    Raised when sex provided to filter forenames is not supported.
+    Raised while attempting to retrieve special field name when it is
+    not a special one.
     """
 
-    def __init__(self, supported_sex_list: tuple):
-        """Initialize InvalidSex exception with details.
+    def __init__(
+            self,
+            field_name: str,
+    ):
+        """Initialize NotASpecialFieldError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
-        supported_sex_list : int
-            A list of supported sex values
+        field_name : str
+            A field name
         """
-        super().__init__(f"Invalid sex (use {' / '.join(supported_sex_list)})!")
-
-
-class DataNotFound(Exception):
-    """A custom Exception class for not found data.
-
-    Raised while attempting to filter data by a column's value that
-    does not match any row.
-    """
-
-    pass
-
-
-class OutOfStock(Exception):
-    """A custom Exception class for consuming all data.
-
-    Raised while attempting to get next unique value when all were
-    consumed already.
-    """
-
-    pass
+        msg = f"Provided field [{field_name}] is not a special one (use {'{:NAME:}'})!"
+        super().__init__(msg)
```

### Comparing `mimeograph-0.4.2/src/mimeo/database/first_names.py` & `mimeograph-0.4.3/src/mimeo/database/first_names.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,191 +2,217 @@
 
 It exports classes related to forenames CSV data:
     * FirstName
         DTO class representing a single row in forenames CSV data.
     * FirstNamesDB
         Class exposing READ operations on forenames CSV data.
 """
-from typing import List
+from __future__ import annotations
 
 import pandas
 
 from mimeo import tools
-from mimeo.database.exc import InvalidIndex, InvalidSex
+from mimeo.database.exc import InvalidIndexError, InvalidSexError
 
 
 class FirstName:
     """DTO class representing a single row in forenames CSV data.
 
     Attributes
     ----------
     name : str
         A first name
     sex : str
         A sex value
     """
 
-    def __init__(self, name: str, sex: str):
+    def __init__(
+            self,
+            name: str,
+            sex: str,
+    ):
         """Initialize FirstName class.
 
         Parameters
         ----------
         name : str
             A first name
         sex : str
             A sex value
         """
         self.name = name
         self.sex = sex
 
-    def __str__(self) -> str:
+    def __str__(
+            self,
+    ) -> str:
         """Stringify the FirstName instance.
 
         Returns
         -------
         str
             A stringified `dict` representation of the FirstName instance
         """
         return str({
             "name": self.name,
-            "sex": self.sex
+            "sex": self.sex,
         })
 
-    def __repr__(self) -> str:
+    def __repr__(
+            self,
+    ) -> str:
         """Represent the FirstName instance.
 
         Returns
         -------
         str
             A python representation of the FirstName instance
         """
-        return f"FirstName('{self.name}', '{self.sex}')"
+        return (f"FirstName("
+                f"name='{self.name}', "
+                f"sex='{self.sex}')")
 
 
 class FirstNamesDB:
     """Class exposing READ operations on forenames CSV data.
 
     Attributes
     ----------
     NUM_OF_RECORDS : int
         A number of rows in forenames CSV data
 
     Methods
     -------
-    get_first_names() -> List[FirstName]
+    get_first_names() -> list[FirstName]
         Get all first names.
-    get_first_names_by_sex(sex: str) -> List[FirstName]
+    get_first_names_by_sex(sex: str) -> list[FirstName]
         Get first names for a specific sex.
     get_first_name_at(index: int) -> FirstName
         Get a first name at `index` position.
     """
 
     NUM_OF_RECORDS = 7455
     __SUPPORTED_SEX = ("M", "F")
     __FIRST_NAMES_DB = "forenames.csv"
     __FIRST_NAMES_DF = None
     __FIRST_NAMES = None
     __NAMES_FOR_SEX = {}
 
-    def get_first_name_at(self, index: int) -> FirstName:
+    def get_first_name_at(
+            self,
+            index: int,
+    ) -> FirstName:
         """Get a first name at `index` position.
 
         Parameters
         ----------
         index : int
             A first name row index
 
         Returns
         -------
         FirstName
             A specific first name
 
         Raises
         ------
-        InvalidIndex
+        InvalidIndexError
             If the provided `index` is out of bounds
         """
         first_names = self.__get_first_names()
         try:
             return first_names[index]
         except IndexError:
-            raise InvalidIndex(index, FirstNamesDB.NUM_OF_RECORDS-1)
+            last_index = FirstNamesDB.NUM_OF_RECORDS-1
+            raise InvalidIndexError(index, last_index) from IndexError
 
-    def get_first_names_by_sex(self, sex: str) -> List[FirstName]:
+    def get_first_names_by_sex(
+            self,
+            sex: str,
+    ) -> list[FirstName]:
         """Get first names for a specific sex.
 
         Parameters
         ----------
         sex : str
             A sex value to filter first names
 
         Returns
         -------
-        List[FirstName]
+        list[FirstName]
             List of first names filtered by sex
 
         Raises
         ------
-        InvalidSex
+        InvalidSexError
             If the provided `sex` value is not supported
         """
-        if sex in FirstNamesDB.__SUPPORTED_SEX:
-            return self.__get_first_names_by_sex(sex).copy()
-        else:
-            raise InvalidSex(FirstNamesDB.__SUPPORTED_SEX)
+        if sex not in FirstNamesDB.__SUPPORTED_SEX:
+            raise InvalidSexError(FirstNamesDB.__SUPPORTED_SEX)
+        return self.__get_first_names_by_sex(sex).copy()
 
     @classmethod
-    def get_first_names(cls) -> List[FirstName]:
+    def get_first_names(
+            cls,
+    ) -> list[FirstName]:
         """Get all first names.
 
         Returns
         -------
-        List[FirstName]
+        list[FirstName]
             List of all first names
         """
         return cls.__get_first_names().copy()
 
     @classmethod
-    def __get_first_names_by_sex(cls, sex: str) -> List[FirstName]:
+    def __get_first_names_by_sex(
+            cls,
+            sex: str,
+    ) -> list[FirstName]:
         """Get first names for a specific sex from cache.
 
         The first names list for sex is initialized for the first time
         and cached in internal class attribute.
 
         Parameters
         ----------
         sex : str
             A sex value to filter first names
 
         Returns
         -------
-        List[FirstName]
+        list[FirstName]
             List of first names filtered by sex
         """
         if sex not in cls.__NAMES_FOR_SEX:
             first_names = cls.__get_first_names()
-            cls.__NAMES_FOR_SEX[sex] = list(filter(lambda first_name: first_name.sex == sex, first_names))
+            cls.__NAMES_FOR_SEX[sex] = list(filter(lambda n: n.sex == sex, first_names))
         return cls.__NAMES_FOR_SEX[sex]
 
     @classmethod
-    def __get_first_names(cls) -> List[FirstName]:
+    def __get_first_names(
+            cls,
+    ) -> list[FirstName]:
         """Get all first names from cache.
 
         The first names list is initialized for the first time and
         cached in internal class attribute.
 
         Returns
         -------
-        List[FirstName]
+        list[FirstName]
             List of all first names
         """
         if cls.__FIRST_NAMES is None:
             cls.__FIRST_NAMES = [FirstName(row.NAME, row.SEX)
                                  for row in cls.__get_first_names_df().itertuples()]
         return cls.__FIRST_NAMES
 
     @classmethod
-    def __get_first_names_df(cls) -> pandas.DataFrame:
+    def __get_first_names_df(
+            cls,
+    ) -> pandas.DataFrame:
         """Load forenames CSV data and save in internal class attribute."""
         if cls.__FIRST_NAMES_DF is None:
-            cls.__FIRST_NAMES_DF = pandas.read_csv(tools.get_resource(FirstNamesDB.__FIRST_NAMES_DB))
+            data = tools.get_resource(FirstNamesDB.__FIRST_NAMES_DB)
+            cls.__FIRST_NAMES_DF = pandas.read_csv(data)
         return cls.__FIRST_NAMES_DF
```

### Comparing `mimeograph-0.4.2/src/mimeo/database/last_names.py` & `mimeograph-0.4.3/src/mimeo/database/last_names.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,83 +1,91 @@
 """The Last Names module.
 
 It exports a class related to surnames CSV data:
     * LastNamesDB
         Class exposing READ operations on surnames CSV data.
 """
-from typing import List
+from __future__ import annotations
 
 from mimeo import tools
-from mimeo.database.exc import InvalidIndex
+from mimeo.database.exc import InvalidIndexError
 
 
 class LastNamesDB:
     """Class exposing READ operations on surnames CSV data.
 
     Attributes
     ----------
     NUM_OF_RECORDS : int
         A number of rows in surnames CSV data
 
     Methods
     -------
-    get_last_names() -> List[str]
+    get_last_names() -> list[str]
         Get all last names.
     get_last_name_at(index: int) -> str
         Get a last name at `index` position.
     """
 
     NUM_OF_RECORDS = 151670
     _LAST_NAMES_DB = "surnames.txt"
     _LAST_NAMES = None
 
-    def get_last_name_at(self, index: int) -> str:
+    def get_last_name_at(
+            self,
+            index: int,
+    ) -> str:
         """Get a last name at `index` position.
 
         Parameters
         ----------
         index : int
             A last name row index
 
         Returns
         -------
         str
             A last name
 
         Raises
         ------
-        InvalidIndex
+        InvalidIndexError
             If the provided `index` is out of bounds
         """
         last_names = self.__get_last_names()
         try:
             return last_names[index]
         except IndexError:
-            raise InvalidIndex(index, LastNamesDB.NUM_OF_RECORDS-1)
+            last_index = LastNamesDB.NUM_OF_RECORDS-1
+            raise InvalidIndexError(index, last_index) from IndexError
 
     @classmethod
-    def get_last_names(cls) -> List[str]:
+    def get_last_names(
+            cls,
+    ) -> list[str]:
         """Get all last names.
 
         Returns
         -------
-        List[str]
+        list[str]
             List of all last names
         """
         return cls.__get_last_names().copy()
 
     @classmethod
-    def __get_last_names(cls) -> list:
+    def __get_last_names(
+            cls,
+    ) -> list:
         """Get all last names from cache.
 
         The last names list is initialized for the first time and
         cached in internal class attribute.
 
         Returns
         -------
-        List[str]
+        list[str]
             List of all last names
         """
         if cls._LAST_NAMES is None:
             with tools.get_resource(LastNamesDB._LAST_NAMES_DB) as last_names:
                 cls._LAST_NAMES = [line.rstrip() for line in last_names.readlines()]
         return cls._LAST_NAMES
```

### Comparing `mimeograph-0.4.2/src/mimeo/database/mimeo_db.py` & `mimeograph-0.4.3/src/mimeo/database/mimeo_db.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The Mimeo Database module.
 
 It exports a class related to all Mimeo CSV data:
     * MimeoDB
         Facade class exposing READ operations on all Mimeo CSV data.
 """
-from typing import List
+from __future__ import annotations
 
 from mimeo.database import (CitiesDB, City, CountriesDB, Country, FirstName,
                             FirstNamesDB, LastNamesDB)
 
 
 class MimeoDB:
     """Facade class exposing READ operations on all Mimeo CSV data.
@@ -29,64 +29,71 @@
     NUM_OF_FIRST_NAMES : int
         A number of rows in forenames CSV data
     NUM_OF_LAST_NAMES : int
         A number of rows in surnames CSV data
 
     Methods
     -------
-    get_cities() -> List[City]
+    get_cities() -> list[City]
         Get all cities.
-    get_cities_of(country: str) -> List[City]
+    get_cities_of(country: str) -> list[City]
         Get cities of a specific country.
     get_city_at(index: int) -> City
         Get a city at `index` position.
-    get_countries() -> List[Country]
+    get_countries() -> list[Country]
         Get all countries.
     get_country_at(index: int) -> Country
         Get a country at `index` position.
     get_country_by_iso_3(iso_3: str) -> Country
         Get a country having a specific ISO3 code.
     get_country_by_iso_3(iso_2: str) -> Country
         Get a country having a specific ISO2 code.
     get_country_by_name(name: str) -> Country
         Get a country having a specific name.
-    get_first_names() -> List[FirstName]
+    get_first_names() -> list[FirstName]
         Get all first names.
-    get_first_names_by_sex(sex: str) -> List[FirstName]
+    get_first_names_by_sex(sex: str) -> list[FirstName]
         Get first names for a specific sex.
     get_first_name_at(index: int) -> FirstName
         Get a first name at `index` position.
-    get_last_names() -> List[str]
+    get_last_names() -> list[str]
         Get all last names.
     get_last_name_at(index: int) -> str
         Get a last name at `index` position.
     """
 
     NUM_OF_CITIES = CitiesDB.NUM_OF_RECORDS
     NUM_OF_COUNTRIES = CountriesDB.NUM_OF_RECORDS
     NUM_OF_FIRST_NAMES = FirstNamesDB.NUM_OF_RECORDS
     NUM_OF_LAST_NAMES = LastNamesDB.NUM_OF_RECORDS
 
-    def __init__(self):
+    def __init__(
+            self,
+    ):
         self.__cities_db = CitiesDB()
         self.__countries_db = CountriesDB()
         self.__first_names_db = FirstNamesDB()
         self.__last_names_db = LastNamesDB()
 
-    def get_cities(self) -> List[City]:
+    def get_cities(
+            self,
+    ) -> list[City]:
         """Get all cities.
 
         Returns
         -------
-        List[City]
+        list[City]
             List of all cities
         """
         return self.__cities_db.get_cities()
 
-    def get_cities_of(self, country: str) -> List[City]:
+    def get_cities_of(
+            self,
+            country: str,
+    ) -> list[City]:
         """Get cities of a specific country.
 
         In contrast to CitiesDB.get_cities_of() method it combines
         CitiesDB and CountriesDB to allow for any country detail
         providing. It can be ISO3 code, ISO2 code and name.
         First it will find the specific country and extract its
         ISO3 code to use in CitiesDB.get_cities_of() call.
@@ -94,190 +101,222 @@
         Parameters
         ----------
         country : str
             A country ISO3 / ISO2 code or name to filter cities
 
         Returns
         -------
-        List[City]
+        list[City]
             List of cities filtered by country
         """
-        country = next(filter(lambda c: country in [c.iso_3, c.iso_2, c.name], self.get_countries()), None)
+        countries = filter(
+            lambda c: country in [c.iso_3, c.iso_2, c.name],
+            self.get_countries())
+        country = next(countries, None)
         if country is None:
             return []
-        else:
-            return self.__cities_db.get_cities_of(country.iso_3)
+        return self.__cities_db.get_cities_of(country.iso_3)
 
-    def get_city_at(self, index: int) -> City:
+    def get_city_at(
+            self,
+            index: int,
+    ) -> City:
         """Get a city at `index` position.
 
         Parameters
         ----------
         index : int
             A city row index
 
         Returns
         -------
         City
             A specific city
 
         Raises
         ------
-        InvalidIndex
+        InvalidIndexError
             If the provided `index` is out of bounds
         """
         return self.__cities_db.get_city_at(index)
 
-    def get_countries(self) -> List[Country]:
+    def get_countries(
+            self,
+    ) -> list[Country]:
         """Get all countries.
 
         Returns
         -------
-        List[Country]
+        list[Country]
             List of all countries
         """
         return self.__countries_db.get_countries()
 
-    def get_country_at(self, index: int) -> Country:
+    def get_country_at(
+            self,
+            index: int,
+    ) -> Country:
         """Get a country at `index` position.
 
         Parameters
         ----------
         index : int
             A country row index
 
         Returns
         -------
         Country
             A specific country
 
         Raises
         ------
-        InvalidIndex
+        InvalidIndexError
             If the provided `index` is out of bounds
         """
         return self.__countries_db.get_country_at(index)
 
-    def get_country_by_iso_3(self, iso_3: str) -> Country:
+    def get_country_by_iso_3(
+            self,
+            iso_3: str,
+    ) -> Country:
         """Get a country having a specific ISO3 code.
 
         Parameters
         ----------
         iso_3 : str
             An ISO3 code to find a country
 
         Returns
         -------
         Country
             A specific country or None
         """
         return self.__countries_db.get_country_by_iso_3(iso_3)
 
-    def get_country_by_iso_2(self, iso_2: str) -> Country:
+    def get_country_by_iso_2(
+            self,
+            iso_2: str,
+    ) -> Country:
         """Get a country having a specific ISO2 code.
 
         Parameters
         ----------
         iso_2 : str
             An ISO2 code to find a country
 
         Returns
         -------
         Country
             A specific country or None
         """
         return self.__countries_db.get_country_by_iso_2(iso_2)
 
-    def get_country_by_name(self, name: str) -> Country:
+    def get_country_by_name(
+            self,
+            name: str,
+    ) -> Country:
         """Get a country having a specific name.
 
         Parameters
         ----------
         name : str
             A name to find a country
 
         Returns
         -------
         Country
             A specific country or None
         """
         return self.__countries_db.get_country_by_name(name)
 
-    def get_first_names(self) -> List[FirstName]:
+    def get_first_names(
+            self,
+    ) -> list[FirstName]:
         """Get all first names.
 
         Returns
         -------
-        List[FirstName]
+        list[FirstName]
             List of all first names
         """
         return self.__first_names_db.get_first_names()
 
-    def get_first_names_by_sex(self, sex: str) -> List[FirstName]:
+    def get_first_names_by_sex(
+            self,
+            sex: str,
+    ) -> list[FirstName]:
         """Get first names for a specific sex.
 
         Parameters
         ----------
         sex : str
             A sex value to filter first names
 
         Returns
         -------
-        List[FirstName]
+        list[FirstName]
             List of first names filtered by sex
 
         Raises
         ------
-        InvalidSex
+        InvalidSexError
             If the provided `sex` value is not supported
         """
         return self.__first_names_db.get_first_names_by_sex(sex)
 
-    def get_first_name_at(self, index: int) -> FirstName:
+    def get_first_name_at(
+            self,
+            index: int,
+    ) -> FirstName:
         """Get a first name at `index` position.
 
         Parameters
         ----------
         index : int
             A first name row index
 
         Returns
         -------
         FirstName
             A specific first name
 
         Raises
         ------
-        InvalidIndex
+        InvalidIndexError
             If the provided `index` is out of bounds
         """
         return self.__first_names_db.get_first_name_at(index)
 
-    def get_last_names(self) -> List[str]:
+    def get_last_names(
+            self,
+    ) -> list[str]:
         """Get all last names.
 
         Returns
         -------
-        List[str]
+        list[str]
             List of all last names
         """
         return self.__last_names_db.get_last_names()
 
-    def get_last_name_at(self, index: int) -> str:
+    def get_last_name_at(
+            self,
+            index: int,
+    ) -> str:
         """Get a last name at `index` position.
 
         Parameters
         ----------
         index : int
             A last name row index
 
         Returns
         -------
         str
             A last name
 
         Raises
         ------
-        InvalidIndex
+        InvalidIndexError
             If the provided `index` is out of bounds
         """
         return self.__last_names_db.get_last_name_at(index)
```

### Comparing `mimeograph-0.4.2/src/mimeo/generators/__init__.py` & `mimeograph-0.4.3/src/mimeo/generators/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,7 +19,9 @@
 
 To use this package, simply import the desired class:
     from mimeo.generators import GeneratorFactory
 """
 from .generator import Generator
 from .xml_generator import XMLGenerator
 from .generator_factory import GeneratorFactory
+
+__all__ = ["Generator", "XMLGenerator", "GeneratorFactory"]
```

### Comparing `mimeograph-0.4.2/src/mimeo/generators/generator.py` & `mimeograph-0.4.3/src/mimeo/generators/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,102 +3,99 @@
 It exports only one class:
     * Generator
         An abstract class for data generators in Mimeo.
 """
 from __future__ import annotations
 
 from abc import ABCMeta, abstractmethod
-from typing import Any, Iterator, Union
+from typing import Any, Iterator
 
-from mimeo.config.mimeo_config import MimeoConfig, MimeoTemplate
+from mimeo.config.mimeo_config import MimeoTemplate
 
 
 class Generator(metaclass=ABCMeta):
     """An abstract class for data generators in Mimeo.
 
     Its subclasses are meant to be used in the Mimeo processing.
     Every supported output format has a Generator representation.
 
     Methods
     -------
     generate(
-        templates: Union[list, Iterator[MimeoTemplate]],
+        templates: list | Iterator[MimeoTemplate],
         parent: Any = None
     ) -> Iterator[Any]
         Generate data based on the Mimeo Configuration.
     stringify(
         data: Any,
         mimeo_config: MimeoConfig
     ) -> str
         Stringify data generated by the generate() method.
     """
 
     @classmethod
     def __subclasshook__(
             cls,
-            subclass: Generator
+            subclass: Generator,
     ):
         """Verify if a subclass implements all abstract methods.
 
         Parameters
         ----------
         subclass : Generator
             A Generator subclass
 
         Returns
         -------
         bool
             True if the subclass includes the generate and stringify
             methods
         """
-        return ('generate' in subclass.__dict__ and callable(subclass.generate) and
-                'stringify' in subclass.__dict__ and callable(subclass.stringify))
+        return ("generate" in subclass.__dict__ and callable(subclass.generate) and
+                "stringify" in subclass.__dict__ and callable(subclass.stringify))
 
     @abstractmethod
     def generate(
             self,
-            templates: Union[list, Iterator[MimeoTemplate]],
-            parent: Any = None
+            templates: list | Iterator[MimeoTemplate],
+            parent: Any = None,
     ) -> Iterator[Any]:
         """Generate data based on the Mimeo Configuration.
 
         It is an abstract method to implement in subclasses
 
         Parameters
         ----------
-        templates : Union[list, Iterator[MimeoTemplate]]
+        templates : list | Iterator[MimeoTemplate]
             A collection of Mimeo Templates to process
         parent : Any, default None
             A parent node for the currently processed template.
             It is passed only when a Mimeo Config contain nested
             templates.
 
         Returns
         -------
         Iterator[Any]
             Iterator for generated nodes
         """
-        pass
+        raise NotImplementedError
 
     @abstractmethod
     def stringify(
             self,
             data_unit: Any,
-            mimeo_config: MimeoConfig
     ) -> str:
         """Stringify data generated by the generate() method.
 
         It is an abstract method to implement in subclasses
 
         Parameters
         ----------
         data_unit: Any
             A single data unit generated by the generate() method
-        mimeo_config: MimeoConfig
-            A Mimeo Configuration providing output details
 
         Returns
         -------
         str
             Stringified data unit
         """
-        pass
+        raise NotImplementedError
```

### Comparing `mimeograph-0.4.2/src/mimeo/generators/generator_factory.py` & `mimeograph-0.4.3/src/mimeo/generators/generator_factory.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """The Mimeo Generator Factory module.
 
 It exports only one class:
     * GeneratorFactory
         A Factory class instantiating a Generator based on Mimeo Config.
 """
-from mimeo.config.exc import UnsupportedPropertyValue
+from __future__ import annotations
+
+from mimeo.config.exc import UnsupportedPropertyValueError
 from mimeo.config.mimeo_config import MimeoConfig
 from mimeo.generators import Generator, XMLGenerator
 
 
 class GeneratorFactory:
     """A Factory class instantiating a Generator based on Mimeo Config.
 
@@ -25,32 +27,34 @@
     get_generator(mimeo_config: MimeoConfig) -> Generator
         Initialize a Generator based on the Mimeo Output Format.
     """
 
     XML = MimeoConfig.OUTPUT_FORMAT_XML
 
     @staticmethod
-    def get_generator(mimeo_config: MimeoConfig) -> Generator:
+    def get_generator(
+            mimeo_config: MimeoConfig,
+    ) -> Generator:
         """Initialize a Generator based on the Mimeo Output Format.
 
         Parameters
         ----------
         mimeo_config : MimeoConfig
             A Mimeo Configuration
 
         Returns
         -------
         Generator
             A Generator's implementation instance
 
         Raises
         ------
-        UnsupportedPropertyValue
+        UnsupportedPropertyValueError
             If the output format is not supported
         """
-        output_format = mimeo_config.output_details.format
+        output_format = mimeo_config.output.format
         if output_format == GeneratorFactory.XML:
             return XMLGenerator(mimeo_config)
-        else:
-            raise UnsupportedPropertyValue(MimeoConfig.OUTPUT_DETAILS_FORMAT_KEY,
-                                           output_format,
-                                           MimeoConfig.SUPPORTED_OUTPUT_FORMATS)
+        raise UnsupportedPropertyValueError(
+            MimeoConfig.OUTPUT_FORMAT_KEY,
+            output_format,
+            MimeoConfig.SUPPORTED_OUTPUT_FORMATS)
```

### Comparing `mimeograph-0.4.2/src/mimeo/logging/__init__.py` & `mimeograph-0.4.3/src/mimeo/logging/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,23 +14,27 @@
 * setup_logging
     Set up customized logging configuration.
 
 To use this package, simply import the desired class or function:
     from mimeo.logging import RegularFilter
     from mimeo.logging import setup_logging
 """
+from __future__ import annotations
+
 import logging.config
 
 import yaml
 from haggis.logs import add_logging_level
 
 from mimeo import tools
 
 from .filters import DetailedFilter, RegularFilter
 
+__all__ = ["DetailedFilter", "RegularFilter", "setup_logging"]
+
 
 def setup_logging():
     """Set up customized logging configuration.
 
     The configuration is stored in the logging.yaml file in
     the resources package. Besides that a new log level is defined,
     FINE, together with a method logger.fine().
```

### Comparing `mimeograph-0.4.2/src/mimeo/logging/filters.py` & `mimeograph-0.4.3/src/mimeo/logging/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,34 @@
 This module contains all filters used in logging.
 It exports the following filters:
     * RegularFilter
         A Filter subclass filtering out log records below INFO level.
     * DetailedFilter
         A Filter subclass filtering out log records above DEBUG level.
 """
+from __future__ import annotations
+
 from logging import DEBUG, INFO, Filter, LogRecord
 
 
 class RegularFilter(Filter):
     """A Filter subclass filtering out log records below INFO level.
 
     It is meant to be used for logging info in regular format.
 
     Methods
     -------
     filter(record: LogRecord)
         Determine if the specified record is to be logged.
     """
 
-    def filter(self, record: LogRecord) -> bool:
+    def filter(
+            self,
+            record: LogRecord,
+    ) -> bool:
         """Determine if the specified record is to be logged.
 
         Parameters
         ----------
         record : LogRecord
             A log record
 
@@ -44,15 +49,18 @@
 
     Methods
     -------
     filter(record: LogRecord)
         Determine if the specified record is to be logged.
     """
 
-    def filter(self, record: LogRecord):
+    def filter(
+            self,
+            record: LogRecord,
+    ):
         """Determine if the specified record is to be logged.
 
         Parameters
         ----------
         record : LogRecord
             A log record
```

### Comparing `mimeograph-0.4.2/src/mimeo/meta/__init__.py` & `mimeograph-0.4.3/src/mimeo/meta/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,8 +14,12 @@
     A type ensuring there's only one instance qualified to be used.
 - Alive
     A superclass for OnlyOneAlive classes.
 
 To use this package, simply import the desired class:
     from mimeo.meta import Alive, OnlyOneAlive
 """
+from __future__ import annotations
+
 from .alive import Alive, OnlyOneAlive
+
+__all__ = ["Alive", "OnlyOneAlive"]
```

### Comparing `mimeograph-0.4.2/src/mimeo/meta/alive.py` & `mimeograph-0.4.3/src/mimeo/meta/alive.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,40 +33,45 @@
     x_2 = alive_2.get_x()
 
     print('Alive 1:', x_1)  # 1
     print('Alive 2:', x_2)  # 1
 """
 from __future__ import annotations
 
-from mimeo.meta.exc import InstanceNotAlive
+from types import TracebackType
+
+from mimeo.meta.exc import InstanceNotAliveError
 
 
 class OnlyOneAlive(type):
     """A type ensuring there's only one instance qualified to be used.
 
     The OnlyOneAlive type caches all instances being created for each
     Alive subclass. If there is any instance being alive, it is
     returned by a constructor. Otherwise, an Alive subclass is
     instantiated and returned.
     """
 
     _INSTANCES = {}
 
-    def __call__(cls, *args, **kwargs):
+    def __call__(
+            cls,
+            *args,
+            **kwargs,
+    ):
         """Ensure there's only one instance qualified to be used."""
         if cls not in cls._INSTANCES:
             cls._INSTANCES[cls] = []
 
-        alive_instance = next((instance for instance in cls._INSTANCES[cls] if instance.is_alive()), None)
-        if alive_instance is not None:
-            return alive_instance
-        else:
+        alive_instance = next((i for i in cls._INSTANCES[cls] if i.is_alive()), None)
+        if alive_instance is None:
             instance = super().__call__(*args, **kwargs)
             cls._INSTANCES[cls].append(instance)
             return instance
+        return alive_instance
 
 
 class Alive:
     """A superclass for OnlyOneAlive classes.
 
     It provides several features defined to use OnlyOneAlive pattern:
     * Context Manager functionality
@@ -77,65 +82,77 @@
     -------
     is_alive()
         Verify if the instance is alive.
     assert_alive()
         Assert the instance is alive.
     """
 
-    def __init__(self):
+    def __init__(
+            self,
+    ):
         self._alive = False
 
-    def __enter__(self) -> Alive:
+    def __enter__(
+            self,
+    ) -> Alive:
         """Enter the Alive instance.
 
         It sets the internal `alive` attribute to True.
 
         Returns
         -------
         self : Alive
             A Alive instance
         """
         self._alive = True
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+    def __exit__(
+            self,
+            exc_type: type | None,
+            exc_val: BaseException | None,
+            exc_tb: TracebackType | None,
+    ) -> None:
         """Exit the Alive instance.
 
         It sets the internal `alive` attribute to False.
 
         Parameters
         ----------
-        exc_type
+        exc_type : type | None
             An exception's type
-        exc_val
+        exc_val : BaseException | None
             An exception's value
-        exc_tb
+        exc_tb  TracebackType | None
             An exception's traceback
 
         Returns
         -------
         None
             A None value
         """
         self._alive = False
-        return None
 
-    def assert_alive(self) -> bool:
+    def assert_alive(
+            self,
+    ) -> bool:
         """Assert the instance is alive.
 
         Returns
         -------
         bool
             True
 
         Raises
         ------
         InstanceNotAlive
             If the instance is not alive
         """
         if not self.is_alive():
-            raise InstanceNotAlive()
+            raise InstanceNotAliveError
         return self.is_alive()
 
-    def is_alive(self) -> bool:
+    def is_alive(
+            self,
+    ) -> bool:
         """Verify if the instance is alive."""
         return self._alive
```

### Comparing `mimeograph-0.4.2/src/mimeo/meta/exc.py` & `mimeograph-0.4.3/src/mimeo/meta/exc.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 
 It contains all custom exceptions related to useful abstract classes:
     * InstanceNotAlive
         A custom Exception class for using non-alive instance.
 """
 
 
-class InstanceNotAlive(Exception):
+from __future__ import annotations
+
+
+class InstanceNotAliveError(Exception):
     """A custom Exception class for using non-alive instance.
 
     Raised when using OnlyOneAlive class that is not alive.
     """
 
-    def __init__(self):
-        """Initialize InstanceNotAlive exception with details.
+    def __init__(
+            self,
+    ):
+        """Initialize InstanceNotAliveError exception with details.
 
         Extends Exception constructor with a constant message.
         """
         super().__init__("The instance is not alive!")
```

### Comparing `mimeograph-0.4.2/src/mimeo/mimeo.py` & `mimeograph-0.4.3/src/mimeo/mimeo.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """The Mimeo module.
 
 This module is a main module providing the most high level class
 in Mimeo:
     * Mimeograph
         A class responsible for the Mimeo processing.
 """
+from __future__ import annotations
+
 import logging
 
 from mimeo.config.mimeo_config import MimeoConfig
 from mimeo.consumers import ConsumerFactory
 from mimeo.context import MimeoContextManager
 from mimeo.generators import GeneratorFactory
 
@@ -23,20 +25,25 @@
 
     Methods
     -------
     process()
         Process the Mimeo Configuration (generate data and consume).
     """
 
-    def __init__(self, mimeo_config: MimeoConfig):
+    def __init__(
+            self,
+            mimeo_config: MimeoConfig,
+    ):
         self._mimeo_config = mimeo_config
         self._generator = GeneratorFactory.get_generator(self._mimeo_config)
         self._consumer = ConsumerFactory.get_consumer(self._mimeo_config)
 
-    def process(self):
+    def process(
+            self,
+    ):
         """Process the Mimeo Configuration (generate data and consume)."""
         logger.info("Starting data generation")
         with MimeoContextManager(self._mimeo_config):
             for data in self._generator.generate(self._mimeo_config.templates):
-                data_str = self._generator.stringify(data, self._mimeo_config)
+                data_str = self._generator.stringify(data)
                 self._consumer.consume(data_str)
         logger.info("Data has been processed")
```

### Comparing `mimeograph-0.4.2/src/mimeo/resources/cities.csv` & `mimeograph-0.4.3/src/mimeo/resources/cities.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.2/src/mimeo/resources/countries.csv` & `mimeograph-0.4.3/src/mimeo/resources/countries.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.2/src/mimeo/resources/exc.py` & `mimeograph-0.4.3/src/mimeo/resources/exc.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 
 It contains all custom exceptions related to Mimeo resources:
     * ResourceNotFound
         A custom Exception class for a not found resource.
 """
 
 
-class ResourceNotFound(Exception):
+from __future__ import annotations
+
+
+class ResourceNotFoundError(Exception):
     """A custom Exception class for a not found resource.
 
     Raised while attempting to get a resource that does exist.
     """
 
-    def __init__(self, resource_name: str):
-        """Initialize ResourceNotFound exception with details.
+    def __init__(
+            self,
+            resource_name: str,
+    ):
+        """Initialize ResourceNotFoundError exception with details.
 
         Extends Exception constructor with a custom message.
 
         Parameters
         ----------
         resource_name : str
             A resource name
```

### Comparing `mimeograph-0.4.2/src/mimeo/resources/forenames.csv` & `mimeograph-0.4.3/src/mimeo/resources/forenames.csv`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.2/src/mimeo/resources/logging.yaml` & `mimeograph-0.4.3/src/mimeo/resources/logging.yaml`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.2/src/mimeo/resources/surnames.txt` & `mimeograph-0.4.3/src/mimeo/resources/surnames.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.2/src/mimeo/tools.py` & `mimeograph-0.4.3/src/mimeo/tools.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 """The Mimeo Tools module.
 
 It is meant to store all useful functions that can help in any
 non-Mimeo-specific operations. It exports the following functions:
     * get_resource(resource_name: str) -> TextIO
         Return a Mimeo resource.
 """
-from typing.io import TextIO
+from __future__ import annotations
 
-from mimeo.resources.exc import ResourceNotFound
-
-try:
-    import importlib.resources as pkg_resources
-except ImportError:  # Python < 3.7
-    import importlib_resources as pkg_resources
+import importlib.resources as pkg_resources
+from typing import TextIO
 
 from mimeo import resources as data
+from mimeo.resources.exc import ResourceNotFoundError
 
 
-def get_resource(resource_name: str) -> TextIO:
+def get_resource(
+        resource_name: str,
+) -> TextIO:
     """Return a Mimeo resource.
 
     The resource needs to be included in mimeo.resources package
     to be returned.
 
     Parameters
     ----------
@@ -37,8 +36,8 @@
     ------
     ResourceNotFound
         If the resource does not exist
     """
     try:
         return pkg_resources.open_text(data, resource_name)
     except FileNotFoundError:
-        raise ResourceNotFound(resource_name)
+        raise ResourceNotFoundError(resource_name) from FileNotFoundError
```

### Comparing `mimeograph-0.4.2/src/mimeo/utils/mimeo_utils.py` & `mimeograph-0.4.3/src/mimeo/utils/mimeo_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,51 +35,56 @@
 from abc import ABCMeta, abstractmethod
 from datetime import date, datetime, timedelta
 from typing import Any
 
 from mimeo.context import MimeoContext, MimeoContextManager
 from mimeo.context.decorators import mimeo_context
 from mimeo.database import Country, MimeoDB
-from mimeo.database.exc import DataNotFound, InvalidSex
-from mimeo.utils.exc import InvalidValue
+from mimeo.database.exc import DataNotFoundError, InvalidSexError
+from mimeo.utils.exc import InvalidValueError
 
 
 class MimeoUtil(metaclass=ABCMeta):
     """A superclass for all Mimeo Utils.
 
     It defines abstract methods to be implemented in each subclass.
 
     Methods
     -------
     render
         Render a value.
     """
 
     @classmethod
-    def __subclasshook__(cls, subclass: MimeoUtil):
+    def __subclasshook__(
+            cls,
+            subclass: MimeoUtil,
+    ):
         """Verify if a subclass implements all abstract methods.
 
         Parameters
         ----------
         subclass : MimeoUtil
             A MimeoUtil subclass
 
         Returns
         -------
         bool
             True if the subclass includes the render method and KEY
             attribute
         """
-        return ('KEY' in subclass.__dict__ and
+        return ("KEY" in subclass.__dict__ and
                 not callable(subclass.KEY) and
-                'render' in subclass.__dict__ and
+                "render" in subclass.__dict__ and
                 callable(subclass.render))
 
     @abstractmethod
-    def render(self) -> Any:
+    def render(
+            self,
+    ) -> Any:
         """Render a value.
 
         It is an abstract method to implement in subclasses
         """
         raise NotImplementedError
 
 
@@ -95,27 +100,33 @@
     ----------
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "random_str"
 
-    def __init__(self, length: int = 20, **kwargs):
+    def __init__(
+            self,
+            length: int = 20,
+            **kwargs,
+    ):
         """Initialize RandomStringUtil class.
 
         Parameters
         ----------
         length : int, default 20
             A length of a string to render
         kwargs : dict
             Arbitrary keyword arguments (ignored).
         """
         self._length = length
 
-    def render(self) -> str:
+    def render(
+            self,
+    ) -> str:
         """Render a random string value.
 
         Returns
         -------
         str
             A random string value
         """
@@ -134,30 +145,37 @@
     ----------
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "random_int"
 
-    def __init__(self, start: int = 1, limit: int = 100, **kwargs):
+    def __init__(
+            self,
+            start: int = 1,
+            limit: int = 100,
+            **kwargs,
+    ):
         """Initialize RandomIntegerUtil class.
 
         Parameters
         ----------
         start : int, default 1
             A lower bound for integers (inclusive)
         limit : int, default 100
             An upper bound for integers (inclusive)
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
         self._start = start
         self._limit = limit
 
-    def render(self) -> int:
+    def render(
+            self,
+    ) -> int:
         """Render a random integer value.
 
         Returns
         -------
         int
             A random integer value
         """
@@ -176,27 +194,33 @@
     ----------
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "random_item"
 
-    def __init__(self, items: list = None, **kwargs):
+    def __init__(
+            self,
+            items: list = None,
+            **kwargs,
+    ):
         """Initialize RandomItemUtil class.
 
         Parameters
         ----------
         items : int, default ['']
             A list of items from which a value will be picked up
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
         self._items = items if items is not None and len(items) != 0 else [""]
 
-    def render(self) -> Any:
+    def render(
+            self,
+    ) -> Any:
         """Render a random item.
 
         Returns
         -------
         Any
             A random item
         """
@@ -216,35 +240,44 @@
     ----------
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "date"
 
-    def __init__(self, days_delta: int = 0, **kwargs):
+    def __init__(
+            self,
+            days_delta: int = 0,
+            **kwargs,
+    ):
         """Initialize DateUtil class.
 
         Parameters
         ----------
         days_delta : int, default 0
             An integer value of days to add or subtract from today
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
         self._days_delta = days_delta
 
-    def render(self) -> str:
+    def render(
+            self,
+    ) -> str:
         """Render a stringified date value.
 
         Returns
         -------
         str
             A stringified date value in format %Y-%m-%d
         """
-        date_value = date.today() if self._days_delta == 0 else date.today() + timedelta(days=self._days_delta)
+        if self._days_delta == 0:
+            date_value = date.today()
+        else:
+            date_value = date.today() + timedelta(days=self._days_delta)
         return date_value.strftime("%Y-%m-%d")
 
 
 class DateTimeUtil(MimeoUtil):
     """A MimeoUtil implementation rendering a stringified date time value.
 
     Methods
@@ -282,15 +315,17 @@
             Arbitrary keyword arguments (ignored)
         """
         self._days_delta = days_delta
         self._hours_delta = hours_delta
         self._minutes_delta = minutes_delta
         self._seconds_delta = seconds_delta
 
-    def render(self) -> str:
+    def render(
+            self,
+    ) -> str:
         """Render a stringified date time value.
 
         Returns
         -------
         str
             A stringified date time value in format %Y-%m-%dT%H:%M:%S
         """
@@ -299,15 +334,15 @@
                                                 minutes=self._minutes_delta,
                                                 seconds=self._seconds_delta)
         return time_value.strftime("%Y-%m-%dT%H:%M:%S")
 
 
 class AutoIncrementUtil(MimeoUtil):
     """A MimeoUtil implementation rendering an auto incremented ID.
-    
+
     It is a Mimeo Context-dependent Mimeo Util. Rendered ID value is
     pulled from the Context.
 
     Methods
     -------
     render
         Render an auto incremented identifier.
@@ -316,57 +351,65 @@
     ----------
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "auto_increment"
 
-    def __init__(self, pattern: str = "{:05d}", **kwargs):
+    def __init__(
+            self,
+            pattern: str = "{:05d}",
+            **kwargs,
+    ):
         """Initialize AutoIncrementUtil class.
 
         Parameters
         ----------
         pattern : str, default '{:05d}'
             A pattern to inject incremented ID
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
         self._pattern = pattern
 
     @mimeo_context
-    def render(self, context: MimeoContext = None) -> str:
+    def render(
+            self,
+            context: MimeoContext = None,
+    ) -> str:
         """Render an auto incremented identifier.
-        
+
         Parameters
         ----------
         context : MimeoContext, default None
             A current Mimeo Context injected by a decorator
 
         Returns
         -------
         str
             An auto incremented identifier in a parametrized format
-        
+
         Raises
         ------
         InvalidValue
             If the pattern is not a string value
         """
         try:
             identifier = context.next_id()
             return self._pattern.format(identifier)
         except AttributeError:
             context.prev_id()
-            raise InvalidValue(f"The {self.KEY} Mimeo Util require a string value for the pattern parameter "
-                               f"and was: [{self._pattern}].")
+            msg = (f"The {self.KEY} Mimeo Util require a string value for the pattern "
+                   f"parameter and was: [{self._pattern}].")
+            raise InvalidValueError(msg) from AttributeError
 
 
 class CurrentIterationUtil(MimeoUtil):
     """A MimeoUtil implementation rendering a current iteration ID.
-    
+
     It is a Mimeo Context-dependent Mimeo Util. Rendered ID value is
     pulled from the Context.
 
     Methods
     -------
     render
         Render a current iteration ID.
@@ -375,47 +418,55 @@
     ----------
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "curr_iter"
 
-    def __init__(self, context: str = None, **kwargs):
+    def __init__(
+            self,
+            context: str = None,
+            **kwargs,
+    ):
         """Initialize CurrentIterationUtil class.
 
         Parameters
         ----------
         context : str, default None
             A context name to reach the current iteration
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
         self._context_name = context
 
     @mimeo_context
-    def render(self, context: MimeoContext = None) -> int:
+    def render(
+            self,
+            context: MimeoContext = None,
+    ) -> int:
         """Render a current iteration ID.
-        
+
         Parameters
         ----------
         context : MimeoContext, default None
             A current Mimeo Context injected by a decorator
 
         Returns
         -------
         int
             A specific Mimeo Context's current iteration ID
         """
-        context = context if self._context_name is None else MimeoContextManager().get_context(self._context_name)
+        if self._context_name is not None:
+            context = MimeoContextManager().get_context(self._context_name)
         return context.curr_iteration().id
 
 
 class KeyUtil(MimeoUtil):
     """A MimeoUtil implementation rendering a unique identifier.
-    
+
     It is a Mimeo Context-dependent Mimeo Util. Rendered identifiers
     are stored in a MimeoContext and pulled from it when the Mimeo
     Util is parametrized to do so.
 
     Methods
     -------
     render
@@ -425,15 +476,20 @@
     ----------
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "key"
 
-    def __init__(self, context: str = None, iteration: int = None, **kwargs):
+    def __init__(
+            self,
+            context: str = None,
+            iteration: int = None,
+            **kwargs,
+    ):
         """Initialize KeyUtil class.
 
         Parameters
         ----------
         context : str, default None
             A context name to reach already generated identifier
         iteration : int, default None
@@ -441,43 +497,50 @@
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
         self._context_name = context
         self._iteration = iteration
 
     @mimeo_context
-    def render(self, context: MimeoContext = None) -> str:
+    def render(
+            self,
+            context: MimeoContext = None,
+    ) -> str:
         """Render a unique identifier.
-        
+
         By default, Key Mimeo Util renders identifier from the current
         iteration of the current Mimeo Context.
         If the context name is parametrized and iteration is not, then
         identifier is pulled from the current iteration of THIS
         context. If the iteration is parametrized, then the identifier
         is pulled from the specific iteration of Mimeo Context (current
         or parametrized).
-        
+
         Parameters
         ----------
         context : MimeoContext, default None
             A current Mimeo Context injected by a decorator
 
         Returns
         -------
         str
             A unique identifier
         """
-        context = context if self._context_name is None else MimeoContextManager().get_context(self._context_name)
-        iteration = context.curr_iteration() if self._iteration is None else context.get_iteration(self._iteration)
+        if self._context_name is not None:
+            context = MimeoContextManager().get_context(self._context_name)
+        if self._iteration is None:
+            iteration = context.curr_iteration()
+        else:
+            iteration = context.get_iteration(self._iteration)
         return iteration.key
 
 
 class CityUtil(MimeoUtil):
     """A MimeoUtil implementation rendering city names.
-    
+
     It is a Mimeo Context-dependent Mimeo Util only when parametrized
     to generate unique city names.
 
     Methods
     -------
     render
         Render a city name.
@@ -487,15 +550,20 @@
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "city"
     _MIMEO_DB = MimeoDB()
 
-    def __init__(self, unique: bool = True, country: str = None, **kwargs):
+    def __init__(
+            self,
+            unique: bool = True,
+            country: str = None,
+            **kwargs,
+    ):
         """Initialize CityUtil class.
 
         Parameters
         ----------
         unique : bool, default True
             Indicates if rendered city names will be unique across
             a Mimeo Context
@@ -504,15 +572,18 @@
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
         self._unique = unique
         self._country = country
 
     @mimeo_context
-    def render(self, context: MimeoContext = None) -> str:
+    def render(
+            self,
+            context: MimeoContext = None,
+    ) -> str:
         """Render a city name.
 
         By default, City Mimeo Util generates a unique city name across
         a Mimeo Context without `country` limitation. If `country` is
         parametrized, then this Mimeo Util will render only those
         city names that lie in the specific country.
 
@@ -524,31 +595,33 @@
         Returns
         -------
         str
             A city name
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all unique cities have been consumed already
-        DataNotFound
+        DataNotFoundError
             If database does not contain any cities for the provided
             `country`
         """
         if self._country is None:
             if self._unique:
                 index = context.next_city_index()
             else:
                 index = random.randrange(MimeoDB.NUM_OF_CITIES)
             city = self._MIMEO_DB.get_city_at(index)
         else:
             country_cities = self._MIMEO_DB.get_cities_of(self._country)
             country_cities_count = len(country_cities)
             if country_cities_count == 0:
-                raise DataNotFound(f"Mimeo database does not contain any cities of provided country [{self._country}].")
+                msg = (f"Mimeo database doesn't contain any cities "
+                       f"of provided country [{self._country}].")
+                raise DataNotFoundError(msg)
 
             if self._unique:
                 index = context.next_city_index(self._country)
             else:
                 index = random.randrange(country_cities_count)
             city = country_cities[index]
 
@@ -575,15 +648,21 @@
     KEY = "country"
 
     __VALUE_NAME = "name"
     __VALUE_ISO3 = "iso3"
     __VALUE_ISO2 = "iso2"
     __MIMEO_DB = MimeoDB()
 
-    def __init__(self, value: str = None, unique: bool = True, country: str = None, **kwargs):
+    def __init__(
+            self,
+            value: str = None,
+            unique: bool = True,
+            country: str = None,
+            **kwargs,
+    ):
         """Initialize CountryUtil class.
 
         Parameters
         ----------
         value : str, default 'name'
             Indicates which country detail should be rendered:
             name, ISO3 code or ISO2 code.
@@ -596,15 +675,18 @@
             Arbitrary keyword arguments (ignored)
         """
         self._value = value if value is not None else self.__VALUE_NAME
         self._unique = unique
         self._country = country
 
     @mimeo_context
-    def render(self, context: MimeoContext = None) -> str:
+    def render(
+            self,
+            context: MimeoContext = None,
+    ) -> str:
         """Render a country name.
 
         By default, Country Mimeo Util generates a unique country name
         across a Mimeo Context. If `value` is parametrized, then it
         will render a specific country detail (name, ISO3 code or ISO2
         code). This Mimeo Util allows you to provide a `country` detail
         (e.g. ISO3 code) to get another detail (e.g. name).
@@ -621,46 +703,51 @@
         str
             A country detail
 
         Raises
         ------
         InvalidValue
             If the `country` parameter value is not supported
-        OutOfStock
+        OutOfStockError
             If all unique countries have been consumed already
-        DataNotFound
+        DataNotFoundError
             If database does not contain the provided `country`
         """
         if self._value == self.__VALUE_NAME:
             return self._get_country(context).name
-        elif self._value == self.__VALUE_ISO3:
+        if self._value == self.__VALUE_ISO3:
             return self._get_country(context).iso_3
-        elif self._value == self.__VALUE_ISO2:
+        if self._value == self.__VALUE_ISO2:
             return self._get_country(context).iso_2
-        else:
-            raise InvalidValue(f"The `country` Mimeo Util does not support such value [{self._value}]. "
-                               f"Supported values are: "
-                               f"{self.__VALUE_NAME} (default), {self.__VALUE_ISO3}, {self.__VALUE_ISO2}.")
-
-    def _get_country(self, context: MimeoContext) -> Country:
+        msg = (f"The country Mimeo Util does not support a value [{self._value}]. "
+               f"Supported values are: {self.__VALUE_NAME} (default), "
+               f"{self.__VALUE_ISO3}, {self.__VALUE_ISO2}.")
+        raise InvalidValueError(msg)
+
+    def _get_country(
+            self,
+            context: MimeoContext,
+    ) -> Country:
         if self._country is not None:
             countries = self.__MIMEO_DB.get_countries()
-            country_found = next(filter(lambda c: self._country in [c.name, c.iso_3, c.iso_2], countries), None)
-            if country_found is not None:
-                return country_found
-            else:
-                raise DataNotFound(f"Mimeo database does not contain such a country [{self._country}].")
-        else:
-            if self._unique:
-                index = context.next_country_index()
-            else:
-                index = random.randrange(MimeoDB.NUM_OF_COUNTRIES)
+            country_found = next(
+                filter(lambda c: self._country in [c.name, c.iso_3, c.iso_2],
+                       countries),
+                None,
+            )
+            if country_found is None:
+                msg = f"Mimeo database doesn't contain a country [{self._country}]."
+                raise DataNotFoundError(msg)
+            return country_found
 
-            country = self.__MIMEO_DB.get_country_at(index)
-            return country
+        if self._unique:
+            index = context.next_country_index()
+        else:
+            index = random.randrange(MimeoDB.NUM_OF_COUNTRIES)
+        return self.__MIMEO_DB.get_country_at(index)
 
 
 class FirstNameUtil(MimeoUtil):
     """A MimeoUtil implementation rendering forenames.
 
     It is a Mimeo Context-dependent Mimeo Util only when parametrized
     to generate unique forenames.
@@ -675,15 +762,20 @@
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "first_name"
     __MIMEO_DB = MimeoDB()
 
-    def __init__(self, unique: bool = True, sex: str = None, **kwargs):
+    def __init__(
+            self,
+            unique: bool = True,
+            sex: str = None,
+            **kwargs,
+    ):
         """Initialize FirstNameUtil class.
 
         Parameters
         ----------
         unique : bool, default True
             Indicates if rendered forenames will be unique across
             a Mimeo Context
@@ -692,15 +784,18 @@
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
         self._unique = unique
         self._sex = self._standardize_sex(sex)
 
     @mimeo_context
-    def render(self, context: MimeoContext = None) -> str:
+    def render(
+            self,
+            context: MimeoContext = None,
+    ) -> str:
         """Render a first name.
 
         By default, First Name Mimeo Util generates a unique forename
         across a Mimeo Context without sex limitation. If `sex` is
         parametrized, then this Mimeo Util will render only those
         first names that are assigned to the specific sex.
 
@@ -712,17 +807,17 @@
         Returns
         -------
         str
             A first name
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all unique first names have been consumed already
-        InvalidSex
+        InvalidSexError
             If the `sex` parameter value is not supported
         """
         if self._sex is None:
             if self._unique:
                 index = context.next_first_name_index()
             else:
                 index = random.randrange(MimeoDB.NUM_OF_FIRST_NAMES)
@@ -736,23 +831,25 @@
             else:
                 index = random.randrange(first_name_for_sex_count)
             first_name = first_name_for_sex[index]
 
         return first_name.name
 
     @classmethod
-    def _standardize_sex(cls, sex: str):
+    def _standardize_sex(
+            cls,
+            sex: str,
+    ):
         if sex is None:
             return sex
-        elif sex.upper() in ["M", "MALE"]:
+        if sex.upper() in ["M", "MALE"]:
             return "M"
-        elif sex.upper() in ["F", "FEMALE"]:
+        if sex.upper() in ["F", "FEMALE"]:
             return "F"
-        else:
-            raise InvalidSex(("M", "F", "Male", "Female"))
+        raise InvalidSexError(("M", "F", "Male", "Female"))
 
 
 class LastNameUtil(MimeoUtil):
     """A MimeoUtil implementation rendering surnames.
 
     It is a Mimeo Context-dependent Mimeo Util only when parametrized
     to generate unique surnames.
@@ -767,29 +864,36 @@
     KEY : str
         A Mimeo Util key
     """
 
     KEY = "last_name"
     __MIMEO_DB = MimeoDB()
 
-    def __init__(self, unique: bool = True, **kwargs):
+    def __init__(
+            self,
+            unique: bool = True,
+            **kwargs,
+    ):
         """Initialize LastNameUtil class.
 
         Parameters
         ----------
         unique : bool, default True
             Indicates if rendered forenames will be unique across
             a Mimeo Context
         kwargs : dict
             Arbitrary keyword arguments (ignored)
         """
         self._unique = unique
 
     @mimeo_context
-    def render(self, context: MimeoContext = None) -> str:
+    def render(
+            self,
+            context: MimeoContext = None,
+    ) -> str:
         """Render a last name.
 
         By default, First Name Mimeo Util generates a unique surname
         across a Mimeo Context.
 
         Parameters
         ----------
@@ -799,17 +903,15 @@
         Returns
         -------
         str
             A last name
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all unique last names have been consumed already
         """
         if self._unique:
             index = context.next_first_name_index()
         else:
             index = random.randrange(MimeoDB.NUM_OF_FIRST_NAMES)
-        last_name = self.__MIMEO_DB.get_last_name_at(index)
-
-        return last_name
+        return self.__MIMEO_DB.get_last_name_at(index)
```

### Comparing `mimeograph-0.4.2/src/mimeo/utils/renderers.py` & `mimeograph-0.4.3/src/mimeo/utils/renderers.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,26 +7,28 @@
     * UtilsRenderer
         A class rendering Mimeo Utils.
     * VarsRenderer
         A class rendering Mimeo Vars.
     * SpecialFieldsRenderer
         A class rendering Mimeo Special Fields.
 """
+from __future__ import annotations
+
 import logging
 import re
-from typing import Any, Union
+from typing import Any
 
 from mimeo.config import MimeoConfig
 from mimeo.context import MimeoContext, MimeoContextManager
 from mimeo.context.decorators import mimeo_context
 from mimeo.utils import (AutoIncrementUtil, CityUtil, CountryUtil,
                          CurrentIterationUtil, DateTimeUtil, DateUtil,
                          FirstNameUtil, KeyUtil, LastNameUtil, MimeoUtil,
                          RandomIntegerUtil, RandomItemUtil, RandomStringUtil)
-from mimeo.utils.exc import InvalidMimeoUtil, NotASpecialField
+from mimeo.utils.exc import InvalidMimeoUtilError, NotASpecialFieldError
 
 logger = logging.getLogger(__name__)
 
 
 class UtilsRenderer:
     """A class rendering Mimeo Utils.
 
@@ -53,15 +55,18 @@
         CountryUtil.KEY: CountryUtil,
         FirstNameUtil.KEY: FirstNameUtil,
         LastNameUtil.KEY: LastNameUtil,
     }
     _INSTANCES = {}
 
     @classmethod
-    def render_raw(cls, mimeo_util_key: str) -> Any:
+    def render_raw(
+            cls,
+            mimeo_util_key: str,
+    ) -> Any:
         """Render a Mimeo Util in a raw form.
 
         Parameters
         ----------
         mimeo_util_key : str
             A Mimeo Util key (name)
 
@@ -72,18 +77,23 @@
 
         Raises
         ------
         InvalidMimeoUtil
             If the Mimeo Util name does not match any existing Mimeo
             Util.
         """
-        return cls.render_parametrized({MimeoConfig.MODEL_MIMEO_UTIL_NAME_KEY: mimeo_util_key})
+        return cls.render_parametrized({
+            MimeoConfig.MODEL_MIMEO_UTIL_NAME_KEY: mimeo_util_key,
+        })
 
     @classmethod
-    def render_parametrized(cls, mimeo_util_config: dict) -> Any:
+    def render_parametrized(
+            cls,
+            mimeo_util_config: dict,
+    ) -> Any:
         """Render a Mimeo Util in a parametrized form.
 
         Parameters
         ----------
         mimeo_util_config : dict
             A Mimeo Util configuration
 
@@ -96,74 +106,82 @@
         ------
         InvalidMimeoUtil
             If the Mimeo Util configuration does not include Mimeo
             Util name, or the parametrized name does not match any
             existing Mimeo Util.
         InvalidValue
             If a Mimeo Util is incorrectly parametrized.
-        InvalidSex
+        InvalidSexError
             If the First Name Mimeo Util has not supported `sex`
             parameter value assigned.
         """
-        logger.fine(f"Rendering a mimeo util [{mimeo_util_config}]")
+        logger.fine("Rendering a mimeo util [%s]", mimeo_util_config)
         mimeo_util = cls._get_mimeo_util(mimeo_util_config)
         return mimeo_util.render()
 
     @classmethod
-    def _get_mimeo_util(cls, mimeo_util_config: dict) -> MimeoUtil:
+    def _get_mimeo_util(
+            cls,
+            config: dict,
+    ) -> MimeoUtil:
         """Get a Mimeo Util instance based on the configuration.
 
         All instances are cached to not re-create a Util with the same
         parameters. This method instantiate a Mimeo Util for the first
         time and use the one in the future.
 
         Parameters
         ----------
-        mimeo_util_config : dict
+        config : dict
             A Mimeo Util configuration
 
         Returns
         -------
         MimeoUtil
             A Mimeo Util instance
 
         Raises
         ------
         InvalidMimeoUtil
             If the Mimeo Util configuration does not include Mimeo
             Util name, or the parametrized name does not match any
             existing Mimeo Util.
         """
-        cache_key = cls._generate_cache_key(mimeo_util_config)
+        cache_key = cls._generate_cache_key(config)
         if cache_key not in cls._INSTANCES:
-            return cls._instantiate_mimeo_util(cache_key, mimeo_util_config)
-        else:
-            return cls._INSTANCES.get(cache_key)
+            return cls._instantiate_mimeo_util(cache_key, config)
+        return cls._INSTANCES.get(cache_key)
 
     @staticmethod
-    def _generate_cache_key(mimeo_util_config: dict) -> str:
+    def _generate_cache_key(
+            config: dict,
+    ) -> str:
         """Generate an internal Mimeo Util key from its parameters.
 
         This method ensures that Mimeo Util instances are cached
         properly for the same parameters.
 
         Parameters
         ----------
-        mimeo_util_config : dict
+        config : dict
             A Mimeo Util configuration
 
         Returns
         -------
         str
             An internal Mimeo Util cache key
         """
-        return "-".join(":".join([key, str(val)]) for key, val in mimeo_util_config.items())
+        return "-".join(":".join([key, str(val)]) for key, val in config.items())
 
     @classmethod
-    def _instantiate_mimeo_util(cls, cache_key: str, config: dict) -> MimeoUtil:
+    def _instantiate_mimeo_util(
+            cls,
+            cache_key: str,
+            config: dict,
+    ) -> MimeoUtil:
         """Instantiate a Mimeo Util based on the configuration.
 
         After instantiation the Mimeo Util is cached for the future.
 
         Parameters
         ----------
         cache_key : str
@@ -185,39 +203,44 @@
         """
         mimeo_util_name = cls.get_mimeo_util_name(config)
         mimeo_util = cls.MIMEO_UTILS.get(mimeo_util_name)(**config)
         cls._INSTANCES[cache_key] = mimeo_util
         return mimeo_util
 
     @classmethod
-    def get_mimeo_util_name(cls, mimeo_util_config: dict) -> str:
+    def get_mimeo_util_name(
+            cls,
+            config: dict,
+    ) -> str:
         """Return a verified Mimeo Util name.
 
         Parameters
         ----------
-        mimeo_util_config : dict
+        config : dict
             A Mimeo Util configuration
 
         Returns
         -------
         str
             A Mimeo Util name
 
         Raises
         ------
         InvalidMimeoUtil
             If the Mimeo Util configuration does not include Mimeo
             Util name, or the parametrized name does not match any
             existing Mimeo Util.
         """
-        mimeo_util_name = mimeo_util_config.get(MimeoConfig.MODEL_MIMEO_UTIL_NAME_KEY)
+        mimeo_util_name = config.get(MimeoConfig.MODEL_MIMEO_UTIL_NAME_KEY)
         if mimeo_util_name is None:
-            raise InvalidMimeoUtil(f"Missing Mimeo Util name in configuration [{mimeo_util_config}]!")
-        elif mimeo_util_name not in cls.MIMEO_UTILS:
-            raise InvalidMimeoUtil(f"No such Mimeo Util [{mimeo_util_name}]!")
+            msg = f"Missing Mimeo Util name in configuration [{config}]!"
+            raise InvalidMimeoUtilError(msg)
+        if mimeo_util_name not in cls.MIMEO_UTILS:
+            msg = f"No such Mimeo Util [{mimeo_util_name}]!"
+            raise InvalidMimeoUtilError(msg)
         return mimeo_util_name
 
 
 class VarsRenderer:
     """A class rendering Mimeo Vars.
 
     It contains only a class method.
@@ -225,15 +248,18 @@
     Methods
     -------
     render(var: str) -> Any
         Render a Mimeo Var.
     """
 
     @classmethod
-    def render(cls, var: str) -> Union[str, int, bool, dict]:
+    def render(
+            cls,
+            var: str,
+    ) -> str | int | bool | dict:
         """Render a Mimeo Var.
 
         Parameters
         ----------
         var : str
             A variable name
 
@@ -242,18 +268,18 @@
         Any
             A variable value
 
         Raises
         ------
         InstanceNotAlive
             If the MimeoContextManager instance is not alive
-        VarNotFound
+        VarNotFoundError
             If the Mimeo Var with the `var` provided does not exist
         """
-        logger.fine(f"Rendering a variable [{var}]")
+        logger.fine("Rendering a variable [%s]", var)
         return MimeoContextManager().get_var(var)
 
 
 class SpecialFieldsRenderer:
     """A class rendering Mimeo Special Fields.
 
     It contains only a class method.
@@ -262,37 +288,41 @@
     -------
     render(field_name: str, context: MimeoContext = None) -> Any
         Render a Mimeo Special Field.
     """
 
     @classmethod
     @mimeo_context
-    def render(cls, field_name: str, context: MimeoContext = None) -> Union[str, int, bool]:
+    def render(
+            cls,
+            field: str,
+            context: MimeoContext = None,
+    ) -> str | int | bool:
         """Render a Mimeo Special Field.
 
         Parameters
         ----------
-        field_name : str
+        field : str
             A special field name
         context : MimeoContext, default None
             A current Mimeo Context injected by a decorator
 
         Returns
         -------
-        Union[str, int, bool]
+        str | int | bool
 
         Raises
         ------
-        UninitializedContextIteration
+        UninitializedContextIterationError
             If no iteration has been initialized yet for the context
-        SpecialFieldNotFound
+        SpecialFieldNotFoundError
             If the special field does not exist.
         """
-        logger.fine(f"Rendering a special field [{field_name}]")
-        return context.curr_iteration().get_special_field(field_name)
+        logger.fine("Rendering a special field [%s]", field)
+        return context.curr_iteration().get_special_field(field)
 
 
 class MimeoRenderer:
     """A Facade class rendering Mimeo Utils, Vars and Special Fields.
 
     It contains only class methods.
 
@@ -311,15 +341,18 @@
     """
 
     _UTILS_PATTERN = re.compile("^{(.+)}$")
     _VARS_PATTERN = re.compile(".*({[A-Z_0-9]+})")
     _SPECIAL_FIELDS_PATTERN = re.compile(".*({:([a-zA-Z]+:)?[-_a-zA-Z0-9]+:})")
 
     @classmethod
-    def get_special_field_name(cls, wrapped_field_name: str) -> str:
+    def get_special_field_name(
+            cls,
+            wrapped_field_name: str,
+    ) -> str:
         """Extract a special field name.
 
         Parameters
         ----------
         wrapped_field_name : str
             A field name wrapped with curly braces and colons,
             e.g. {:Field:}
@@ -331,20 +364,23 @@
 
         Raises
         ------
         NotASpecialField
             If the `wrapped_field_name` is not of form {:FIELD_NAME:}
         """
         if not cls.is_special_field(wrapped_field_name):
-            raise NotASpecialField(wrapped_field_name)
+            raise NotASpecialFieldError(wrapped_field_name)
 
         return wrapped_field_name[2:][:-2]
 
     @classmethod
-    def is_special_field(cls, special_field: str) -> bool:
+    def is_special_field(
+            cls,
+            special_field: str,
+    ) -> bool:
         """Verify if the field is special (of form {:FIELD_NAME:}).
 
         Parameters
         ----------
         special_field : str
             A special field
 
@@ -353,15 +389,18 @@
         bool
             True if the field is of form {:FIELD_NAME:}. Otherwise,
             False.
         """
         return bool(re.match(r"^{:([a-zA-Z]+:)?[-_a-zA-Z0-9]+:}$", special_field))
 
     @classmethod
-    def is_raw_mimeo_util(cls, value: str) -> bool:
+    def is_raw_mimeo_util(
+            cls,
+            value: str,
+    ) -> bool:
         """Verify if the value is a raw Mimeo Util.
 
         Parameters
         ----------
         value : str
             A string value
 
@@ -372,32 +411,40 @@
             Otherwise, False.
         """
         raw_mimeo_utils = UtilsRenderer.MIMEO_UTILS.keys()
         raw_mimeo_utils_re = "^{(" + "|".join(raw_mimeo_utils) + ")}$"
         return bool(re.match(raw_mimeo_utils_re, value))
 
     @classmethod
-    def is_parametrized_mimeo_util(cls, value: dict):
+    def is_parametrized_mimeo_util(
+            cls,
+            value: dict,
+    ):
         """Verify if the value is a parametrized Mimeo Util.
 
         Parameters
         ----------
         value : dict
             A dict value
 
         Returns
         -------
         bool
             True if the value is a dictionary having only one key,
             "_mimeo_util". Otherwise, False.
         """
-        return isinstance(value, dict) and len(value) == 1 and MimeoConfig.MODEL_MIMEO_UTIL_KEY in value
+        return (isinstance(value, dict) and
+                len(value) == 1 and
+                MimeoConfig.MODEL_MIMEO_UTIL_KEY in value)
 
     @classmethod
-    def render(cls, value: Any) -> Any:
+    def render(
+            cls,
+            value: Any,
+    ) -> Any:
         """Render a value.
 
         This method renders a value accordingly to its type and form.
         If the value takes a form of Mimeo Util it is rendered as
         Mimeo Util (raw or parametrized); if it takes a form of
         a special field this renderer will try to reach it from
         the current context; when the value takes a form of a Mimeo Var,
@@ -415,46 +462,47 @@
         Any
             A rendered value
 
         Raises
         ------
         InstanceNotAlive
             If the MimeoContextManager instance is not alive
-        UninitializedContextIteration
+        UninitializedContextIterationError
             If no iteration has been initialized yet for the context
-        VarNotFound
+        VarNotFoundError
             If the Mimeo Var does not exist
         InvalidMimeoUtil
             If the Mimeo Util node has missing _name property, or it
             does not match any Mimeo Util.
         InvalidValue
             If Mimeo Util node is incorrectly parametrized
-        OutOfStock
+        OutOfStockError
             If all unique values have been consumed already
-        DataNotFound
+        DataNotFoundError
             If database does not contain the expected value
-        InvalidSex
+        InvalidSexError
             If the First Name Mimeo Util has not supported `sex`
             parameter value assigned.
         """
-        logger.fine(f"Rendering a value [{value}]")
+        logger.fine("Rendering a value [%s]", value)
         try:
             if isinstance(value, str):
-                return cls._render_string_value(value)
-            elif cls.is_parametrized_mimeo_util(value):
-                return cls._render_parametrized_mimeo_util(value)
-            else:
-                return value
-        except Exception as err:
-            error_name = type(err).__name__
-            logger.error(f"The [{error_name}] error occurred during rendering a value [{value}]: [{err}].")
-            raise err
+                value = cls._render_string_value(value)
+            if cls.is_parametrized_mimeo_util(value):
+                value = cls._render_parametrized_mimeo_util(value)
+        except Exception:
+            logger.exception("An error occurred for [%s].", value)
+            raise
+        return value
 
     @classmethod
-    def _render_string_value(cls, value: str) -> Any:
+    def _render_string_value(
+            cls,
+            value: str,
+    ) -> Any:
         """Render a string value.
 
         Depending on value form it can render it as a raw value,
         a special field, a Mimeo Var or a raw Mimeo Util.
 
         Parameters
         ----------
@@ -464,23 +512,25 @@
         Returns
         -------
         Any
             A rendered value
         """
         if cls._SPECIAL_FIELDS_PATTERN.match(value):
             return cls._render_special_field(value)
-        elif cls._VARS_PATTERN.match(value):
+        if cls._VARS_PATTERN.match(value):
             return cls._render_var(value)
-        elif cls.is_raw_mimeo_util(value):
+        if cls.is_raw_mimeo_util(value):
             return cls._render_raw_mimeo_util(value)
-        else:
-            return value
+        return value
 
     @classmethod
-    def _render_special_field(cls, value: str) -> Any:
+    def _render_special_field(
+            cls,
+            value: str,
+    ) -> Any:
         """Render a value containing a Mimeo Special Field.
 
         This method finds first special field and replaces all
         occurrences. Then the result is passed to the render() method
         again, to return a final value.
 
         Parameters
@@ -491,30 +541,33 @@
         Returns
         -------
         Any
             A rendered value
 
         Raises
         ------
-        UninitializedContextIteration
+        UninitializedContextIterationError
             If no iteration has been initialized yet for the context
-        SpecialFieldNotFound
+        SpecialFieldNotFoundError
             If the special field does not exist.
         """
         match = next(cls._SPECIAL_FIELDS_PATTERN.finditer(value))
         wrapped_special_field = match.group(1)
-        rendered_value = SpecialFieldsRenderer.render(wrapped_special_field[2:][:-2])
-        logger.fine(f"Rendered special field value [{rendered_value}]")
+        r_val = SpecialFieldsRenderer.render(wrapped_special_field[2:][:-2])
+        logger.fine("Rendered special field value [%s]", r_val)
         if len(wrapped_special_field) != len(value):
-            rendered_value = str(rendered_value).lower() if isinstance(rendered_value, bool) else str(rendered_value)
-            rendered_value = value.replace(wrapped_special_field, str(rendered_value))
-        return cls.render(rendered_value)
+            r_val = str(r_val).lower() if isinstance(r_val, bool) else str(r_val)
+            r_val = value.replace(wrapped_special_field, str(r_val))
+        return cls.render(r_val)
 
     @classmethod
-    def _render_var(cls, value: str) -> Any:
+    def _render_var(
+            cls,
+            value: str,
+    ) -> Any:
         """Render a value containing a Mimeo Var.
 
         This method finds first variable and replaces all occurrences.
         Then the result is passed to the render() method again, to
         return a final value.
 
         Parameters
@@ -527,54 +580,60 @@
         Any
             A rendered value
 
         Raises
         ------
         InstanceNotAlive
             If the MimeoContextManager instance is not alive
-        VarNotFound
+        VarNotFoundError
             If the Mimeo Var with the `var` provided does not exist
         """
         match = next(cls._VARS_PATTERN.finditer(value))
         wrapped_var = match.group(1)
-        rendered_value = VarsRenderer.render(wrapped_var[1:][:-1])
-        logger.fine(f"Rendered variable value [{rendered_value}]")
-        if cls.is_parametrized_mimeo_util(rendered_value):
-            rendered_value = cls._render_parametrized_mimeo_util(rendered_value)
+        r_val = VarsRenderer.render(wrapped_var[1:][:-1])
+        logger.fine("Rendered variable value [%s]", r_val)
+        if cls.is_parametrized_mimeo_util(r_val):
+            r_val = cls._render_parametrized_mimeo_util(r_val)
         if len(wrapped_var) != len(value):
-            rendered_value = str(rendered_value).lower() if isinstance(rendered_value, bool) else str(rendered_value)
-            rendered_value = value.replace(wrapped_var, str(rendered_value))
-        return cls.render(rendered_value)
+            r_val = str(r_val).lower() if isinstance(r_val, bool) else str(r_val)
+            r_val = value.replace(wrapped_var, str(r_val))
+        return cls.render(r_val)
 
     @classmethod
-    def _render_raw_mimeo_util(cls, value: str) -> Any:
+    def _render_raw_mimeo_util(
+            cls,
+            value: str,
+    ) -> Any:
         """Render a raw Mimeo Util.
 
         Parameters
         ----------
         value : str
             A raw Mimeo Util
 
         Returns
         -------
         Any
             A rendered value
 
         Raises
         ------
-        OutOfStock
+        OutOfStockError
             If all unique values have been consumed already
-        DataNotFound
+        DataNotFoundError
             If database does not contain the expected value
         """
         rendered_value = UtilsRenderer.render_raw(value[1:][:-1])
         return cls.render(rendered_value)
 
     @classmethod
-    def _render_parametrized_mimeo_util(cls, value: dict) -> Any:
+    def _render_parametrized_mimeo_util(
+            cls,
+            value: dict,
+    ) -> Any:
         """Render a parametrized Mimeo Util.
 
         Before the Mimeo Util itself will be rendered, first all its
         parameters (except name) are rendered.
 
         Parameters
         ----------
@@ -586,30 +645,33 @@
         Any
             A rendered value
 
         Raises
         ------
         InvalidValue
             If a Mimeo Util is incorrectly parametrized.
-        OutOfStock
+        OutOfStockError
             If all unique values have been consumed already
-        DataNotFound
+        DataNotFoundError
             If database does not contain the expected value
-        InvalidSex
+        InvalidSexError
             If the First Name Mimeo Util has not supported `sex`
             parameter value assigned.
         """
         mimeo_util = value[MimeoConfig.MODEL_MIMEO_UTIL_KEY]
         mimeo_util = cls._render_mimeo_util_parameters(mimeo_util)
-        logger.fine(f"Pre-rendered mimeo util [{mimeo_util}]")
-        rendered_value = UtilsRenderer.render_parametrized(mimeo_util)
-        return cls.render(rendered_value)
+        logger.fine("Pre-rendered mimeo util [%s]", mimeo_util)
+        r_val = UtilsRenderer.render_parametrized(mimeo_util)
+        return cls.render(r_val)
 
     @classmethod
-    def _render_mimeo_util_parameters(cls, mimeo_util_config: dict) -> dict:
+    def _render_mimeo_util_parameters(
+            cls,
+            mimeo_util_config: dict,
+    ) -> dict:
         """Render Mimeo Util's parameters.
 
         Parameters
         ----------
         mimeo_util_config : dict
             A parametrized Mimeo Util
 
@@ -618,17 +680,18 @@
         dict
             A Mimeo Util with pre-rendered parameters
 
         Raises
         ------
         InvalidValue
             If a Mimeo Util is incorrectly parametrized.
-        OutOfStock
+        OutOfStockError
             If all unique values have been consumed already
-        DataNotFound
+        DataNotFoundError
             If database does not contain the expected value
-        InvalidSex
+        InvalidSexError
             If the First Name Mimeo Util has not supported `sex`
             parameter value assigned.
         """
         logger.fine("Rendering mimeo util parameters")
-        return {key: cls.render(value) if key != "_name" else value for key, value in mimeo_util_config.items()}
+        return {key: cls.render(value) if key != "_name" else value
+                for key, value in mimeo_util_config.items()}
```

### Comparing `mimeograph-0.4.2/src/mimeograph.egg-info/PKG-INFO` & `mimeograph-0.4.3/src/mimeograph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mimeograph
-Version: 0.4.2
+Version: 0.4.3
 Summary: Generate data based on a simple template
 Author-email: "T.A. Programming Svcs." <tomasz.maciej.aniolowski@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tomasz Aniołowski
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -21,33 +21,45 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
-Keywords: mimeograph,mimeo,generate,generator
+Project-URL: GitHub, https://github.com/TomaszAniolowski/mimeo
+Keywords: mimeograph,mimeo,generate,generator,data,xml
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: test
 License-File: LICENSE
 
-
 # Mimeo (Mimeograph)
 
-**Mimeo** is a command line tool and python library generating custom data based on a template.
+[![License](https://img.shields.io/github/license/TomaszAniolowski/mimeo?label=License&style=plastic)](https://github.com/TomaszAniolowski/mimeo/blob/develop/LICENSE)
+[![Version](https://img.shields.io/pypi/v/mimeograph?color=blue&label=PyPI&style=plastic)](https://pypi.org/project/mimeograph/)  
+[![Build](https://img.shields.io/github/actions/workflow/status/TomaszAniolowski/mimeo/test.yml?color=brightgreen&label=Test%20Mimeo&style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/test.yml?query=branch%3Amain)
+[![Code Coverage](https://img.shields.io/badge/Code%20Coverage-100%25-brightgreen?style=plastic)](https://github.com/TomaszAniolowski/mimeo/actions/workflows/coverage_badge.yml?query=branch%3Amain)
+
+[Mimeo](https://github.com/TomaszAniolowski/mimeo) is a command line tool and python library generating custom data based on a template.
 It can be used by developers, testers or even business analysts in their daily work.
 
 
 ## Installation
 
 Install Mimeo with pip
 
@@ -165,31 +177,31 @@
 
 ### Mimeo CLI
 
 #### Mimeo Configuration arguments
 
 When using Mimeo command line tool you can overwrite Mimeo Configuration properties:
 
-| Short option | Long option         | Description                                                                          |
-|:------------:|:--------------------|:-------------------------------------------------------------------------------------|
-|     `-o`     | `--output`          | overwrite the `output_details/direction` property                                    |
-|     `-x`     | `--xml-declaration` | overwrite the `output_details/xml_declaration` property                              |
-|     `-i`     | `--indent`          | overwrite the `output_details/indent` property                                       |
-|     `-d`     | `--directory`       | overwrite the `output_details/directory_path` property                               |
-|     `-f`     | `--file`            | overwrite the `output_details/file_name` property                                    |
-|     `-H`     | `--http-host`       | overwrite the `output_details/host` property                                         |
-|     `-p`     | `--http-port`       | overwrite the `output_details/port` property                                         |
-|     `-E`     | `--http-endpoint`   | overwrite the `output_details/endpoint` property                                     |
-|     `-U`     | `--http-user`       | overwrite the `output_details/username` property                                     |
-|     `-P`     | `--http-password`   | overwrite the `output_details/password` property                                     |
-|              | `--http-method`     | overwrite the `output_details/method` property                                       |
-|              | `--http-protocol`   | overwrite the `output_details/protocol` property                                     |
-|              | `--http-auth`       | overwrite the `output_details/auth` property                                         |
-|     `-e`     | `--http-env`        | overwrite the output_details http properties using a mimeo environment configuration |
-|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                         |
+| Short option | Long option         | Description                                                                  |
+|:------------:|:--------------------|:-----------------------------------------------------------------------------|
+|     `-o`     | `--output`          | overwrite the `output/direction` property                            |
+|     `-x`     | `--xml-declaration` | overwrite the `output/xml_declaration` property                      |
+|     `-i`     | `--indent`          | overwrite the `output/indent` property                               |
+|     `-d`     | `--directory`       | overwrite the `output/directory_path` property                       |
+|     `-f`     | `--file`            | overwrite the `output/file_name` property                            |
+|     `-H`     | `--http-host`       | overwrite the `output/host` property                                 |
+|     `-p`     | `--http-port`       | overwrite the `output/port` property                                 |
+|     `-E`     | `--http-endpoint`   | overwrite the `output/endpoint` property                             |
+|     `-U`     | `--http-user`       | overwrite the `output/username` property                             |
+|     `-P`     | `--http-password`   | overwrite the `output/password` property                             |
+|              | `--http-method`     | overwrite the `output/method` property                               |
+|              | `--http-protocol`   | overwrite the `output/protocol` property                             |
+|              | `--http-auth`       | overwrite the `output/auth` property                                 |
+|     `-e`     | `--http-env`        | overwrite the output http properties using a mimeo env configuration |
+|              | `--http-envs-file`  | use a custom environments file (by default: mimeo.envs.json)                 |
 
 #### Logging arguments
 
 | Short option | Long option | Description       |
 |:------------:|:------------|:------------------|
 |              | `--silent`  | disable INFO logs |
 |              | `--debug`   | enable DEBUG mode |
@@ -197,29 +209,29 @@
 
 ### Mimeo Configuration
 
 Mimeo configuration is defined in a JSON file using internal settings and data templates.
 
 | Key                              |  Level   |      Required      |     Supported values     |    Default     | Description                                                                                                                                             |
 |:---------------------------------|:--------:|:------------------:|:------------------------:|:--------------:|---------------------------------------------------------------------------------------------------------------------------------------------------------|
-| `output_details`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
-| `output_details/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
-| `output_details/format`          |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
-| `output_details/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
-| `output_details/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
-| `output_details/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
-| `output_details/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
-| `output_details/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
-| `output_details/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
-| `output_details/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
-| `output_details/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
-| `output_details/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
-| `output_details/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
-| `output_details/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
-| `output_details/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
+| `output`                 |  Config  |        :x:         |          object          |      ---       | Defines output details on how it will be consumed                                                                                                       |
+| `output/direction`       |  Config  |        :x:         | `file`, `stdout`, `http` |     `file`     | Defines how output will be consumed                                                                                                                     |
+| `output/format`          |  Config  |        :x:         |          `xml`           |     `xml`      | Defines output data format                                                                                                                              |
+| `output/indent`          |  Config  |        :x:         |         integer          |     `null`     | Defines indent applied in output data                                                                                                                   |
+| `output/xml_declaration` |  Config  |        :x:         |         boolean          |    `false`     | Indicates whether an xml declaration should be added to output data                                                                                     |
+| `output/directory_path`  |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output directory                                                                                                      |
+| `output/file_name`       |  Config  |        :x:         |          string          | `mimeo-output` | For `file` direction - defines an output file name                                                                                                      |
+| `output/method`          |  Config  |        :x:         |      `POST`, `PUT`       |     `POST`     | For `http` direction - defines a request method                                                                                                         |
+| `output/protocol`        |  Config  |        :x:         |     `http`, `https`      |     `http`     | For `http` direction - defines a url protocol                                                                                                           |
+| `output/host`            |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url host                                                                                                               |
+| `output/port`            |  Config  |        :x:         |         integer          |     `null`     | For `http` direction - defines a url port (can be empty)                                                                                                |
+| `output/endpoint`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a url endpoint                                                                                                           |
+| `output/auth`            |  Config  |        :x:         |    `basic`, `digest`     |    `basic`     | For `http` direction - defines a auth method                                                                                                            |
+| `output/username`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a username                                                                                                               |
+| `output/password`        |  Config  | :heavy_check_mark: |          string          |      ---       | For `http` direction - defines a password                                                                                                               |
 | `vars`                           |  Config  |        :x:         |          object          |      ---       | Defines variables to be used in a Mimeo Template (read more in next section)                                                                            |
 | `_templates_`                    |  Config  | :heavy_check_mark: |          array           |      ---       | Stores templates for data generation                                                                                                                    |
 | `count`                          | Template | :heavy_check_mark: |         integer          |      ---       | Indicates number of copies                                                                                                                              |
 | `model`                          | Template | :heavy_check_mark: |          object          |      ---       | Defines data template to be copied                                                                                                                      |
 | `context`                        |  Model   |        :x:         |          object          |      ---       | Defines a context name that is internally used e.g. using `curr_iter()` and `get_key()` mimeo utils (by default model name is used as the context name) |
 
 #### Mimeo Environment
```

### Comparing `mimeograph-0.4.2/src/mimeograph.egg-info/SOURCES.txt` & `mimeograph-0.4.3/src/mimeograph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mimeograph-0.4.2/tests/test_mimeograph.py` & `mimeograph-0.4.3/tests/test_mimeograph.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 
 import shutil
-from os import path
+from pathlib import Path
 
 import pytest
 
 from mimeo import Mimeograph
 from mimeo.config import MimeoConfig
 from mimeo.context import MimeoContextManager
 
 
 @pytest.fixture(autouse=True)
-def teardown():
+def _teardown():
     yield
     # Teardown
     shutil.rmtree("test_mimeograph-dir")
 
 
 def test_produce():
     config = {
-        "output_details": {
+        "output": {
             "direction": "file",
             "format": "xml",
             "indent": 4,
             "xml_declaration": True,
             "directory_path": "test_mimeograph-dir",
-            "file_name": "output"
+            "file_name": "output",
         },
         "_templates_": [
             {
                 "count": 10,
                 "model": {
                     "SomeEntity": {
                         "ChildNode1": 1,
                         "ChildNode2": "value-2",
-                        "ChildNode3": True
-                    }
-                }
-            }
-        ]
+                        "ChildNode3": True,
+                    },
+                },
+            },
+        ],
     }
     mimeo_config = MimeoConfig(config)
     with MimeoContextManager(mimeo_config):
         mimeo = Mimeograph(mimeo_config)
 
-        assert not path.exists("test_mimeograph-dir")
+        assert not Path("test_mimeograph-dir").exists()
         mimeo.process()
-        assert path.exists("test_mimeograph-dir")
+        assert Path("test_mimeograph-dir").exists()
         for i in range(1, 11):
             file_path = f"test_mimeograph-dir/output-{i}.xml"
-            assert path.exists(file_path)
+            assert Path(file_path).exists()
 
-            with open(file_path, "r") as file_content:
-                assert file_content.readline() == '<?xml version="1.0" encoding="utf-8"?>\n'
-                assert file_content.readline() == '<SomeEntity>\n'
-                assert file_content.readline() == '    <ChildNode1>1</ChildNode1>\n'
-                assert file_content.readline() == '    <ChildNode2>value-2</ChildNode2>\n'
-                assert file_content.readline() == '    <ChildNode3>true</ChildNode3>\n'
-                assert file_content.readline() == '</SomeEntity>\n'
+            with Path(file_path).open() as file:
+                assert file.readline() == '<?xml version="1.0" encoding="utf-8"?>\n'
+                assert file.readline() == "<SomeEntity>\n"
+                assert file.readline() == "    <ChildNode1>1</ChildNode1>\n"
+                assert file.readline() == "    <ChildNode2>value-2</ChildNode2>\n"
+                assert file.readline() == "    <ChildNode3>true</ChildNode3>\n"
+                assert file.readline() == "</SomeEntity>\n"
```

