# Comparing `tmp/pii-extract-plg-regex-0.3.0.tar.gz` & `tmp/pii-extract-plg-regex-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pii-extract-plg-regex-0.3.0.tar", last modified: Wed Mar 22 22:06:53 2023, max compression
+gzip compressed data, was "pii-extract-plg-regex-0.4.0.tar", last modified: Wed May 10 18:09:59 2023, max compression
```

## Comparing `pii-extract-plg-regex-0.3.0.tar` & `pii-extract-plg-regex-0.4.0.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-extract-plg-regex-0.3.0/LICENSE
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       25 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/MANIFEST.in
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2542 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2280 2023-03-22 22:06:20.000000 pii-extract-plg-regex-0.3.0/README.md
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      138 2023-03-22 22:06:20.000000 pii-extract-plg-regex-0.3.0/requirements.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/setup.cfg
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2668 2023-03-17 19:24:22.000000 pii-extract-plg-regex-0.3.0/setup.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.460882 pii-extract-plg-regex-0.3.0/src/
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.464882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       18 2023-03-22 22:06:20.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      268 2023-03-20 21:11:54.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/defs.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.464882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      106 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.464882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/any/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/any/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1251 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/any/bitcoin_address.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2284 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/any/credit_card.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      449 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/any/email.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      492 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/any/ip_address.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.464882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.464882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/any/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/any/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      506 2023-03-22 22:06:20.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/any/age.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1127 2023-03-17 19:24:22.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/any/international_phone_number.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.464882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/au/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/au/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1074 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/au/abn.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      759 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/au/tfn.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.464882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/ca/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/ca/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1618 2023-03-17 19:24:22.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/ca/phone_number.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1152 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/ca/social_insurance_number.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/in_/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/in_/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      744 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/in_/aadhaar.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1794 2023-03-17 19:24:22.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/in_/phone_number.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/us/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/us/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1424 2023-01-25 22:50:31.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/us/phone_number.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      465 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/us/social_security_number.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1670 2023-03-22 22:06:20.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/us/zipcode.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/any/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/any/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      762 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/any/international_phone_number.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/es/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/es/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1218 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/es/bank_account.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1888 2023-01-25 22:50:31.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/es/govid.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1949 2023-02-20 12:24:29.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/es/phone_number.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/mx/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/mx/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1174 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/mx/curp.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1651 2023-01-25 22:50:31.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/mx/phone_number.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/ca/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/ca/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      391 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/ca/social_insurance_number.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/fr/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/fr/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2692 2023-02-20 12:24:29.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/fr/govid.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1852 2023-02-20 12:24:29.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/fr/phone_number.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      106 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/br/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/br/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      707 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/br/cpf.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/pt/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/pt/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1778 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/pt/govid.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/ro/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/ro/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/ro/ro/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/ro/ro/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1052 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/ro/ro/govid.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/zh/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/zh/__init__.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.468882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/zh/cn/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/zh/cn/__init__.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      928 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/zh/cn/govid.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1033 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/zh/cn/misc.py
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     1548 2023-03-22 22:06:20.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/plugin_loader.py
-drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-03-22 22:06:53.464882 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex.egg-info/
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     2542 2023-03-22 22:06:53.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex.egg-info/PKG-INFO
--rw-rw-r--   0 paulo     (1000) paulo     (1000)     3164 2023-03-22 22:06:53.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex.egg-info/SOURCES.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-03-22 22:06:53.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex.egg-info/dependency_links.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      106 2023-03-22 22:06:53.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex.egg-info/entry_points.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)      154 2023-03-22 22:06:53.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex.egg-info/requires.txt
--rw-rw-r--   0 paulo     (1000) paulo     (1000)       22 2023-03-22 22:06:53.000000 pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex.egg-info/top_level.txt
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)    11357 2021-11-20 15:10:50.000000 pii-extract-plg-regex-0.4.0/LICENSE
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       25 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/MANIFEST.in
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2317 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2562 2023-05-10 16:13:12.000000 pii-extract-plg-regex-0.4.0/README.md
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      138 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/requirements.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       38 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/setup.cfg
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2668 2023-03-17 19:24:22.000000 pii-extract-plg-regex-0.4.0/setup.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.185294 pii-extract-plg-regex-0.4.0/src/
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.185294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       18 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      268 2023-03-20 21:11:54.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/defs.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.185294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      106 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.185294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/any/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/any/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1251 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/any/bitcoin_address.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2284 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/any/credit_card.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1511 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/any/email.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      492 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/any/ip_address.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.185294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.185294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/any/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/any/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      511 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/any/age.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1127 2023-03-17 19:24:22.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/any/international_phone_number.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.185294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/au/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/au/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1074 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/au/abn.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1616 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/au/phone_number.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      759 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/au/tfn.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.185294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/ca/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/ca/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1699 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/ca/phone_number.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1152 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/ca/social_insurance_number.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/in_/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/in_/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      744 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/in_/aadhaar.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1911 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/in_/phone_number.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/us/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/us/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1515 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/us/phone_number.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      460 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/us/social_security_number.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1661 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/us/zipcode.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/any/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/any/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      762 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/any/international_phone_number.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/es/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/es/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1277 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/es/bank_account.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1859 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/es/govid.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2046 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/es/phone_number.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/mx/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/mx/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1163 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/mx/curp.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1705 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/mx/phone_number.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/ca/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/ca/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      391 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/ca/social_insurance_number.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/fr/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/fr/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2692 2023-02-20 12:24:29.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/fr/govid.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1862 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/fr/phone_number.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      106 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/br/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/br/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      707 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/br/cpf.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/pt/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/pt/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1778 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/pt/govid.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/ro/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/ro/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/ro/ro/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/ro/ro/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1052 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/ro/ro/govid.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/zh/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/zh/__init__.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.189294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/zh/cn/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        0 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/zh/cn/__init__.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      928 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/zh/cn/govid.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1033 2023-01-23 19:55:40.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/zh/cn/misc.py
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     1557 2023-05-10 16:13:30.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/plugin_loader.py
+drwxrwxr-x   0 paulo     (1000) paulo     (1000)        0 2023-05-10 18:09:59.185294 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex.egg-info/
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     2317 2023-05-10 18:09:59.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex.egg-info/PKG-INFO
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)     3220 2023-05-10 18:09:59.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex.egg-info/SOURCES.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)        1 2023-05-10 18:09:59.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex.egg-info/dependency_links.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      105 2023-05-10 18:09:59.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex.egg-info/entry_points.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)      154 2023-05-10 18:09:59.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex.egg-info/requires.txt
+-rw-rw-r--   0 paulo     (1000) paulo     (1000)       22 2023-05-10 18:09:59.000000 pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex.egg-info/top_level.txt
```

### Comparing `pii-extract-plg-regex-0.3.0/LICENSE` & `pii-extract-plg-regex-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/PKG-INFO` & `pii-extract-plg-regex-0.4.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 Metadata-Version: 2.1
 Name: pii-extract-plg-regex
