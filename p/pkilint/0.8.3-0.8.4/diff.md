# Comparing `tmp/pkilint-0.8.3.tar.gz` & `tmp/pkilint-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkilint-0.8.3.tar", last modified: Mon May  8 20:14:59 2023, max compression
+gzip compressed data, was "pkilint-0.8.4.tar", last modified: Wed May 10 13:20:29 2023, max compression
```

## Comparing `pkilint-0.8.3.tar` & `pkilint-0.8.4.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.426457 pkilint-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-08 20:14:49.000000 pkilint-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-08 20:14:59.426457 pkilint-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-05-08 20:14:49.000000 pkilint-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-08 20:14:49.000000 pkilint-0.8.3/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.410457 pkilint-0.8.3/pkilint/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint/adobe/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/adobe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/adobe/adobe_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint/adobe/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/adobe/asn1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/convert_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_cabf_serverauth_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_cabf_smime_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_pkix_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint/cabf/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_crl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/cabf_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/cabf/servercert/
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/cabf/servercert/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/asn1/ev_guidelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/servercert_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/servercert_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/servercert_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/servercert/servercert_name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/cabf/smime/
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/smime_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/smime_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/smime_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/cabf/smime/smime_name.py
--rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/document.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/etsi/
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/etsi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/etsi/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/etsi/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/etsi/asn1/en_319_412_5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/etsi/asn1/ts_119_495.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/iso/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/iso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/iso/lei.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/itu/bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/itu/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/itu/x520_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/msft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/msft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.418457 pkilint-0.8.3/pkilint/msft/asn1/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/msft/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/msft/msft_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/oid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/pkilint/pkix/
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/pkilint/pkix/certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26221 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/certificate/certificate_validity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/pkilint/pkix/crl/
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/crl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/crl/crl_extension.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/crl/crl_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/crl/crl_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/extension.py
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/general_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/name.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/pkilint/pkix/ocsp/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/ocsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_basic_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_validity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/pkix/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-08 20:14:49.000000 pkilint-0.8.3/pkilint/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.414457 pkilint-0.8.3/pkilint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:14:59.000000 pkilint-0.8.3/pkilint.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-08 20:14:59.426457 pkilint-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-08 20:14:49.000000 pkilint-0.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.422457 pkilint-0.8.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.426457 pkilint-0.8.3/tests/integration_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/integration_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/integration_certificate/test_cabf_smime_cert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/integration_certificate/test_pkix_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:59.426457 pkilint-0.8.3/tests/itu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/itu/test_bitstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/itu/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-08 20:14:49.000000 pkilint-0.8.3/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-10 13:20:20.000000 pkilint-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-10 13:20:29.015799 pkilint-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11263 2023-05-10 13:20:20.000000 pkilint-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-10 13:20:20.000000 pkilint-0.8.4/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.007799 pkilint-0.8.4/pkilint/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.007799 pkilint-0.8.4/pkilint/adobe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/adobe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/adobe/adobe_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.007799 pkilint-0.8.4/pkilint/adobe/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/adobe/asn1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/convert_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_cabf_serverauth_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_pkix_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/cabf/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11939 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/cabf_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/cabf/servercert/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/cabf/servercert/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/asn1/ev_guidelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/servercert_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/servercert_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/servercert_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/servercert/servercert_name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/cabf/smime/
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/smime_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/smime_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/smime_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/cabf/smime/smime_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13154 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/document.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/etsi/
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/etsi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/etsi/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/etsi/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/etsi/asn1/en_319_412_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/etsi/asn1/ts_119_495.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/iso/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/iso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/iso/lei.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/itu/bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/itu/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/itu/x520_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/msft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/msft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.011799 pkilint-0.8.4/pkilint/msft/asn1/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/msft/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/msft/msft_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/oid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/pkilint/pkix/
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/pkilint/pkix/certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26221 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7570 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/certificate/certificate_validity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/pkilint/pkix/crl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/crl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/crl/crl_extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/crl/crl_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/crl/crl_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/general_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7476 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/name.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/pkilint/pkix/ocsp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/ocsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_basic_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_validity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/pkix/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5799 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-10 13:20:20.000000 pkilint-0.8.4/pkilint/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.007799 pkilint-0.8.4/pkilint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-10 13:20:29.000000 pkilint-0.8.4/pkilint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 13:20:28.000000 pkilint-0.8.4/pkilint.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-10 13:20:29.015799 pkilint-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 13:20:20.000000 pkilint-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/tests/integration_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/integration_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/integration_certificate/test_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/integration_certificate/test_pkix_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:29.015799 pkilint-0.8.4/tests/itu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/itu/test_bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/itu/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-10 13:20:20.000000 pkilint-0.8.4/tests/util.py
```

### Comparing `pkilint-0.8.3/LICENSE` & `pkilint-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/PKG-INFO` & `pkilint-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.3
+Version: 0.8.4
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pkilint-0.8.3/README.md` & `pkilint-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/adobe/adobe_validator.py` & `pkilint-0.8.4/pkilint/adobe/adobe_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/adobe/asn1/__init__.py` & `pkilint-0.8.4/pkilint/adobe/asn1/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/bin/convert_cert.py` & `pkilint-0.8.4/pkilint/bin/convert_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/bin/lint_cabf_serverauth_cert.py` & `pkilint-0.8.4/pkilint/bin/lint_cabf_serverauth_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/bin/lint_cabf_smime_cert.py` & `pkilint-0.8.4/pkilint/bin/lint_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/bin/lint_crl.py` & `pkilint-0.8.4/pkilint/bin/lint_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/bin/lint_ocsp_response.py` & `pkilint-0.8.4/pkilint/bin/lint_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/bin/lint_pkix_cert.py` & `pkilint-0.8.4/pkilint/bin/lint_pkix_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/bin/lint_pkix_signer_signee_cert_chain.py` & `pkilint-0.8.4/pkilint/bin/lint_pkix_signer_signee_cert_chain.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/__init__.py` & `pkilint-0.8.4/pkilint/cabf/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/cabf_constants.py` & `pkilint-0.8.4/pkilint/cabf/cabf_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/cabf_crl.py` & `pkilint-0.8.4/pkilint/cabf/cabf_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/cabf_extension.py` & `pkilint-0.8.4/pkilint/cabf/cabf_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/cabf_key.py` & `pkilint-0.8.4/pkilint/cabf/cabf_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/cabf_name.py` & `pkilint-0.8.4/pkilint/cabf/cabf_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/servercert/__init__.py` & `pkilint-0.8.4/pkilint/cabf/servercert/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/servercert/asn1/ev_guidelines.py` & `pkilint-0.8.4/pkilint/cabf/servercert/asn1/ev_guidelines.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/servercert/servercert_extension.py` & `pkilint-0.8.4/pkilint/cabf/servercert/servercert_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/servercert/servercert_key.py` & `pkilint-0.8.4/pkilint/cabf/servercert/servercert_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/servercert/servercert_name.py` & `pkilint-0.8.4/pkilint/cabf/servercert/servercert_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/smime/__init__.py` & `pkilint-0.8.4/pkilint/cabf/smime/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,25 +18,24 @@
 from pkilint.iso import lei
 import pkilint.adobe.asn1 as adobe_asn1
 from pkilint.adobe import adobe_validator
 from pkilint.msft import msft_name
 from pkilint.pkix import certificate, time
 from pkilint.pkix.general_name import OTHER_NAME_MAPPINGS as PKIX_OTHERNAME_MAPPINGS
 
