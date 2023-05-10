# Comparing `tmp/pyocf-1.0.0.tar.gz` & `tmp/pyocf-1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyocf-1.0.0.tar", last modified: Wed May 10 11:03:21 2023, max compression
+gzip compressed data, was "pyocf-1.0b1.tar", last modified: Wed Mar 15 20:14:42 2023, max compression
```

## Comparing `pyocf-1.0.0.tar` & `pyocf-1.0b1.tar`

### file list

```diff
@@ -1,260 +1,259 @@
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.110310 pyocf-1.0.0/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      442 2023-05-10 11:03:20.000000 pyocf-1.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      339 2023-05-10 11:03:20.000000 pyocf-1.0.0/.readthedocs.yaml
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      181 2023-05-10 11:03:20.000000 pyocf-1.0.0/CHANGES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1092 2023-05-10 11:03:20.000000 pyocf-1.0.0/LICENSE.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      217 2023-05-10 11:03:20.000000 pyocf-1.0.0/MANIFEST.in
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1551 2023-05-10 11:03:20.000000 pyocf-1.0.0/Makefile
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1532 2023-05-10 11:03:21.110310 pyocf-1.0.0/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      301 2023-05-10 11:03:20.000000 pyocf-1.0.0/README.rst
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1400 2023-05-10 11:03:21.110310 pyocf-1.0.0/setup.cfg
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-05-10 11:03:20.000000 pyocf-1.0.0/setup.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.090310 pyocf-1.0.0/src/
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.090310 pyocf-1.0.0/src/pyocf/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    13995 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/api.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7774 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/captable.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.094310 pyocf-1.0.0/src/pyocf/enums/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      641 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/accrualperiodtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      525 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/addresstype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1748 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/allocationtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      526 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/compensationtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      544 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/compoundingtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      912 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/conversionmechanismtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      695 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/conversionrighttype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      749 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/conversiontimingtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1239 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/conversiontriggertype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      585 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/convertibletype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      580 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/daycounttype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      525 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/emailtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1043 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/filetype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      594 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/interestpayouttype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2833 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/objecttype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      607 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/ocfversiontype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      507 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/optiontype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      664 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/parentsecuritytype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      527 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/periodtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      558 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/phonetype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      531 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/roundingtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      997 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/stakeholderrelationshiptype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      624 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/stakeholdertype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      520 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/stockclasstype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      859 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/terminationwindowtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      477 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/valuationtype.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3003 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/vestingdayofmonth.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      698 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/enums/vestingtriggertype.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.094310 pyocf-1.0.0/src/pyocf/files/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/files/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3583 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/files/ocfmanifestfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      775 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/files/stakeholdersfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      776 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/files/stockclassesfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      879 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/files/stocklegendtemplatesfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      760 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/files/stockplansfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5299 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/files/transactionsfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      755 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/files/valuationsfile.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      784 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/files/vestingtermsfile.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1907 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/issuer.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1731 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/stakeholder.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3252 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/stockclass.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      909 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/stocklegendtemplate.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1602 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/stockplan.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1816 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/convertibleacceptance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1826 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/plansecurityacceptance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1777 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/stockacceptance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1789 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/warrantacceptance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/adjustment/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/adjustment/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1709 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/adjustment/stockclassauthorizedsharesadjustment.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2556 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/adjustment/stockclassconversionratioadjustment.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1991 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/adjustment/stockplanpooladjustment.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2141 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/convertiblecancellation.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2161 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/plansecuritycancellation.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2119 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/stockcancellation.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2131 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/warrantcancellation.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/conversion/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/conversion/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2953 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/conversion/convertibleconversion.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2147 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/conversion/stockconversion.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/exercise/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/exercise/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2158 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/exercise/plansecurityexercise.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2133 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/exercise/warrantexercise.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/issuance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/issuance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4654 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/issuance/convertibleissuance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3609 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/issuance/plansecurityissuance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3672 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/issuance/stockissuance.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4528 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/issuance/warrantissuance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/reissuance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/reissuance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2187 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/reissuance/stockreissuance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/release/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/release/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2463 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/release/plansecurityrelease.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.098310 pyocf-1.0.0/src/pyocf/objects/transactions/repurchase/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/repurchase/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2271 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/repurchase/stockrepurchase.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/objects/transactions/retraction/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/retraction/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1873 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/retraction/convertibleretraction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1865 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/retraction/plansecurityretraction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1834 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/retraction/stockretraction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1846 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/retraction/warrantretraction.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/objects/transactions/split/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/split/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1397 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/split/stockclasssplit.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/objects/transactions/transfer/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/transfer/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2356 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/transfer/convertibletransfer.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2326 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/transfer/plansecuritytransfer.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2334 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/transfer/stocktransfer.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2346 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/transfer/warranttransfer.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/objects/transactions/vesting/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/vesting/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2069 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/vesting/vestingacceleration.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1961 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/vesting/vestingevent.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1968 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/transactions/vesting/vestingstart.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1496 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/valuation.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1275 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/objects/vestingterms.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/files/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/files/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      635 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/files/file.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      783 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/object.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/acceptance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/acceptance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      561 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/acceptance/acceptance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/cancellation/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/cancellation/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      831 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/cancellation/cancellation.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/conversion/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/conversion/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      720 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/conversion/conversion.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/exercise/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/exercise/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      873 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/exercise/exercise.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/issuance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/issuance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1218 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/issuance/issuance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/reissuance/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/reissuance/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1044 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/reissuance/reissuance.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/release/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/release/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1315 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/release/release.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/repurchase/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/repurchase/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1108 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/repurchase/repurchase.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.102310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/retraction/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/retraction/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      615 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/retraction/retraction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1225 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/securitytransaction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      753 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/stockclasstransaction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      744 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/stockplantransaction.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      674 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/transaction.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.106310 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/transfer/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/transfer/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1032 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/objects/transactions/transfer/transfer.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.106310 pyocf-1.0.0/src/pyocf/primitives/types/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.106310 pyocf-1.0.0/src/pyocf/primitives/types/conversion_mechanisms/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       32 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/conversion_mechanisms/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      776 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/conversion_mechanisms/conversionmechanism.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.106310 pyocf-1.0.0/src/pyocf/primitives/types/conversion_rights/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       28 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/conversion_rights/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2357 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/conversion_rights/conversionright.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.106310 pyocf-1.0.0/src/pyocf/primitives/types/conversion_triggers/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       30 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/conversion_triggers/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1909 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/conversion_triggers/conversiontrigger.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.106310 pyocf-1.0.0/src/pyocf/primitives/types/vesting/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/vesting/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      892 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/vesting/vestingconditiontrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1090 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/primitives/types/vesting/vestingperiod.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1513 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/simplebase.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.106310 pyocf-1.0.0/src/pyocf/types/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1164 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/address.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1650 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/capitalizationdefinition.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      840 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/contactinfo.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.106310 pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       32 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1156 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/customconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      943 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/fixedamountconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2171 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/noteconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1464 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/percentcapitalizationconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1392 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/ratioconversionmechanism.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1813 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/safeconversionmechanism.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.106310 pyocf-1.0.0/src/pyocf/types/conversion_rights/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       28 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_rights/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2147 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_rights/convertibleconversionright.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1326 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_rights/stockclassconversionright.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1940 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_rights/warrantconversionright.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.110310 pyocf-1.0.0/src/pyocf/types/conversion_triggers/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       30 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_triggers/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2037 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_triggers/automaticconversiononconditiontrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1925 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_triggers/automaticconversionondatetrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1891 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_triggers/electiveconversionatwilltrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2041 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_triggers/electiveconversionindaterangetrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2045 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_triggers/electiveconversiononconditiontrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1881 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/conversion_triggers/unspecifiedconversiontrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      608 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/countrycode.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      681 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/countrysubdivisioncode.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      592 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/currencycode.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      563 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/date.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      649 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/email.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      583 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/file.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1114 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/interestrate.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      778 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/md5.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      724 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/monetary.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      720 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/name.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      637 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/numeric.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      763 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/percentage.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      796 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/phone.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      961 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/ratio.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1135 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/securityexemption.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1202 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/sharenumberrange.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1096 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/stockparent.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      824 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/taxid.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      914 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/terminationwindow.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.110310 pyocf-1.0.0/src/pyocf/types/vesting/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/vesting/__init__.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2259 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/vesting/vestingcondition.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1558 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/vesting/vestingconditionportion.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      764 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/vesting/vestingeventtrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1005 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/vesting/vestingperiodindays.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1167 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/vesting/vestingperiodinmonths.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      855 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/vesting/vestingscheduleabsolutetrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1596 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/vesting/vestingschedulerelativetrigger.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      776 2023-05-10 11:03:20.000000 pyocf-1.0.0/src/pyocf/types/vesting/vestingstarttrigger.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.094310 pyocf-1.0.0/src/pyocf.egg-info/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1532 2023-05-10 11:03:21.000000 pyocf-1.0.0/src/pyocf.egg-info/PKG-INFO
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9738 2023-05-10 11:03:21.000000 pyocf-1.0.0/src/pyocf.egg-info/SOURCES.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-05-10 11:03:21.000000 pyocf-1.0.0/src/pyocf.egg-info/dependency_links.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      163 2023-05-10 11:03:21.000000 pyocf-1.0.0/src/pyocf.egg-info/requires.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        6 2023-05-10 11:03:21.000000 pyocf-1.0.0/src/pyocf.egg-info/top_level.txt
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-05-10 11:03:21.000000 pyocf-1.0.0/src/pyocf.egg-info/zip-safe
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.110310 pyocf-1.0.0/tests/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:20.000000 pyocf-1.0.0/tests/__init__.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.110310 pyocf-1.0.0/tests/samples/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    12085 2023-05-10 11:03:20.000000 pyocf-1.0.0/tests/samples/Captable.ocf.zip
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2262 2023-05-10 11:03:20.000000 pyocf-1.0.0/tests/test_basic.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    12312 2023-05-10 11:03:20.000000 pyocf-1.0.0/tests/test_load.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2156 2023-05-10 11:03:20.000000 pyocf-1.0.0/tests/test_save.py
-drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-05-10 11:03:21.110310 pyocf-1.0.0/utils/
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      362 2023-05-10 11:03:20.000000 pyocf-1.0.0/utils/enum.mako
--rwxrwxr-x   0 lregebro  (1000) lregebro  (1000)    14379 2023-05-10 11:03:20.000000 pyocf-1.0.0/utils/generate.py
--rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      613 2023-05-10 11:03:20.000000 pyocf-1.0.0/utils/object.mako
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      443 2023-03-15 20:14:42.000000 pyocf-1.0b1/.pre-commit-config.yaml
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       70 2023-03-15 20:14:42.000000 pyocf-1.0b1/CHANGES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1092 2023-03-15 20:14:42.000000 pyocf-1.0b1/LICENSE.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      192 2023-03-15 20:14:42.000000 pyocf-1.0b1/MANIFEST.in
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1340 2023-03-15 20:14:42.000000 pyocf-1.0b1/Makefile
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1188 2023-03-15 20:14:42.347033 pyocf-1.0b1/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      270 2023-03-15 20:14:42.000000 pyocf-1.0b1/README.rst
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1240 2023-03-15 20:14:42.351033 pyocf-1.0b1/setup.cfg
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       38 2023-03-15 20:14:42.000000 pyocf-1.0b1/setup.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.327033 pyocf-1.0b1/src/
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.331033 pyocf-1.0b1/src/pyocf/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     7744 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/captable.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/enums/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      660 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/accrualperiodtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      544 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/addresstype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1376 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/allocationtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      545 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/compensationtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      563 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/compoundingtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      931 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/conversionmechanismtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      714 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/conversionrighttype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      716 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/conversiontimingtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1080 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/conversiontriggertype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      604 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/convertibletype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      599 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/daycounttype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      544 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/emailtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1047 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/filetype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      613 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/interestpayouttype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2852 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/objecttype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      626 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/ocfversiontype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      526 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/optiontype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      683 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/parentsecuritytype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      546 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/periodtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      577 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/phonetype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      550 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/roundingtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1016 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/stakeholderrelationshiptype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      643 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/stakeholdertype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      539 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/stockclasstype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      878 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/terminationwindowtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      496 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/valuationtype.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2241 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/vestingdayofmonth.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      717 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/enums/vestingtriggertype.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/files/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3522 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/ocfmanifestfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      794 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/stakeholdersfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      795 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/stockclassesfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      898 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/stocklegendtemplatesfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      779 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/stockplansfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     5318 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/transactionsfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      774 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/valuationsfile.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      803 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/files/vestingtermsfile.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1922 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/issuer.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1750 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/stakeholder.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3271 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/stockclass.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      928 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/stocklegendtemplate.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1621 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/stockplan.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1835 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/convertibleacceptance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1845 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/plansecurityacceptance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1796 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/stockacceptance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1808 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/warrantacceptance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1721 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockclassauthorizedsharesadjustment.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2240 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockclassconversionratioadjustment.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2010 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockplanpooladjustment.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2160 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/convertiblecancellation.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2180 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/plansecuritycancellation.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2135 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/stockcancellation.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2150 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/warrantcancellation.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/conversion/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/conversion/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2972 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/conversion/convertibleconversion.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2166 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/conversion/stockconversion.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.335033 pyocf-1.0b1/src/pyocf/objects/transactions/exercise/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/exercise/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2177 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/exercise/plansecurityexercise.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2152 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/exercise/warrantexercise.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4651 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/convertibleissuance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4014 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/plansecurityissuance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     3679 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/stockissuance.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4535 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/issuance/warrantissuance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/reissuance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/reissuance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2206 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/reissuance/stockreissuance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/release/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/release/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2482 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/release/plansecurityrelease.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/repurchase/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/repurchase/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2290 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/repurchase/stockrepurchase.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1892 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/convertibleretraction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1884 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/plansecurityretraction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1853 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/stockretraction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1865 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/retraction/warrantretraction.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/split/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/split/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1416 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/split/stockclasssplit.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2375 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/convertibletransfer.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2345 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/plansecuritytransfer.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2353 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/stocktransfer.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2365 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/transfer/warranttransfer.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2027 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingacceleration.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1953 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingevent.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1960 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingstart.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1515 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/valuation.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1294 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/objects/vestingterms.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/files/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/files/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      654 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/files/file.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      802 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/object.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/acceptance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/acceptance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      580 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/acceptance/acceptance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/cancellation/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       23 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/cancellation/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      850 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/cancellation/cancellation.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/conversion/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/conversion/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      739 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/conversion/conversion.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/exercise/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/exercise/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      892 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/exercise/exercise.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.339033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/issuance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/issuance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1237 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/issuance/issuance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/reissuance/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/reissuance/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1063 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/reissuance/reissuance.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/release/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/release/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1334 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/release/release.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/repurchase/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/repurchase/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1127 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/repurchase/repurchase.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/retraction/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       21 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/retraction/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      634 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/retraction/retraction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1214 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/securitytransaction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      749 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/stockclasstransaction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      740 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/stockplantransaction.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      693 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transaction.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transfer/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       19 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transfer/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1051 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transfer/transfer.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/conversion_mechanisms/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       32 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_mechanisms/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      795 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_mechanisms/conversionmechanism.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/conversion_rights/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       28 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_rights/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2350 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_rights/conversionright.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/conversion_triggers/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       30 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_triggers/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1921 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/conversion_triggers/conversiontrigger.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.343033 pyocf-1.0b1/src/pyocf/primitives/types/vesting/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/vesting/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      837 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/vesting/vestingconditiontrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1066 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/primitives/types/vesting/vestingperiod.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1484 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/simplebase.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       16 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1183 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/address.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1588 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/capitalizationdefinition.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      859 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/contactinfo.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       32 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1090 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/customconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      962 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/fixedamountconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2187 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/noteconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1374 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/percentcapitalizationconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1320 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/ratioconversionmechanism.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1796 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/safeconversionmechanism.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/conversion_rights/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       28 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_rights/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2152 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_rights/convertibleconversionright.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1333 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_rights/stockclassconversionright.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1945 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_rights/warrantconversionright.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/conversion_triggers/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       30 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2056 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/automaticconversiononconditiontrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1944 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/automaticconversionondatetrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1886 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversionatwilltrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2040 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversionindaterangetrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2064 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversiononconditiontrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1868 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/conversion_triggers/unspecifiedconversiontrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      627 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/countrycode.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      700 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/countrysubdivisioncode.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      611 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/currencycode.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      582 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/date.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      668 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/email.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      602 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/file.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1133 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/interestrate.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      729 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/md5.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      743 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/monetary.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      739 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/name.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      645 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/numeric.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      742 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/percentage.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      815 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/phone.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      946 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/prereleaseomission.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      953 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/ratio.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1074 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/securityexemption.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1091 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/sharenumberrange.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1018 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/stockparent.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      805 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/taxid.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      933 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/terminationwindow.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/src/pyocf/types/vesting/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)       18 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/__init__.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     2278 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingcondition.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1567 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingconditionportion.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      776 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingeventtrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1018 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingperiodindays.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1171 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingperiodinmonths.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      874 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingscheduleabsolutetrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1575 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingschedulerelativetrigger.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      790 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf/types/vesting/vestingstarttrigger.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.331033 pyocf-1.0b1/src/pyocf.egg-info/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1188 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/PKG-INFO
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     9741 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/SOURCES.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/dependency_links.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      163 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/requires.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        6 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/top_level.txt
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        1 2023-03-15 20:14:42.000000 pyocf-1.0b1/src/pyocf.egg-info/zip-safe
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/tests/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/__init__.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/tests/samples/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    12054 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/samples/Captable.ocf.zip
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     4086 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/test_basic.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)    14197 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/test_load.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)     1529 2023-03-15 20:14:42.000000 pyocf-1.0b1/tests/test_save.py
+drwxrwxr-x   0 lregebro  (1000) lregebro  (1000)        0 2023-03-15 20:14:42.347033 pyocf-1.0b1/utils/
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      399 2023-03-15 20:14:42.000000 pyocf-1.0b1/utils/enum.mako
+-rwxrwxr-x   0 lregebro  (1000) lregebro  (1000)    14740 2023-03-15 20:14:42.000000 pyocf-1.0b1/utils/generate.py
+-rw-rw-r--   0 lregebro  (1000) lregebro  (1000)      723 2023-03-15 20:14:42.000000 pyocf-1.0b1/utils/object.mako
```

### Comparing `pyocf-1.0.0/LICENSE.txt` & `pyocf-1.0b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyocf-1.0.0/Makefile` & `pyocf-1.0b1/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,56 @@
 root_dir := $(shell dirname $(realpath $(lastword $(MAKEFILE_LIST))))
