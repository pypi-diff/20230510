# Comparing `tmp/mindee-3.7.1.tar.gz` & `tmp/mindee-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindee-3.7.1.tar", last modified: Thu Apr 20 15:50:58 2023, max compression
+gzip compressed data, was "mindee-3.8.0.tar", last modified: Wed May 10 13:39:45 2023, max compression
```

## Comparing `mindee-3.7.1.tar` & `mindee-3.8.0.tar`

### file list

```diff
@@ -1,144 +1,147 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.204862 mindee-3.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 15:50:35.000000 mindee-3.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-20 15:50:58.204862 mindee-3.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-04-20 15:50:35.000000 mindee-3.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    13956 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/cropper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/cropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/cropper/cropper_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/custom/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/custom/custom_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/eu/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/eu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/eu/license_plate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/eu/license_plate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/eu/license_plate/license_plate_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/financial/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/financial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/financial/financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/financial/financial_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/fr/bank_account_details/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/bank_account_details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee/documents/fr/carte_grise/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/carte_grise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/carte_grise/carte_grise_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/fr/carte_vitale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/carte_vitale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/fr/id_card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/id_card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/fr/id_card/id_card_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/invoice/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/line_item_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/invoice/reconstruct.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/passport/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/passport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/passport/passport_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.184860 mindee-3.7.1/mindee/documents/proof_of_address/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/proof_of_address/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/proof_of_address/proof_of_address_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.188861 mindee-3.7.1/mindee/documents/receipt/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/line_item_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/receipt/receipt_v5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.188861 mindee-3.7.1/mindee/documents/shipping_container/
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/shipping_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/shipping_container/shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.188861 mindee-3.7.1/mindee/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/us/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.188861 mindee-3.7.1/mindee/documents/us/bank_check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/us/bank_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/documents/us/bank_check/bank_check_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.192861 mindee-3.7.1/mindee/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/amount.py
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/api_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/company_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/locale.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/fields/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.192861 mindee-3.7.1/mindee/input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/input/page_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/input/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/response.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/version
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-20 15:50:35.000000 mindee-3.7.1/mindee/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.180860 mindee-3.7.1/mindee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:50:39.000000 mindee-3.7.1/mindee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 15:50:58.000000 mindee-3.7.1/mindee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-20 15:50:35.000000 mindee-3.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-20 15:50:58.204862 mindee-3.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-20 15:50:35.000000 mindee-3.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.196861 mindee-3.7.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.200862 mindee-3.7.1/tests/documents/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.200862 mindee-3.7.1/tests/documents/fr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/test_bank_account_details_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/test_carte_grise_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/test_carte_vitale_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/fr/test_id_card_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_cropper_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_custom_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_financial_document_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_financial_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_invoice_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_invoice_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_passport_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_proof_of_address_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_receipt_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_receipt_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_receipt_v5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/test_shipping_container_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.200862 mindee-3.7.1/tests/documents/us/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/us/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/documents/us/test_bank_check_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:58.204862 mindee-3.7.1/tests/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_amount.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_locale.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_payment_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/fields/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_pkg_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-20 15:50:35.000000 mindee-3.7.1/tests/test_response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-10 13:39:26.000000 mindee-3.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-10 13:39:45.412331 mindee-3.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-10 13:39:26.000000 mindee-3.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee/documents/cropper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/cropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/cropper/cropper_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee/documents/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/custom/custom_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/eu/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/eu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/eu/license_plate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/eu/license_plate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/eu/license_plate/license_plate_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/financial/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/financial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7934 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/financial/financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/financial/financial_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/bank_account_details/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/bank_account_details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/carte_grise/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/carte_grise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/carte_grise/carte_grise_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/carte_vitale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/carte_vitale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2644 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/fr/id_card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/id_card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/fr/id_card/id_card_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/invoice/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/line_item_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice/reconstruct.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/invoice_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/invoice_splitter/invoice_splitter_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/passport/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/passport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9582 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/passport/passport_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/proof_of_address/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/proof_of_address/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/proof_of_address/proof_of_address_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.404331 mindee-3.8.0/mindee/documents/receipt/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/line_item_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6719 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/receipt/receipt_v5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/documents/shipping_container/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/shipping_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/shipping_container/shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/us/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/documents/us/bank_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/us/bank_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/documents/us/bank_check/bank_check_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/api_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/company_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/fields/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/mindee/input/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/input/page_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/input/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/version
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-10 13:39:26.000000 mindee-3.8.0/mindee/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.400331 mindee-3.8.0/mindee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:39:30.000000 mindee-3.8.0/mindee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 13:39:45.000000 mindee-3.8.0/mindee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-10 13:39:26.000000 mindee-3.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-05-10 13:39:45.412331 mindee-3.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-10 13:39:26.000000 mindee-3.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.408331 mindee-3.8.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/tests/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/tests/documents/fr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/test_bank_account_details_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/test_carte_grise_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/test_carte_vitale_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/fr/test_id_card_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_cropper_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_custom_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_financial_document_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11163 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_financial_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_invoice_splitter_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_invoice_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13481 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_invoice_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_passport_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_proof_of_address_v1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_receipt_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_receipt_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_receipt_v5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/test_shipping_container_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/tests/documents/us/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/us/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/documents/us/test_bank_check_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:45.412331 mindee-3.8.0/tests/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_amount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_payment_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/fields/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-10 13:39:26.000000 mindee-3.8.0/tests/test_pkg_versions.py
```

### Comparing `mindee-3.7.1/LICENSE` & `mindee-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/PKG-INFO` & `mindee-3.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.7.1
+Version: 3.8.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.7.1/README.md` & `mindee-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/client.py` & `mindee-3.8.0/mindee/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,30 +11,30 @@
     BytesInput,
     FileInput,
     LocalInputSource,
     PathInput,
     UrlInputSource,
 )
 from mindee.logger import logger