-
 OTHER_NAME_MAPPINGS = {
     **PKIX_OTHERNAME_MAPPINGS,
     rfc8398.id_on_SmtpUTF8Mailbox: rfc8398.SmtpUTF8Mailbox(),
     microsoft_asn1.id_on_UserPrincipalName: microsoft_asn1.UserPrincipalName(),
 }
 
 
 def determine_validation_level_and_generation(cert,
                                               config: Mapping[univ.ObjectIdentifier,
-                                                Tuple[
+                                              Tuple[
                                                   smime_constants.ValidationLevel, smime_extension.Generation]] = None):
     crypto_cert = cert.cryptography_object
 
     try:
         ext = crypto_cert.extensions.get_extension_for_oid(x509.OID_CERTIFICATE_POLICIES)
 
         oids = {ObjectIdentifier(pi.policy_identifier.dotted_string) for pi in ext.value}
@@ -61,43 +60,46 @@
     return None
 
 
 def _has_subject_attr(cert, attr):
     return any(cert.get_subject_attributes_by_type(attr))
 
 
-def _get_first_subject_attr_value(cert, attr, attr_asn1_cls):
+def _get_first_subject_attr_dirstring_value(cert, attr, attr_asn1_cls):
     attrs = cert.get_subject_attributes_by_type(attr)
 
     if any(attrs):
         attr, _ = attrs[0]
 
         attr_value_pdu = attr.children['value'].pdu
 
         decoded_value = document.decode_substrate(cert, attr_value_pdu, attr_asn1_cls())
 
-        return str(decoded_value.pdu)
+        # assume DirectoryString
+        _, attr_value_choice_value = decoded_value.child
+
+        return str(attr_value_choice_value.pdu)
     else:
         return None
 
 
 def guess_validation_level_and_generation(cert,
                                           config: Mapping[univ.ObjectIdentifier,
-                                            Tuple[smime_constants.ValidationLevel, smime_extension.Generation]]=None):
+                                          Tuple[smime_constants.ValidationLevel, smime_extension.Generation]] = None):
     v_g = determine_validation_level_and_generation(cert, config)
 
     if v_g is not None:
         return v_g
 
     # assume Legacy generation
     g = smime_constants.Generation.LEGACY
 
-    o = _get_first_subject_attr_value(cert, rfc5280.id_at_organizationName, rfc5280.X520OrganizationName)
+    o = _get_first_subject_attr_dirstring_value(cert, rfc5280.id_at_organizationName, rfc5280.X520OrganizationName)
     has_o = o is not None