-ifdef NO_VENV
-bin_dir :=
-python_exe := python3
-endif
-ifndef NO_VENV
-bin_dir := $(root_dir)/ve/bin/
-python_exe := $(bin_dir)python3
-endif
+bin_dir := $(root_dir)/ve/bin
 git_source := https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF.git
-git_branch := release-v1.0.0
+git_branch := main
 
 all: devenv fetch build
 
 build: generate check docs
 
 # The fullrelease script is a part of zest.releaser, which is the last
 # package installed, so if it exists, the devenv is installed.
-devenv:	$(bin_dir)fullrelease
+devenv:	ve/bin/fullrelease
 
-$(bin_dir):
+ve/bin/fullrelease:
 	virtualenv ve --python python3.9
-
-$(bin_dir)fullrelease: $(bin_dir)
-	$(python_exe) -m pip install -e .[build]
+	$(bin_dir)/pip install -e .[build]
 
 fetch: Open-Cap-Format-OCF update
 
 Open-Cap-Format-OCF:
 	git clone $(git_source)
 
 update:
 	cd Open-Cap-Format-OCF; \
 	git checkout $(git_branch); \
 	git pull
 
 generate:
-	$(bin_dir)python3 utils/generate.py
-	$(bin_dir)black src/
+	$(bin_dir)/python3 utils/generate.py
+	$(bin_dir)/black src/
 
 check:
-	$(bin_dir)black src utils tests docs
-	$(bin_dir)flake8 src utils tests docs
-	$(bin_dir)pyroma -d .
+	$(bin_dir)/black src utils tests
+	$(bin_dir)/flake8 src utils tests
+	$(bin_dir)/pyroma -d .
 
 coverage:
-	$(bin_dir)coverage run $(bin_dir)pytest
-	$(bin_dir)coverage html
-	$(bin_dir)coverage report
+	$(bin_dir)/coverage run $(bin_dir)/pytest
+	$(bin_dir)/coverage html
+	$(bin_dir)/coverage report
 
 .PHONY: docs
 docs:
 	cd ./docs; make html doctest
 