-from mindee.response import PredictResponse
+from mindee.response import AsyncPredictResponse, PredictResponse
 
 
 def get_bound_classname(type_var) -> str:
     """Get the name of the bound class."""
     return type_var.__bound__.__name__
 
 
 class DocumentClient:
-    input_doc: Union[LocalInputSource, UrlInputSource]
+    input_doc: Optional[Union[LocalInputSource, UrlInputSource]]
     doc_configs: DocumentConfigDict
     raise_on_error: bool = True
 
     def __init__(
         self,
-        input_doc: Union[LocalInputSource, UrlInputSource],
+        input_doc: Optional[Union[LocalInputSource, UrlInputSource]],
         doc_configs: DocumentConfigDict,
         raise_on_error: bool,
     ):
         self.raise_on_error = raise_on_error
         self.doc_configs = doc_configs
         self.input_doc = input_doc
 
@@ -70,97 +70,266 @@
 
         :param page_options: If set, remove pages from the document as specified.
             This is done before sending the file to the server and is useful to avoid page limitations.
 
         :param cropper: Whether to include cropper results for each page.
             This performs a cropping operation on the server and will increase response time.
         """
+        if self.input_doc is None:
+            raise TypeError("The 'parse' function requires an input document.")
         bound_classname = get_bound_classname(document_class)
         if bound_classname != documents.CustomV1.__name__:
             endpoint_name = get_bound_classname(document_class)
         elif endpoint_name is None:
             raise RuntimeError(
                 f"endpoint_name is required when using {bound_classname} class"
             )
 
         logger.debug("Parsing document as '%s'", endpoint_name)
 
-        found = []
-        for k in self.doc_configs.keys():
-            if k[1] == endpoint_name:
-                found.append(k)
+        doc_config = self._check_config(endpoint_name, account_name)
+        if not isinstance(self.input_doc, UrlInputSource):
+            if page_options and self.input_doc.is_pdf():
+                self.input_doc.process_pdf(
+                    page_options.operation,
+                    page_options.on_min_pages,
+                    page_options.page_indexes,
+                )
+        return self._make_request(
+            document_class,
+            doc_config,
+            include_words,
+            close_file,
+            cropper,
+        )
 
-        if len(found) == 0:
-            raise RuntimeError(f"Document type not configured: {endpoint_name}")
+    def enqueue(
+        self,
+        document_class: TypeDocument,
+        endpoint_name: Optional[str] = None,
+        account_name: Optional[str] = None,
+        include_words: bool = False,
+        close_file: bool = True,
+        page_options: Optional[PageOptions] = None,
+        cropper: bool = False,
+    ) -> AsyncPredictResponse[TypeDocument]:
+        """
+        Enqueueing to an async endpoint.
 