-    cn = _get_first_subject_attr_value(cert, rfc5280.id_at_commonName, rfc5280.X520CommonName)
+    cn = _get_first_subject_attr_dirstring_value(cert, rfc5280.id_at_commonName, rfc5280.X520CommonName)
     has_cn = cn is not None
     has_natural_name = _has_subject_attr(cert, rfc5280.id_at_surname) or _has_subject_attr(
         cert, rfc5280.id_at_givenName)
 
     if has_o and (has_natural_name or (has_cn and o != cn and '@' not in cn)):
         v = smime_constants.ValidationLevel.SPONSORED
     elif has_o:
```

### Comparing `pkilint-0.8.3/pkilint/cabf/smime/smime_constants.py` & `pkilint-0.8.4/pkilint/cabf/smime/smime_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/smime/smime_extension.py` & `pkilint-0.8.4/pkilint/cabf/smime/smime_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/smime/smime_key.py` & `pkilint-0.8.4/pkilint/cabf/smime/smime_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/cabf/smime/smime_name.py` & `pkilint-0.8.4/pkilint/cabf/smime/smime_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/document.py` & `pkilint-0.8.4/pkilint/document.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/etsi/__init__.py` & `pkilint-0.8.4/pkilint/etsi/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/etsi/asn1/en_319_412_5.py` & `pkilint-0.8.4/pkilint/etsi/asn1/en_319_412_5.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/etsi/asn1/ts_119_495.py` & `pkilint-0.8.4/pkilint/etsi/asn1/ts_119_495.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/iso/lei.py` & `pkilint-0.8.4/pkilint/iso/lei.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/itu/bitstring.py` & `pkilint-0.8.4/pkilint/itu/bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/itu/string.py` & `pkilint-0.8.4/pkilint/itu/string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/itu/x520_name.py` & `pkilint-0.8.4/pkilint/itu/x520_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/loader.py` & `pkilint-0.8.4/pkilint/loader.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/msft/msft_name.py` & `pkilint-0.8.4/pkilint/msft/msft_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/__init__.py` & `pkilint-0.8.4/pkilint/pkix/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/algorithm.py` & `pkilint-0.8.4/pkilint/pkix/algorithm.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/certificate/__init__.py` & `pkilint-0.8.4/pkilint/pkix/certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/certificate/certificate_extension.py` & `pkilint-0.8.4/pkilint/pkix/certificate/certificate_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/certificate/certificate_key.py` & `pkilint-0.8.4/pkilint/pkix/certificate/certificate_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/certificate/certificate_name.py` & `pkilint-0.8.4/pkilint/pkix/certificate/certificate_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/certificate/certificate_validator.py` & `pkilint-0.8.4/pkilint/pkix/certificate/certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/certificate/certificate_validity.py` & `pkilint-0.8.4/pkilint/pkix/certificate/certificate_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/crl/__init__.py` & `pkilint-0.8.4/pkilint/pkix/crl/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/crl/crl_extension.py` & `pkilint-0.8.4/pkilint/pkix/crl/crl_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/crl/crl_validator.py` & `pkilint-0.8.4/pkilint/pkix/crl/crl_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/crl/crl_validity.py` & `pkilint-0.8.4/pkilint/pkix/crl/crl_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/extension.py` & `pkilint-0.8.4/pkilint/pkix/extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/general_name.py` & `pkilint-0.8.4/pkilint/pkix/general_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/name.py` & `pkilint-0.8.4/pkilint/pkix/name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/ocsp/__init__.py` & `pkilint-0.8.4/pkilint/pkix/ocsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_basic_response.py` & `pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_basic_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_response.py` & `pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/ocsp/ocsp_validity.py` & `pkilint-0.8.4/pkilint/pkix/ocsp/ocsp_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/pkix/time.py` & `pkilint-0.8.4/pkilint/pkix/time.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/report.py` & `pkilint-0.8.4/pkilint/report.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/util.py` & `pkilint-0.8.4/pkilint/util.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint/validation.py` & `pkilint-0.8.4/pkilint/validation.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/pkilint.egg-info/PKG-INFO` & `pkilint-0.8.4/pkilint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.8.3
+Version: 0.8.4
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pkilint-0.8.3/pkilint.egg-info/SOURCES.txt` & `pkilint-0.8.4/pkilint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/setup.cfg` & `pkilint-0.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/tests/integration_certificate/__init__.py` & `pkilint-0.8.4/tests/integration_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/tests/integration_certificate/test_cabf_smime_cert.py` & `pkilint-0.8.4/tests/integration_certificate/test_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/tests/integration_certificate/test_pkix_cert.py` & `pkilint-0.8.4/tests/integration_certificate/test_pkix_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/tests/itu/test_bitstring.py` & `pkilint-0.8.4/tests/itu/test_bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/tests/itu/test_string.py` & `pkilint-0.8.4/tests/itu/test_string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.8.3/tests/util.py` & `pkilint-0.8.4/tests/util.py`

 * *Files identical despite different names*