-Version: 0.3.0
+Version: 0.4.0
 Summary: Regex modules for the extraction of PII from text chunks
 Home-page: https://github.com/piisa/pii-extract-plg-regex
+Download-URL: https://github.com/piisa/pii-extract-plg-regex/tarball/v0.4.0
 Author: Paulo Villegas
 Author-email: paulo.vllgs@gmail.com
 License: Apache
-Download-URL: https://github.com/piisa/pii-extract-plg-regex/tarball/v0.3.0
-Description: # Pii Extractor plugin: regex
-        
-        
-        This repository builds a Python package that installs a pii-extract-base
-        plugin to performs PII detection for text data based on regular expressions
-        (with optional context). The name of the plugin entry point is 
-        `piisa-detectors-regex`.
-        
-        The PII Tasks in the package are structured by language & country, since many
-        of the PII elements are language- and/or -country dependent.
-        
-        
-        ## Requirements
-        
-        The package
-         * needs at least Python 3.8
-         * needs the pii-data and the pii-extract-base base packages
-         * uses the python-stdnum package to validate numeric identifiers
-        
-        
-        ## Usage
-        
-        The package does not have any user-facing entry points, and it is used
-        automatically by the PIISA framework.
-        
-        
-        ## Building
-        
-        The provided Makefile can be used to process the package:
-         * `make pkg` will build the Python package, creating a file that can be
-           installed with `pip`
-         * `make unit` will launch all unit tests (using pytest, so pytest must be
-           available)
-         * `make install` will install the package in a Python virtualenv. The
-           virtualenv will be chosen as, in this order:
-             - the one defined in the `VENV` environment variable, if it is defined
-             - if there is a virtualenv activated in the shell, it will be used
-             - otherwise, a default is chosen as `/opt/venv/bigscience` (it will be
-               created if it does not exist)
-        
-        
-        ## Contributing
-        
-        To add a new PII processing task, please see the contributing instructions.
-        
-        
-        
 Keywords: PIISA, PII
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# Pii Extractor plugin: regex
+
+
+This repository builds a Python package that installs a pii-extract-base
+plugin to performs PII detection for text data based on regular expressions
+(with optional context). The name of the plugin entry point is 
+`piisa-detectors-regex`.
+
+The PII Tasks in the package are structured by language & country, since many
+of the PII elements are language- and/or -country dependent.
+
+
+## Requirements
+
+The package
+ * needs at least Python 3.8
+ * needs the pii-data and the pii-extract-base base packages
+ * uses the regex package (instead of the standard `re` package in the core
+   Python library)
+ * uses the python-stdnum package to validate many identifiers (and the 
+   python-phonenumbers to validate phone numbers)
+
+
+## Usage
+
+The package does not have any user-facing entry points, and it is used
+automatically by the PIISA framework.
+
+
+## Building
+
+The provided Makefile can be used to process the package:
+ * `make pkg` will build the Python package, creating a file that can be
+   installed with `pip`
+ * `make unit` will launch all unit tests (using pytest, so pytest must be
+   available)
+ * `make install` will install the package in a Python virtualenv. The
+   virtualenv will be chosen as, in this order:
+     - the one defined in the `VENV` environment variable, if it is defined
+     - if there is a virtualenv activated in the shell, it will be used
+     - otherwise, a default is chosen as `/opt/venv/bigscience` (it will be
+       created if it does not exist)
+
+
+## Contributing
+
+To add a new PII processing task, please see the contributing instructions.
+
+
```

### Comparing `pii-extract-plg-regex-0.3.0/README.md` & `pii-extract-plg-regex-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 
 ## Requirements
 
 The package
  * needs at least Python 3.8
  * needs the [pii-data] and the [pii-extract-base] base packages