-        if account_name:
-            config_key = (account_name, endpoint_name)
-        elif len(found) == 1:
-            config_key = found[0]
-        else:
-            usernames = [k[0] for k in found]
+        :param document_class: The document class to use.
+            The response object will be instantiated based on this parameter.
+
+        :param endpoint_name: For custom endpoints, the "API name" field in the "Settings" page of the API Builder.
+            Do not set for standard (off the shelf) endpoints.
+
+        :param account_name: For custom endpoints, your account or organization username on the API Builder.
+            This is normally not required unless you have a custom endpoint which has the
+            same name as standard (off the shelf) endpoint.
+            Do not set for standard (off the shelf) endpoints.
+
+        :param include_words: Whether to include the full text for each page.
+            This performs a full OCR operation on the server and will increase response time.
+
+        :param close_file: Whether to ``close()`` the file after parsing it.
+          Set to ``False`` if you need to access the file after this operation.
+
+        :param page_options: If set, remove pages from the document as specified.
+            This is done before sending the file to the server and is useful to avoid page limitations.
+
+        :param cropper: Whether to include cropper results for each page.
+            This performs a cropping operation on the server and will increase response time.
+        """
+        if self.input_doc is None:
+            raise TypeError("The 'enqueue' function requires an input document.")
+        bound_classname = get_bound_classname(document_class)
+        if bound_classname != documents.CustomV1.__name__:
+            endpoint_name = get_bound_classname(document_class)
+        elif endpoint_name is None:
             raise RuntimeError(
-                (
-                    "Duplicate configuration detected.\n"
-                    f"You specified a document_type '{endpoint_name}' in your custom config.\n"
-                    "To avoid confusion, please add the 'account_name' attribute to "
-                    f"the parse method, one of {usernames}."
-                )
+                f"endpoint_name is required when using {bound_classname} class"
             )
 
-        doc_config = self.doc_configs[config_key]
-        doc_config.check_api_keys()
+        logger.debug("Enqueuing document as '%s'", endpoint_name)
+
+        doc_config = self._check_config(endpoint_name, account_name)
         if not isinstance(self.input_doc, UrlInputSource):
             if page_options and self.input_doc.is_pdf():
                 self.input_doc.process_pdf(
                     page_options.operation,
                     page_options.on_min_pages,
                     page_options.page_indexes,
                 )
-        return self._make_request(
-            document_class, doc_config, include_words, close_file, cropper
-        )
+        return self._predict_async(doc_config, include_words, close_file, cropper)
+
+    def parse_queued(
+        self,
+        document_class: TypeDocument,
+        queue_id: str,
+        endpoint_name: Optional[str] = None,
+        account_name: Optional[str] = None,
+    ) -> AsyncPredictResponse[TypeDocument]:
+        """
+        Parses a queued document.
+
+        :param queue_id: queue_id received from the API
+        :param endpoint_name: For custom endpoints, the "API name" field in the "Settings" page of the API Builder.
+            Do not set for standard (off the shelf) endpoints.
+        :param account_name: For custom endpoints, your account or organization username on the API Builder.
+            This is normally not required unless you have a custom endpoint which has the
+            same name as standard (off the shelf) endpoint.
+            Do not set for standard (off the shelf) endpoints.
+        """
+        bound_classname = get_bound_classname(document_class)
+        if bound_classname != documents.CustomV1.__name__:
+            endpoint_name = get_bound_classname(document_class)
+        elif endpoint_name is None:
+            raise RuntimeError(
+                f"endpoint_name is required when using {bound_classname} class"
+            )
+
+        logger.debug("Fetching queued document as '%s'", endpoint_name)
+
+        doc_config = self._check_config(endpoint_name, account_name)
+
+        return self._get_queued_document(doc_config, queue_id)
 
     def _make_request(
         self,
         document_class: TypeDocument,
         doc_config: DocumentConfig,
         include_words: bool,
         close_file: bool,
         cropper: bool,
     ) -> PredictResponse[TypeDocument]:
         if get_bound_classname(document_class) != doc_config.document_class.__name__:
             raise RuntimeError("Document class mismatch!")
-
+        if self.input_doc is None:
+            raise TypeError(
+                "The '_make_request' class method requires an input document."
+            )
         response = doc_config.document_class.request(
             doc_config.endpoints,
             self.input_doc,
             include_words=include_words,
             close_file=close_file,
             cropper=cropper,
         )
 
         dict_response = response.json()
 
         if not response.ok and self.raise_on_error:
             raise HTTPException(
                 f"API {response.status_code} HTTP error: {json.dumps(dict_response)}"
             )
+
         return PredictResponse[TypeDocument](
             http_response=dict_response,
             doc_config=doc_config,
             input_source=self.input_doc,
             response_ok=response.ok,
         )
 
+    def _predict_async(
+        self,
+        doc_config: DocumentConfig,
+        include_words: bool = False,
+        close_file: bool = True,
+        cropper: bool = False,
+    ) -> AsyncPredictResponse[TypeDocument]:
+        """
+        Sends a document to the queue, and sends back an asynchronous predict response.
+
+        :param doc_config: Configuration of the document.
+        """
+        if self.input_doc is None:
+            raise TypeError(
+                "The '_predict_async' class method requires an input document."
+            )
+        response = doc_config.endpoints[0].predict_async_req_post(
+            self.input_doc, include_words, close_file, cropper
+        )
+
+        dict_response = response.json()
+
+        if not response.ok and self.raise_on_error:
+            raise HTTPException(
+                f"API {response.status_code} HTTP error: {json.dumps(dict_response)}"
+            )
+
+        return AsyncPredictResponse[TypeDocument](
+            http_response=dict_response,
+            doc_config=doc_config,
+            input_source=self.input_doc,
+            response_ok=response.ok,
+        )
+
+    def _get_queued_document(
+        self,
+        doc_config: DocumentConfig,
+        queue_id: str,
+    ) -> AsyncPredictResponse[TypeDocument]:
+        """
+        Fetches a document or a Job from a given queue.
+
+        :param queue_id: Queue_id received from the API
+        :param doc_config: Pre-checked document configuration.
+        """
+        queue_response = doc_config.endpoints[0].document_queue_req_get(
+            queue_id=queue_id
+        )
+
+        if (
+            not queue_response.status_code
+            or queue_response.status_code < 200
+            or queue_response.status_code > 302
+        ):
+            raise HTTPException(
+                f"API {queue_response.status_code} HTTP error: {json.dumps(queue_response.json())}"
+            )
+
+        return AsyncPredictResponse[TypeDocument](
+            http_response=queue_response.json(),
+            doc_config=doc_config,
+            input_source=self.input_doc,
+            response_ok=queue_response.ok,
+        )
+
     def close(self) -> None:
         """Close the file object."""
-        if not isinstance(self.input_doc, UrlInputSource):
+        if isinstance(self.input_doc, LocalInputSource):
             self.input_doc.file_object.close()
 
+    def _check_config(self, endpoint_name, account_name) -> DocumentConfig:
+        found = []
+        for k in self.doc_configs.keys():
+            if k[1] == endpoint_name:
+                found.append(k)
+
+        if len(found) == 0:
+            raise RuntimeError(f"Document type not configured: {endpoint_name}")
+
+        if account_name:
+            config_key = (account_name, endpoint_name)
+        elif len(found) == 1:
+            config_key = found[0]
+        else:
+            usernames = [k[0] for k in found]
+            raise RuntimeError(
+                (
+                    "Duplicate configuration detected.\n"
+                    f"You specified a document_type '{endpoint_name}' in your custom config.\n"
+                    "To avoid confusion, please add the 'account_name' attribute to "
+                    f"the parse method, one of {usernames}."
+                )
+            )
+
+        doc_config = self.doc_configs[config_key]
+        doc_config.check_api_keys()
+        return doc_config
+
 
 class ConfigSpec(NamedTuple):
     doc_class: Type[Document]
     url_name: str
     version: str
 
 
@@ -277,15 +446,21 @@
                 version="1",
             ),
             ConfigSpec(
                 doc_class=documents.eu.LicensePlateV1,
                 url_name="license_plates",
                 version="1",
             ),
+            ConfigSpec(
+                doc_class=documents.InvoiceSplitterV1,
+                url_name="invoice_splitter",
+                version="1",
+            ),
         ]
+
         for config in configs:
             config_key = (OTS_OWNER, config.doc_class.__name__)
             self._doc_configs[config_key] = self._standard_doc_config(
                 config.doc_class, config.url_name, config.version
             )
         self._doc_configs[OTS_OWNER, documents.FinancialV1.__name__] = DocumentConfig(
             document_class=documents.FinancialV1,
@@ -419,7 +594,17 @@
             url,
         )
         return DocumentClient(
             input_doc=input_doc,
             doc_configs=self._doc_configs,
             raise_on_error=self.raise_on_error,
         )
+
+    def doc_for_async(
+        self,
+    ) -> DocumentClient:
+        """Creates an empty doc for asynchronous parsing requests."""
+        return DocumentClient(
+            input_doc=None,
+            doc_configs=self._doc_configs,
+            raise_on_error=self.raise_on_error,
+        )
```

### Comparing `mindee-3.7.1/mindee/documents/__init__.py` & `mindee-3.8.0/mindee/documents/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from mindee.documents.financial import (
     FinancialDocumentV1,
     FinancialV1,
     TypeFinancialDocumentV1,
     TypeFinancialV1,
 )
 from mindee.documents.invoice import InvoiceV3, InvoiceV4, TypeInvoiceV3, TypeInvoiceV4
+from mindee.documents.invoice_splitter import InvoiceSplitterV1, TypeInvoiceSplitterV1
 from mindee.documents.passport import PassportV1, TypePassportV1
 from mindee.documents.proof_of_address import ProofOfAddressV1, TypeProofOfAddressV1
 from mindee.documents.receipt import (
     ReceiptV3,
     ReceiptV4,
     ReceiptV5,
     TypeReceiptV3,
```

### Comparing `mindee-3.7.1/mindee/documents/base.py` & `mindee-3.8.0/mindee/documents/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     orientation: Optional[OrientationField] = None
     """Page orientation"""
     cropper: List[PositionField]
     """Cropper results"""
 
     def __init__(
         self,
-        input_source: Union[LocalInputSource, UrlInputSource],
+        input_source: Optional[Union[LocalInputSource, UrlInputSource]],
         document_type: Optional[str],
         api_prediction: TypeApiPrediction,
         page_n: Optional[int] = None,
     ):
         if input_source:
             if isinstance(input_source, UrlInputSource):
                 self.filename = input_source.url
```

### Comparing `mindee-3.7.1/mindee/documents/config.py` & `mindee-3.8.0/mindee/documents/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def check_api_keys(self) -> None:
         """Raise an exception unless all API keys are present."""
         for endpoint in self.endpoints:
             if not endpoint.api_key:
                 raise RuntimeError(
                     (
                         f"Missing API key for '{endpoint.url_name} v{endpoint.version}',"
-                        "check your Client configuration.\n"
+                        " check your Client configuration.\n"
                         "You can set this using the "
                         f"'{API_KEY_ENV_NAME}' environment variable."
                     )
                 )
 
 
 DocumentConfigDict = Dict[Tuple[str, str], DocumentConfig]
```

### Comparing `mindee-3.7.1/mindee/documents/cropper/cropper_v1.py` & `mindee-3.8.0/mindee/documents/cropper/cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/custom/custom_v1.py` & `mindee-3.8.0/mindee/documents/custom/custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/eu/license_plate/license_plate_v1.py` & `mindee-3.8.0/mindee/documents/eu/license_plate/license_plate_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/financial/financial_document_v1.py` & `mindee-3.8.0/mindee/documents/financial/financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/financial/financial_v1.py` & `mindee-3.8.0/mindee/documents/financial/financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/fr/bank_account_details/bank_account_details_v1.py` & `mindee-3.8.0/mindee/documents/fr/bank_account_details/bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/fr/carte_grise/carte_grise_v1.py` & `mindee-3.8.0/mindee/documents/fr/carte_grise/carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/fr/carte_vitale/carte_vitale_v1.py` & `mindee-3.8.0/mindee/documents/fr/carte_vitale/carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/fr/id_card/id_card_v1.py` & `mindee-3.8.0/mindee/documents/fr/id_card/id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/invoice/checks.py` & `mindee-3.8.0/mindee/documents/invoice/checks.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/invoice/invoice_v3.py` & `mindee-3.8.0/mindee/documents/invoice/invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/invoice/invoice_v4.py` & `mindee-3.8.0/mindee/documents/invoice/invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/invoice/line_item_v4.py` & `mindee-3.8.0/mindee/documents/invoice/line_item_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/invoice/reconstruct.py` & `mindee-3.8.0/mindee/documents/invoice/reconstruct.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/passport/passport_v1.py` & `mindee-3.8.0/mindee/documents/passport/passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/proof_of_address/proof_of_address_v1.py` & `mindee-3.8.0/mindee/documents/proof_of_address/proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/receipt/line_item_v5.py` & `mindee-3.8.0/mindee/documents/receipt/line_item_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/receipt/receipt_v3.py` & `mindee-3.8.0/mindee/documents/receipt/receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/receipt/receipt_v4.py` & `mindee-3.8.0/mindee/documents/receipt/receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/receipt/receipt_v5.py` & `mindee-3.8.0/mindee/documents/receipt/receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/shipping_container/shipping_container_v1.py` & `mindee-3.8.0/mindee/documents/shipping_container/shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/documents/us/bank_check/bank_check_v1.py` & `mindee-3.8.0/mindee/documents/us/bank_check/bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/endpoints.py` & `mindee-3.8.0/mindee/endpoints.py`

 * *Files 20% similar despite different names*

```diff
@@ -107,41 +107,92 @@
 
         :param input_source: Input object
         :param include_words: Include raw OCR words in the response
         :param close_file: Whether to `close()` the file after parsing it.
         :param cropper: Including Mindee cropping results.
         :return: requests response
         """