-Open-Cap-Format-OCF/samples/*.json: devenv fetch generate
-
 tests/samples/Captable.ocf.zip: Open-Cap-Format-OCF/samples/*.json
 	zip -j tests/samples/Captable.ocf.zip Open-Cap-Format-OCF/samples/*.json
 
 test: tests/samples/Captable.ocf.zip
-	$(bin_dir)pytest
+	$(bin_dir)/pytest
 
 release:
-	$(bin_dir)fullrelease
+	$(bin_dir)/fullrelease
 
 clean:
 	rm -rf Open-Cap-Format-OCF ve .coverage htmlcov build .pytest_cache docs/source/generated docs/build
```

### Comparing `pyocf-1.0.0/setup.cfg` & `pyocf-1.0b1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 [metadata]
 name = pyocf
-version = 1.0.0
+version = 1.0b1
 description = Open Captable Format objects and parser
 long_description = file: README.rst, CONTRIBUTORS.txt, CHANGES.txt
 classifiers = 
 	Development Status :: 2 - Pre-Alpha
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: 3 :: Only
 	Topic :: Office/Business :: Financial
 keywords = captable, ocf
 author = Lennart Regebro
-author_email = lennart.regebro@fidelity.com
+author_email = lregebro@shoobx.com
+url = https://open-cap-table-coalition.github.io/Open-Cap-Format-OCF/
 license = MIT
-project_urls = 
-	Documentation = https://pyocf.readthedocs.io/
-	Source Code = https://github.com/Shoobx/pyocf
-	OCF = https://open-cap-table-coalition.github.io/Open-Cap-Format-OCF/
 
 [options]
-python_requires = >=3.9
+python_requires = >3.9
 install_requires = 
 	setuptools
 	pydantic >= 1.10.0
 zip_safe = True
 include_package_data = True
 packages = find:
 package_dir =
```

### Comparing `pyocf-1.0.0/src/pyocf/captable.py` & `pyocf-1.0b1/src/pyocf/captable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,8 @@
 """OCF Captable object"""
-
-# Copyright © 2023 FMR LLC
-
 import datetime
 import hashlib
 import json
 import pathlib
 import zipfile
 
 from packaging import version
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/accrualperiodtype.py` & `pyocf-1.0b1/src/pyocf/enums/periodtype.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,19 @@
-"""Enumeration of interest accrual period types"""
+"""Enumeration of time period types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/AccrualPeriodType.schema.json
+# OCF/tree/main/schema/enums/PeriodType.schema.json
 
 from enum import Enum
 
 
-class AccrualPeriodType(Enum):
-    """Enumeration of interest accrual period types"""
+class PeriodType(Enum):
+    """Enumeration of time period types"""
 
-    ENUM_DAILY = "DAILY"
-    ENUM_MONTHLY = "MONTHLY"
-    ENUM_QUARTERLY = "QUARTERLY"
-    ENUM_SEMI_ANNUAL = "SEMI_ANNUAL"
-    ENUM_ANNUAL = "ANNUAL"
+    ENUM_DAYS = "DAYS"
+    ENUM_MONTHS = "MONTHS"
+    ENUM_YEARS = "YEARS"
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/addresstype.py` & `pyocf-1.0b1/src/pyocf/enums/addresstype.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of address types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/AddressType.schema.json
+# OCF/tree/main/schema/enums/AddressType.schema.json
 
 from enum import Enum
 
 
 class AddressType(Enum):
     """Enumeration of address types"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/allocationtype.py` & `pyocf-1.0b1/src/pyocf/enums/allocationtype.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,16 @@
-"""Enumeration of allocation types for vesting terms. Using an example of 18 shares
-split across 4 tranches, each allocation type results in a different schedule as
-follows:
-  1.  Cumulative Rounding (5 - 4 - 5 - 4)
-  2.  Cumulative Round Down (4 - 5 - 4 - 5)
-  3.  Front Loaded (5 - 5 - 4 - 4)
-  4.  Back Loaded (4 - 4 - 5 - 5)
-  5.  Front Loaded to Single Tranche (6 - 4 - 4 - 4)
-  6.  Back Loaded to Single Tranche (4 - 4 - 4 - 6)
-  7.  Fractional (4.5 - 4.5 - 4.5 - 4.5)"""
+"""Enumeration of allocation types for vesting terms. Using an example of 18 shares"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/AllocationType.schema.json
+# OCF/tree/main/schema/enums/AllocationType.schema.json
 
 from enum import Enum
 
 
 class AllocationType(Enum):
     """Enumeration of allocation types for vesting terms. Using an example of 18 shares
     split across 4 tranches, each allocation type results in a different schedule as
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/compensationtype.py` & `pyocf-1.0b1/src/pyocf/enums/compensationtype.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of stock compensation types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/CompensationType.schema.json
+# OCF/tree/main/schema/enums/CompensationType.schema.json
 
 from enum import Enum
 
 
 class CompensationType(Enum):
     """Enumeration of stock compensation types"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/compoundingtype.py` & `pyocf-1.0b1/src/pyocf/enums/optiontype.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-"""Enumeration of interest compounding types"""
+"""Enumeration of option types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/CompoundingType.schema.json
+# OCF/tree/main/schema/enums/OptionType.schema.json
 
 from enum import Enum
 
 
-class CompoundingType(Enum):
-    """Enumeration of interest compounding types"""
+class OptionType(Enum):
+    """Enumeration of option types"""
 
-    ENUM_COMPOUNDING = "COMPOUNDING"
-    ENUM_SIMPLE = "SIMPLE"
+    ENUM_NSO = "NSO"
+    ENUM_ISO = "ISO"
+    ENUM_INTL = "INTL"
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/conversionmechanismtype.py` & `pyocf-1.0b1/src/pyocf/enums/conversionmechanismtype.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of convertible conversion calculation types."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ConversionMechanismType.schema.json
+# OCF/tree/main/schema/enums/ConversionMechanismType.schema.json
 
 from enum import Enum
 
 
 class ConversionMechanismType(Enum):
     """Enumeration of convertible conversion calculation types."""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/conversiontimingtype.py` & `pyocf-1.0b1/src/pyocf/enums/conversiontimingtype.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Enumeration of convertible conversion timing for calculation purposes (e.g. does
-the instrument convert based on pre or post money)."""
+"""Enumeration of convertible conversion timing for calculation purposes (e.g. does"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ConversionTimingType.schema.json
+# OCF/tree/main/schema/enums/ConversionTimingType.schema.json
 
 from enum import Enum
 
 
 class ConversionTimingType(Enum):
     """Enumeration of convertible conversion timing for calculation purposes (e.g. does
     the instrument convert based on pre or post money).
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/conversiontriggertype.py` & `pyocf-1.0b1/src/pyocf/enums/conversiontriggertype.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-"""Enumeration of types of triggers common to various legal rights - e.g. does the
-satisfaction of a condition trigger an automatic conversion or merely a right to
-convert? If `UNSPECIFIED`, the system of record cannot represent this data in a
-structured form."""
+"""Enumeration of types of triggers common to various legal rights - e.g. does the"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ConversionTriggerType.schema.json
+# OCF/tree/main/schema/enums/ConversionTriggerType.schema.json
 
 from enum import Enum
 
 
 class ConversionTriggerType(Enum):
     """Enumeration of types of triggers common to various legal rights - e.g. does the
     satisfaction of a condition trigger an automatic conversion or merely a right to
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/convertibletype.py` & `pyocf-1.0b1/src/pyocf/enums/phonetype.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-"""Enumeration of convertible instrument types"""
+"""Enumeration of phone number types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ConvertibleType.schema.json
+# OCF/tree/main/schema/enums/PhoneType.schema.json
 
 from enum import Enum
 
 
-class ConvertibleType(Enum):
-    """Enumeration of convertible instrument types"""
+class PhoneType(Enum):
+    """Enumeration of phone number types"""
 
-    ENUM_NOTE = "NOTE"
-    ENUM_SAFE = "SAFE"
-    ENUM_CONVERTIBLE_SECURITY = "CONVERTIBLE_SECURITY"
+    ENUM_HOME = "HOME"
+    ENUM_MOBILE = "MOBILE"
+    ENUM_BUSINESS = "BUSINESS"
+    ENUM_OTHER = "OTHER"
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/daycounttype.py` & `pyocf-1.0b1/src/pyocf/enums/daycounttype.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of how the number of days are determined per period"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/DayCountType.schema.json
+# OCF/tree/main/schema/enums/DayCountType.schema.json
 
 from enum import Enum
 
 
 class DayCountType(Enum):
     """Enumeration of how the number of days are determined per period"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/emailtype.py` & `pyocf-1.0b1/src/pyocf/enums/emailtype.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of email types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/EmailType.schema.json
+# OCF/tree/main/schema/enums/EmailType.schema.json
 
 from enum import Enum
 
 
 class EmailType(Enum):
     """Enumeration of email types"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/filetype.py` & `pyocf-1.0b1/src/pyocf/enums/filetype.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Enumeration of different OCF file types which are used to load proper schemas
-for validation"""
+"""Enumeration of different OCF file types which are used to load proper schemas"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/FileType.schema.json
+# OCF/tree/main/schema/enums/FileType.schema.json
 
 from enum import Enum
 
 
 class FileType(Enum):
     """Enumeration of different OCF file types which are used to load proper schemas
     for validation
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/objecttype.py` & `pyocf-1.0b1/src/pyocf/enums/objecttype.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of object types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ObjectType.schema.json
+# OCF/tree/main/schema/enums/ObjectType.schema.json
 
 from enum import Enum
 
 
 class ObjectType(Enum):
     """Enumeration of object types"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/ocfversiontype.py` & `pyocf-1.0b1/src/pyocf/enums/ocfversiontype.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of recognized OCF versions"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/OCFVersionType.schema.json
+# OCF/tree/main/schema/enums/OCFVersionType.schema.json
 
 from enum import Enum
 
 
 class OCFVersionType(Enum):
     """Enumeration of recognized OCF versions"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/parentsecuritytype.py` & `pyocf-1.0b1/src/pyocf/enums/parentsecuritytype.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of parent sources a stock can be issued or created from"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/ParentSecurityType.schema.json
+# OCF/tree/main/schema/enums/ParentSecurityType.schema.json
 
 from enum import Enum
 
 
 class ParentSecurityType(Enum):
     """Enumeration of parent sources a stock can be issued or created from"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/periodtype.py` & `pyocf-1.0b1/src/pyocf/enums/stakeholdertype.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-"""Enumeration of time period types"""
+"""Enumeration of stakeholder types - individual (human) or institution (entity)"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/PeriodType.schema.json
+# OCF/tree/main/schema/enums/StakeholderType.schema.json
 
 from enum import Enum
 
 
-class PeriodType(Enum):
-    """Enumeration of time period types"""
+class StakeholderType(Enum):
+    """Enumeration of stakeholder types - individual (human) or institution (entity)"""
 
-    ENUM_DAYS = "DAYS"
-    ENUM_MONTHS = "MONTHS"
-    ENUM_YEARS = "YEARS"
+    ENUM_INDIVIDUAL = "INDIVIDUAL"
+    ENUM_INSTITUTION = "INSTITUTION"
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/phonetype.py` & `pyocf-1.0b1/src/pyocf/enums/stockclasstype.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,18 @@
-"""Enumeration of phone number types"""
+"""Enumeration of stock class types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/PhoneType.schema.json
+# OCF/tree/main/schema/enums/StockClassType.schema.json
 
 from enum import Enum
 
 
-class PhoneType(Enum):
-    """Enumeration of phone number types"""
+class StockClassType(Enum):
+    """Enumeration of stock class types"""
 
-    ENUM_HOME = "HOME"
-    ENUM_MOBILE = "MOBILE"
-    ENUM_BUSINESS = "BUSINESS"
-    ENUM_OTHER = "OTHER"
+    ENUM_COMMON = "COMMON"
+    ENUM_PREFERRED = "PREFERRED"
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/roundingtype.py` & `pyocf-1.0b1/src/pyocf/enums/roundingtype.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of rounding types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/RoundingType.schema.json
+# OCF/tree/main/schema/enums/RoundingType.schema.json
 
 from enum import Enum
 
 
 class RoundingType(Enum):
     """Enumeration of rounding types"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/stakeholderrelationshiptype.py` & `pyocf-1.0b1/src/pyocf/enums/stakeholderrelationshiptype.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of types of relationships between stakeholder and issuer"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/StakeholderRelationshipType.schema.json
+# OCF/tree/main/schema/enums/StakeholderRelationshipType.schema.json
 
 from enum import Enum
 
 
 class StakeholderRelationshipType(Enum):
     """Enumeration of types of relationships between stakeholder and issuer"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/stakeholdertype.py` & `pyocf-1.0b1/src/pyocf/enums/interestpayouttype.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""Enumeration of stakeholder types - individual (human) or institution (entity)"""
+"""Enumeration of interest payout types (e.g. deferred or cash payment)"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/StakeholderType.schema.json
+# OCF/tree/main/schema/enums/InterestPayoutType.schema.json
 
 from enum import Enum
 
 
-class StakeholderType(Enum):
-    """Enumeration of stakeholder types - individual (human) or institution (entity)"""
+class InterestPayoutType(Enum):
+    """Enumeration of interest payout types (e.g. deferred or cash payment)"""
 
-    ENUM_INDIVIDUAL = "INDIVIDUAL"
-    ENUM_INSTITUTION = "INSTITUTION"
+    ENUM_DEFERRED = "DEFERRED"
+    ENUM_CASH = "CASH"
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/stockclasstype.py` & `pyocf-1.0b1/src/pyocf/enums/compoundingtype.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""Enumeration of stock class types"""
+"""Enumeration of interest compounding types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/StockClassType.schema.json
+# OCF/tree/main/schema/enums/CompoundingType.schema.json
 
 from enum import Enum
 
 
-class StockClassType(Enum):
-    """Enumeration of stock class types"""
+class CompoundingType(Enum):
+    """Enumeration of interest compounding types"""
 
-    ENUM_COMMON = "COMMON"
-    ENUM_PREFERRED = "PREFERRED"
+    ENUM_COMPOUNDING = "COMPOUNDING"
+    ENUM_SIMPLE = "SIMPLE"
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/terminationwindowtype.py` & `pyocf-1.0b1/src/pyocf/enums/terminationwindowtype.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of termination window types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/TerminationWindowType.schema.json
+# OCF/tree/main/schema/enums/TerminationWindowType.schema.json
 
 from enum import Enum
 
 
 class TerminationWindowType(Enum):
     """Enumeration of termination window types"""
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/vestingdayofmonth.py` & `pyocf-1.0b1/src/pyocf/enums/vestingdayofmonth.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,16 @@
-"""Enumeration representing a vesting "day of month". Since not all months have 29,
-30, or 31 days, this enum requires those values to also specify an overflow
-behavior.
- - `01` - `28` : Day 1, 2... 28 of the month; e.g. `03` means vesting occurs on
-the 3rd of the month.
- - `29_OR_LAST_DAY_OF_MONTH` - `31_OR_LAST_DAY_OF_MONTH` : Day 29, 30, or 31 of
-the month, defaulting to the last day of the month for shorter months; e.g.
-`31_OR_LAST_DAY_OF_MONTH` means monthly vesting occurs on Jan 31, Feb 28/29, Mar
-31, Apr 30, etc.
- - `VESTING_START_DAY_OR_LAST_DAY_OF_MONTH` vests on the same day of month as
-the day of the `VESTING_START` condition; e.g. if vesting commences on Jan 15
-then any vesting will accrue on the 15th of future vesting months. If vesting
-commencement occurs on days 29-31, this has the same behavior as the other
-`*_LAST_DAY_OF_MONTH` values."""
+"""Enumeration representing a vesting "day of month". Since not all months have 29,"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/VestingDayOfMonth.schema.json
+# OCF/tree/main/schema/enums/VestingDayOfMonth.schema.json
 
 from enum import Enum
 
 
 class VestingDayOfMonth(Enum):
     """Enumeration representing a vesting "day of month". Since not all months have 29,
     30, or 31 days, this enum requires those values to also specify an overflow
```

### Comparing `pyocf-1.0.0/src/pyocf/enums/vestingtriggertype.py` & `pyocf-1.0b1/src/pyocf/enums/vestingtriggertype.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Enumeration of vesting trigger types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/enums/VestingTriggerType.schema.json
+# OCF/tree/main/schema/enums/VestingTriggerType.schema.json
 
 from enum import Enum
 
 
 class VestingTriggerType(Enum):
     """Enumeration of vesting trigger types"""
```

### Comparing `pyocf-1.0.0/src/pyocf/files/ocfmanifestfile.py` & `pyocf-1.0b1/src/pyocf/files/ocfmanifestfile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Top-level schema describing the OCF Manifest, which holds issuer information and
-references ocf files containing transactions, stakeholders, stock classes, etc."""
+"""Top-level schema describing the OCF Manifest, which holds issuer information and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/OCFManifestFile.schema.json
+# OCF/tree/main/schema/files/OCFManifestFile.schema.json
 
 from pyocf.enums.ocfversiontype import OCFVersionType
 from pyocf.objects.issuer import Issuer
 from pyocf.primitives.files.file import FileObject
 from pyocf.types.date import Date
 from pyocf.types.file import File
 from typing import Literal
```

### Comparing `pyocf-1.0.0/src/pyocf/files/stocklegendtemplatesfile.py` & `pyocf-1.0b1/src/pyocf/files/stocklegendtemplatesfile.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """JSON containing file type identifier and list of stock legend templates"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/StockLegendTemplatesFile.schema.json
+# OCF/tree/main/schema/files/StockLegendTemplatesFile.schema.json
 
 from pyocf.objects.stocklegendtemplate import StockLegendTemplate
 from pyocf.primitives.files.file import FileObject
 from typing import Literal
 
 
 class StockLegendTemplatesFile(FileObject):
```

### Comparing `pyocf-1.0.0/src/pyocf/files/stockplansfile.py` & `pyocf-1.0b1/src/pyocf/files/stockplansfile.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """JSON containing file type identifier and list of stock plans"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/StockPlansFile.schema.json
+# OCF/tree/main/schema/files/StockPlansFile.schema.json
 
 from pyocf.objects.stockplan import StockPlan
 from pyocf.primitives.files.file import FileObject
 from typing import Literal
 
 
 class StockPlansFile(FileObject):
```

### Comparing `pyocf-1.0.0/src/pyocf/files/transactionsfile.py` & `pyocf-1.0b1/src/pyocf/files/transactionsfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """JSON containing file type identifier and list transactions"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/TransactionsFile.schema.json
+# OCF/tree/main/schema/files/TransactionsFile.schema.json
 
 from pydantic import Field
 from pyocf.objects.transactions.acceptance.convertibleacceptance import (
     ConvertibleAcceptance,
 )
 from pyocf.objects.transactions.acceptance.plansecurityacceptance import (
     PlanSecurityAcceptance,
```

### Comparing `pyocf-1.0.0/src/pyocf/files/valuationsfile.py` & `pyocf-1.0b1/src/pyocf/files/valuationsfile.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """JSON containing file type identifier and list of valuations"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/ValuationsFile.schema.json
+# OCF/tree/main/schema/files/ValuationsFile.schema.json
 
 from pyocf.objects.valuation import Valuation
 from pyocf.primitives.files.file import FileObject
 from typing import Literal
 
 
 class ValuationsFile(FileObject):
```

### Comparing `pyocf-1.0.0/src/pyocf/files/vestingtermsfile.py` & `pyocf-1.0b1/src/pyocf/files/vestingtermsfile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """JSON containing file type identifier and list of vesting terms"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/files/VestingTermsFile.schema.json
+# OCF/tree/main/schema/files/VestingTermsFile.schema.json
 
 from pyocf.objects.vestingterms import VestingTerms
 from pyocf.primitives.files.file import FileObject
 from typing import Literal
 
 
 class VestingTermsFile(FileObject):
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/issuer.py` & `pyocf-1.0b1/src/pyocf/objects/issuer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Object describing the issuer of the cap table (the company whose cap table this
-is)"""
+"""Object describing the issuer of the cap table (the company whose cap table this"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/Issuer.schema.json
+# OCF/tree/main/schema/objects/Issuer.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.types.address import Address
 from pyocf.types.countrycode import CountryCode
 from pyocf.types.countrysubdivisioncode import CountrySubdivisionCode
 from pyocf.types.date import Date
 from pyocf.types.email import Email
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/stakeholder.py` & `pyocf-1.0b1/src/pyocf/objects/stakeholder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a stakeholder"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/Stakeholder.schema.json
+# OCF/tree/main/schema/objects/Stakeholder.schema.json
 
 from pyocf.enums.stakeholderrelationshiptype import StakeholderRelationshipType
 from pyocf.enums.stakeholdertype import StakeholderType
 from pyocf.primitives.objects.object import Object
 from pyocf.types.address import Address
 from pyocf.types.contactinfo import ContactInfo
 from pyocf.types.name import Name
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/stockclass.py` & `pyocf-1.0b1/src/pyocf/objects/stockclass.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a class of stock issued by the issuer"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/StockClass.schema.json
+# OCF/tree/main/schema/objects/StockClass.schema.json
 
 from pyocf.enums.stockclasstype import StockClassType
 from pyocf.primitives.objects.object import Object
 from pyocf.types.conversion_rights.stockclassconversionright import (
     StockClassConversionRight,
 )
 from pyocf.types.date import Date
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/stocklegendtemplate.py` & `pyocf-1.0b1/src/pyocf/objects/stocklegendtemplate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a stock legend template"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/StockLegendTemplate.schema.json
+# OCF/tree/main/schema/objects/StockLegendTemplate.schema.json
 
 from pyocf.primitives.objects.object import Object
 from typing import Literal
 from typing import Optional
 
 
 class StockLegendTemplate(Object):
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/stockplan.py` & `pyocf-1.0b1/src/pyocf/objects/stockplan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a plan which stock options are issued from"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/StockPlan.schema.json
+# OCF/tree/main/schema/objects/StockPlan.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/convertibleacceptance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/convertibleacceptance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Object describing a convertible acceptance transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/acceptance/ConvertibleAcceptance.schema.j
-# son
+# ree/main/schema/objects/transactions/acceptance/ConvertibleAcceptance.schema.jso
+# n
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.acceptance.acceptance import Acceptance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/plansecurityacceptance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/plansecurityacceptance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Object describing a plan security acceptance transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/acceptance/PlanSecurityAcceptance.schema.
-# json
+# ree/main/schema/objects/transactions/acceptance/PlanSecurityAcceptance.schema.js
+# on
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.acceptance.acceptance import Acceptance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/stockacceptance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/stockacceptance.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a stock acceptance transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/acceptance/StockAcceptance.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/acceptance/StockAcceptance.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.acceptance.acceptance import Acceptance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/acceptance/warrantacceptance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/acceptance/warrantacceptance.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a warrant acceptance transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/acceptance/WarrantAcceptance.schema.json
+# ree/main/schema/objects/transactions/acceptance/WarrantAcceptance.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.acceptance.acceptance import Acceptance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/adjustment/stockclassauthorizedsharesadjustment.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockclassauthorizedsharesadjustment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""Object describing an event to change the number of authoried shares of a stock
-class."""
+"""Object describing an event to change the number of authoried shares of a stock"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/adjustment/StockClassAuthorizedSharesAdju
-# stment.schema.json
+# ree/main/schema/objects/transactions/adjustment/StockClassAuthorizedSharesAdjust
+# ment.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.stockclasstransaction import (
     StockClassTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/adjustment/stockclassconversionratioadjustment.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockclassconversionratioadjustment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,17 @@
-"""Object describing the conversion ratio adjustment of a stock class that has a
-RatioConversionMechanism conversion mechanism where there was an actual
-repricing due to a down-round. The actual determination of the new conversion
-ratio / conversion price is calculated outside of OCF, so the specific mechanism
-- e.g. broad-based weighted-average anti-dilution protection vs. full ratchet
-anti-dilution protection."""
+"""Object describing the conversion ratio adjustment of a stock class that has a"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/adjustment/StockClassConversionRatioAdjus
-# tment.schema.json
+# ree/main/schema/objects/transactions/adjustment/StockClassConversionRatioAdjustm
+# ent.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.stockclasstransaction import (
     StockClassTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.conversion_mechanisms.ratioconversionmechanism import (
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/adjustment/stockplanpooladjustment.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/adjustment/stockplanpooladjustment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Object describing the change in the size of a Stock Plan pool."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/adjustment/StockPlanPoolAdjustment.schema
-# .json
+# ree/main/schema/objects/transactions/adjustment/StockPlanPoolAdjustment.schema.j
+# son
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.stockplantransaction import (
     StockPlanTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/convertiblecancellation.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/plansecuritycancellation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
-"""Object describing a cancellation of a convertible security"""
+"""Object describing a cancellation of a plan security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/cancellation/ConvertibleCancellation.sche
-# ma.json
+# ree/main/schema/objects/transactions/cancellation/PlanSecurityCancellation.schem
+# a.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.cancellation.cancellation import Cancellation
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from pyocf.types.monetary import Monetary
+from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
 
 
-class ConvertibleCancellation(Object, Transaction, SecurityTransaction, Cancellation):
-    """Object describing a cancellation of a convertible security"""
+class PlanSecurityCancellation(Object, Transaction, SecurityTransaction, Cancellation):
+    """Object describing a cancellation of a plan security"""
 
-    object_type: Literal["TX_CONVERTIBLE_CANCELLATION"] = "TX_CONVERTIBLE_CANCELLATION"
-    # Amount of monetary value cancelled
-    amount: Monetary
+    object_type: Literal[
+        "TX_PLAN_SECURITY_CANCELLATION"
+    ] = "TX_PLAN_SECURITY_CANCELLATION"
+    # Quantity of non-monetary security units cancelled
+    quantity: Numeric
     # Identifier for the object
     id: str
     # Unstructured text comments related to and stored for the object
     comments: Optional[list[str]]
     # Identifier for the security (stock, plan security, warrant, or convertible) by
     # which it can be referenced by other transaction objects. Note that while this
     # identifier is created with an issuance object, it should be different than the
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/plansecuritycancellation.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/warrantcancellation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-"""Object describing a cancellation of a plan security"""
+"""Object describing a cancellation of a warrant security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/cancellation/PlanSecurityCancellation.sch
-# ema.json
+# ree/main/schema/objects/transactions/cancellation/WarrantCancellation.schema.jso
+# n
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.cancellation.cancellation import Cancellation
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
 
 
-class PlanSecurityCancellation(Object, Transaction, SecurityTransaction, Cancellation):
-    """Object describing a cancellation of a plan security"""
+class WarrantCancellation(Object, Transaction, SecurityTransaction, Cancellation):
+    """Object describing a cancellation of a warrant security"""
 
-    object_type: Literal[
-        "TX_PLAN_SECURITY_CANCELLATION"
-    ] = "TX_PLAN_SECURITY_CANCELLATION"
+    object_type: Literal["TX_WARRANT_CANCELLATION"] = "TX_WARRANT_CANCELLATION"
     # Quantity of non-monetary security units cancelled
     quantity: Numeric
     # Identifier for the object
     id: str
     # Unstructured text comments related to and stored for the object
     comments: Optional[list[str]]
     # Identifier for the security (stock, plan security, warrant, or convertible) by
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/stockcancellation.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/stockcancellation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Object describing a cancellation of a stock security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/cancellation/StockCancellation.schema.jso
-# n
+# ree/main/schema/objects/transactions/cancellation/StockCancellation.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.cancellation.cancellation import Cancellation
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/cancellation/warrantcancellation.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/cancellation/convertiblecancellation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""Object describing a cancellation of a warrant security"""
+"""Object describing a cancellation of a convertible security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/cancellation/WarrantCancellation.schema.j
-# son
+# ree/main/schema/objects/transactions/cancellation/ConvertibleCancellation.schema
+# .json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.cancellation.cancellation import Cancellation
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
-from pyocf.types.numeric import Numeric
+from pyocf.types.monetary import Monetary
 from typing import Literal
 from typing import Optional
 
 
-class WarrantCancellation(Object, Transaction, SecurityTransaction, Cancellation):
-    """Object describing a cancellation of a warrant security"""
+class ConvertibleCancellation(Object, Transaction, SecurityTransaction, Cancellation):
+    """Object describing a cancellation of a convertible security"""
 
-    object_type: Literal["TX_WARRANT_CANCELLATION"] = "TX_WARRANT_CANCELLATION"
-    # Quantity of non-monetary security units cancelled
-    quantity: Numeric
+    object_type: Literal["TX_CONVERTIBLE_CANCELLATION"] = "TX_CONVERTIBLE_CANCELLATION"
+    # Amount of monetary value cancelled
+    amount: Monetary
     # Identifier for the object
     id: str
     # Unstructured text comments related to and stored for the object
     comments: Optional[list[str]]
     # Identifier for the security (stock, plan security, warrant, or convertible) by
     # which it can be referenced by other transaction objects. Note that while this
     # identifier is created with an issuance object, it should be different than the
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/conversion/convertibleconversion.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/conversion/convertibleconversion.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Object describing a conversion of a convertible security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/conversion/ConvertibleConversion.schema.j
-# son
+# ree/main/schema/objects/transactions/conversion/ConvertibleConversion.schema.jso
+# n
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.conversion.conversion import Conversion
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/conversion/stockconversion.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/conversion/stockconversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a conversion of stock"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/conversion/StockConversion.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/conversion/StockConversion.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.conversion.conversion import Conversion
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/exercise/plansecurityexercise.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/exercise/plansecurityexercise.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a plan security exercise transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/exercise/PlanSecurityExercise.schema.json
+# ree/main/schema/objects/transactions/exercise/PlanSecurityExercise.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.exercise.exercise import Exercise
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/exercise/warrantexercise.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/exercise/warrantexercise.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a warrant exercise transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/exercise/WarrantExercise.schema.json
+# OCF/tree/main/schema/objects/transactions/exercise/WarrantExercise.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.exercise.exercise import Exercise
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/issuance/convertibleissuance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/issuance/convertibleissuance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Object describing convertible instrument issuance transaction by the issuer and
-held by a stakeholder"""
+"""Object describing convertible instrument issuance transaction by the issuer and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/issuance/ConvertibleIssuance.schema.json
+# ree/main/schema/objects/transactions/issuance/ConvertibleIssuance.schema.json
 
 from pydantic import Field
 from pyocf.enums.convertibletype import ConvertibleType
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.issuance.issuance import Issuance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/issuance/plansecurityissuance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/issuance/plansecurityissuance.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""Object describing securities issuance transaction from a plan by the issuer and
-held by a stakeholder"""
+"""Object describing securities issuance transaction from a plan by the issuer and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/issuance/PlanSecurityIssuance.schema.json
+# ree/main/schema/objects/transactions/issuance/PlanSecurityIssuance.schema.json
 
+from pydantic import root_validator
 from pyocf.enums.compensationtype import CompensationType
 from pyocf.enums.optiontype import OptionType
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.issuance.issuance import Issuance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
@@ -72,7 +72,19 @@
     # Date of board approval for the security
     board_approval_date: Optional[Date]
     # Unstructured text description of consideration provided in exchange for security
     # issuance
     consideration_text: Optional[str]
     # List of security law exemptions (and applicable jurisdictions) for this security
     security_law_exemptions: list[SecurityExemption]
+
+    @root_validator(pre=True)
+    def validator_compensation_type(cls, values):
+        if (
+            values.get("compensation_type") == "OPTION"
+            and values.get("option_grant_type") is None
+        ):
+            raise ValueError(
+                "When compensation_type is 'OPTION' then option_grant_type is required"
+            )
+
+        return values
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/issuance/stockissuance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/issuance/stockissuance.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Object describing a stock issuance transaction by the issuer and held by a
-stakeholder"""
+"""Object describing a stock issuance transaction by the issuer and held by a"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/issuance/StockIssuance.schema.json
+# OCF/tree/main/schema/objects/transactions/issuance/StockIssuance.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.issuance.issuance import Issuance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/issuance/warrantissuance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/issuance/warrantissuance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Object describing warrant issuance transaction by the issuer and held by a
-stakeholder"""
+"""Object describing warrant issuance transaction by the issuer and held by a"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/issuance/WarrantIssuance.schema.json
+# OCF/tree/main/schema/objects/transactions/issuance/WarrantIssuance.schema.json
 
 from pydantic import Field
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.issuance.issuance import Issuance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/reissuance/stockreissuance.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/reissuance/stockreissuance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a re-issuance of stock"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/reissuance/StockReissuance.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/reissuance/StockReissuance.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.reissuance.reissuance import Reissuance
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/release/plansecurityrelease.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/release/plansecurityrelease.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a plan security release transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/release/PlanSecurityRelease.schema.json
+# ree/main/schema/objects/transactions/release/PlanSecurityRelease.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.release.release import Release
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/repurchase/stockrepurchase.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/repurchase/stockrepurchase.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a stock repurchase transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/repurchase/StockRepurchase.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/repurchase/StockRepurchase.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.repurchase.repurchase import Repurchase
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/retraction/convertibleretraction.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/retraction/plansecurityretraction.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""Object describing a retraction of a convertible security"""
+"""Object describing a retraction of a plan security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/retraction/ConvertibleRetraction.schema.j
-# son
+# ree/main/schema/objects/transactions/retraction/PlanSecurityRetraction.schema.js
+# on
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.retraction.retraction import Retraction
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
 from typing import Literal
 from typing import Optional
 
 
-class ConvertibleRetraction(Object, Transaction, SecurityTransaction, Retraction):
-    """Object describing a retraction of a convertible security"""
+class PlanSecurityRetraction(Object, Transaction, SecurityTransaction, Retraction):
+    """Object describing a retraction of a plan security"""
 
-    object_type: Literal["TX_CONVERTIBLE_RETRACTION"] = "TX_CONVERTIBLE_RETRACTION"
+    object_type: Literal["TX_PLAN_SECURITY_RETRACTION"] = "TX_PLAN_SECURITY_RETRACTION"
     # Identifier for the object
     id: str
     # Unstructured text comments related to and stored for the object
     comments: Optional[list[str]]
     # Identifier for the security (stock, plan security, warrant, or convertible) by
     # which it can be referenced by other transaction objects. Note that while this
     # identifier is created with an issuance object, it should be different than the
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/retraction/plansecurityretraction.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/retraction/warrantretraction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,32 @@
-"""Object describing a retraction of a plan security"""
+"""Object describing a retraction of a warrant security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/retraction/PlanSecurityRetraction.schema.
-# json
+# ree/main/schema/objects/transactions/retraction/WarrantRetraction.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.retraction.retraction import Retraction
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
 from typing import Literal
 from typing import Optional
 
 
-class PlanSecurityRetraction(Object, Transaction, SecurityTransaction, Retraction):
-    """Object describing a retraction of a plan security"""
+class WarrantRetraction(Object, Transaction, SecurityTransaction, Retraction):
+    """Object describing a retraction of a warrant security"""
 
-    object_type: Literal["TX_PLAN_SECURITY_RETRACTION"] = "TX_PLAN_SECURITY_RETRACTION"
+    object_type: Literal["TX_WARRANT_RETRACTION"] = "TX_WARRANT_RETRACTION"
     # Identifier for the object
     id: str
     # Unstructured text comments related to and stored for the object
     comments: Optional[list[str]]
     # Identifier for the security (stock, plan security, warrant, or convertible) by
     # which it can be referenced by other transaction objects. Note that while this
     # identifier is created with an issuance object, it should be different than the
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/retraction/stockretraction.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/retraction/stockretraction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a retraction of a stock security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/retraction/StockRetraction.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/objects/transactions/retraction/StockRetraction.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.retraction.retraction import Retraction
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/retraction/warrantretraction.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/retraction/convertibleretraction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-"""Object describing a retraction of a warrant security"""
+"""Object describing a retraction of a convertible security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/retraction/WarrantRetraction.schema.json
+# ree/main/schema/objects/transactions/retraction/ConvertibleRetraction.schema.jso
+# n
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.retraction.retraction import Retraction
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
 from typing import Literal
 from typing import Optional
 
 
-class WarrantRetraction(Object, Transaction, SecurityTransaction, Retraction):
-    """Object describing a retraction of a warrant security"""
+class ConvertibleRetraction(Object, Transaction, SecurityTransaction, Retraction):
+    """Object describing a retraction of a convertible security"""
 
-    object_type: Literal["TX_WARRANT_RETRACTION"] = "TX_WARRANT_RETRACTION"
+    object_type: Literal["TX_CONVERTIBLE_RETRACTION"] = "TX_CONVERTIBLE_RETRACTION"
     # Identifier for the object
     id: str
     # Unstructured text comments related to and stored for the object
     comments: Optional[list[str]]
     # Identifier for the security (stock, plan security, warrant, or convertible) by
     # which it can be referenced by other transaction objects. Note that while this
     # identifier is created with an issuance object, it should be different than the
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/split/stockclasssplit.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/split/stockclasssplit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a split of a stock class"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/split/StockClassSplit.schema.json
+# OCF/tree/main/schema/objects/transactions/split/StockClassSplit.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.stockclasstransaction import (
     StockClassTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/transfer/convertibletransfer.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/transfer/convertibletransfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a transfer or secondary sale of a convertible security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/transfer/ConvertibleTransfer.schema.json
+# ree/main/schema/objects/transactions/transfer/ConvertibleTransfer.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/transfer/plansecuritytransfer.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/transfer/plansecuritytransfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a transfer of a plan security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/transfer/PlanSecurityTransfer.schema.json
+# ree/main/schema/objects/transactions/transfer/PlanSecurityTransfer.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/transfer/stocktransfer.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/transfer/warranttransfer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""Object describing a transfer or secondary sale of a stock security"""
+"""Object describing a transfer or secondary sale of a warrant security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/transfer/StockTransfer.schema.json
+# OCF/tree/main/schema/objects/transactions/transfer/WarrantTransfer.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
 
 
-class StockTransfer(Object, Transaction, SecurityTransaction, Transfer):
-    """Object describing a transfer or secondary sale of a stock security"""
+class WarrantTransfer(Object, Transaction, SecurityTransaction, Transfer):
+    """Object describing a transfer or secondary sale of a warrant security"""
 
-    object_type: Literal["TX_STOCK_TRANSFER"] = "TX_STOCK_TRANSFER"
+    object_type: Literal["TX_WARRANT_TRANSFER"] = "TX_WARRANT_TRANSFER"
     # Quantity of non-monetary security units transferred
     quantity: Numeric
     # Identifier for the object
     id: str
     # Unstructured text comments related to and stored for the object
     comments: Optional[list[str]]
     # Identifier for the security (stock, plan security, warrant, or convertible) by
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/transfer/warranttransfer.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/transfer/stocktransfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-"""Object describing a transfer or secondary sale of a warrant security"""
+"""Object describing a transfer or secondary sale of a stock security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/transfer/WarrantTransfer.schema.json
+# OCF/tree/main/schema/objects/transactions/transfer/StockTransfer.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.primitives.objects.transactions.transfer.transfer import Transfer
 from pyocf.types.date import Date
 from pyocf.types.numeric import Numeric
 from typing import Literal
 from typing import Optional
 
 
-class WarrantTransfer(Object, Transaction, SecurityTransaction, Transfer):
-    """Object describing a transfer or secondary sale of a warrant security"""
+class StockTransfer(Object, Transaction, SecurityTransaction, Transfer):
+    """Object describing a transfer or secondary sale of a stock security"""
 
-    object_type: Literal["TX_WARRANT_TRANSFER"] = "TX_WARRANT_TRANSFER"
+    object_type: Literal["TX_STOCK_TRANSFER"] = "TX_STOCK_TRANSFER"
     # Quantity of non-monetary security units transferred
     quantity: Numeric
     # Identifier for the object
     id: str
     # Unstructured text comments related to and stored for the object
     comments: Optional[list[str]]
     # Identifier for the security (stock, plan security, warrant, or convertible) by
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/vesting/vestingacceleration.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingacceleration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Object describing an acceleration of vesting, in which additional shares vest
-ahead of the schedule specified in security's vesting terms."""
+"""Object describing an acceleration of vesting, in which additional shares vest"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/objects/transactions/vesting/VestingAcceleration.schema.json
+# ree/main/schema/objects/transactions/vesting/VestingAcceleration.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/vesting/vestingevent.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingevent.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Object describing the transaction of an non-schedule-driven vesting event
-associated with a security"""
+"""Object describing the transaction of an non-schedule-driven vesting event"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/vesting/VestingEvent.schema.json
+# OCF/tree/main/schema/objects/transactions/vesting/VestingEvent.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/transactions/vesting/vestingstart.py` & `pyocf-1.0b1/src/pyocf/objects/transactions/vesting/vestingstart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Object describing the transaction of vesting schedule start / commencement
-associated with a security"""
+"""Object describing the transaction of vesting schedule start / commencement"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/transactions/vesting/VestingStart.schema.json
+# OCF/tree/main/schema/objects/transactions/vesting/VestingStart.schema.json
 
 from pyocf.primitives.objects.object import Object
 from pyocf.primitives.objects.transactions.securitytransaction import (
     SecurityTransaction,
 )
 from pyocf.primitives.objects.transactions.transaction import Transaction
 from pyocf.types.date import Date
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/valuation.py` & `pyocf-1.0b1/src/pyocf/objects/valuation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing a valuation used in the cap table"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/Valuation.schema.json
+# OCF/tree/main/schema/objects/Valuation.schema.json
 
 from pyocf.enums.valuationtype import ValuationType
 from pyocf.primitives.objects.object import Object
 from pyocf.types.date import Date
 from pyocf.types.monetary import Monetary
 from typing import Literal
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/objects/vestingterms.py` & `pyocf-1.0b1/src/pyocf/objects/vestingterms.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Object describing the terms under which a security vests"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/objects/VestingTerms.schema.json
+# OCF/tree/main/schema/objects/VestingTerms.schema.json
 
 from pyocf.enums.allocationtype import AllocationType
 from pyocf.primitives.objects.object import Object
 from pyocf.types.vesting.vestingcondition import VestingCondition
 from typing import Literal
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/files/file.py` & `pyocf-1.0b1/src/pyocf/primitives/files/file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Abstract file to be extended by all other files"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/primitives/files/File.schema.json
+# OCF/tree/main/schema/primitives/files/File.schema.json
 
 from pydantic import BaseModel
 from pyocf.enums.filetype import FileType
 
 
 class FileObject(BaseModel):
     """Abstract file to be extended by all other files"""
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/object.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/object.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Abstract object to be extended by all other objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/primitives/objects/Object.schema.json
+# OCF/tree/main/schema/primitives/objects/Object.schema.json
 
 from pydantic import BaseModel
 from pyocf.enums.objecttype import ObjectType
 from typing import Optional
 
 
 class Object(BaseModel):
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/acceptance/acceptance.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/acceptance/acceptance.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Abstract object describing a security acceptance transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/acceptance/Acceptance.schema.j
-# son
+# ree/main/schema/primitives/objects/transactions/acceptance/Acceptance.schema.jso
+# n
 
 from pydantic import BaseModel
 
 
 class Acceptance(BaseModel):
     """Abstract object describing a security acceptance transaction"""
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/cancellation/cancellation.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/cancellation/cancellation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Abstract object describing fields common to all cancellation transaction objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/cancellation/Cancellation.sche
-# ma.json
+# ree/main/schema/primitives/objects/transactions/cancellation/Cancellation.schema
+# .json
 
 from pydantic import BaseModel
 from typing import Optional
 
 
 class Cancellation(BaseModel):
     """Abstract object describing fields common to all cancellation transaction objects"""
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/conversion/conversion.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/conversion/conversion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Abstract object describing fields common to all conversion transaction objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/conversion/Conversion.schema.j
-# son
+# ree/main/schema/primitives/objects/transactions/conversion/Conversion.schema.jso
+# n
 
 from pydantic import BaseModel
 
 
 class Conversion(BaseModel):
     """Abstract object describing fields common to all conversion transaction objects"""
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/exercise/exercise.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/exercise/exercise.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Abstract object describing fields common to all exercise transaction objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/exercise/Exercise.schema.json
+# ree/main/schema/primitives/objects/transactions/exercise/Exercise.schema.json
 
 from pydantic import BaseModel
 from typing import Optional
 
 
 class Exercise(BaseModel):
     """Abstract object describing fields common to all exercise transaction objects"""
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/issuance/issuance.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/issuance/issuance.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Abstract object describing fields common to all issuance objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/issuance/Issuance.schema.json
+# ree/main/schema/primitives/objects/transactions/issuance/Issuance.schema.json
 
 from pydantic import BaseModel
 from pyocf.types.date import Date
 from pyocf.types.securityexemption import SecurityExemption
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/reissuance/reissuance.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/reissuance/reissuance.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Abstract object describing common properties to a reissuance of a security"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/reissuance/Reissuance.schema.j
-# son
+# ree/main/schema/primitives/objects/transactions/reissuance/Reissuance.schema.jso
+# n
 
 from pydantic import BaseModel
 from typing import Optional
 
 
 class Reissuance(BaseModel):
     """Abstract object describing common properties to a reissuance of a security"""
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/release/release.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/release/release.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Abstract object describing fields common to all release transaction objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/release/Release.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/primitives/objects/transactions/release/Release.schema.json
 
 from pydantic import BaseModel
 from pyocf.types.date import Date
 from pyocf.types.monetary import Monetary
 from pyocf.types.numeric import Numeric
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/repurchase/repurchase.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/repurchase/repurchase.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Abstract object describing common properties to a repurchase transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/repurchase/Repurchase.schema.j
-# son
+# ree/main/schema/primitives/objects/transactions/repurchase/Repurchase.schema.jso
+# n
 
 from pydantic import BaseModel
 from pyocf.types.monetary import Monetary
 from pyocf.types.numeric import Numeric
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/securitytransaction.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/securitytransaction.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""Abstract transaction object to be extended by all transaction objects that deal
-with individual securities"""
+"""Abstract transaction object to be extended by all transaction objects that deal"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/SecurityTransaction.schema.jso
-# n
+# ree/main/schema/primitives/objects/transactions/SecurityTransaction.schema.json
 
 from pydantic import BaseModel
 
 
 class SecurityTransaction(BaseModel):
     """Abstract transaction object to be extended by all transaction objects that deal
     with individual securities
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/stockclasstransaction.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/stockclasstransaction.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""Abstract transaction object to be extended by all transaction objects that
-affect the stock class"""
+"""Abstract transaction object to be extended by all transaction objects that"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/StockClassTransaction.schema.j
-# son
+# ree/main/schema/primitives/objects/transactions/StockClassTransaction.schema.jso
+# n
 
 from pydantic import BaseModel
 
 
 class StockClassTransaction(BaseModel):
     """Abstract transaction object to be extended by all transaction objects that
     affect the stock class
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/stockplantransaction.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/stockplantransaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""Abstract transaction object to be extended by all transaction objects that
-affect a stock plan"""
+"""Abstract transaction object to be extended by all transaction objects that"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/StockPlanTransaction.schema.js
-# on
+# ree/main/schema/primitives/objects/transactions/StockPlanTransaction.schema.json
 
 from pydantic import BaseModel
 
 
 class StockPlanTransaction(BaseModel):
     """Abstract transaction object to be extended by all transaction objects that
     affect a stock plan
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/transaction.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transaction.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Abstract transaction object to be extended by all other transaction objects"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/primitives/objects/transactions/Transaction.schema.json
+# OCF/tree/main/schema/primitives/objects/transactions/Transaction.schema.json
 
 from pydantic import BaseModel
 from pyocf.types.date import Date
 
 
 class Transaction(BaseModel):
     """Abstract transaction object to be extended by all other transaction objects"""
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/objects/transactions/transfer/transfer.py` & `pyocf-1.0b1/src/pyocf/primitives/objects/transactions/transfer/transfer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Abstract object describing a security transfer or secondary sale transaction"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/objects/transactions/transfer/Transfer.schema.json
+# ree/main/schema/primitives/objects/transactions/transfer/Transfer.schema.json
 
 from pydantic import BaseModel
 from typing import Optional
 
 
 class Transfer(BaseModel):
     """Abstract object describing a security transfer or secondary sale transaction"""
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/types/conversion_mechanisms/conversionmechanism.py` & `pyocf-1.0b1/src/pyocf/primitives/types/conversion_mechanisms/conversionmechanism.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Abstract type setting forth required field(s) for ALL conversion mechanism types"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/types/conversion_mechanisms/ConversionMechanism.sch
-# ema.json
+# ree/main/schema/primitives/types/conversion_mechanisms/ConversionMechanism.schem
+# a.json
 
 from pydantic import BaseModel
 from pyocf.enums.conversionmechanismtype import ConversionMechanismType
 
 
 class ConversionMechanism(BaseModel):
     """Abstract type setting forth required field(s) for ALL conversion mechanism types"""
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/types/conversion_rights/conversionright.py` & `pyocf-1.0b1/src/pyocf/primitives/types/conversion_rights/conversionright.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Abstract type representation of a conversion right from a non-plan security into
-another non-plan security"""
+"""Abstract type representation of a conversion right from a non-plan security into"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/types/conversion_rights/ConversionRight.schema.json
+# ree/main/schema/primitives/types/conversion_rights/ConversionRight.schema.json
 
 from pydantic import BaseModel
 from pydantic import Field
 from pyocf.enums.conversionrighttype import ConversionRightType
 from pyocf.types.conversion_mechanisms.customconversionmechanism import (
     CustomConversionMechanism,
 )
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/types/conversion_triggers/conversiontrigger.py` & `pyocf-1.0b1/src/pyocf/primitives/types/conversion_triggers/conversiontrigger.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""Abstract type representation of required fields require for conversion rights
-types."""
+"""Abstract type representation of required fields require for conversion rights"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/types/conversion_triggers/ConversionTrigger.schema.
-# json
+# ree/main/schema/primitives/types/conversion_triggers/ConversionTrigger.schema.js
+# on
 
 from pydantic import BaseModel
 from pydantic import Field
 from pyocf.enums.conversiontriggertype import ConversionTriggerType
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
 )
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/types/vesting/vestingconditiontrigger.py` & `pyocf-1.0b1/src/pyocf/primitives/types/vesting/vestingconditiontrigger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Abstract type describing fields needed in all triggers types, with a 'trigger'
-being a condition that must be satisfied for a VestingCondition to be met"""
+"""Abstract type describing fields needed in all triggers types, with a 'trigger'"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/primitives/types/vesting/VestingConditionTrigger.schema.json
+# ree/main/schema/primitives/types/vesting/VestingConditionTrigger.schema.json
 
 from pydantic import BaseModel
 from pyocf.enums.vestingtriggertype import VestingTriggerType
 
 
 class VestingConditionTrigger(BaseModel):
     """Abstract type describing fields needed in all triggers types, with a 'trigger'
```

### Comparing `pyocf-1.0.0/src/pyocf/primitives/types/vesting/vestingperiod.py` & `pyocf-1.0b1/src/pyocf/primitives/types/vesting/vestingperiod.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Abstract type describing the fields common to all periods of time (e.g. 3
-months, 365 days) for use in Vesting Terms"""
+"""Abstract type describing the fields common to all periods of time (e.g. 3"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/primitives/types/vesting/VestingPeriod.schema.json
+# OCF/tree/main/schema/primitives/types/vesting/VestingPeriod.schema.json
 
 from pydantic import BaseModel
 from pyocf.enums.periodtype import PeriodType
 
 
 class VestingPeriod(BaseModel):
     """Abstract type describing the fields common to all periods of time (e.g. 3
```

### Comparing `pyocf-1.0.0/src/pyocf/simplebase.py` & `pyocf-1.0b1/src/pyocf/simplebase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """A pydantic model for simple types with no attributes"""
 
-# Copyright © 2023 FMR LLC
-
 from pydantic import BaseModel
 
 
 class SimpleBaseModel(BaseModel):
     """A pydantic model for simple types with no attributes
 
     This model allows you to pass the value into object initialization
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.0/src/pyocf/types/address.py` & `pyocf-1.0b1/src/pyocf/types/address.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of an address"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Address.schema.json
+# OCF/tree/main/schema/types/Address.schema.json
 
 from pydantic import BaseModel
 from pyocf.enums.addresstype import AddressType
 from pyocf.types.countrycode import CountryCode
 from pyocf.types.countrysubdivisioncode import CountrySubdivisionCode
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/types/capitalizationdefinition.py` & `pyocf-1.0b1/src/pyocf/types/capitalizationdefinition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Type represents a group of securities that constitutes some formally defined
-part of the company (e.g. post-money capitalization vs pre-money for a security)"""
+"""Type represents a group of securities that constitutes some formally defined"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/CapitalizationDefinition.schema.json
+# OCF/tree/main/schema/types/CapitalizationDefinition.schema.json
 
 from pydantic import BaseModel
 
 
 class CapitalizationDefinition(BaseModel):
     """Type represents a group of securities that constitutes some formally defined
     part of the company (e.g. post-money capitalization vs pre-money for a security)
```

### Comparing `pyocf-1.0.0/src/pyocf/types/contactinfo.py` & `pyocf-1.0b1/src/pyocf/types/contactinfo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of a primary contact person for a stakeholder (e.g. a fund)"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/ContactInfo.schema.json
+# OCF/tree/main/schema/types/ContactInfo.schema.json
 
 from pydantic import BaseModel
 from pyocf.types.email import Email
 from pyocf.types.name import Name
 from pyocf.types.phone import Phone
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/customconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/customconversionmechanism.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-"""Sets forth inputs and conversion mechanism of a custom conversion, a conversion
-type that cannot be accurately modelled with any other OCF conversion mechanism
-type"""
+"""Sets forth inputs and conversion mechanism of a custom conversion, a conversion"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/CustomConversionMechanism.schema.j
-# son
+# ree/main/schema/types/conversion_mechanisms/CustomConversionMechanism.schema.jso
+# n
 
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
 from typing import Literal
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/fixedamountconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/fixedamountconversionmechanism.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Describes how a security converts into a fixed amount of a stock class"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/FixedAmountConversionMechanism.sch
-# ema.json
+# ree/main/schema/types/conversion_mechanisms/FixedAmountConversionMechanism.schem
+# a.json
 
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
 from pyocf.types.numeric import Numeric
 from typing import Literal
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/noteconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/noteconversionmechanism.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Sets forth inputs and conversion mechanism of a convertible note"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/NoteConversionMechanism.schema.jso
-# n
+# ree/main/schema/types/conversion_mechanisms/NoteConversionMechanism.schema.json
 
 from pyocf.enums.accrualperiodtype import AccrualPeriodType
 from pyocf.enums.compoundingtype import CompoundingType
 from pyocf.enums.daycounttype import DayCountType
 from pyocf.enums.interestpayouttype import InterestPayoutType
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/percentcapitalizationconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/percentcapitalizationconversionmechanism.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-"""Sets forth inputs and conversion mechanism of percent of capitalization
-conversion (where an instrument purports to grant a percent of company
-capitalization at some point in time)"""
+"""Sets forth inputs and conversion mechanism of percent of capitalization"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/PercentCapitalizationConversionMec
-# hanism.schema.json
+# ree/main/schema/types/conversion_mechanisms/PercentCapitalizationConversionMecha
+# nism.schema.json
 
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
 from pyocf.types.percentage import Percentage
 from typing import Literal
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/ratioconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/ratioconversionmechanism.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-"""Sets forth inputs and conversion mechanism of a ratio conversion (primarily used
-to describe conversion from one stock class (e.g. Preferred) into another (e.g.
-Common)"""
+"""Sets forth inputs and conversion mechanism of a ratio conversion (primarily used"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/RatioConversionMechanism.schema.js
-# on
+# ree/main/schema/types/conversion_mechanisms/RatioConversionMechanism.schema.json
 
 from pyocf.enums.roundingtype import RoundingType
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
 from pyocf.types.monetary import Monetary
 from pyocf.types.ratio import Ratio
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_mechanisms/safeconversionmechanism.py` & `pyocf-1.0b1/src/pyocf/types/conversion_mechanisms/safeconversionmechanism.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""Sets forth inputs and conversion mechanism of a SAFE (mirrors the flavors and
-inputs of the Y Combinator SAFE)"""
+"""Sets forth inputs and conversion mechanism of a SAFE (mirrors the flavors and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_mechanisms/SAFEConversionMechanism.schema.jso
-# n
+# ree/main/schema/types/conversion_mechanisms/SAFEConversionMechanism.schema.json
 
 from pyocf.enums.conversiontimingtype import ConversionTimingType
 from pyocf.primitives.types.conversion_mechanisms.conversionmechanism import (
     ConversionMechanism,
 )
 from pyocf.types.monetary import Monetary
 from pyocf.types.percentage import Percentage
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_rights/convertibleconversionright.py` & `pyocf-1.0b1/src/pyocf/types/conversion_rights/convertibleconversionright.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Type representation of a conversion right from a convertible into another non-
-plan security"""
+"""Type representation of a conversion right from a convertible into another non-"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_rights/ConvertibleConversionRight.schema.json
+# ree/main/schema/types/conversion_rights/ConvertibleConversionRight.schema.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_rights.conversionright import ConversionRight
 from pyocf.types.conversion_mechanisms.customconversionmechanism import (
     CustomConversionMechanism,
 )
 from pyocf.types.conversion_mechanisms.fixedamountconversionmechanism import (
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_rights/stockclassconversionright.py` & `pyocf-1.0b1/src/pyocf/types/conversion_rights/stockclassconversionright.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Type representation of a conversion right from one Stock Class into another
-Stock Class"""
+"""Type representation of a conversion right from one Stock Class into another"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_rights/StockClassConversionRight.schema.json
+# ree/main/schema/types/conversion_rights/StockClassConversionRight.schema.json
 
 from pyocf.primitives.types.conversion_rights.conversionright import ConversionRight
 from pyocf.types.conversion_mechanisms.ratioconversionmechanism import (
     RatioConversionMechanism,
 )
 from typing import Literal
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_rights/warrantconversionright.py` & `pyocf-1.0b1/src/pyocf/types/conversion_rights/warrantconversionright.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Type representation of a conversion right from a convertible into another non-
-plan security"""
+"""Type representation of a conversion right from a convertible into another non-"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
-# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_rights/WarrantConversionRight.schema.json
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
+# OCF/tree/main/schema/types/conversion_rights/WarrantConversionRight.schema.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_rights.conversionright import ConversionRight
 from pyocf.types.conversion_mechanisms.customconversionmechanism import (
     CustomConversionMechanism,
 )
 from pyocf.types.conversion_mechanisms.fixedamountconversionmechanism import (
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_triggers/automaticconversiononconditiontrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversiononconditiontrigger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Type representation of automatic trigger on a tive or condition."""
+"""Type representation of elective trigger on fulfillment of a condition."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/AutomaticConversionOnConditionTrigge
-# r.schema.json
+# ree/main/schema/types/conversion_triggers/ElectiveConversionOnConditionTrigger.s
+# chema.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
@@ -22,29 +22,29 @@
 from pyocf.types.conversion_rights.warrantconversionright import WarrantConversionRight
 from typing import Annotated
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 
-class AutomaticConversionOnConditionTrigger(ConversionTrigger):
-    """Type representation of automatic trigger on a tive or condition."""
+class ElectiveConversionOnConditionTrigger(ConversionTrigger):
+    """Type representation of elective trigger on fulfillment of a condition."""
 
     # Legal language describing what conditions must be satisfied for the conversion
     # to take place (ideally, this should be excerpted from the instrument where
     # possible)
     trigger_condition: str
     # Id for this conversion trigger, unique within list of ConversionTriggers in
     # parent convertible issuance's `conversion_triggers` field.
     trigger_id: str
     # Human-friendly nickname to describe the conversion right
     nickname: Optional[str]
     # Long-form description of the trigger
     trigger_description: Optional[str]
-    type: Literal["AUTOMATIC_ON_CONDITION"] = "AUTOMATIC_ON_CONDITION"
+    type: Literal["ELECTIVE_ON_CONDITION"] = "ELECTIVE_ON_CONDITION"
     # When the conditions of the trigger are met, how does the convertible convert?
     conversion_right: Annotated[
         Union[
             ConvertibleConversionRight,
             WarrantConversionRight,
             StockClassConversionRight,
         ],
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_triggers/automaticconversionondatetrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/automaticconversionondatetrigger.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Type representation of an automatic trigger on a date."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/AutomaticConversionOnDateTrigger.sch
-# ema.json
+# ree/main/schema/types/conversion_triggers/AutomaticConversionOnDateTrigger.schem
+# a.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_triggers/electiveconversionatwilltrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversionindaterangetrigger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,53 @@
-"""Type representation of elective trigger valid at will (so long as instrument is
-valid and outstanding)."""
+"""Type representation of elective trigger valid on or after start_date and until"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/ElectiveConversionAtWillTrigger.sche
-# ma.json
+# ree/main/schema/types/conversion_triggers/ElectiveConversionInDateRangeTrigger.s
+# chema.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
 )
 from pyocf.types.conversion_rights.stockclassconversionright import (
     StockClassConversionRight,
 )
 from pyocf.types.conversion_rights.warrantconversionright import WarrantConversionRight
+from pyocf.types.date import Date
 from typing import Annotated
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 
-class ElectiveConversionAtWillTrigger(ConversionTrigger):
-    """Type representation of elective trigger valid at will (so long as instrument is
-    valid and outstanding).
+class ElectiveConversionInDateRangeTrigger(ConversionTrigger):
+    """Type representation of elective trigger valid on or after start_date and until
+    or before end_date.
     """
 
     # Id for this conversion trigger, unique within list of ConversionTriggers in
     # parent convertible issuance's `conversion_triggers` field.
     trigger_id: str
+    type: Literal["ELECTIVE_IN_RANGE"] = "ELECTIVE_IN_RANGE"
+    # Start date of range (inclusive)
+    start_date: Date
+    # End date of range (inclusive)
+    end_date: Date
     # Human-friendly nickname to describe the conversion right
     nickname: Optional[str]
     # Long-form description of the trigger
     trigger_description: Optional[str]
-    type: Literal["ELECTIVE_AT_WILL"] = "ELECTIVE_AT_WILL"
     # When the conditions of the trigger are met, how does the convertible convert?
     conversion_right: Annotated[
         Union[
             ConvertibleConversionRight,
             WarrantConversionRight,
             StockClassConversionRight,
         ],
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_triggers/electiveconversionindaterangetrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/electiveconversionatwilltrigger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,48 @@
-"""Type representation of elective trigger valid on or after start_date and until
-or before end_date."""
+"""Type representation of elective trigger valid at will (so long as instrument is"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/ElectiveConversionInDateRangeTrigger
-# .schema.json
+# ree/main/schema/types/conversion_triggers/ElectiveConversionAtWillTrigger.schema
+# .json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
 )
 from pyocf.types.conversion_rights.stockclassconversionright import (
     StockClassConversionRight,
 )
 from pyocf.types.conversion_rights.warrantconversionright import WarrantConversionRight
-from pyocf.types.date import Date
 from typing import Annotated
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 
-class ElectiveConversionInDateRangeTrigger(ConversionTrigger):
-    """Type representation of elective trigger valid on or after start_date and until
-    or before end_date.
+class ElectiveConversionAtWillTrigger(ConversionTrigger):
+    """Type representation of elective trigger valid at will (so long as instrument is
+    valid and outstanding).
     """
 
     # Id for this conversion trigger, unique within list of ConversionTriggers in
     # parent convertible issuance's `conversion_triggers` field.
     trigger_id: str
-    type: Literal["ELECTIVE_IN_RANGE"] = "ELECTIVE_IN_RANGE"
-    # Start date of range (inclusive)
-    start_date: Date
-    # End date of range (inclusive)
-    end_date: Date
     # Human-friendly nickname to describe the conversion right
     nickname: Optional[str]
     # Long-form description of the trigger
     trigger_description: Optional[str]
+    type: Literal["ELECTIVE_AT_WILL"] = "ELECTIVE_AT_WILL"
     # When the conditions of the trigger are met, how does the convertible convert?
     conversion_right: Annotated[
         Union[
             ConvertibleConversionRight,
             WarrantConversionRight,
             StockClassConversionRight,
         ],
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_triggers/electiveconversiononconditiontrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/automaticconversiononconditiontrigger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-"""Type representation of elective trigger on fulfillment of a condition."""
+"""Type representation of automatic trigger on a tive or condition."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/ElectiveConversionOnConditionTrigger
-# .schema.json
+# ree/main/schema/types/conversion_triggers/AutomaticConversionOnConditionTrigger.
+# schema.json
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
@@ -22,29 +22,29 @@
 from pyocf.types.conversion_rights.warrantconversionright import WarrantConversionRight
 from typing import Annotated
 from typing import Literal
 from typing import Optional
 from typing import Union
 
 
-class ElectiveConversionOnConditionTrigger(ConversionTrigger):
-    """Type representation of elective trigger on fulfillment of a condition."""
+class AutomaticConversionOnConditionTrigger(ConversionTrigger):
+    """Type representation of automatic trigger on a tive or condition."""
 
     # Legal language describing what conditions must be satisfied for the conversion
     # to take place (ideally, this should be excerpted from the instrument where
     # possible)
     trigger_condition: str
     # Id for this conversion trigger, unique within list of ConversionTriggers in
     # parent convertible issuance's `conversion_triggers` field.
     trigger_id: str
     # Human-friendly nickname to describe the conversion right
     nickname: Optional[str]
     # Long-form description of the trigger
     trigger_description: Optional[str]
-    type: Literal["ELECTIVE_ON_CONDITION"] = "ELECTIVE_ON_CONDITION"
+    type: Literal["AUTOMATIC_ON_CONDITION"] = "AUTOMATIC_ON_CONDITION"
     # When the conditions of the trigger are met, how does the convertible convert?
     conversion_right: Annotated[
         Union[
             ConvertibleConversionRight,
             WarrantConversionRight,
             StockClassConversionRight,
         ],
```

### Comparing `pyocf-1.0.0/src/pyocf/types/conversion_triggers/unspecifiedconversiontrigger.py` & `pyocf-1.0b1/src/pyocf/types/conversion_triggers/unspecifiedconversiontrigger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-"""Use this where no structured data is available regarding what triggers the
-conversion of a given security."""
+"""Use this where no structured data is available regarding what triggers the"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-OCF/t
-# ree/v1.0.0/schema/types/conversion_triggers/UnspecifiedConversionTrigger.schema.
-# json
+# ree/main/schema/types/conversion_triggers/UnspecifiedConversionTrigger.schema.js
+# on
 
 from pydantic import Field
 from pyocf.primitives.types.conversion_triggers.conversiontrigger import (
     ConversionTrigger,
 )
 from pyocf.types.conversion_rights.convertibleconversionright import (
     ConvertibleConversionRight,
```

### Comparing `pyocf-1.0.0/src/pyocf/types/countrycode.py` & `pyocf-1.0b1/src/pyocf/types/countrycode.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of an ISO 3166-1 alpha 2 country code"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/CountryCode.schema.json
+# OCF/tree/main/schema/types/CountryCode.schema.json
 
 from pydantic import constr
 from pyocf.simplebase import SimpleBaseModel
 
 
 class CountryCode(SimpleBaseModel):
     """Type representation of an ISO 3166-1 alpha 2 country code"""
```

### Comparing `pyocf-1.0.0/src/pyocf/types/countrysubdivisioncode.py` & `pyocf-1.0b1/src/pyocf/types/countrysubdivisioncode.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of the second part of an ISO 3166-2 country subdivision code"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/CountrySubdivisionCode.schema.json
+# OCF/tree/main/schema/types/CountrySubdivisionCode.schema.json
 
 from pydantic import constr
 from pyocf.simplebase import SimpleBaseModel
 
 
 class CountrySubdivisionCode(SimpleBaseModel):
     """Type representation of the second part of an ISO 3166-2 country subdivision code"""
```

### Comparing `pyocf-1.0.0/src/pyocf/types/currencycode.py` & `pyocf-1.0b1/src/pyocf/types/currencycode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of an ISO 4217 currency code"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/CurrencyCode.schema.json
+# OCF/tree/main/schema/types/CurrencyCode.schema.json
 
 from pydantic import constr
 from pyocf.simplebase import SimpleBaseModel
 
 
 class CurrencyCode(SimpleBaseModel):
     """Type representation of an ISO 4217 currency code"""
```

### Comparing `pyocf-1.0.0/src/pyocf/types/file.py` & `pyocf-1.0b1/src/pyocf/types/file.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of a file"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/File.schema.json
+# OCF/tree/main/schema/types/File.schema.json
 
 from pydantic import BaseModel
 from pyocf.types.md5 import Md5
 
 
 class File(BaseModel):
     """Type representation of a file"""
```

### Comparing `pyocf-1.0.0/src/pyocf/types/interestrate.py` & `pyocf-1.0b1/src/pyocf/types/interestrate.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of an interest rate, including accrual start and end dates"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/InterestRate.schema.json
+# OCF/tree/main/schema/types/InterestRate.schema.json
 
 from pydantic import BaseModel
 from pyocf.types.date import Date
 from pyocf.types.percentage import Percentage
 from typing import Optional
```

### Comparing `pyocf-1.0.0/src/pyocf/types/md5.py` & `pyocf-1.0b1/src/pyocf/types/md5.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""String representation of MD5 hash with basic validation for a string of 32
-characters composed of letters (uppercase or lowercase) and numbers"""
+"""String representation of MD5 hash with basic validation for a string of 32"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Md5.schema.json
+# OCF/tree/main/schema/types/Md5.schema.json
 
 from pydantic import constr
 from pyocf.simplebase import SimpleBaseModel
 
 
 class Md5(SimpleBaseModel):
     """String representation of MD5 hash with basic validation for a string of 32
```

### Comparing `pyocf-1.0.0/src/pyocf/types/numeric.py` & `pyocf-1.0b1/src/pyocf/types/numeric.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Fixed-point string representation of a number (up to 10 decimal places
-supported)"""
+"""Fixed-point string representation of a number (up to 10 decimal places"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Numeric.schema.json
+# OCF/tree/main/schema/types/Numeric.schema.json
 
 from decimal import Decimal
 from pyocf.simplebase import SimpleBaseModel
 
 
 class Numeric(SimpleBaseModel):
     """Fixed-point string representation of a number (up to 10 decimal places
```

### Comparing `pyocf-1.0.0/src/pyocf/types/phone.py` & `pyocf-1.0b1/src/pyocf/types/phone.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of a phone number"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/Phone.schema.json
+# OCF/tree/main/schema/types/Phone.schema.json
 
 from pydantic import BaseModel
 from pydantic import constr
 from pyocf.enums.phonetype import PhoneType
 
 
 class Phone(BaseModel):
```

### Comparing `pyocf-1.0.0/src/pyocf/types/securityexemption.py` & `pyocf-1.0b1/src/pyocf/types/securityexemption.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Type representation of a securities issuance exemption that includes an
-unstructured description and a country code for ease of processing and analysis"""
+"""Type representation of a securities issuance exemption that includes an"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/SecurityExemption.schema.json
+# OCF/tree/main/schema/types/SecurityExemption.schema.json
 
 from pydantic import BaseModel
 
 
 class SecurityExemption(BaseModel):
     """Type representation of a securities issuance exemption that includes an
     unstructured description and a country code for ease of processing and analysis
```

### Comparing `pyocf-1.0.0/src/pyocf/types/sharenumberrange.py` & `pyocf-1.0b1/src/pyocf/types/sharenumberrange.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""Type representation of a range of share numbers associated with an event (such
-as the share numbers associated with an issuance) - for use where shares are not
-fungible and need unique identifiers *per share*"""
+"""Type representation of a range of share numbers associated with an event (such"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/ShareNumberRange.schema.json
+# OCF/tree/main/schema/types/ShareNumberRange.schema.json
 
 from pydantic import BaseModel
 from pyocf.types.numeric import Numeric
 
 
 class ShareNumberRange(BaseModel):
     """Type representation of a range of share numbers associated with an event (such
```

### Comparing `pyocf-1.0.0/src/pyocf/types/stockparent.py` & `pyocf-1.0b1/src/pyocf/types/stockparent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-"""Type representation of the parent security of a given stock issuance (e.g. if a
-stock issuance came from a plan, such as an RSA, or if a stock came from a
-previous stock entry)"""
+"""Type representation of the parent security of a given stock issuance (e.g. if a"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/StockParent.schema.json
+# OCF/tree/main/schema/types/StockParent.schema.json
 
 from pydantic import BaseModel
 from pyocf.enums.parentsecuritytype import ParentSecurityType
 
 
 class StockParent(BaseModel):
     """Type representation of the parent security of a given stock issuance (e.g. if a
```

### Comparing `pyocf-1.0.0/src/pyocf/types/taxid.py` & `pyocf-1.0b1/src/pyocf/types/taxid.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Type representation of a government identifier for tax purposes (e.g. EIN) and
-corresponding country code (ISO-3166)"""
+"""Type representation of a government identifier for tax purposes (e.g. EIN) and"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/TaxID.schema.json
+# OCF/tree/main/schema/types/TaxID.schema.json
 
 from pydantic import BaseModel
 from pyocf.types.countrycode import CountryCode
 
 
 class TaxID(BaseModel):
     """Type representation of a government identifier for tax purposes (e.g. EIN) and
```

### Comparing `pyocf-1.0.0/src/pyocf/types/terminationwindow.py` & `pyocf-1.0b1/src/pyocf/types/terminationwindow.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Type representation of a termination window"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/TerminationWindow.schema.json
+# OCF/tree/main/schema/types/TerminationWindow.schema.json
 
 from pydantic import BaseModel
 from pyocf.enums.periodtype import PeriodType
 from pyocf.enums.terminationwindowtype import TerminationWindowType
 
 
 class TerminationWindow(BaseModel):
```

### Comparing `pyocf-1.0.0/src/pyocf/types/vesting/vestingcondition.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingcondition.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Describes condition / triggers to be satisfied for vesting to occur"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingCondition.schema.json
+# OCF/tree/main/schema/types/vesting/VestingCondition.schema.json
 
 from pydantic import BaseModel
 from pydantic import Field
 from pyocf.types.numeric import Numeric
 from pyocf.types.vesting.vestingconditionportion import VestingConditionPortion
 from pyocf.types.vesting.vestingeventtrigger import VestingEventTrigger
 from pyocf.types.vesting.vestingscheduleabsolutetrigger import (
```

### Comparing `pyocf-1.0.0/src/pyocf/types/vesting/vestingconditionportion.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingconditionportion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Describes a fractional portion (ratio) of shares associated with a Vesting
-Condition"""
+"""Describes a fractional portion (ratio) of shares associated with a Vesting"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingConditionPortion.schema.json
+# OCF/tree/main/schema/types/vesting/VestingConditionPortion.schema.json
 
 from pydantic import BaseModel
 from pyocf.types.numeric import Numeric
 from typing import Optional
 
 
 class VestingConditionPortion(BaseModel):
```

### Comparing `pyocf-1.0.0/src/pyocf/types/vesting/vestingeventtrigger.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingeventtrigger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Describes a vesting condition satisfied when a particular unscheduled event
-occurs"""
+"""Describes a vesting condition satisfied when a particular unscheduled event"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingEventTrigger.schema.json
+# OCF/tree/main/schema/types/vesting/VestingEventTrigger.schema.json
 
 from pyocf.primitives.types.vesting.vestingconditiontrigger import (
     VestingConditionTrigger,
 )
 from typing import Literal
```

### Comparing `pyocf-1.0.0/src/pyocf/types/vesting/vestingperiodindays.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingperiodindays.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Describes a period of time expressed in days (e.g. 365 days) for use in Vesting
-Terms"""
+"""Describes a period of time expressed in days (e.g. 365 days) for use in Vesting"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingPeriodInDays.schema.json
+# OCF/tree/main/schema/types/vesting/VestingPeriodInDays.schema.json
 
 from pyocf.primitives.types.vesting.vestingperiod import VestingPeriod
 from typing import Literal
 
 
 class VestingPeriodInDays(VestingPeriod):
     """Describes a period of time expressed in days (e.g. 365 days) for use in Vesting
```

### Comparing `pyocf-1.0.0/src/pyocf/types/vesting/vestingperiodinmonths.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingperiodinmonths.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Describes a period of time expressed in months (e.g. 3 months) for use in
-Vesting Terms."""
+"""Describes a period of time expressed in months (e.g. 3 months) for use in"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingPeriodInMonths.schema.json
+# OCF/tree/main/schema/types/vesting/VestingPeriodInMonths.schema.json
 
 from pyocf.enums.vestingdayofmonth import VestingDayOfMonth
 from pyocf.primitives.types.vesting.vestingperiod import VestingPeriod
 from typing import Literal
 
 
 class VestingPeriodInMonths(VestingPeriod):
```

### Comparing `pyocf-1.0.0/src/pyocf/types/vesting/vestingscheduleabsolutetrigger.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingscheduleabsolutetrigger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Describes a vesting condition satisfied on an absolute date."""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingScheduleAbsoluteTrigger.schema.json
+# OCF/tree/main/schema/types/vesting/VestingScheduleAbsoluteTrigger.schema.json
 
 from pyocf.primitives.types.vesting.vestingconditiontrigger import (
     VestingConditionTrigger,
 )
 from pyocf.types.date import Date
 from typing import Literal
```

### Comparing `pyocf-1.0.0/src/pyocf/types/vesting/vestingschedulerelativetrigger.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingschedulerelativetrigger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Describes a vesting condition satisfied when a period of time, relative to
-another vesting condition, has elapsed."""
+"""Describes a vesting condition satisfied when a period of time, relative to"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingScheduleRelativeTrigger.schema.json
+# OCF/tree/main/schema/types/vesting/VestingScheduleRelativeTrigger.schema.json
 
 from pydantic import Field
 from pyocf.primitives.types.vesting.vestingconditiontrigger import (
     VestingConditionTrigger,
 )
 from pyocf.types.vesting.vestingperiodindays import VestingPeriodInDays
 from pyocf.types.vesting.vestingperiodinmonths import VestingPeriodInMonths
```

### Comparing `pyocf-1.0.0/src/pyocf/types/vesting/vestingstarttrigger.py` & `pyocf-1.0b1/src/pyocf/types/vesting/vestingstarttrigger.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-"""Describes a vesting condition satisfied at the security's vesting commencement
-date"""
+"""Describes a vesting condition satisfied at the security's vesting commencement"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
-# Copyright © 2022 Open Cap Table Coalition (https://opencaptablecoalition.com) /
+# Copyright © 2023 Open Cap Table Coalition (https://opencaptablecoalition.com) /
 # Original File: https://github.com/Open-Cap-Table-Coalition/Open-Cap-Format-
-# OCF/tree/v1.0.0/schema/types/vesting/VestingStartTrigger.schema.json
+# OCF/tree/main/schema/types/vesting/VestingStartTrigger.schema.json
 
 from pyocf.primitives.types.vesting.vestingconditiontrigger import (
     VestingConditionTrigger,
 )
 from typing import Literal
```

### Comparing `pyocf-1.0.0/src/pyocf.egg-info/SOURCES.txt` & `pyocf-1.0b1/src/pyocf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 .pre-commit-config.yaml
-.readthedocs.yaml
 CHANGES.txt
 LICENSE.txt
 MANIFEST.in
 Makefile
 README.rst
 setup.cfg
 setup.py
 src/pyocf/__init__.py
-src/pyocf/api.py
 src/pyocf/captable.py
 src/pyocf/simplebase.py
 src/pyocf.egg-info/PKG-INFO
 src/pyocf.egg-info/SOURCES.txt
 src/pyocf.egg-info/dependency_links.txt
 src/pyocf.egg-info/requires.txt
 src/pyocf.egg-info/top_level.txt
@@ -164,14 +162,15 @@
 src/pyocf/types/interestrate.py
 src/pyocf/types/md5.py
 src/pyocf/types/monetary.py
 src/pyocf/types/name.py
 src/pyocf/types/numeric.py
 src/pyocf/types/percentage.py
 src/pyocf/types/phone.py
+src/pyocf/types/prereleaseomission.py
 src/pyocf/types/ratio.py
 src/pyocf/types/securityexemption.py
 src/pyocf/types/sharenumberrange.py
 src/pyocf/types/stockparent.py
 src/pyocf/types/taxid.py
 src/pyocf/types/terminationwindow.py
 src/pyocf/types/conversion_mechanisms/__init__.py
```

### Comparing `pyocf-1.0.0/tests/samples/Captable.ocf.zip` & `pyocf-1.0b1/tests/samples/Captable.ocf.zip`

 * *Files 27% similar despite different names*

#### zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 12085 bytes, number of entries: 11
--rw-rw-r--  3.0 unx     2126 tx defN 23-Apr-27 12:35 Manifest.ocf.json
--rw-rw-r--  3.0 unx      544 tx defN 23-Apr-27 12:35 Stakeholders.ocf.json
--rw-rw-r--  3.0 unx     1672 tx defN 23-Apr-27 12:35 StockClasses.ocf.json
--rw-rw-r--  3.0 unx      667 tx defN 23-Apr-27 12:35 StockLegends.ocf.json
--rw-rw-r--  3.0 unx      480 tx defN 23-Apr-27 12:35 StockPlans.ocf.json
--rw-rw-r--  3.0 unx    35552 tx defN 23-Apr-27 12:35 Transactions.ocf.json
--rw-rw-r--  3.0 unx      505 tx defN 23-Apr-27 12:35 Valuations.ocf.json
--rw-rw-r--  3.0 unx    13193 tx defN 23-Apr-27 12:35 VestingTerms.ocf.json
--rw-rw-r--  3.0 unx      669 tx defN 23-Apr-27 12:35 VestingTerms.example1.ocf.json
--rw-rw-r--  3.0 unx     1988 tx defN 23-Apr-27 12:35 VestingTerms.example2.ocf.json
--rw-rw-r--  3.0 unx      440 tx defN 23-Apr-27 12:35 VestingTransactions.examples.ocf.json
-11 files, 57836 bytes uncompressed, 10141 bytes compressed:  82.5%
+Zip file size: 12054 bytes, number of entries: 11
+-rw-rw-r--  3.0 unx     2126 tx defN 23-Mar-15 19:30 Manifest.ocf.json
+-rw-rw-r--  3.0 unx      544 tx defN 23-Mar-15 19:30 Stakeholders.ocf.json
+-rw-rw-r--  3.0 unx     1672 tx defN 23-Mar-15 19:30 StockClasses.ocf.json
+-rw-rw-r--  3.0 unx      667 tx defN 23-Mar-15 19:30 StockLegends.ocf.json
+-rw-rw-r--  3.0 unx      480 tx defN 23-Mar-15 19:30 StockPlans.ocf.json
+-rw-rw-r--  3.0 unx    34857 tx defN 23-Mar-15 19:30 Transactions.ocf.json
+-rw-rw-r--  3.0 unx      505 tx defN 23-Mar-15 19:30 Valuations.ocf.json
+-rw-rw-r--  3.0 unx    13193 tx defN 23-Mar-15 19:30 VestingTerms.ocf.json
+-rw-rw-r--  3.0 unx      669 tx defN 23-Mar-15 19:30 VestingTerms.example1.ocf.json
+-rw-rw-r--  3.0 unx     1988 tx defN 23-Mar-15 19:30 VestingTerms.example2.ocf.json
+-rw-rw-r--  3.0 unx      440 tx defN 23-Mar-15 19:30 VestingTransactions.examples.ocf.json
+11 files, 57141 bytes uncompressed, 10110 bytes compressed:  82.3%
```

#### Transactions.ocf.json

##### Pretty-printed

 * *Similarity: 0.9965277777777778%*

 * *Differences: {"'items'": '{delete: [41]}'}*

```diff
@@ -750,40 +750,14 @@
         {
             "cost_basis": {
                 "amount": "0",
                 "currency": "USD"
             },
             "custom_id": "S-1",
             "date": "2022-02-01",
-            "id": "test-stock-issuance-minimal-RSA",
-            "issuance_type": "RSA",
-            "object_type": "TX_STOCK_ISSUANCE",
-            "quantity": "1000",
-            "security_id": "test-security-id",
-            "security_law_exemptions": [],
-            "share_price": {
-                "amount": "1.00",
-                "currency": "USD"
-            },
-            "stakeholder_id": "stakeholder-id",
-            "stock_class_id": "stock-class-id",
-            "stock_legend_ids": [
-                "stock-legend-id-1",
-                "stock-legend-id-2"
-            ],
-            "stock_plan_id": "2022-Plan",
-            "vesting_terms_id": "4yr-1yr-cliff-schedule"
-        },
-        {
-            "cost_basis": {
-                "amount": "0",
-                "currency": "USD"
-            },
-            "custom_id": "S-1",
-            "date": "2022-02-01",
             "id": "test-stock-issuance-with-share-tracking",
             "object_type": "TX_STOCK_ISSUANCE",
             "quantity": "1000",
             "security_id": "test-security-id",
             "security_law_exemptions": [],
             "share_numbers_issued": [
                 {
```

### Comparing `pyocf-1.0.0/tests/test_load.py` & `pyocf-1.0b1/tests/test_load.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,274 +1,339 @@
-# Copyright © 2023 FMR LLC
-
 import datetime
 import decimal
 import json
 
 from pathlib import Path
-from pyocf import api
+from pyocf.files import (
+    ocfmanifestfile,
+    stakeholdersfile,
+    stockclassesfile,
+    stocklegendtemplatesfile,
+    stockplansfile,
+    transactionsfile,
+    valuationsfile,
+    vestingtermsfile,
+)
 from pyocf.captable import Captable
+from pyocf.objects import (
+    transactions,
+    stockplan,
+    stakeholder,
+    stockclass,
+    stocklegendtemplate,
+    valuation,
+    vestingterms,
+)
+from pyocf.types import (
+    conversion_mechanisms as conv_mechs,
+    conversion_rights as conv_rights,
+    conversion_triggers as conv_trigs,
+    file,
+    interestrate,
+    name,
+    numeric,
+    monetary,
+    vesting,
+)
+from pyocf.enums import (
+    accrualperiodtype,
+    allocationtype,
+    compoundingtype,
+    daycounttype,
+    interestpayouttype,
+    ocfversiontype,
+    stockclasstype,
+    vestingdayofmonth,
+)
+
 
 sample_path = Path(Path(__file__).parent.parent, "Open-Cap-Format-OCF/samples")
 
 
 def test_load_sample_manifest():
     path = Path(Path(__file__).parent, Path(sample_path, "Manifest.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.OCFManifestFile(**json.load(infile))
+        obj = ocfmanifestfile.OCFManifestFile(**json.load(infile))
 
-    assert obj.ocf_version == api.OCFVersionType.ENUM_100
+    assert obj.ocf_version == ocfversiontype.OCFVersionType.ENUM_100
     assert obj.comments == [
         "This is an optional comment",
         """These md5 hashes are just dummy values. They've not been recalculated """
         """in a long time, but we should look into recalculating them dynamically """
         """via an actions or pre-commit hook.""",
     ]
     assert len(obj.stakeholders_files) == 1
-    assert isinstance(obj.stakeholders_files[0], api.File)
+    assert isinstance(obj.stakeholders_files[0], file.File)
 
 
 def test_load_sample_stakeholders():
     path = Path(Path(__file__).parent, Path(sample_path, "Stakeholders.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.StakeholdersFile(**json.load(infile))
+        obj = stakeholdersfile.StakeholdersFile(**json.load(infile))
     assert len(obj.items) == 2
     item = obj.items[0]
-    assert isinstance(item, api.Stakeholder)
+    assert isinstance(item, stakeholder.Stakeholder)
     assert item.object_type == "STAKEHOLDER"
-    assert isinstance(item.name, api.Name)
+    assert isinstance(item.name, name.Name)
 
 
 def test_load_sample_stock_classes():
     path = Path(Path(__file__).parent, Path(sample_path, "StockClasses.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.StockClassesFile(**json.load(infile))
+        obj = stockclassesfile.StockClassesFile(**json.load(infile))
 
     assert len(obj.items) == 2
     item = obj.items[0]
-    assert isinstance(item, api.StockClass)
+    assert isinstance(item, stockclass.StockClass)
     assert item.object_type == "STOCK_CLASS"
     assert item.name == "Common Stock"
-    assert item.class_type == api.StockClassType.ENUM_COMMON
-    assert isinstance(item.par_value, api.Monetary)
+    assert item.class_type == stockclasstype.StockClassType.ENUM_COMMON
+    assert isinstance(item.par_value, monetary.Monetary)
     assert item.par_value.currency == "USD"
     assert item.par_value.amount == decimal.Decimal("0.0001000000")
 
     item = obj.items[1]
-    assert item.class_type == api.StockClassType.ENUM_PREFERRED
+    assert item.class_type == stockclasstype.StockClassType.ENUM_PREFERRED
 
 
 def test_load_sample_stock_legend_templates():
     path = Path(Path(__file__).parent, Path(sample_path, "StockLegends.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.StockLegendTemplatesFile(**json.load(infile))
+        obj = stocklegendtemplatesfile.StockLegendTemplatesFile(**json.load(infile))
 
     assert len(obj.items) == 1
     item = obj.items[0]
-    assert isinstance(item, api.StockLegendTemplate)
+    assert isinstance(item, stocklegendtemplate.StockLegendTemplate)
     item.object_type == "STOCK_LEGEND_TEMPLATE"
     item.name == "1933 Act Legend"
 
 
 def test_load_sample_stock_plans():
     path = Path(Path(__file__).parent, Path(sample_path, "StockPlans.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.StockPlansFile(**json.load(infile))
+        obj = stockplansfile.StockPlansFile(**json.load(infile))
     assert len(obj.items) == 1
     item = obj.items[0]
-    assert isinstance(item, api.StockPlan)
+    assert isinstance(item, stockplan.StockPlan)
     assert item.object_type == "STOCK_PLAN"
     assert item.plan_name == "2021 Stock Incentive Plan"
     assert item.board_approval_date == datetime.date(1983, 12, 31)
     assert item.initial_shares_reserved == decimal.Decimal("10000000")
     assert item.stock_class_id == "8d8371e8-d41d-4a49-9f42-b91758fd155d"
     assert item.comments == [
         "Using new form of SOP released by Firm Y's benefits & comp team on 10/10/2021."
     ]
 
 
 def test_load_sample_transactions():
     path = Path(Path(__file__).parent, Path(sample_path, "Transactions.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.TransactionsFile(**json.load(infile))
+        obj = transactionsfile.TransactionsFile(**json.load(infile))
     item = obj.items[0]
-    assert isinstance(item, api.ConvertibleAcceptance)
+    assert isinstance(
+        item, transactions.acceptance.convertibleacceptance.ConvertibleAcceptance
+    )
     assert item.id == "test-convertible-acceptance-minimal"
     assert item.security_id == "2936wa8yefhdsvcn"
     assert item.object_type == "TX_CONVERTIBLE_ACCEPTANCE"
     assert item.date == datetime.date(2022, 1, 20)
 
     item = obj.items[8]
-    assert isinstance(item, api.ConvertibleIssuance)
+    assert isinstance(
+        item, transactions.issuance.convertibleissuance.ConvertibleIssuance
+    )
     assert item.id == "test-convertible-issuance-minimal"
     assert item.security_id == "con_123456"
     assert item.object_type == "TX_CONVERTIBLE_ISSUANCE"
     assert item.date == datetime.date(1978, 5, 27)
     assert item.comments is None
     trigger = item.conversion_triggers[0]
     assert isinstance(
         trigger,
-        api.AutomaticConversionOnDateTrigger,
+        conv_trigs.automaticconversionondatetrigger.AutomaticConversionOnDateTrigger,
     )
     assert trigger.type == "AUTOMATIC_ON_DATE"
     assert trigger.trigger_id == "CN-1.TRIG.1"
     assert trigger.nickname == "Converts on Maturity"
     assert (
         trigger.trigger_description == "The note shall convert on the date of maturity"
     )
     assert trigger.trigger_date == datetime.date(2022, 1, 1)
 
     cr = trigger.conversion_right
-    assert isinstance(cr, api.ConvertibleConversionRight)
+    assert isinstance(
+        cr, conv_rights.convertibleconversionright.ConvertibleConversionRight
+    )
     assert cr.type == "CONVERTIBLE_CONVERSION_RIGHT"
     cm = cr.conversion_mechanism
-    assert isinstance(cm, api.NoteConversionMechanism)
+    assert isinstance(cm, conv_mechs.noteconversionmechanism.NoteConversionMechanism)
     assert cm.type == "CONVERTIBLE_NOTE_CONVERSION"
-    assert cm.day_count_convention == api.DayCountType.ENUM_ACTUAL_365
-    assert cm.interest_payout == api.InterestPayoutType.ENUM_DEFERRED
-    assert cm.interest_accrual_period == api.AccrualPeriodType.ENUM_MONTHLY
-    assert cm.compounding_type == api.CompoundingType.ENUM_COMPOUNDING
+    assert cm.day_count_convention == daycounttype.DayCountType.ENUM_ACTUAL_365
+    assert cm.interest_payout == interestpayouttype.InterestPayoutType.ENUM_DEFERRED
+    assert (
+        cm.interest_accrual_period == accrualperiodtype.AccrualPeriodType.ENUM_MONTHLY
+    )
+    assert cm.compounding_type == compoundingtype.CompoundingType.ENUM_COMPOUNDING
     assert cm.conversion_discount is None
     assert cm.conversion_valuation_cap is None
     assert cm.exit_multiple is None
     assert cm.conversion_mfn is None
     ir = cm.interest_rates[0]
-    assert isinstance(ir, api.InterestRate)
+    assert isinstance(ir, interestrate.InterestRate)
     assert ir.rate == "0.0899"
     assert ir.accrual_start_date == datetime.date(2021, 1, 1)
     assert ir.accrual_end_date is None
 
     item = obj.items[58]
-    assert isinstance(item, api.WarrantAcceptance)
+    assert isinstance(item, transactions.acceptance.warrantacceptance.WarrantAcceptance)
     assert item.id == "test-warrant-acceptance-full-fields"
     assert item.security_id == "test-security-id"
     assert item.object_type == "TX_WARRANT_ACCEPTANCE"
     assert item.date == datetime.date(2022, 2, 1)
     assert item.comments == ["Here is a comment", "Here is another comment"]
 
     item = obj.items[63]
-    assert isinstance(item, api.WarrantIssuance)
+    assert isinstance(item, transactions.issuance.warrantissuance.WarrantIssuance)
     assert item.id == "test-warrant-issuance-minimal"
     assert item.custom_id == "W-1"
     assert item.object_type == "TX_WARRANT_ISSUANCE"
-    assert isinstance(item.exercise_price, api.Monetary)
+    assert isinstance(item.exercise_price, monetary.Monetary)
     assert item.exercise_price.amount == 1
-    assert isinstance(item.purchase_price, api.Monetary)
+    assert isinstance(item.purchase_price, monetary.Monetary)
     assert item.purchase_price.amount == 1
 
     et = item.exercise_triggers[0]
-    assert isinstance(et, api.AutomaticConversionOnConditionTrigger)
+    accot = conv_trigs.automaticconversiononconditiontrigger
+    assert isinstance(et, accot.AutomaticConversionOnConditionTrigger)
     assert et.type == "AUTOMATIC_ON_CONDITION"
     assert et.trigger_id == "WARRANT-1.TRIG.1"
     assert et.nickname.startswith("Automatic exercise immediately prior to")
 
     cr = et.conversion_right
-    assert isinstance(cr, api.WarrantConversionRight)
+    assert isinstance(cr, conv_rights.warrantconversionright.WarrantConversionRight)
     assert cr.type == "WARRANT_CONVERSION_RIGHT"
     assert cr.converts_to_future_round is None
     assert cr.converts_to_stock_class_id == "stock-class-id"
 
     cm = cr.conversion_mechanism
-    assert isinstance(cm, api.FixedAmountConversionMechanism)
+    assert isinstance(
+        cm, conv_mechs.fixedamountconversionmechanism.FixedAmountConversionMechanism
+    )
     assert cm.type == "FIXED_AMOUNT_CONVERSION"
     assert cm.converts_to_quantity == decimal.Decimal("10000.00")
 
     item = obj.items[67]
-    assert isinstance(item, api.WarrantRetraction)
+    assert isinstance(item, transactions.retraction.warrantretraction.WarrantRetraction)
     assert item.id == "test-warrant-retraction-full-fields"
     assert item.security_id == "test-security-id"
     assert item.object_type == "TX_WARRANT_RETRACTION"
     assert item.reason_text == "Need to retract"
     assert item.date == datetime.date(2022, 2, 1)
     assert item.comments == ["Here is a comment", "Here is another comment"]
 
 
 def test_load_sample_valuations_files():
     path = Path(Path(__file__).parent, Path(sample_path, "Valuations.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.ValuationsFile(**json.load(infile))
+        obj = valuationsfile.ValuationsFile(**json.load(infile))
 
     assert len(obj.items) == 1
     item = obj.items[0]
-    assert isinstance(item, api.Valuation)
+    assert isinstance(item, valuation.Valuation)
     item.object_type == "VALUATION"
     item.valuation_type == "409A",
 
 
 def test_load_sample_vesting_terms():
     path = Path(Path(__file__).parent, Path(sample_path, "VestingTerms.ocf.json"))
     with path.open("rt") as infile:
-        obj = api.VestingTermsFile(**json.load(infile))
+        obj = vestingtermsfile.VestingTermsFile(**json.load(infile))
 
     assert len(obj.items) == 5
     item = obj.items[0]
-    assert isinstance(item, api.VestingTerms)
+    assert isinstance(item, vestingterms.VestingTerms)
     item.object_type == "VESTING_TERMS"
     assert item.name == "Four Year / One Year Cliff"
-    assert item.allocation_type == api.AllocationType.ENUM_CUMULATIVE_ROUNDING
+    assert (
+        item.allocation_type == allocationtype.AllocationType.ENUM_CUMULATIVE_ROUNDING
+    )
 
     assert len(item.vesting_conditions) == 3
-    assert isinstance(item.vesting_conditions[0], api.VestingCondition)
+    assert isinstance(
+        item.vesting_conditions[0], vesting.vestingcondition.VestingCondition
+    )
     assert item.vesting_conditions[0].id == "vesting-start"
     assert item.vesting_conditions[0].next_condition_ids == ["cliff"]
 
     # Vesting conditions can have different trigger types
     condition = item.vesting_conditions[0]
-    assert isinstance(condition.trigger, api.VestingStartTrigger)
+    assert isinstance(
+        condition.trigger, vesting.vestingstarttrigger.VestingStartTrigger
+    )
     assert condition.portion is None
 
     condition = item.vesting_conditions[1]
-    assert isinstance(condition.portion, api.VestingConditionPortion)
+    assert isinstance(
+        condition.portion, vesting.vestingconditionportion.VestingConditionPortion
+    )
     # You can instantiate simple types by just passing in the value
-    assert condition.portion.numerator == api.Numeric("12")
+    assert condition.portion.numerator == numeric.Numeric("12")
     # But pydantic will pass it in with the name "__root__"
-    assert condition.portion.denominator == api.Numeric(__root__="48")
+    assert condition.portion.denominator == numeric.Numeric(__root__="48")
 
     trigger = condition.trigger
-    assert isinstance(trigger, api.VestingScheduleRelativeTrigger)
-    assert isinstance(trigger.period, api.VestingPeriodInMonths)
+    assert isinstance(
+        trigger, vesting.vestingschedulerelativetrigger.VestingScheduleRelativeTrigger
+    )
+    assert isinstance(
+        trigger.period, vesting.vestingperiodinmonths.VestingPeriodInMonths
+    )
     assert trigger.period.length == 12
     assert trigger.period.occurrences == 1
     assert (
         trigger.period.day_of_month
-        == api.VestingDayOfMonth.ENUM_VESTING_START_DAY_OR_LAST_DAY_OF_MONTH
+        == vestingdayofmonth.VestingDayOfMonth.ENUM_VESTING_START_DAY_OR_LAST_DAY_OF_MONTH
     )
 
     condition = item.vesting_conditions[2]
     trigger = condition.trigger
     assert trigger.period.length == 1
     assert trigger.period.occurrences == 36
 
     item = obj.items[1]
-    assert item.allocation_type == api.AllocationType.ENUM_CUMULATIVE_ROUND_DOWN
+    assert (
+        item.allocation_type == allocationtype.AllocationType.ENUM_CUMULATIVE_ROUND_DOWN
+    )
     assert len(item.vesting_conditions) == 8
-    assert isinstance(item.vesting_conditions[0], api.VestingCondition)
+    assert isinstance(
+        item.vesting_conditions[0], vesting.vestingcondition.VestingCondition
+    )
     assert item.vesting_conditions[0].id == "vesting-start"
 
     condition = item.vesting_conditions[1]
     assert condition.portion is None
     assert condition.quantity == 0
 
     condition = item.vesting_conditions[2]
     assert condition.portion.numerator == 1
     assert condition.portion.denominator == 1
 
     trigger = condition.trigger
-    assert isinstance(trigger, api.VestingEventTrigger)
+    assert isinstance(trigger, vesting.vestingeventtrigger.VestingEventTrigger)
     assert trigger.type == "VESTING_EVENT"
 
     item = obj.items[3]
-    assert item.allocation_type == api.AllocationType.ENUM_BACK_LOADED
+    assert item.allocation_type == allocationtype.AllocationType.ENUM_BACK_LOADED
 
     item = obj.items[4]
     condition = item.vesting_conditions[4]
     assert condition.quantity == 0
     assert isinstance(
         condition.trigger,
-        api.VestingScheduleAbsoluteTrigger,
+        vesting.vestingscheduleabsolutetrigger.VestingScheduleAbsoluteTrigger,
     )
     assert condition.trigger.date == datetime.date(2017, 4, 1)
 
 
 def test_load_captable_directory():
     path = Path(Path(__file__).parent, Path(sample_path, "Manifest.ocf.json"))
     # Just check that each type of data is not empty, ie, that it has been loaded.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.0/tests/test_save.py` & `pyocf-1.0b1/tests/test_save.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,47 @@
-# Copyright © 2023 FMR LLC
-
 import tempfile
 import zipfile
 
 from pathlib import Path
 
 from pyocf.captable import Captable
 
 sample_path = Path(Path(__file__).parent.parent, "Open-Cap-Format-OCF/samples")
 
 
 def test_save_zip():
     path = Path(Path(__file__).parent, "samples/Captable.ocf.zip")
     captable = Captable.load(path)
 
-    try:
-        with tempfile.TemporaryDirectory() as outdir:
-            outpath = Path(outdir, "outfile.zip")
-
-            captable.save(outpath, pretty=True)
-            with zipfile.ZipFile(outpath) as zipped:
-                assert len(zipped.filelist) == 8
-                # Make sure the manifest file is in there
-                assert zipped.filelist[7].filename == "Manifest.ocf.json"
-
-                manifest = zipped.open("Manifest.ocf.json")
-                data = manifest.read()
-
-                # Do some simple checks on the data
-                assert b'"file_type": "OCF_MANIFEST_FILE"' in data
-                assert b'"filepath": "StockLegends.ocf.json",' in data
-
-            outpath.unlink()
-
-    except (PermissionError, NotADirectoryError):
-        # Bugs in windows give permission errors for absolutely no reason
-        # when deleting temporary files. Ignore them.
-        pass
+    with tempfile.NamedTemporaryFile("wb") as outfile:
+        captable.save(outfile, pretty=True)
+
+        zipped = zipfile.ZipFile(outfile.name)
+        assert len(zipped.filelist) == 8
+        # Make sure the manifest file is in there
+        assert zipped.filelist[7].filename == "Manifest.ocf.json"
+
+        manifest = zipped.open("Manifest.ocf.json")
+        data = manifest.read()
+
+        # Do some simple checks on the data
+        assert b'"file_type": "OCF_MANIFEST_FILE"' in data
+        assert b'"filepath": "StockLegends.ocf.json",' in data
 
 
 def test_save_directory():
     path = Path(Path(__file__).parent, "samples/Captable.ocf.zip")
     captable = Captable.load(path)
 
-    try:
-        with tempfile.TemporaryDirectory() as outdir:
-            captable.save(outdir, zip=False, pretty=True)
-
-            path = Path(outdir)
-            files = [x for x in path.iterdir()]
-            assert len(files) == 8
-            # Make sure the manifest file is in there
-            manifest = [x for x in files if x.name == "Manifest.ocf.json"][0]
-            data = manifest.open("rb").read()
-
-            # Do some simple checks on the data
-            assert b'"file_type": "OCF_MANIFEST_FILE"' in data
-            assert b'"filepath": "StockLegends.ocf.json",' in data
-    except (PermissionError, NotADirectoryError):
-        # Bugs in windows give permission errors for absolutely no reason
-        # when deleting temporary files. Ignore them.
-        pass
+    with tempfile.TemporaryDirectory() as outdir:
+        captable.save(outdir, zip=False, pretty=True)
+
+        path = Path(outdir)
+        files = [x for x in path.iterdir()]
+        assert len(files) == 8
+        # Make sure the manifest file is in there
+        manifest = [x for x in files if x.name == "Manifest.ocf.json"][0]
+        data = manifest.open("rb").read()
+
+        # Do some simple checks on the data
+        assert b'"file_type": "OCF_MANIFEST_FILE"' in data
+        assert b'"filepath": "StockLegends.ocf.json",' in data
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.0/utils/generate.py` & `pyocf-1.0b1/utils/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,14 +334,17 @@
             if isinstance(superclass, Schema):
                 imports.add(superclass.import_statement)
             elif superclass == "BaseModel":
                 imports.add("from pydantic import BaseModel")
             elif superclass == "SimpleBaseModel":
                 imports.add("from pyocf.simplebase import SimpleBaseModel")
 
+        if list(self.validators):
+            imports.add("from pydantic import root_validator")
+
         if self.root_constraint:
             if "constr" in self.root_constraint:
                 imports.add("from pydantic import constr")
             if "date" in self.root_constraint:
                 imports.add("from datetime import date")
             if "Decimal" in self.root_constraint:
                 imports.add("from decimal import Decimal")
@@ -355,14 +358,43 @@
         path = ("pyocf",) + self.path.parts[root:]
         pkg = ".".join(path[:-1])
         module = self.filename.split(".")[0]
         imp = f"from {pkg}.{module} import {self.name}"
         return imp
 
     @property
+    def validators(self):
+        """Custom validators, pretty unique per class"""
+        if "anyOf" in self.json:
+            # This currently just supports the case when one property is
+            # required when another property is set to a specific value,
+            # like PlanSecurityIssuance.schema.json
+            assert len(self.json["anyOf"]) == 2
+            for item in self.json["anyOf"]:
+                if "required" in item:
+                    break
+            else:
+                return None
+
+            parameter = list(item["properties"].keys())[0]
+            value = item["properties"][parameter]["const"]
+            required = item["required"][0]
+
+            yield f"""@root_validator(pre=True)
+    def validator_{parameter}(cls, values):
+        if (values.get("{parameter}") == "{value}" and
+            values.get("{required}") is None):
+            raise ValueError(
+                "When {parameter} is '{value}' then {required} is required"
+            )
+
+        return values
+"""
+
+    @property
     def root_constraint(self):
         if "format" in self.json:
             return self.json["format"]
         if self.name == "Numeric":
             return "Decimal"
 
         if "pattern" in self.json:
@@ -386,53 +418,35 @@
         if filepath.name.startswith("_"):
             continue
         if filepath.is_dir():
             make_inits(filepath, types)
         elif not filepath.name.endswith(".py"):
             continue
 
-    with pathlib.Path(path, "__init__.py").open("wt", encoding="utf-8") as initfile:
+    with pathlib.Path(path, "__init__.py").open("wt") as initfile:
         initfile.write(f'"""OCF {path.parts[-1]}"""')
 
 
 def generate_files():
     templdir = pathlib.Path(__file__).parent
     outdir = pathlib.Path(templdir.parent, "src/pyocf")
     types = defaultdict(dict)
     roottypes = defaultdict(dict)
-    all_classes = {}
     for schema in all_schemas.values():
         rootlevel = schema.path.parts.index("schema") + 1
         schema_dir = pathlib.Path(*schema.path.parts[rootlevel:-1])
         object_type = schema.object_type
         if object_type is not None:
             types[pathlib.Path(outdir, schema_dir)][object_type] = schema
             roottypes[object_type] = schema
         tmpl = Template(filename=f"{templdir}/{schema.metatype}.mako")
         path = pathlib.Path(schema_dir, schema.filename + ".py")
         outfile = pathlib.Path(outdir, path)
         outfile.parent.mkdir(parents=True, exist_ok=True)
-        with outfile.open("wt", encoding="utf-8") as outfile:
+        with outfile.open("tw") as outfile:
             outfile.write(tmpl.render(schema=schema))
-        if schema.name in all_classes:
-            raise ValueError(
-                "The schema has changed to include duplicate class names, "
-                "that's new and needs dealing with!"
-            )
-        all_classes[schema.name] = schema.import_statement
-
-    classes_file = pathlib.Path(outdir, "api.py")
-    with classes_file.open("wt", encoding="utf-8") as outfile:
-        outfile.write('"""All PyOCF classes, for easier import"""\n\n')
-        outfile.write("# Autogenerated, do not edit.\n# Copyright © 2023 FMR LLC\n\n")
-
-        for imports in sorted(all_classes.values()):
-            outfile.write(f"{imports}\n")
-
-        outfile.write(f"\n__all__ = [{', '.join(sorted(all_classes))}]")
-
     make_inits(outdir, types)
 
 
 if __name__ == "__main__":
     load_schemas("./Open-Cap-Format-OCF/schema")
     generate_files()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyocf-1.0.0/utils/object.mako` & `pyocf-1.0b1/utils/object.mako`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-"""${schema.description}"""
+"""${schema.description.splitlines()[0]}"""
 
 # Autogenerated, do not edit.
-# Copyright © 2023 FMR LLC
+# Copyright © 2023 Shoobx, Fidelity Investments
 #
 # Based on the Open Captable Format schema:
 % for line in schema.comment.splitlines():
 # ${line}
 % endfor
 
 % if schema.import_statements:
@@ -25,7 +25,11 @@
     % endif
     % for property in schema.properties:
     % for line in property.description:
     # ${line}
     % endfor
     ${property.definition}
     % endfor
+
+    % for validator in schema.validators:
+    ${validator}
+    % endfor
```