- * uses the [python-stdnum] package to validate numeric identifiers
+ * uses the [regex] package (instead of the standard `re` package in the core
+   Python library)
+ * uses the [python-stdnum] package to validate many identifiers (and the 
+   [python-phonenumbers] to validate phone numbers)
 
 
 ## Usage
 
 The package does not have any user-facing entry points, and it is [used
 automatically] by the PIISA framework.
 
@@ -52,7 +55,9 @@
 [pii-extract-base]: https://github.com/piisa/pii-extract-base
 [structured by language & country]: src/pii_extract_plg_regex/modules
 [python-stdnum]: https://github.com/arthurdejong/python-stdnum
 [Makefile]: Makefile
 [pytest]: https://docs.pytest.org
 [usage]: doc/usage.md
 [contributing instructions]: doc/contributing.md
+[python-phonenumbers]: https://github.com/daviddrysdale/python-phonenumbers
+[regex]: https://github.com/mrabarnett/mrab-regex
```

### Comparing `pii-extract-plg-regex-0.3.0/setup.py` & `pii-extract-plg-regex-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/any/bitcoin_address.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/any/bitcoin_address.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/any/credit_card.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/any/credit_card.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/any/international_phone_number.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/any/international_phone_number.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/au/abn.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/au/abn.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/au/tfn.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/au/tfn.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/ca/phone_number.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/ca/phone_number.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,31 @@
 import phonenumbers
 
 from pii_data.types import PiiEnum
 
 # Regex for phone numbers
 PHONE_REGEX = r"""
    (?<! \w )
-   (?: 1[- ] )?                         # country code
+   (?: 1[- \xa0] )?                     # country code
    (?: \( \d{3} \) | \d{3} )            # area code
-   [- /]?
+   [- \xa0/]?
    \d{3}                                # central office code/exchange code
-   [- ]?
+   [- \xa0]?
    \d{4}                                # station code
    (?! [-\w] )
 """
 
 # Context that must be found around the phone number
 CONTEXT_REGEX = r"""
  \b
  (?:
    (?: tele )? phone s? |
    mobile s? |
-   call
+   call |
+   tel | cell | mob | ph\.
  )
  \b
 """
 
 # ----------------------------------------------------------------------------
 
 # compiled regex