+        return self._custom_request(
+            "predict", input_source, include_words, close_file, cropper
+        )
+
+    def predict_async_req_post(
+        self,
+        input_source: Union[LocalInputSource, UrlInputSource],
+        include_words: bool = False,
+        close_file: bool = True,
+        cropper: bool = False,
+    ) -> requests.Response:
+        """
+        Make an asynchronous request to POST a document for prediction.
+
+        :param input_source: Input object
+        :param include_words: Include raw OCR words in the response
+        :param close_file: Whether to `close()` the file after parsing it.
+        :param cropper: Including Mindee cropping results.
+        :return: requests response
+        """
+        return self._custom_request(
+            "predict_async", input_source, include_words, close_file, cropper
+        )
+
+    def _custom_request(
+        self,
+        route: str,
+        input_source: Union[LocalInputSource, UrlInputSource],
+        include_words: bool = False,
+        close_file: bool = True,
+        cropper: bool = False,
+    ):
         data = {}
         if include_words:
             data["include_mvision"] = "true"
 
         params = {}
         if cropper:
             params["cropper"] = "true"
 
         if isinstance(input_source, UrlInputSource):
             data["document"] = input_source.url
             response = requests.post(
-                f"{self._url_root}/predict",
+                f"{self._url_root}/{route}",
                 headers=self.base_headers,
                 data=data,
                 params=params,
                 timeout=self._request_timeout,
             )
         else:
             files = {"document": input_source.read_contents(close_file)}
             response = requests.post(
-                f"{self._url_root}/predict",
+                f"{self._url_root}/{route}",
                 files=files,
                 headers=self.base_headers,
                 data=data,
                 params=params,
                 timeout=self._request_timeout,
             )
+
+        return response
+
+    def document_queue_req_get(self, queue_id: str) -> requests.Response:
+        """
+        Sends a request matching a given queue_id. Returns either a Job or a Document.
+
+        :param queue_id: queue_id received from the API
+        :param include_words: Whether to include the full text for each page.
+            This performs a full OCR operation on the server and will increase response time.
+        :param cropper: Whether to include cropper results for each page.
+            This performs a cropping operation on the server and will increase response time.
+
+        """
+        response = requests.get(
+            f"{self._url_root}/documents/queue/{queue_id}",
+            headers=self.base_headers,
+            timeout=self._request_timeout,
+        )
         return response
 
 
 class CustomEndpoint(Endpoint):
     def training_req_post(
         self, input_source: LocalInputSource, close_file: bool = True
     ) -> requests.Response:
```

### Comparing `mindee-3.7.1/mindee/fields/amount.py` & `mindee-3.8.0/mindee/fields/amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/api_builder.py` & `mindee-3.8.0/mindee/fields/api_builder.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/base.py` & `mindee-3.8.0/mindee/fields/base.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/company_registration.py` & `mindee-3.8.0/mindee/fields/company_registration.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/date.py` & `mindee-3.8.0/mindee/fields/date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/locale.py` & `mindee-3.8.0/mindee/fields/locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/orientation.py` & `mindee-3.8.0/mindee/fields/orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/payment_details.py` & `mindee-3.8.0/mindee/fields/payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/position.py` & `mindee-3.8.0/mindee/fields/position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/tax.py` & `mindee-3.8.0/mindee/fields/tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/fields/text.py` & `mindee-3.8.0/mindee/fields/text.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/geometry.py` & `mindee-3.8.0/mindee/geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """Minimum"""
     max: float
     """Maximum"""
 
 
 class Polygon(list):
     """
-    Contains any number of vertices coordinates (Points).
+    Contains any number of vertex coordinates (Points).
 
     Inherits from base class ``list`` so is compatible with type ``Points``.
     """
 
 
 Points = Sequence[Point]