@@ -46,27 +47,29 @@
     global _REGEX
     if _REGEX is None:
         _REGEX = re.compile(PHONE_REGEX, flags=re.X)
 
     # Find all instances
     for match in _REGEX.finditer(text):
         item_value = match.group()
-        ph = phonenumbers.parse(item_value, "CA")
+        try:
+            ph = phonenumbers.parse(item_value, "CA")
+        except phonenumbers.NumberParseException:
+            continue
         if phonenumbers.is_valid_number_for_region(ph, "CA"):
             yield item_value, match.start()
 
 # ---------------------------------------------------------------------
 
 
 PII_TASKS = {
     "class": "callable",
     "task": CA_phone_number,
     "pii": {
         "type": PiiEnum.PHONE_NUMBER,
-        "subtype": "Canadian phone number",
         "method": "soft-regex,context",
         "context": {
             "type": "regex",
             "value": CONTEXT_REGEX,
             "width": [64, 64]
         }
     }
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/ca/social_insurance_number.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/ca/social_insurance_number.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/in_/aadhaar.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/in_/aadhaar.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/us/phone_number.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/mx/phone_number.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,74 @@
 """
-US phone numbers
+Argentinian phone numbers, using only libphonenumbers
 """
 import re
 
 from typing import Iterable, Tuple
 
 import phonenumbers
 
 from pii_data.types import PiiEnum
 
 # Regex for phone numbers
 PHONE_REGEX = r"""
-   (?<! \w )
-   (?: 1[- ] )?
-   (?: \( \d{3} \) | \d{3} )
-   [- ]?
-   \d{3} [- ]? \d{4}
-   (?! [-\w] )
+  (?<![\w\+])
+  (?:
+     \d{2} [ \xa0]? \d{4} [ \xa0]? \d{4}
+     |
+     \d{3} [ \xa0]? \d{3} [ \xa0]? \d{4}
+  )
+  \b
 """
 
 # Context that must be found around the phone number
 CONTEXT_REGEX = r"""
  \b
  (?:
-   (?: tele )? phone s? |
-   mobile s? |
-   call
+   tel[ée]fonos? |
+   (?: tf | tel | tel[éf] | tfno ) \. |        # abbreviations
+   celular (?: es )? |                         # mobile
+   ll[aá]m[aeoáéó][bdilmrs]?\w*                # conjugation for "llamar"
  )
- \b
+ (?! \w )
 """
 
 # ----------------------------------------------------------------------------
 
 # compiled regex
 _REGEX = None
 
 
-def US_phone_number(text: str) -> Iterable[Tuple[str, int]]:
+def MX_phone_number(text: str) -> Iterable[Tuple[str, int]]:
     """
-    US Phone Numbers
+    Mexican phone number
     """
     # Compile regex if needed
     global _REGEX
     if _REGEX is None:
         _REGEX = re.compile(PHONE_REGEX, flags=re.X)
 
     # Find all instances
     for match in _REGEX.finditer(text):
         item_value = match.group()
-        ph = phonenumbers.parse(item_value, "US")
-        if phonenumbers.is_valid_number_for_region(ph, "US"):
+        try:
+            ph = phonenumbers.parse(item_value, "MX")
+        except phonenumbers.NumberParseException:
+            continue
+        if phonenumbers.is_valid_number_for_region(ph, "MX"):
             yield item_value, match.start()
 
-# ---------------------------------------------------------------------
 
+# ---------------------------------------------------------------------
 
 PII_TASKS = {
     "class": "callable",
-    "task": US_phone_number,
+    "task": MX_phone_number,
     "pii": {
         "type": PiiEnum.PHONE_NUMBER,
-        "subtype": "US phone number",
         "method": "soft-regex,context",
         "context": {
             "type": "regex",
             "value": CONTEXT_REGEX,
             "width": [64, 64]
         }
     }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/en/us/zipcode.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/us/zipcode.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,12 +102,12 @@
 # ---------------------------------------------------------------------
 
 
 PII_TASKS = {
     "class": "callable",
     "task": US_zipcode,
     "pii": {
-        "type": PiiEnum.STREET_ADDRESS,
-        "subtype": "US zipcode",
+        "type": PiiEnum.LOCATION,
+        "subtype": "zipcode",
         "method": "soft-regex"
     }
 }
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/any/international_phone_number.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/any/international_phone_number.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/es/bank_account.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/au/phone_number.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,50 +1,75 @@
 """
-Spanish bank account numbers (CCC - código cuenta cliente)
-
-Note: **NOT** IBAN numbers, those are country (& language) independent
+Asutralian phone numbers
 """
-
 import re
 
 from typing import Iterable, Tuple
 
-from stdnum.es import ccc
+import phonenumbers
 
 from pii_data.types import PiiEnum
 
-# ----------------------------------------------------------------------------
+# Regex for phone numbers
+PHONE_REGEX = r"""
+   (?<! \w )
+   (?:
+      (?: \( 0[2378] \) | 0[2378] ) [ \xa0]?  \d{4}  [ \xa0]?  \d{4}  # landline
+      |
+      0[45]\d{2}  [ \xa0]?  \d{3}  [ \xa0]?  \d{3}                    # mobile
+   )
+   (?! [-\w] )
+"""
 
-# regex for a Código Cuenta Cliente, with optional spaces separating the pieces
-_CCC_PATTERN = r"\d{4}\s?\d{4}\s?\d{2}\s?\d{10}"
+# Context that must be found around the phone number
+CONTEXT_REGEX = r"""
+ \b
+ (?:
+   (?: tele )? phone s? |
+   mobile s? |
+   call |
+   tel | cell | mob | ph\.
+ )
+ \b
+"""
+
+# ----------------------------------------------------------------------------
 
 # compiled regex
 _REGEX = None
 
 
-def spanish_bank_ccc(text: str) -> Iterable[Tuple[str, int]]:
+def AU_phone_number(text: str) -> Iterable[Tuple[str, int]]:
     """
-    Spanish Bank Accounts (código cuenta cliente, 10-digit code, pre-IBAN)
+    AU Phone Numbers
     """
     # Compile regex if needed
     global _REGEX
     if _REGEX is None:
-        _REGEX = re.compile(_CCC_PATTERN, flags=re.X)
+        _REGEX = re.compile(PHONE_REGEX, flags=re.X)
 
-    # Find all matches
+    # Find all instances
     for match in _REGEX.finditer(text):
-        item = match.group()
-        if ccc.is_valid(item):
-            yield item, match.start()
-
+        item_value = match.group()
+        try:
+            ph = phonenumbers.parse(item_value, "AU")
+        except phonenumbers.NumberParseException:
+            continue
+        if phonenumbers.is_valid_number_for_region(ph, "AU"):
+            yield item_value, match.start()
 
 # ---------------------------------------------------------------------
 
+
 PII_TASKS = {
     "class": "callable",
-    "task": spanish_bank_ccc,
+    "task": AU_phone_number,
     "pii": {
-        "type": PiiEnum.BANK_ACCOUNT,
-        "subtype": "Spanish Bank CCC",
-        "method": "soft-regex,checksum"
+        "type": PiiEnum.PHONE_NUMBER,
+        "method": "soft-regex,context",
+        "context": {
+            "type": "regex",
+            "value": CONTEXT_REGEX,
+            "width": [64, 64]
+        }
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/es/govid.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/es/govid.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,14 @@
 
 # ---------------------------------------------------------------------
 
 # Task descriptor
 PII_TASKS = {
     "class": "PiiTask",
     "task": Spanish_DNI_NIE,
-    "name": "Spanish DNI and NIE numbers",
+    "name": "ES DNI and NIE",
     "pii": {
         "type": PiiEnum.GOV_ID,
-        "subtype": ["Spanish DNI", "Spanish NIE"],
+        "subtype": ["DNI", "NIE"],
         "method": "regex,checksum"
     }
 }
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/es/phone_number.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/es/phone_number.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # ----------------------------------------------------------------------------
 
 # Regex for mobile & landline phone numbers.
 # Also includes the 016 Domestic abuse helpline, which by law cannot appear in phone bills
 PHONE_REGEX = r"""
   (?<![\w\+])
   (?:
-     \d{3} \s? \d{3} \s? \d{3}
+     \d{3} [ \xa0]? \d{3} [ \xa0]? \d{3}
      |
-     (?: \d{3} \s? \d{2} | \d{2} \s? \d{3}) \s? \d{2} \s? \d{2}
+     (?: \d{3} [ \xa0]? \d{2} | \d{2} [ \xa0]? \d{3}) [ \xa0]? \d{2} [ \xa0]? \d{2}
      |
      016
   )
   \b
 """
 
 # Context that must be found around the phone number
@@ -42,39 +42,41 @@
 
 # compiled regex
 _REGEX = None
 
 
 def ES_phone_number(text: str) -> Iterable[Tuple[str, int]]:
     """
-    ES Phone Numbers, mobile & landline
+    Spanish phone numbers, mobile & landline
     """
     # Compile regex if needed
     global _REGEX
     if _REGEX is None:
         _REGEX = re.compile(PHONE_REGEX, flags=re.X)
     # Find all instances
     for match in _REGEX.finditer(text):
         item_value = match.group()
         if item_value == "016":
             yield item_value, match.start()
         else:
-            ph = phonenumbers.parse(item_value, "ES")
+            try:
+                ph = phonenumbers.parse(item_value, "ES")
+            except phonenumbers.NumberParseException:
+                continue
             if phonenumbers.is_valid_number(ph):
                 yield item_value, match.start()
 
 
 # ---------------------------------------------------------------------
 
 PII_TASKS = {
     "class": "callable",
     "task": ES_phone_number,
     "pii": {
         "type": PiiEnum.PHONE_NUMBER,
-        "subtype": "ES phone number",
         "method": "soft-regex,context",
         "context": {
             "type": "regex",
             "value": CONTEXT_REGEX,
             "width": [64, 64]
         }
     }
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/mx/curp.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/es/mx/curp.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 _CURP_PATTERN = r"\b [A-Z] [AEIOU] [A-Z]{2} \d{6} [HM] [A-Z]{5} [0-9A-Z] \d \b"
 
 # -------------------------------------------------------------------------
 
 # compiled regex
 _REGEX = None
 
-def Mexican_CURP(text: str) -> Iterable[Tuple[str, int]]:
+def MX_CURP(text: str) -> Iterable[Tuple[str, int]]:
     """
-    Mexican Clave Única de Registro de Población
+    Mexican Clave Única de Registro de Población (CURP)
     """
     # Compile regex if needed
     global _REGEX
     if _REGEX is None:
         _REGEX = re.compile(_CURP_PATTERN, flags=re.X)
 
     # Find all instances
@@ -36,14 +36,14 @@
             yield item_value, match.start()
 
 
 # -------------------------------------------------------------------------
 
 PII_TASKS = {
     "class": "callable",
-    "task": Mexican_CURP,
+    "task": MX_CURP,
     "pii": {
         "type": PiiEnum.GOV_ID,
-        "subtype": "Mexican CURP",
+        "subtype": "CURP",
         "method": "strong-regex,checksum"
     }
 }
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/es/mx/phone_number.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/en/in_/phone_number.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,77 @@
 """
-Argentinian phone numbers, using only libphonenumbers
+Indian phone numbers, in English context
 """
 import re
 
 from typing import Iterable, Tuple
 
 import phonenumbers
 
 from pii_data.types import PiiEnum
 
-# Regex for phone numbers
+# Regex for Indian phone numbers
 PHONE_REGEX = r"""
-  (?<![\w\+])
-  (?:
-     \d{2} \s? \d{4} \s? \d{4}
-     |
-     \d{3} \s? \d{3} \s? \d{4}
-  )
-  \b
+   (?<! [\(\w] )
+   (?:
+      [6-9]\d{3} -? \d{6} |                                         # mobile
+      \d{3} [- ] \d{8} | \d{4} [- ]\d{7} | \d{5} [- ]\d{6} |        # just dashes
+      (?P<p1>\()? 0\d{2} (?(p1)\)) [ \xa0]? \d{4} [ \xa0]? \d{4} |  # 3-digit area code
+      (?P<p2>\()? 0\d{3} (?(p2)\)) [ \xa0]? \d{3} [ \xa0]? \d{4} |  # 4-digit area code
+      (?P<p3>\()? 0\d{4} (?(p3)\)) [ \xa0]? \d{2} [ \xa0]? \d{4}    # 5-digit area code
+   )
+   (?! [-\w] )
 """
 
+
 # Context that must be found around the phone number
 CONTEXT_REGEX = r"""
  \b
  (?:
-   tel[ée]fonos? |
-   (?: tf | tel | tel[éf] | tfno ) \. |        # abbreviations
-   celular (?: es )? |                         # mobile
-   ll[aá]m[aeoáéó][bdilmrs]?\w*                # conjugation for "llamar"
+   (?: tele )? phone s? |
+   mobile s? |
+   call |
+   tel | cell | mob | ph\.
  )
- (?! \w )
+ \b
 """
 
 # ----------------------------------------------------------------------------
 
 # compiled regex
 _REGEX = None
 
 
-def Mexican_phone_number(text: str) -> Iterable[Tuple[str, int]]:
+def Indian_phone_number(text: str) -> Iterable[Tuple[str, int]]:
     """
-    Mexican Phone Numbers
+    Indian Phone Numbers
     """
     # Compile regex if needed
     global _REGEX
     if _REGEX is None:
         _REGEX = re.compile(PHONE_REGEX, flags=re.X)
 
     # Find all instances
     for match in _REGEX.finditer(text):
         item_value = match.group()
-        ph = phonenumbers.parse(item_value, "MX")
-        if phonenumbers.is_valid_number_for_region(ph, "MX"):
+        try:
+            ph = phonenumbers.parse(item_value, "IN")
+        except phonenumbers.NumberParseException:
+            continue
+        if phonenumbers.is_valid_number_for_region(ph, "IN"):
             yield item_value, match.start()
 
-
 # ---------------------------------------------------------------------
 
+
 PII_TASKS = {
     "class": "callable",
-    "task": Mexican_phone_number,
+    "task": Indian_phone_number,
     "pii": {
         "type": PiiEnum.PHONE_NUMBER,
-        "subtype": "Mexican phone number",
         "method": "soft-regex,context",
         "context": {
             "type": "regex",
             "value": CONTEXT_REGEX,
             "width": [64, 64]
         }
     }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/fr/govid.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/fr/govid.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/fr/fr/phone_number.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/fr/fr/phone_number.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from pii_data.types import PiiEnum
 
 # ----------------------------------------------------------------------------
 
 # Regex for mobile & landline phone numbers
 PHONE_REGEX = r"""
     \b
-    0\s*[1-9]             # 0 + Area code (1-9)
-    (?:[\s.-]*\d{2}){4}   # Remaining 8 numbers (all together or by pairs)
+    0 [ \xa0]? [1-9]           # 0 + Area code (1-9)
+    (?:[ \xa0.-]*\d{2}){4}     # Remaining 8 numbers (all together or by pairs)
     \b
 """
 
 # Context that must be found around the phone number
 CONTEXT_REGEX = r"""
     \b
     t[ée]l[ée]phon((es?)|iques?) |                      # Phone & corresponding adjective
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/br/cpf.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/br/cpf.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/pt/pt/govid.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/pt/pt/govid.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/ro/ro/govid.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/ro/ro/govid.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/zh/cn/govid.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/zh/cn/govid.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/modules/zh/cn/misc.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/modules/zh/cn/misc.py`

 * *Files identical despite different names*

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex/plugin_loader.py` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex/plugin_loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 The plugin entry point
 """
 
 from pathlib import Path
 
 from typing import Dict, Iterable
 
-from pii_extract.gather.collector import FolderTaskCollector
+from pii_extract.gather.collection.sources import FolderTaskCollector
 from pii_extract.helper.logger import PiiLogger
 
 from . import VERSION, defs
 
 
 # Define the folder holding the detection modules
 _MODPATH = Path(__file__).parent / "modules"
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex.egg-info/PKG-INFO` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,68 @@
 Metadata-Version: 2.1
 Name: pii-extract-plg-regex
-Version: 0.3.0
+Version: 0.4.0
 Summary: Regex modules for the extraction of PII from text chunks
 Home-page: https://github.com/piisa/pii-extract-plg-regex
+Download-URL: https://github.com/piisa/pii-extract-plg-regex/tarball/v0.4.0
 Author: Paulo Villegas
 Author-email: paulo.vllgs@gmail.com
 License: Apache
-Download-URL: https://github.com/piisa/pii-extract-plg-regex/tarball/v0.3.0
-Description: # Pii Extractor plugin: regex
-        
-        
-        This repository builds a Python package that installs a pii-extract-base
-        plugin to performs PII detection for text data based on regular expressions
-        (with optional context). The name of the plugin entry point is 
-        `piisa-detectors-regex`.
-        
-        The PII Tasks in the package are structured by language & country, since many
-        of the PII elements are language- and/or -country dependent.
-        
-        
-        ## Requirements
-        
-        The package
-         * needs at least Python 3.8
-         * needs the pii-data and the pii-extract-base base packages
-         * uses the python-stdnum package to validate numeric identifiers
-        
-        
-        ## Usage
-        
-        The package does not have any user-facing entry points, and it is used
-        automatically by the PIISA framework.
-        
-        
-        ## Building
-        
-        The provided Makefile can be used to process the package:
-         * `make pkg` will build the Python package, creating a file that can be
-           installed with `pip`
-         * `make unit` will launch all unit tests (using pytest, so pytest must be
-           available)
-         * `make install` will install the package in a Python virtualenv. The
-           virtualenv will be chosen as, in this order:
-             - the one defined in the `VENV` environment variable, if it is defined
-             - if there is a virtualenv activated in the shell, it will be used
-             - otherwise, a default is chosen as `/opt/venv/bigscience` (it will be
-               created if it does not exist)
-        
-        
-        ## Contributing
-        
-        To add a new PII processing task, please see the contributing instructions.
-        
-        
-        
 Keywords: PIISA, PII
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
+License-File: LICENSE
+
+# Pii Extractor plugin: regex
+
+
+This repository builds a Python package that installs a pii-extract-base
+plugin to performs PII detection for text data based on regular expressions
+(with optional context). The name of the plugin entry point is 
+`piisa-detectors-regex`.
+
+The PII Tasks in the package are structured by language & country, since many
+of the PII elements are language- and/or -country dependent.
+
+
+## Requirements
+
+The package
+ * needs at least Python 3.8
+ * needs the pii-data and the pii-extract-base base packages
+ * uses the regex package (instead of the standard `re` package in the core
+   Python library)
+ * uses the python-stdnum package to validate many identifiers (and the 
+   python-phonenumbers to validate phone numbers)
+
+
+## Usage
+
+The package does not have any user-facing entry points, and it is used
+automatically by the PIISA framework.
+
+
+## Building
+
+The provided Makefile can be used to process the package:
+ * `make pkg` will build the Python package, creating a file that can be
+   installed with `pip`
+ * `make unit` will launch all unit tests (using pytest, so pytest must be
+   available)
+ * `make install` will install the package in a Python virtualenv. The
+   virtualenv will be chosen as, in this order:
+     - the one defined in the `VENV` environment variable, if it is defined
+     - if there is a virtualenv activated in the shell, it will be used
+     - otherwise, a default is chosen as `/opt/venv/bigscience` (it will be
+       created if it does not exist)
+
+
+## Contributing
+
+To add a new PII processing task, please see the contributing instructions.
+
+
```

### Comparing `pii-extract-plg-regex-0.3.0/src/pii_extract_plg_regex.egg-info/SOURCES.txt` & `pii-extract-plg-regex-0.4.0/src/pii_extract_plg_regex.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/pii_extract_plg_regex/modules/any/ip_address.py
 src/pii_extract_plg_regex/modules/en/__init__.py
 src/pii_extract_plg_regex/modules/en/any/__init__.py
 src/pii_extract_plg_regex/modules/en/any/age.py
 src/pii_extract_plg_regex/modules/en/any/international_phone_number.py
 src/pii_extract_plg_regex/modules/en/au/__init__.py
 src/pii_extract_plg_regex/modules/en/au/abn.py
+src/pii_extract_plg_regex/modules/en/au/phone_number.py
 src/pii_extract_plg_regex/modules/en/au/tfn.py
 src/pii_extract_plg_regex/modules/en/ca/__init__.py
 src/pii_extract_plg_regex/modules/en/ca/phone_number.py
 src/pii_extract_plg_regex/modules/en/ca/social_insurance_number.py
 src/pii_extract_plg_regex/modules/en/in_/__init__.py
 src/pii_extract_plg_regex/modules/en/in_/aadhaar.py
 src/pii_extract_plg_regex/modules/en/in_/phone_number.py
```