```

### Comparing `mindee-3.7.1/mindee/input/page_options.py` & `mindee-3.8.0/mindee/input/page_options.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/input/sources.py` & `mindee-3.8.0/mindee/input/sources.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee/versions.py` & `mindee-3.8.0/mindee/versions.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/mindee.egg-info/PKG-INFO` & `mindee-3.8.0/mindee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindee
-Version: 3.7.1
+Version: 3.8.0
 Summary: Mindee API helper library for Python
 Home-page: https://mindee.com/
 Author: Mindee
 Author-email: devrel@mindee.com
 License: MIT
 Project-URL: Documentation, https://developers.mindee.com/docs/python-sdk
 Project-URL: Source, https://github.com/publicMindee/mindee-api-python
```

### Comparing `mindee-3.7.1/mindee.egg-info/SOURCES.txt` & `mindee-3.8.0/mindee.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,16 @@
 mindee/documents/fr/id_card/id_card_v1.py
 mindee/documents/invoice/__init__.py
 mindee/documents/invoice/checks.py
 mindee/documents/invoice/invoice_v3.py
 mindee/documents/invoice/invoice_v4.py
 mindee/documents/invoice/line_item_v4.py
 mindee/documents/invoice/reconstruct.py
+mindee/documents/invoice_splitter/__init__.py
+mindee/documents/invoice_splitter/invoice_splitter_v1.py
 mindee/documents/passport/__init__.py
 mindee/documents/passport/passport_v1.py
 mindee/documents/proof_of_address/__init__.py
 mindee/documents/proof_of_address/proof_of_address_v1.py
 mindee/documents/receipt/__init__.py
 mindee/documents/receipt/line_item_v5.py
 mindee/documents/receipt/receipt_v3.py
@@ -79,20 +81,20 @@
 mindee/input/page_options.py
 mindee/input/sources.py
 tests/test_cli.py
 tests/test_client.py
 tests/test_geometry.py
 tests/test_inputs.py
 tests/test_pkg_versions.py
-tests/test_response.py
 tests/documents/__init__.py
 tests/documents/test_cropper_v1.py
 tests/documents/test_custom_v1.py
 tests/documents/test_financial_document_v1.py
 tests/documents/test_financial_v1.py
+tests/documents/test_invoice_splitter_v1.py
 tests/documents/test_invoice_v3.py
 tests/documents/test_invoice_v4.py
 tests/documents/test_passport_v1.py
 tests/documents/test_proof_of_address_v1.py
 tests/documents/test_receipt_v3.py
 tests/documents/test_receipt_v4.py
 tests/documents/test_receipt_v5.py
```

### Comparing `mindee-3.7.1/pyproject.toml` & `mindee-3.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/setup.cfg` & `mindee-3.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/fr/test_bank_account_details_v1.py` & `mindee-3.8.0/tests/documents/fr/test_bank_account_details_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/fr/test_carte_grise_v1.py` & `mindee-3.8.0/tests/documents/fr/test_carte_grise_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/fr/test_carte_vitale_v1.py` & `mindee-3.8.0/tests/documents/fr/test_carte_vitale_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/fr/test_id_card_v1.py` & `mindee-3.8.0/tests/documents/fr/test_id_card_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_cropper_v1.py` & `mindee-3.8.0/tests/documents/test_cropper_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_custom_v1.py` & `mindee-3.8.0/tests/documents/test_custom_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_financial_document_v1.py` & `mindee-3.8.0/tests/documents/test_financial_document_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_financial_v1.py` & `mindee-3.8.0/tests/documents/test_financial_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_invoice_v3.py` & `mindee-3.8.0/tests/documents/test_invoice_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_invoice_v4.py` & `mindee-3.8.0/tests/documents/test_invoice_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_passport_v1.py` & `mindee-3.8.0/tests/documents/test_passport_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_proof_of_address_v1.py` & `mindee-3.8.0/tests/documents/test_proof_of_address_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_receipt_v3.py` & `mindee-3.8.0/tests/documents/test_receipt_v3.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_receipt_v4.py` & `mindee-3.8.0/tests/documents/test_receipt_v4.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_receipt_v5.py` & `mindee-3.8.0/tests/documents/test_receipt_v5.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/test_shipping_container_v1.py` & `mindee-3.8.0/tests/documents/test_shipping_container_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/documents/us/test_bank_check_v1.py` & `mindee-3.8.0/tests/documents/us/test_bank_check_v1.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/fields/test_amount.py` & `mindee-3.8.0/tests/fields/test_amount.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/fields/test_date.py` & `mindee-3.8.0/tests/fields/test_date.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/fields/test_field.py` & `mindee-3.8.0/tests/fields/test_field.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/fields/test_locale.py` & `mindee-3.8.0/tests/fields/test_locale.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/fields/test_orientation.py` & `mindee-3.8.0/tests/fields/test_orientation.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/fields/test_payment_details.py` & `mindee-3.8.0/tests/fields/test_payment_details.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/fields/test_position.py` & `mindee-3.8.0/tests/fields/test_position.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/fields/test_tax.py` & `mindee-3.8.0/tests/fields/test_tax.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/test_client.py` & `mindee-3.8.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/test_geometry.py` & `mindee-3.8.0/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/test_inputs.py` & `mindee-3.8.0/tests/test_inputs.py`

 * *Files identical despite different names*

### Comparing `mindee-3.7.1/tests/test_pkg_versions.py` & `mindee-3.8.0/tests/test_pkg_versions.py`

 * *Files identical despite different names*

