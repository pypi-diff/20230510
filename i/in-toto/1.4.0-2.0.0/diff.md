# Comparing `tmp/in_toto-1.4.0.tar.gz` & `tmp/in_toto-2.0.0.tar.gz`

## Comparing `in_toto-1.4.0.tar` & `in_toto-2.0.0.tar`

### file list

```diff
@@ -1,96 +1,116 @@
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 in_toto-1.4.0/.coveragerc
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements-dev.txt
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements-docs.txt
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements-pinned.txt
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements-tox.txt
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 in_toto-1.4.0/requirements.txt
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 in_toto-1.4.0/tox.ini
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/__init__.py
--rw-r--r--   0        0        0     6404 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/common_args.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/exceptions.py
--rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/formats.py
--rw-r--r--   0        0        0     4893 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_keygen.py
--rwxr-xr-x   0        0        0     3571 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_mock.py
--rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_record.py
--rwxr-xr-x   0        0        0     8666 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_run.py
--rw-r--r--   0        0        0    12640 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_sign.py
--rwxr-xr-x   0        0        0     7426 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/in_toto_verify.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/log.py
--rw-r--r--   0        0        0    10037 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/rulelib.py
--rw-r--r--   0        0        0    40820 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/runlib.py
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/settings.py
--rw-r--r--   0        0        0     5943 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/user_settings.py
--rw-r--r--   0        0        0    50740 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/verifylib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/__init__.py
--rw-r--r--   0        0        0     7659 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/_signer.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/common.py
--rw-r--r--   0        0        0    22230 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/layout.py
--rw-r--r--   0        0        0     5682 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/link.py
--rw-r--r--   0        0        0    13268 2020-02-02 00:00:00.000000 in_toto-1.4.0/in_toto/models/metadata.py
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/__init__.py
--rw-r--r--   0        0        0     5395 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/common.py
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/runtests.py
--rw-r--r--   0        0        0     3549 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_common_args.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_keygen.py
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_mock.py
--rw-r--r--   0        0        0    11441 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_record.py
--rwxr-xr-x   0        0        0    13626 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_run.py
--rw-r--r--   0        0        0    13346 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_sign.py
--rwxr-xr-x   0        0        0    13887 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_in_toto_verify.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_log.py
--rw-r--r--   0        0        0     6422 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_param_substitution.py
--rw-r--r--   0        0        0    10867 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_rulelib.py
--rwxr-xr-x   0        0        0    39644 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_runlib.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_settings.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_user_settings.py
--rw-r--r--   0        0        0    59574 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/test_verifylib.py
--rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_dsse_files/demo.layout.template
--rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_dsse_files/package.2f89b927.link
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_dsse_files/write-code.776a00e2.link
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/alice
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/alice.pub
--rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/bob
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/bob.pub
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/carl
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/carl.pub
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/danny
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/danny.pub
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/demo.layout.template
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/foo.tar.gz
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/package.2f89b927.link
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files/write-code.776a00e2.link
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files_gpg/demo.layout.template
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files_gpg/foo.tar.gz
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files_gpg/package.7b3abb26.link
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/demo_files_gpg/write-code.8288ef56.link
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/random_seed
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/secring.gpg
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/dsa/trustdb.gpg
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
--rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/pubring.gpg
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/random_seed
--rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/secring.gpg
--rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/gpg_keyrings/rsa/trustdb.gpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/__init__.py
--rwxr-xr-x   0        0        0      701 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_common.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_envelope.py
--rwxr-xr-x   0        0        0     1820 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_inspection.py
--rwxr-xr-x   0        0        0    13227 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_layout.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_link.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_metadata.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_signer.py
--rwxr-xr-x   0        0        0     2943 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_step.py
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/models/test_supply_chain_item.py
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/rc_test/.in_totorc
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/scripts/expr
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/scripts/tar
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 in_toto-1.4.0/tests/scripts/touch
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 in_toto-1.4.0/.gitignore
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 in_toto-1.4.0/LICENSE
--rw-r--r--   0        0        0    11304 2020-02-02 00:00:00.000000 in_toto-1.4.0/README.md
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 in_toto-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    12838 2020-02-02 00:00:00.000000 in_toto-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 in_toto-2.0.0/.coveragerc
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 in_toto-2.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 in_toto-2.0.0/requirements-docs.txt
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 in_toto-2.0.0/requirements-pinned.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 in_toto-2.0.0/requirements-tox.txt
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 in_toto-2.0.0/requirements.txt
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 in_toto-2.0.0/tox.ini
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/__init__.py
+-rw-r--r--   0        0        0     6705 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/common_args.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/exceptions.py
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/formats.py
+-rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/in_toto_keygen.py
+-rwxr-xr-x   0        0        0     2594 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/in_toto_match_products.py
+-rwxr-xr-x   0        0        0     3810 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/in_toto_mock.py
+-rw-r--r--   0        0        0     9387 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/in_toto_record.py
+-rwxr-xr-x   0        0        0     9494 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/in_toto_run.py
+-rw-r--r--   0        0        0    14178 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/in_toto_sign.py
+-rwxr-xr-x   0        0        0     8352 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/in_toto_verify.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/log.py
+-rw-r--r--   0        0        0    11311 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/rulelib.py
+-rw-r--r--   0        0        0    38741 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/runlib.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/settings.py
+-rw-r--r--   0        0        0    55967 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/verifylib.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/models/__init__.py
+-rw-r--r--   0        0        0     8402 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/models/_signer.py
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/models/common.py
+-rw-r--r--   0        0        0    24409 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/models/layout.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/models/link.py
+-rw-r--r--   0        0        0    14378 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/models/metadata.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/resolver/__init__.py
+-rw-r--r--   0        0        0     8456 2020-02-02 00:00:00.000000 in_toto-2.0.0/in_toto/resolver/_resolver.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     5830 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/common.py
+-rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/runtests.py
+-rw-r--r--   0        0        0     3865 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_common_args.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_in_toto_keygen.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_in_toto_match_products.py
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_in_toto_mock.py
+-rw-r--r--   0        0        0    14461 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_in_toto_record.py
+-rwxr-xr-x   0        0        0    16277 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_in_toto_run.py
+-rw-r--r--   0        0        0    17737 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_in_toto_sign.py
+-rwxr-xr-x   0        0        0    15769 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_in_toto_verify.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_log.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_ostree_resolver.py
+-rw-r--r--   0        0        0     8087 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_param_substitution.py
+-rw-r--r--   0        0        0     3016 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_resolver.py
+-rw-r--r--   0        0        0    13445 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_rulelib.py
+-rwxr-xr-x   0        0        0    49785 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_runlib.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_settings.py
+-rw-r--r--   0        0        0    68055 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/test_verifylib.py
+-rw-r--r--   0        0        0     3637 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_dsse_files/demo.layout.template
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_dsse_files/package.2f89b927.link
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_dsse_files/write-code.776a00e2.link
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/alice
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/alice.pub
+-rw-r--r--   0        0        0     2459 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/bob
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/bob.pub
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/carl
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/carl.pub
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/danny
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/danny.pub
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/demo.layout.template
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/foo.tar.gz
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/package.2f89b927.link
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files/write-code.776a00e2.link
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files_gpg/demo.layout.template
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files_gpg/foo.tar.gz
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files_gpg/package.7b3abb26.link
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/demo_files_gpg/write-code.8288ef56.link
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/dsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/dsa/random_seed
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/dsa/secring.gpg
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/dsa/trustdb.gpg
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/rsa/7B3ABB26B97B655AB9296BD15B0BD02E1C768C43.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/rsa/8288EF560ED3795F9DF2C0DB56193089B285DA58.ssh
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/rsa/8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17.ssh
+-rw-r--r--   0        0        0    17740 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/rsa/pubring.gpg
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/rsa/random_seed
+-rw-r--r--   0        0        0    27893 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/rsa/secring.gpg
+-rw-r--r--   0        0        0     1960 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/gpg_keyrings/rsa/trustdb.gpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/__init__.py
+-rwxr-xr-x   0        0        0      714 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/test_common.py
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/test_envelope.py
+-rwxr-xr-x   0        0        0     1931 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/test_inspection.py
+-rwxr-xr-x   0        0        0    14364 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/test_layout.py
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/test_link.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/test_metadata.py
+-rw-r--r--   0        0        0     5449 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/test_signer.py
+-rwxr-xr-x   0        0        0     3150 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/test_step.py
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/models/test_supply_chain_item.py
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/rc_test/.in_totorc
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/config
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/04/d3e76d327333f3a5fcfb2fd067b90cc36a906d23db28adb3819e02e99f0f6a.dirtree
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/17/57d5e638ba33b5b43bee22ad24f8eecd14487965c076225664e64787a772c4.file
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/46/33304404a9fb8b9c98145aa85851d285b491e3b77e9cef663392857c4b1000.file
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/57/3c8b6ed22f77d085206364b0fca4334ab88c429a4e3d335f9b863ca421adc6.dirtree
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/6d/f05c195832bd23b044a3fdd76b3a30011c762dea6c271133cb20f7309abcb5.dirtree
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/6e/340b9cffb37a989ca544e6bb780a2c78901d3fb33738768511a30617afa01d.dirtree
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/77/3e0833bada391e17908ef72be2f3bab9662b6223b5cd6064af8ce7753368d1.dirtree
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/85/b69cc1ae509c55992d4eb47572cebb0fcfdf640aa2cdc0ad4b517cb6cf8b5d.dirtree
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/a6/1f97fffc19dbe77a59de47641b16a03a6a835cbe3d7f8a86f4fbb85342b551.file
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/cd/1875c7cb1d1c169f4ae48baee61c00d1be51efe0f0c2777759644e3a62012f.dirmeta
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/cf/3e103a6aed64aec261e2161d1026aa26349d422d238b1ad9e2e2a7eeed8591.commit
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/e3/777ae4075244944a952fa9705d5b26fa24cf5a841e7ce278f390ee3fc1928b.dirtree
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/f3/43cfdc0f6c428bdb30fc0dbf6c230972564153579b68e5fe5261444cf65abe.file
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/objects/f7/d5cf77d40b20cbf35b0de40a6bc693d13afeac5c1e07b63f71754e0d6704a2.dirtree
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/resolver/ostree_repo/refs/heads/test-branch
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/scripts/expr
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/scripts/tar
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 in_toto-2.0.0/tests/scripts/touch
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 in_toto-2.0.0/.gitignore
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 in_toto-2.0.0/LICENSE
+-rw-r--r--   0        0        0    10611 2020-02-02 00:00:00.000000 in_toto-2.0.0/README.md
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 in_toto-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    12196 2020-02-02 00:00:00.000000 in_toto-2.0.0/PKG-INFO
```

### Comparing `in_toto-1.4.0/requirements-pinned.txt` & `in_toto-2.0.0/requirements-pinned.txt`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/in_toto/common_args.py` & `in_toto-2.0.0/in_toto/common_args.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,178 +26,212 @@
   parser = argparse.ArgumentParser()
   parser.add_argument(*EXCLUDE_KWARGS, **EXCLUDE_KWARGS)
   ```
 
 """
 import sys
 
-from in_toto import (SUPPORTED_KEY_TYPES, KEY_TYPE_RSA, KEY_TYPE_ED25519,
-                    KEY_TYPE_ECDSA)
+from in_toto import (
+    KEY_TYPE_ECDSA,
+    KEY_TYPE_ED25519,
+    KEY_TYPE_RSA,
+    SUPPORTED_KEY_TYPES,
+)
 
 EXCLUDE_ARGS = ["--exclude"]
 EXCLUDE_KWARGS = {
-  "dest": "exclude_patterns",
-  "required": False,
-  "metavar": "<pattern>",
-  "nargs": "+",
-  "help": ("path patterns to match paths that should not be recorded as"
-           " 'materials' or 'products'. Passed patterns override patterns"
-           " defined in environment variables or config files. See Config docs"
-           " for details.")
-  }
+    "dest": "exclude_patterns",
+    "required": False,
+    "metavar": "<pattern>",
+    "nargs": "+",
+    "help": (
+        "path patterns to match paths that should not be recorded as"
+        " 'materials' or 'products'. Passed patterns override patterns"
+        " defined in environment variables or config files. See Config docs"
+        " for details."
+    ),
+}
 
 BASE_PATH_ARGS = ["--base-path"]
 BASE_PATH_KWARGS = {
-  "dest": "base_path",
-  "required": False,
-  "metavar": "<path>",
-  "help": ("base path for relative paths passed via '--materials' and"
-           " '--products'. It is used to locate and record artifacts, and is"
-           " not included in the resulting link metadata. Default is the"
-           " current working directory.")
-  }
+    "dest": "base_path",
+    "required": False,
+    "metavar": "<path>",
+    "help": (
+        "base path for relative paths passed via '--materials' and"
+        " '--products'. It is used to locate and record artifacts, and is"
+        " not included in the resulting link metadata. Default is the"
+        " current working directory."
+    ),
+}
 
 LSTRIP_PATHS_ARGS = ["--lstrip-paths"]
 LSTRIP_PATHS_KWARGS = {
-  "dest": "lstrip_paths",
-  "required": False,
-  "nargs": "+",
-  "metavar": "<path>",
-  "help": ("path prefixes used to left-strip artifact paths before storing"
-           " them to the resulting link metadata. If multiple prefixes are"
-           " specified, only a single prefix can match the path of any"
-           " artifact and that is then left-stripped. All prefixes are checked"
-           " to ensure none of them are a left substring of another.")
+    "dest": "lstrip_paths",
+    "required": False,
+    "nargs": "+",
+    "metavar": "<path>",
+    "help": (
+        "path prefixes used to left-strip artifact paths before storing"
+        " them to the resulting link metadata. If multiple prefixes are"
+        " specified, only a single prefix can match the path of any"
+        " artifact and that is then left-stripped. All prefixes are checked"
+        " to ensure none of them are a left substring of another."
+    ),
 }
 
 KEY_ARGS = ["-k", "--key"]
 KEY_KWARGS = {
- "type": str,
- "metavar": "<path>",
- "help": ("path to a private key file to sign the resulting link metadata."
-          " The keyid prefix is used as an infix for the link metadata"
-          " filename, i.e. '<name>.<keyid prefix>.link'. See '--key-type' for"
-          " available formats. Passing one of '--key' or '--gpg' is required.")
+    "type": str,
+    "metavar": "<path>",
+    "help": (
+        "path to a private key file to sign the resulting link metadata."
+        " The keyid prefix is used as an infix for the link metadata"
+        " filename, i.e. '<name>.<keyid prefix>.link'. See '--key-type' for"
+        " available formats. Passing one of '--key' or '--gpg' is required."
+    ),
 }
 
 KEY_TYPE_ARGS = ["-t", "--key-type"]
 KEY_TYPE_KWARGS = {
-  "dest": "key_type",
-  "type": str,
-  "choices": SUPPORTED_KEY_TYPES,
-  "default": KEY_TYPE_RSA,
-  "help": ("type of key specified by the '--key' option. '{rsa}' keys are"
-           " expected in a 'PEM' format. '{ed25519}' and '{ecdsa}' are"
-           " expected to be in a custom 'securesystemslib/json' format."
-           " Default is '{rsa}'."
-           .format(rsa=KEY_TYPE_RSA, ed25519=KEY_TYPE_ED25519,
-                   ecdsa=KEY_TYPE_ECDSA))
+    "dest": "key_type",
+    "type": str,
+    "choices": SUPPORTED_KEY_TYPES,
+    "default": KEY_TYPE_RSA,
+    "help": (
+        "type of key specified by the '--key' option. '{rsa}' keys are"
+        " expected in a 'PEM' format. '{ed25519}' and '{ecdsa}' are"
+        " expected to be in a custom 'securesystemslib/json' format."
+        " Default is '{rsa}'.".format(
+            rsa=KEY_TYPE_RSA, ed25519=KEY_TYPE_ED25519, ecdsa=KEY_TYPE_ECDSA
+        )
+    ),
 }
 
 KEY_PASSWORD_ARGS = ["-P", "--password"]
 KEY_PASSWORD_KWARGS = {
-  "nargs": "?",
-  "const": True,
-  "metavar": "<password>",
-  "help": ("password for encrypted key specified with '--key'. Passing  '-P'"
-           " without <password> opens a prompt. If no password is passed, or"
-           " entered on the prompt, the key is treated as unencrypted. (Do "
-           " not confuse with '-p/--products'!)")
+    "nargs": "?",
+    "const": True,
+    "metavar": "<password>",
+    "help": (
+        "password for encrypted key specified with '--key'. Passing  '-P'"
+        " without <password> opens a prompt. If no password is passed, or"
+        " entered on the prompt, the key is treated as unencrypted. (Do "
+        " not confuse with '-p/--products'!)"
+    ),
 }
 OPTS_TITLE = "Optional Arguments" if sys.version_info < (3, 10) else "Options"
+
+
 def parse_password_and_prompt_args(args):
-  """Parse -P/--password optional arg (nargs=?, const=True). """
-   # --P was provided without argument (True)
-  if args.password is True:
-    password = None
-    prompt = True
-  # --P was not provided (None), or provided with argument (<password>)
-  else:
-    password = args.password
-    prompt = False
+    """Parse -P/--password optional arg (nargs=?, const=True)."""
+    # --P was provided without argument (True)
+    if args.password is True:
+        password = None
+        prompt = True
+    # --P was not provided (None), or provided with argument (<password>)
+    else:
+        password = args.password
+        prompt = False
+
+    return password, prompt
 
-  return password, prompt
 
 GPG_ARGS = ["-g", "--gpg"]
 GPG_KWARGS = {
-  "nargs": "?",
-  "const": True,
-  "metavar": "<id>",
-  "help": ("GPG keyid to sign the resulting link metadata.  When '--gpg' is"
-           " passed without the keyid, the default GPG key is used. The keyid"
-           " prefix is used as an infix for the link metadata filename, i.e."
-           " '<name>.<keyid prefix>.link'. Passing one of '--key' or '--gpg'"
-           " is required.")
+    "nargs": "?",
+    "const": True,
+    "metavar": "<id>",
+    "help": (
+        "GPG keyid to sign the resulting link metadata.  When '--gpg' is"
+        " passed without the keyid, the default GPG key is used. The keyid"
+        " prefix is used as an infix for the link metadata filename, i.e."
+        " '<name>.<keyid prefix>.link'. Passing one of '--key' or '--gpg'"
+        " is required."
+    ),
 }
 
 GPG_HOME_ARGS = ["--gpg-home"]
 GPG_HOME_KWARGS = {
-  "dest": "gpg_home",
-  "type": str,
-  "metavar": "<path>",
-  "help": ("path to a GPG home directory used to load a GPG key identified"
-           " by '--gpg'. If '--gpg-home' is not passed, the default GPG home"
-           " directory is used.")
+    "dest": "gpg_home",
+    "type": str,
+    "metavar": "<path>",
+    "help": (
+        "path to a GPG home directory used to load a GPG key identified"
+        " by '--gpg'. If '--gpg-home' is not passed, the default GPG home"
+        " directory is used."
+    ),
 }
 
 VERBOSE_ARGS = ["-v", "--verbose"]
 VERBOSE_KWARGS = {
-  "dest": "verbose",
-  "action": "store_true",
-  "help": "show more output"
+    "dest": "verbose",
+    "action": "store_true",
+    "help": "show more output",
 }
 
 QUIET_ARGS = ["-q", "--quiet"]
 QUIET_KWARGS = {
-  "dest": "quiet",
-  "action": "store_true",
-  "help": "suppress all output"
+    "dest": "quiet",
+    "action": "store_true",
+    "help": "suppress all output",
 }
 
 METADATA_DIRECTORY_ARGS = ["-d", "--metadata-directory"]
 METADATA_DIRECTORY_KWARGS = {
-  "required": False,
-  "type": str,
-  "metavar": "<directory>",
-  "help": ("path to a directory to dump metadata. If '--metadata-directory'"
-           " is not passed, the current working direcotry is used.")
+    "required": False,
+    "type": str,
+    "metavar": "<directory>",
+    "help": (
+        "path to a directory to dump metadata. If '--metadata-directory'"
+        " is not passed, the current working direcotry is used."
+    ),
 }
 
 DSSE_ARGS = ["--use-dsse"]
 DSSE_KWARGS = {
-  "dest": "use_dsse",
-  "default": False,
-  "action": "store_true",
-  "help": ("generate metadata using dsse (experimental)."),
+    "dest": "use_dsse",
+    "default": False,
+    "action": "store_true",
+    "help": ("generate metadata using dsse (experimental)."),
 }
 
 
 def title_case_action_groups(parser):
-  """Capitalize the first character of all words in the title of each action
-  group of the passed parser.
+    """Capitalize the first character of all words in the title of each action
+    group of the passed parser.
 
-  This is useful for consistency when using the sphinx argparse extension,
-  which title-cases default action groups only.
+    This is useful for consistency when using the sphinx argparse extension,
+    which title-cases default action groups only.
 
-  """
-  for action_group in parser._action_groups: # pylint: disable=protected-access
-    action_group.title = action_group.title.title()
+    """
+    for (
+        action_group
+    ) in parser._action_groups:  # pylint: disable=protected-access
+        action_group.title = action_group.title.title()
 
 
 def sort_action_groups(parser, title_order=None):
-  """Sort action groups of passed parser by their titles according to the
-  passed (or a default) order.
-
-  """
-  if title_order is None:
-    title_order = ["Required Named Arguments", "Positional Arguments",
-                   OPTS_TITLE]
-
-  action_group_dict = {}
-  for action_group in parser._action_groups: # pylint: disable=protected-access
-    action_group_dict[action_group.title] = action_group
-
-  ordered_action_groups = []
-  for title in title_order:
-    ordered_action_groups.append(action_group_dict[title])
+    """Sort action groups of passed parser by their titles according to the
+    passed (or a default) order.
 
-  parser._action_groups = ordered_action_groups # pylint: disable=protected-access
+    """
+    if title_order is None:
+        title_order = [
+            "Required Named Arguments",
+            "Positional Arguments",
+            OPTS_TITLE,
+        ]
+
+    action_group_dict = {}
+    for (
+        action_group
+    ) in parser._action_groups:  # pylint: disable=protected-access
+        action_group_dict[action_group.title] = action_group
+
+    ordered_action_groups = []
+    for title in title_order:
+        ordered_action_groups.append(action_group_dict[title])
+
+    parser._action_groups = (  # pylint: disable=protected-access
+        ordered_action_groups
+    )
```

### Comparing `in_toto-1.4.0/in_toto/exceptions.py` & `in_toto-2.0.0/in_toto/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 # Copyright New York University and the in-toto contributors
 # SPDX-License-Identifier: Apache-2.0
 
 # TODO: Add module docstring and remove pylint exemption in in-toto/in-toto#126
 # pylint: disable=missing-docstring
 from securesystemslib.exceptions import Error
 
+
 class SignatureVerificationError(Error):
-  """Indicates a signature verification Error. """
+    """Indicates a signature verification Error."""
+
 
 class LayoutExpiredError(Error):
-  """Indicates that the layout expired. """
+    """Indicates that the layout expired."""
+
 
 class RuleVerificationError(Error):
-  """Indicates that artifact rule verification failed. """
+    """Indicates that artifact rule verification failed."""
+
 
 class ThresholdVerificationError(Error):
-  """Indicates that signature threshold verification failed. """
+    """Indicates that signature threshold verification failed."""
+
 
 class BadReturnValueError(Error):
-  """Indicates that a ran command exited with non-int or non-zero return
-  value. """
+    """Indicates that a ran command exited with non-int or non-zero return
+    value."""
+
 
 class LinkNotFoundError(Error):
-  """Indicates that a link file was not found. """
+    """Indicates that a link file was not found."""
+
 
 class UnsupportedKeyTypeError(Error):
-  """Indicates that the specified key type is not yet supported. """
+    """Indicates that the specified key type is not yet supported."""
+
 
 class PrefixError(Error):
-  """Indicates that there is an error because of the prefixes passed. """
+    """Indicates that there is an error because of the prefixes passed."""
+
 
 class InvalidMetadata(Error):
-  """Indicates that the metadata is not valid."""
+    """Indicates that the metadata is not valid."""
```

### Comparing `in_toto-1.4.0/in_toto/formats.py` & `in_toto-2.0.0/in_toto/formats.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,11 +27,11 @@
   `check_match` raises a securesystemslib.exceptions.FormatError and `matches`
   returns False if the verified object does not match the schema (True
   otherwise).
 
 """
 import securesystemslib.schema as ssl_schema
 
-PARAMETER_DICTIONARY_KEY = ssl_schema.RegularExpression(r'[a-zA-Z0-9_-]+')
+PARAMETER_DICTIONARY_KEY = ssl_schema.RegularExpression(r"[a-zA-Z0-9_-]+")
 PARAMETER_DICTIONARY_SCHEMA = ssl_schema.DictOf(
-    key_schema = PARAMETER_DICTIONARY_KEY,
-    value_schema = ssl_schema.AnyString())
+    key_schema=PARAMETER_DICTIONARY_KEY, value_schema=ssl_schema.AnyString()
+)
```

### Comparing `in_toto-1.4.0/in_toto/in_toto_keygen.py` & `in_toto-2.0.0/in_toto/in_toto_keygen.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,50 +25,56 @@
 
 <Return Codes>
   2 if an exception occurred during argument parsing
   1 if an exception occurred
   0 if no exception occurred
 
 """
-import sys
 import argparse
 import logging
+import sys
 
-from in_toto.common_args import title_case_action_groups
-from in_toto import (
-    __version__, SUPPORTED_KEY_TYPES, KEY_TYPE_RSA, KEY_TYPE_ED25519,
-    KEY_TYPE_ECDSA)
 from securesystemslib import interface
 
+from in_toto import (
+    KEY_TYPE_ECDSA,
+    KEY_TYPE_ED25519,
+    KEY_TYPE_RSA,
+    SUPPORTED_KEY_TYPES,
+    __version__,
+)
+from in_toto.common_args import title_case_action_groups
+
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
 
 def create_parser():
-  """
-  <Purpose>
-    A function which parses the user supplied arguments.
-
-  <Arguments>
-    None
-
-  <Exceptions>
-    None
-
-  <Returns>
-    Parsed arguments (args object)
-  """
-  parser = argparse.ArgumentParser(
-    formatter_class=argparse.RawDescriptionHelpFormatter,
-    description="in-toto-keygen is a tool to generate, optionally encrypt, and"
-                " write cryptographic keys to disk. These keys may be used"
-                " with other in-toto tooling to e.g. sign or verify link or"
-                " layout metadata.")
+    """
+    <Purpose>
+      A function which parses the user supplied arguments.
+
+    <Arguments>
+      None
+
+    <Exceptions>
+      None
+
+    <Returns>
+      Parsed arguments (args object)
+    """
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description="in-toto-keygen is a tool to generate, optionally encrypt, and"
+        " write cryptographic keys to disk. These keys may be used"
+        " with other in-toto tooling to e.g. sign or verify link or"
+        " layout metadata.",
+    )
 
-  parser.epilog = """EXAMPLE USAGE
+    parser.epilog = """EXAMPLE USAGE
 
 Generate RSA key pair of size 2048 bits, prompt for a password to encrypt
 the private key, and write 'alice' (private encrypted) and 'alice.pub' (public)
 as PEM-formatted key files to the current working directory.
 
   in-toto-keygen -p -t rsa -b 2048 alice
 
@@ -78,72 +84,106 @@
 directory.
 
   in-toto-keygen -t ed25519 bob
 
 
 """
 
-  parser.add_argument("-p", "--prompt", action="store_true",
-                            help="prompts for a password used to encrypt the"
-                            " private key before storing it")
-
-  parser.add_argument("-t", "--type", type=str,
-                            choices=SUPPORTED_KEY_TYPES,
-                            default=KEY_TYPE_RSA,
-                            help="type of the key to be generated. '{rsa}'"
-                            " keys are written in a 'PEM' format. '{ed25519}'"
-                            " and '{ecdsa}' keys are written in a custom"
-                            " 'securesystemslib/json' format. Default is"
-                            " '{rsa}'.".format(rsa=KEY_TYPE_RSA,
-                                               ed25519=KEY_TYPE_ED25519,
-                                               ecdsa=KEY_TYPE_ECDSA))
-
-
-  parser.add_argument("name", type=str, metavar="<filename>",
-                            help="filename for the resulting key files, which"
-                            " are written to '<filename>' (private key) and"
-                            " '<filename>.pub' (public key).")
-
-  parser.add_argument("-b", "--bits", default=3072, type=int, metavar="<bits>",
-                            help="key size, or key length, of the RSA key")
-
-  parser.add_argument('--version', action='version',
-                      version='{} {}'.format(parser.prog, __version__))
+    parser.add_argument(
+        "-p",
+        "--prompt",
+        action="store_true",
+        help="prompts for a password used to encrypt the"
+        " private key before storing it",
+    )
+
+    parser.add_argument(
+        "-t",
+        "--type",
+        type=str,
+        choices=SUPPORTED_KEY_TYPES,
+        default=KEY_TYPE_RSA,
+        help="type of the key to be generated. '{rsa}'"
+        " keys are written in a 'PEM' format. '{ed25519}'"
+        " and '{ecdsa}' keys are written in a custom"
+        " 'securesystemslib/json' format. Default is"
+        " '{rsa}'.".format(
+            rsa=KEY_TYPE_RSA, ed25519=KEY_TYPE_ED25519, ecdsa=KEY_TYPE_ECDSA
+        ),
+    )
+
+    parser.add_argument(
+        "name",
+        type=str,
+        metavar="<filename>",
+        help="filename for the resulting key files, which"
+        " are written to '<filename>' (private key) and"
+        " '<filename>.pub' (public key).",
+    )
+
+    parser.add_argument(
+        "-b",
+        "--bits",
+        default=3072,
+        type=int,
+        metavar="<bits>",
+        help="key size, or key length, of the RSA key",
+    )
+
+    parser.add_argument(
+        "--version",
+        action="version",
+        version="{} {}".format(parser.prog, __version__),
+    )
 
-  title_case_action_groups(parser)
-
-  return parser
+    title_case_action_groups(parser)
 
+    return parser
 
 
 def main():
-  """
-  First calls parse_args to parse the arguments, and then calls either
-  _generate_and_write_rsa_keypair or _generate_and_write_ed25519_keypair
-  depending upon the arguments. It then dumps the corresponding key files as:
-  <filename> and <filename>.pub (Private key and Public key respectively)
-  """
-  parser = create_parser()
-  args = parser.parse_args()
-
-  try:
-    if args.type == KEY_TYPE_RSA:
-      interface._generate_and_write_rsa_keypair( # pylint: disable=protected-access
-          filepath=args.name, bits=args.bits, prompt=args.prompt)
-    elif args.type == KEY_TYPE_ED25519:
-      interface._generate_and_write_ed25519_keypair( # pylint: disable=protected-access
-          filepath=args.name, prompt=args.prompt)
-    elif args.type == KEY_TYPE_ECDSA:
-      interface._generate_and_write_ecdsa_keypair( # pylint: disable=protected-access
-          filepath=args.name, prompt=args.prompt)
-    else:  # pragma: no cover
-      LOG.error(
-          "(in-toto-keygen) Unsupported keytype: {0}".format(str(args.type)))
-      sys.exit(1)
-    sys.exit(0)
-
-  except Exception as e:
-    LOG.error("(in-toto-keygen) {0}: {1}".format(type(e).__name__, e))
-    sys.exit(1)
+    """
+    First calls parse_args to parse the arguments, and then calls either
+    _generate_and_write_rsa_keypair or _generate_and_write_ed25519_keypair
+    depending upon the arguments. It then dumps the corresponding key files as:
+    <filename> and <filename>.pub (Private key and Public key respectively)
+    """
+    parser = create_parser()
+    args = parser.parse_args()
+
+    if args.type != KEY_TYPE_RSA:
+        if args.bits is not None:
+            parser.print_help()
+            parser.error(
+                "wrong arguments: bits specified,"
+                " only Type RSA supports Bits as a parameter"
+            )
+
+    try:
+        if args.type == KEY_TYPE_RSA:
+            interface._generate_and_write_rsa_keypair(  # pylint: disable=protected-access
+                filepath=args.name, bits=args.bits, prompt=args.prompt
+            )
+        elif args.type == KEY_TYPE_ED25519:
+            interface._generate_and_write_ed25519_keypair(  # pylint: disable=protected-access
+                filepath=args.name, prompt=args.prompt
+            )
+        elif args.type == KEY_TYPE_ECDSA:
+            interface._generate_and_write_ecdsa_keypair(  # pylint: disable=protected-access
+                filepath=args.name, prompt=args.prompt
+            )
+        else:  # pragma: no cover
+            LOG.error(
+                "(in-toto-keygen) Unsupported keytype: {0}".format(
+                    str(args.type)
+                )
+            )
+            sys.exit(1)
+        sys.exit(0)
+
+    except Exception as e:
+        LOG.error("(in-toto-keygen) {0}: {1}".format(type(e).__name__, e))
+        sys.exit(1)
+
 
 if __name__ == "__main__":
-  main()
+    main()
```

### Comparing `in_toto-1.4.0/in_toto/in_toto_record.py` & `in_toto-2.0.0/in_toto/in_toto_record.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,49 +22,70 @@
 
 <Return Codes>
   2 if an exception occurred during argument parsing
   1 if an exception occurred
   0 if no exception occurred
 
 """
-import sys
 import argparse
 import logging
-import in_toto.user_settings
-import in_toto.runlib
-from in_toto import __version__
-
-from in_toto.common_args import (EXCLUDE_ARGS, EXCLUDE_KWARGS, BASE_PATH_ARGS,
-    BASE_PATH_KWARGS, LSTRIP_PATHS_ARGS, LSTRIP_PATHS_KWARGS, KEY_ARGS,
-    KEY_KWARGS, KEY_TYPE_KWARGS, KEY_TYPE_ARGS, GPG_ARGS, GPG_KWARGS,
-    GPG_HOME_ARGS, GPG_HOME_KWARGS, VERBOSE_ARGS, VERBOSE_KWARGS, QUIET_ARGS,
-    QUIET_KWARGS, METADATA_DIRECTORY_ARGS, METADATA_DIRECTORY_KWARGS,
-    KEY_PASSWORD_ARGS, KEY_PASSWORD_KWARGS, parse_password_and_prompt_args,
-    sort_action_groups, title_case_action_groups, OPTS_TITLE, DSSE_ARGS,
-    DSSE_KWARGS)
+import sys
 
 from securesystemslib import interface
 
+import in_toto.runlib
+from in_toto import __version__
+from in_toto.common_args import (
+    BASE_PATH_ARGS,
+    BASE_PATH_KWARGS,
+    DSSE_ARGS,
+    DSSE_KWARGS,
+    EXCLUDE_ARGS,
+    EXCLUDE_KWARGS,
+    GPG_ARGS,
+    GPG_HOME_ARGS,
+    GPG_HOME_KWARGS,
+    GPG_KWARGS,
+    KEY_ARGS,
+    KEY_KWARGS,
+    KEY_PASSWORD_ARGS,
+    KEY_PASSWORD_KWARGS,
+    KEY_TYPE_ARGS,
+    KEY_TYPE_KWARGS,
+    LSTRIP_PATHS_ARGS,
+    LSTRIP_PATHS_KWARGS,
+    METADATA_DIRECTORY_ARGS,
+    METADATA_DIRECTORY_KWARGS,
+    OPTS_TITLE,
+    QUIET_ARGS,
+    QUIET_KWARGS,
+    VERBOSE_ARGS,
+    VERBOSE_KWARGS,
+    parse_password_and_prompt_args,
+    sort_action_groups,
+    title_case_action_groups,
+)
 
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
 
 def create_parser():
-  """Create and return configured ArgumentParser instance. """
+    """Create and return configured ArgumentParser instance."""
 
-  parser = argparse.ArgumentParser(
-      formatter_class=argparse.RawDescriptionHelpFormatter,
-      description="""
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description="""
 in-toto-record creates a signed link metadata file in two steps, in order to
 provide evidence for supply chain steps that cannot be carried out by a single
 command (for which 'in-toto-run' should be used). It returns a non-zero value
-on failure and zero otherwise.""")
+on failure and zero otherwise.""",
+    )
 
-  parser.epilog = """EXAMPLE USAGE
+    parser.epilog = """EXAMPLE USAGE
 
 Create link metadata file in two commands, signing it with the private key
 loaded from 'key_file', recording all files in the CWD as materials (on
 start), and as products (on stop).
 
   {prog} start -n edit-files -k path/to/key_file -m .
   {prog} stop -n edit-files -k path/to/key_file -p .
@@ -80,146 +101,204 @@
 Create link metadata file signed with the private key loaded from 'key_file',
 record all files in the CWD as material and product, and dump finished link
 file to the target directory (on stop).
 
   {prog} start -n edit-files -k path/to/key_file -m .
   {prog} stop -d path/to/target/dir -n edit-files -k path/to/key_file -p .
 
-""".format(prog=parser.prog)
+""".format(
+        prog=parser.prog
+    )
+
+    # The subparsers inherit the arguments from the parent parser
+    parent_parser = argparse.ArgumentParser(add_help=False)
+    subparsers = parser.add_subparsers(dest="command")
+
+    # Workaround to make subcommands mandatory in Python>=3.3
+    # https://bugs.python.org/issue9253#msg186387
+    subparsers.required = True
+
+    parent_named_args = parent_parser.add_argument_group(
+        "required named arguments"
+    )
+
+    # FIXME: Do we limit the allowed characters for the name?
+    parent_named_args.add_argument(
+        "-n",
+        "--step-name",
+        type=str,
+        required=True,
+        metavar="<name>",
+        help=(
+            "name for the resulting link metadata file. It is also used to associate"
+            " the link with a step defined in an in-toto layout."
+        ),
+    )
+
+    parent_named_args.add_argument(*KEY_ARGS, **KEY_KWARGS)
+    parent_parser.add_argument(*KEY_TYPE_ARGS, **KEY_TYPE_KWARGS)
+    parent_parser.add_argument(*KEY_PASSWORD_ARGS, **KEY_PASSWORD_KWARGS)
+
+    parent_named_args.add_argument(*GPG_ARGS, **GPG_KWARGS)
+    parent_parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
+
+    parent_parser.add_argument(*EXCLUDE_ARGS, **EXCLUDE_KWARGS)
+    parent_parser.add_argument(*BASE_PATH_ARGS, **BASE_PATH_KWARGS)
+    parent_parser.add_argument(*LSTRIP_PATHS_ARGS, **LSTRIP_PATHS_KWARGS)
+    parent_parser.add_argument(*DSSE_ARGS, **DSSE_KWARGS)
+
+    verbosity_args = parent_parser.add_mutually_exclusive_group(required=False)
+    verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
+    verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
+
+    subparser_start = subparsers.add_parser(
+        "start",
+        parents=[parent_parser],
+        help=(
+            "creates a preliminary link file recording the paths and hashes of"
+            " the passed materials and signs it with the passed functionary's"
+            " key. The resulting link file is stored as"
+            " '.<name>.<keyid prefix>.link-unfinished'."
+        ),
+    )
+
+    subparser_stop = subparsers.add_parser(
+        "stop",
+        parents=[parent_parser],
+        help=(
+            "expects preliminary link file '.<name>.<keyid prefix>.link-unfinished'"
+            " in the CWD, signed by the passed functionary's key. If found, it"
+            " records and adds the paths and hashes of the passed products to the"
+            " link metadata file, updates the signature and renames the file to"
+            " '<name>.<keyid prefix>.link'."
+        ),
+    )
+
+    subparser_start.add_argument(
+        "-m",
+        "--materials",
+        type=str,
+        required=False,
+        nargs="+",
+        metavar="<path>",
+        help=(
+            "paths to files or directories, whose paths and hashes are stored in the"
+            " resulting link metadata's material section when running the 'start'"
+            " subcommand. Symlinks to files are followed."
+        ),
+    )
+
+    subparser_stop.add_argument(
+        "-p",
+        "--products",
+        type=str,
+        required=False,
+        nargs="+",
+        metavar="<path>",
+        help=(
+            "paths to files or directories, whose paths and hashes are stored in the"
+            " resulting link metadata's product section when running the 'stop'"
+            " subcommand. Symlinks to files are followed."
+        ),
+    )
+
+    subparser_stop.add_argument(
+        *METADATA_DIRECTORY_ARGS, **METADATA_DIRECTORY_KWARGS
+    )
+
+    parser.add_argument(
+        "--version",
+        action="version",
+        version="{} {}".format(parser.prog, __version__),
+    )
+
+    for _parser, _order in [
+        (parser, ["Positional Arguments", OPTS_TITLE]),
+        (subparser_start, None),
+        (subparser_stop, None),
+    ]:
+        title_case_action_groups(_parser)
+        sort_action_groups(_parser, _order)
 
-  # The subparsers inherit the arguments from the parent parser
-  parent_parser = argparse.ArgumentParser(add_help=False)
-  subparsers = parser.add_subparsers(dest="command")
-
-  # Workaround to make subcommands mandatory in Python>=3.3
-  # https://bugs.python.org/issue9253#msg186387
-  subparsers.required = True
-
-  parent_named_args = parent_parser.add_argument_group(
-      "required named arguments")
-
-  # FIXME: Do we limit the allowed characters for the name?
-  parent_named_args.add_argument("-n", "--step-name", type=str, required=True,
-      metavar="<name>", help=(
-      "name for the resulting link metadata file. It is also used to associate"
-      " the link with a step defined in an in-toto layout."))
-
-  parent_named_args.add_argument(*KEY_ARGS, **KEY_KWARGS)
-  parent_parser.add_argument(*KEY_TYPE_ARGS, **KEY_TYPE_KWARGS)
-  parent_parser.add_argument(*KEY_PASSWORD_ARGS, **KEY_PASSWORD_KWARGS)
-
-  parent_named_args.add_argument(*GPG_ARGS, **GPG_KWARGS)
-  parent_parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
-
-  parent_parser.add_argument(*EXCLUDE_ARGS, **EXCLUDE_KWARGS)
-  parent_parser.add_argument(*BASE_PATH_ARGS, **BASE_PATH_KWARGS)
-  parent_parser.add_argument(*LSTRIP_PATHS_ARGS, **LSTRIP_PATHS_KWARGS)
-  parent_parser.add_argument(*DSSE_ARGS, **DSSE_KWARGS)
-
-  verbosity_args = parent_parser.add_mutually_exclusive_group(required=False)
-  verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
-  verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
-
-  subparser_start = subparsers.add_parser("start", parents=[parent_parser],
-      help=(
-      "creates a preliminary link file recording the paths and hashes of"
-      " the passed materials and signs it with the passed functionary's"
-      " key. The resulting link file is stored as"
-      " '.<name>.<keyid prefix>.link-unfinished'."))
-
-  subparser_stop = subparsers.add_parser("stop", parents=[parent_parser],
-      help=(
-      "expects preliminary link file '.<name>.<keyid prefix>.link-unfinished'"
-      " in the CWD, signed by the passed functionary's key. If found, it"
-      " records and adds the paths and hashes of the passed products to the"
-      " link metadata file, updates the signature and renames the file to"
-      " '<name>.<keyid prefix>.link'."))
-
-  subparser_start.add_argument("-m", "--materials", type=str, required=False,
-      nargs='+', metavar="<path>", help=(
-      "paths to files or directories, whose paths and hashes are stored in the"
-      " resulting link metadata's material section when running the 'start'"
-      " subcommand. Symlinks to files are followed."))
-
-  subparser_stop.add_argument("-p", "--products", type=str, required=False,
-      nargs='+', metavar="<path>", help=(
-      "paths to files or directories, whose paths and hashes are stored in the"
-      " resulting link metadata's product section when running the 'stop'"
-      " subcommand. Symlinks to files are followed."))
-
-  subparser_stop.add_argument(*METADATA_DIRECTORY_ARGS,
-      **METADATA_DIRECTORY_KWARGS)
-
-  parser.add_argument('--version', action='version',
-                      version='{} {}'.format(parser.prog, __version__))
-
-  for _parser, _order in [
-    (parser, ["Positional Arguments", OPTS_TITLE]),
-    (subparser_start, None), (subparser_stop, None)]:
-    title_case_action_groups(_parser)
-    sort_action_groups(_parser, _order)
-
-  return parser
+    return parser
 
 
 def main():
-  """Parse arguments, load key from disk (if passed) and call
-  either runlib.in_toto_record_start or runlib.in_toto_record_stop depending
-  on the specified subcommand. """
-
-  parser = create_parser()
-  args = parser.parse_args()
-
-  LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
-
-  # Override defaults in settings.py with environment variables and RCfiles
-  in_toto.user_settings.set_settings()
-
-  # Regular signing and GPG signing are mutually exclusive
-  if (args.key is None) == (args.gpg is None):
-    parser.print_usage()
-    parser.error("Specify either '--key <key path>' or '--gpg [<keyid>]'")
-
-  password, prompt = parse_password_and_prompt_args(args)
-
-  # If `--gpg` was set without argument it has the value `True` and
-  # we will try to sign with the default key
-  gpg_use_default = args.gpg is True
-
-  # Otherwise gpg_keyid stays either None or gets the passed argument assigned
-  gpg_keyid = None
-  if not gpg_use_default and args.gpg:
-    gpg_keyid = args.gpg
-
-  try:
-    # We load the key here because it might prompt the user for a password in
-    # case the key is encrypted. Something that should not happen in the lib.
-    key = None
-    if args.key:
-      key = interface.import_privatekey_from_file(
-          args.key, key_type=args.key_type, password=password, prompt=prompt)
-
-    if args.command == "start":
-      in_toto.runlib.in_toto_record_start(args.step_name, args.materials,
-          signing_key=key, gpg_keyid=gpg_keyid,
-          gpg_use_default=gpg_use_default, gpg_home=args.gpg_home,
-          exclude_patterns=args.exclude_patterns, base_path=args.base_path,
-          lstrip_paths=args.lstrip_paths, use_dsse=args.use_dsse)
-
-    # Mutually exclusiveness is guaranteed by argparser
-    else: # args.command == "stop":
-      in_toto.runlib.in_toto_record_stop(args.step_name, args.products,
-          signing_key=key, gpg_keyid=gpg_keyid,
-          gpg_use_default=gpg_use_default, gpg_home=args.gpg_home,
-          exclude_patterns=args.exclude_patterns, base_path=args.base_path,
-          lstrip_paths=args.lstrip_paths,
-          metadata_directory=args.metadata_directory)
-
-  except Exception as e:
-    LOG.error("(in-toto-record {0}) {1}: {2}"
-        .format(args.command, type(e).__name__, e))
-    sys.exit(1)
+    """Parse arguments, load key from disk (if passed) and call
+    either runlib.in_toto_record_start or runlib.in_toto_record_stop depending
+    on the specified subcommand."""
+
+    parser = create_parser()
+    args = parser.parse_args()
+
+    LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
+
+    # Regular signing and GPG signing are mutually exclusive
+    if (args.key is None) == (args.gpg is None):
+        parser.print_usage()
+        parser.error("Specify either '--key <key path>' or '--gpg [<keyid>]'")
+
+    password, prompt = parse_password_and_prompt_args(args)
+
+    # If `--gpg` was set without argument it has the value `True` and
+    # we will try to sign with the default key
+    gpg_use_default = args.gpg is True
+
+    # Otherwise gpg_keyid stays either None or gets the passed argument assigned
+    gpg_keyid = None
+    if not gpg_use_default and args.gpg:
+        gpg_keyid = args.gpg
+
+    try:
+        # We load the key here because it might prompt the user for a password in
+        # case the key is encrypted. Something that should not happen in the lib.
+        key = None
+        if args.key:
+            key = interface.import_privatekey_from_file(
+                args.key,
+                key_type=args.key_type,
+                password=password,
+                prompt=prompt,
+            )
+
+        if args.command == "start":
+            in_toto.runlib.in_toto_record_start(
+                args.step_name,
+                args.materials,
+                signing_key=key,
+                gpg_keyid=gpg_keyid,
+                gpg_use_default=gpg_use_default,
+                gpg_home=args.gpg_home,
+                exclude_patterns=args.exclude_patterns,
+                base_path=args.base_path,
+                lstrip_paths=args.lstrip_paths,
+                use_dsse=args.use_dsse,
+            )
+
+        # Mutually exclusiveness is guaranteed by argparser
+        else:  # args.command == "stop":
+            in_toto.runlib.in_toto_record_stop(
+                args.step_name,
+                args.products,
+                signing_key=key,
+                gpg_keyid=gpg_keyid,
+                gpg_use_default=gpg_use_default,
+                gpg_home=args.gpg_home,
+                exclude_patterns=args.exclude_patterns,
+                base_path=args.base_path,
+                lstrip_paths=args.lstrip_paths,
+                metadata_directory=args.metadata_directory,
+            )
+
+    except Exception as e:
+        LOG.error(
+            "(in-toto-record {0}) {1}: {2}".format(
+                args.command, type(e).__name__, e
+            )
+        )
+        sys.exit(1)
+
+    sys.exit(0)
 
-  sys.exit(0)
 
 if __name__ == "__main__":
-  main()
+    main()
```

### Comparing `in_toto-1.4.0/in_toto/in_toto_run.py` & `in_toto-2.0.0/in_toto/in_toto_run.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,54 +22,78 @@
 <Return Codes>
   2 if an exception occurred during argument parsing
   1 if an exception occurred
   0 if no exception occurred
 
 """
 
-import sys
 import argparse
 import logging
-import in_toto.user_settings
-from in_toto import (runlib, __version__)
-
-from in_toto.common_args import (EXCLUDE_ARGS, EXCLUDE_KWARGS, BASE_PATH_ARGS,
-    BASE_PATH_KWARGS, LSTRIP_PATHS_ARGS, LSTRIP_PATHS_KWARGS, KEY_ARGS,
-    KEY_KWARGS, KEY_TYPE_KWARGS, KEY_TYPE_ARGS, GPG_ARGS, GPG_KWARGS,
-    GPG_HOME_ARGS, GPG_HOME_KWARGS, VERBOSE_ARGS, VERBOSE_KWARGS, QUIET_ARGS,
-    QUIET_KWARGS, METADATA_DIRECTORY_ARGS, METADATA_DIRECTORY_KWARGS,
-    KEY_PASSWORD_ARGS, KEY_PASSWORD_KWARGS, parse_password_and_prompt_args,
-    sort_action_groups, title_case_action_groups, OPTS_TITLE, DSSE_ARGS,
-    DSSE_KWARGS,)
+import sys
 
 from securesystemslib import interface
 
+from in_toto import __version__, runlib
+from in_toto.common_args import (
+    BASE_PATH_ARGS,
+    BASE_PATH_KWARGS,
+    DSSE_ARGS,
+    DSSE_KWARGS,
+    EXCLUDE_ARGS,
+    EXCLUDE_KWARGS,
+    GPG_ARGS,
+    GPG_HOME_ARGS,
+    GPG_HOME_KWARGS,
+    GPG_KWARGS,
+    KEY_ARGS,
+    KEY_KWARGS,
+    KEY_PASSWORD_ARGS,
+    KEY_PASSWORD_KWARGS,
+    KEY_TYPE_ARGS,
+    KEY_TYPE_KWARGS,
+    LSTRIP_PATHS_ARGS,
+    LSTRIP_PATHS_KWARGS,
+    METADATA_DIRECTORY_ARGS,
+    METADATA_DIRECTORY_KWARGS,
+    OPTS_TITLE,
+    QUIET_ARGS,
+    QUIET_KWARGS,
+    VERBOSE_ARGS,
+    VERBOSE_KWARGS,
+    parse_password_and_prompt_args,
+    sort_action_groups,
+    title_case_action_groups,
+)
+
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
 
 def create_parser():
-  """Create and return configured ArgumentParser instance. """
-  parser = argparse.ArgumentParser(
-      formatter_class=argparse.RawDescriptionHelpFormatter,
-      description="""
+    """Create and return configured ArgumentParser instance."""
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description="""
 in-toto-run is the main command line interface for generating link
 metadata while carrying out a supply chain step. To do this, it wraps the
 passed command, and attempts to track all relevant information about the
 wrapped command's execution. It records paths and hashes of 'materials' (files
 before command execution) and 'products' (files after command execution) and
 writes them together with other information (executed command, return value,
 stdout and stderr) to a link metadata file, which is signed with the passed
-key. It returns a non-zero value on failure and zero otherwise.""")
+key. It returns a non-zero value on failure and zero otherwise.""",
+    )
 
-  parser.usage = (
-    "%(prog)s <named arguments> [{}] \\\n\t -- <command> [args]".format(
-      OPTS_TITLE.lower()))
+    parser.usage = (
+        "%(prog)s <named arguments> [{}] \\\n\t -- <command> [args]".format(
+            OPTS_TITLE.lower()
+        )
+    )
 
-  parser.epilog = """EXAMPLE USAGE
+    parser.epilog = """EXAMPLE USAGE
 
 Tag a git repo, storing files in CWD as products, signing the resulting link
 file with the private key loaded from 'key_file'.
 
   {prog} -n tag -p . -k key_file -- git tag v1.0
 
 
@@ -103,137 +127,194 @@
 e.g. 'document.pdf'.
 
   {prog} -n review -k key_file \\
          -m /tmp/my/review/docs/document.pdf \\
          --lstrip-paths /tmp/my/review/docs/ -x
 
 
-""".format(prog=parser.prog)
-
-
-  named_args = parser.add_argument_group("required named arguments")
-
-  # FIXME: Do we limit the allowed characters for the name?
-  named_args.add_argument("-n", "--step-name", type=str, required=True,
-      metavar="<name>", help=(
-      "name for the resulting link metadata file, which is written to"
-      " '<name>.<keyid prefix>.link'. It is also used to associate the link"
-      " with a step defined in an in-toto layout."))
-
-  parser.add_argument("-m", "--materials", type=str, required=False,
-      nargs='+', metavar="<path>", help=(
-      "paths to files or directories, for which paths and hashes are stored in"
-      " the resulting link metadata before the command is executed. Symlinks"
-      " to files are followed."))
-
-  parser.add_argument("-p", "--products", type=str, required=False,
-      nargs='+', metavar="<path>", help=(
-      "paths to files or directories, for which paths and hashes are stored in"
-      " the resulting link metadata after the command is executed. Symlinks to"
-      " files are followed."))
-
-  parser.add_argument("-s", "--record-streams", dest="record_streams",
-      default=False, action="store_true", help=(
-      "duplicate 'stdout' and 'stderr' of the executed command and store the"
-      " contents in the resulting link metadata. Do not use with interactive"
-      " commands."))
-
-  parser.add_argument("-x", "--no-command", dest="no_command", default=False,
-    action="store_true", help=(
-    "generate link metadata without executing a command, e.g. for a"
-    " signed-off-by step."))
-
-  named_args.add_argument(*KEY_ARGS, **KEY_KWARGS)
-  parser.add_argument(*KEY_TYPE_ARGS, **KEY_TYPE_KWARGS)
-  parser.add_argument(*KEY_PASSWORD_ARGS, **KEY_PASSWORD_KWARGS)
-
-  named_args.add_argument(*GPG_ARGS, **GPG_KWARGS)
-  parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
-
-  parser.add_argument(*EXCLUDE_ARGS, **EXCLUDE_KWARGS)
-  parser.add_argument(*BASE_PATH_ARGS, **BASE_PATH_KWARGS)
-  parser.add_argument(*LSTRIP_PATHS_ARGS, **LSTRIP_PATHS_KWARGS)
-  parser.add_argument(*METADATA_DIRECTORY_ARGS, **METADATA_DIRECTORY_KWARGS)
-  parser.add_argument(*DSSE_ARGS, **DSSE_KWARGS)
-
-  verbosity_args = parser.add_mutually_exclusive_group(required=False)
-  verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
-  verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
-
-
-  # FIXME: This is not yet ideal.
-  # What should we do with tokens like > or ; ?
-  parser.add_argument("link_cmd", nargs="*", metavar="<command>",
-      help=(
-      "command to be executed. It is separated from named and optional"
-      " arguments by a double dash '--'."))
-
-  parser.add_argument('--version', action='version',
-                      version='{} {}'.format(parser.prog, __version__))
+""".format(
+        prog=parser.prog
+    )
+
+    named_args = parser.add_argument_group("required named arguments")
+
+    # FIXME: Do we limit the allowed characters for the name?
+    named_args.add_argument(
+        "-n",
+        "--step-name",
+        type=str,
+        required=True,
+        metavar="<name>",
+        help=(
+            "name for the resulting link metadata file, which is written to"
+            " '<name>.<keyid prefix>.link'. It is also used to associate the link"
+            " with a step defined in an in-toto layout."
+        ),
+    )
+
+    parser.add_argument(
+        "-m",
+        "--materials",
+        type=str,
+        required=False,
+        nargs="+",
+        metavar="<path>",
+        help=(
+            "paths to files or directories, for which paths and hashes are stored in"
+            " the resulting link metadata before the command is executed. Symlinks"
+            " to files are followed."
+        ),
+    )
+
+    parser.add_argument(
+        "-p",
+        "--products",
+        type=str,
+        required=False,
+        nargs="+",
+        metavar="<path>",
+        help=(
+            "paths to files or directories, for which paths and hashes are stored in"
+            " the resulting link metadata after the command is executed. Symlinks to"
+            " files are followed."
+        ),
+    )
+
+    parser.add_argument(
+        "-s",
+        "--record-streams",
+        dest="record_streams",
+        default=False,
+        action="store_true",
+        help=(
+            "duplicate 'stdout' and 'stderr' of the executed command and store the"
+            " contents in the resulting link metadata. Do not use with interactive"
+            " commands."
+        ),
+    )
+
+    parser.add_argument(
+        "-x",
+        "--no-command",
+        dest="no_command",
+        default=False,
+        action="store_true",
+        help=(
+            "generate link metadata without executing a command, e.g. for a"
+            " signed-off-by step."
+        ),
+    )
+
+    named_args.add_argument(*KEY_ARGS, **KEY_KWARGS)
+    parser.add_argument(*KEY_TYPE_ARGS, **KEY_TYPE_KWARGS)
+    parser.add_argument(*KEY_PASSWORD_ARGS, **KEY_PASSWORD_KWARGS)
+
+    named_args.add_argument(*GPG_ARGS, **GPG_KWARGS)
+    parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
+
+    parser.add_argument(*EXCLUDE_ARGS, **EXCLUDE_KWARGS)
+    parser.add_argument(*BASE_PATH_ARGS, **BASE_PATH_KWARGS)
+    parser.add_argument(*LSTRIP_PATHS_ARGS, **LSTRIP_PATHS_KWARGS)
+    parser.add_argument(*METADATA_DIRECTORY_ARGS, **METADATA_DIRECTORY_KWARGS)
+    parser.add_argument(*DSSE_ARGS, **DSSE_KWARGS)
+
+    verbosity_args = parser.add_mutually_exclusive_group(required=False)
+    verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
+    verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
+
+    # FIXME: This is not yet ideal.
+    # What should we do with tokens like > or ; ?
+    parser.add_argument(
+        "link_cmd",
+        nargs="*",
+        metavar="<command>",
+        help=(
+            "command to be executed. It is separated from named and optional"
+            " arguments by a double dash '--'."
+        ),
+    )
+
+    parser.add_argument(
+        "--version",
+        action="version",
+        version="{} {}".format(parser.prog, __version__),
+    )
 
-  title_case_action_groups(parser)
-  sort_action_groups(parser)
+    title_case_action_groups(parser)
+    sort_action_groups(parser)
 
-  return parser
+    return parser
 
 
 def main():
-  """Parse arguments, load key from disk (prompts for password if key is
-  encrypted) and call in_toto_run.  """
-  parser = create_parser()
-  args = parser.parse_args()
-
-  LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
-
-  # Override defaults in settings.py with environment variables and RCfiles
-  in_toto.user_settings.set_settings()
-
-  # Regular signing and GPG signing are mutually exclusive
-  if (args.key is None) == (args.gpg is None):
-    parser.print_usage()
-    parser.error("Specify either '--key <key path>' or '--gpg [<keyid>]'")
-
-  password, prompt = parse_password_and_prompt_args(args)
-
-  # If `--gpg` was set without argument it has the value `True` and
-  # we will try to sign with the default key
-  gpg_use_default = args.gpg is True
-
-  # Otherwise we interpret it as actual keyid
-  gpg_keyid = None
-  if args.gpg is not True:
-    gpg_keyid = args.gpg
-
-  # If no_command is specified run in_toto_run without executing a command
-  if args.no_command:
-    args.link_cmd = []
-
-  elif not args.link_cmd: # pragma: no branch
-    parser.print_usage()
-    parser.error("No command specified."
-        " Please specify (or use the --no-command option)")
-
-  try:
-    # We load the key here because it might prompt the user for a password in
-    # case the key is encrypted. Something that should not happen in the lib.
-    key = None
-    if args.key:
-      key = interface.import_privatekey_from_file(
-          args.key, key_type=args.key_type, password=password, prompt=prompt)
-
-    runlib.in_toto_run(
-        args.step_name, args.materials, args.products, args.link_cmd,
-        record_streams=args.record_streams, signing_key=key,
-        gpg_keyid=gpg_keyid, gpg_use_default=gpg_use_default,
-        gpg_home=args.gpg_home, exclude_patterns=args.exclude_patterns,
-        base_path=args.base_path, lstrip_paths=args.lstrip_paths,
-        metadata_directory=args.metadata_directory, use_dsse=args.use_dsse)
-
-  except Exception as e:
-    LOG.error("(in-toto-run) {0}: {1}".format(type(e).__name__, e))
-    sys.exit(1)
+    """Parse arguments, load key from disk (prompts for password if key is
+    encrypted) and call in_toto_run."""
+    parser = create_parser()
+    args = parser.parse_args()
+
+    LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
+
+    # Regular signing and GPG signing are mutually exclusive
+    if (args.key is None) == (args.gpg is None):
+        parser.print_usage()
+        parser.error("Specify either '--key <key path>' or '--gpg [<keyid>]'")
+
+    password, prompt = parse_password_and_prompt_args(args)
+
+    # If `--gpg` was set without argument it has the value `True` and
+    # we will try to sign with the default key
+    gpg_use_default = args.gpg is True
+
+    # Otherwise we interpret it as actual keyid
+    gpg_keyid = None
+    if args.gpg is not True:
+        gpg_keyid = args.gpg
+
+    # If no_command is specified run in_toto_run without executing a command
+    if args.no_command:
+        args.link_cmd = []
+
+    elif not args.link_cmd:  # pragma: no branch
+        parser.print_usage()
+        parser.error(
+            "No command specified."
+            " Please specify (or use the --no-command option)"
+        )
+
+    try:
+        # We load the key here because it might prompt the user for a password in
+        # case the key is encrypted. Something that should not happen in the lib.
+        key = None
+        if args.key:
+            key = interface.import_privatekey_from_file(
+                args.key,
+                key_type=args.key_type,
+                password=password,
+                prompt=prompt,
+            )
+
+        runlib.in_toto_run(
+            args.step_name,
+            args.materials,
+            args.products,
+            args.link_cmd,
+            record_streams=args.record_streams,
+            signing_key=key,
+            gpg_keyid=gpg_keyid,
+            gpg_use_default=gpg_use_default,
+            gpg_home=args.gpg_home,
+            exclude_patterns=args.exclude_patterns,
+            base_path=args.base_path,
+            lstrip_paths=args.lstrip_paths,
+            metadata_directory=args.metadata_directory,
+            use_dsse=args.use_dsse,
+        )
+
+    except Exception as e:
+        LOG.error("(in-toto-run) {0}: {1}".format(type(e).__name__, e))
+        sys.exit(1)
 
-  sys.exit(0)
+    sys.exit(0)
 
 
 if __name__ == "__main__":
-  main()
+    main()
```

### Comparing `in_toto-1.4.0/in_toto/in_toto_sign.py` & `in_toto-2.0.0/in_toto/in_toto_sign.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,201 +18,219 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Provides command line interface to sign in-toto link or layout metadata
   or to verify its signatures.
 
 """
-import sys
 import argparse
 import logging
+import sys
 
-from in_toto import exceptions
-from in_toto.models.link import FILENAME_FORMAT
-from in_toto.models.metadata import Metadata
-from in_toto.models._signer import GPGSigner
-from in_toto.common_args import (GPG_HOME_ARGS, GPG_HOME_KWARGS, VERBOSE_ARGS,
-    VERBOSE_KWARGS, QUIET_ARGS, QUIET_KWARGS, title_case_action_groups,
-    sort_action_groups)
-from in_toto import (
-    __version__, SUPPORTED_KEY_TYPES, KEY_TYPE_RSA, KEY_TYPE_ED25519,
-    KEY_TYPE_ECDSA)
-
-import securesystemslib.formats
 import securesystemslib.exceptions
+import securesystemslib.formats
 from securesystemslib import interface
 from securesystemslib.gpg import functions as gpg_interface
 from securesystemslib.signer import SSlibSigner
 
+from in_toto import (
+    KEY_TYPE_ECDSA,
+    KEY_TYPE_ED25519,
+    KEY_TYPE_RSA,
+    SUPPORTED_KEY_TYPES,
+    __version__,
+    exceptions,
+)
+from in_toto.common_args import (
+    GPG_HOME_ARGS,
+    GPG_HOME_KWARGS,
+    QUIET_ARGS,
+    QUIET_KWARGS,
+    VERBOSE_ARGS,
+    VERBOSE_KWARGS,
+    sort_action_groups,
+    title_case_action_groups,
+)
+from in_toto.models._signer import GPGSigner
+from in_toto.models.link import FILENAME_FORMAT
+from in_toto.models.metadata import Metadata
 
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
 
 def _sign_and_dump_metadata(metadata, args):
-  """
-  <Purpose>
-    Internal method to sign link or layout metadata and dump it to disk.
-
-  <Arguments>
-    metadata:
-            Metadata object (contains Link or Layout object)
-    args:
-            see argparser
-
-  <Exceptions>
-    SystemExit(0) if signing is successful
-    SystemExit(2) if any exception occurs
-
-  """
-
-  try:
-    if not args.append:
-      metadata.signatures = []
-
-    signature = None
-    # If the cli tool was called with `--gpg [KEYID ...]` `args.gpg` is
-    # a list (not None) and we will try to sign with gpg.
-    # If `--gpg-home` was not set, args.gpg_home is None and the signer tries
-    # to use the default gpg keyring.
-    if args.gpg is not None:
-      # If `--gpg` was passed without argument we sign with the default key
-      # Excluded so that coverage does not vary in different test environments
-      if len(args.gpg) == 0: # pragma: no cover
-        signature = metadata.create_signature(
-          GPGSigner(None, homedir=args.gpg_home))
-
-      # Otherwise we sign with each passed keyid
-      for keyid in args.gpg:
-        securesystemslib.formats.KEYID_SCHEMA.check_match(keyid)
-        signature = metadata.create_signature(
-            GPGSigner(keyid, homedir=args.gpg_home))
-
-    # Alternatively we iterate over passed private key paths `--key KEYPATH
-    # ...` load the corresponding key from disk and sign with it
-    elif args.key is not None: # pragma: no branch
-
-      if args.key_type is None:
-        args.key_type = [KEY_TYPE_RSA] * len(args.key)
-
-      if len(args.key_type) != len(args.key):
-        raise securesystemslib.exceptions.FormatError(
-          "number of key_types should match with the number"
-          " of keys specified")
-
-      for idx, key_path in enumerate(args.key):
-        key = interface.import_privatekey_from_file(
-            key_path, key_type=args.key_type[idx], prompt=args.prompt)
-        signature = metadata.create_signature(SSlibSigner(key))
-
-    payload = metadata.get_payload()
-    _type = payload.type_
-
-    # If `--output` was specified we store the signed link or layout metadata
-    # to that location no matter what
-    if args.output:
-      out_path = args.output
-
-    # Otherwise, in case of links, we build the filename using the link/step
-    # name and the keyid of the created signature (there is only one for links)
-    elif _type == "link":
-      keyid = signature.keyid
-      out_path = FILENAME_FORMAT.format(step_name=payload.name, keyid=keyid)
-
-    # In case of layouts we just override the input file.
-    elif _type == "layout": # pragma: no branch
-      out_path = args.file
-
-    LOG.info("Dumping {0} to '{1}'...".format(_type, out_path))
-
-    metadata.dump(out_path)
-    sys.exit(0)
-
-  except Exception as e:
-    LOG.error("The following error occurred while signing: "
-        "{}".format(e))
-    sys.exit(2)
+    """
+    <Purpose>
+      Internal method to sign link or layout metadata and dump it to disk.
+
+    <Arguments>
+      metadata:
+              Metadata object (contains Link or Layout object)
+      args:
+              see argparser
+
+    <Exceptions>
+      SystemExit(0) if signing is successful
+      SystemExit(2) if any exception occurs
+
+    """
+
+    try:
+        if not args.append:
+            metadata.signatures = []
+
+        signature = None
+        # If the cli tool was called with `--gpg [KEYID ...]` `args.gpg` is
+        # a list (not None) and we will try to sign with gpg.
+        # If `--gpg-home` was not set, args.gpg_home is None and the signer tries
+        # to use the default gpg keyring.
+        if args.gpg is not None:
+            # If `--gpg` was passed without argument we sign with the default key
+            # Excluded so that coverage does not vary in different test environments
+            if len(args.gpg) == 0:  # pragma: no cover
+                signature = metadata.create_signature(
+                    GPGSigner(None, homedir=args.gpg_home)
+                )
+
+            # Otherwise we sign with each passed keyid
+            for keyid in args.gpg:
+                securesystemslib.formats.KEYID_SCHEMA.check_match(keyid)
+                signature = metadata.create_signature(
+                    GPGSigner(keyid, homedir=args.gpg_home)
+                )
+
+        # Alternatively we iterate over passed private key paths `--key KEYPATH
+        # ...` load the corresponding key from disk and sign with it
+        elif args.key is not None:  # pragma: no branch
+            if args.key_type is None:
+                args.key_type = [KEY_TYPE_RSA] * len(args.key)
+
+            if len(args.key_type) != len(args.key):
+                raise securesystemslib.exceptions.FormatError(
+                    "number of key_types should match with the number"
+                    " of keys specified"
+                )
+
+            for idx, key_path in enumerate(args.key):
+                key = interface.import_privatekey_from_file(
+                    key_path, key_type=args.key_type[idx], prompt=args.prompt
+                )
+                signature = metadata.create_signature(SSlibSigner(key))
+
+        payload = metadata.get_payload()
+        _type = payload.type_
+
+        # If `--output` was specified we store the signed link or layout metadata
+        # to that location no matter what
+        if args.output:
+            out_path = args.output
+
+        # Otherwise, in case of links, we build the filename using the link/step
+        # name and the keyid of the created signature (there is only one for links)
+        elif _type == "link":
+            keyid = signature.keyid
+            out_path = FILENAME_FORMAT.format(
+                step_name=payload.name, keyid=keyid
+            )
+
+        # In case of layouts we just override the input file.
+        elif _type == "layout":  # pragma: no branch
+            out_path = args.file
+
+        LOG.info("Dumping {0} to '{1}'...".format(_type, out_path))
+
+        metadata.dump(out_path)
+        sys.exit(0)
+
+    except Exception as e:
+        LOG.error("The following error occurred while signing: " "{}".format(e))
+        sys.exit(2)
 
 
 def _verify_metadata(metadata, args):
-  """
-  <Purpose>
-    Internal method to verify link or layout signatures.
-
-  <Arguments>
-    metadata:
-            Metadata object (contains Link or Layout object)
-    args:
-            see argparser
-
-  <Exceptions>
-    SystemExit(0) if verification passes
-    SystemExit(1) if verification fails
-    SystemExit(2) if any exception occurs
-
-  """
-  try:
-    # Load pubkeys from disk ....
-    if args.key is not None:
-      pub_key_dict = interface.import_publickeys_from_file(args.key,
-          args.key_type)
-
-    # ... or from gpg keyring
-    elif args.gpg is not None: # pragma: no branch
-      pub_key_dict = gpg_interface.export_pubkeys(
-          args.gpg, args.gpg_home)
-
-
-    for keyid, verification_key in pub_key_dict.items():
-      metadata.verify_signature(verification_key)
-      LOG.info("Signature verification passed for keyid '{}'"
-          .format(keyid))
-
-    sys.exit(0)
-
-  except exceptions.SignatureVerificationError as e:
-    LOG.error("Signature verification failed: {}".format(e))
-    sys.exit(1)
-
-  except Exception as e:
-    LOG.error("The following error occurred while verifying signatures: "
-        "{}".format(e))
-    sys.exit(2)
+    """
+    <Purpose>
+      Internal method to verify link or layout signatures.
+
+    <Arguments>
+      metadata:
+              Metadata object (contains Link or Layout object)
+      args:
+              see argparser
+
+    <Exceptions>
+      SystemExit(0) if verification passes
+      SystemExit(1) if verification fails
+      SystemExit(2) if any exception occurs
+
+    """
+    try:
+        # Load pubkeys from disk ....
+        if args.key is not None:
+            pub_key_dict = interface.import_publickeys_from_file(
+                args.key, args.key_type
+            )
+
+        # ... or from gpg keyring
+        elif args.gpg is not None:  # pragma: no branch
+            pub_key_dict = gpg_interface.export_pubkeys(args.gpg, args.gpg_home)
+
+        for keyid, verification_key in pub_key_dict.items():
+            metadata.verify_signature(verification_key)
+            LOG.info(
+                "Signature verification passed for keyid '{}'".format(keyid)
+            )
+
+        sys.exit(0)
+
+    except exceptions.SignatureVerificationError as e:
+        LOG.error("Signature verification failed: {}".format(e))
+        sys.exit(1)
+
+    except Exception as e:
+        LOG.error(
+            "The following error occurred while verifying signatures: "
+            "{}".format(e)
+        )
+        sys.exit(2)
 
 
 def _load_metadata(file_path):
-  """
-  <Purpose>
-    Loads Metadata (link or layout metadata) file from disk
-
-  <Arguments>
-    file_path:
-            path to link or layout metadata file
-
-  <Exceptions>
-    SystemExit(2) if any exception occurs
-
-  <Returns>
-    in-toto Metadata object (contains Link or Layout object)
-
-  """
-  try:
-    return Metadata.load(file_path)
-
-  except Exception as e:
-    LOG.error("The following error occurred while loading the file '{}': "
-        "{}".format(file_path, e))
-    sys.exit(2)
+    """
+    <Purpose>
+      Loads Metadata (link or layout metadata) file from disk
+
+    <Arguments>
+      file_path:
+              path to link or layout metadata file
+
+    <Exceptions>
+      SystemExit(2) if any exception occurs
+
+    <Returns>
+      in-toto Metadata object (contains Link or Layout object)
+
+    """
+    try:
+        return Metadata.load(file_path)
+
+    except Exception as e:
+        LOG.error(
+            "The following error occurred while loading the file '{}': "
+            "{}".format(file_path, e)
+        )
+        sys.exit(2)
 
 
 def create_parser():
-  """Create and return configured ArgumentParser instance. """
-  parser = argparse.ArgumentParser(
-      formatter_class=argparse.RawDescriptionHelpFormatter,
-      description="""
+    """Create and return configured ArgumentParser instance."""
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description="""
 in-toto-sign provides a command line interface to sign in-toto link or layout
 metadata or verify their signatures, with options to:
 
   * replace (default) or add signatures:
 
     + layout metadata can be signed by multiple keys at once,
     + link metadata can only be signed by one key at a time.
@@ -224,17 +242,18 @@
 
   * verify signatures
 
 in-toto-sign is useful to re-sign metadata (e.g. when changing keys), or to
 sign unsigned links (e.g. generated with 'in-toto-mock'). For layouts, it is
 useful to append signatures in case threshold signing of layouts is necessary.
 
-It returns a non-zero value on failure and zero otherwise.""")
+It returns a non-zero value on failure and zero otherwise.""",
+    )
 
-  parser.epilog = """EXAMPLE USAGE
+    parser.epilog = """EXAMPLE USAGE
 
 Sign 'unsigned.layout' with two keys and write it to 'root.layout'.
 
   {prog} -f unsigned.layout -k priv_key1 priv_key2 -o root.layout
 
 
 Replace signature in link file and write to default filename, i.e.
@@ -254,134 +273,196 @@
 
 
 Verify layout with a gpg key identified by keyid '...439F3C2'.
 
   {prog} -f root.layout --verify \\
       --gpg 3BF8135765A07E21BD12BF89A5627F6BF439F3C2
 
-""".format(prog=parser.prog)
-
+""".format(
+        prog=parser.prog
+    )
+
+    named_args = parser.add_argument_group("required named arguments")
+
+    named_args.add_argument(
+        "-f",
+        "--file",
+        type=str,
+        required=True,
+        metavar="<path>",
+        help=("path to link or layout file to be signed or verified."),
+    )
+
+    parser.add_argument(
+        "-k",
+        "--key",
+        nargs="+",
+        metavar="<path>",
+        help=(
+            "paths to key files, used to sign the passed link or layout metadata"
+            " or to verify its signatures. See '--key-type' for available formats."
+        ),
+    )
+
+    parser.add_argument(
+        "-t",
+        "--key-type",
+        dest="key_type",
+        type=str,
+        choices=SUPPORTED_KEY_TYPES,
+        nargs="+",
+        help=(
+            "types of keys specified by the '--key' option. '{rsa}' keys are"
+            " expected in a 'PEM' format. '{ed25519}' and '{ecdsa} are expected in a"
+            " custom 'securesystemslib/json' format. If multiple keys are passed via"
+            " '--key' the same amount of key types must be passed. Key"
+            " types are then associated with keys by index. If '--key-type' is"
+            " omitted, the default of '{rsa}' is used for all keys.".format(
+                rsa=KEY_TYPE_RSA, ed25519=KEY_TYPE_ED25519, ecdsa=KEY_TYPE_ECDSA
+            )
+        ),
+    )
+
+    parser.add_argument(
+        "-p",
+        "--prompt",
+        action="store_true",
+        help="prompt for signing key decryption password",
+    )
+
+    parser.add_argument(
+        "-g",
+        "--gpg",
+        nargs="*",
+        metavar="<id>",
+        help=(
+            "GPG keyids used to sign the passed link or layout metadata or to verify"
+            " its signatures. If passed without keyids, the default GPG key is"
+            " used."
+        ),
+    )
+
+    parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
+
+    # Only when signing
+    parser.add_argument(
+        "-o",
+        "--output",
+        type=str,
+        metavar="<path>",
+        help=(
+            "path to location where the metadata file is stored after signing. If"
+            " not passed, layout metadata is written to the path of the input file"
+            " and link metadata is written to '<name>.<keyid prefix>.link'"
+        ),
+    )
+
+    # Only when signing
+    parser.add_argument(
+        "-a",
+        "--append",
+        action="store_true",
+        help=(
+            "add signatures rather than replacing existing signatures. This option"
+            " is only availabe for layout metdata."
+        ),
+    )
+
+    parser.add_argument(
+        "--verify",
+        action="store_true",
+        help="verify signatures of passed link or layout metadata using the"
+        " public keys passed via '--key' and/or '--gpg' options.",
+    )
+
+    verbosity_args = parser.add_mutually_exclusive_group(required=False)
+    verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
+    verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
+
+    parser.add_argument(
+        "--version",
+        action="version",
+        version="{} {}".format(parser.prog, __version__),
+    )
 
-  named_args = parser.add_argument_group("required named arguments")
+    title_case_action_groups(parser)
+    sort_action_groups(parser)
 
-  named_args.add_argument("-f", "--file", type=str, required=True,
-      metavar="<path>", help=(
-        "path to link or layout file to be signed or verified."))
-
-  parser.add_argument("-k", "--key", nargs="+", metavar="<path>", help=(
-      "paths to key files, used to sign the passed link or layout metadata"
-      " or to verify its signatures. See '--key-type' for available formats."))
-
-  parser.add_argument("-t", "--key-type", dest="key_type",
-      type=str, choices=SUPPORTED_KEY_TYPES,
-      nargs="+", help=(
-      "types of keys specified by the '--key' option. '{rsa}' keys are"
-      " expected in a 'PEM' format. '{ed25519}' and '{ecdsa} are expected in a"
-      " custom 'securesystemslib/json' format. If multiple keys are passed via"
-      " '--key' the same amount of key types must be passed. Key"
-      " types are then associated with keys by index. If '--key-type' is"
-      " omitted, the default of '{rsa}' is used for all keys.".format(
-      rsa=KEY_TYPE_RSA, ed25519=KEY_TYPE_ED25519, ecdsa=KEY_TYPE_ECDSA)))
-
-  parser.add_argument("-p", "--prompt", action="store_true",
-      help="prompt for signing key decryption password")
-
-  parser.add_argument("-g", "--gpg", nargs="*", metavar="<id>", help=(
-      "GPG keyids used to sign the passed link or layout metadata or to verify"
-      " its signatures. If passed without keyids, the default GPG key is"
-      " used."))
-
-  parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
-
-  # Only when signing
-  parser.add_argument("-o", "--output", type=str, metavar="<path>",
-      help=(
-      "path to location where the metadata file is stored after signing. If"
-      " not passed, layout metadata is written to the path of the input file"
-      " and link metadata is written to '<name>.<keyid prefix>.link'"))
-
-  # Only when signing
-  parser.add_argument("-a", "--append", action="store_true",
-      help=(
-      "add signatures rather than replacing existing signatures. This option"
-      " is only availabe for layout metdata."))
-
-  parser.add_argument("--verify", action="store_true",
-      help="verify signatures of passed link or layout metadata using the"
-      " public keys passed via '--key' and/or '--gpg' options.")
-
-  verbosity_args = parser.add_mutually_exclusive_group(required=False)
-  verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
-  verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
-
-  parser.add_argument('--version', action='version',
-                      version='{} {}'.format(parser.prog, __version__))
-
-  title_case_action_groups(parser)
-  sort_action_groups(parser)
-
-  return parser
+    return parser
 
 
 def main():
-  """Parse arguments, load link or layout metadata file and either sign
-  metadata file or verify its signatures. """
+    """Parse arguments, load link or layout metadata file and either sign
+    metadata file or verify its signatures."""
 
-  parser = create_parser()
-  args = parser.parse_args()
+    parser = create_parser()
+    args = parser.parse_args()
 
-  LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
+    LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
 
-  # Additional argparse sanitization
-  # NOTE: This tool is starting to have many inter-dependent argument
-  # restrictions. Maybe we should make it less sophisticated at some point.
-  if args.verify and (args.append or args.output):
-    parser.print_help()
-    parser.error("conflicting arguments: don't specify any of"
-        " 'append' or 'output' when verifying signatures")
-
-  # Regular signing and GPG signing are mutually exclusive
-  if (args.key is None) == (args.gpg is None):
-    parser.print_help()
-    parser.error("wrong arguments: specify either '--key PATH [PATH ...]'"
-      " or '--gpg [KEYID [KEYID ...]]'")
-
-  # For gpg verification we must specify a keyid (no default key is loaded)
-  if args.verify and args.gpg is not None and len(args.gpg) < 1:
-    parser.print_help()
-    parser.error("missing arguments: specify at least one keyid for GPG"
-      " signature verification ('--gpg KEYID ...')")
-
-  metadata = _load_metadata(args.file)
-
-  # Specific command line argument restrictions if we deal with links
-  payload = metadata.get_payload()
-  if payload.type_ == "link":
-    # Above we check that it's either `--key ...` or `--gpg ...`
-    # Here we check that it is not more than one in each case when dealing
-    # with links
-    link_error_message = ("link metadata is associated with a"
-        " single functionary and is usually namespaced accordingly:"
-        " '<name>.<keyid prefix>.link'.")
-
-    if ((args.key is not None and len(args.key) > 1) or
-        (args.gpg is not None and len(args.gpg) > 1)):
-      parser.print_help()
-      parser.error("too many arguments: {} Hence signing Link metadata"
-          " with multiple keys is not allowed.".format(link_error_message))
-
-    if args.append:
-      parser.print_help()
-      parser.error("wrong arguments: {}. Hence adding signatures to"
-          " existing signatures on link metadata is not allowed."
-          .format(link_error_message))
+    # Additional argparse sanitization
+    # NOTE: This tool is starting to have many inter-dependent argument
+    # restrictions. Maybe we should make it less sophisticated at some point.
+    if args.verify and (args.append or args.output):
+        parser.print_help()
+        parser.error(
+            "conflicting arguments: don't specify any of"
+            " 'append' or 'output' when verifying signatures"
+        )
+
+    # Regular signing and GPG signing are mutually exclusive
+    if (args.key is None) == (args.gpg is None):
+        parser.print_help()
+        parser.error(
+            "wrong arguments: specify either '--key PATH [PATH ...]'"
+            " or '--gpg [KEYID [KEYID ...]]'"
+        )
+
+    # For gpg verification we must specify a keyid (no default key is loaded)
+    if args.verify and args.gpg is not None and len(args.gpg) < 1:
+        parser.print_help()
+        parser.error(
+            "missing arguments: specify at least one keyid for GPG"
+            " signature verification ('--gpg KEYID ...')"
+        )
 
+    metadata = _load_metadata(args.file)
+
+    # Specific command line argument restrictions if we deal with links
+    payload = metadata.get_payload()
+    if payload.type_ == "link":
+        # Above we check that it's either `--key ...` or `--gpg ...`
+        # Here we check that it is not more than one in each case when dealing
+        # with links
+        link_error_message = (
+            "link metadata is associated with a"
+            " single functionary and is usually namespaced accordingly:"
+            " '<name>.<keyid prefix>.link'."
+        )
+
+        if (args.key is not None and len(args.key) > 1) or (
+            args.gpg is not None and len(args.gpg) > 1
+        ):
+            parser.print_help()
+            parser.error(
+                "too many arguments: {} Hence signing Link metadata"
+                " with multiple keys is not allowed.".format(link_error_message)
+            )
+
+        if args.append:
+            parser.print_help()
+            parser.error(
+                "wrong arguments: {}. Hence adding signatures to"
+                " existing signatures on link metadata is not allowed.".format(
+                    link_error_message
+                )
+            )
 
-  if args.verify:
-    _verify_metadata(metadata, args)
+    if args.verify:
+        _verify_metadata(metadata, args)
 
-  else:
-    _sign_and_dump_metadata(metadata, args)
+    else:
+        _sign_and_dump_metadata(metadata, args)
 
 
 if __name__ == "__main__":
-  main()
+    main()
```

### Comparing `in_toto-1.4.0/in_toto/in_toto_verify.py` & `in_toto-2.0.0/in_toto/in_toto_verify.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,37 +21,51 @@
 
 <Return Codes>
   2 if an exception occurred during argument parsing
   1 if an exception occurred (verification failed)
   0 if no exception occurred (verification passed)
 
 """
-import sys
 import argparse
 import logging
+import sys
 
-from in_toto import verifylib
-from in_toto.common_args import (GPG_HOME_ARGS, GPG_HOME_KWARGS, VERBOSE_ARGS,
-    VERBOSE_KWARGS, QUIET_ARGS, QUIET_KWARGS, title_case_action_groups,
-    sort_action_groups, OPTS_TITLE)
-from in_toto.models.metadata import Metadata
-from in_toto import (
-    __version__, SUPPORTED_KEY_TYPES, KEY_TYPE_RSA, KEY_TYPE_ED25519,
-    KEY_TYPE_ECDSA)
 from securesystemslib import interface
 from securesystemslib.gpg import functions as gpg_interface
 
+from in_toto import (
+    KEY_TYPE_ECDSA,
+    KEY_TYPE_ED25519,
+    KEY_TYPE_RSA,
+    SUPPORTED_KEY_TYPES,
+    __version__,
+    verifylib,
+)
+from in_toto.common_args import (
+    GPG_HOME_ARGS,
+    GPG_HOME_KWARGS,
+    OPTS_TITLE,
+    QUIET_ARGS,
+    QUIET_KWARGS,
+    VERBOSE_ARGS,
+    VERBOSE_KWARGS,
+    sort_action_groups,
+    title_case_action_groups,
+)
+from in_toto.models.metadata import Metadata
+
 # Command line interfaces should use in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger("in_toto")
 
+
 def create_parser():
-  """Create and return configured ArgumentParser instance. """
-  parser = argparse.ArgumentParser(
-      formatter_class=argparse.RawDescriptionHelpFormatter,
-      description="""
+    """Create and return configured ArgumentParser instance."""
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description="""
 in-toto-verify is the main verification tool of the suite, and it is used to
 verify that the software supply chain of the delivered product was carried out
 as defined in the passed in-toto supply chain layout. Evidence for supply chain
 steps must be available in the form of link metadata files named
 '<step name>.<functionary keyid prefix>.link'.
 
 Both 'in-toto-run' and 'in-toto-record' generate link metadata named in this
@@ -71,20 +85,26 @@
 
 If the layout includes sublayouts, the verification routine will recurse into a
 subdirectory named '<step name>.<keyid prefix>', where all the links relevant
 to that sublayout must exist. The sublayout itself must be in the same
 directory as the other links of the superlayout. (i.e. '<step name>.<keyid
 prefix>.link')
 
+The verification workflow is performed in isolation and does not rely on
+information about keys that are available through external sources. For example,
+in-toto does not rely on the creation time, revocation status, and usage flags
+for PGP keys.
+
 The command returns 2 if it is called with wrong arguments, 1 if in-toto
-verification fails and 0 if verification passes. """)
+verification fails and 0 if verification passes. """,
+    )
 
-  parser.usage = "%(prog)s <named arguments> [{}]".format(OPTS_TITLE.lower())
+    parser.usage = "%(prog)s <named arguments> [{}]".format(OPTS_TITLE.lower())
 
-  parser.epilog = """EXAMPLE USAGE
+    parser.epilog = """EXAMPLE USAGE
 
 Verify supply chain in 'root.layout', signed with private part of
 'key_file.pub'.
 
   {prog} --layout root.layout --layout-keys key_file.pub
 
 
@@ -99,106 +119,150 @@
 for which the public part can be found in the GPG keyring at '~/.gnupg'.
 
   {prog} --layout root.layout \\
       --gpg 8465A1E2E0FB2B40ADB2478E18FB3F537E0C8A17 \\
       --gpg-home ~/.gnupg
 
 
-""".format(prog=parser.prog)
-
-
-  named_args = parser.add_argument_group("required named arguments")
-
-  named_args.add_argument("-l", "--layout", type=str, required=True,
-      metavar="<path>", help=(
-      "path to root layout specifying the software supply chain to be"
-      " verified."))
-
-  named_args.add_argument("-k", "--layout-keys", type=str, metavar="<path>",
-      nargs="+", help=(
-      "paths to public key files used to verify the passed root layout's"
-      " signatures. See '--key-types' for available formats. Passing at least"
-      " one key using '--layout-keys' and/or '--gpg' is required. For each"
-      " passed key the layout must carry a valid signature."))
-
-  parser.add_argument("-t", "--key-types", dest="key_types",
-      type=str, choices=SUPPORTED_KEY_TYPES,
-      nargs="+", help=(
-      "types of keys specified by the '--layout-keys' option. '{rsa}' keys are"
-      " expected in a 'PEM' format. '{ed25519}' and '{ecdsa}' are expected"
-      " in a custom 'securesystemslib/json' format. If multiple keys are"
-      " passed via '--layout-keys' the same amount of key types must be"
-      " passed. Key types are then associated with keys by index. If"
-      " '--key-types' is omitted, the default of '{rsa}' is used for all"
-      " keys.".format(
-      rsa=KEY_TYPE_RSA, ed25519=KEY_TYPE_ED25519, ecdsa=KEY_TYPE_ECDSA)))
-
-  named_args.add_argument("-g", "--gpg", nargs="+", metavar="<id>",
-      help=(
-      "GPG keyid, identifying a public key in the GPG keyring used to verify"
-      " the passed root layout's signatures."
-      " Passing at least one key using '--layout-keys' and/or '--gpg' is"
-      " required. For each passed key the layout must carry a valid"
-      " signature."))
-
-  parser.add_argument("--link-dir", dest="link_dir", type=str,
-      metavar="<path>", default=".", help=(
-          "path to directory from which link metadata files for steps defined"
-          " in the root layout should be loaded. If not passed, links are"
-          " loaded from the current working directory."))
-
-  parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
-
-  verbosity_args = parser.add_mutually_exclusive_group(required=False)
-  verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
-  verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
+""".format(
+        prog=parser.prog
+    )
+
+    named_args = parser.add_argument_group("required named arguments")
+
+    named_args.add_argument(
+        "-l",
+        "--layout",
+        type=str,
+        required=True,
+        metavar="<path>",
+        help=(
+            "path to root layout specifying the software supply chain to be"
+            " verified."
+        ),
+    )
+
+    named_args.add_argument(
+        "-k",
+        "--layout-keys",
+        type=str,
+        metavar="<path>",
+        nargs="+",
+        help=(
+            "paths to public key files used to verify the passed root layout's"
+            " signatures. See '--key-types' for available formats. Passing at least"
+            " one key using '--layout-keys' and/or '--gpg' is required. For each"
+            " passed key the layout must carry a valid signature."
+        ),
+    )
+
+    parser.add_argument(
+        "-t",
+        "--key-types",
+        dest="key_types",
+        type=str,
+        choices=SUPPORTED_KEY_TYPES,
+        nargs="+",
+        help=(
+            "types of keys specified by the '--layout-keys' option. '{rsa}' keys are"
+            " expected in a 'PEM' format. '{ed25519}' and '{ecdsa}' are expected"
+            " in a custom 'securesystemslib/json' format. If multiple keys are"
+            " passed via '--layout-keys' the same amount of key types must be"
+            " passed. Key types are then associated with keys by index. If"
+            " '--key-types' is omitted, the default of '{rsa}' is used for all"
+            " keys.".format(
+                rsa=KEY_TYPE_RSA, ed25519=KEY_TYPE_ED25519, ecdsa=KEY_TYPE_ECDSA
+            )
+        ),
+    )
+
+    named_args.add_argument(
+        "-g",
+        "--gpg",
+        nargs="+",
+        metavar="<id>",
+        help=(
+            "GPG keyid, identifying a public key in the GPG keyring used to verify"
+            " the passed root layout's signatures."
+            " Passing at least one key using '--layout-keys' and/or '--gpg' is"
+            " required. For each passed key the layout must carry a valid"
+            " signature."
+        ),
+    )
+
+    parser.add_argument(
+        "--link-dir",
+        dest="link_dir",
+        type=str,
+        metavar="<path>",
+        default=".",
+        help=(
+            "path to directory from which link metadata files for steps defined"
+            " in the root layout should be loaded. If not passed, links are"
+            " loaded from the current working directory."
+        ),
+    )
+
+    parser.add_argument(*GPG_HOME_ARGS, **GPG_HOME_KWARGS)
+
+    verbosity_args = parser.add_mutually_exclusive_group(required=False)
+    verbosity_args.add_argument(*VERBOSE_ARGS, **VERBOSE_KWARGS)
+    verbosity_args.add_argument(*QUIET_ARGS, **QUIET_KWARGS)
+
+    parser.add_argument(
+        "--version",
+        action="version",
+        version="{} {}".format(parser.prog, __version__),
+    )
 
-  parser.add_argument('--version', action='version',
-                      version='{} {}'.format(parser.prog, __version__))
+    title_case_action_groups(parser)
+    sort_action_groups(parser)
 
-  title_case_action_groups(parser)
-  sort_action_groups(parser)
+    return parser
 
-  return parser
 
 def main():
-  """Parse arguments and call in_toto_verify. """
-  parser = create_parser()
-  args = parser.parse_args()
-
-  LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
-
-  # For verifying at least one of --layout-keys or --gpg must be specified
-  # Note: Passing both at the same time is possible.
-  if (args.layout_keys is None) and (args.gpg is None):
-    parser.print_help()
-    parser.error("wrong arguments: specify at least one of"
-        " '--layout-keys path [path ...]' or '--gpg id [id ...]'")
-
-  try:
-    LOG.info("Loading layout...")
-    layout = Metadata.load(args.layout)
-
-    layout_key_dict = {}
-    if args.layout_keys is not None:
-      LOG.info("Loading layout key(s)...")
-      layout_key_dict.update(
-          interface.import_publickeys_from_file(
-              args.layout_keys, args.key_types))
-
-    if args.gpg is not None:
-      LOG.info("Loading layout gpg key(s)...")
-      layout_key_dict.update(
-          gpg_interface.export_pubkeys(
-              args.gpg, homedir=args.gpg_home))
-
-    verifylib.in_toto_verify(layout, layout_key_dict, args.link_dir)
-
-  except Exception as e:
-    LOG.error("(in-toto-verify) {0}: {1}".format(type(e).__name__, e))
-    sys.exit(1)
+    """Parse arguments and call in_toto_verify."""
+    parser = create_parser()
+    args = parser.parse_args()
+
+    LOG.setLevelVerboseOrQuiet(args.verbose, args.quiet)
+
+    # For verifying at least one of --layout-keys or --gpg must be specified
+    # Note: Passing both at the same time is possible.
+    if (args.layout_keys is None) and (args.gpg is None):
+        parser.print_help()
+        parser.error(
+            "wrong arguments: specify at least one of"
+            " '--layout-keys path [path ...]' or '--gpg id [id ...]'"
+        )
+
+    try:
+        LOG.info("Loading layout...")
+        layout = Metadata.load(args.layout)
+
+        layout_key_dict = {}
+        if args.layout_keys is not None:
+            LOG.info("Loading layout key(s)...")
+            layout_key_dict.update(
+                interface.import_publickeys_from_file(
+                    args.layout_keys, args.key_types
+                )
+            )
+
+        if args.gpg is not None:
+            LOG.info("Loading layout gpg key(s)...")
+            layout_key_dict.update(
+                gpg_interface.export_pubkeys(args.gpg, homedir=args.gpg_home)
+            )
+
+        verifylib.in_toto_verify(layout, layout_key_dict, args.link_dir)
+
+    except Exception as e:
+        LOG.error("(in-toto-verify) {0}: {1}".format(type(e).__name__, e))
+        sys.exit(1)
 
-  sys.exit(0)
+    sys.exit(0)
 
 
 if __name__ == "__main__":
-  main()
+    main()
```

### Comparing `in_toto-1.4.0/in_toto/log.py` & `in_toto-2.0.0/in_toto/log.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,66 +65,73 @@
 
   LOG.info("In debug mode it looks something like this)
   # in_toto.runlib:400:INFO:In debug mode it looks something like this
 
   ```
 
 """
-import sys
 import logging
+import sys
+
 import in_toto.settings
 
 # Different log message formats for different log levels
 FORMAT_MESSAGE = "%(message)s"
 FORMAT_DEBUG = "%(name)s:%(lineno)d:%(levelname)s:%(message)s"
 
 # Cache default logger class, should be logging.Logger if not changed elsewhere
 _LOGGER_CLASS = logging.getLoggerClass()
 
+
 # Create logger subclass
 class InTotoLogger(_LOGGER_CLASS):
-  """logger.Logging subclass, using providing custom error method and
-  convenience method for log levels. """
+    """logger.Logging subclass, using providing custom error method and
+    convenience method for log levels."""
 
-  QUIET = logging.CRITICAL + 1
+    QUIET = logging.CRITICAL + 1
 
-  def error(self, msg):
-    """Show stacktrace depending on its availability and the logger's log
-    level, i.e. only show stacktrace in DEBUG level. """
-    show_stacktrace = (self.level == logging.DEBUG and
-        sys.exc_info() != (None, None, None))
-    return super(InTotoLogger, self).error(msg, exc_info=show_stacktrace)
-
-  # Allow non snake_case function name for consistency with logging library
-  def setLevelVerboseOrQuiet(self, verbose, quiet): # pylint: disable=invalid-name
-    """Convenience method to set the logger's verbosity level based on the
-    passed booleans verbose and quiet (useful for cli tools). """
-    if verbose:
-      self.setLevel(logging.INFO)
-
-    elif quiet:
-      # TODO: Is it enough to use logging.CRITICAL + 1 to suppress all output?
-      # A saver way would be to use a NullHandler or Filters.
-      self.setLevel(self.QUIET)
+    def error(self, msg):
+        """Show stacktrace depending on its availability and the logger's log
+        level, i.e. only show stacktrace in DEBUG level."""
+        show_stacktrace = self.level == logging.DEBUG and sys.exc_info() != (
+            None,
+            None,
+            None,
+        )
+        return super(InTotoLogger, self).error(msg, exc_info=show_stacktrace)
+
+    # Allow non snake_case function name for consistency with logging library
+    def setLevelVerboseOrQuiet(
+        self, verbose, quiet
+    ):  # pylint: disable=invalid-name
+        """Convenience method to set the logger's verbosity level based on the
+        passed booleans verbose and quiet (useful for cli tools)."""
+        if verbose:
+            self.setLevel(logging.INFO)
+
+        elif quiet:
+            # TODO: Is it enough to use logging.CRITICAL + 1 to suppress all output?
+            # A saver way would be to use a NullHandler or Filters.
+            self.setLevel(self.QUIET)
 
 
 # Temporarily change logger default class to instantiate an in-toto base logger
 logging.setLoggerClass(InTotoLogger)
 LOGGER = logging.getLogger("in_toto")
 logging.setLoggerClass(_LOGGER_CLASS)
 
 # In DEBUG mode we log all log types and add additional information,
 # otherwise we only log warning, error and critical and only the message.
-if in_toto.settings.DEBUG: # pragma: no cover
-  LEVEL = logging.DEBUG
-  FORMAT_STRING = FORMAT_DEBUG
+if in_toto.settings.DEBUG:  # pragma: no cover
+    LEVEL = logging.DEBUG
+    FORMAT_STRING = FORMAT_DEBUG
 
 else:
-  LEVEL = logging.WARNING
-  FORMAT_STRING = FORMAT_MESSAGE
+    LEVEL = logging.WARNING
+    FORMAT_STRING = FORMAT_MESSAGE
 
 # Add a StreamHandler with the chosen format to in-toto's base logger,
 # which will write log messages to `sys.stderr`.
 FORMATTER = logging.Formatter(FORMAT_STRING)
 HANDLER = logging.StreamHandler()
 HANDLER.setFormatter(FORMATTER)
 LOGGER.addHandler(HANDLER)
```

### Comparing `in_toto-1.4.0/in_toto/rulelib.py` & `in_toto-2.0.0/in_toto/rulelib.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,290 +19,344 @@
   This module provides functions parse artifact rules and validate their
   syntax.
 
 """
 import securesystemslib.exceptions
 import securesystemslib.formats
 
-GENERIC_RULES = {"create", "modify", "delete", "allow", "disallow", "require",}
-COMPLEX_RULES = {"match",}
+GENERIC_RULES = {
+    "create",
+    "modify",
+    "delete",
+    "allow",
+    "disallow",
+    "require",
+}
+COMPLEX_RULES = {
+    "match",
+}
 ALL_RULES = GENERIC_RULES | COMPLEX_RULES
 
+
 def unpack_rule(rule):
-  """
-  Parses the rule and extracts and returns the necessary data to apply the
-  rule. Can also be used to verify if a rule complies with any of the formats
-
-  <Arguments>
-    rule:
-        The list of rule elements, in one of the following formats:
+    """
+    Parses the rule and extracts and returns the necessary data to apply the
+    rule. Can also be used to verify if a rule complies with any of the formats
+
+    <Arguments>
+      rule:
+          The list of rule elements, in one of the following formats:
+          MATCH <pattern> [IN <source-path-prefix>] WITH (MATERIALS|PRODUCTS)
+              [IN <destination-path-prefix>] FROM <step>,
+          CREATE <pattern>,
+          DELETE <pattern>,
+          MODIFY <pattern>,
+          ALLOW <pattern>,
+          DISALLOW <pattern>,
+          REQUIRE <file>
+
+    Note that REQUIRE is somewhat of a weird animal that does not use patterns
+    but rather single filenames (for now).
+
+    <Exceptions>
+      raises FormatError, if the rule does not comply with any of the formats.
+
+    <Side Effects>
+      None.
+
+    <Returns>
+      A dictionary of the artifact rule data,
+      if it is a generic rule the dictionary is:
+      {
+        "rule_type": rule[0] ("CREATE"|"MODIFY"|"DELETE"|"ALLOW"|"DISALLOW")
+        "pattern" : rule[1], a path pattern
+      }
+
+      if it is a match rule, the dictionary is:
+      {
+        "rule_type": rule[0],  ("MATCH"),
+        "pattern": rule[1], a path pattern
+        "source_prefix": path or empty string
+        "dest_prefix": path or empty string
+        "dest_type" : destination artifact type, ("MATERIAL"|"PRODUCT")
+        "dest_name": destination step/inspection name
+      }
+
+    """
+    securesystemslib.formats.LIST_OF_ANY_STRING_SCHEMA.check_match(rule)
+
+    # Create all lower rule copy to case insensitively parse out tokens whose
+    # position we don't know yet
+    # We keep the original rule to retain the non-token elements' case
+    rule_lower = []
+    for rule_elem in rule:
+        rule_lower.append(rule_elem.lower())
+
+    rule_len = len(rule)
+
+    if rule_len < 2 or rule_lower[0] not in ALL_RULES:
+        raise securesystemslib.exceptions.FormatError(
+            "Wrong rule format,"
+            " rules must start with one of '{0}' and specify a 'pattern' as"
+            " second element.\n"
+            "Got: \n\t'{1}'".format(", ".join(ALL_RULES), rule)
+        )
+
+    rule_type = rule_lower[0]
+    pattern = rule[1]
+
+    # Type is one of "CREATE", "MODIFY", "DELETE", "ALLOW", "DISALLOW"
+    if rule_type in GENERIC_RULES:
+        # pylint: disable=no-else-raise
+        if rule_len != 2:
+            raise securesystemslib.exceptions.FormatError(
+                "Wrong rule format,"
+                " generic rules must have one of the formats:\n\t"
+                "CREATE <pattern>\n\t"
+                "MODIFY <pattern>\n\t"
+                "DELETE <pattern>\n\t"
+                "ALLOW <pattern>\n\t"
+                "DISALLOW <pattern>\n"
+                "REQUIRE <file>\n"
+                "Got:\n\t{}".format(rule)
+            )
+        else:
+            return {
+                "rule_type": rule_type,
+                "pattern": pattern,
+            }
+
+    # Type is "MATCH"
+    # NOTE: Can't reach `else` branch, if the rule is neither in GENERIC_RULES
+    # nor in COMPLEX_RULES an exception is raised earlier.
+    elif rule_type in COMPLEX_RULES:  # pragma: no branch
+        # ... IN <source-path-prefix> WITH (MATERIALS|PRODUCTS)
+        # IN <destination-path-prefix> FROM <step>
+        if (
+            rule_len == 10
+            and rule_lower[2] == "in"
+            and rule_lower[4] == "with"
+            and rule_lower[6] == "in"
+            and rule_lower[8] == "from"
+        ):
+            source_prefix = rule[3]
+            dest_type = rule_lower[5]
+            dest_prefix = rule[7]
+            dest_name = rule[9]
+
+        # ... IN <source-path-prefix> WITH (MATERIALS|PRODUCTS) FROM <step>
+        elif (
+            rule_len == 8
+            and rule_lower[2] == "in"
+            and rule_lower[4] == "with"
+            and rule_lower[6] == "from"
+        ):
+            source_prefix = rule[3]
+            dest_type = rule_lower[5]
+            dest_prefix = ""
+            dest_name = rule[7]
+
+        # ... WITH (MATERIALS|PRODUCTS) IN <destination-path-prefix> FROM <step>
+        elif (
+            rule_len == 8
+            and rule_lower[2] == "with"
+            and rule_lower[4] == "in"
+            and rule_lower[6] == "from"
+        ):
+            source_prefix = ""
+            dest_type = rule_lower[3]
+            dest_prefix = rule[5]
+            dest_name = rule[7]
+
+        # ... WITH (MATERIALS|PRODUCTS) FROM <step>
+        elif (
+            rule_len == 6
+            and rule_lower[2] == "with"
+            and rule_lower[4] == "from"
+        ):
+            source_prefix = ""
+            dest_type = rule_lower[3]
+            dest_prefix = ""
+            dest_name = rule[5]
+
+        else:
+            raise securesystemslib.exceptions.FormatError(
+                "Wrong rule format,"
+                " match rules must have the format:\n\t"
+                " MATCH <pattern> [IN <source-path-prefix>] WITH"
+                " (MATERIALS|PRODUCTS) [IN <destination-path-prefix>] FROM <step>.\n"
+                "Got: \n\t{}".format(rule)
+            )
+
+        if dest_type not in {"materials", "products"}:
+            raise securesystemslib.exceptions.FormatError(
+                "Wrong rule format,"
+                " match rules must have either MATERIALS or PRODUCTS (case"
+                " insensitive) as destination.\n"
+                "Got: \n\t{}".format(rule)
+            )
+
+        return {
+            "rule_type": rule_type,
+            "pattern": pattern,
+            "source_prefix": source_prefix,
+            "dest_prefix": dest_prefix,
+            "dest_type": dest_type,
+            "dest_name": dest_name,
+        }
+
+
+def pack_rule(
+    rule_type,
+    pattern,
+    source_prefix=None,
+    dest_type=None,
+    dest_prefix=None,
+    dest_name=None,
+):
+    """
+    <Purpose>
+      Create an artifact rule in the passed arguments and return it as list
+      as it is stored in a step's or inspection's expected_material or
+      expected_product field.
+
+    <Arguments>
+      rule_type:
+              One of "MATCH", "CREATE", "DELETE", MODIFY, ALLOW, DISALLOW,
+              REQUIRE (case insensitive).
+
+      pattern:
+              A glob pattern to match artifact paths.
+
+      source_prefix: (only for "MATCH" rules)
+              A prefix for 'pattern' to match artifacts reported by the link
+              corresponding to the step that contains the rule.
+
+      dest_type: (only for "MATCH" rules)
+              One of "MATERIALS" or "PRODUCTS" (case insensitive) to specify
+              if materials or products of the link corresponding to the step
+              identified by 'dest_name' should be matched.
+
+      dest_prefix: (only for "MATCH" rules)
+              A prefix for 'pattern' to match artifacts reported by the link
+              corresponding to the step identified by 'dest_name'.
+
+      dest_name: (only for "MATCH" rules)
+              The name of the step whose corresponding link is used to match
+              artifacts.
+
+
+    <Exceptions>
+      securesystemslib.exceptions.FormatError
+              if any of the arguments is malformed.
+
+
+    <Returns>
+      One of the following rule formats in as a list
         MATCH <pattern> [IN <source-path-prefix>] WITH (MATERIALS|PRODUCTS)
             [IN <destination-path-prefix>] FROM <step>,
         CREATE <pattern>,
         DELETE <pattern>,
         MODIFY <pattern>,
         ALLOW <pattern>,
         DISALLOW <pattern>,
         REQUIRE <file>
 
-  Note that REQUIRE is somewhat of a weird animal that does not use patterns
-  but rather single filenames (for now).
-
-  <Exceptions>
-    raises FormatError, if the rule does not comply with any of the formats.
+      Note that REQUIRE is somewhat of a weird animal that does not use patterns
+      but rather single filenames (for now).
+    """
+    securesystemslib.formats.ANY_STRING_SCHEMA.check_match(rule_type)
+    securesystemslib.formats.ANY_STRING_SCHEMA.check_match(pattern)
+
+    if rule_type.lower() not in ALL_RULES:
+        raise securesystemslib.exceptions.FormatError(
+            "'{0}' is not a valid "
+            "'type'.  Rule type must be one of:  {1} (case insensitive).".format(
+                rule_type, ", ".join(ALL_RULES)
+            )
+        )
+
+    if rule_type.upper() == "MATCH":
+        if not securesystemslib.formats.ANY_STRING_SCHEMA.matches(
+            dest_type
+        ) or not (
+            dest_type.lower() == "materials" or dest_type.lower() == "products"
+        ):
+            raise securesystemslib.exceptions.FormatError(
+                "'{}' is not a valid"
+                " 'dest_type'. Rules of type 'MATCH' require a destination type of"
+                " either 'MATERIALS' or 'PRODUCTS' (case insensitive).".format(
+                    dest_type
+                )
+            )
+
+        if not (
+            securesystemslib.formats.ANY_STRING_SCHEMA.matches(dest_name)
+            and dest_name
+        ):
+            raise securesystemslib.exceptions.FormatError(
+                "'{}' is not a valid"
+                " 'dest_name'. Rules of type 'MATCH' require a step name as a"
+                " destination name.".format(dest_name)
+            )
+
+        # Construct rule
+        rule = ["MATCH", pattern]
+
+        if source_prefix:
+            securesystemslib.formats.ANY_STRING_SCHEMA.check_match(
+                source_prefix
+            )
+            rule += ["IN", source_prefix]
+
+        rule += ["WITH", dest_type.upper()]
+
+        if dest_prefix:
+            securesystemslib.formats.ANY_STRING_SCHEMA.check_match(dest_prefix)
+            rule += ["IN", dest_prefix]
 
-  <Side Effects>
-    None.
+        rule += ["FROM", dest_name]
 
-  <Returns>
-    A dictionary of the artifact rule data,
-    if it is a generic rule the dictionary is:
-    {
-      "rule_type": rule[0] ("CREATE"|"MODIFY"|"DELETE"|"ALLOW"|"DISALLOW")
-      "pattern" : rule[1], a path pattern
-    }
-
-    if it is a match rule, the dictionary is:
-    {
-      "rule_type": rule[0],  ("MATCH"),
-      "pattern": rule[1], a path pattern
-      "source_prefix": path or empty string
-      "dest_prefix": path or empty string
-      "dest_type" : destination artifact type, ("MATERIAL"|"PRODUCT")
-      "dest_name": destination step/inspection name
-    }
-
-  """
-  securesystemslib.formats.LIST_OF_ANY_STRING_SCHEMA.check_match(rule)
-
-  # Create all lower rule copy to case insensitively parse out tokens whose
-  # position we don't know yet
-  # We keep the original rule to retain the non-token elements' case
-  rule_lower = []
-  for rule_elem in rule:
-    rule_lower.append(rule_elem.lower())
-
-  rule_len = len(rule)
-
-  if rule_len < 2 or rule_lower[0] not in ALL_RULES:
-    raise securesystemslib.exceptions.FormatError("Wrong rule format,"
-        " rules must start with one of '{0}' and specify a 'pattern' as"
-        " second element.\n"
-        "Got: \n\t'{1}'".format(", ".join(ALL_RULES), rule))
-
-  rule_type = rule_lower[0]
-  pattern = rule[1]
-
-  # Type is one of "CREATE", "MODIFY", "DELETE", "ALLOW", "DISALLOW"
-  if rule_type in GENERIC_RULES:
-    # pylint: disable=no-else-raise
-    if rule_len != 2:
-      raise securesystemslib.exceptions.FormatError("Wrong rule format,"
-        " generic rules must have one of the formats:\n\t"
-        "CREATE <pattern>\n\t"
-        "MODIFY <pattern>\n\t"
-        "DELETE <pattern>\n\t"
-        "ALLOW <pattern>\n\t"
-        "DISALLOW <pattern>\n"
-        "REQUIRE <file>\n"
-        "Got:\n\t{}".format(rule))
     else:
-      return {
-        "rule_type": rule_type,
-        "pattern": pattern,
-      }
+        rule = [rule_type.upper(), pattern]
 
-  # Type is "MATCH"
-  # NOTE: Can't reach `else` branch, if the rule is neither in GENERIC_RULES
-  # nor in COMPLEX_RULES an exception is raised earlier.
-  elif rule_type in COMPLEX_RULES: # pragma: no branch
-    # ... IN <source-path-prefix> WITH (MATERIALS|PRODUCTS)
-    # IN <destination-path-prefix> FROM <step>
-    if (rule_len == 10 and rule_lower[2] == "in" and
-        rule_lower[4] == "with" and rule_lower[6] == "in" and
-        rule_lower[8] == "from"):
-      source_prefix = rule[3]
-      dest_type = rule_lower[5]
-      dest_prefix = rule[7]
-      dest_name = rule[9]
-
-    # ... IN <source-path-prefix> WITH (MATERIALS|PRODUCTS) FROM <step>
-    elif (rule_len == 8 and rule_lower[2] == "in" and
-        rule_lower[4] == "with" and rule_lower[6] == "from"):
-      source_prefix = rule[3]
-      dest_type = rule_lower[5]
-      dest_prefix = ""
-      dest_name = rule[7]
-
-    # ... WITH (MATERIALS|PRODUCTS) IN <destination-path-prefix> FROM <step>
-    elif (rule_len == 8 and rule_lower[2] == "with" and
-        rule_lower[4] == "in" and rule_lower[6] == "from"):
-      source_prefix = ""
-      dest_type = rule_lower[3]
-      dest_prefix = rule[5]
-      dest_name = rule[7]
-
-    # ... WITH (MATERIALS|PRODUCTS) FROM <step>
-    elif (rule_len == 6 and rule_lower[2] == "with" and
-        rule_lower[4] == "from"):
-      source_prefix = ""
-      dest_type = rule_lower[3]
-      dest_prefix = ""
-      dest_name = rule[5]
-
-    else:
-      raise securesystemslib.exceptions.FormatError("Wrong rule format,"
-          " match rules must have the format:\n\t"
-          " MATCH <pattern> [IN <source-path-prefix>] WITH"
-          " (MATERIALS|PRODUCTS) [IN <destination-path-prefix>] FROM <step>.\n"
-          "Got: \n\t{}".format(rule))
-
-    if dest_type not in {"materials", "products"}:
-      raise securesystemslib.exceptions.FormatError("Wrong rule format,"
-          " match rules must have either MATERIALS or PRODUCTS (case"
-          " insensitive) as destination.\n"
-          "Got: \n\t{}".format(rule))
-
-    return {
-      "rule_type": rule_type,
-      "pattern": pattern,
-      "source_prefix": source_prefix,
-      "dest_prefix": dest_prefix,
-      "dest_type" : dest_type,
-      "dest_name": dest_name
-    }
-
-
-def pack_rule(rule_type, pattern, source_prefix=None, dest_type=None,
-      dest_prefix=None, dest_name=None):
-  """
-  <Purpose>
-    Create an artifact rule in the passed arguments and return it as list
-    as it is stored in a step's or inspection's expected_material or
-    expected_product field.
-
-  <Arguments>
-    rule_type:
-            One of "MATCH", "CREATE", "DELETE", MODIFY, ALLOW, DISALLOW,
-            REQUIRE (case insensitive).
-
-    pattern:
-            A glob pattern to match artifact paths.
-
-    source_prefix: (only for "MATCH" rules)
-            A prefix for 'pattern' to match artifacts reported by the link
-            corresponding to the step that contains the rule.
-
-    dest_type: (only for "MATCH" rules)
-            One of "MATERIALS" or "PRODUCTS" (case insensitive) to specify
-            if materials or products of the link corresponding to the step
-            identified by 'dest_name' should be matched.
-
-    dest_prefix: (only for "MATCH" rules)
-            A prefix for 'pattern' to match artifacts reported by the link
-            corresponding to the step identified by 'dest_name'.
-
-    dest_name: (only for "MATCH" rules)
-            The name of the step whose corresponding link is used to match
-            artifacts.
-
-
-  <Exceptions>
-    securesystemslib.exceptions.FormatError
-            if any of the arguments is malformed.
-
-
-  <Returns>
-    One of the following rule formats in as a list
-      MATCH <pattern> [IN <source-path-prefix>] WITH (MATERIALS|PRODUCTS)
-          [IN <destination-path-prefix>] FROM <step>,
-      CREATE <pattern>,
-      DELETE <pattern>,
-      MODIFY <pattern>,
-      ALLOW <pattern>,
-      DISALLOW <pattern>,
-      REQUIRE <file>
-
-    Note that REQUIRE is somewhat of a weird animal that does not use patterns
-    but rather single filenames (for now).
-  """
-  securesystemslib.formats.ANY_STRING_SCHEMA.check_match(rule_type)
-  securesystemslib.formats.ANY_STRING_SCHEMA.check_match(pattern)
-
-  if rule_type.lower() not in ALL_RULES:
-    raise securesystemslib.exceptions.FormatError("'{0}' is not a valid "
-        "'type'.  Rule type must be one of:  {1} (case insensitive)."
-        .format(rule_type, ", ".join(ALL_RULES)))
-
-  if rule_type.upper() == "MATCH":
-    if (not securesystemslib.formats.ANY_STRING_SCHEMA.matches(dest_type) or
-        not (dest_type.lower() == "materials" or
-        dest_type.lower() == "products")):
-      raise securesystemslib.exceptions.FormatError("'{}' is not a valid"
-          " 'dest_type'. Rules of type 'MATCH' require a destination type of"
-          " either 'MATERIALS' or 'PRODUCTS' (case insensitive)."
-          .format(dest_type))
-
-    if not (securesystemslib.formats.ANY_STRING_SCHEMA.matches(dest_name) and
-        dest_name):
-      raise securesystemslib.exceptions.FormatError("'{}' is not a valid"
-          " 'dest_name'. Rules of type 'MATCH' require a step name as a"
-          " destination name.".format(dest_name))
-
-    # Construct rule
-    rule = ["MATCH", pattern]
-
-    if source_prefix:
-      securesystemslib.formats.ANY_STRING_SCHEMA.check_match(source_prefix)
-      rule += ["IN", source_prefix]
-
-    rule += ["WITH", dest_type.upper()]
-
-    if dest_prefix:
-      securesystemslib.formats.ANY_STRING_SCHEMA.check_match(dest_prefix)
-      rule += ["IN", dest_prefix]
-
-    rule += ["FROM", dest_name]
-
-  else:
-    rule = [rule_type.upper(), pattern]
-
-  return rule
+    return rule
 
 
 def pack_rule_data(rule_data):
-  """Shortcut for 'pack_rule' to pack a rule based on a rule_data dictionary
-  as returned by 'unpack_rule'. """
-  return pack_rule(**rule_data)
+    """Shortcut for 'pack_rule' to pack a rule based on a rule_data dictionary
+    as returned by 'unpack_rule'."""
+    return pack_rule(**rule_data)
 
 
 def pack_create_rule(pattern):
-  """Shortcut for 'pack_rule' to pack a CREATE rule. """
-  return pack_rule("CREATE", pattern)
+    """Shortcut for 'pack_rule' to pack a CREATE rule."""
+    return pack_rule("CREATE", pattern)
 
 
 def pack_delete_rule(pattern):
-  """Shortcut for 'pack_rule' to pack a DELETE rule. """
-  return pack_rule("DELETE", pattern)
+    """Shortcut for 'pack_rule' to pack a DELETE rule."""
+    return pack_rule("DELETE", pattern)
 
 
 def pack_modify_rule(pattern):
-  """Shortcut for 'pack_rule' to pack a MODIFY rule. """
-  return pack_rule("MODIFY", pattern)
+    """Shortcut for 'pack_rule' to pack a MODIFY rule."""
+    return pack_rule("MODIFY", pattern)
 
 
 def pack_allow_rule(pattern):
-  """Shortcut for 'pack_rule' to pack an ALLOW rule. """
-  return pack_rule("ALLOW", pattern)
+    """Shortcut for 'pack_rule' to pack an ALLOW rule."""
+    return pack_rule("ALLOW", pattern)
 
 
 def pack_disallow_rule(pattern):
-  """Shortcut for 'pack_rule' to pack a DISALLOW rule. """
-  return pack_rule("DISALLOW", pattern)
+    """Shortcut for 'pack_rule' to pack a DISALLOW rule."""
+    return pack_rule("DISALLOW", pattern)
+
 
 def pack_require_rule(filename):
-  """
-  Shortcut for 'pack_rule' to pack a REQUIRE rule:
-  note that REQUIRE is somewhat of a weird animal that does not use patterns
-  but rather single filenames (for now).
-  """
-  return pack_rule("REQUIRE", filename)
+    """
+    Shortcut for 'pack_rule' to pack a REQUIRE rule:
+    note that REQUIRE is somewhat of a weird animal that does not use patterns
+    but rather single filenames (for now).
+    """
+    return pack_rule("REQUIRE", filename)
```

### Comparing `in_toto-1.4.0/in_toto/runlib.py` & `in_toto-2.0.0/in_toto/runlib.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,506 +24,394 @@
     - Execute command
       - Capture stdout/stderr/return value of the executed command
     - Record state of product (files after the command was executed)
     - Return Metadata containing a Link object which can be can be signed
       and stored to disk
 """
 import glob
+import io
 import logging
 import os
-import itertools
-import io
 import subprocess  # nosec
 import sys
 import tempfile
 import time
+from collections import defaultdict
 
-from pathspec import PathSpec
-
-import in_toto.settings
-import in_toto.exceptions
-
-from in_toto.models._signer import GPGSigner
-from in_toto.models.link import (UNFINISHED_FILENAME_FORMAT, FILENAME_FORMAT,
-    FILENAME_FORMAT_SHORT, UNFINISHED_FILENAME_FORMAT_GLOB)
-from in_toto.models.metadata import (Metadata, Envelope, Metablock)
-
-import securesystemslib.formats
-import securesystemslib.hash
 import securesystemslib.exceptions
+import securesystemslib.formats
 import securesystemslib.gpg
-from securesystemslib.signer import SSlibSigner, Signature
-
+import securesystemslib.hash
+from securesystemslib.signer import Signature, SSlibSigner
 
+import in_toto.exceptions
+import in_toto.settings
+from in_toto.models._signer import GPGSigner
+from in_toto.models.link import (
+    FILENAME_FORMAT,
+    FILENAME_FORMAT_SHORT,
+    UNFINISHED_FILENAME_FORMAT,
+    UNFINISHED_FILENAME_FORMAT_GLOB,
+)
+from in_toto.models.metadata import Envelope, Metablock, Metadata
+from in_toto.resolver import (
+    RESOLVER_FOR_URI_SCHEME,
+    FileResolver,
+    OSTreeResolver,
+    Resolver,
+)
 
 # Inherits from in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger(__name__)
 
 
+def record_artifacts_as_dict(
+    artifacts,
+    exclude_patterns=None,
+    base_path=None,
+    follow_symlink_dirs=False,
+    normalize_line_endings=False,
+    lstrip_paths=None,
+):
+    """
+    <Purpose>
+      Hashes each file in the passed path list. If the path list contains
+      paths to directories the directory tree(s) are traversed.
+
+      The files a link command is executed on are called materials.
+      The files that result form a link command execution are called
+      products.
+
+      Paths are normalized for matching and storing by left stripping "./"
+
+      NOTE on exclude patterns:
+        - Uses PathSpec to compile gitignore-style patterns, making use of the
+          GitWildMatchPattern class (registered as 'gitwildmatch')
+
+        - Patterns are checked for match against the full path relative to each
+          path passed in the artifacts list
+
+        - If a directory is excluded, all its files and subdirectories are also
+          excluded
+
+        - How it differs from .gitignore
+              - No need to escape #
+              - No ignoring of trailing spaces
+              - No general negation with exclamation mark !
+              - No special treatment of slash /
+              - No special treatment of consecutive asterisks **
+
+        - Exclude patterns are likely to become command line arguments or part of
+          a config file.
+
+    <Arguments>
+      artifacts:
+              A list of file or directory paths used as materials or products for
+              the link command.
+
+      exclude_patterns: (optional)
+              Artifacts matched by the pattern are excluded from the result.
+              Exclude patterns can be passed as argument or specified via
+              ARTIFACT_EXCLUDE_PATTERNS setting (see `in_toto.settings`).
+              If passed, patterns specified via settings are overriden.
+
+      base_path: (optional)
+              Change to base_path and record artifacts relative from there.
+              If not passed, current working directory is used as base_path.
+              NOTE: The base_path part of the recorded artifact is not included
+              in the returned paths.
+
+      follow_symlink_dirs: (optional)
+              Follow symlinked dirs if the linked dir exists (default is False).
+              The recorded path contains the symlink name, not the resolved name.
+              NOTE: This parameter toggles following linked directories only,
+              linked files are always recorded, independently of this parameter.
+              NOTE: Beware of infinite recursions that can occur if a symlink
+              points to a parent directory or itself.
+
+      normalize_line_endings: (optional)
+              If True, replaces windows and mac line endings with unix line
+              endings before hashing the content of the passed files, for
+              cross-platform support.
+
+      lstrip_paths: (optional)
+              If a prefix path is passed, the prefix is left stripped from
+              the path of every artifact that contains the prefix.
+
+    <Exceptions>
+      OSError: cannot change to base path directory.
+      ValueError: arguments are malformed.
+
+    <Side Effects>
+      Calls functions to generate cryptographic hashes.
+
+    <Returns>
+      A dictionary with file paths as keys and the files' hashes as values.
+
+    """
+    artifact_hashes = {}
+
+    if not artifacts:
+        return artifact_hashes
+
+    if not base_path:
+        base_path = in_toto.settings.ARTIFACT_BASE_PATH
+
+    if not exclude_patterns:
+        exclude_patterns = in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS
+
+    # Configure resolver with resolver specific arguments
+    # FIXME: This should happen closer to the user boundary, where
+    # resolver-specific config arguments are passed and global state is managed.
+    RESOLVER_FOR_URI_SCHEME[FileResolver.SCHEME] = FileResolver(
+        exclude_patterns,
+        base_path,
+        follow_symlink_dirs,
+        normalize_line_endings,
+        lstrip_paths,
+    )
+
+    # Configure resolver for OSTree
+    RESOLVER_FOR_URI_SCHEME[OSTreeResolver.SCHEME] = OSTreeResolver(base_path)
+
+    # Aggregate artifacts per resolver
+    resolver_for_uris = defaultdict(list)
+    for artifact in artifacts:
+        resolver = Resolver.for_uri(artifact)
+        resolver_for_uris[resolver].append(artifact)
+
+    # Hash artifacts in a batch per resolver
+    # FIXME: The behavior may change if we hash each artifact individually,
+    # because the left-prefix duplicate check in FileResolver only works for the
+    # artifacts hashed in one batch.
+    for resolver, uris in resolver_for_uris.items():
+        artifact_hashes.update(resolver.hash_artifacts(uris))
+
+    # Clear resolvers to not preserve global state change beyond this function.
+    # FIXME: This also clears resolver registered elsewhere. For now we
+    # assume that we only modify RESOLVER_FOR_URI_SCHEME in this function.
+    RESOLVER_FOR_URI_SCHEME.clear()
 
+    return artifact_hashes
 
 
-def _hash_artifact(filepath, hash_algorithms=None,
-      normalize_line_endings=False):
-  """Internal helper that takes a filename and hashes the respective file's
-  contents using the passed hash_algorithms and returns a hashdict conformant
-  with securesystemslib.formats.HASHDICT_SCHEMA. """
-  if not hash_algorithms:
-    hash_algorithms = ['sha256']
-
-  securesystemslib.formats.HASHALGORITHMS_SCHEMA.check_match(hash_algorithms)
-  hash_dict = {}
-
-  for algorithm in hash_algorithms:
-    digest_object = securesystemslib.hash.digest_filename(filepath, algorithm,
-        normalize_line_endings=normalize_line_endings)
-    hash_dict.update({algorithm: digest_object.hexdigest()})
-
-  securesystemslib.formats.HASHDICT_SCHEMA.check_match(hash_dict)
-
-  return hash_dict
-
-
-def _apply_exclude_patterns(names, exclude_filter):
-  """Exclude matched patterns from passed names."""
-  included = set(names)
-
-  # Assume old way for easier testing
-  if hasattr(exclude_filter, '__iter__'):
-    exclude_filter = PathSpec.from_lines('gitwildmatch', exclude_filter)
-
-  for excluded in exclude_filter.match_files(names):
-    included.discard(excluded)
-
-  return sorted(included)
-
-
-def _apply_left_strip(artifact_filepath, artifacts_dict, lstrip_paths=None):
-  """ Internal helper function to left strip dictionary keys based on
-  prefixes passed by the user. """
-  if lstrip_paths:
-    # If a prefix is passed using the argument --lstrip-paths,
-    # that prefix is left stripped from the filepath passed.
-    # Note: if the prefix doesn't include a trailing /, the dictionary key
-    # may include an unexpected /.
-    for prefix in lstrip_paths:
-      if artifact_filepath.startswith(prefix):
-        artifact_filepath = artifact_filepath[len(prefix):]
-        break
-
-    if artifact_filepath in artifacts_dict:
-      raise in_toto.exceptions.PrefixError("Prefix selection has "
-          "resulted in non unique dictionary key '{}'"
-          .format(artifact_filepath))
-
-  return artifact_filepath
-
-
-def record_artifacts_as_dict(artifacts, exclude_patterns=None,
-    base_path=None, follow_symlink_dirs=False, normalize_line_endings=False,
-    lstrip_paths=None):
-  """
-  <Purpose>
-    Hashes each file in the passed path list. If the path list contains
-    paths to directories the directory tree(s) are traversed.
-
-    The files a link command is executed on are called materials.
-    The files that result form a link command execution are called
-    products.
-
-    Paths are normalized for matching and storing by left stripping "./"
-
-    NOTE on exclude patterns:
-      - Uses PathSpec to compile gitignore-style patterns, making use of the
-        GitWildMatchPattern class (registered as 'gitwildmatch')
-
-      - Patterns are checked for match against the full path relative to each
-        path passed in the artifacts list
-
-      - If a directory is excluded, all its files and subdirectories are also
-        excluded
-
-      - How it differs from .gitignore
-            - No need to escape #
-            - No ignoring of trailing spaces
-            - No general negation with exclamation mark !
-            - No special treatment of slash /
-            - No special treatment of consecutive asterisks **
-
-      - Exclude patterns are likely to become command line arguments or part of
-        a config file.
-
-  <Arguments>
-    artifacts:
-            A list of file or directory paths used as materials or products for
-            the link command.
-
-    exclude_patterns: (optional)
-            Artifacts matched by the pattern are excluded from the result.
-            Exclude patterns can be passed as argument or specified via
-            ARTIFACT_EXCLUDE_PATTERNS setting (see `in_toto.settings`) or
-            via envvars or rcfiles (see `in_toto.user_settings`).
-            If passed, patterns specified via settings are overriden.
-
-    base_path: (optional)
-            Change to base_path and record artifacts relative from there.
-            If not passed, current working directory is used as base_path.
-            NOTE: The base_path part of the recorded artifact is not included
-            in the returned paths.
-
-    follow_symlink_dirs: (optional)
-            Follow symlinked dirs if the linked dir exists (default is False).
-            The recorded path contains the symlink name, not the resolved name.
-            NOTE: This parameter toggles following linked directories only,
-            linked files are always recorded, independently of this parameter.
-            NOTE: Beware of infinite recursions that can occur if a symlink
-            points to a parent directory or itself.
-
-    normalize_line_endings: (optional)
-            If True, replaces windows and mac line endings with unix line
-            endings before hashing the content of the passed files, for
-            cross-platform support.
-
-    lstrip_paths: (optional)
-            If a prefix path is passed, the prefix is left stripped from
-            the path of every artifact that contains the prefix.
-
-  <Exceptions>
-    in_toto.exceptions.ValueError,
-        if we cannot change to base path directory
-
-    in_toto.exceptions.FormatError,
-        if the list of exlcude patterns does not match format
-        securesystemslib.formats.NAMES_SCHEMA
-
-  <Side Effects>
-    Calls functions to generate cryptographic hashes.
-
-  <Returns>
-    A dictionary with file paths as keys and the files' hashes as values.
-  """
-
-  artifacts_dict = {}
-
-  if not artifacts:
-    return artifacts_dict
-
-  if base_path:
-    LOG.info("Overriding setting ARTIFACT_BASE_PATH with passed"
-        " base path.")
-  else:
-    base_path = in_toto.settings.ARTIFACT_BASE_PATH
-
-
-  # Temporarily change into base path dir if set
-  if base_path:
-    original_cwd = os.getcwd()
-    try:
-      os.chdir(base_path)
-
-    except Exception as e:
-      raise ValueError("Could not use '{}' as base path: '{}'".format(
-          base_path, e)) from  e
-
-  # Normalize passed paths
-  norm_artifacts = []
-  for path in artifacts:
-    norm_artifacts.append(os.path.normpath(path))
-
-  # Passed exclude patterns take precedence over exclude pattern settings
-  if exclude_patterns:
-    LOG.info("Overriding setting ARTIFACT_EXCLUDE_PATTERNS with passed"
-        " exclude patterns.")
-  else:
-    # TODO: Do we want to keep the exclude pattern setting?
-    exclude_patterns = in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS
-
-  # Apply exclude patterns on the passed artifact paths if available
-  if exclude_patterns:
-    securesystemslib.formats.NAMES_SCHEMA.check_match(exclude_patterns)
-    norm_artifacts = _apply_exclude_patterns(norm_artifacts, exclude_patterns)
-
-  # Check if any of the prefixes passed for left stripping is a left substring
-  # of another
-  if lstrip_paths:
-    for prefix_one, prefix_two in itertools.combinations(lstrip_paths, 2):
-      if prefix_one.startswith(prefix_two) or \
-          prefix_two.startswith(prefix_one):
-        raise in_toto.exceptions.PrefixError("'{}' and '{}' "
-            "triggered a left substring error".format(prefix_one, prefix_two))
-
-  # Compile the gitignore-style patterns
-  exclude_filter = PathSpec.from_lines('gitwildmatch', exclude_patterns or [])
-
-  # Iterate over remaining normalized artifact paths
-  for artifact in norm_artifacts:
-    if os.path.isfile(artifact):
-      # FIXME: this is necessary to provide consisency between windows
-      # filepaths and *nix filepaths. A better solution may be in order
-      # though...
-      artifact = artifact.replace('\\', '/')
-      key = _apply_left_strip(artifact, artifacts_dict, lstrip_paths)
-      artifacts_dict[key] = _hash_artifact(artifact,
-          normalize_line_endings=normalize_line_endings)
-
-    elif os.path.isdir(artifact):
-      for root, dirs, files in os.walk(artifact,
-          followlinks=follow_symlink_dirs):
-        # Create a list of normalized dirpaths
-        dirpaths = []
-        for dirname in dirs:
-          norm_dirpath = os.path.normpath(os.path.join(root, dirname))
-          dirpaths.append(norm_dirpath)
-
-        # Applying exclude patterns on the directory paths returned by walk
-        # allows to exclude a subdirectory 'sub' with a pattern 'sub'.
-        # If we only applied the patterns below on the subdirectory's
-        # containing file paths, we'd have to use a wildcard, e.g.: 'sub*'
-        if exclude_patterns:
-          dirpaths = _apply_exclude_patterns(dirpaths, exclude_filter)
-
-        # Reset and refill dirs with remaining names after exclusion
-        # Modify (not reassign) dirnames to only recurse into remaining dirs
-        dirs[:] = []
-        for dirpath in dirpaths:
-          # Dirs only contain the basename and not the full path
-          name = os.path.basename(dirpath)
-          dirs.append(name)
-
-        # Create a list of normalized filepaths
-        filepaths = []
-        for filename in files:
-          norm_filepath = os.path.normpath(os.path.join(root, filename))
-
-          # `os.walk` could also list dead symlinks, which would
-          # result in an error later when trying to read the file
-          if os.path.isfile(norm_filepath):
-            filepaths.append(norm_filepath)
-
-          else:
-            LOG.info("File '{}' appears to be a broken symlink. Skipping..."
-                .format(norm_filepath))
-
-        # Apply exlcude patterns on the normalized file paths returned by walk
-        if exclude_patterns:
-          filepaths = _apply_exclude_patterns(filepaths, exclude_filter)
-
-        for filepath in filepaths:
-          # FIXME: this is necessary to provide consisency between windows
-          # filepaths and *nix filepaths. A better solution may be in order
-          # though...
-          normalized_filepath = filepath.replace("\\", "/")
-          key = _apply_left_strip(
-              normalized_filepath, artifacts_dict, lstrip_paths)
-          artifacts_dict[key] = _hash_artifact(filepath,
-              normalize_line_endings=normalize_line_endings)
-
-    # Path is no file and no directory
-    else:
-      LOG.info("path: {} does not exist, skipping..".format(artifact))
-
-
-  # Change back to where original current working dir
-  if base_path:
-    os.chdir(original_cwd)
-
-  return artifacts_dict
-
 def _subprocess_run_duplicate_streams(cmd, timeout):
-  """Helper to run subprocess and both print and capture standards streams.
+    """Helper to run subprocess and both print and capture standards streams.
 
-  Caveat:
-  * Might behave unexpectedly with interactive commands.
-  * Might not duplicate output in real time, if the command buffers it (see
-    e.g. `print("foo")` vs. `print("foo", flush=True)`).
-  * Possible race condition on Windows when removing temporary files.
+    Caveat:
+    * Might behave unexpectedly with interactive commands.
+    * Might not duplicate output in real time, if the command buffers it (see
+      e.g. `print("foo")` vs. `print("foo", flush=True)`).
+    * Possible race condition on Windows when removing temporary files.
+
+    """
+    # Use temporary files as targets for child process standard stream redirects
+    # They seem to work better (i.e. do not hang) than pipes, when using
+    # interactive commands like `vi`.
+    stdout_fd, stdout_name = tempfile.mkstemp()
+    stderr_fd, stderr_name = tempfile.mkstemp()
+    try:
+        with io.open(  # pylint: disable=unspecified-encoding
+            stdout_name, "r"
+        ) as stdout_reader, os.fdopen(  # pylint: disable=unspecified-encoding
+            stdout_fd, "w"
+        ) as stdout_writer, io.open(  # pylint: disable=unspecified-encoding
+            stderr_name, "r"
+        ) as stderr_reader, os.fdopen(
+            stderr_fd, "w"
+        ) as stderr_writer:
+            # Store stream results in mutable dict to update it inside nested helper
+            _std = {"out": "", "err": ""}
+
+            def _duplicate_streams():
+                """Helper to read from child process standard streams, write their
+                contents to parent process standard streams, and build up return values
+                for outer function.
+                """
+                # Read until EOF but at most `io.DEFAULT_BUFFER_SIZE` bytes per call.
+                # Reading and writing in reasonably sized chunks prevents us from
+                # subverting a timeout, due to being busy for too long or indefinitely.
+                stdout_part = stdout_reader.read(io.DEFAULT_BUFFER_SIZE)
+                stderr_part = stderr_reader.read(io.DEFAULT_BUFFER_SIZE)
+                sys.stdout.write(stdout_part)
+                sys.stderr.write(stderr_part)
+                sys.stdout.flush()
+                sys.stderr.flush()
+                _std["out"] += stdout_part
+                _std["err"] += stderr_part
+
+            # Start child process, writing its standard streams to temporary files
+            proc = subprocess.Popen(  # pylint: disable=consider-using-with  # nosec
+                cmd,
+                stdout=stdout_writer,
+                stderr=stderr_writer,
+                universal_newlines=True,
+            )
+            proc_start_time = time.time()
+
+            # Duplicate streams until the process exits (or times out)
+            while proc.poll() is None:
+                # Time out as Python's `subprocess.run` would do it
+                if (
+                    timeout is not None
+                    and time.time() > proc_start_time + timeout
+                ):
+                    proc.kill()
+                    proc.wait()
+                    raise subprocess.TimeoutExpired(cmd, timeout)
+
+                _duplicate_streams()
+
+            # Read/write once more to grab everything that the process wrote between
+            # our last read in the loop and exiting, i.e. breaking the loop.
+            _duplicate_streams()
+
+    finally:
+        # The work is done or was interrupted, the temp files can be removed
+        os.remove(stdout_name)
+        os.remove(stderr_name)
 
-  """
-  # Use temporary files as targets for child process standard stream redirects
-  # They seem to work better (i.e. do not hang) than pipes, when using
-  # interactive commands like `vi`.
-  stdout_fd, stdout_name = tempfile.mkstemp()
-  stderr_fd, stderr_name = tempfile.mkstemp()
-  try:
-    with io.open(  # pylint: disable=unspecified-encoding
-      stdout_name, "r"
-    ) as stdout_reader, os.fdopen(  # pylint: disable=unspecified-encoding
-      stdout_fd, "w"
-    ) as stdout_writer, io.open(  # pylint: disable=unspecified-encoding
-      stderr_name, "r"
-    ) as stderr_reader, os.fdopen(
-      stderr_fd, "w"
-    ) as stderr_writer:
-
-      # Store stream results in mutable dict to update it inside nested helper
-      _std = {"out": "", "err": ""}
-
-      def _duplicate_streams():
-        """Helper to read from child process standard streams, write their
-        contents to parent process standard streams, and build up return values
-        for outer function.
-        """
-        # Read until EOF but at most `io.DEFAULT_BUFFER_SIZE` bytes per call.
-        # Reading and writing in reasonably sized chunks prevents us from
-        # subverting a timeout, due to being busy for too long or indefinitely.
-        stdout_part = stdout_reader.read(io.DEFAULT_BUFFER_SIZE)
-        stderr_part = stderr_reader.read(io.DEFAULT_BUFFER_SIZE)
-        sys.stdout.write(stdout_part)
-        sys.stderr.write(stderr_part)
-        sys.stdout.flush()
-        sys.stderr.flush()
-        _std["out"] += stdout_part
-        _std["err"] += stderr_part
-
-      # Start child process, writing its standard streams to temporary files
-      proc = subprocess.Popen(  # pylint: disable=consider-using-with  # nosec
-        cmd,
-        stdout=stdout_writer,
-        stderr=stderr_writer,
-        universal_newlines=True,
-      )
-      proc_start_time = time.time()
-
-      # Duplicate streams until the process exits (or times out)
-      while proc.poll() is None:
-        # Time out as Python's `subprocess.run` would do it
-        if (
-          timeout is not None
-          and time.time() > proc_start_time + timeout
-        ):
-          proc.kill()
-          proc.wait()
-          raise subprocess.TimeoutExpired(cmd, timeout)
-
-        _duplicate_streams()
-
-      # Read/write once more to grab everything that the process wrote between
-      # our last read in the loop and exiting, i.e. breaking the loop.
-      _duplicate_streams()
-
-  finally:
-    # The work is done or was interrupted, the temp files can be removed
-    os.remove(stdout_name)
-    os.remove(stderr_name)
+    # Return process exit code and captured streams
+    return proc.poll(), _std["out"], _std["err"]
 
-  # Return process exit code and captured streams
-  return proc.poll(), _std["out"], _std["err"]
 
 def execute_link(link_cmd_args, record_streams):
-  """
-  <Purpose>
-    Executes the passed command plus arguments in a subprocess and returns
-    the return value of the executed command. If the specified standard output
-    and standard error of the command are recorded and also returned to the
-    caller.
-
-  <Arguments>
-    link_cmd_args:
-            A list where the first element is a command and the remaining
-            elements are arguments passed to that command.
-    record_streams:
-            A bool that specifies whether to redirect standard output and
-            and standard error to a temporary file which is returned to the
-            caller (True) or not (False).
-
-  <Exceptions>
-    OSError:
-            The given command is not present or non-executable
-
-    subprocess.TimeoutExpired:
-            The execution of the given command times (see
-            in_toto.settings.LINK_CMD_EXEC_TIMEOUT).
-
-  <Side Effects>
-    Executes passed command in a subprocess and redirects stdout and stderr
-    if specified.
-
-  <Returns>
-    - A dictionary containing standard output and standard error of the
-      executed command, called by-products.
-      Note: If record_streams is False, the dict values are empty strings.
-    - The return value of the executed command.
-  """
-  if record_streams:
-    return_code, stdout_str, stderr_str = \
-        _subprocess_run_duplicate_streams(
-            link_cmd_args,
-            timeout=float(in_toto.settings.LINK_CMD_EXEC_TIMEOUT))
+    """
+    <Purpose>
+      Executes the passed command plus arguments in a subprocess and returns
+      the return value of the executed command. If the specified standard output
+      and standard error of the command are recorded and also returned to the
+      caller.
+
+    <Arguments>
+      link_cmd_args:
+              A list where the first element is a command and the remaining
+              elements are arguments passed to that command.
+      record_streams:
+              A bool that specifies whether to redirect standard output and
+              and standard error to a temporary file which is returned to the
+              caller (True) or not (False).
+
+    <Exceptions>
+      OSError:
+              The given command is not present or non-executable
+
+      subprocess.TimeoutExpired:
+              The execution of the given command times (see
+              in_toto.settings.LINK_CMD_EXEC_TIMEOUT).
+
+    <Side Effects>
+      Executes passed command in a subprocess and redirects stdout and stderr
+      if specified.
+
+    <Returns>
+      - A dictionary containing standard output and standard error of the
+        executed command, called by-products.
+        Note: If record_streams is False, the dict values are empty strings.
+      - The return value of the executed command.
+    """
+    if record_streams:
+        return_code, stdout_str, stderr_str = _subprocess_run_duplicate_streams(
+            link_cmd_args, timeout=float(in_toto.settings.LINK_CMD_EXEC_TIMEOUT)
+        )
 
-  else:
-    process = subprocess.run(link_cmd_args, check=False,  # nosec
-      timeout=float(in_toto.settings.LINK_CMD_EXEC_TIMEOUT),
-      stdout=subprocess.DEVNULL,
-      stderr=subprocess.DEVNULL)
-    stdout_str = stderr_str = ""
-    return_code = process.returncode
-
-  return {
-      "stdout": stdout_str,
-      "stderr": stderr_str,
-      "return-value": return_code
+    else:
+        process = subprocess.run(
+            link_cmd_args,
+            check=False,  # nosec
+            timeout=float(in_toto.settings.LINK_CMD_EXEC_TIMEOUT),
+            stdout=subprocess.DEVNULL,
+            stderr=subprocess.DEVNULL,
+        )
+        stdout_str = stderr_str = ""
+        return_code = process.returncode
+
+    return {
+        "stdout": stdout_str,
+        "stderr": stderr_str,
+        "return-value": return_code,
     }
 
 
 def in_toto_mock(name, link_cmd_args, use_dsse=False):
-  """
-  <Purpose>
-    in_toto_run with defaults
-     - Records materials and products in current directory
-     - Does not sign resulting link file
-     - Stores resulting link file under "<name>.link"
-
-  <Arguments>
-    name:
-            A unique name to relate mock link metadata with a step or
-            inspection defined in the layout.
-    link_cmd_args:
-            A list where the first element is a command and the remaining
-            elements are arguments passed to that command.
-    use_dsse (optional):
-            A boolean indicating if DSSE should be used to generate metadata.
-
-  <Exceptions>
-    None.
-
-  <Side Effects>
-    Writes newly created link metadata file to disk using the filename scheme
-    from link.FILENAME_FORMAT_SHORT
-
-  <Returns>
-    Newly created Metadata object containing a Link object
-
-  """
-  link_metadata = in_toto_run(name, ["."], ["."], link_cmd_args,
-      record_streams=True, use_dsse=use_dsse)
+    """
+    <Purpose>
+      in_toto_run with defaults
+       - Records materials and products in current directory
+       - Does not sign resulting link file
+       - Stores resulting link file under "<name>.link"
+
+    <Arguments>
+      name:
+              A unique name to relate mock link metadata with a step or
+              inspection defined in the layout.
+      link_cmd_args:
+              A list where the first element is a command and the remaining
+              elements are arguments passed to that command.
+      use_dsse (optional):
+              A boolean indicating if DSSE should be used to generate metadata.
+
+    <Exceptions>
+      None.
+
+    <Side Effects>
+      Writes newly created link metadata file to disk using the filename scheme
+      from link.FILENAME_FORMAT_SHORT
+
+    <Returns>
+      Newly created Metadata object containing a Link object
+
+    """
+    link_metadata = in_toto_run(
+        name,
+        ["."],
+        ["."],
+        link_cmd_args,
+        record_streams=True,
+        use_dsse=use_dsse,
+    )
 
-  filename = FILENAME_FORMAT_SHORT.format(step_name=name)
-  LOG.info("Storing unsigned link metadata to '{}'...".format(filename))
-  link_metadata.dump(filename)
-  return link_metadata
+    filename = FILENAME_FORMAT_SHORT.format(step_name=name)
+    LOG.info("Storing unsigned link metadata to '{}'...".format(filename))
+    link_metadata.dump(filename)
+    return link_metadata
 
 
 def _check_match_signing_key(signing_key):
-  """ Helper method to check if the signing_key has securesystemslib's
-  KEY_SCHEMA and the private part is not empty.
-  # FIXME: Add private key format check to formats
-  """
-  securesystemslib.formats.KEY_SCHEMA.check_match(signing_key)
-  if not signing_key["keyval"].get("private"):
-    raise securesystemslib.exceptions.FormatError(
-        "Signing key needs to be a private key.")
-
-
-def in_toto_run(name, material_list, product_list, link_cmd_args,
-    record_streams=False, signing_key=None, gpg_keyid=None,
-    gpg_use_default=False, gpg_home=None, exclude_patterns=None,
-    base_path=None, compact_json=False, record_environment=False,
-    normalize_line_endings=False, lstrip_paths=None, metadata_directory=None,
-    use_dsse=False):
-  """Performs a supply chain step or inspection generating link metadata.
+    """Helper method to check if the signing_key has securesystemslib's
+    KEY_SCHEMA and the private part is not empty.
+    # FIXME: Add private key format check to formats
+    """
+    securesystemslib.formats.KEY_SCHEMA.check_match(signing_key)
+    if not signing_key["keyval"].get("private"):
+        raise securesystemslib.exceptions.FormatError(
+            "Signing key needs to be a private key."
+        )
+
+
+def in_toto_run(
+    name,
+    material_list,
+    product_list,
+    link_cmd_args,
+    record_streams=False,
+    signing_key=None,
+    gpg_keyid=None,
+    gpg_use_default=False,
+    gpg_home=None,
+    exclude_patterns=None,
+    base_path=None,
+    compact_json=False,
+    record_environment=False,
+    normalize_line_endings=False,
+    lstrip_paths=None,
+    metadata_directory=None,
+    use_dsse=False,
+):
+    """Performs a supply chain step or inspection generating link metadata.
 
   Executes link_cmd_args, recording paths and hashes of files before and after
   command execution (aka. artifacts) in a link metadata file. The metadata is
   signed with the passed signing_key, a gpg key identified by its ID, or the
   default gpg key. If multiple key arguments are passed, only one key is used
   in above order of precedence. The resulting link file is written to
   ``STEP-NAME.KEYID-PREFIX.link``. If no key argument is passed the link
@@ -581,15 +469,15 @@
 
     use_dsse (optional): A boolean indicating if DSSE should be used to
         generate metadata.
 
   Raises:
     securesystemslib.exceptions.FormatError: Passed arguments are malformed.
 
-    ValueError: Cannot change to base path directory.
+    OSError: Cannot change to base path directory.
 
     securesystemslib.exceptions.StorageError: Cannot hash artifacts.
 
     PrefixError: Left-stripping artifact paths results in non-unique dict keys.
 
     subprocess.TimeoutExpired: Link command times out.
 
@@ -610,106 +498,130 @@
     Calls system gpg in a subprocess, if a gpg key argument is passed.
     Writes link metadata file to disk, if any key argument is passed.
 
   Returns:
     A Metadata object that contains the resulting link object.
 
   """
-  LOG.info("Running '{}'...".format(name))
-
-  # Check key formats to fail early
-  if signing_key:
-    _check_match_signing_key(signing_key)
-  if gpg_keyid:
-    securesystemslib.formats.KEYID_SCHEMA.check_match(gpg_keyid)
-
-  if exclude_patterns:
-    securesystemslib.formats.NAMES_SCHEMA.check_match(exclude_patterns)
-
-  if base_path:
-    securesystemslib.formats.PATH_SCHEMA.check_match(base_path)
-
-  if metadata_directory:
-    securesystemslib.formats.PATH_SCHEMA.check_match(metadata_directory)
-
-  if material_list:
-    LOG.info("Recording materials '{}'...".format(", ".join(material_list)))
-
-  materials_dict = record_artifacts_as_dict(material_list,
-      exclude_patterns=exclude_patterns, base_path=base_path,
-      follow_symlink_dirs=True, normalize_line_endings=normalize_line_endings,
-      lstrip_paths=lstrip_paths)
-
-  if link_cmd_args:
-    securesystemslib.formats.LIST_OF_ANY_STRING_SCHEMA.check_match(
-        link_cmd_args)
-    LOG.info("Running command '{}'...".format(" ".join(link_cmd_args)))
-    byproducts = execute_link(link_cmd_args, record_streams)
-  else:
-    byproducts = {}
-
-  if product_list:
-    securesystemslib.formats.PATHS_SCHEMA.check_match(product_list)
-    LOG.info("Recording products '{}'...".format(", ".join(product_list)))
-
-  products_dict = record_artifacts_as_dict(product_list,
-      exclude_patterns=exclude_patterns, base_path=base_path,
-      follow_symlink_dirs=True, normalize_line_endings=normalize_line_endings,
-      lstrip_paths=lstrip_paths)
-
-  LOG.info("Creating link metadata...")
-  environment = {}
-  if record_environment:
-    environment['workdir'] = os.getcwd().replace('\\', '/')
-
-  link = in_toto.models.link.Link(name=name,
-      materials=materials_dict, products=products_dict, command=link_cmd_args,
-      byproducts=byproducts, environment=environment)
-
-  if use_dsse:
-    LOG.info("Generating link metadata using DSSE...")
-    link_metadata = Envelope.from_signable(link)
-  else:
-    LOG.info("Generating link metadata using Metablock...")
-    link_metadata = Metablock(signed=link, compact_json=compact_json)
-
-  signer = None
-  if signing_key:
-    LOG.info("Signing link metadata using passed key...")
-    signer = SSlibSigner(signing_key)
-
-  elif gpg_keyid:
-    LOG.info("Signing link metadata using passed GPG keyid...")
-    signer = GPGSigner(keyid=gpg_keyid, homedir=gpg_home)
-
-  elif gpg_use_default:
-    LOG.info("Signing link metadata using default GPG key ...")
-    signer = GPGSigner(keyid=None, homedir=gpg_home)
-
-  # We need the signature's keyid to write the link to keyid infix'ed filename
-  if signer:
-    signature = link_metadata.create_signature(signer)
-    signing_keyid = signature.keyid
-
-    filename = FILENAME_FORMAT.format(step_name=name, keyid=signing_keyid)
-
-    if metadata_directory is not None:
-      filename = os.path.join(metadata_directory, filename)
+    LOG.info("Running '{}'...".format(name))
 
-    LOG.info("Storing link metadata to '{}'...".format(filename))
-    link_metadata.dump(filename)
-
-  return link_metadata
+    # Check key formats to fail early
+    if signing_key:
+        _check_match_signing_key(signing_key)
+    if gpg_keyid:
+        securesystemslib.formats.KEYID_SCHEMA.check_match(gpg_keyid)
+
+    if exclude_patterns:
+        securesystemslib.formats.NAMES_SCHEMA.check_match(exclude_patterns)
+
+    if base_path:
+        securesystemslib.formats.PATH_SCHEMA.check_match(base_path)
+
+    if metadata_directory:
+        securesystemslib.formats.PATH_SCHEMA.check_match(metadata_directory)
+
+    if material_list:
+        LOG.info("Recording materials '{}'...".format(", ".join(material_list)))
+
+    materials_dict = record_artifacts_as_dict(
+        material_list,
+        exclude_patterns=exclude_patterns,
+        base_path=base_path,
+        follow_symlink_dirs=True,
+        normalize_line_endings=normalize_line_endings,
+        lstrip_paths=lstrip_paths,
+    )
+
+    if link_cmd_args:
+        securesystemslib.formats.LIST_OF_ANY_STRING_SCHEMA.check_match(
+            link_cmd_args
+        )
+        LOG.info("Running command '{}'...".format(" ".join(link_cmd_args)))
+        byproducts = execute_link(link_cmd_args, record_streams)
+    else:
+        byproducts = {}
 
+    if product_list:
+        securesystemslib.formats.PATHS_SCHEMA.check_match(product_list)
+        LOG.info("Recording products '{}'...".format(", ".join(product_list)))
+
+    products_dict = record_artifacts_as_dict(
+        product_list,
+        exclude_patterns=exclude_patterns,
+        base_path=base_path,
+        follow_symlink_dirs=True,
+        normalize_line_endings=normalize_line_endings,
+        lstrip_paths=lstrip_paths,
+    )
+
+    LOG.info("Creating link metadata...")
+    environment = {}
+    if record_environment:
+        environment["workdir"] = os.getcwd().replace("\\", "/")
+
+    link = in_toto.models.link.Link(
+        name=name,
+        materials=materials_dict,
+        products=products_dict,
+        command=link_cmd_args,
+        byproducts=byproducts,
+        environment=environment,
+    )
+
+    if use_dsse:
+        LOG.info("Generating link metadata using DSSE...")
+        link_metadata = Envelope.from_signable(link)
+    else:
+        LOG.info("Generating link metadata using Metablock...")
+        link_metadata = Metablock(signed=link, compact_json=compact_json)
 
-def in_toto_record_start(step_name, material_list, signing_key=None,
-    gpg_keyid=None, gpg_use_default=False, gpg_home=None,
-    exclude_patterns=None, base_path=None, record_environment=False,
-    normalize_line_endings=False, lstrip_paths=None, use_dsse=False):
-  """Generates preliminary link metadata.
+    signer = None
+    if signing_key:
+        LOG.info("Signing link metadata using passed key...")
+        signer = SSlibSigner(signing_key)
+
+    elif gpg_keyid:
+        LOG.info("Signing link metadata using passed GPG keyid...")
+        signer = GPGSigner(keyid=gpg_keyid, homedir=gpg_home)
+
+    elif gpg_use_default:
+        LOG.info("Signing link metadata using default GPG key ...")
+        signer = GPGSigner(keyid=None, homedir=gpg_home)
+
+    # We need the signature's keyid to write the link to keyid infix'ed filename
+    if signer:
+        signature = link_metadata.create_signature(signer)
+        signing_keyid = signature.keyid
+
+        filename = FILENAME_FORMAT.format(step_name=name, keyid=signing_keyid)
+
+        if metadata_directory is not None:
+            filename = os.path.join(metadata_directory, filename)
+
+        LOG.info("Storing link metadata to '{}'...".format(filename))
+        link_metadata.dump(filename)
+
+    return link_metadata
+
+
+def in_toto_record_start(
+    step_name,
+    material_list,
+    signing_key=None,
+    gpg_keyid=None,
+    gpg_use_default=False,
+    gpg_home=None,
+    exclude_patterns=None,
+    base_path=None,
+    record_environment=False,
+    normalize_line_endings=False,
+    lstrip_paths=None,
+    use_dsse=False,
+):
+    """Generates preliminary link metadata.
 
   Records paths and hashes of materials in a preliminary link metadata file.
   The metadata is signed with the passed signing_key, a gpg key identified by
   its ID, or the default gpg key. If multiple key arguments are passed, only
   one key is used in above order of precedence. At least one key argument must
   be passed. The resulting link file is written to
   ``.STEP-NAME.KEYID-PREFIX.link-unfinished``.
@@ -780,88 +692,111 @@
 
   Side Effects:
     Reads artifact files from disk.
     Calls system gpg in a subprocess, if a gpg key argument is passed.
     Writes preliminary link metadata file to disk.
 
   """
-  LOG.info("Start recording '{}'...".format(step_name))
+    LOG.info("Start recording '{}'...".format(step_name))
+
+    # Fail if there is no signing key arg at all
+    if not signing_key and not gpg_keyid and not gpg_use_default:
+        raise ValueError(
+            "Pass either a signing key, a gpg keyid or set"
+            " gpg_use_default to True!"
+        )
+
+    # Check key formats to fail early
+    if signing_key:
+        _check_match_signing_key(signing_key)
+    if gpg_keyid:
+        securesystemslib.formats.KEYID_SCHEMA.check_match(gpg_keyid)
+
+    if exclude_patterns:
+        securesystemslib.formats.NAMES_SCHEMA.check_match(exclude_patterns)
+
+    if base_path:
+        securesystemslib.formats.PATH_SCHEMA.check_match(base_path)
+
+    if material_list:
+        LOG.info("Recording materials '{}'...".format(", ".join(material_list)))
+
+    materials_dict = record_artifacts_as_dict(
+        material_list,
+        exclude_patterns=exclude_patterns,
+        base_path=base_path,
+        follow_symlink_dirs=True,
+        normalize_line_endings=normalize_line_endings,
+        lstrip_paths=lstrip_paths,
+    )
+
+    LOG.info("Creating preliminary link metadata...")
+    environment = {}
+    if record_environment:
+        environment["workdir"] = os.getcwd().replace("\\", "/")
+
+    link = in_toto.models.link.Link(
+        name=step_name,
+        materials=materials_dict,
+        products={},
+        command=[],
+        byproducts={},
+        environment=environment,
+    )
+
+    if use_dsse:
+        LOG.info("Generating link metadata using DSSE...")
+        link_metadata = Envelope.from_signable(link)
+    else:
+        LOG.info("Generating link metadata using Metablock...")
+        link_metadata = Metablock(signed=link)
 
-  # Fail if there is no signing key arg at all
-  if not signing_key and not gpg_keyid and not gpg_use_default:
-    raise ValueError("Pass either a signing key, a gpg keyid or set"
-        " gpg_use_default to True!")
-
-  # Check key formats to fail early
-  if signing_key:
-    _check_match_signing_key(signing_key)
-  if gpg_keyid:
-    securesystemslib.formats.KEYID_SCHEMA.check_match(gpg_keyid)
-
-  if exclude_patterns:
-    securesystemslib.formats.NAMES_SCHEMA.check_match(exclude_patterns)
-
-  if base_path:
-    securesystemslib.formats.PATH_SCHEMA.check_match(base_path)
-
-  if material_list:
-    LOG.info("Recording materials '{}'...".format(", ".join(material_list)))
-
-  materials_dict = record_artifacts_as_dict(material_list,
-      exclude_patterns=exclude_patterns, base_path=base_path,
-      follow_symlink_dirs=True, normalize_line_endings=normalize_line_endings,
-      lstrip_paths=lstrip_paths)
-
-  LOG.info("Creating preliminary link metadata...")
-  environment = {}
-  if record_environment:
-    environment['workdir'] = os.getcwd().replace('\\', '/')
-
-  link = in_toto.models.link.Link(name=step_name,
-          materials=materials_dict, products={}, command=[], byproducts={},
-          environment=environment)
-
-  if use_dsse:
-    LOG.info("Generating link metadata using DSSE...")
-    link_metadata = Envelope.from_signable(link)
-  else:
-    LOG.info("Generating link metadata using Metablock...")
-    link_metadata = Metablock(signed=link)
-
-  if signing_key:
-    LOG.info("Signing link metadata using passed key...")
-    signer = SSlibSigner(signing_key)
-
-  elif gpg_keyid:
-    LOG.info("Signing link metadata using passed GPG keyid...")
-    signer = GPGSigner(keyid=gpg_keyid, homedir=gpg_home)
-
-  else:  # (gpg_use_default)
-    LOG.info("Signing link metadata using default GPG key ...")
-    signer = GPGSigner(keyid=None, homedir=gpg_home)
-
-  signature = link_metadata.create_signature(signer)
-  # We need the signature's keyid to write the link to keyid infix'ed filename
-  signing_keyid = signature.keyid
-
-  unfinished_fn = UNFINISHED_FILENAME_FORMAT.format(step_name=step_name,
-    keyid=signing_keyid)
-
-  LOG.info(
-      "Storing preliminary link metadata to '{}'...".format(unfinished_fn))
-  link_metadata.dump(unfinished_fn)
-
-
-
-def in_toto_record_stop(step_name, product_list, signing_key=None,
-    gpg_keyid=None, gpg_use_default=False, gpg_home=None,
-    exclude_patterns=None, base_path=None, normalize_line_endings=False,
-    lstrip_paths=None, metadata_directory=None, command=None, byproducts=None,
-    environment=None):
-  """Finalizes preliminary link metadata generated with in_toto_record_start.
+    if signing_key:
+        LOG.info("Signing link metadata using passed key...")
+        signer = SSlibSigner(signing_key)
+
+    elif gpg_keyid:
+        LOG.info("Signing link metadata using passed GPG keyid...")
+        signer = GPGSigner(keyid=gpg_keyid, homedir=gpg_home)
+
+    else:  # (gpg_use_default)
+        LOG.info("Signing link metadata using default GPG key ...")
+        signer = GPGSigner(keyid=None, homedir=gpg_home)
+
+    signature = link_metadata.create_signature(signer)
+    # We need the signature's keyid to write the link to keyid infix'ed filename
+    signing_keyid = signature.keyid
+
+    unfinished_fn = UNFINISHED_FILENAME_FORMAT.format(
+        step_name=step_name, keyid=signing_keyid
+    )
+
+    LOG.info(
+        "Storing preliminary link metadata to '{}'...".format(unfinished_fn)
+    )
+    link_metadata.dump(unfinished_fn)
+
+
+def in_toto_record_stop(
+    step_name,
+    product_list,
+    signing_key=None,
+    gpg_keyid=None,
+    gpg_use_default=False,
+    gpg_home=None,
+    exclude_patterns=None,
+    base_path=None,
+    normalize_line_endings=False,
+    lstrip_paths=None,
+    metadata_directory=None,
+    command=None,
+    byproducts=None,
+    environment=None,
+):
+    """Finalizes preliminary link metadata generated with in_toto_record_start.
 
   Loads preliminary link metadata file, verifies its signature, and records
   paths and hashes as products, thus finalizing the link metadata. The metadata
   is signed with the passed signing_key, a gpg key identified by its ID, or the
   default gpg key. If multiple key arguments are passed, only one key is used
   in above order of precedence. At least one key argument must be passed and it
   must be the same as the one used to sign the preliminary link metadata file.
@@ -911,14 +846,15 @@
 
     byproducts (optional): A dictionary that lists byproducts of the link
         command execution. It should have at least the following entries
         "stdout" (str), "stderr" (str) and "return-value" (int).
 
     environment (optional): A dictionary to capture information about
         the environment to be added in the resulting link metadata eg.::
+
             {
               "variables": "<list of env var KEY=value pairs>",
               "filesystem": "<filesystem info>",
               "workdir": "<CWD when executing link command>"
             }
 
   Raises:
@@ -950,141 +886,200 @@
     Reads preliminary link metadata file from disk.
     Reads artifact files from disk.
     Calls system gpg in a subprocess, if a gpg key argument is passed.
     Writes resulting link metadata file to disk.
     Removes preliminary link metadata file from disk.
 
   """
-  LOG.info("Stop recording '{}'...".format(step_name))
+    LOG.info("Stop recording '{}'...".format(step_name))
 
-  # Check that we have something to sign and if the formats are right
-  if not signing_key and not gpg_keyid and not gpg_use_default:
-    raise ValueError("Pass either a signing key, a gpg keyid or set"
-        " gpg_use_default to True")
-
-  if signing_key:
-    _check_match_signing_key(signing_key)
-  if gpg_keyid:
-    securesystemslib.formats.KEYID_SCHEMA.check_match(gpg_keyid)
-
-  if exclude_patterns:
-    securesystemslib.formats.NAMES_SCHEMA.check_match(exclude_patterns)
-
-  if base_path:
-    securesystemslib.formats.PATH_SCHEMA.check_match(base_path)
-
-  if metadata_directory:
-    securesystemslib.formats.PATH_SCHEMA.check_match(metadata_directory)
-
-  # Load preliminary link file
-  # If we have a signing key we can use the keyid to construct the name
-  if signing_key:
-    unfinished_fn = UNFINISHED_FILENAME_FORMAT.format(step_name=step_name,
-        keyid=signing_key["keyid"])
-
-  # FIXME: Currently there is no way to know the default GPG key's keyid and
-  # so we glob for preliminary link files
-  else:
-    unfinished_fn_glob = UNFINISHED_FILENAME_FORMAT_GLOB.format(
-        step_name=step_name, pattern="*")
-    unfinished_fn_list = glob.glob(unfinished_fn_glob)
-
-    if not len(unfinished_fn_list):
-      raise in_toto.exceptions.LinkNotFoundError("Could not find a preliminary"
-          " link for step '{}' in the current working directory.".format(
-          step_name))
-
-    if len(unfinished_fn_list) > 1:
-      raise in_toto.exceptions.LinkNotFoundError("Found more than one"
-          " preliminary links for step '{}' in the current working directory:"
-          " {}. We need exactly one to stop recording.".format(
-          step_name, ", ".join(unfinished_fn_list)))
-
-    unfinished_fn = unfinished_fn_list[0]
-
-  LOG.info("Loading preliminary link metadata '{}'...".format(unfinished_fn))
-  link_metadata = Metadata.load(unfinished_fn)
-
-  # The file must have been signed by the same key
-  # If we have a signing_key we use it for verification as well
-  if signing_key:
-    LOG.info(
-        "Verifying preliminary link signature using passed signing key...")
-    keyid = signing_key["keyid"]
-    verification_key = signing_key
-
-  elif gpg_keyid:
-    LOG.info("Verifying preliminary link signature using passed gpg key...")
-    gpg_pubkey = securesystemslib.gpg.functions.export_pubkey(
-        gpg_keyid, gpg_home)
-    keyid = gpg_pubkey["keyid"]
-    verification_key = gpg_pubkey
-
-  else: # must be gpg_use_default
-    # FIXME: Currently there is no way to know the default GPG key's keyid
-    # before signing. As a workaround we extract the keyid of the preliminary
-    # Link file's signature and try to export a pubkey from the gpg
-    # home directory. We do this even if a gpg_keyid was specified, because gpg
-    # accepts many different ids (mail, name, parts of an id, ...) but we
-    # need a specific format.
-    LOG.info("Verifying preliminary link signature using default gpg key...")
-    # signatures are objects in DSSE.
-    sig = link_metadata.signatures[0]
-    if isinstance(sig, Signature):
-      keyid = sig.keyid
+    # Check that we have something to sign and if the formats are right
+    if not signing_key and not gpg_keyid and not gpg_use_default:
+        raise ValueError(
+            "Pass either a signing key, a gpg keyid or set"
+            " gpg_use_default to True"
+        )
+
+    if signing_key:
+        _check_match_signing_key(signing_key)
+    if gpg_keyid:
+        securesystemslib.formats.KEYID_SCHEMA.check_match(gpg_keyid)
+
+    if exclude_patterns:
+        securesystemslib.formats.NAMES_SCHEMA.check_match(exclude_patterns)
+
+    if base_path:
+        securesystemslib.formats.PATH_SCHEMA.check_match(base_path)
+
+    if metadata_directory:
+        securesystemslib.formats.PATH_SCHEMA.check_match(metadata_directory)
+
+    # Load preliminary link file
+    # If we have a signing key we can use the keyid to construct the name
+    if signing_key:
+        unfinished_fn = UNFINISHED_FILENAME_FORMAT.format(
+            step_name=step_name, keyid=signing_key["keyid"]
+        )
+
+    # FIXME: Currently there is no way to know the default GPG key's keyid and
+    # so we glob for preliminary link files
     else:
-      keyid = sig["keyid"]
-    gpg_pubkey = securesystemslib.gpg.functions.export_pubkey(
-        keyid, gpg_home)
-    verification_key = gpg_pubkey
-
-  link_metadata.verify_signature(verification_key)
-
-  LOG.info("Extracting Link from metadata...")
-  link = link_metadata.get_payload()
-
-  # Record products if a product path list was passed
-  if product_list:
-    LOG.info("Recording products '{}'...".format(", ".join(product_list)))
-
-  link.products = record_artifacts_as_dict(
-      product_list, exclude_patterns=exclude_patterns, base_path=base_path,
-      follow_symlink_dirs=True, normalize_line_endings=normalize_line_endings,
-      lstrip_paths=lstrip_paths)
-
-  if command:
-    link.command = command
-
-  if byproducts:
-    link.byproducts = byproducts
-
-  if environment:
-    link.environment = environment
-
-  if isinstance(link_metadata, Metablock):
-    LOG.info("Generating link metadata using Metablock...")
-    link_metadata = Metablock(signed=link)
-  else:
-    LOG.info("Generating link metadata using DSSE...")
-    link_metadata = Envelope.from_signable(link)
-
-  if signing_key:
-    LOG.info("Updating signature with key '{:.8}...'...".format(keyid))
-    signer = SSlibSigner(signing_key)
-
-  else: # gpg_keyid or gpg_use_default
-    # In both cases we use the keyid we got from verifying the preliminary
-    # link signature above.
-    LOG.info("Updating signature with gpg key '{:.8}...'...".format(keyid))
-    signer = GPGSigner(keyid=keyid, homedir=gpg_home)
-
-  link_metadata.create_signature(signer)
-  fn = FILENAME_FORMAT.format(step_name=step_name, keyid=keyid)
+        unfinished_fn_glob = UNFINISHED_FILENAME_FORMAT_GLOB.format(
+            step_name=step_name, pattern="*"
+        )
+        unfinished_fn_list = glob.glob(unfinished_fn_glob)
+
+        if not len(unfinished_fn_list):
+            raise in_toto.exceptions.LinkNotFoundError(
+                "Could not find a preliminary"
+                " link for step '{}' in the current working directory.".format(
+                    step_name
+                )
+            )
+
+        if len(unfinished_fn_list) > 1:
+            raise in_toto.exceptions.LinkNotFoundError(
+                "Found more than one"
+                " preliminary links for step '{}' in the current working directory:"
+                " {}. We need exactly one to stop recording.".format(
+                    step_name, ", ".join(unfinished_fn_list)
+                )
+            )
+
+        unfinished_fn = unfinished_fn_list[0]
+
+    LOG.info("Loading preliminary link metadata '{}'...".format(unfinished_fn))
+    link_metadata = Metadata.load(unfinished_fn)
+
+    # The file must have been signed by the same key
+    # If we have a signing_key we use it for verification as well
+    if signing_key:
+        LOG.info(
+            "Verifying preliminary link signature using passed signing key..."
+        )
+        keyid = signing_key["keyid"]
+        verification_key = signing_key
+
+    elif gpg_keyid:
+        LOG.info("Verifying preliminary link signature using passed gpg key...")
+        gpg_pubkey = securesystemslib.gpg.functions.export_pubkey(
+            gpg_keyid, gpg_home
+        )
+        keyid = gpg_pubkey["keyid"]
+        verification_key = gpg_pubkey
+
+    else:  # must be gpg_use_default
+        # FIXME: Currently there is no way to know the default GPG key's keyid
+        # before signing. As a workaround we extract the keyid of the preliminary
+        # Link file's signature and try to export a pubkey from the gpg
+        # home directory. We do this even if a gpg_keyid was specified, because gpg
+        # accepts many different ids (mail, name, parts of an id, ...) but we
+        # need a specific format.
+        LOG.info(
+            "Verifying preliminary link signature using default gpg key..."
+        )
+        # signatures are objects in DSSE.
+        sig = link_metadata.signatures[0]
+        if isinstance(sig, Signature):
+            keyid = sig.keyid
+        else:
+            keyid = sig["keyid"]
+        gpg_pubkey = securesystemslib.gpg.functions.export_pubkey(
+            keyid, gpg_home
+        )
+        verification_key = gpg_pubkey
+
+    link_metadata.verify_signature(verification_key)
+
+    LOG.info("Extracting Link from metadata...")
+    link = link_metadata.get_payload()
+
+    # Record products if a product path list was passed
+    if product_list:
+        LOG.info("Recording products '{}'...".format(", ".join(product_list)))
+
+    link.products = record_artifacts_as_dict(
+        product_list,
+        exclude_patterns=exclude_patterns,
+        base_path=base_path,
+        follow_symlink_dirs=True,
+        normalize_line_endings=normalize_line_endings,
+        lstrip_paths=lstrip_paths,
+    )
+
+    if command:
+        link.command = command
+
+    if byproducts:
+        link.byproducts = byproducts
+
+    if environment:
+        link.environment = environment
+
+    if isinstance(link_metadata, Metablock):
+        LOG.info("Generating link metadata using Metablock...")
+        link_metadata = Metablock(signed=link)
+    else:
+        LOG.info("Generating link metadata using DSSE...")
+        link_metadata = Envelope.from_signable(link)
+
+    if signing_key:
+        LOG.info("Updating signature with key '{:.8}...'...".format(keyid))
+        signer = SSlibSigner(signing_key)
+
+    else:  # gpg_keyid or gpg_use_default
+        # In both cases we use the keyid we got from verifying the preliminary
+        # link signature above.
+        LOG.info("Updating signature with gpg key '{:.8}...'...".format(keyid))
+        signer = GPGSigner(keyid=keyid, homedir=gpg_home)
 
-  if metadata_directory is not None:
-    fn = os.path.join(metadata_directory, fn)
+    link_metadata.create_signature(signer)
+    fn = FILENAME_FORMAT.format(step_name=step_name, keyid=keyid)
 
-  LOG.info("Storing link metadata to '{}'...".format(fn))
-  link_metadata.dump(fn)
+    if metadata_directory is not None:
+        fn = os.path.join(metadata_directory, fn)
+
+    LOG.info("Storing link metadata to '{}'...".format(fn))
+    link_metadata.dump(fn)
+
+    LOG.info("Removing unfinished link metadata '{}'...".format(unfinished_fn))
+    os.remove(unfinished_fn)
+
+
+def in_toto_match_products(
+    link, paths=None, exclude_patterns=None, lstrip_paths=None
+):
+    """Check if local artifacts match products in passed link.
+
+    NOTE: Does not check integrity or authenticity of passed link!
+
+    Arguments:
+      link: The Link object to match.
+
+    See ``in_toto_run`` for details about arguments, and exceptions that may
+    occur while recording artifact hashes.
+
+    Returns:
+      A 3-tuple with artifact names that are
+      - only in products,
+      - not in products,
+      - have different hashes.
+    """
+    if paths is None:
+        paths = ["."]
+
+    artifacts = record_artifacts_as_dict(
+        paths, exclude_patterns=exclude_patterns, lstrip_paths=lstrip_paths
+    )
+
+    artifact_names = artifacts.keys()
+    product_names = link.products.keys()
+
+    only_products = product_names - artifact_names
+    not_in_products = artifact_names - product_names
+    differ = {
+        name
+        for name in product_names & artifact_names
+        if link.products[name] != artifacts[name]
+    }
 
-  LOG.info("Removing unfinished link metadata '{}'...".format(unfinished_fn))
-  os.remove(unfinished_fn)
+    return only_products, not_in_products, differ
```

### Comparing `in_toto-1.4.0/in_toto/settings.py` & `in_toto-2.0.0/in_toto/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,22 +21,16 @@
   Defaults can be changed,
    - here (hardcoded),
    - programmatically, e.g.
      ```
      import in_toto.settings
      in_toto.settings.ARTIFACT_BASE_PATH = "/home/user/project"
      ```
-  - or, when using in-toto via command line tooling, with environment variables
-    or RCfiles, see the `in_toto.user_settings` module
-
 """
 # The debug setting is used to set to the in-toto base logger to logging.DEBUG
-# TODO: This setting is currently not available via environment variables or
-# rcfiles, partially because at the moment it is read before we parse
-# envvars/rcfiles. Do we want to make it available to those as well?
 DEBUG = False
 
 # See docstring of `in-toto.record_artifacts_as_dict` for how this is used
 ARTIFACT_EXCLUDE_PATTERNS = ["*.link*", ".git", "*.pyc", "*~"]
 
 # Used as base path for --materials and --products arguments when running
 # in-toto-run/in-toto-record
```

### Comparing `in_toto-1.4.0/in_toto/verifylib.py` & `in_toto-2.0.0/in_toto/verifylib.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,1519 +21,1608 @@
   a software supply chain layout.
 
   Take a look at `in_toto_verify`'s docstring for more details about the
   entire verification workflow.
 
 """
 
-import os
 import datetime
-import iso8601
 import fnmatch
 import logging
-from dateutil import tz
+import os
 
+import iso8601
 import securesystemslib.exceptions
+import securesystemslib.formats
+from dateutil import tz
+from securesystemslib.gpg.exceptions import KeyExpirationError
 
-import in_toto.settings
-import in_toto.runlib
+import in_toto.formats
 import in_toto.models.layout
 import in_toto.models.link
-import in_toto.formats
-from in_toto.models.metadata import Metadata
-from in_toto.exceptions import (RuleVerificationError, LayoutExpiredError,
-    ThresholdVerificationError, BadReturnValueError,
-    SignatureVerificationError)
 import in_toto.rulelib
-
-import securesystemslib.formats
-from securesystemslib.gpg.exceptions import KeyExpirationError
+import in_toto.runlib
+import in_toto.settings
+from in_toto.exceptions import (
+    BadReturnValueError,
+    LayoutExpiredError,
+    RuleVerificationError,
+    SignatureVerificationError,
+    ThresholdVerificationError,
+)
+from in_toto.models.metadata import Metadata
 
 # Inherits from in_toto base logger (c.f. in_toto.log)
 LOG = logging.getLogger(__name__)
 
 RULE_TRACE = {}
 
 
 def _raise_on_bad_retval(return_value, command=None):
-  """
-  <Purpose>
-    Internal function that checks return values of shell commands, e.g. from
-    inspections. Raises exception if the passed value is non-int and non-zero.
-
-  <Arguments>
-    return_value:
-            The return value to be verified
-    command: (optional)
-            The command whose execution returned the value, used for exception
-            message.
-
-  <Exceptions>
-    BadReturnValueError if the return_value is non-int and non-zero
-
-  <Side Effects>
-    None.
-
-  <Returns>
-    None.
-  """
-
-  msg = "Got non-{what} " + "return value '{}'".format(return_value)
-  if command:
-    msg = "{0} from command '{1}'.".format(msg, command)
-  else:
-    msg = "{0}.".format(msg)
+    """
+    <Purpose>
+      Internal function that checks return values of shell commands, e.g. from
+      inspections. Raises exception if the passed value is non-int and non-zero.
+
+    <Arguments>
+      return_value:
+              The return value to be verified
+      command: (optional)
+              The command whose execution returned the value, used for exception
+              message.
+
+    <Exceptions>
+      BadReturnValueError if the return_value is non-int and non-zero
+
+    <Side Effects>
+      None.
+
+    <Returns>
+      None.
+    """
+
+    msg = "Got non-{what} " + "return value '{}'".format(return_value)
+    if command:
+        msg = "{0} from command '{1}'.".format(msg, command)
+    else:
+        msg = "{0}.".format(msg)
 
-  if not isinstance(return_value, int):
-    raise BadReturnValueError(msg.format(what="int"))
+    if not isinstance(return_value, int):
+        raise BadReturnValueError(msg.format(what="int"))
 
-  # TODO: in-toto specification suggests special behavior on
-  # return_value == 127, but does not fully define that behavior yet
+    # TODO: in-toto specification suggests special behavior on
+    # return_value == 127, but does not fully define that behavior yet
 
-  if return_value != 0:
-    raise BadReturnValueError(msg.format(what="zero"))
+    if return_value != 0:
+        raise BadReturnValueError(msg.format(what="zero"))
 
 
 def load_links_for_layout(layout, link_dir_path):
-  """
-  <Purpose>
-    Try to load all existing metadata files for each Step of the Layout
-    from the current directory.
-
-    For each step the metadata might consist of multiple (thresholds) Link
-    or Layout (sub-layouts) files.
-
-  <Arguments>
-    layout:
-          Layout object
-
-    link_dir_path:
-          A path to directory where links are loaded from
-
-
-  <Side Effects>
-    Calls function to read files from disk
-
-  <Exceptions>
-    in_toto.exceptions.LinkNotFoundError,
-            if fewer than `threshold` link files can be found for any given
-            step of the supply chain (preliminary threshold check)
-
-  <Returns>
-    A dictionary carrying all the found metadata corresponding to the
-    passed layout, e.g.:
-
-    {
-      <step name> : {
-        <functionary key id> : <Metadata containing a Link or Layout object>,
-        ...
-      }, ...
-    }
-
-
-  """
-  steps_metadata = {}
-
-  # Iterate over all the steps in the layout
-  for step in layout.steps:
-    links_per_step = {}
-
-    # We try to load a link for every authorized functionary, but don't fail
-    # if the file does not exist (authorized != required)
-    # FIXME: Should we really pass on IOError, or just skip inexistent links?
-    for authorized_keyid in step.pubkeys:
-      # Iterate over the authorized key and if present over subkeys
-      for keyid in [authorized_keyid] + list(layout.keys.get(authorized_keyid,
-          {}).get("subkeys", {}).keys()):
-
-        filename = in_toto.models.link.FILENAME_FORMAT.format(
-            step_name=step.name, keyid=keyid)
-        filepath = os.path.join(link_dir_path, filename)
-
-        try:
-          metadata = Metadata.load(filepath)
-          links_per_step[keyid] = metadata
+    """
+    <Purpose>
+      Try to load all existing metadata files for each Step of the Layout
+      from the current directory.
+
+      For each step the metadata might consist of multiple (thresholds) Link
+      or Layout (sub-layouts) files.
+
+    <Arguments>
+      layout:
+            Layout object
+
+      link_dir_path:
+            A path to directory where links are loaded from
+
+
+    <Side Effects>
+      Calls function to read files from disk
+
+    <Exceptions>
+      in_toto.exceptions.LinkNotFoundError,
+              if fewer than `threshold` link files can be found for any given
+              step of the supply chain (preliminary threshold check)
+
+    <Returns>
+      A dictionary carrying all the found metadata corresponding to the
+      passed layout, e.g.:
+
+      {
+        <step name> : {
+          <functionary key id> : <Metadata containing a Link or Layout object>,
+          ...
+        }, ...
+      }
+
+
+    """
+    steps_metadata = {}
+
+    # Iterate over all the steps in the layout
+    for step in layout.steps:
+        links_per_step = {}
+
+        # We try to load a link for every authorized functionary, but don't fail
+        # if the file does not exist (authorized != required)
+        # FIXME: Should we really pass on IOError, or just skip inexistent links?
+        for authorized_keyid in step.pubkeys:
+            # Iterate over the authorized key and if present over subkeys
+            for keyid in [authorized_keyid] + list(
+                layout.keys.get(authorized_keyid, {}).get("subkeys", {}).keys()
+            ):
+                filename = in_toto.models.link.FILENAME_FORMAT.format(
+                    step_name=step.name, keyid=keyid
+                )
+                filepath = os.path.join(link_dir_path, filename)
+
+                try:
+                    metadata = Metadata.load(filepath)
+                    links_per_step[keyid] = metadata
+
+                except IOError:
+                    pass
+
+        # This is only a preliminary threshold check, based on (authorized)
+        # filenames, to fail early. A more thorough signature-based threshold
+        # check is indispensable.
+        if len(links_per_step) < step.threshold:
+            raise in_toto.exceptions.LinkNotFoundError(
+                "Step '{0}' requires '{1}'"
+                " link metadata file(s), found '{2}'.".format(
+                    step.name, step.threshold, len(links_per_step)
+                )
+            )
 
-        except IOError:
-          pass
+        steps_metadata[step.name] = links_per_step
 
-    # This is only a preliminary threshold check, based on (authorized)
-    # filenames, to fail early. A more thorough signature-based threshold
-    # check is indispensable.
-    if len(links_per_step) < step.threshold:
-      raise in_toto.exceptions.LinkNotFoundError("Step '{0}' requires '{1}'"
-          " link metadata file(s), found '{2}'."
-          .format(step.name, step.threshold, len(links_per_step)))
-
-    steps_metadata[step.name] = links_per_step
-
-  return steps_metadata
+    return steps_metadata
 
 
 def run_all_inspections(layout, persist_inspection_links):
-  """
-  <Purpose>
-    Extracts all inspections from a passed Layout's inspect field and
-    iteratively runs each command defined in the Inspection's `run` field using
-    `runlib.in_toto_run`, which returns a Link object.
-
-    If a link command returns non-zero the verification is aborted.
-
-  <Arguments>
-    layout:
-            A Layout object which is used to extract the Inspections.
-
-    persist_inspection_links:
-            A boolean indicating whether link metadata files for inspection
-            are written to cwd.
-
-  <Exceptions>
-    Calls function that raises BadReturnValueError if an inspection returned
-    non-int or non-zero.
-
-  <Returns>
-    A dictionary of metadata about the executed inspections, e.g.:
-
-    {
-      <inspection name> : {
-        <Link object>,
-        ...
-      }, ...
-    }
-
-  """
-  inspection_links_dict = {}
-  for inspection in layout.inspect:
-    LOG.info("Executing command for inspection '{}'...".format(
-        inspection.name))
-
-    # FIXME: We don't want to use the base path for runlib so we patch this
-    # for now. This will not stay!
-    base_path_backup = in_toto.settings.ARTIFACT_BASE_PATH
-    in_toto.settings.ARTIFACT_BASE_PATH = None
-
-    # FIXME: What should we record as material/product?
-    # Is the current directory a sensible default? In general?
-    # If so, we should probably make it a default in run_link
-    # We could use artifact rule paths.
-    material_list = product_list = ["."]
-    link = in_toto.runlib.in_toto_run(inspection.name, material_list,
-        product_list, inspection.run)
-
-    _raise_on_bad_retval(
-        link.signed.byproducts.get("return-value"),
-        inspection.run)
-
-    inspection_links_dict[inspection.name] = link.signed
-
-    # If client requests persistent inspection links,
-    # Dump the inspection link file for auditing
-    # Keep in mind that this pollutes the verifier's (client's) filesystem.
-    if persist_inspection_links:
-      filename = in_toto.models.link.FILENAME_FORMAT_SHORT.format(
-          step_name=inspection.name)
-      link.dump(filename)
+    """
+    <Purpose>
+      Extracts all inspections from a passed Layout's inspect field and
+      iteratively runs each command defined in the Inspection's `run` field using
+      `runlib.in_toto_run`, which returns a Link object.
+
+      If a link command returns non-zero the verification is aborted.
+
+    <Arguments>
+      layout:
+              A Layout object which is used to extract the Inspections.
+
+      persist_inspection_links:
+              A boolean indicating whether link metadata files for inspection
+              are written to cwd.
+
+    <Exceptions>
+      Calls function that raises BadReturnValueError if an inspection returned
+      non-int or non-zero.
+
+    <Returns>
+      A dictionary of metadata about the executed inspections, e.g.:
+
+      {
+        <inspection name> : {
+          <Link object>,
+          ...
+        }, ...
+      }
+
+    """
+    inspection_links_dict = {}
+    for inspection in layout.inspect:
+        LOG.info(
+            "Executing command for inspection '{}'...".format(inspection.name)
+        )
+
+        # FIXME: We don't want to use the base path for runlib so we patch this
+        # for now. This will not stay!
+        base_path_backup = in_toto.settings.ARTIFACT_BASE_PATH
+        in_toto.settings.ARTIFACT_BASE_PATH = None
+
+        # FIXME: What should we record as material/product?
+        # Is the current directory a sensible default? In general?
+        # If so, we should probably make it a default in run_link
+        # We could use artifact rule paths.
+        material_list = product_list = ["."]
+        link = in_toto.runlib.in_toto_run(
+            inspection.name, material_list, product_list, inspection.run
+        )
+
+        _raise_on_bad_retval(
+            link.signed.byproducts.get("return-value"), inspection.run
+        )
+
+        inspection_links_dict[inspection.name] = link.signed
+
+        # If client requests persistent inspection links,
+        # Dump the inspection link file for auditing
+        # Keep in mind that this pollutes the verifier's (client's) filesystem.
+        if persist_inspection_links:
+            filename = in_toto.models.link.FILENAME_FORMAT_SHORT.format(
+                step_name=inspection.name
+            )
+            link.dump(filename)
 
-    in_toto.settings.ARTIFACT_BASE_PATH = base_path_backup
+        in_toto.settings.ARTIFACT_BASE_PATH = base_path_backup
 
-  return inspection_links_dict
+    return inspection_links_dict
 
 
 def verify_layout_expiration(layout):
-  """
-  <Purpose>
-    Raises an exception if the passed layout has expired, i.e. if its
-    `expires` property is lesser "now".
-    Time zone aware datetime objects in UTC+00:00 (Zulu Time) are used.
-
-  <Arguments>
-    layout:
-            The Layout object to be verified.
-
-  <Exceptions>
-    LayoutExpiredError
-    TBA (see https://github.com/in-toto/in-toto/issues/6)
-
-  <Side Effects>
-    None.
-
-  """
-  expire_datetime = iso8601.parse_date(layout.expires)
-  if expire_datetime < datetime.datetime.now(tz.tzutc()):
-    raise LayoutExpiredError("Layout expired")
+    """
+    <Purpose>
+      Raises an exception if the passed layout has expired, i.e. if its
+      `expires` property is lesser "now".
+      Time zone aware datetime objects in UTC+00:00 (Zulu Time) are used.
+
+    <Arguments>
+      layout:
+              The Layout object to be verified.
+
+    <Exceptions>
+      LayoutExpiredError
+      TBA (see https://github.com/in-toto/in-toto/issues/6)
+
+    <Side Effects>
+      None.
+
+    """
+    expire_datetime = iso8601.parse_date(layout.expires)
+    if expire_datetime < datetime.datetime.now(tz.tzutc()):
+        raise LayoutExpiredError("Layout expired")
 
 
 def substitute_parameters(layout, parameter_dictionary):
-  """
-  <Purpose>
-    This function is a transitionary measure for parameter substitution (or
-    any other solution defined by the in-toto team). As of now, it acts as
-    a very simple replacement layer for python-like parameters
-
-  <Arguments>
-    layout:
-            The Layout object to process.
-
-      parameter_dictionary:
-            A dictionary containing key-value pairs for substitution.
-
-  <Exceptions>
-    securesystemslib.exceptions.FormatError:
-      if the parameter dictionary is malformed.
-
-    KeyError:
-      if one of the keys in the parameter dictionary are not present for
-      substitution
-
-  <Side Effects>
-    The layout object will have any tags replaced with the corresponding
-    values defined in the parameter dictionary.
-  """
-  in_toto.formats.PARAMETER_DICTIONARY_SCHEMA.check_match(parameter_dictionary)
-
-  for step in layout.steps:
-
-    new_material_rules = []
-    for rule in step.expected_materials:
-      new_rule = []
-      for stanza in rule:
-        new_rule.append(stanza.format(**parameter_dictionary))
-      new_material_rules.append(new_rule)
-
-    new_product_rules = []
-    for rule in step.expected_products:
-      new_rule = []
-      for stanza in rule:
-        new_rule.append(stanza.format(**parameter_dictionary))
-      new_product_rules.append(new_rule)
-
-    new_expected_command = []
-    for argv in step.expected_command:
-      new_expected_command.append(argv.format(**parameter_dictionary))
-
-    step.expected_command = new_expected_command
-    step.expected_materials = new_material_rules
-    step.expected_products = new_product_rules
-
-  for inspection in layout.inspect:
-    new_material_rules = []
-    for rule in inspection.expected_materials:
-      new_rule = []
-      for stanza in rule:
-        new_rule.append(stanza.format(**parameter_dictionary))
-      new_material_rules.append(new_rule)
-
-    new_product_rules = []
-    for rule in inspection.expected_products:
-      new_rule = []
-      for stanza in rule:
-        new_rule.append(stanza.format(**parameter_dictionary))
-      new_product_rules.append(new_rule)
-
-    new_run = []
-    for argv in inspection.run:
-      new_run.append(argv.format(**parameter_dictionary))
-
-    inspection.run = new_run
-    inspection.expected_materials = new_material_rules
-    inspection.expected_products = new_product_rules
-
+    """
+    <Purpose>
+      This function is a transitionary measure for parameter substitution (or
+      any other solution defined by the in-toto team). As of now, it acts as
+      a very simple replacement layer for python-like parameters
+
+    <Arguments>
+      layout:
+              The Layout object to process.
+
+        parameter_dictionary:
+              A dictionary containing key-value pairs for substitution.
+
+    <Exceptions>
+      securesystemslib.exceptions.FormatError:
+        if the parameter dictionary is malformed.
+
+      KeyError:
+        if one of the keys in the parameter dictionary are not present for
+        substitution
+
+    <Side Effects>
+      The layout object will have any tags replaced with the corresponding
+      values defined in the parameter dictionary.
+    """
+    in_toto.formats.PARAMETER_DICTIONARY_SCHEMA.check_match(
+        parameter_dictionary
+    )
+
+    for step in layout.steps:
+        new_material_rules = []
+        for rule in step.expected_materials:
+            new_rule = []
+            for stanza in rule:
+                new_rule.append(stanza.format(**parameter_dictionary))
+            new_material_rules.append(new_rule)
+
+        new_product_rules = []
+        for rule in step.expected_products:
+            new_rule = []
+            for stanza in rule:
+                new_rule.append(stanza.format(**parameter_dictionary))
+            new_product_rules.append(new_rule)
+
+        new_expected_command = []
+        for argv in step.expected_command:
+            new_expected_command.append(argv.format(**parameter_dictionary))
+
+        step.expected_command = new_expected_command
+        step.expected_materials = new_material_rules
+        step.expected_products = new_product_rules
+
+    for inspection in layout.inspect:
+        new_material_rules = []
+        for rule in inspection.expected_materials:
+            new_rule = []
+            for stanza in rule:
+                new_rule.append(stanza.format(**parameter_dictionary))
+            new_material_rules.append(new_rule)
+
+        new_product_rules = []
+        for rule in inspection.expected_products:
+            new_rule = []
+            for stanza in rule:
+                new_rule.append(stanza.format(**parameter_dictionary))
+            new_product_rules.append(new_rule)
+
+        new_run = []
+        for argv in inspection.run:
+            new_run.append(argv.format(**parameter_dictionary))
+
+        inspection.run = new_run
+        inspection.expected_materials = new_material_rules
+        inspection.expected_products = new_product_rules
 
 
 def verify_metadata_signatures(metadata, keys_dict):
-  """
-  <Purpose>
-    Iteratively verifies the signatures of a Metadata object containing
-    a Layout object for every verification key in the passed keys dictionary.
-
-    Requires at least one key to be passed and requires every passed key to
-    find a valid signature.
-
-  <Arguments>
-    metadata:
-            A Metadata object containing a Layout whose signatures are
-            verified.
-
-    keys_dict:
-            A dictionary of keys to verify the signatures conformant with
-            securesystemslib.formats.VERIFICATION_KEY_DICT_SCHEMA.
-
-  <Exceptions>
-    securesystemslib.exceptions.FormatError
-      if the passed key dict does not match VERIFICATION_KEY_DICT_SCHEMA.
-
-    SignatureVerificationError
-      if an empty verification key dictionary was passed, or
-      if any of the passed verification keys fails to verify a signature.
-
-    securesystemslib.gpg.exceptions.KeyExpirationError:
-      if any of the passed verification keys is an expired gpg key
-
-  """
-  securesystemslib.formats.VERIFICATION_KEY_DICT_SCHEMA.check_match(keys_dict)
-
-  # Fail if an empty verification key dictionary was passed
-  if len(keys_dict) < 1:
-    raise SignatureVerificationError("Layout signature verification"
-        " requires at least one key.")
-
-  # Fail if any of the passed keys can't verify a signature on the Layout
-  for junk, verify_key in keys_dict.items():
-    metadata.verify_signature(verify_key)
+    """
+    <Purpose>
+      Iteratively verifies the signatures of a Metadata object containing
+      a Layout object for every verification key in the passed keys dictionary.
+
+      Requires at least one key to be passed and requires every passed key to
+      find a valid signature.
+
+    <Arguments>
+      metadata:
+              A Metadata object containing a Layout whose signatures are
+              verified.
+
+      keys_dict:
+              A dictionary of keys to verify the signatures conformant with
+              securesystemslib.formats.VERIFICATION_KEY_DICT_SCHEMA.
+
+    <Exceptions>
+      securesystemslib.exceptions.FormatError
+        if the passed key dict does not match VERIFICATION_KEY_DICT_SCHEMA.
+
+      SignatureVerificationError
+        if an empty verification key dictionary was passed, or
+        if any of the passed verification keys fails to verify a signature.
+
+      securesystemslib.gpg.exceptions.KeyExpirationError:
+        if any of the passed verification keys is an expired gpg key
+
+    """
+    securesystemslib.formats.VERIFICATION_KEY_DICT_SCHEMA.check_match(keys_dict)
+
+    # Fail if an empty verification key dictionary was passed
+    if len(keys_dict) < 1:
+        raise SignatureVerificationError(
+            "Layout signature verification requires at least one key."
+        )
+
+    # Fail if any of the passed keys can't verify a signature on the Layout
+    for junk, verify_key in keys_dict.items():
+        metadata.verify_signature(verify_key)
 
 
 def verify_link_signature_thresholds(layout, steps_metadata):
-  """
-  <Purpose>
-    Verify that for each step of the layout there are at least `threshold`
-    links metadata, signed by different authorized functionaries and return the
-    verified link metadata dictionary containing only authorized links metadata
-    whose signatures were successfully verified.
-
-    NOTE: If the layout's key store (`layout.keys`) lists a (master) key `K`,
-    with a subkey `K'`, then `K'` is authorized implicitly, to sign any link
-    that `K` is authorized to sign. In other words, the trust in a master key
-    extends to the trust in a subkey. The inverse is not true.
-
-  <Arguments>
-    layout:
-            A Layout object whose Steps are extracted and verified.
-
-    steps_metadata:
-            A dictionary containing link metadata per functionary per step,
-            e.g.:
-            {
-              <link name> : {
-                <functionary key id> : <Metadata containing a Link or Layout
-                                        object>,
-                ...
-              }, ...
-            }
+    """
+    <Purpose>
+      Verify that for each step of the layout there are at least `threshold`
+      links metadata, signed by different authorized functionaries and return the
+      verified link metadata dictionary containing only authorized links metadata
+      whose signatures were successfully verified.
+
+      NOTE: If the layout's key store (`layout.keys`) lists a (master) key `K`,
+      with a subkey `K'`, then `K'` is authorized implicitly, to sign any link
+      that `K` is authorized to sign. In other words, the trust in a master key
+      extends to the trust in a subkey. The inverse is not true.
+
+    <Arguments>
+      layout:
+              A Layout object whose Steps are extracted and verified.
+
+      steps_metadata:
+              A dictionary containing link metadata per functionary per step,
+              e.g.:
+              {
+                <link name> : {
+                  <functionary key id> : <Metadata containing a Link or Layout
+                                          object>,
+                  ...
+                }, ...
+              }
+
+    <Exceptions>
+      ThresholdVerificationError
+              If any of the steps of the passed layout does not have enough
+              (`step.threshold`) links signed by different authorized
+              functionaries.
+
+    <Returns>
+      A steps_metadata containing only links with valid signatures created by
+      authorized functionaries.
+
+    """
+    # Create an inverse keys-subkeys dictionary, with subkey keyids as
+    # dictionary keys and main keys as dictionary values. This will be
+    # required below to assess main-subkey trust delegations.
+    # We assume that a given subkey can only belong to one master key
+    # TODO: Is this a safe assumption? Should we assert for it?
+    main_keys_for_subkeys = {}
+    for main_key in list(layout.keys.values()):
+        for sub_keyid in main_key.get("subkeys", []):
+            main_keys_for_subkeys[sub_keyid] = main_key
+
+    # Dict for valid and authorized links of all steps of the layout
+    verified_steps_metadata = {}
+
+    # For each step of the layout check the signatures of corresponding links.
+    # Consider only links where the signature is valid and keys are authorized,
+    # and discard others.
+    # Only count one of multiple links signed with different subkeys of a main
+    # key towards link threshold.
+    # Only proceed with final product verification if threshold requirements are
+    # fulfilled.
+    for step in layout.steps:
+        # Dict for valid and authorized links of a given step
+        verified_key_link_dict = {}
+        # List of used keyids
+        used_main_keyids = []
+
+        # Do per step link threshold verification
+        for link_keyid, link in steps_metadata.get(step.name, {}).items():
+            # Iterate over authorized keyids to find a key or subkey corresponding
+            # to the given link and check if the link's keyid is authorized.
+            # Subkeys of authorized main keys are authorized implicitly.
+            for authorized_keyid in step.pubkeys:
+                authorized_key = layout.keys.get(authorized_keyid)
+                main_key_for_subkey = main_keys_for_subkeys.get(
+                    authorized_keyid
+                )
+
+                # The signing key is authorized ...
+                if authorized_key and link_keyid == authorized_keyid:
+                    verification_key = authorized_key
+                    break
+
+                # ... or the signing key is an authorized subkey ...
+                if main_key_for_subkey and link_keyid == authorized_keyid:
+                    verification_key = main_key_for_subkey
+                    break
+
+                # ... or the signing key is a subkey of an authorized key
+                if (
+                    authorized_key
+                    and link_keyid in authorized_key.get("subkeys", {}).keys()
+                ):
+                    verification_key = authorized_key
+                    break
+
+            else:
+                LOG.info(
+                    "Skipping link. Keyid '{0}' is not authorized to sign links"
+                    " for step '{1}'".format(link_keyid, step.name)
+                )
+                continue
+
+            # Verify signature and skip invalidly signed links
+            try:
+                link.verify_signature(verification_key)
+
+            except SignatureVerificationError:
+                LOG.info(
+                    "Skipping link. Broken link signature with keyid '{0}'"
+                    " for step '{1}'".format(link_keyid, step.name)
+                )
+                continue
+
+            except KeyExpirationError as e:
+                LOG.info("Skipping link. {}".format(e))
+                continue
+
+            # Warn if there are links signed by different subkeys of same main key
+            if verification_key["keyid"] in used_main_keyids:
+                LOG.warning(
+                    "Found links signed by different subkeys of the same main"
+                    " key '{}' for step '{}'. Only one of them is counted towards the"
+                    " step threshold.".format(
+                        verification_key["keyid"], step.name
+                    )
+                )
+
+            used_main_keyids.append(verification_key["keyid"])
+
+            # Keep only links with valid and authorized signature
+            verified_key_link_dict[link_keyid] = link
+
+        # For each step, verify that we have enough validly signed links from
+        # distinct authorized functionaries. Links signed by different subkeys of
+        # the same main key are counted only once towards the threshold.
+        valid_authorized_links_cnt = len(set(used_main_keyids))
+        # TODO: To guarantee that links are signed by different functionaries
+        # we rely on the layout to not carry duplicate verification keys under
+        # different dictionary keys, e.g. {keyid1: KEY1, keyid2: KEY1}
+        # Maybe we should add such a check to the layout validation? Or here?
+        if valid_authorized_links_cnt < step.threshold:
+            raise ThresholdVerificationError(
+                "Step '{}' requires at least '{}' links"
+                " validly signed by different authorized functionaries. Only"
+                " found '{}'".format(
+                    step.name, step.threshold, valid_authorized_links_cnt
+                )
+            )
+
+        # Add all good links of this step to the dictionary of links of all steps
+        verified_steps_metadata[step.name] = verified_key_link_dict
+
+    # Threshold verification succeeded, return valid and authorized links for
+    # further verification
+    return verified_steps_metadata
 
-  <Exceptions>
-    ThresholdVerificationError
-            If any of the steps of the passed layout does not have enough
-            (`step.threshold`) links signed by different authorized
-            functionaries.
-
-  <Returns>
-    A steps_metadata containing only links with valid signatures created by
-    authorized functionaries.
-
-  """
-  # Create an inverse keys-subkeys dictionary, with subkey keyids as
-  # dictionary keys and main keys as dictionary values. This will be
-  # required below to assess main-subkey trust delegations.
-  # We assume that a given subkey can only belong to one master key
-  # TODO: Is this a safe assumption? Should we assert for it?
-  main_keys_for_subkeys = {}
-  for main_key in list(layout.keys.values()):
-    for sub_keyid in main_key.get("subkeys", []):
-      main_keys_for_subkeys[sub_keyid] = main_key
-
-  # Dict for valid and authorized links of all steps of the layout
-  verified_steps_metadata = {}
-
-  # For each step of the layout check the signatures of corresponding links.
-  # Consider only links where the signature is valid and keys are authorized,
-  # and discard others.
-  # Only count one of multiple links signed with different subkeys of a main
-  # key towards link threshold.
-  # Only proceed with final product verification if threshold requirements are
-  # fulfilled.
-  for step in layout.steps:
-    # Dict for valid and authorized links of a given step
-    verified_key_link_dict = {}
-    # List of used keyids
-    used_main_keyids = []
-
-    # Do per step link threshold verification
-    for link_keyid, link in steps_metadata.get(step.name, {}).items():
-      # Iterate over authorized keyids to find a key or subkey corresponding
-      # to the given link and check if the link's keyid is authorized.
-      # Subkeys of authorized main keys are authorized implicitly.
-      for authorized_keyid in step.pubkeys:
-
-        authorized_key = layout.keys.get(authorized_keyid)
-        main_key_for_subkey = main_keys_for_subkeys.get(authorized_keyid)
-
-        # The signing key is authorized ...
-        if authorized_key and link_keyid == authorized_keyid:
-          verification_key = authorized_key
-          break
-
-        # ... or the signing key is an authorized subkey ...
-        if main_key_for_subkey and link_keyid == authorized_keyid:
-          verification_key = main_key_for_subkey
-          break
-
-        # ... or the signing key is a subkey of an authorized key
-        if (authorized_key and
-            link_keyid in authorized_key.get("subkeys", {}).keys()):
-          verification_key = authorized_key
-          break
-
-      else:
-        LOG.info("Skipping link. Keyid '{0}' is not authorized to sign links"
-            " for step '{1}'".format(link_keyid, step.name))
-        continue
-
-      # Verify signature and skip invalidly signed links
-      try:
-        link.verify_signature(verification_key)
-
-      except SignatureVerificationError:
-        LOG.info("Skipping link. Broken link signature with keyid '{0}'"
-            " for step '{1}'".format(link_keyid, step.name))
-        continue
-
-      except KeyExpirationError as e:
-        LOG.info("Skipping link. {}".format(e))
-        continue
-
-      # Warn if there are links signed by different subkeys of same main key
-      if verification_key["keyid"] in used_main_keyids:
-        LOG.warning("Found links signed by different subkeys of the same main"
-            " key '{}' for step '{}'. Only one of them is counted towards the"
-            " step threshold.".format(verification_key["keyid"], step.name))
-
-      used_main_keyids.append(verification_key["keyid"])
-
-      # Keep only links with valid and authorized signature
-      verified_key_link_dict[link_keyid] = link
-
-    # For each step, verify that we have enough validly signed links from
-    # distinct authorized functionaries. Links signed by different subkeys of
-    # the same main key are counted only once towards the threshold.
-    valid_authorized_links_cnt = len(set(used_main_keyids))
-    # TODO: To guarantee that links are signed by different functionaries
-    # we rely on the layout to not carry duplicate verification keys under
-    # different dictionary keys, e.g. {keyid1: KEY1, keyid2: KEY1}
-    # Maybe we should add such a check to the layout validation? Or here?
-    if valid_authorized_links_cnt < step.threshold:
-      raise ThresholdVerificationError("Step '{}' requires at least '{}' links"
-          " validly signed by different authorized functionaries. Only"
-          " found '{}'".format(step.name, step.threshold,
-          valid_authorized_links_cnt))
-
-    # Add all good links of this step to the dictionary of links of all steps
-    verified_steps_metadata[step.name] = verified_key_link_dict
-
-  # Threshold verification succeeded, return valid and authorized links for
-  # further verification
-  return verified_steps_metadata
 
 def verify_command_alignment(command, expected_command):
-  """
-  <Purpose>
-    Checks if a run command aligns with an expected command. The commands align
-    if all of their elements are equal. If alignment fails, a warning is
-    printed.
-
-    Note:
-      Command alignment is a weak guarantee. Because a functionary can easily
-      alias commands.
-
-  <Arguments>
-    command:
-            A command list, e.g. ["vi", "foo.py"]
-    expected_command:
-            A command list, e.g. ["make", "install"]
-
-  <Exceptions>
-    None.
-
-  <Side Effects>
-    Logs warning in case commands do not align.
-
-  """
-  # In what case command alignment should fail and how that failure should be
-  # propagated has been thoughly discussed in:
-  # https://github.com/in-toto/in-toto/issues/46 and
-  # https://github.com/in-toto/in-toto/pull/47
-  # We chose the simplest solution for now, i.e. Warn if they do not align.
-  if command != expected_command:
-    LOG.warning("Run command '{0}' differs from expected command '{1}'"
-        .format(command, expected_command))
+    """
+    <Purpose>
+      Checks if a run command aligns with an expected command. The commands align
+      if all of their elements are equal. If alignment fails, a warning is
+      printed.
+
+      Note:
+        Command alignment is a weak guarantee. Because a functionary can easily
+        alias commands.
+
+    <Arguments>
+      command:
+              A command list, e.g. ["vi", "foo.py"]
+      expected_command:
+              A command list, e.g. ["make", "install"]
+
+    <Exceptions>
+      None.
+
+    <Side Effects>
+      Logs warning in case commands do not align.
+
+    """
+    # In what case command alignment should fail and how that failure should be
+    # propagated has been thoughly discussed in:
+    # https://github.com/in-toto/in-toto/issues/46 and
+    # https://github.com/in-toto/in-toto/pull/47
+    # We chose the simplest solution for now, i.e. Warn if they do not align.
+    if command != expected_command:
+        LOG.warning(
+            "Run command '{0}' differs from expected command '{1}'".format(
+                command, expected_command
+            )
+        )
 
 
 def verify_all_steps_command_alignment(layout, chain_link_dict):
-  """
-  <Purpose>
-    Iteratively checks if all expected commands as defined in the
-    Steps of a Layout align with the actual commands as recorded in the Link
-    metadata.
-
-  <Arguments>
-    layout:
-            A Layout object to extract the expected commands from.
-
-    chain_link_dict:
-            A dictionary containing link metadata per functionary per step,
-            e.g.:
-            {
-              <link name> : {
-                <functionary key id> : <Link object>,
-                ...
-              }, ...
-            }
+    """
+    <Purpose>
+      Iteratively checks if all expected commands as defined in the
+      Steps of a Layout align with the actual commands as recorded in the Link
+      metadata.
+
+    <Arguments>
+      layout:
+              A Layout object to extract the expected commands from.
+
+      chain_link_dict:
+              A dictionary containing link metadata per functionary per step,
+              e.g.:
+              {
+                <link name> : {
+                  <functionary key id> : <Link object>,
+                  ...
+                }, ...
+              }
+
+    <Exceptions>
+      None.
+
+    <Side Effects>
+      None.
+
+    """
+    for step in layout.steps:
+        # Find the according link for this step
+        expected_command = step.expected_command
+        key_link_dict = chain_link_dict[step.name]
+
+        # FIXME: I think we could do this for one link per step only
+        # providing that we verify command alignment AFTER threshold equality
+        for keyid, link in key_link_dict.items():
+            LOG.info(
+                "Verifying command alignment for '{0}'...".format(
+                    in_toto.models.link.FILENAME_FORMAT.format(
+                        step_name=step.name, keyid=keyid
+                    )
+                )
+            )
 
-  <Exceptions>
-    None.
+            command = link.command
+            verify_command_alignment(command, expected_command)
 
-  <Side Effects>
-    None.
 
-  """
-  for step in layout.steps:
-    # Find the according link for this step
-    expected_command = step.expected_command
-    key_link_dict = chain_link_dict[step.name]
-
-    # FIXME: I think we could do this for one link per step only
-    # providing that we verify command alignment AFTER threshold equality
-    for keyid, link in key_link_dict.items():
-      LOG.info("Verifying command alignment for '{0}'...".format(
-          in_toto.models.link.FILENAME_FORMAT.format(step_name=step.name,
-              keyid=keyid)))
+def verify_match_rule(rule_data, artifacts_queue, source_artifacts, links):
+    """
+    <Purpose>
+      Filters artifacts from artifact queue using rule pattern and optional rule
+      source prefix and consumes them if there is a corresponding destination
+      artifact, filtered using the same rule pattern and an optional rule
+      destination prefix, and source and destination artifacts have matching
+      hashes.
+
+      NOTE: The destination artifacts are extracted from the links dictionary,
+      using destination name and destination type from the rule data. The source
+      artifacts could also be extracted from the links dictionary, but would
+      require the caller to pass source name and source type, as those are not
+      encoded in the rule. However, we choose to let the caller directly pass the
+      relevant artifacts.
+
+
+    <Arguments>
+      rule_data:
+              An unpacked "MATCH" rule (see in_toto.rulelib).
+
+      artifacts_queue:
+              Not yet consumed artifacts (paths only).
+
+
+      source_artifacts:
+              All artifacts of the source item (including hashes).
+
+      links:
+              A dictionary containing link metadata per step or inspection, e.g.:
+              {
+                <link name> : <Link object>,
+                ...
+              }
 
-      command = link.command
-      verify_command_alignment(command, expected_command)
+    <Exceptions>
+      None.
 
+    <Side Effects>
+      None.
 
-def verify_match_rule(rule_data, artifacts_queue, source_artifacts, links):
-  """
-  <Purpose>
-    Filters artifacts from artifact queue using rule pattern and optional rule
-    source prefix and consumes them if there is a corresponding destination
-    artifact, filtered using the same rule pattern and an optional rule
-    destination prefix, and source and destination artifacts have matching
-    hashes.
-
-    NOTE: The destination artifacts are extracted from the links dictionary,
-    using destination name and destination type from the rule data. The source
-    artifacts could also be extracted from the links dictionary, but would
-    require the caller to pass source name and source type, as those are not
-    encoded in the rule. However, we choose to let the caller directly pass the
-    relevant artifacts.
-
-
-  <Arguments>
-    rule_data:
-            An unpacked "MATCH" rule (see in_toto.rulelib).
-
-    artifacts_queue:
-            Not yet consumed artifacts (paths only).
-
-
-    source_artifacts:
-            All artifacts of the source item (including hashes).
-
-    links:
-            A dictionary containing link metadata per step or inspection, e.g.:
-            {
-              <link name> : <Link object>,
-              ...
-            }
-
-  <Exceptions>
-    None.
-
-  <Side Effects>
-    None.
-
-  <Returns>
-    The set of consumed artifacts (paths only).
-
-  """
-  consumed = set()
-
-  # The rule can only consume artifacts if the destination link exists
-  dest_link = links.get(rule_data["dest_name"])
-  if not dest_link:
-    return consumed
+    <Returns>
+      The set of consumed artifacts (paths only).
 
-  # Extract destination artifacts from destination link
-  dest_artifacts = getattr(dest_link, rule_data["dest_type"])
+    """
+    consumed = set()
 
-  # Filter part 1 - Filter artifacts using optional source prefix, and subtract
-  # prefix before filtering with rule pattern (see filter part 2) to prevent
-  # globbing in the prefix.
-  if rule_data["source_prefix"]:
-    filtered_source_paths = []
-    # Add trailing slash to source prefix if it does not exist
-    normalized_source_prefix = os.path.join(
-        rule_data["source_prefix"], "").replace("\\", "/")
-
-    for artifact_path in artifacts_queue:
-      if artifact_path.startswith(normalized_source_prefix):
-        filtered_source_paths.append(
-            artifact_path[len(normalized_source_prefix):])
-
-  else:
-    filtered_source_paths = artifacts_queue
-
-  # Filter part 2 - glob above filtered artifact paths
-  filtered_source_paths = fnmatch.filter(
-      filtered_source_paths, rule_data["pattern"])
-
-  # Iterate over filtered source paths and try to match the corresponding
-  # source artifact hash with the corresponding destination artifact hash
-  for path in filtered_source_paths:
-    # If a source prefix was specified, we subtracted the prefix above before
-    # globbing. We have to re-prepend the prefix in order to retrieve the
-    # corresponding source artifact below.
+    # The rule can only consume artifacts if the destination link exists
+    dest_link = links.get(rule_data["dest_name"])
+    if not dest_link:
+        return consumed
+
+    # Extract destination artifacts from destination link
+    dest_artifacts = getattr(dest_link, rule_data["dest_type"])
+
+    # Filter part 1 - Filter artifacts using optional source prefix, and subtract
+    # prefix before filtering with rule pattern (see filter part 2) to prevent
+    # globbing in the prefix.
     if rule_data["source_prefix"]:
-      full_source_path = os.path.join(
-          rule_data["source_prefix"], path).replace("\\", "/")
+        filtered_source_paths = []
+        # Add trailing slash to source prefix if it does not exist
+        normalized_source_prefix = os.path.join(
+            rule_data["source_prefix"], ""
+        ).replace("\\", "/")
+
+        for artifact_path in artifacts_queue:
+            if artifact_path.startswith(normalized_source_prefix):
+                filtered_source_paths.append(
+                    artifact_path[len(normalized_source_prefix) :]
+                )
 
     else:
-      full_source_path = path
+        filtered_source_paths = artifacts_queue
 
-    # If a destination prefix was specified, the destination artifact should
-    # be queried with the full destination path, i.e. the prefix joined with
-    # the globbed path.
-    if rule_data["dest_prefix"]:
-      full_dest_path = os.path.join(
-          rule_data["dest_prefix"], path).replace("\\", "/")
+    # Filter part 2 - glob above filtered artifact paths
+    filtered_source_paths = fnmatch.filter(
+        filtered_source_paths, rule_data["pattern"]
+    )
+
+    # Iterate over filtered source paths and try to match the corresponding
+    # source artifact hash with the corresponding destination artifact hash
+    for path in filtered_source_paths:
+        # If a source prefix was specified, we subtracted the prefix above before
+        # globbing. We have to re-prepend the prefix in order to retrieve the
+        # corresponding source artifact below.
+        if rule_data["source_prefix"]:
+            full_source_path = os.path.join(
+                rule_data["source_prefix"], path
+            ).replace("\\", "/")
+
+        else:
+            full_source_path = path
+
+        # If a destination prefix was specified, the destination artifact should
+        # be queried with the full destination path, i.e. the prefix joined with
+        # the globbed path.
+        if rule_data["dest_prefix"]:
+            full_dest_path = os.path.join(
+                rule_data["dest_prefix"], path
+            ).replace("\\", "/")
+
+        else:
+            full_dest_path = path
+
+        # Extract source artifact hash dict
+        # We know the source artifact is available, it is also in the queue
+        source_artifact = source_artifacts[full_source_path]
 
-    else:
-      full_dest_path = path
-
-    # Extract source artifact hash dict
-    # We know the source artifact is available, it is also in the queue
-    source_artifact = source_artifacts[full_source_path]
-
-    # Don't consume source artifact w/o corresponding dest artifact (by path)
-    try:
-      dest_artifact = dest_artifacts[full_dest_path]
-    except KeyError:
-      continue
-
-    # Don't consume source artifact w/o corresponding dest artifact (by hash)
-    if source_artifact != dest_artifact:
-      continue
+        # Don't consume source artifact w/o corresponding dest artifact (by path)
+        try:
+            dest_artifact = dest_artifacts[full_dest_path]
+        except KeyError:
+            continue
+
+        # Don't consume source artifact w/o corresponding dest artifact (by hash)
+        if source_artifact != dest_artifact:
+            continue
 
-    # Source and destination matched, consume artifact
-    consumed.add(full_source_path)
+        # Source and destination matched, consume artifact
+        consumed.add(full_source_path)
 
-  return consumed
+    return consumed
 
 
 def verify_create_rule(rule_pattern, artifacts_queue, materials, products):
-  """
-  <Purpose>
-    Filters artifacts from artifacts queue using rule pattern and consumes them
-    if they are not in the materials set but are in the products set, i.e.
-    were created.
+    """
+    <Purpose>
+      Filters artifacts from artifacts queue using rule pattern and consumes them
+      if they are not in the materials set but are in the products set, i.e.
+      were created.
 
-  <Arguments>
-    rule_pattern:
-            A "CREATE" rule pattern (see in_toto.rulelib).
+    <Arguments>
+      rule_pattern:
+              A "CREATE" rule pattern (see in_toto.rulelib).
 
-    artifacts_queue:
-            Not yet consumed artifacts (paths only).
+      artifacts_queue:
+              Not yet consumed artifacts (paths only).
 
-    materials:
-            All materials of an item (paths only).
+      materials:
+              All materials of an item (paths only).
 
-    products:
-            All products of an item (paths only).
+      products:
+              All products of an item (paths only).
 
-  <Exceptions>
-    None.
+    <Exceptions>
+      None.
 
-  <Side Effects>
-    None.
+    <Side Effects>
+      None.
 
-  <Returns>
-    The set of consumed artifacts (paths only).
+    <Returns>
+      The set of consumed artifacts (paths only).
 
-  """
-  # Filter queued artifacts using the rule pattern
-  filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
+    """
+    # Filter queued artifacts using the rule pattern
+    filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
 
-  # Consume filtered artifacts that are products but not materials
-  consumed = set(filtered_artifacts) & (products - materials)
+    # Consume filtered artifacts that are products but not materials
+    consumed = set(filtered_artifacts) & (products - materials)
 
-  return consumed
+    return consumed
 
 
 def verify_delete_rule(rule_pattern, artifacts_queue, materials, products):
-  """
-  <Purpose>
-    Filters artifacts from artifacts queue using rule pattern and consumes them
-    if they are in the materials set but are not in the products set, i.e.
-    were deleted.
+    """
+    <Purpose>
+      Filters artifacts from artifacts queue using rule pattern and consumes them
+      if they are in the materials set but are not in the products set, i.e.
+      were deleted.
 
-  <Arguments>
-    rule_pattern:
-            A "DELETE" rule pattern (see in_toto.rulelib).
+    <Arguments>
+      rule_pattern:
+              A "DELETE" rule pattern (see in_toto.rulelib).
 
-    artifacts_queue:
-            Not yet consumed artifacts (paths only).
+      artifacts_queue:
+              Not yet consumed artifacts (paths only).
 
-    materials:
-            All materials of an item (paths only).
+      materials:
+              All materials of an item (paths only).
 
-    products:
-            All products of an item (paths only).
+      products:
+              All products of an item (paths only).
 
-  <Exceptions>
-    None.
+    <Exceptions>
+      None.
 
-  <Side Effects>
-    None.
+    <Side Effects>
+      None.
 
-  <Returns>
-    The set of consumed artifacts (paths only).
+    <Returns>
+      The set of consumed artifacts (paths only).
 
-  """
-  # Filter queued artifacts using the rule pattern
-  filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
+    """
+    # Filter queued artifacts using the rule pattern
+    filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
 
-  # Consume filtered artifacts that are materials but not products
-  consumed = set(filtered_artifacts) & (materials - products)
+    # Consume filtered artifacts that are materials but not products
+    consumed = set(filtered_artifacts) & (materials - products)
 
-  return consumed
+    return consumed
 
 
 def verify_modify_rule(rule_pattern, artifacts_queue, materials, products):
-  """
-  <Purpose>
-    Filters artifacts from artifacts queue using rule pattern and consumes them
-    if they are in both the materials dict and in the products doct, but have
-    different hashes, i.e. were modified.
+    """
+    <Purpose>
+      Filters artifacts from artifacts queue using rule pattern and consumes them
+      if they are in both the materials dict and in the products doct, but have
+      different hashes, i.e. were modified.
 
-  <Arguments>
-    rule_pattern:
-            A "MODIFY" rule pattern (see in_toto.rulelib).
+    <Arguments>
+      rule_pattern:
+              A "MODIFY" rule pattern (see in_toto.rulelib).
 
-    artifacts_queue:
-            Not yet consumed artifacts (paths only).
+      artifacts_queue:
+              Not yet consumed artifacts (paths only).
 
-    materials:
-            All materials of an item (including hashes).
+      materials:
+              All materials of an item (including hashes).
 
-    products:
-            All products of an item (including hashes).
+      products:
+              All products of an item (including hashes).
 
-  <Exceptions>
-    None.
+    <Exceptions>
+      None.
 
-  <Side Effects>
-    None.
+    <Side Effects>
+      None.
 
-  <Returns>
-    The set of consumed artifacts (paths only).
+    <Returns>
+      The set of consumed artifacts (paths only).
 
-  """
-  # Filter queued artifacts using the rule pattern
-  filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
+    """
+    # Filter queued artifacts using the rule pattern
+    filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
 
-  # Filter filtered artifacts that are materials and products
-  filtered_artifacts = set(filtered_artifacts) & \
-      set(materials.keys()) & set(products.keys())
+    # Filter filtered artifacts that are materials and products
+    filtered_artifacts = (
+        set(filtered_artifacts) & set(materials.keys()) & set(products.keys())
+    )
 
-  # Consume filtered artifacts that have different hashes
-  consumed = set()
-  for path in filtered_artifacts:
-    if materials[path] != products[path]:
-      consumed.add(path)
+    # Consume filtered artifacts that have different hashes
+    consumed = set()
+    for path in filtered_artifacts:
+        if materials[path] != products[path]:
+            consumed.add(path)
 
-  return consumed
+    return consumed
 
 
 def verify_allow_rule(rule_pattern, artifacts_queue):
-  """
-  <Purpose>
-    Consumes artifacts, filtered from the artifacts queue using rule pattern.
+    """
+    <Purpose>
+      Consumes artifacts, filtered from the artifacts queue using rule pattern.
 
-  <Arguments>
-    rule_pattern:
-            An "ALLOW" rule pattern (see in_toto.rulelib).
+    <Arguments>
+      rule_pattern:
+              An "ALLOW" rule pattern (see in_toto.rulelib).
 
-    artifacts_queue:
-            Not yet consumed artifacts (paths only).
+      artifacts_queue:
+              Not yet consumed artifacts (paths only).
 
-  <Exceptions>
-    None.
+    <Exceptions>
+      None.
 
-  <Side Effects>
-    None.
+    <Side Effects>
+      None.
 
-  <Returns>
-    The set of consumed artifacts (paths only).
+    <Returns>
+      The set of consumed artifacts (paths only).
 
-  """
-  # Filter queued artifacts using the rule pattern
-  filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
+    """
+    # Filter queued artifacts using the rule pattern
+    filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
 
-  # Consume all filtered artifacts
-  return set(filtered_artifacts)
+    # Consume all filtered artifacts
+    return set(filtered_artifacts)
 
 
 def verify_disallow_rule(rule_pattern, artifacts_queue):
-  """
-  <Purpose>
-    Raises RuleVerificationError if rule pattern applies to any artifacts in
-    the queue.
-
-    NOTE: Each set of rules should have a terminal DISALLOW rule to make
-    overall verification fail in case preceding rules did not consume all
-    artifacts as intended.
-
-  <Arguments>
-    rule_pattern:
-            A "DISALLOW" rule pattern (see in_toto.rulelib).
-
-    artifacts_queue:
-            Not yet consumed artifacts (paths only).
-
-  <Exceptions>
-    RuleVerificationError
-        if the rule pattern filters artifacts in the artifact queue.
-
-  <Side Effects>
-    None.
-
-  <Returns>
-    None.
-
-  """
-  filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
-
-  if len(filtered_artifacts):
-    raise RuleVerificationError("'DISALLOW {}' matched the following "
-      "artifacts: {}\n{}".format(rule_pattern, filtered_artifacts,
-      _get_artifact_rule_traceback()))
+    """
+    <Purpose>
+      Raises RuleVerificationError if rule pattern applies to any artifacts in
+      the queue.
+
+      NOTE: Each set of rules should have a terminal DISALLOW rule to make
+      overall verification fail in case preceding rules did not consume all
+      artifacts as intended.
+
+    <Arguments>
+      rule_pattern:
+              A "DISALLOW" rule pattern (see in_toto.rulelib).
+
+      artifacts_queue:
+              Not yet consumed artifacts (paths only).
+
+    <Exceptions>
+      RuleVerificationError
+          if the rule pattern filters artifacts in the artifact queue.
+
+    <Side Effects>
+      None.
+
+    <Returns>
+      None.
+
+    """
+    filtered_artifacts = fnmatch.filter(artifacts_queue, rule_pattern)
+
+    if len(filtered_artifacts):
+        raise RuleVerificationError(
+            "'DISALLOW {}' matched the following "
+            "artifacts: {}\n{}".format(
+                rule_pattern, filtered_artifacts, _get_artifact_rule_traceback()
+            )
+        )
 
 
 def verify_require_rule(filename, artifacts_queue):
-  """
-  <Purpose>
-    Raises RuleVerificationError if the filename provided does not exist in the
-    artifacts_queue
-
-  <Arguments>
-    filename:
-            A single filename (see issues #193 and #152). We will ignore the
-            artifact rule pattern because it's ambiguous and instead treat it
-            as a literal file name.
-
-    artifacts_queue:
-            Not yet consumed artifacts (paths only).
-
-  <Exceptions>
-    RuleVerificationError:
-      if the filename is not present in the artifacts queue
-
-  <Side Effects>
-    None.
-
-  <Returns>
-    None.
-
-  """
-  if filename not in artifacts_queue:
-    raise RuleVerificationError("'REQUIRE {filename}' did not find {filename} "
-        "in: {queue}\n{traceback}".format(filename=filename,
-        queue=artifacts_queue, traceback=_get_artifact_rule_traceback()))
+    """
+    <Purpose>
+      Raises RuleVerificationError if the filename provided does not exist in the
+      artifacts_queue
+
+    <Arguments>
+      filename:
+              A single filename (see issues #193 and #152). We will ignore the
+              artifact rule pattern because it's ambiguous and instead treat it
+              as a literal file name.
+
+      artifacts_queue:
+              Not yet consumed artifacts (paths only).
+
+    <Exceptions>
+      RuleVerificationError:
+        if the filename is not present in the artifacts queue
+
+    <Side Effects>
+      None.
+
+    <Returns>
+      None.
+
+    """
+    if filename not in artifacts_queue:
+        raise RuleVerificationError(
+            "'REQUIRE {filename}' did not find {filename} "
+            "in: {queue}\n{traceback}".format(
+                filename=filename,
+                queue=artifacts_queue,
+                traceback=_get_artifact_rule_traceback(),
+            )
+        )
 
 
 def _get_artifact_rule_traceback():
-  """Build and return string form global `RULE_TRACE` which may be used as
-  error message for RuleVerificationError.
+    """Build and return string form global `RULE_TRACE` which may be used as
+    error message for RuleVerificationError.
 
-  """
-  traceback_str = "Full trace for 'expected_{0}' of item '{1}':\n".format(
-      RULE_TRACE["source_type"], RULE_TRACE["source_name"])
-
-  # Show all materials and products available in the beginning and
-  # label the one that is used to generate a queue.
-  for source_type in ["materials", "products"]:
-    traceback_str += "Available {}{}:\n{}\n".format(
-        source_type,
-        [" (used for queue)", ""][RULE_TRACE["source_type"] != source_type],
-        RULE_TRACE[source_type])
-
-  for trace_entry in RULE_TRACE["trace"]:
-    traceback_str += "Queue after '{0}':\n".format(
-        " ".join(trace_entry["rule"]))
-    traceback_str += "{}\n".format(trace_entry["queue"])
+    """
+    traceback_str = "Full trace for 'expected_{0}' of item '{1}':\n".format(
+        RULE_TRACE["source_type"], RULE_TRACE["source_name"]
+    )
+
+    # Show all materials and products available in the beginning and
+    # label the one that is used to generate a queue.
+    for source_type in ["materials", "products"]:
+        traceback_str += "Available {}{}:\n{}\n".format(
+            source_type,
+            [" (used for queue)", ""][RULE_TRACE["source_type"] != source_type],
+            RULE_TRACE[source_type],
+        )
+
+    for trace_entry in RULE_TRACE["trace"]:
+        traceback_str += "Queue after '{0}':\n".format(
+            " ".join(trace_entry["rule"])
+        )
+        traceback_str += "{}\n".format(trace_entry["queue"])
 
-  return traceback_str
+    return traceback_str
 
 
 def verify_item_rules(source_name, source_type, rules, links):
-  """
-  <Purpose>
-    Apply all passed material or product rules (see source_type) of a given
-    step or inspection (see source_name), to enforce and authorize the
-    corresponding artifacts and to guarantee that artifacts are linked together
-    across steps of the supply chain.
-
-    The mode of operation is similar to that of a firewall:
-    In the beginning all materials or products of the step or inspection are
-    placed into an artifact queue. The rules are then applied sequentially,
-    consuming artifacts in the queue, i.e. removing them from the queue upon
-    successful application.
-
-    The consumption of artifacts by itself has no effects on the verification.
-    Only through a subsequent "DISALLOW" rule, that finds unconsumed artifacts,
-    is an exception raised. Similarly does the "REQUIRE" rule raise exception,
-    if it does not find the artifact it requires, because it has falsely been
-    consumed or was not there from the beginning.
-
-
-
-  <Arguments>
-    source_name:
-            The name of the item (step or inspection) being verified.
-
-    source_type:
-            One of "materials" or "products" depending on whether the rules are
-            taken from the "expected_materials" or "expected_products" field of
-            the item being verified.
-
-    rules:
-            The list of rules (material or product rules) for the item being
-            verified.
-
-    links:
-            A dictionary containing link metadata per step or inspection, e.g.:
-            {
-              <link name> : <Link object>,
-              ...
-            }
-
-  <Exceptions>
-    FormatError
-        if source_type is not "materials" or "products", or
-        if a rule in the passed list of rules does not conform with any rule
-        format.
-
-    RuleVerificationError
-        if a DISALLOW rule matches disallowed artifacts, or
-        if a REQUIRE rule does not find a required artifact.
-
-  <Side Effects>
-    Clears and populates the global RULE_TRACE data structure.
-
-  """
-  if source_type not in ["materials", "products"]:
-    raise securesystemslib.exceptions.FormatError(
-        "Argument 'source_type' of function 'verify_item_rules' has to be "
-        "one of 'materials' or 'products'. Got: '{}'".format(source_type))
-
-  # Create shortcuts to item's materials and products (including hashes),
-  # required to verify "modify" and "match" rules.
-  materials_dict = links[source_name].materials
-  products_dict = links[source_name].products
-
-  # All other rules only require materials or products paths (without hashes)
-  materials_paths = set(materials_dict.keys())
-  products_paths = set(products_dict.keys())
-
-  # Depending on the source type we create the artifact queue from the item's
-  # materials or products and use it to keep track of (not) consumed artifacts.
-  # The queue also only contains aritfact keys (without hashes)
-  artifacts = getattr(links[source_name], source_type)
-  artifacts_queue = set(artifacts.keys())
-
-  # Reset and re-populate rule traceback info dict for a rich error message
-  RULE_TRACE.clear()
-  RULE_TRACE["source_name"] = source_name
-  RULE_TRACE["source_type"] = source_type
-  RULE_TRACE["materials"] = list(materials_dict)
-  RULE_TRACE["products"] = list(products_dict)
-  RULE_TRACE["trace"] = []
-
-  # Process rules and remove consumed items from queue in each iteration
-  for rule in rules:
-    LOG.info("Verifying '{}'...".format(" ".join(rule)))
-
-    # Parse the rule and create two shortcuts to contained rule data
-    rule_data = in_toto.rulelib.unpack_rule(rule)
-    _type = rule_data["rule_type"]
-    _pattern = rule_data["pattern"]
-
-
-    # Initialize empty consumed set as fallback for rules that do not consume
-    # artifacts. All rules except "disallow" and "require" consume artifacts.
-    consumed = set()
+    """
+    <Purpose>
+      Apply all passed material or product rules (see source_type) of a given
+      step or inspection (see source_name), to enforce and authorize the
+      corresponding artifacts and to guarantee that artifacts are linked together
+      across steps of the supply chain.
+
+      The mode of operation is similar to that of a firewall:
+      In the beginning all materials or products of the step or inspection are
+      placed into an artifact queue. The rules are then applied sequentially,
+      consuming artifacts in the queue, i.e. removing them from the queue upon
+      successful application.
+
+      The consumption of artifacts by itself has no effects on the verification.
+      Only through a subsequent "DISALLOW" rule, that finds unconsumed artifacts,
+      is an exception raised. Similarly does the "REQUIRE" rule raise exception,
+      if it does not find the artifact it requires, because it has falsely been
+      consumed or was not there from the beginning.
 
-    if _type == "match":
-      consumed = verify_match_rule(
-          rule_data, artifacts_queue, artifacts, links)
-
-    elif _type == "create":
-      consumed = verify_create_rule(
-          _pattern, artifacts_queue, materials_paths, products_paths)
-
-    elif _type == "delete":
-      consumed = verify_delete_rule(
-          _pattern, artifacts_queue, materials_paths, products_paths)
-
-    elif _type == "modify":
-      consumed = verify_modify_rule(
-          _pattern, artifacts_queue, materials_dict, products_dict)
-
-    elif _type == "allow":
-      consumed = verify_allow_rule(_pattern, artifacts_queue)
-
-    # It's up to the "disallow" and "require" rule to raise an error if
-    # artifacts were not consumed as intended
-    elif _type == "disallow":
-      verify_disallow_rule(_pattern, artifacts_queue)
-
-    elif _type == "require":
-      verify_require_rule(_pattern, artifacts_queue)
-
-    else: # pragma: no cover (unreachable)
-      raise securesystemslib.exceptions.FormatError(
-          "Invaldid rule type '{}'.".format(_type))
-
-    artifacts_queue -= consumed
-
-    # Append rule and copy of queue to global info for a rich error message
-    RULE_TRACE["trace"].append({
-          "rule": rule,
-          "queue": list(artifacts_queue)
-        })
 
 
-def verify_all_item_rules(items, links):
-  """
-  <Purpose>
-    Iteratively verifies artifact rules of passed items (Steps or Inspections).
-
-  <Arguments>
-    items:
-            A list containing Step or Inspection objects whose material
-            and product rules will be verified.
-
-    links:
-            A dictionary containing link metadata per step or inspection, e.g.:
-            {
-              <link name> : <Link object>,
-              ...
-            }
-
-  <Exceptions>
-    None.
-
-  <Side Effects>
-    None.
-
-  """
-  for item in items:
-    LOG.info("Verifying material rules for '{}'...".format(item.name))
-    verify_item_rules(item.name, "materials", item.expected_materials, links)
+    <Arguments>
+      source_name:
+              The name of the item (step or inspection) being verified.
+
+      source_type:
+              One of "materials" or "products" depending on whether the rules are
+              taken from the "expected_materials" or "expected_products" field of
+              the item being verified.
+
+      rules:
+              The list of rules (material or product rules) for the item being
+              verified.
+
+      links:
+              A dictionary containing link metadata per step or inspection, e.g.:
+              {
+                <link name> : <Link object>,
+                ...
+              }
 
-    LOG.info("Verifying product rules for '{}'...".format(item.name))
-    verify_item_rules(item.name, "products", item.expected_products, links)
+    <Exceptions>
+      FormatError
+          if source_type is not "materials" or "products", or
+          if a rule in the passed list of rules does not conform with any rule
+          format.
+
+      RuleVerificationError
+          if a DISALLOW rule matches disallowed artifacts, or
+          if a REQUIRE rule does not find a required artifact.
+
+    <Side Effects>
+      Clears and populates the global RULE_TRACE data structure.
+
+    """
+    if source_type not in ["materials", "products"]:
+        raise securesystemslib.exceptions.FormatError(
+            "Argument 'source_type' of function 'verify_item_rules' has to be "
+            "one of 'materials' or 'products'. Got: '{}'".format(source_type)
+        )
+
+    # Create shortcuts to item's materials and products (including hashes),
+    # required to verify "modify" and "match" rules.
+    materials_dict = links[source_name].materials
+    products_dict = links[source_name].products
+
+    # All other rules only require materials or products paths (without hashes)
+    materials_paths = set(materials_dict.keys())
+    products_paths = set(products_dict.keys())
+
+    # Depending on the source type we create the artifact queue from the item's
+    # materials or products and use it to keep track of (not) consumed artifacts.
+    # The queue also only contains aritfact keys (without hashes)
+    artifacts = getattr(links[source_name], source_type)
+    artifacts_queue = set(artifacts.keys())
+
+    # Reset and re-populate rule traceback info dict for a rich error message
+    RULE_TRACE.clear()
+    RULE_TRACE["source_name"] = source_name
+    RULE_TRACE["source_type"] = source_type
+    RULE_TRACE["materials"] = list(materials_dict)
+    RULE_TRACE["products"] = list(products_dict)
+    RULE_TRACE["trace"] = []
+
+    # Process rules and remove consumed items from queue in each iteration
+    for rule in rules:
+        LOG.info("Verifying '{}'...".format(" ".join(rule)))
+
+        # Parse the rule and create two shortcuts to contained rule data
+        rule_data = in_toto.rulelib.unpack_rule(rule)
+        _type = rule_data["rule_type"]
+        _pattern = rule_data["pattern"]
+
+        # Initialize empty consumed set as fallback for rules that do not consume
+        # artifacts. All rules except "disallow" and "require" consume artifacts.
+        consumed = set()
+
+        if _type == "match":
+            consumed = verify_match_rule(
+                rule_data, artifacts_queue, artifacts, links
+            )
+
+        elif _type == "create":
+            consumed = verify_create_rule(
+                _pattern, artifacts_queue, materials_paths, products_paths
+            )
+
+        elif _type == "delete":
+            consumed = verify_delete_rule(
+                _pattern, artifacts_queue, materials_paths, products_paths
+            )
+
+        elif _type == "modify":
+            consumed = verify_modify_rule(
+                _pattern, artifacts_queue, materials_dict, products_dict
+            )
+
+        elif _type == "allow":
+            consumed = verify_allow_rule(_pattern, artifacts_queue)
+
+        # It's up to the "disallow" and "require" rule to raise an error if
+        # artifacts were not consumed as intended
+        elif _type == "disallow":
+            verify_disallow_rule(_pattern, artifacts_queue)
+
+        elif _type == "require":
+            verify_require_rule(_pattern, artifacts_queue)
+
+        else:  # pragma: no cover (unreachable)
+            raise securesystemslib.exceptions.FormatError(
+                "Invaldid rule type '{}'.".format(_type)
+            )
+
+        artifacts_queue -= consumed
+
+        # Append rule and copy of queue to global info for a rich error message
+        RULE_TRACE["trace"].append(
+            {"rule": rule, "queue": list(artifacts_queue)}
+        )
 
 
-def verify_threshold_constraints(layout, chain_link_dict):
-  """
-  <Purpose>
-    Verifies that all links corresponding to a given step report the same
-    materials and products.
-
-    NOTE: This function does not verify if the signatures of each link
-    corresponding to a step are valid or created by a different authorized
-    functionary. This should be done earlier, using the function
-    `verify_link_signature_thresholds`.
-
-  <Arguments>
-    layout:
-            The layout whose step thresholds are being verified
-
-    chain_link_dict:
-            A dictionary containing link metadata per functionary per step,
-            e.g.:
-            {
-              <link name> : {
-                <functionary key id> : <Link object>,
+def verify_all_item_rules(items, links):
+    """
+    <Purpose>
+      Iteratively verifies artifact rules of passed items (Steps or Inspections).
+
+    <Arguments>
+      items:
+              A list containing Step or Inspection objects whose material
+              and product rules will be verified.
+
+      links:
+              A dictionary containing link metadata per step or inspection, e.g.:
+              {
+                <link name> : <Link object>,
                 ...
-              }, ...
-            }
-
-  <Exceptions>
-    ThresholdVerificationError
-        If there are not enough (threshold) links for a steps
-
-        If the artifacts for all links of a step are not equal
-
-
-  <Side Effects>
-    None.
-
-  """
-
-  # We are only interested in links that are related to steps defined in the
-  # Layout, so iterate over layout.steps
-  for step in layout.steps:
-    # Skip steps that don't require multiple functionaries
-    if step.threshold <= 1:
-      LOG.info("Skipping threshold verification for step '{0}' with"
-          " threshold '{1}'...".format(step.name, step.threshold))
-      continue
-
-    LOG.info("Verifying threshold for step '{0}' with"
-        " threshold '{1}'...".format(step.name, step.threshold))
-    # Extract the key_link_dict for this step from the passed chain_link_dict
-    key_link_dict = chain_link_dict[step.name]
-
-    # Check if we have at least <threshold> links for this step
-    # NOTE: This is already done in `verify_link_signature_thresholds`,
-    # Should we remove the check?
-    if len(key_link_dict) < step.threshold:
-      raise ThresholdVerificationError("Step '{0}' not performed"
-          " by enough functionaries!".format(step.name))
-
-    # Take a reference link (e.g. the first in the step_link_dict)
-    reference_keyid = list(key_link_dict.keys())[0]
-    reference_link = key_link_dict[reference_keyid]
-
-    # Iterate over all links to compare their properties with a reference_link
-    for keyid, link in key_link_dict.items():
-      # TODO: Do we only care for artifacts, or do we want to
-      # assert equality of other properties as well?
-      if (reference_link.materials != link.materials or
-          reference_link.products != link.products):
-        raise ThresholdVerificationError("Links '{0}' and '{1}' have different"
-            " artifacts!".format(
-                in_toto.models.link.FILENAME_FORMAT.format(
-                    step_name=step.name, keyid=reference_keyid),
-                in_toto.models.link.FILENAME_FORMAT.format(
-                    step_name=step.name, keyid=keyid)))
+              }
 
+    <Exceptions>
+      None.
 
-def reduce_chain_links(chain_link_dict):
-  """
-  <Purpose>
-    Iterates through the passed chain_link_dict and builds a dict with
-    step-name as keys and link objects as values.
-    We already check if the links of different functionaries are
-    identical.
-
-  <Arguments>
-    layout:
-            The layout specified by the project owner against which the
-            threshold will be verified.
-
-    chain_link_dict:
-            A dictionary containing link metadata per functionary per step,
-            e.g.:
-            {
-              <link name> : {
-                <functionary key id> : <Link object>,
-                ...
-              }, ...
-            }
+    <Side Effects>
+      None.
 
-  <Exceptions>
-    None.
+    """
+    for item in items:
+        LOG.info("Verifying material rules for '{}'...".format(item.name))
+        verify_item_rules(
+            item.name, "materials", item.expected_materials, links
+        )
 
-  <Side Effects>
-    None.
+        LOG.info("Verifying product rules for '{}'...".format(item.name))
+        verify_item_rules(item.name, "products", item.expected_products, links)
 
-  <Returns>
-    A dictionary containing one Link metadata object per step only if
-    the link artifacts of all link objects are identical for a step.
 
-  """
+def verify_threshold_constraints(layout, chain_link_dict):
+    """
+    <Purpose>
+      Verifies that all links corresponding to a given step report the same
+      materials and products.
+
+      NOTE: This function does not verify if the signatures of each link
+      corresponding to a step are valid or created by a different authorized
+      functionary. This should be done earlier, using the function
+      `verify_link_signature_thresholds`.
+
+    <Arguments>
+      layout:
+              The layout whose step thresholds are being verified
+
+      chain_link_dict:
+              A dictionary containing link metadata per functionary per step,
+              e.g.:
+              {
+                <link name> : {
+                  <functionary key id> : <Link object>,
+                  ...
+                }, ...
+              }
+
+    <Exceptions>
+      ThresholdVerificationError
+          If there are not enough (threshold) links for a steps
+
+          If the artifacts for all links of a step are not equal
+
+
+    <Side Effects>
+      None.
+
+    """
+
+    # We are only interested in links that are related to steps defined in the
+    # Layout, so iterate over layout.steps
+    for step in layout.steps:
+        # Skip steps that don't require multiple functionaries
+        if step.threshold <= 1:
+            LOG.info(
+                "Skipping threshold verification for step '{0}' with"
+                " threshold '{1}'...".format(step.name, step.threshold)
+            )
+            continue
+
+        LOG.info(
+            "Verifying threshold for step '{0}' with"
+            " threshold '{1}'...".format(step.name, step.threshold)
+        )
+        # Extract the key_link_dict for this step from the passed chain_link_dict
+        key_link_dict = chain_link_dict[step.name]
+
+        # Check if we have at least <threshold> links for this step
+        # NOTE: This is already done in `verify_link_signature_thresholds`,
+        # Should we remove the check?
+        if len(key_link_dict) < step.threshold:
+            raise ThresholdVerificationError(
+                "Step '{0}' not performed"
+                " by enough functionaries!".format(step.name)
+            )
+
+        # Take a reference link (e.g. the first in the step_link_dict)
+        reference_keyid = list(key_link_dict.keys())[0]
+        reference_link = key_link_dict[reference_keyid]
+
+        # Iterate over all links to compare their properties with a reference_link
+        for keyid, link in key_link_dict.items():
+            # TODO: Do we only care for artifacts, or do we want to
+            # assert equality of other properties as well?
+            if (
+                reference_link.materials != link.materials
+                or reference_link.products != link.products
+            ):
+                raise ThresholdVerificationError(
+                    "Links '{0}' and '{1}' have different"
+                    " artifacts!".format(
+                        in_toto.models.link.FILENAME_FORMAT.format(
+                            step_name=step.name, keyid=reference_keyid
+                        ),
+                        in_toto.models.link.FILENAME_FORMAT.format(
+                            step_name=step.name, keyid=keyid
+                        ),
+                    )
+                )
 
-  reduced_chain_link_dict = {}
 
-  for step_name, key_link_dict in chain_link_dict.items():
-    # Extract the key_link_dict for this step from the passed chain_link_dict
-    # take one exemplary link (e.g. the first in the step_link_dict)
-    # form the reduced_chain_link_dict to return
-    reduced_chain_link_dict[step_name] = list(key_link_dict.values())[0]
+def reduce_chain_links(chain_link_dict):
+    """
+    <Purpose>
+      Iterates through the passed chain_link_dict and builds a dict with
+      step-name as keys and link objects as values.
+      We already check if the links of different functionaries are
+      identical.
+
+    <Arguments>
+      layout:
+              The layout specified by the project owner against which the
+              threshold will be verified.
+
+      chain_link_dict:
+              A dictionary containing link metadata per functionary per step,
+              e.g.:
+              {
+                <link name> : {
+                  <functionary key id> : <Link object>,
+                  ...
+                }, ...
+              }
+
+    <Exceptions>
+      None.
+
+    <Side Effects>
+      None.
+
+    <Returns>
+      A dictionary containing one Link metadata object per step only if
+      the link artifacts of all link objects are identical for a step.
+
+    """
+
+    reduced_chain_link_dict = {}
+
+    for step_name, key_link_dict in chain_link_dict.items():
+        # Extract the key_link_dict for this step from the passed chain_link_dict
+        # take one exemplary link (e.g. the first in the step_link_dict)
+        # form the reduced_chain_link_dict to return
+        reduced_chain_link_dict[step_name] = list(key_link_dict.values())[0]
 
-  return reduced_chain_link_dict
+    return reduced_chain_link_dict
 
 
 def verify_sublayouts(layout, steps_metadata, superlayout_link_dir_path):
-  """
-  <Purpose>
-    Extracts link or layout object for each step in steps_metadata. Checks if
-    any step has been delegated by the functionary, recurses into the
-    delegation, and replaces the layout object with an equivalent link object.
-    Returns the extracted link objects in a dict called chain_link_dict.
-
-  <Arguments>
-    layout:
-            The layout specified by the project owner.
-
-    steps_metadata:
-            A dictionary containing link metadata per functionary per step,
-            e.g.:
-            {
-              <link name> : {
-                <functionary key id> : <Metadata containing a Link or Layout
-                                          object>,
-                ...
-              }, ...
-            }
-
-    superlayout_link_dir_path:
-            A path to a directory, where links of the superlayout are loaded
-            from. Links of the sublayout are expected to be in a subdirectory
-            relative to this path, with a name in the format
-            in_toto.models.layout.SUBLAYOUT_LINK_DIR_FORMAT.
-
-  <Exceptions>
-    raises an Exception if verification of the delegated step fails.
-
-  <Side Effects>
-    None.
-
-  <Returns>
-    The passed dictionary containing Link objects instead of metadata per
-    functionary per step, with layouts replaced with summary links.
-    e.g.:
-    {
-      <link name> : {
-        <functionary key id> : <Link object>,
-        ...
-      }, ...
-    }
-
-  """
-  chain_link_dict = {}
-
-  for step_name, metadata_dict in steps_metadata.items():
-
-    key_link_dict = {}
-    for keyid, metadata in metadata_dict.items():
-
-      payload = metadata.get_payload()
-
-      if payload.type_ == "layout":
-
-        LOG.info("Verifying sublayout {}...".format(step_name))
-        layout_key_dict = {}
-
-        # Retrieve the entire key object for the keyid
-        # corresponding to the link
-        layout_key_dict = {keyid: layout.keys.get(keyid)}
-
-        # Sublayout links are expected to be in a directory with the following
-        # name relative the the current link directory path, i.e. if there
-        # are multiple levels of sublayout nesting, the links are expected to
-        # be nested accordingly
-        sub_link_dir = in_toto.models.layout.SUBLAYOUT_LINK_DIR_FORMAT.format(
-            name=step_name, keyid=keyid)
-
-        sublayout_link_dir_path = os.path.join(
-            superlayout_link_dir_path, sub_link_dir)
-
-        # Make a recursive call to in_toto_verify with the
-        # layout and the extracted key object
-        summary_link = in_toto_verify(metadata, layout_key_dict,
-            link_dir_path=sublayout_link_dir_path, step_name=step_name)
-
-        # Replace the layout object with the link object returned
-        # by in-toto-verify
-        payload = summary_link
+    """
+    <Purpose>
+      Extracts link or layout object for each step in steps_metadata. Checks if
+      any step has been delegated by the functionary, recurses into the
+      delegation, and replaces the layout object with an equivalent link object.
+      Returns the extracted link objects in a dict called chain_link_dict.
+
+    <Arguments>
+      layout:
+              The layout specified by the project owner.
+
+      steps_metadata:
+              A dictionary containing link metadata per functionary per step,
+              e.g.:
+              {
+                <link name> : {
+                  <functionary key id> : <Metadata containing a Link or Layout
+                                            object>,
+                  ...
+                }, ...
+              }
+
+      superlayout_link_dir_path:
+              A path to a directory, where links of the superlayout are loaded
+              from. Links of the sublayout are expected to be in a subdirectory
+              relative to this path, with a name in the format
+              in_toto.models.layout.SUBLAYOUT_LINK_DIR_FORMAT.
+
+    <Exceptions>
+      raises an Exception if verification of the delegated step fails.
+
+    <Side Effects>
+      None.
+
+    <Returns>
+      The passed dictionary containing Link objects instead of metadata per
+      functionary per step, with layouts replaced with summary links.
+      e.g.:
+      {
+        <link name> : {
+          <functionary key id> : <Link object>,
+          ...
+        }, ...
+      }
+
+    """
+    chain_link_dict = {}
+
+    for step_name, metadata_dict in steps_metadata.items():
+        key_link_dict = {}
+        for keyid, metadata in metadata_dict.items():
+            payload = metadata.get_payload()
+
+            if payload.type_ == "layout":
+                LOG.info("Verifying sublayout {}...".format(step_name))
+                layout_key_dict = {}
+
+                # Retrieve the entire key object for the keyid
+                # corresponding to the link
+                layout_key_dict = {keyid: layout.keys.get(keyid)}
+
+                # Sublayout links are expected to be in a directory with the following
+                # name relative the the current link directory path, i.e. if there
+                # are multiple levels of sublayout nesting, the links are expected to
+                # be nested accordingly
+                sub_link_dir = (
+                    in_toto.models.layout.SUBLAYOUT_LINK_DIR_FORMAT.format(
+                        name=step_name, keyid=keyid
+                    )
+                )
+
+                sublayout_link_dir_path = os.path.join(
+                    superlayout_link_dir_path, sub_link_dir
+                )
+
+                # Make a recursive call to in_toto_verify with the
+                # layout and the extracted key object
+                summary_link = in_toto_verify(
+                    metadata,
+                    layout_key_dict,
+                    link_dir_path=sublayout_link_dir_path,
+                    step_name=step_name,
+                )
+
+                # Replace the layout object with the link object returned
+                # by in-toto-verify
+                payload = summary_link
 
-      key_link_dict[keyid] = payload
-    chain_link_dict[step_name] = key_link_dict
+            key_link_dict[keyid] = payload
+        chain_link_dict[step_name] = key_link_dict
 
-  return chain_link_dict
+    return chain_link_dict
 
 
 def get_summary_link(layout, reduced_chain_link_dict, name):
-  """
-  <Purpose>
-    Merges the materials of the first step (as mentioned in the layout)
-    and the products of the last step and returns a new link.
-    This link reports the materials and products and summarizes the
-    overall software supply chain.
-    NOTE: The assumption is that the steps mentioned in the layout are
-    to be performed sequentially. So, the first step mentioned in the
-    layout denotes what comes into the supply chain and the last step
-    denotes what goes out.
-
-  <Arguments>
-    layout:
-            The layout specified by the project owner.
-
-    reduced_chain_link_dict:
-            A dictionary containing link metadata per step,
-            e.g.:
-            {
-              <link name> : <Link object>,
-              ...
-            }
-    name:
-            The name that the summary link will be associated with.
-
-  <Exceptions>
-    None.
-
-  <Side Effects>
-    None.
-
-  <Returns>
-    A Link object which summarizes the materials and products of the overall
-    software supply chain.
-
-  """
-  # Create empty link object
-  summary_link = in_toto.models.link.Link()
-
-  # Take first and last link in the order the corresponding
-  # steps appear in the layout, if there are any.
-  if len(layout.steps) > 0:
-    first_step_link = reduced_chain_link_dict[layout.steps[0].name]
-    last_step_link = reduced_chain_link_dict[layout.steps[-1].name]
-
-    summary_link.materials = first_step_link.materials
-    summary_link.name = name
-
-    summary_link.products = last_step_link.products
-    summary_link.byproducts = last_step_link.byproducts
-    summary_link.command = last_step_link.command
-
-  return summary_link
-
-
-def in_toto_verify(metadata, layout_key_dict, link_dir_path=".",
-    substitution_parameters=None, step_name="",
-    persist_inspection_links=True):
-  """Performs complete in-toto supply chain verification for a final product.
-
-  The verification procedure consists of the following activities, performed in
-  the given order:
-
-  1.  Verify layout signatures
-  2.  Verify layout expiration date
-  3.  Substitute placeholders in the layout
-  4.  Load link metadata
-  5.  Verify link signatures with keys in layout
-  6.  Recurse into sublayout verification
-  7.  Soft-verify alignment of reported and expected commands. Note:
-      verification does not fail if commands don't match, instead a warning is
-      logged as per the in-toto specification --
-      https://github.com/in-toto/docs/blob/master/in-toto-spec.md#431-steps
-  8.  Verify threshold artifact constraints
-  9.  Process step product and material rules
-  10. Execute inspection commands and generate inspection links
-  11. Process inspection product and material rules
-
-  Arguments:
-    metadata: A Metadata object that contains a Layout object to be verified.
-
-    layout_key_dict: A public key dictionary. The verification routine requires
-        at least one key, and a valid signature on the layout for each key.
-
-    link_dir_path (optional): A directory path to link metadata files. The
-        expected filename format for link metadata files is
-        ``STEP-NAME.KEYID-PREFIX.link``. Link metadata files for a sublayout
-        are loaded from a subdirectory relative to the link_dir_path of the
-        superlayout. The expected directory name format is
-        ``SUBLAYOUT-STEP-NAME.KEYID-PREFIX``.
-
-    substitution_parameters (optional): A dictionary with substitution values
-        for artifact rules (steps and inspections), the expected command
-        attribute (steps), and the run attribute (inspections) in the layout.
-
-    step_name (optional): A name assigned to the returned link. This is mostly
-        useful during recursive sublayout verification.
-
-    persist_inspection_links (optional): A boolean that determines whether or
-        not link metadata files for inspection are written to cwd.
-
-  Raises:
-    securesystemslib.exceptions.FormatError: Passed parameters are malformed.
-
-    SignatureVerificationError: No layout verification key is passed, or any of
-        the passed keys fails to verify a signature.
-
-    LayoutExpiredError: The layout is expired.
-
-    LinkNotFoundError: Fewer than threshold link metadata files can be found
-        for a step of the layout.
-
-    ThresholdVerificationError: Fewer than threshold links, validly signed by
-        different authorized functionaries, who agree on the recorded materials
-        and products, can be found for a step of the layout. (Links with
-        invalid signatures or signatures by unauthorized functionaries are
-        ignored.)
-
-    RuleVerificationError: A DISALLOW rule matches disallowed artifacts, or
-        a REQUIRE rule does not find a required artifact.
-
-    BadReturnValueError: An inspection command returns a non-zero value.
-
-  Side Effects:
-    Reads link metadata files from disk.
-    Runs inspection commands in subprocess.
-
-  Returns:
-    A Link object, which summarizes the materials and products of the overall
-    software supply chain. This is mostly useful during recursive sublayout
-    verification.
-
-  """
-
-  LOG.info("Verifying layout metadata signatures...")
-  verify_metadata_signatures(metadata, layout_key_dict)
-
-  # For the rest of the verification we only care about the layout payload
-  # (Layout) that carries all the information and not about the layout
-  # container (Metablock) that also carries the signatures
-  LOG.info("Extracting layout from metadata...")
-  layout = metadata.get_payload()
-
-  LOG.info("Verifying layout expiration...")
-  verify_layout_expiration(layout)
-
-  # If there are parameters sent to the translation layer, substitute them
-  if substitution_parameters is not None:
-    LOG.info('Performing parameter substitution...')
-    substitute_parameters(layout, substitution_parameters)
-
-  LOG.info("Reading link metadata files...")
-  steps_metadata = load_links_for_layout(layout, link_dir_path)
-
-  LOG.info("Verifying link metadata signatures...")
-  steps_metadata = verify_link_signature_thresholds(layout, steps_metadata)
-
-  LOG.info("Verifying sublayouts...")
-  chain_link_dict = verify_sublayouts(layout, steps_metadata, link_dir_path)
-
-  LOG.info("Verifying alignment of reported commands...")
-  verify_all_steps_command_alignment(layout, chain_link_dict)
-
-  LOG.info("Verifying threshold constraints...")
-  verify_threshold_constraints(layout, chain_link_dict)
-  reduced_chain_link_dict = reduce_chain_links(chain_link_dict)
-
-  # NOTE: Processing step rules before executing inspections guarantees that
-  # inspection commands don't run on compromised target files, however, this
-  # also precludes step match rules from referencing inspection artifacts.
-  LOG.info("Verifying Step rules...")
-  verify_all_item_rules(layout.steps, reduced_chain_link_dict)
-
-  LOG.info("Executing Inspection commands...")
-  inspection_link_dict = run_all_inspections(layout, persist_inspection_links)
-
-  LOG.info("Verifying Inspection rules...")
-  # Artifact rules for inspections can reference links that correspond to
-  # Steps or Inspections, hence the concatenation of both collections of links
-  combined_links = reduced_chain_link_dict.copy()
-  combined_links.update(inspection_link_dict)
-  verify_all_item_rules(layout.inspect, combined_links)
-
-  # We made it this far without exception that means, verification passed
-  LOG.info("The software product passed all verification.")
-
-  # Return a link file which summarizes the entire software supply chain
-  # This is mostly relevant if the currently verified supply chain is embedded
-  # in another supply chain
-  return get_summary_link(layout, reduced_chain_link_dict, step_name)
+    """
+    <Purpose>
+      Merges the materials of the first step (as mentioned in the layout)
+      and the products of the last step and returns a new link.
+      This link reports the materials and products and summarizes the
+      overall software supply chain.
+      NOTE: The assumption is that the steps mentioned in the layout are
+      to be performed sequentially. So, the first step mentioned in the
+      layout denotes what comes into the supply chain and the last step
+      denotes what goes out.
+
+    <Arguments>
+      layout:
+              The layout specified by the project owner.
+
+      reduced_chain_link_dict:
+              A dictionary containing link metadata per step,
+              e.g.:
+              {
+                <link name> : <Link object>,
+                ...
+              }
+      name:
+              The name that the summary link will be associated with.
+
+    <Exceptions>
+      None.
+
+    <Side Effects>
+      None.
+
+    <Returns>
+      A Link object which summarizes the materials and products of the overall
+      software supply chain.
+
+    """
+    # Create empty link object
+    summary_link = in_toto.models.link.Link()
+
+    # Take first and last link in the order the corresponding
+    # steps appear in the layout, if there are any.
+    if len(layout.steps) > 0:
+        first_step_link = reduced_chain_link_dict[layout.steps[0].name]
+        last_step_link = reduced_chain_link_dict[layout.steps[-1].name]
+
+        summary_link.materials = first_step_link.materials
+        summary_link.name = name
+
+        summary_link.products = last_step_link.products
+        summary_link.byproducts = last_step_link.byproducts
+        summary_link.command = last_step_link.command
+
+    return summary_link
+
+
+def in_toto_verify(
+    metadata,
+    layout_key_dict,
+    link_dir_path=".",
+    substitution_parameters=None,
+    step_name="",
+    persist_inspection_links=True,
+):
+    """Performs complete in-toto supply chain verification for a final product.
+
+    The verification procedure consists of the following activities, performed in
+    the given order:
+
+    1.  Verify layout signatures
+    2.  Verify layout expiration date
+    3.  Substitute placeholders in the layout
+    4.  Load link metadata
+    5.  Verify link signatures with keys in layout
+    6.  Recurse into sublayout verification
+    7.  Soft-verify alignment of reported and expected commands. Note:
+        verification does not fail if commands don't match, instead a warning is
+        logged as per the in-toto specification --
+        https://github.com/in-toto/docs/blob/master/in-toto-spec.md#431-steps
+    8.  Verify threshold artifact constraints
+    9.  Process step product and material rules
+    10. Execute inspection commands and generate inspection links
+    11. Process inspection product and material rules
+
+    Note: in-toto's verification workflow directly uses the key for verifying
+    signatures. It does not communicate with external sources of information for
+    specific attributes about keys. This ensures that verification can be
+    performed in isolation. It is the supply chain owner's responsibility to
+    consider such attributes before using the key to sign the layout or adding
+    it to the layout. For example, in-toto does not rely on the creation time,
+    revocation status, and usage flags for PGP keys. To revoke or otherwise
+    affect the usage of a key, the supply chain owner must sign a new layout
+    with the corresponding changes.
+
+    Arguments:
+      metadata: A Metadata object that contains a Layout object to be verified.
+
+      layout_key_dict: A public key dictionary. The verification routine requires
+          at least one key, and a valid signature on the layout for each key.
+
+      link_dir_path (optional): A directory path to link metadata files. The
+          expected filename format for link metadata files is
+          ``STEP-NAME.KEYID-PREFIX.link``. Link metadata files for a sublayout
+          are loaded from a subdirectory relative to the link_dir_path of the
+          superlayout. The expected directory name format is
+          ``SUBLAYOUT-STEP-NAME.KEYID-PREFIX``.
+
+      substitution_parameters (optional): A dictionary with substitution values
+          for artifact rules (steps and inspections), the expected command
+          attribute (steps), and the run attribute (inspections) in the layout.
+
+      step_name (optional): A name assigned to the returned link. This is mostly
+          useful during recursive sublayout verification.
+
+      persist_inspection_links (optional): A boolean that determines whether or
+          not link metadata files for inspection are written to cwd.
+
+    Raises:
+      securesystemslib.exceptions.FormatError: Passed parameters are malformed.
+
+      SignatureVerificationError: No layout verification key is passed, or any of
+          the passed keys fails to verify a signature.
+
+      LayoutExpiredError: The layout is expired.
+
+      LinkNotFoundError: Fewer than threshold link metadata files can be found
+          for a step of the layout.
+
+      ThresholdVerificationError: Fewer than threshold links, validly signed by
+          different authorized functionaries, who agree on the recorded materials
+          and products, can be found for a step of the layout. (Links with
+          invalid signatures or signatures by unauthorized functionaries are
+          ignored.)
+
+      RuleVerificationError: A DISALLOW rule matches disallowed artifacts, or
+          a REQUIRE rule does not find a required artifact.
+
+      BadReturnValueError: An inspection command returns a non-zero value.
+
+    Side Effects:
+      Reads link metadata files from disk.
+      Runs inspection commands in subprocess.
+
+    Returns:
+      A Link object, which summarizes the materials and products of the overall
+      software supply chain. This is mostly useful during recursive sublayout
+      verification.
+
+    """
+
+    LOG.info("Verifying layout metadata signatures...")
+    verify_metadata_signatures(metadata, layout_key_dict)
+
+    # For the rest of the verification we only care about the layout payload
+    # (Layout) that carries all the information and not about the layout
+    # container (Metablock) that also carries the signatures
+    LOG.info("Extracting layout from metadata...")
+    layout = metadata.get_payload()
+
+    LOG.info("Verifying layout expiration...")
+    verify_layout_expiration(layout)
+
+    # If there are parameters sent to the translation layer, substitute them
+    if substitution_parameters is not None:
+        LOG.info("Performing parameter substitution...")
+        substitute_parameters(layout, substitution_parameters)
+
+    LOG.info("Reading link metadata files...")
+    steps_metadata = load_links_for_layout(layout, link_dir_path)
+
+    LOG.info("Verifying link metadata signatures...")
+    steps_metadata = verify_link_signature_thresholds(layout, steps_metadata)
+
+    LOG.info("Verifying sublayouts...")
+    chain_link_dict = verify_sublayouts(layout, steps_metadata, link_dir_path)
+
+    LOG.info("Verifying alignment of reported commands...")
+    verify_all_steps_command_alignment(layout, chain_link_dict)
+
+    LOG.info("Verifying threshold constraints...")
+    verify_threshold_constraints(layout, chain_link_dict)
+    reduced_chain_link_dict = reduce_chain_links(chain_link_dict)
+
+    # NOTE: Processing step rules before executing inspections guarantees that
+    # inspection commands don't run on compromised target files, however, this
+    # also precludes step match rules from referencing inspection artifacts.
+    LOG.info("Verifying Step rules...")
+    verify_all_item_rules(layout.steps, reduced_chain_link_dict)
+
+    LOG.info("Executing Inspection commands...")
+    inspection_link_dict = run_all_inspections(layout, persist_inspection_links)
+
+    LOG.info("Verifying Inspection rules...")
+    # Artifact rules for inspections can reference links that correspond to
+    # Steps or Inspections, hence the concatenation of both collections of links
+    combined_links = reduced_chain_link_dict.copy()
+    combined_links.update(inspection_link_dict)
+    verify_all_item_rules(layout.inspect, combined_links)
+
+    # We made it this far without exception that means, verification passed
+    LOG.info("The software product passed all verification.")
+
+    # Return a link file which summarizes the entire software supply chain
+    # This is mostly relevant if the currently verified supply chain is embedded
+    # in another supply chain
+    return get_summary_link(layout, reduced_chain_link_dict, step_name)
```

### Comparing `in_toto-1.4.0/in_toto/models/_signer.py` & `in_toto-2.0.0/in_toto/models/_signer.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,238 +21,234 @@
 
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
 import securesystemslib.gpg.exceptions as gpg_exceptions
 import securesystemslib.gpg.functions as gpg
 from securesystemslib import exceptions
-from securesystemslib.signer import Key, Signature, Signer, SecretsHandler
+from securesystemslib.signer import Key, SecretsHandler, Signature, Signer
 
 
 class GPGSignature(Signature):
-  """A container class containing information about a gpg signature.
-  Besides the signature, it also contains other meta information
-  needed to uniquely identify the key used to generate the signature.
-
-  Attributes:
-    keyid: HEX string used as a unique identifier of the key.
-    signature: HEX string representing the signature.
-    other_headers: HEX representation of additional GPG headers.
-  """
-
-  def __init__(
-    self,
-    keyid: str,
-    signature: str,
-    other_headers: str,
-  ):
-    super().__init__(keyid, signature)
-    self.other_headers = other_headers
-
-  @classmethod
-  def from_dict(cls, signature_dict: Dict) -> "GPGSignature":
-    """Creates a ``GPGSignature`` object from its JSON/dict
-    representation.
-
-    Arguments:
-      signature_dict: Dict containing valid "keyid", "signature" and
-        "other_fields" fields.
-    Raises:
-      KeyError: If any of the "keyid", "sig" or "other_headers" fields
-        are missing from the signature_dict.
-    Returns:
-      ``GPGSignature`` instance.
+    """A container class containing information about a gpg signature.
+    Besides the signature, it also contains other meta information
+    needed to uniquely identify the key used to generate the signature.
+
+    Attributes:
+      keyid: HEX string used as a unique identifier of the key.
+      signature: HEX string representing the signature.
+      other_headers: HEX representation of additional GPG headers.
     """
 
-    return cls(
-      signature_dict["keyid"],
-      signature_dict["signature"],
-      signature_dict["other_headers"],
-    )
-
-  def to_dict(self) -> Dict:
-    """Returns the JSON-serializable dictionary representation of self."""
-    return {
-      "keyid": self.keyid,
-      "signature": self.signature,
-      "other_headers": self.other_headers,
-    }
+    def __init__(
+        self,
+        keyid: str,
+        signature: str,
+        other_headers: str,
+    ):
+        super().__init__(keyid, signature)
+        self.other_headers = other_headers
+
+    @classmethod
+    def from_dict(cls, signature_dict: Dict) -> "GPGSignature":
+        """Creates a ``GPGSignature`` object from its JSON/dict
+        representation.
+
+        Arguments:
+          signature_dict: Dict containing valid "keyid", "signature" and
+            "other_fields" fields.
+        Raises:
+          KeyError: If any of the "keyid", "sig" or "other_headers" fields
+            are missing from the signature_dict.
+        Returns:
+          ``GPGSignature`` instance.
+        """
+
+        return cls(
+            signature_dict["keyid"],
+            signature_dict["signature"],
+            signature_dict["other_headers"],
+        )
+
+    def to_dict(self) -> Dict:
+        """Returns the JSON-serializable dictionary representation of self."""
+        return {
+            "keyid": self.keyid,
+            "signature": self.signature,
+            "other_headers": self.other_headers,
+        }
 
 
 class GPGSigner(Signer):
-  """A in-toto gpg implementation of the ``Signer`` interface.
-  Provides a sign method to generate a cryptographic signature with gpg, using
-  an RSA, DSA or EdDSA private key identified by the keyid on the instance.
-
-  Arguments:
-    keyid: The keyid of the gpg signing keyid. If not passed the default
-      key in the keyring is used.
-    homedir: Path to the gpg keyring. If not passed the default keyring
-      is used.
-  """
-
-  def __init__(
-    self,
-    keyid: Optional[str] = None,
-    homedir: Optional[str] = None
-  ):
-    self.keyid = keyid
-    self.homedir = homedir
-
-  @classmethod
-  def from_priv_key_uri(
-    cls,
-    priv_key_uri: str,
-    public_key: Key,
-    secrets_handler: Optional[SecretsHandler] = None
-  ) -> "GPGSigner":
-
-    raise NotImplementedError(
-      "Incompatible with private key URIs")  # pragma: no cover
-
-
-  def sign(self, payload: bytes) -> GPGSignature:
-    """Signs a given payload by the key assigned to the ``GPGSigner``
-    instance. Calls the gpg command line utility to sign the passed content
-    with the key identified by the passed keyid from the gpg keyring at the
-    passed homedir.
+    """A in-toto gpg implementation of the ``Signer`` interface.
+    Provides a sign method to generate a cryptographic signature with gpg, using
+    an RSA, DSA or EdDSA private key identified by the keyid on the instance.
 
     Arguments:
-      payload: The bytes to be signed.
-    Raises:
-      securesystemslib.exceptions.FormatError:
-        If the keyid was passed and does not match
-        securesystemslib.formats.KEYID_SCHEMA.
-      ValueError: the gpg command failed to create a valid signature.
-      OSError: the gpg command is not present or non-executable.
-      securesystemslib.exceptions.UnsupportedLibraryError: the gpg command is
-        not available, or the cryptography library is not installed.
-      securesystemslib.gpg.exceptions.CommandError: the gpg command returned a
-        non-zero exit code.
-      securesystemslib.gpg.exceptions.KeyNotFoundError: the used gpg version is
-        not fully supported and no public key can be found for short keyid.
-      Returns:
-        Returns a ``GPGSignature`` class instance.
+      keyid: The keyid of the gpg signing keyid. If not passed the default
+        key in the keyring is used.
+      homedir: Path to the gpg keyring. If not passed the default keyring
+        is used.
     """
 
-    sig_dict = gpg.create_signature(payload, self.keyid, self.homedir)
-    return GPGSignature(**sig_dict)
+    def __init__(
+        self, keyid: Optional[str] = None, homedir: Optional[str] = None
+    ):
+        self.keyid = keyid
+        self.homedir = homedir
+
+    @classmethod
+    def from_priv_key_uri(
+        cls,
+        priv_key_uri: str,
+        public_key: Key,
+        secrets_handler: Optional[SecretsHandler] = None,
+    ) -> "GPGSigner":
+        raise NotImplementedError(
+            "Incompatible with private key URIs"
+        )  # pragma: no cover
+
+    def sign(self, payload: bytes) -> GPGSignature:
+        """Signs a given payload by the key assigned to the ``GPGSigner``
+        instance. Calls the gpg command line utility to sign the passed content
+        with the key identified by the passed keyid from the gpg keyring at the
+        passed homedir.
+
+        Arguments:
+          payload: The bytes to be signed.
+        Raises:
+          securesystemslib.exceptions.FormatError:
+            If the keyid was passed and does not match
+            securesystemslib.formats.KEYID_SCHEMA.
+          ValueError: the gpg command failed to create a valid signature.
+          OSError: the gpg command is not present or non-executable.
+          securesystemslib.exceptions.UnsupportedLibraryError: the gpg command is
+            not available, or the cryptography library is not installed.
+          securesystemslib.gpg.exceptions.CommandError: the gpg command returned a
+            non-zero exit code.
+          securesystemslib.gpg.exceptions.KeyNotFoundError: the used gpg version is
+            not fully supported and no public key can be found for short keyid.
+          Returns:
+            Returns a ``GPGSignature`` class instance.
+        """
+
+        sig_dict = gpg.create_signature(payload, self.keyid, self.homedir)
+        return GPGSignature(**sig_dict)
 
 
 @dataclass
 class GPGKey(Key):
-  """A container class representing public key portion of a GPG key.
-  Provides a verify method to verify a cryptographic signature with a
-  gpg-style rsa, dsa or ecdsa public key on the instance.
-
-  Attributes:
-    type: Key type, e.g. "rsa", "dsa" or "ecdsa".
-    method: GPG Key Scheme, For example:
-      "pgp+rsa-pkcsv1.5", "pgp+dsa-fips-180-2", and "pgp+eddsa-ed25519".
-    hashes: list of GPG Hash Algorithms, e.g. "pgp+SHA2".
-    keyval: Opaque key content.
-    keyid: Key identifier that is unique within the metadata it is used in.
-      Keyid is not verified to be the hash of a specific representation
-      of the key.
-    creation_time: Unix timestamp when GPG key was created.
-    validity_period: Validity of the GPG Keys in days.
-    subkeys: A dictionary containing keyid and GPG subkey.
-  """
-
-  type: str
-  method: str
-  hashes: List[str]
-  keyval: Dict[str, str]
-  keyid: str
-  creation_time: Optional[int] = None
-  validity_period: Optional[int] = None
-  subkeys: Optional[Dict[str, "GPGKey"]] = None
-
-  @classmethod
-  def from_dict(cls, keyid: str, key_dict: Dict[str, Any]):
-    """Creates ``GPGKey`` object from its json/dict representation.
-    Raises:
-      KeyError, TypeError: Invalid arguments.
-    """
-    subkeys_dict = key_dict.get("subkeys")
-
-    gpg_subkeys = None
-    if subkeys_dict:
-      gpg_subkeys = {
-        _keyid: GPGKey.from_dict(_keyid, subkey_dict)
-        for (_keyid, subkey_dict) in subkeys_dict.items()
-      }
-
-    return cls(
-      key_dict["type"],
-      key_dict["method"],
-      key_dict["hashes"],
-      key_dict["keyval"],
-      keyid,
-      key_dict.get("creation_time"),
-      key_dict.get("validity_period"),
-      gpg_subkeys,
-    )
-
-  @classmethod
-  def from_legacy_dict(cls, key_dict: Dict[str, Any]):
-    """Create GPGKey from legacy dictionary representation."""
-
-    keyid = key_dict["keyid"]
-    return cls.from_dict(keyid, key_dict)
-
-  def to_dict(self):
-    """Returns the dictionary representation of self."""
-
-    key_dict = {
-      "method": self.method,
-      "type": self.type,
-      "hashes": self.hashes,
-      "keyid": self.keyid,
-      "keyval": self.keyval,
-    }
-
-    if self.creation_time:
-      key_dict["creation_time"] = self.creation_time
-    if self.validity_period:
-      key_dict["validity_period"] = self.validity_period
-    if self.subkeys:
-      subkeys_dict = {
-        keyid: subkey.to_dict()
-        for (keyid, subkey) in self.subkeys.items()
-      }
-      key_dict["subkeys"] = subkeys_dict
-
-    return key_dict
-
-  @classmethod
-  def from_keyring(cls, keyid, homedir=None):
-    """Creates ``GPGKey`` object from GnuPG Keyring."""
-
-    pubkey_dict = gpg.export_pubkey(keyid, homedir)
-    return cls.from_dict(keyid, pubkey_dict)
-
-  def verify_signature(
-    self,
-    signature: GPGSignature,
-    data: bytes
-  ) -> None:
-    """Verifies a given payload by the key assigned to the GPGKey
-    instance.
-
-    Arguments:
-      signature: A ``GPGSignature`` class instance.
-      data: The bytes to be verified.
+    """A container class representing public key portion of a GPG key.
+    Provides a verify method to verify a cryptographic signature with a
+    gpg-style rsa, dsa or ecdsa public key on the instance.
+
+    Attributes:
+      type: Key type, e.g. "rsa", "dsa" or "ecdsa".
+      method: GPG Key Scheme, For example:
+        "pgp+rsa-pkcsv1.5", "pgp+dsa-fips-180-2", and "pgp+eddsa-ed25519".
+      hashes: list of GPG Hash Algorithms, e.g. "pgp+SHA2".
+      keyval: Opaque key content.
+      keyid: Key identifier that is unique within the metadata it is used in.
+        Keyid is not verified to be the hash of a specific representation
+        of the key.
+      creation_time: Unix timestamp when GPG key was created.
+      validity_period: Validity of the GPG Keys in days.
+      subkeys: A dictionary containing keyid and GPG subkey.
     """
 
-    try:
-      if not gpg.verify_signature(signature.to_dict(), self.to_dict(), data):
-        raise exceptions.UnverifiedSignatureError(
-          f"Failed to verify signature by {self.keyid}")
-    except (
-      exceptions.FormatError,
-      exceptions.UnsupportedLibraryError,
-      gpg_exceptions.KeyExpirationError,
-    ) as e:
-      raise exceptions.VerificationError(
-        f"Unknown failure to verify signature by {self.keyid}"
-      ) from e
+    type: str
+    method: str
+    hashes: List[str]
+    keyval: Dict[str, str]
+    keyid: str
+    creation_time: Optional[int] = None
+    validity_period: Optional[int] = None
+    subkeys: Optional[Dict[str, "GPGKey"]] = None
+
+    @classmethod
+    def from_dict(cls, keyid: str, key_dict: Dict[str, Any]):
+        """Creates ``GPGKey`` object from its json/dict representation.
+        Raises:
+          KeyError, TypeError: Invalid arguments.
+        """
+        subkeys_dict = key_dict.get("subkeys")
+
+        gpg_subkeys = None
+        if subkeys_dict:
+            gpg_subkeys = {
+                _keyid: GPGKey.from_dict(_keyid, subkey_dict)
+                for (_keyid, subkey_dict) in subkeys_dict.items()
+            }
+
+        return cls(
+            key_dict["type"],
+            key_dict["method"],
+            key_dict["hashes"],
+            key_dict["keyval"],
+            keyid,
+            key_dict.get("creation_time"),
+            key_dict.get("validity_period"),
+            gpg_subkeys,
+        )
+
+    @classmethod
+    def from_legacy_dict(cls, key_dict: Dict[str, Any]):
+        """Create GPGKey from legacy dictionary representation."""
+
+        keyid = key_dict["keyid"]
+        return cls.from_dict(keyid, key_dict)
+
+    def to_dict(self):
+        """Returns the dictionary representation of self."""
+
+        key_dict = {
+            "method": self.method,
+            "type": self.type,
+            "hashes": self.hashes,
+            "keyid": self.keyid,
+            "keyval": self.keyval,
+        }
+
+        if self.creation_time:
+            key_dict["creation_time"] = self.creation_time
+        if self.validity_period:
+            key_dict["validity_period"] = self.validity_period
+        if self.subkeys:
+            subkeys_dict = {
+                keyid: subkey.to_dict()
+                for (keyid, subkey) in self.subkeys.items()
+            }
+            key_dict["subkeys"] = subkeys_dict
+
+        return key_dict
+
+    @classmethod
+    def from_keyring(cls, keyid, homedir=None):
+        """Creates ``GPGKey`` object from GnuPG Keyring."""
+
+        pubkey_dict = gpg.export_pubkey(keyid, homedir)
+        return cls.from_dict(keyid, pubkey_dict)
+
+    def verify_signature(self, signature: GPGSignature, data: bytes) -> None:
+        """Verifies a given payload by the key assigned to the GPGKey
+        instance.
+
+        Arguments:
+          signature: A ``GPGSignature`` class instance.
+          data: The bytes to be verified.
+        """
+
+        try:
+            if not gpg.verify_signature(
+                signature.to_dict(), self.to_dict(), data
+            ):
+                raise exceptions.UnverifiedSignatureError(
+                    f"Failed to verify signature by {self.keyid}"
+                )
+        except (
+            exceptions.FormatError,
+            exceptions.UnsupportedLibraryError,
+            gpg_exceptions.KeyExpirationError,
+        ) as e:
+            raise exceptions.VerificationError(
+                f"Unknown failure to verify signature by {self.keyid}"
+            ) from e
```

### Comparing `in_toto-1.4.0/in_toto/models/common.py` & `in_toto-2.0.0/in_toto/models/common.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,48 +16,49 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Provides base classes for various classes in the model.
 
 """
 
+import inspect
 import json
+
 import attr
-import inspect
 import securesystemslib.formats
 
 
-
 class ValidationMixin(object):
-  """ The validation mixin provides a self-inspecting method, validate, to
-  allow in-toto's objects to check that they are proper. """
-
-  def validate(self):
-    """Validates attributes of the instance.
+    """The validation mixin provides a self-inspecting method, validate, to
+    allow in-toto's objects to check that they are proper."""
 
-    Raises:
-      securesystemslib.formats.FormatError: An attribute value is invalid.
+    def validate(self):
+        """Validates attributes of the instance.
 
-    """
-    for method in inspect.getmembers(self, predicate=inspect.ismethod):
-      if method[0].startswith("_validate_"):
-        method[1]()
+        Raises:
+          securesystemslib.formats.FormatError: An attribute value is invalid.
 
+        """
+        for method in inspect.getmembers(self, predicate=inspect.ismethod):
+            if method[0].startswith("_validate_"):
+                method[1]()
 
 
 @attr.s(repr=False, init=False)
 class Signable(ValidationMixin):
-  """Objects with base class Signable are to be included in a Metablock class
-  to be signed (hence the name). They provide a `signable_bytes` property
-  used to create deterministic signatures. """
-
-  def __repr__(self):
-    """Returns an indented JSON string of the metadata object. """
-    return json.dumps(attr.asdict(self),
-        indent=1, separators=(",", ": "), sort_keys=True)
-
-  @property
-  def signable_bytes(self):
-    """The UTF-8 encoded canonical JSON byte representation of the dictionary
-    representation of the instance. """
-    return securesystemslib.formats.encode_canonical(
-        attr.asdict(self)).encode("UTF-8")
+    """Objects with base class Signable are to be included in a Metablock class
+    to be signed (hence the name). They provide a `signable_bytes` property
+    used to create deterministic signatures."""
+
+    def __repr__(self):
+        """Returns an indented JSON string of the metadata object."""
+        return json.dumps(
+            attr.asdict(self), indent=1, separators=(",", ": "), sort_keys=True
+        )
+
+    @property
+    def signable_bytes(self):
+        """The UTF-8 encoded canonical JSON byte representation of the dictionary
+        representation of the instance."""
+        return securesystemslib.formats.encode_canonical(
+            attr.asdict(self)
+        ).encode("UTF-8")
```

### Comparing `in_toto-1.4.0/in_toto/models/layout.py` & `in_toto-2.0.0/in_toto/models/layout.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,727 +28,712 @@
   Step:
       represents one step of the software supply chain, performed by one or
       many functionaries, who are identified by a key also stored to the layout
 
   Inspection:
       represents a hook that is run at verification
 """
-import attr
-import shlex
 import json
-
+import shlex
 from datetime import datetime
-from dateutil.relativedelta import relativedelta
-from dateutil.parser import parse
-
-from in_toto.models.common import Signable, ValidationMixin
-import in_toto.rulelib
-import in_toto.exceptions
 
+import attr
 import securesystemslib.exceptions
 import securesystemslib.formats
-import securesystemslib.schema
-import securesystemslib.interface
 import securesystemslib.gpg.functions
+import securesystemslib.interface
+import securesystemslib.schema
+from dateutil.parser import parse
+from dateutil.relativedelta import relativedelta
 
+import in_toto.exceptions
+import in_toto.rulelib
+from in_toto.models.common import Signable, ValidationMixin
 
 # Link metadata for sublayouts are expected to be found in a subdirectory
 # with the following name, relative to the verification directory
 SUBLAYOUT_LINK_DIR_FORMAT = "{name}.{keyid:.8}"
 
 
-
 @attr.s(repr=False, init=False)
 class Layout(Signable):
-  """A definition for a software supply chain.
+    """A definition for a software supply chain.
 
-  A layout lists the sequence of steps of the software supply chain in the
-  order they are expected to be performed, the functionaries authorized and
-  required to perform them, and inspections to be performed by the client upon
-  final product verification.
+    A layout lists the sequence of steps of the software supply chain in the
+    order they are expected to be performed, the functionaries authorized and
+    required to perform them, and inspections to be performed by the client upon
+    final product verification.
 
-  A Layout object is usually contained in a generic Metablock object for
-  signing, serialization and I/O capabilities.
+    A Layout object is usually contained in a generic Metablock object for
+    signing, serialization and I/O capabilities.
 
-  Attributes:
-    steps: A list of Step objects.
+    Attributes:
+      steps: A list of Step objects.
 
-    inspect: A list of Inspection objects.
+      inspect: A list of Inspection objects.
 
-    keys: A dictionary of functionary public keys, with keyids as dict keys and
-        keys as values.
+      keys: A dictionary of functionary public keys, with keyids as dict keys and
+          keys as values.
 
-    expires: The layout expiration.
+      expires: The layout expiration.
 
-    readme: A human readable description of the software supply chain.
-
-  """
-  _type = attr.ib()
-  steps = attr.ib()
-  inspect = attr.ib()
-  keys = attr.ib()
-  expires = attr.ib()
-  readme = attr.ib()
-
-
-  def __init__(self, **kwargs):
-    super(Layout, self).__init__()
-    self._type = "layout"
-    self.steps = kwargs.get("steps", [])
-    self.inspect = kwargs.get("inspect", [])
-    self.keys = kwargs.get("keys", {})
-    self.readme = kwargs.get("readme", "")
-
-    # Assign a default expiration (one month) if not expiration date is passed
-    # TODO: Is one month a sensible default? In any case, we need a valid
-    # expiration date in order for the layout object to validate.
-    # (see self._validate_expires)
-    self.expires = kwargs.get("expires")
-    if not self.expires:
-      self.set_relative_expiration(months=1)
-
-    # TODO: Should we validate in the constructor or allow the user to create
-    # an invalid layout and call validate explicitly?
-    self.validate()
-
-
-  @property
-  def type_(self):
-    """The string "layout" to indentify the in-toto metadata type."""
-    # NOTE: We expose the type_ property in the API documentation instead of
-    # _type to protect it against modification.
-    # NOTE: Trailing underscore is used by convention (pep8) to avoid conflict
-    # with Python's type keyword.
-    return self._type
-
-
-  @staticmethod
-  def read(data):
-    """Creates a Layout object from its dictionary representation.
-
-    Arguments:
-      data: A dictionary with layout metadata fields.
-
-    Raises:
-      securesystemslib.exceptions.FormatError: Passed data is invalid.
-
-    Returns:
-      The created Layout object.
+      readme: A human readable description of the software supply chain.
 
     """
-    steps = []
 
-    for step_data in data.get("steps"):
-      steps.append(Step.read(step_data))
-    data["steps"] = steps
+    _type = attr.ib()
+    steps = attr.ib()
+    inspect = attr.ib()
+    keys = attr.ib()
+    expires = attr.ib()
+    readme = attr.ib()
 
-    inspections = []
-    for inspect_data in data.get("inspect"):
-      inspections.append(Inspection.read(inspect_data))
-    data["inspect"] = inspections
+    def __init__(self, **kwargs):
+        super(Layout, self).__init__()
+        self._type = "layout"
+        self.steps = kwargs.get("steps", [])
+        self.inspect = kwargs.get("inspect", [])
+        self.keys = kwargs.get("keys", {})
+        self.readme = kwargs.get("readme", "")
 
-    return Layout(**data)
+        # Assign a default expiration (one month) if not expiration date is passed
+        # TODO: Is one month a sensible default? In any case, we need a valid
+        # expiration date in order for the layout object to validate.
+        # (see self._validate_expires)
+        self.expires = kwargs.get("expires")
+        if not self.expires:
+            self.set_relative_expiration(months=1)
 
+        # TODO: Should we validate in the constructor or allow the user to create
+        # an invalid layout and call validate explicitly?
+        self.validate()
 
-  def set_relative_expiration(self, days=0, months=0, years=0):
-    """Sets layout expiration relative to today.
+    @property
+    def type_(self):
+        """The string "layout" to indentify the in-toto metadata type."""
+        # NOTE: We expose the type_ property in the API documentation instead of
+        # _type to protect it against modification.
+        # NOTE: Trailing underscore is used by convention (pep8) to avoid conflict
+        # with Python's type keyword.
+        return self._type
 
-    If not argument is passed the set exipration date is now.
+    @staticmethod
+    def read(data):
+        """Creates a Layout object from its dictionary representation.
 
-    Arguments:
-      days (optional): Days from today.
-      months (optional): Months from today.
-      years (optional): Years from today.
+        Arguments:
+          data: A dictionary with layout metadata fields.
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Arguments are not ints.
+        Raises:
+          securesystemslib.exceptions.FormatError: Passed data is invalid.
 
-    """
-    securesystemslib.schema.Integer().check_match(days)
-    securesystemslib.schema.Integer().check_match(months)
-    securesystemslib.schema.Integer().check_match(years)
+        Returns:
+          The created Layout object.
 
-    self.expires = (datetime.today() + relativedelta(
-        days=days, months=months, years=years)).strftime("%Y-%m-%dT%H:%M:%SZ")
+        """
+        steps = []
 
+        for step_data in data.get("steps"):
+            steps.append(Step.read(step_data))
+        data["steps"] = steps
 
-  def get_step_name_list(self):
-    """Returns ordered list of step names as they appear in the layout.
+        inspections = []
+        for inspect_data in data.get("inspect"):
+            inspections.append(Inspection.read(inspect_data))
+        data["inspect"] = inspections
 
-    Returns:
-      A list of step names.
+        return Layout(**data)
 
-    """
-    step_names = []
-    for step in self.steps:
-      step_names.append(step.name)
+    def set_relative_expiration(self, days=0, months=0, years=0):
+        """Sets layout expiration relative to today.
 
-    return step_names
+        If not argument is passed the set exipration date is now.
 
+        Arguments:
+          days (optional): Days from today.
+          months (optional): Months from today.
+          years (optional): Years from today.
 
-  def get_step_by_name(self, step_name):
-    """Returns step identified by step_name from the layout.
+        Raises:
+          securesystemslib.exceptions.FormatError: Arguments are not ints.
 
-    NOTE: Returns the first step identified only, which should be the only step
-    for a given name of a valid layout.
+        """
+        securesystemslib.schema.Integer().check_match(days)
+        securesystemslib.schema.Integer().check_match(months)
+        securesystemslib.schema.Integer().check_match(years)
 
-    Arguments:
-      step_name: A step name.
+        self.expires = (
+            datetime.today()
+            + relativedelta(days=days, months=months, years=years)
+        ).strftime("%Y-%m-%dT%H:%M:%SZ")
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is not a string.
+    def get_step_name_list(self):
+        """Returns ordered list of step names as they appear in the layout.
 
-    Returns:
-      A Step object.
+        Returns:
+          A list of step names.
 
-    """
-    securesystemslib.schema.AnyString().check_match(step_name)
+        """
+        step_names = []
+        for step in self.steps:
+            step_names.append(step.name)
 
-    for step in self.steps: # pragma: no branch
-      if step.name == step_name:
-        return step
+        return step_names
 
+    def get_step_by_name(self, step_name):
+        """Returns step identified by step_name from the layout.
 
-  def remove_step_by_name(self, step_name):
-    """Removes steps identified by step_name from the layout.
+        NOTE: Returns the first step identified only, which should be the only step
+        for a given name of a valid layout.
 
-    NOTE: Removes all steps identified, which should be only one step for a
-    given name of a valid layout.
+        Arguments:
+          step_name: A step name.
 
-    Arguments:
-      step_name: A step name.
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is not a string.
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is not a string.
+        Returns:
+          A Step object.
 
-    """
-    securesystemslib.schema.AnyString().check_match(step_name)
+        """
+        securesystemslib.schema.AnyString().check_match(step_name)
 
-    for step in self.steps:
-      if step.name == step_name:
-        self.steps.remove(step)
+        for step in self.steps:  # pragma: no branch
+            if step.name == step_name:
+                return step
 
+    def remove_step_by_name(self, step_name):
+        """Removes steps identified by step_name from the layout.
 
-  def get_inspection_name_list(self):
-    """Returns ordered list of inspection names as they appear in the layout.
+        NOTE: Removes all steps identified, which should be only one step for a
+        given name of a valid layout.
 
-    Returns:
-      A list of inspection names.
+        Arguments:
+          step_name: A step name.
 
-    """
-    inspection_names = []
-    for inspection in self.inspect:
-      inspection_names.append(inspection.name)
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is not a string.
 
-    return inspection_names
+        """
+        securesystemslib.schema.AnyString().check_match(step_name)
 
+        for step in self.steps:
+            if step.name == step_name:
+                self.steps.remove(step)
 
-  def get_inspection_by_name(self, inspection_name):
-    """Returns inspection identified by inspection_names from the layout.
+    def get_inspection_name_list(self):
+        """Returns ordered list of inspection names as they appear in the layout.
 
-    NOTE: Returns the first inspection identified only, which should be the
-    only inspection for a given name of a valid layout.
+        Returns:
+          A list of inspection names.
 
-    Arguments:
-      inspection_name: An inspection name.
+        """
+        inspection_names = []
+        for inspection in self.inspect:
+            inspection_names.append(inspection.name)
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is not a string.
+        return inspection_names
 
-    Returns:
-      An Inspection object.
+    def get_inspection_by_name(self, inspection_name):
+        """Returns inspection identified by inspection_names from the layout.
 
-    """
-    securesystemslib.schema.AnyString().check_match(inspection_name)
+        NOTE: Returns the first inspection identified only, which should be the
+        only inspection for a given name of a valid layout.
 
-    for inspection in self.inspect: # pragma: no branch
-      if inspection.name == inspection_name:
-        return inspection
+        Arguments:
+          inspection_name: An inspection name.
 
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is not a string.
 
-  def remove_inspection_by_name(self, inspection_name):
-    """Removes inspections identified by inspection_name from the layout.
+        Returns:
+          An Inspection object.
 
-    NOTE: Removes all inspections identified, which should be only one
-    inspection for a given name of a valid layout.
+        """
+        securesystemslib.schema.AnyString().check_match(inspection_name)
 
-    Arguments:
-      inspection_name: An inspection name.
+        for inspection in self.inspect:  # pragma: no branch
+            if inspection.name == inspection_name:
+                return inspection
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is not a string.
+    def remove_inspection_by_name(self, inspection_name):
+        """Removes inspections identified by inspection_name from the layout.
 
-    """
-    securesystemslib.schema.AnyString().check_match(inspection_name)
+        NOTE: Removes all inspections identified, which should be only one
+        inspection for a given name of a valid layout.
 
-    for inspection in self.inspect:
-      if inspection.name == inspection_name:
-        self.inspect.remove(inspection)
+        Arguments:
+          inspection_name: An inspection name.
 
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is not a string.
 
-  def get_functionary_key_id_list(self):
-    """Returns list of functionary keyids from the layout.
+        """
+        securesystemslib.schema.AnyString().check_match(inspection_name)
 
-    Returns:
-      A list of keyids.
+        for inspection in self.inspect:
+            if inspection.name == inspection_name:
+                self.inspect.remove(inspection)
 
-    """
-    return list(self.keys.keys())
+    def get_functionary_key_id_list(self):
+        """Returns list of functionary keyids from the layout.
 
+        Returns:
+          A list of keyids.
 
-  def add_functionary_key(self, key):
-    """Adds key as functionary key to layout.
+        """
+        return list(self.keys.keys())
 
-    Arguments:
-      key: A public key. Format is securesystemslib.formats.ANY_PUBKEY_SCHEMA.
+    def add_functionary_key(self, key):
+        """Adds key as functionary key to layout.
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is malformed.
+        Arguments:
+          key: A public key. Format is securesystemslib.formats.ANY_PUBKEY_SCHEMA.
 
-    Returns:
-      The added key.
-
-    """
-    securesystemslib.formats.ANY_PUBKEY_SCHEMA.check_match(key)
-    keyid = key["keyid"]
-    self.keys[keyid] = key
-    return key
-
-
-  def add_functionary_key_from_path(self, key_path):
-    """Loads key from disk and adds as functionary key to layout.
-
-    Arguments:
-      key_path: A path to a PEM-formatted RSA public key. Format is
-          securesystemslib.formats.PATH_SCHEMA.
-
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is malformed.
-      securesystemslib.exceptions.Error: Key cannot be imported.
-
-    Returns:
-      The added functionary public key.
-
-    """
-    securesystemslib.formats.PATH_SCHEMA.check_match(key_path)
-    key = securesystemslib.interface.import_rsa_publickey_from_file(key_path)
-
-    return self.add_functionary_key(key)
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is malformed.
 
+        Returns:
+          The added key.
 
+        """
+        securesystemslib.formats.ANY_PUBKEY_SCHEMA.check_match(key)
+        keyid = key["keyid"]
+        self.keys[keyid] = key
+        return key
 
-  def add_functionary_key_from_gpg_keyid(self, gpg_keyid, gpg_home=None):
-    """Loads key from gpg keychain and adds as functionary key to layout.
+    def add_functionary_key_from_path(self, key_path):
+        """Loads key from disk and adds as functionary key to layout.
 
-    Arguments:
-      gpg_keyid: A keyid used to identify a local gpg public key.
-      gpg_home (optional): A path to the gpg home directory. If not set the
-          default gpg home directory is used.
+        Arguments:
+          key_path: A path to a PEM-formatted RSA public key. Format is
+              securesystemslib.formats.PATH_SCHEMA.
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Arguments are malformed.
-      securesystemslib.gpg.execeptions.KeyNotFoundError: Key cannot be found.
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is malformed.
+          securesystemslib.exceptions.Error: Key cannot be imported.
 
-    Side Effects:
-      Calls system gpg command in a subprocess.
+        Returns:
+          The added functionary public key.
 
-    Returns:
-      The added key.
-
-    """
-    securesystemslib.formats.KEYID_SCHEMA.check_match(gpg_keyid)
-    if gpg_home: # pragma: no branch
-      securesystemslib.formats.PATH_SCHEMA.check_match(gpg_home)
-
-    key = securesystemslib.gpg.functions.export_pubkey(gpg_keyid,
-        homedir=gpg_home)
-    return self.add_functionary_key(key)
-
-
-  def add_functionary_keys_from_paths(self, key_path_list):
-    """Loads keys from disk and adds as functionary keys to layout.
-
-    Arguments:
-      key_path_list: A list of paths to PEM-formatted RSA public keys. Format
-          of each path is securesystemslib.formats.PATH_SCHEMA.
-
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is malformed.
-      securesystemslib.exceptions.Error: A key cannot be imported.
-
-    Returns:
-      A dictionary of the added functionary keys, with keyids as dictionary
-      keys and keys as values.
-
-    """
-    securesystemslib.formats.PATHS_SCHEMA.check_match(key_path_list)
-    key_dict = {}
-    for key_path in key_path_list:
-      key = self.add_functionary_key_from_path(key_path)
-      key_dict[key["keyid"]] = key
-
-    return key_dict
-
-
-  def add_functionary_keys_from_gpg_keyids(self, gpg_keyid_list,
-      gpg_home=None):
-    """Loads keys from gpg keychain and adds as functionary keys to layout.
-
-    Arguments:
-      gpg_keyid_list: A list of keyids used to identify local gpg public keys.
-      gpg_home (optional): A path to the gpg home directory. If not set the
-          default gpg home directory is used.
-
-    Raises:
-      securesystemslib.exceptions.FormatError: Arguments are malformed.
-      securesystemslib.gpg.execeptions.KeyNotFoundError: A key cannot be found.
-
-    Side Effects:
-      Calls system gpg command in a subprocess.
-
-    Returns:
-      A dictionary of the added functionary keys, with keyids as dictionary
-      keys and keys as values.
+        """
+        securesystemslib.formats.PATH_SCHEMA.check_match(key_path)
+        key = securesystemslib.interface.import_rsa_publickey_from_file(
+            key_path
+        )
 
-    """
-    securesystemslib.formats.KEYIDS_SCHEMA.check_match(gpg_keyid_list)
-    key_dict = {}
-    for gpg_keyid in gpg_keyid_list:
-      key = self.add_functionary_key_from_gpg_keyid(gpg_keyid, gpg_home)
-      key_dict[key["keyid"]] = key
-
-    return key_dict
-
-
-  def _validate_type(self):
-    """Private method to check that the type string is set to layout."""
-    if self._type != "layout":
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid _type value for layout (Should be 'layout')")
-
-
-  def _validate_expires(self):
-    """Private method to verify if the expiration field has the right format
-    and can be parsed."""
-    try:
-      # We do both 'parse' and 'check_match' because the format check does not
-      # detect bogus dates (e.g. Jan 35th) and parse can do more formats.
-      parse(self.expires)
-      securesystemslib.formats.ISO8601_DATETIME_SCHEMA.check_match(
-          self.expires)
-    except Exception as e:
-      raise securesystemslib.exceptions.FormatError(
-          "Malformed date string in layout. Exception: {}".format(e))
-
-
-  def _validate_readme(self):
-    """Private method to check that the readme field is a string."""
-    if not isinstance(self.readme, str):
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid readme '{}', value must be a string."
-          .format(self.readme))
-
-
-  def _validate_keys(self):
-    """Private method to ensure that the keys contained are right."""
-    securesystemslib.formats.ANY_PUBKEY_DICT_SCHEMA.check_match(self.keys)
-
-
-  def _validate_steps_and_inspections(self):
-    """Private method to verify that the list of steps and inspections are
-    correctly formed."""
-    names_seen = set()
-    if not isinstance(self.steps, list):
-      raise securesystemslib.exceptions.FormatError(
-          "The steps field should be a list!")
-
-    for step in self.steps:
-      if not isinstance(step, Step):
-        raise securesystemslib.exceptions.FormatError(
-            "The steps list should only contain steps!")
-
-      step.validate()
-
-      if step.name in names_seen:
-        raise securesystemslib.exceptions.FormatError(
-            "There is already a step with name '{}'. Step names must be"
-            " unique within a layout.".format(step.name))
-      names_seen.add(step.name)
-
-    if not isinstance(self.inspect, list):
-      raise securesystemslib.exceptions.FormatError(
-          "The inspect field should a be a list!")
-
-    for inspection in self.inspect:
-      if not isinstance(inspection, Inspection):
-        raise securesystemslib.exceptions.FormatError(
-            "The inspect list should only contain inspections!")
-
-      inspection.validate()
-
-      if inspection.name in names_seen:
-        raise securesystemslib.exceptions.FormatError(
-            "There is already an inspection with name '{}'. Inspection names"
-            " must be unique within a layout.".format(inspection.name))
-      names_seen.add(inspection.name)
+        return self.add_functionary_key(key)
 
+    def add_functionary_key_from_gpg_keyid(self, gpg_keyid, gpg_home=None):
+        """Loads key from gpg keychain and adds as functionary key to layout.
 
+        Arguments:
+          gpg_keyid: A keyid used to identify a local gpg public key.
+          gpg_home (optional): A path to the gpg home directory. If not set the
+              default gpg home directory is used.
 
-@attr.s(repr=False, init=False)
-class SupplyChainItem(ValidationMixin):
-  """Common attributes and methods for supply chain steps and inspections.
+        Raises:
+          securesystemslib.exceptions.FormatError: Arguments are malformed.
+          securesystemslib.gpg.execeptions.KeyNotFoundError: Key cannot be found.
 
-  Attributes:
-    name: A unique named used to associate related link metadata.
+        Side Effects:
+          Calls system gpg command in a subprocess.
 
-    expected_materials: A list of rules to encode expectations about used
-        artifacts (see ``rulelib`` for formats).
+        Returns:
+          The added key.
 
-    expected_products:  A list of rules to encode expectations about produced
-        artifacts (see ``rulelib`` for formats).
+        """
+        securesystemslib.formats.KEYID_SCHEMA.check_match(gpg_keyid)
+        if gpg_home:  # pragma: no branch
+            securesystemslib.formats.PATH_SCHEMA.check_match(gpg_home)
 
-  """
-  name = attr.ib()
-  expected_materials = attr.ib()
-  expected_products = attr.ib()
+        key = securesystemslib.gpg.functions.export_pubkey(
+            gpg_keyid, homedir=gpg_home
+        )
+        return self.add_functionary_key(key)
 
+    def add_functionary_keys_from_paths(self, key_path_list):
+        """Loads keys from disk and adds as functionary keys to layout.
 
-  def __init__(self, **kwargs):
-    super(SupplyChainItem, self).__init__()
-    self.name = kwargs.get("name")
-    self.expected_materials = kwargs.get("expected_materials", [])
-    self.expected_products = kwargs.get("expected_products", [])
+        Arguments:
+          key_path_list: A list of paths to PEM-formatted RSA public keys. Format
+              of each path is securesystemslib.formats.PATH_SCHEMA.
 
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is malformed.
+          securesystemslib.exceptions.Error: A key cannot be imported.
 
-  def __repr__(self):
-    """Returns an indented JSON string of the metadata object. """
-    return json.dumps(attr.asdict(self),
-        indent=1, separators=(",", ": "), sort_keys=True)
+        Returns:
+          A dictionary of the added functionary keys, with keyids as dictionary
+          keys and keys as values.
 
+        """
+        securesystemslib.formats.PATHS_SCHEMA.check_match(key_path_list)
+        key_dict = {}
+        for key_path in key_path_list:
+            key = self.add_functionary_key_from_path(key_path)
+            key_dict[key["keyid"]] = key
 
-  def add_material_rule_from_string(self, rule_string):
-    """Parse artifact rule string as list and add to expected_materials.
+        return key_dict
 
-    Arguments:
-      rule_string: An artifact rule string (see ``rulelib`` for formats).
+    def add_functionary_keys_from_gpg_keyids(
+        self, gpg_keyid_list, gpg_home=None
+    ):
+        """Loads keys from gpg keychain and adds as functionary keys to layout.
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is malformed.
+        Arguments:
+          gpg_keyid_list: A list of keyids used to identify local gpg public keys.
+          gpg_home (optional): A path to the gpg home directory. If not set the
+              default gpg home directory is used.
 
-    """
-    securesystemslib.schema.AnyString().check_match(rule_string)
-    rule_list = shlex.split(rule_string)
+        Raises:
+          securesystemslib.exceptions.FormatError: Arguments are malformed.
+          securesystemslib.gpg.execeptions.KeyNotFoundError: A key cannot be found.
 
-    # Raises format error if the parsed rule_string is not a valid rule
-    in_toto.rulelib.unpack_rule(rule_list)
+        Side Effects:
+          Calls system gpg command in a subprocess.
 
-    self.expected_materials.append(rule_list)
+        Returns:
+          A dictionary of the added functionary keys, with keyids as dictionary
+          keys and keys as values.
 
+        """
+        securesystemslib.formats.KEYIDS_SCHEMA.check_match(gpg_keyid_list)
+        key_dict = {}
+        for gpg_keyid in gpg_keyid_list:
+            key = self.add_functionary_key_from_gpg_keyid(gpg_keyid, gpg_home)
+            key_dict[key["keyid"]] = key
 
-  def add_product_rule_from_string(self, rule_string):
-    """Parse artifact rule string as list and add to expected_products.
+        return key_dict
 
-    Arguments:
-      rule_string: An artifact rule string (see ``rulelib`` for formats).
+    def _validate_type(self):
+        """Private method to check that the type string is set to layout."""
+        if self._type != "layout":
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid _type value for layout (Should be 'layout')"
+            )
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is malformed.
+    def _validate_expires(self):
+        """Private method to verify if the expiration field has the right format
+        and can be parsed."""
+        try:
+            # We do both 'parse' and 'check_match' because the format check does not
+            # detect bogus dates (e.g. Jan 35th) and parse can do more formats.
+            parse(self.expires)
+            securesystemslib.formats.ISO8601_DATETIME_SCHEMA.check_match(
+                self.expires
+            )
+        except Exception as e:
+            raise securesystemslib.exceptions.FormatError(
+                "Malformed date string in layout. Exception: {}".format(e)
+            )
 
-    """
-    securesystemslib.schema.AnyString().check_match(rule_string)
-    rule_list = shlex.split(rule_string)
+    def _validate_readme(self):
+        """Private method to check that the readme field is a string."""
+        if not isinstance(self.readme, str):
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid readme '{}', value must be a string.".format(
+                    self.readme
+                )
+            )
 
-    # Raises format error if the parsed rule_string is not a valid rule
-    in_toto.rulelib.unpack_rule(rule_list)
+    def _validate_keys(self):
+        """Private method to ensure that the keys contained are right."""
+        securesystemslib.formats.ANY_PUBKEY_DICT_SCHEMA.check_match(self.keys)
 
-    self.expected_products.append(rule_list)
+    def _validate_steps_and_inspections(self):
+        """Private method to verify that the list of steps and inspections are
+        correctly formed."""
+        names_seen = set()
+        if not isinstance(self.steps, list):
+            raise securesystemslib.exceptions.FormatError(
+                "The steps field should be a list!"
+            )
 
+        for step in self.steps:
+            if not isinstance(step, Step):
+                raise securesystemslib.exceptions.FormatError(
+                    "The steps list should only contain steps!"
+                )
 
-  def _validate_expected_materials(self):
-    """Private method to check that material rules are correctly formed."""
-    if not isinstance(self.expected_materials, list):
-      raise securesystemslib.exceptions.FormatError(
-          "Material rules should be a list!")
+            step.validate()
 
-    for rule in self.expected_materials:
-      in_toto.rulelib.unpack_rule(rule)
+            if step.name in names_seen:
+                raise securesystemslib.exceptions.FormatError(
+                    "There is already a step with name '{}'. Step names must be"
+                    " unique within a layout.".format(step.name)
+                )
+            names_seen.add(step.name)
 
+        if not isinstance(self.inspect, list):
+            raise securesystemslib.exceptions.FormatError(
+                "The inspect field should a be a list!"
+            )
 
-  def _validate_expected_products(self):
-    """Private method to check that product rules are correctly formed."""
-    if not isinstance(self.expected_products, list):
-      raise securesystemslib.exceptions.FormatError(
-          "Product rules should be a list!")
+        for inspection in self.inspect:
+            if not isinstance(inspection, Inspection):
+                raise securesystemslib.exceptions.FormatError(
+                    "The inspect list should only contain inspections!"
+                )
 
-    for rule in self.expected_products:
-      in_toto.rulelib.unpack_rule(rule)
+            inspection.validate()
 
+            if inspection.name in names_seen:
+                raise securesystemslib.exceptions.FormatError(
+                    "There is already an inspection with name '{}'. Inspection names"
+                    " must be unique within a layout.".format(inspection.name)
+                )
+            names_seen.add(inspection.name)
 
 
 @attr.s(repr=False, init=False)
-class Step(SupplyChainItem):
-  """A step of a software supply chain.
-
-  A Step object is usually contained in a Layout object and encodes the
-  expectations for a step of the software supply chain such as, who is
-  authorized to perform the step, what command is executed, and which artifacts
-  are used and produced. Evidence about a performed step is provided by link
-  metadata.
-
-  Attributes:
-    pubkeys: A list of functionary keyids authorized to perform the step.
-
-    threshold: A minimum number of distinct functionaries required to provide
-        evidence for a step.
+class SupplyChainItem(ValidationMixin):
+    """Common attributes and methods for supply chain steps and inspections.
 
-    expected_command: A list of command and command arguments, expected to
-        perform the step.
+    Attributes:
+      name: A unique named used to associate related link metadata.
 
-  """
-  _type = attr.ib()
-  pubkeys = attr.ib()
-  expected_command = attr.ib()
-  threshold = attr.ib()
+      expected_materials: A list of rules to encode expectations about used
+          artifacts (see ``rulelib`` for formats).
 
+      expected_products:  A list of rules to encode expectations about produced
+          artifacts (see ``rulelib`` for formats).
 
-  def __init__(self, **kwargs):
-    super(Step, self).__init__(**kwargs)
-    self._type = "step"
-    self.pubkeys = kwargs.get("pubkeys", [])
-    self.expected_command = kwargs.get("expected_command", [])
-    self.threshold = kwargs.get("threshold", 1)
+    """
 
-    self.validate()
+    name = attr.ib()
+    expected_materials = attr.ib()
+    expected_products = attr.ib()
 
+    def __init__(self, **kwargs):
+        super(SupplyChainItem, self).__init__()
+        self.name = kwargs.get("name")
+        self.expected_materials = kwargs.get("expected_materials", [])
+        self.expected_products = kwargs.get("expected_products", [])
 
-  @staticmethod
-  def read(data):
-    """Creates a Step object from its dictionary representation.
+    def __repr__(self):
+        """Returns an indented JSON string of the metadata object."""
+        return json.dumps(
+            attr.asdict(self), indent=1, separators=(",", ": "), sort_keys=True
+        )
 
-    Arguments:
-      data: A dictionary with step metadata fields.
+    def add_material_rule_from_string(self, rule_string):
+        """Parse artifact rule string as list and add to expected_materials.
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Passed data is invalid.
+        Arguments:
+          rule_string: An artifact rule string (see ``rulelib`` for formats).
 
-    Returns:
-      The created Step object.
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is malformed.
 
-    """
-    return Step(**data)
+        """
+        securesystemslib.schema.AnyString().check_match(rule_string)
+        rule_list = shlex.split(rule_string)
 
+        # Raises format error if the parsed rule_string is not a valid rule
+        in_toto.rulelib.unpack_rule(rule_list)
 
-  def set_expected_command_from_string(self, command_string):
-    """Parse command string as list and assign to expected_command.
+        self.expected_materials.append(rule_list)
 
-    Arguments:
-      command_string: A command and command arguments string.
+    def add_product_rule_from_string(self, rule_string):
+        """Parse artifact rule string as list and add to expected_products.
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is malformed.
+        Arguments:
+          rule_string: An artifact rule string (see ``rulelib`` for formats).
 
-    """
-    securesystemslib.schema.AnyString().check_match(command_string)
-    self.expected_command = shlex.split(command_string)
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is malformed.
 
+        """
+        securesystemslib.schema.AnyString().check_match(rule_string)
+        rule_list = shlex.split(rule_string)
 
-  def _validate_type(self):
-    """Private method to ensure that the type field is set to step."""
-    if self._type != "step":
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid _type value for step (Should be 'step')")
+        # Raises format error if the parsed rule_string is not a valid rule
+        in_toto.rulelib.unpack_rule(rule_list)
 
+        self.expected_products.append(rule_list)
 
-  def _validate_threshold(self):
-    """Private method to check that the threshold field is set to an int."""
-    if not isinstance(self.threshold, int):
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid threshold '{}', value must be an int."
-          .format(self.threshold))
+    def _validate_expected_materials(self):
+        """Private method to check that material rules are correctly formed."""
+        if not isinstance(self.expected_materials, list):
+            raise securesystemslib.exceptions.FormatError(
+                "Material rules should be a list!"
+            )
 
+        for rule in self.expected_materials:
+            in_toto.rulelib.unpack_rule(rule)
 
-  def _validate_pubkeys(self):
-    """Private method to check that the pubkeys is a list of keyids."""
-    if not isinstance(self.pubkeys, list):
-      raise securesystemslib.exceptions.FormatError(
-          "The pubkeys field should be a list!")
+    def _validate_expected_products(self):
+        """Private method to check that product rules are correctly formed."""
+        if not isinstance(self.expected_products, list):
+            raise securesystemslib.exceptions.FormatError(
+                "Product rules should be a list!"
+            )
 
-    for keyid in self.pubkeys:
-      securesystemslib.formats.KEYID_SCHEMA.check_match(keyid)
+        for rule in self.expected_products:
+            in_toto.rulelib.unpack_rule(rule)
 
 
-  def _validate_expected_command(self):
-    """Private method to check that the expected_command is proper."""
-    if not isinstance(self.expected_command, list):
-      raise securesystemslib.exceptions.FormatError(
-          "The expected command field is malformed!")
+@attr.s(repr=False, init=False)
+class Step(SupplyChainItem):
+    """A step of a software supply chain.
 
+    A Step object is usually contained in a Layout object and encodes the
+    expectations for a step of the software supply chain such as, who is
+    authorized to perform the step, what command is executed, and which artifacts
+    are used and produced. Evidence about a performed step is provided by link
+    metadata.
+
+    Attributes:
+      pubkeys: A list of functionary keyids authorized to perform the step.
+
+      threshold: A minimum number of distinct functionaries required to provide
+          evidence for a step.
+
+      expected_command: A list of command and command arguments, expected to
+          perform the step.
+
+    """
+
+    _type = attr.ib()
+    pubkeys = attr.ib()
+    expected_command = attr.ib()
+    threshold = attr.ib()
+
+    def __init__(self, **kwargs):
+        super(Step, self).__init__(**kwargs)
+        self._type = "step"
+        self.pubkeys = kwargs.get("pubkeys", [])
+        self.expected_command = kwargs.get("expected_command", [])
+        self.threshold = kwargs.get("threshold", 1)
+
+        self.validate()
+
+    @staticmethod
+    def read(data):
+        """Creates a Step object from its dictionary representation.
+
+        Arguments:
+          data: A dictionary with step metadata fields.
+
+        Raises:
+          securesystemslib.exceptions.FormatError: Passed data is invalid.
+
+        Returns:
+          The created Step object.
+
+        """
+        return Step(**data)
+
+    def set_expected_command_from_string(self, command_string):
+        """Parse command string as list and assign to expected_command.
+
+        Arguments:
+          command_string: A command and command arguments string.
+
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is malformed.
+
+        """
+        securesystemslib.schema.AnyString().check_match(command_string)
+        self.expected_command = shlex.split(command_string)
+
+    def _validate_type(self):
+        """Private method to ensure that the type field is set to step."""
+        if self._type != "step":
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid _type value for step (Should be 'step')"
+            )
+
+    def _validate_threshold(self):
+        """Private method to check that the threshold field is set to an int."""
+        if not isinstance(self.threshold, int):
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid threshold '{}', value must be an int.".format(
+                    self.threshold
+                )
+            )
+
+    def _validate_pubkeys(self):
+        """Private method to check that the pubkeys is a list of keyids."""
+        if not isinstance(self.pubkeys, list):
+            raise securesystemslib.exceptions.FormatError(
+                "The pubkeys field should be a list!"
+            )
+
+        for keyid in self.pubkeys:
+            securesystemslib.formats.KEYID_SCHEMA.check_match(keyid)
+
+    def _validate_expected_command(self):
+        """Private method to check that the expected_command is proper."""
+        if not isinstance(self.expected_command, list):
+            raise securesystemslib.exceptions.FormatError(
+                "The expected command field is malformed!"
+            )
 
 
 @attr.s(repr=False, init=False)
 class Inspection(SupplyChainItem):
-  """An inspection for a software supply chain.
+    """An inspection for a software supply chain.
 
-  An Inspection object is usually contained in a Layout object and encodes a
-  command to be executed by an in-toto client during final product
-  verification. Akin to steps, inspections can define artifact rules.
+    An Inspection object is usually contained in a Layout object and encodes a
+    command to be executed by an in-toto client during final product
+    verification. Akin to steps, inspections can define artifact rules.
 
-  Attributes:
-    run: A list of command and command arguments to be executed upon final
-        product verification.
-
-  """
-  _type = attr.ib()
-  run = attr.ib()
+    Attributes:
+      run: A list of command and command arguments to be executed upon final
+          product verification.
 
+    """
 
-  def __init__(self, **kwargs):
-    super(Inspection, self).__init__(**kwargs)
-    self._type = "inspection"
-    self.run = kwargs.get("run", [])
+    _type = attr.ib()
+    run = attr.ib()
 
-    self.validate()
+    def __init__(self, **kwargs):
+        super(Inspection, self).__init__(**kwargs)
+        self._type = "inspection"
+        self.run = kwargs.get("run", [])
 
+        self.validate()
 
-  @staticmethod
-  def read(data):
-    """Creates an Inspection object from its dictionary representation.
+    @staticmethod
+    def read(data):
+        """Creates an Inspection object from its dictionary representation.
 
-    Arguments:
-      data: A dictionary with inspection metadata fields.
+        Arguments:
+          data: A dictionary with inspection metadata fields.
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Passed data is invalid.
+        Raises:
+          securesystemslib.exceptions.FormatError: Passed data is invalid.
 
-    Returns:
-      The created Inspection object.
+        Returns:
+          The created Inspection object.
 
-    """
-    return Inspection(**data)
+        """
+        return Inspection(**data)
 
+    def set_run_from_string(self, command_string):
+        """Parse command string as list and assign to run attribute.
 
-  def set_run_from_string(self, command_string):
-    """Parse command string as list and assign to run attribute.
+        Arguments:
+          command_string: A command and command arguments string.
 
-    Arguments:
-      command_string: A command and command arguments string.
+        Raises:
+          securesystemslib.exceptions.FormatError: Argument is malformed.
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Argument is malformed.
-
-    """
-    securesystemslib.schema.AnyString().check_match(command_string)
-    self.run = shlex.split(command_string)
+        """
+        securesystemslib.schema.AnyString().check_match(command_string)
+        self.run = shlex.split(command_string)
 
+    def _validate_type(self):
+        """Private method to ensure that the type field is set to inspection."""
+        if self._type != "inspection":
+            raise securesystemslib.exceptions.FormatError(
+                "The _type field must be set to 'inspection'!"
+            )
 
-  def _validate_type(self):
-    """Private method to ensure that the type field is set to inspection."""
-    if self._type != "inspection":
-      raise securesystemslib.exceptions.FormatError(
-          "The _type field must be set to 'inspection'!")
-
-
-  def _validate_run(self):
-    """Private method to check that the expected command is correct."""
-    if not isinstance(self.run, list):
-      raise securesystemslib.exceptions.FormatError(
-          "The run field is malformed!")
+    def _validate_run(self):
+        """Private method to check that the expected command is correct."""
+        if not isinstance(self.run, list):
+            raise securesystemslib.exceptions.FormatError(
+                "The run field is malformed!"
+            )
```

### Comparing `in_toto-1.4.0/in_toto/models/link.py` & `in_toto-2.0.0/in_toto/models/link.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,164 +20,170 @@
 <Purpose>
   Provides a class for link metadata which is information gathered when a
   step of the supply chain is performed.
 """
 
 import attr
 import securesystemslib.formats
-from in_toto.models.common import Signable
 
+from in_toto.models.common import Signable
 
 FILENAME_FORMAT = "{step_name}.{keyid:.8}.link"
 FILENAME_FORMAT_SHORT = "{step_name}.link"
 UNFINISHED_FILENAME_FORMAT = ".{step_name}.{keyid:.8}.link-unfinished"
 UNFINISHED_FILENAME_FORMAT_GLOB = ".{step_name}.{pattern}.link-unfinished"
 
 
 @attr.s(repr=False, init=False)
 class Link(Signable):
-  """Evidence for a performed step or inspection of the supply chain.
+    """Evidence for a performed step or inspection of the supply chain.
 
-  A Link object is usually contained in a generic Metablock object for signing,
-  serialization and I/O capabilities.
+    A Link object is usually contained in a generic Metablock object for signing,
+    serialization and I/O capabilities.
 
-  Attributes:
-    name: A unique name used to identify the related step or inspection in an
-        in-toto layout.
+    Attributes:
+      name: A unique name used to identify the related step or inspection in an
+          in-toto layout.
 
-    command: A list of command and command arguments that report how the
-        corresponding step is performed.
+      command: A list of command and command arguments that report how the
+          corresponding step is performed.
 
-    materials: A dictionary of the artifacts *used* by the step, i.e::
+      materials: A dictionary of the artifacts *used* by the step, i.e::
 
-            {
-              "<material path>": {
-                "<hash algorithm name>": "<hash digest of material>",
-                ...
-              },
-              ...
-            }
-
-    products: A dictionary of the artifacts *produced* by the step, i.e::
-
-            {
-              "<product path>": {
-                "<hash algorithm name>": "<hash digest of product>",
+              {
+                "<material path>": {
+                  "<hash algorithm name>": "<hash digest of material>",
+                  ...
+                },
                 ...
-              },
-              ...
-            }
-
-    byproducts: An opaque dictionary that lists byproducts of the link command
-        execution. It should have at least the following entries
-        "stdout" (str), "stderr" (str) and "return-value" (int).
-
-    environment: An opaque dictionary that lists information about the
-        execution environment of the link command. eg.::
-
-            {
-              "variables": "<list of env var KEY=value pairs>",
-              "filesystem": "<filesystem info>",
-              "workdir": "<CWD when executing link command>"
-            }
-
-  """
-  _type = attr.ib()
-  name = attr.ib()
-  materials = attr.ib()
-  products = attr.ib()
-  byproducts = attr.ib()
-  command = attr.ib()
-  environment = attr.ib()
-
-
-  def __init__(self, **kwargs):
-    super(Link, self).__init__()
-
-    self._type = "link"
-    self.name = kwargs.get("name")
-    self.materials = kwargs.get("materials", {})
-    self.products = kwargs.get("products", {})
-    self.byproducts = kwargs.get("byproducts", {})
-    self.command = kwargs.get("command", [])
-    self.environment = kwargs.get("environment", {})
-
-    self.validate()
-
-  @property
-  def type_(self):
-    """The string "link" to indentify the in-toto metadata type."""
-    # NOTE: We expose the type_ property in the API documentation instead of
-    # _type to protect it against modification.
-    # NOTE: Trailing underscore is used by convention (pep8) to avoid conflict
-    # with Python's type keyword.
-    return self._type
-
-  @staticmethod
-  def read(data):
-    """Creates a Link object from its dictionary representation.
+              }
 
-    Arguments:
-      data: A dictionary with link metadata fields.
+      products: A dictionary of the artifacts *produced* by the step, i.e::
 
-    Raises:
-      securesystemslib.exceptions.FormatError: Passed data is invalid.
+              {
+                "<product path>": {
+                  "<hash algorithm name>": "<hash digest of product>",
+                  ...
+                },
+                ...
+              }
 
-    Returns:
-      The created Link object.
+      byproducts: An opaque dictionary that lists byproducts of the link command
+          execution. It should have at least the following entries
+          "stdout" (str), "stderr" (str) and "return-value" (int).
+
+      environment: An opaque dictionary that lists information about the
+          execution environment of the link command. eg.::
+
+              {
+                "variables": "<list of env var KEY=value pairs>",
+                "filesystem": "<filesystem info>",
+                "workdir": "<CWD when executing link command>"
+              }
 
     """
-    return Link(**data)
-
-
-  def _validate_type(self):
-    """Private method to check that `_type` is set to "link"."""
-    if self._type != "link":
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid Link: field `_type` must be set to 'link', got: {}"
-          .format(self._type))
-
-
-  def _validate_materials(self):
-    """Private method to check that `materials` is a `dict` of `HASHDICTs`."""
-    if not isinstance(self.materials, dict):
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid Link: field `materials` must be of type dict, got: {}"
-          .format(type(self.materials)))
-
-    for material in list(self.materials.values()):
-      securesystemslib.formats.HASHDICT_SCHEMA.check_match(material)
-
-
-  def _validate_products(self):
-    """Private method to check that `products` is a `dict` of `HASHDICTs`."""
-    if not isinstance(self.products, dict):
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid Link: field `products` must be of type dict, got: {}"
-          .format(type(self.products)))
-
-    for product in list(self.products.values()):
-      securesystemslib.formats.HASHDICT_SCHEMA.check_match(product)
-
-
-  def _validate_byproducts(self):
-    """Private method to check that `byproducts` is a `dict`."""
-    if not isinstance(self.byproducts, dict):
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid Link: field `byproducts` must be of type dict, got: {}"
-          .format(type(self.byproducts)))
-
-
-  def _validate_command(self):
-    """Private method to check that `command` is a `list`."""
-    if not isinstance(self.command, list):
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid Link: field `command` must be of type list, got: {}"
-          .format(type(self.command)))
-
 
-  def _validate_environment(self):
-    """Private method to check that `environment` is a `dict`. """
-    if not isinstance(self.environment, dict):
-      raise securesystemslib.exceptions.FormatError(
-          "Invalid Link: field `environment` must be of type dict, got: {}"
-          .format(type(self.environment)))
+    _type = attr.ib()
+    name = attr.ib()
+    materials = attr.ib()
+    products = attr.ib()
+    byproducts = attr.ib()
+    command = attr.ib()
+    environment = attr.ib()
+
+    def __init__(self, **kwargs):
+        super(Link, self).__init__()
+
+        self._type = "link"
+        self.name = kwargs.get("name")
+        self.materials = kwargs.get("materials", {})
+        self.products = kwargs.get("products", {})
+        self.byproducts = kwargs.get("byproducts", {})
+        self.command = kwargs.get("command", [])
+        self.environment = kwargs.get("environment", {})
+
+        self.validate()
+
+    @property
+    def type_(self):
+        """The string "link" to indentify the in-toto metadata type."""
+        # NOTE: We expose the type_ property in the API documentation instead of
+        # _type to protect it against modification.
+        # NOTE: Trailing underscore is used by convention (pep8) to avoid conflict
+        # with Python's type keyword.
+        return self._type
+
+    @staticmethod
+    def read(data):
+        """Creates a Link object from its dictionary representation.
+
+        Arguments:
+          data: A dictionary with link metadata fields.
+
+        Raises:
+          securesystemslib.exceptions.FormatError: Passed data is invalid.
+
+        Returns:
+          The created Link object.
+
+        """
+        return Link(**data)
+
+    def _validate_type(self):
+        """Private method to check that `_type` is set to "link"."""
+        if self._type != "link":
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid Link: field `_type` must be set to 'link', got: {}".format(
+                    self._type
+                )
+            )
+
+    def _validate_materials(self):
+        """Private method to check that `materials` is a `dict` of `HASHDICTs`."""
+        if not isinstance(self.materials, dict):
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid Link: field `materials` must be of type dict, got: {}".format(
+                    type(self.materials)
+                )
+            )
+
+        for material in list(self.materials.values()):
+            securesystemslib.formats.HASHDICT_SCHEMA.check_match(material)
+
+    def _validate_products(self):
+        """Private method to check that `products` is a `dict` of `HASHDICTs`."""
+        if not isinstance(self.products, dict):
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid Link: field `products` must be of type dict, got: {}".format(
+                    type(self.products)
+                )
+            )
+
+        for product in list(self.products.values()):
+            securesystemslib.formats.HASHDICT_SCHEMA.check_match(product)
+
+    def _validate_byproducts(self):
+        """Private method to check that `byproducts` is a `dict`."""
+        if not isinstance(self.byproducts, dict):
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid Link: field `byproducts` must be of type dict, got: {}".format(
+                    type(self.byproducts)
+                )
+            )
+
+    def _validate_command(self):
+        """Private method to check that `command` is a `list`."""
+        if not isinstance(self.command, list):
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid Link: field `command` must be of type list, got: {}".format(
+                    type(self.command)
+                )
+            )
+
+    def _validate_environment(self):
+        """Private method to check that `environment` is a `dict`."""
+        if not isinstance(self.environment, dict):
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid Link: field `environment` must be of type dict, got: {}".format(
+                    type(self.environment)
+                )
+            )
```

### Comparing `in_toto-1.4.0/in_toto/models/metadata.py` & `in_toto-2.0.0/in_toto/models/metadata.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,289 +18,279 @@
 <Purpose>
   Provides a container class `Metablock` for signed metadata and
   functions for signing, signature verification, de-serialization and
   serialization from and to JSON.
 
 """
 
-import attr
 import json
 from typing import Union
 
-import securesystemslib.keys
-import securesystemslib.formats
+import attr
 import securesystemslib.exceptions
+import securesystemslib.formats
 import securesystemslib.gpg.functions
+import securesystemslib.keys
+from securesystemslib.dsse import Envelope as SSlibEnvelope
 from securesystemslib.exceptions import VerificationError
 from securesystemslib.signer import Signature, Signer, SSlibKey
-from securesystemslib.dsse import Envelope as SSlibEnvelope
 
 from in_toto.exceptions import InvalidMetadata, SignatureVerificationError
 from in_toto.models._signer import GPGSigner
 from in_toto.models.common import Signable, ValidationMixin
-from in_toto.models.link import Link
 from in_toto.models.layout import Layout
-
+from in_toto.models.link import Link
 
 ENVELOPE_PAYLOAD_TYPE = "application/vnd.in-toto+json"
 
 
 class Metadata:
-  """A Metadata abstraction between DSSE Envelope and Metablock."""
+    """A Metadata abstraction between DSSE Envelope and Metablock."""
 
-  @classmethod
-  def from_dict(cls, data):
-    """Loads DSSE or Traditional Metadata from its JSON/dict representation."""
+    @classmethod
+    def from_dict(cls, data):
+        """Loads DSSE or Traditional Metadata from its JSON/dict representation."""
 
-    if "payload" in data:
-      if data.get("payloadType") == ENVELOPE_PAYLOAD_TYPE:
-        return Envelope.from_dict(data)
+        if "payload" in data:
+            if data.get("payloadType") == ENVELOPE_PAYLOAD_TYPE:
+                return Envelope.from_dict(data)
 
-    elif "signed" in data:
-      return Metablock.from_dict(data)
+        elif "signed" in data:
+            return Metablock.from_dict(data)
 
-    raise InvalidMetadata
+        raise InvalidMetadata
 
-  def to_dict(self):
-    """Returns the JSON-serializable dictionary representation of self."""
-    raise NotImplementedError  # pragma: no cover
+    def to_dict(self):
+        """Returns the JSON-serializable dictionary representation of self."""
+        raise NotImplementedError  # pragma: no cover
 
-  @classmethod
-  def load(cls, path):
-    """Loads the JSON string representation of metadata from disk.
+    @classmethod
+    def load(cls, path):
+        """Loads the JSON string representation of metadata from disk.
 
-    Arguments:
-      path: The path to read the file from.
+        Arguments:
+          path: The path to read the file from.
 
-    Raises:
-      IOError: The file cannot be read.
-      InvalidMetadata: Metadata format is invalid.
-      securesystemslib.exceptions.FormatError: Metadata format is invalid.
+        Raises:
+          IOError: The file cannot be read.
+          InvalidMetadata: Metadata format is invalid.
+          securesystemslib.exceptions.FormatError: Metadata format is invalid.
 
-    Returns:
-      A Metadata containing a Link or Layout object.
+        Returns:
+          A Metadata containing a Link or Layout object.
 
-    """
-    with open(path, "r", encoding="utf8") as fp:
-      data = json.load(fp)
+        """
+        with open(path, "r", encoding="utf8") as fp:
+            data = json.load(fp)
 
-    return cls.from_dict(data)
+        return cls.from_dict(data)
 
-  def dump(self, path):
-    """Writes the JSON string representation of the instance to disk.
+    def dump(self, path):
+        """Writes the JSON string representation of the instance to disk.
 
-    Arguments:
-      path: The path to write the file to.
+        Arguments:
+          path: The path to write the file to.
 
-    Raises:
-      IOError: File cannot be written.
+        Raises:
+          IOError: File cannot be written.
 
-    """
-    json_bytes = json.dumps(
-      self.to_dict(),
-      sort_keys=True,
-    ).encode("utf-8")
+        """
+        json_bytes = json.dumps(
+            self.to_dict(),
+            sort_keys=True,
+        ).encode("utf-8")
 
-    with open(path, "wb") as fp:
-      fp.write(json_bytes)
+        with open(path, "wb") as fp:
+            fp.write(json_bytes)
 
-  def create_signature(self, signer: Signer) -> Signature:
-    """Creates signature over signable with Signer and adds it to signatures.
+    def create_signature(self, signer: Signer) -> Signature:
+        """Creates signature over signable with Signer and adds it to signatures.
 
     Arguments:
       signer: A "Signer" class instance to create signature.
 
     Raises:
       securesystemslib.exceptions.CryptoError, \
               securesystemslib.exceptions.UnsupportedAlgorithmError:
           Signing errors.
 
     Returns:
       The signature. A securesystemslib.signer.Signature type.
     """
-    raise NotImplementedError  # pragma: no cover
+        raise NotImplementedError  # pragma: no cover
 
-  def verify_signature(self, verification_key):
-    """Verifies a signature over signable in signatures with verification_key.
+    def verify_signature(self, verification_key):
+        """Verifies a signature over signable in signatures with verification_key.
 
-    Arguments:
-      verification_key: A verification key. The format is
-          securesystemslib.formats.ANY_VERIFICATION_KEY_SCHEMA.
-
-    Raises:
-      securesystemslib.exceptions.FormatError: The passed key is malformed.
-
-      SignatureVerificationError: No signature keyid matches
-          the verification key keyid, or the matching signature is malformed,
-          or the matching signature is invalid.
-    """
-    raise NotImplementedError  # pragma: no cover
-
-  def get_payload(self):
-    """Returns ``Link`` or ``Layout``."""
-    raise NotImplementedError  # pragma: no cover
+        Arguments:
+          verification_key: A verification key. The format is
+              securesystemslib.formats.ANY_VERIFICATION_KEY_SCHEMA.
+
+        Raises:
+          securesystemslib.exceptions.FormatError: The passed key is malformed.
+
+          SignatureVerificationError: No signature keyid matches
+              the verification key keyid, or the matching signature is malformed,
+              or the matching signature is invalid.
+        """
+        raise NotImplementedError  # pragma: no cover
+
+    def get_payload(self):
+        """Returns ``Link`` or ``Layout``."""
+        raise NotImplementedError  # pragma: no cover
 
 
 class Envelope(SSlibEnvelope, Metadata):
-  """DSSE Envelope for in-toto payloads."""
-
-  @classmethod
-  def from_signable(cls, signable: Signable) -> "Envelope":
-    """Creates DSSE envelope with signable bytes as payload."""
-
-    json_bytes = json.dumps(
-      attr.asdict(signable),
-      sort_keys=True,
-    ).encode("utf-8")
-
-    return cls(
-      payload=json_bytes,
-      payload_type=ENVELOPE_PAYLOAD_TYPE,
-      signatures=[]
-    )
-
-  def create_signature(self, signer: Signer) -> Signature:
-    if isinstance(signer, GPGSigner):
-      raise NotImplementedError("GPG Signing is not implemented")
-
-    return super().sign(signer)
-
-  def verify_signature(self, verification_key):
-    key = SSlibKey.from_securesystemslib_key(verification_key)
-    try:
-      super().verify(
-        keys=[key], threshold=1
-      )
-    except VerificationError as exc:
-      raise SignatureVerificationError from exc
+    """DSSE Envelope for in-toto payloads."""
 
-  def get_payload(self) -> Union[Link, Layout]:
-    """Parse DSSE payload into Link or Layout object.
+    @classmethod
+    def from_signable(cls, signable: Signable) -> "Envelope":
+        """Creates DSSE envelope with signable bytes as payload."""
+
+        json_bytes = json.dumps(
+            attr.asdict(signable),
+            sort_keys=True,
+        ).encode("utf-8")
+
+        return cls(
+            payload=json_bytes,
+            payload_type=ENVELOPE_PAYLOAD_TYPE,
+            signatures=[],
+        )
+
+    def create_signature(self, signer: Signer) -> Signature:
+        if isinstance(signer, GPGSigner):
+            raise NotImplementedError("GPG Signing is not implemented")
+
+        return super().sign(signer)
+
+    def verify_signature(self, verification_key):
+        key = SSlibKey.from_securesystemslib_key(verification_key)
+        try:
+            super().verify(keys=[key], threshold=1)
+        except VerificationError as exc:
+            raise SignatureVerificationError from exc
+
+    def get_payload(self) -> Union[Link, Layout]:
+        """Parse DSSE payload into Link or Layout object.
+
+        Raises:
+            InvalidMetadata: If type in payload is not ``link`` or ``layout``.
+
+        Returns:
+            Link or Layout.
+        """
+
+        data = json.loads(self.payload.decode("utf-8"))
+        _type = data.get("_type")
+        if _type == "link":
+            return Link.read(data)
+        if _type == "layout":
+            return Layout.read(data)
 
-      Raises:
-          InvalidMetadata: If type in payload is not ``link`` or ``layout``.
-
-      Returns:
-          Link or Layout.
-    """
-
-    data = json.loads(self.payload.decode("utf-8"))
-    _type = data.get("_type")
-    if _type == "link":
-      return Link.read(data)
-    if _type == "layout":
-      return Layout.read(data)
-
-    raise InvalidMetadata
+        raise InvalidMetadata
 
 
 @attr.s(repr=False, init=False)
 class Metablock(Metadata, ValidationMixin):
-  """A container for signed in-toto metadata.
-
-  Provides methods for metadata JSON (de-)serialization, reading from and
-  writing to disk, creating and verifying signatures, and self-validation.
+    """A container for signed in-toto metadata.
 
-  Attributes:
-    signed: A subclass of Signable which has the actual metadata payload,
-        usually a Link or Layout object.
-    signatures: A list of signatures over the canonical JSON representation
-        of the value of the signed attribute.
-    compact_json: A boolean indicating if the dump method should write a
-        compact JSON string representation of the metadata.
-
-  """
-  signatures = attr.ib()
-  signed = attr.ib()
-
-
-  def __init__(self, **kwargs):
-    self.signatures = kwargs.get("signatures", [])
-    self.signed = kwargs.get("signed")
-    self.compact_json = kwargs.get("compact_json", False)
-
-    self.validate()
-
-
-  def __repr__(self):
-    """Returns the JSON string representation. """
-    indent = None if self.compact_json else 1
-    separators = (',', ':') if self.compact_json else (',', ': ')
-
-    return json.dumps(
-        {
-          "signatures": self.signatures,
-          "signed": attr.asdict(self.signed)
-        },
-        indent=indent,
-        separators=separators,
-        sort_keys=True
-      )
+    Provides methods for metadata JSON (de-)serialization, reading from and
+    writing to disk, creating and verifying signatures, and self-validation.
 
-
-  def dump(self, path):
-    """Writes the JSON string representation of the instance to disk.
-
-    Arguments:
-      path: The path to write the file to.
-
-    Raises:
-      IOError: File cannot be written.
+    Attributes:
+      signed: A subclass of Signable which has the actual metadata payload,
+          usually a Link or Layout object.
+      signatures: A list of signatures over the canonical JSON representation
+          of the value of the signed attribute.
+      compact_json: A boolean indicating if the dump method should write a
+          compact JSON string representation of the metadata.
 
     """
-    with open(path, "wb") as fp:
-      fp.write("{}".format(self).encode("utf-8"))
-
-
-  @classmethod
-  def from_dict(cls, data):
-    """Creates a Metablock object from its JSON/dict representation."""
-
-    signatures = data.get("signatures", [])
-    signed_data = data.get("signed", {})
-    signed_type = signed_data.get("_type")
 
-    if signed_type == "link":
-      signed = Link.read(signed_data)
+    signatures = attr.ib()
+    signed = attr.ib()
 
-    elif signed_type == "layout":
-      signed = Layout.read(signed_data)
+    def __init__(self, **kwargs):
+        self.signatures = kwargs.get("signatures", [])
+        self.signed = kwargs.get("signed")
+        self.compact_json = kwargs.get("compact_json", False)
+
+        self.validate()
+
+    def __repr__(self):
+        """Returns the JSON string representation."""
+        indent = None if self.compact_json else 1
+        separators = (",", ":") if self.compact_json else (",", ": ")
+
+        return json.dumps(
+            {"signatures": self.signatures, "signed": attr.asdict(self.signed)},
+            indent=indent,
+            separators=separators,
+            sort_keys=True,
+        )
+
+    def dump(self, path):
+        """Writes the JSON string representation of the instance to disk.
+
+        Arguments:
+          path: The path to write the file to.
+
+        Raises:
+          IOError: File cannot be written.
+
+        """
+        with open(path, "wb") as fp:
+            fp.write("{}".format(self).encode("utf-8"))
+
+    @classmethod
+    def from_dict(cls, data):
+        """Creates a Metablock object from its JSON/dict representation."""
+
+        signatures = data.get("signatures", [])
+        signed_data = data.get("signed", {})
+        signed_type = signed_data.get("_type")
+
+        if signed_type == "link":
+            signed = Link.read(signed_data)
+
+        elif signed_type == "layout":
+            signed = Layout.read(signed_data)
+
+        else:
+            raise securesystemslib.exceptions.FormatError(
+                "Invalid Metadata format"
+            )
+
+        return cls(signatures=signatures, signed=signed)
+
+    def to_dict(self):
+        """Returns the JSON-serializable dictionary representation of self."""
+
+        return {
+            "signatures": self.signatures,
+            "signed": attr.asdict(self.signed),
+        }
+
+    @property
+    def type_(self):
+        """A shortcut to the `type_` attribute of the object on the signable
+        attribute (should be one of "link" or "layout")."""
+        # NOTE: Trailing underscore is used by convention (pep8) to avoid conflict
+        # with Python's type keyword.
+        return self.signed.type_
+
+    def create_signature(self, signer: Signer):
+        signature = signer.sign(self.signed.signable_bytes)
+        self.signatures.append(signature.to_dict())
 
-    else:
-      raise securesystemslib.exceptions.FormatError("Invalid Metadata format")
+        return signature
 
-    return cls(signatures=signatures, signed=signed)
-
-
-  def to_dict(self):
-    """Returns the JSON-serializable dictionary representation of self."""
-
-    return {
-      "signatures": self.signatures,
-      "signed": attr.asdict(self.signed)
-    }
-
-
-  @property
-  def type_(self):
-    """A shortcut to the `type_` attribute of the object on the signable
-    attribute (should be one of "link" or "layout"). """
-    # NOTE: Trailing underscore is used by convention (pep8) to avoid conflict
-    # with Python's type keyword.
-    return self.signed.type_
-
-
-  def create_signature(self, signer: Signer):
-    signature = signer.sign(self.signed.signable_bytes)
-    self.signatures.append(signature.to_dict())
-
-    return signature
-
-  def sign(self, key):
-    """Creates signature over signable with key and adds it to signatures.
+    def sign(self, key):
+        """Creates signature over signable with key and adds it to signatures.
 
     Uses the UTF-8 encoded canonical JSON byte representation of the signable
     attribute to create signatures deterministically.
 
     Attributes:
       key: A signing key. The format is securesystemslib.formats.KEY_SCHEMA.
 
@@ -310,25 +300,26 @@
               securesystemslib.exceptions.UnsupportedAlgorithmError:
           Signing errors.
 
     Returns:
       The signature. Format is securesystemslib.formats.SIGNATURE_SCHEMA.
 
     """
-    securesystemslib.formats.KEY_SCHEMA.check_match(key)
+        securesystemslib.formats.KEY_SCHEMA.check_match(key)
 
-    signature = securesystemslib.keys.create_signature(key,
-        self.signed.signable_bytes)
+        signature = securesystemslib.keys.create_signature(
+            key, self.signed.signable_bytes
+        )
 
-    self.signatures.append(signature)
+        self.signatures.append(signature)
 
-    return signature
+        return signature
 
-  def sign_gpg(self, gpg_keyid=None, gpg_home=None):
-    """Creates signature over signable with gpg and adds it to signatures.
+    def sign_gpg(self, gpg_keyid=None, gpg_home=None):
+        """Creates signature over signable with gpg and adds it to signatures.
 
     Uses the UTF-8 encoded canonical JSON byte representation of the signable
     attribute to create signatures deterministically.
 
     Arguments:
       gpg_keyid (optional): A keyid used to identify a local gpg signing key.
           If omitted the default signing key is used.
@@ -344,104 +335,114 @@
     Side Effects:
       Calls system gpg command in a subprocess.
 
     Returns:
       The signature. Format is securesystemslib.formats.GPG_SIGNATURE_SCHEMA.
 
     """
-    signature = securesystemslib.gpg.functions.create_signature(
-        self.signed.signable_bytes, gpg_keyid, gpg_home)
-
-    self.signatures.append(signature)
-
-    return signature
-
-
-  def verify_signature(self, verification_key):
-    """Verifies a signature over signable in signatures with verification_key.
-
-    Uses the UTF-8 encoded canonical JSON byte representation of the signable
-    attribute to verify the signature deterministically.
-
-    NOTE: Only the first signature in the signatures attribute, whose keyid
-    matches the verification_key keyid, is verified. If the verification_key
-    format is securesystemslib.formats.GPG_PUBKEY_SCHEMA, subkey keyids are
-    considered too.
-
-    Arguments:
-      verification_key: A verification key. The format is
-          securesystemslib.formats.ANY_VERIFICATION_KEY_SCHEMA.
-
-    Raises:
-      securesystemslib.exceptions.FormatError: The passed key is malformed.
-
-      SignatureVerificationError: No signature keyid matches the verification
-          key keyid, or the matching signature is malformed, or the matching
-          signature is invalid.
-
-      securesystemslib.gpg.exceptions.KeyExpirationError: Passed verification
-          key is an expired gpg key.
-
-    """
-    securesystemslib.formats.ANY_VERIFICATION_KEY_SCHEMA.check_match(
-        verification_key)
-    verification_keyid = verification_key["keyid"]
-
-    # Find a signature that corresponds to the keyid of the passed
-    # verification key or one of its subkeys
-    signature = None
-    for signature in self.signatures:
-      if signature["keyid"] == verification_keyid:
-        break
-
-      if signature["keyid"] in list(
-          verification_key.get("subkeys", {}).keys()):
-        break
-
-    else:
-      raise SignatureVerificationError("No signature found for key '{}'"
-          .format(verification_keyid))
-
-    if securesystemslib.formats.GPG_SIGNATURE_SCHEMA.matches(signature):
-      valid = securesystemslib.gpg.functions.verify_signature(signature,
-          verification_key, self.signed.signable_bytes)
-
-    elif securesystemslib.formats.SIGNATURE_SCHEMA.matches(signature):
-      valid = securesystemslib.keys.verify_signature(
-          verification_key, signature, self.signed.signable_bytes)
-
-    else:
-      valid = False
-
-    if not valid:
-      raise SignatureVerificationError("Invalid signature for keyid '{}'"
-          .format(verification_keyid))
-
-
-  def _validate_signed(self):
-    """Private method to check if the 'signed' attribute contains a valid
-    Layout or Link object. """
-
-    if not (isinstance(self.signed, Layout) or isinstance(self.signed, Link)):
-      raise securesystemslib.exceptions.FormatError("The Metblock's 'signed'"
-        " property has has to be of type 'Link' or 'Layout'.")
-
-    # If the signed object is a Link or Layout object validate it.
-    self.signed.validate()
-
-
-  def _validate_signatures(self):
-    """Private method to check that the 'signatures' attribute is a list of
-    signatures in the format 'securesystemslib.formats.ANY_SIGNATURE_SCHEMA'.
-    """
-
-    if not isinstance(self.signatures, list):
-      raise securesystemslib.exceptions.FormatError("The Metablock's"
-        " 'signatures' property has to be of type 'list'.")
+        signature = securesystemslib.gpg.functions.create_signature(
+            self.signed.signable_bytes, gpg_keyid, gpg_home
+        )
+
+        self.signatures.append(signature)
+
+        return signature
+
+    def verify_signature(self, verification_key):
+        """Verifies a signature over signable in signatures with verification_key.
+
+        Uses the UTF-8 encoded canonical JSON byte representation of the signable
+        attribute to verify the signature deterministically.
+
+        NOTE: Only the first signature in the signatures attribute, whose keyid
+        matches the verification_key keyid, is verified. If the verification_key
+        format is securesystemslib.formats.GPG_PUBKEY_SCHEMA, subkey keyids are
+        considered too.
+
+        Arguments:
+          verification_key: A verification key. The format is
+              securesystemslib.formats.ANY_VERIFICATION_KEY_SCHEMA.
+
+        Raises:
+          securesystemslib.exceptions.FormatError: The passed key is malformed.
+
+          SignatureVerificationError: No signature keyid matches the verification
+              key keyid, or the matching signature is malformed, or the matching
+              signature is invalid.
+
+          securesystemslib.gpg.exceptions.KeyExpirationError: Passed verification
+              key is an expired gpg key.
+
+        """
+        securesystemslib.formats.ANY_VERIFICATION_KEY_SCHEMA.check_match(
+            verification_key
+        )
+        verification_keyid = verification_key["keyid"]
+
+        # Find a signature that corresponds to the keyid of the passed
+        # verification key or one of its subkeys
+        signature = None
+        for signature in self.signatures:
+            if signature["keyid"] == verification_keyid:
+                break
+
+            if signature["keyid"] in list(
+                verification_key.get("subkeys", {}).keys()
+            ):
+                break
+
+        else:
+            raise SignatureVerificationError(
+                "No signature found for key '{}'".format(verification_keyid)
+            )
+
+        if securesystemslib.formats.GPG_SIGNATURE_SCHEMA.matches(signature):
+            valid = securesystemslib.gpg.functions.verify_signature(
+                signature, verification_key, self.signed.signable_bytes
+            )
+
+        elif securesystemslib.formats.SIGNATURE_SCHEMA.matches(signature):
+            valid = securesystemslib.keys.verify_signature(
+                verification_key, signature, self.signed.signable_bytes
+            )
+
+        else:
+            valid = False
+
+        if not valid:
+            raise SignatureVerificationError(
+                "Invalid signature for keyid '{}'".format(verification_keyid)
+            )
+
+    def _validate_signed(self):
+        """Private method to check if the 'signed' attribute contains a valid
+        Layout or Link object."""
+
+        if not (
+            isinstance(self.signed, Layout) or isinstance(self.signed, Link)
+        ):
+            raise securesystemslib.exceptions.FormatError(
+                "The Metblock's 'signed'"
+                " property has has to be of type 'Link' or 'Layout'."
+            )
+
+        # If the signed object is a Link or Layout object validate it.
+        self.signed.validate()
+
+    def _validate_signatures(self):
+        """Private method to check that the 'signatures' attribute is a list of
+        signatures in the format 'securesystemslib.formats.ANY_SIGNATURE_SCHEMA'.
+        """
+
+        if not isinstance(self.signatures, list):
+            raise securesystemslib.exceptions.FormatError(
+                "The Metablock's"
+                " 'signatures' property has to be of type 'list'."
+            )
 
-    for signature in self.signatures:
-      securesystemslib.formats.ANY_SIGNATURE_SCHEMA.check_match(signature)
+        for signature in self.signatures:
+            securesystemslib.formats.ANY_SIGNATURE_SCHEMA.check_match(signature)
 
-  def get_payload(self):
-    """Returns signed of the Metablock."""
+    def get_payload(self):
+        """Returns signed of the Metablock."""
 
-    return self.signed
+        return self.signed
```

### Comparing `in_toto-1.4.0/tests/__init__.py` & `in_toto-2.0.0/tests/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # Copyright New York University and the in-toto contributors
 # SPDX-License-Identifier: Apache-2.0
 
-import sys
 import logging
+import sys
+
 import in_toto
 
+
 class CapturableStreamHandler(logging.StreamHandler):
-  """Override logging.StreamHandler's stream property to always write log
-  output to `sys.stderr` available at the time of logging.
-  """
-  @property
-  def stream(self):
-    """Always use currently available sys.stderr. """
-    return sys.stderr
-
-  @stream.setter
-  def stream(self, value):
-    """Disable setting stream. """
+    """Override logging.StreamHandler's stream property to always write log
+    output to `sys.stderr` available at the time of logging.
+    """
+
+    @property
+    def stream(self):
+        """Always use currently available sys.stderr."""
+        return sys.stderr
+
+    @stream.setter
+    def stream(self, value):
+        """Disable setting stream."""
+
 
 # Python `unittest` is configured to buffer output to `sys.stdout/sys.stderr`
 # (see `TextTestRunner` in `tests/runtests.py`) and only show it in case a test
 # fails. Python `unittest` buffers output by overriding `sys.stdout/sys.stderr`
 # before running tests, hence we need to log to that overridden `sys.stderr`,
 # which we do by using a custom StreamHandler.
 handler = CapturableStreamHandler()
```

### Comparing `in_toto-1.4.0/tests/common.py` & `in_toto-2.0.0/tests/common.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,148 +22,167 @@
 
   Tests importing this module, should be run from the project root, e.g.:
   `python tests/test_in_toto_run.py`
   or using the aggregator script (preferred way):
   `python tests/runtests.py`.
 
 """
-import os
-import sys
 import inspect
+import os
 import shutil
+import sys
 import tempfile
+import unittest
+from unittest.mock import patch
+
 from securesystemslib.interface import (
-    generate_and_write_rsa_keypair,
-    generate_and_write_unencrypted_rsa_keypair,
+    generate_and_write_ecdsa_keypair,
     generate_and_write_ed25519_keypair,
+    generate_and_write_rsa_keypair,
+    generate_and_write_unencrypted_ecdsa_keypair,
     generate_and_write_unencrypted_ed25519_keypair,
-    generate_and_write_ecdsa_keypair,
-    generate_and_write_unencrypted_ecdsa_keypair)
-
-import unittest
-from unittest.mock import patch
+    generate_and_write_unencrypted_rsa_keypair,
+)
 
 
 def run_with_portable_scripts(decorated):
+    print("patching...")
+    scripts_path = os.path.join(
+        os.path.dirname(os.path.realpath(__file__)), "scripts"
+    )
+    print("scripts are located in {}".format(scripts_path))
+
+    @patch.dict(
+        os.environ, {"PATH": "{};{}".format(scripts_path, os.environ["PATH"])}
+    )
+    class Patched(decorated):
+        pass
+
+    return Patched
+
+
+class TmpDirMixin:
+    """Mixin with classmethods to create and change into a temporary directory,
+    and to change back to the original CWD and remove the temporary directory.
 
-  print("patching...")
-  scripts_path = os.path.join(os.path.dirname(os.path.realpath(__file__)), "scripts")
-  print("scripts are located in {}".format(scripts_path))
-  @patch.dict(os.environ, {"PATH": "{};{}".format(scripts_path, os.environ['PATH'])})
-  class Patched(decorated):
-    pass
-
-  return Patched
-
-
-class TmpDirMixin():
-  """Mixin with classmethods to create and change into a temporary directory,
-  and to change back to the original CWD and remove the temporary directory.
-
-  """
-  @classmethod
-  def set_up_test_dir(cls):
-    """Back up CWD, and create and change into temporary directory. """
-    cls.original_cwd = os.getcwd()
-    cls.test_dir = os.path.realpath(tempfile.mkdtemp())
-    os.chdir(cls.test_dir)
-
-  @classmethod
-  def tear_down_test_dir(cls):
-    """Change back to original CWD and remove temporary directory. """
-    os.chdir(cls.original_cwd)
-    shutil.rmtree(cls.test_dir)
-
-
-class GPGKeysMixin():
-  """Mixin with classmethod to copy GPG rsa test keyring to a subdir 'rsa' in
-  the CWD.
-
-  """
-  gnupg_home = "rsa"
-  gpg_key_768C43 = "7b3abb26b97b655ab9296bd15b0bd02e1c768c43"
-  gpg_key_85DA58 = "8288ef560ed3795f9df2c0db56193089b285da58"
-  gpg_key_0C8A17 = "8465a1e2e0fb2b40adb2478e18fb3f537e0c8a17"
-  gpg_key_D924E9 = "c5a0abe6ec19d0d65f85e2c39be9df5131d924e9"
-
-  @classmethod
-  def set_up_gpg_keys(cls):
-    gpg_keys = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "gpg_keyrings", "rsa")
-
-    shutil.copytree(gpg_keys, os.path.join(os.getcwd(), cls.gnupg_home))
-
-
-class GenKeysMixin():
-  """Mixin with classmethod to create cryptographic keys in cwd. """
-  key_pw = "pw"
-
-  @classmethod
-  def set_up_keys(cls):
-    # Generated unencrypted keys
-    cls.rsa_key_path = generate_and_write_unencrypted_rsa_keypair()
-    cls.rsa_key_id = os.path.basename(cls.rsa_key_path)
-
-    cls.ed25519_key_path = generate_and_write_unencrypted_ed25519_keypair()
-    cls.ed25519_key_id = os.path.basename(cls.ed25519_key_path)
-
-    cls.ecdsa_key_path = generate_and_write_unencrypted_ecdsa_keypair()
-    cls.ecdsa_key_id = os.path.basename(cls.ecdsa_key_path)
-
-    # Generate encrypted keys
-    cls.rsa_key_enc_path = generate_and_write_rsa_keypair(password=cls.key_pw)
-    cls.rsa_key_enc_id = os.path.basename(cls.rsa_key_enc_path)
-
-    cls.ed25519_key_enc_path = generate_and_write_ed25519_keypair(password=cls.key_pw)
-    cls.ed25519_key_enc_id = os.path.basename(cls.ed25519_key_enc_path)
-
-    cls.ecdsa_key_enc_path = generate_and_write_ecdsa_keypair(password=cls.key_pw)
-    cls.ecdsa_key_enc_id = os.path.basename(cls.ecdsa_key_enc_path)
+    """
 
+    @classmethod
+    def set_up_test_dir(cls):
+        """Back up CWD, and create and change into temporary directory."""
+        cls.original_cwd = os.getcwd()
+        cls.test_dir = os.path.realpath(tempfile.mkdtemp())
+        os.chdir(cls.test_dir)
+
+    @classmethod
+    def tear_down_test_dir(cls):
+        """Change back to original CWD and remove temporary directory."""
+        os.chdir(cls.original_cwd)
+        shutil.rmtree(cls.test_dir)
+
+
+class GPGKeysMixin:
+    """Mixin with classmethod to copy GPG rsa test keyring to a subdir 'rsa' in
+    the CWD.
 
-class CliTestCase(unittest.TestCase):
-  """TestCase subclass providing a test helper that patches sys.argv with
-  passed arguments and asserts a SystemExit with a return code equal
-  to the passed status argument.
-
-  Subclasses of CliTestCase require a class variable that stores the main
-  function of the cli tool to test as staticmethod, e.g.:
-
-  ```
-  import tests.common
-  from in_toto.in_toto_run import main as in_toto_run_main
-
-  class TestInTotoRunTool(tests.common.CliTestCase):
-    cli_main_func = staticmethod(in_toto_run_main)
-    ...
-
-  ```
-  """
-  cli_main_func = None
-
-  def __init__(self, *args, **kwargs):
-    """Constructor that checks for the presence of a callable cli_main_func
-    class variable. And stores the filename of the module containing that
-    function, to be used as first argument when patching sys.argv in
-    self.assert_cli_sys_exit.
     """
-    if not callable(self.cli_main_func):
-      raise Exception("Subclasses of `CliTestCase` need to assign the main"
-          " function of the cli tool to test using `staticmethod()`: {}"
-          .format(self.__class__.__name__))
 
-    file_path = inspect.getmodule(self.cli_main_func).__file__
-    self.file_name = os.path.basename(file_path)
+    gnupg_home = "rsa"
+    gpg_key_768C43 = "7b3abb26b97b655ab9296bd15b0bd02e1c768c43"
+    gpg_key_85DA58 = "8288ef560ed3795f9df2c0db56193089b285da58"
+    gpg_key_0C8A17 = "8465a1e2e0fb2b40adb2478e18fb3f537e0c8a17"
+    gpg_key_D924E9 = "c5a0abe6ec19d0d65f85e2c39be9df5131d924e9"
+
+    @classmethod
+    def set_up_gpg_keys(cls):
+        gpg_keys = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "gpg_keyrings", "rsa"
+        )
+
+        shutil.copytree(gpg_keys, os.path.join(os.getcwd(), cls.gnupg_home))
+
+
+class GenKeysMixin:
+    """Mixin with classmethod to create cryptographic keys in cwd."""
+
+    key_pw = "pw"
+
+    @classmethod
+    def set_up_keys(cls):
+        # Generated unencrypted keys
+        cls.rsa_key_path = generate_and_write_unencrypted_rsa_keypair()
+        cls.rsa_key_id = os.path.basename(cls.rsa_key_path)
+
+        cls.ed25519_key_path = generate_and_write_unencrypted_ed25519_keypair()
+        cls.ed25519_key_id = os.path.basename(cls.ed25519_key_path)
+
+        cls.ecdsa_key_path = generate_and_write_unencrypted_ecdsa_keypair()
+        cls.ecdsa_key_id = os.path.basename(cls.ecdsa_key_path)
+
+        # Generate encrypted keys
+        cls.rsa_key_enc_path = generate_and_write_rsa_keypair(
+            password=cls.key_pw
+        )
+        cls.rsa_key_enc_id = os.path.basename(cls.rsa_key_enc_path)
+
+        cls.ed25519_key_enc_path = generate_and_write_ed25519_keypair(
+            password=cls.key_pw
+        )
+        cls.ed25519_key_enc_id = os.path.basename(cls.ed25519_key_enc_path)
+
+        cls.ecdsa_key_enc_path = generate_and_write_ecdsa_keypair(
+            password=cls.key_pw
+        )
+        cls.ecdsa_key_enc_id = os.path.basename(cls.ecdsa_key_enc_path)
 
-    super(CliTestCase, self).__init__(*args, **kwargs)
 
+class CliTestCase(unittest.TestCase):
+    """TestCase subclass providing a test helper that patches sys.argv with
+    passed arguments and asserts a SystemExit with a return code equal
+    to the passed status argument.
+
+    Subclasses of CliTestCase require a class variable that stores the main
+    function of the cli tool to test as staticmethod, e.g.:
+
+    ```
+    import tests.common
+    from in_toto.in_toto_run import main as in_toto_run_main
+
+    class TestInTotoRunTool(tests.common.CliTestCase):
+      cli_main_func = staticmethod(in_toto_run_main)
+      ...
 
-  def assert_cli_sys_exit(self, cli_args, status):
-    """Test helper to mock command line call and assert return value.
-    The passed args does not need to contain the command line tool's name.
-    This is assessed from  `self.cli_main_func`
+    ```
     """
-    with patch.object(sys, "argv", [self.file_name]
-        + cli_args), self.assertRaises(SystemExit) as raise_ctx:
-      self.cli_main_func() # pylint: disable=not-callable
 
-    self.assertEqual(raise_ctx.exception.code, status)
+    cli_main_func = None
+
+    def __init__(self, *args, **kwargs):
+        """Constructor that checks for the presence of a callable cli_main_func
+        class variable. And stores the filename of the module containing that
+        function, to be used as first argument when patching sys.argv in
+        self.assert_cli_sys_exit.
+        """
+        if not callable(self.cli_main_func):
+            raise Exception(
+                "Subclasses of `CliTestCase` need to assign the main"
+                " function of the cli tool to test using `staticmethod()`: {}".format(
+                    self.__class__.__name__
+                )
+            )
+
+        file_path = inspect.getmodule(self.cli_main_func).__file__
+        self.file_name = os.path.basename(file_path)
+
+        super(CliTestCase, self).__init__(*args, **kwargs)
+
+    def assert_cli_sys_exit(self, cli_args, status):
+        """Test helper to mock command line call and assert return value.
+        The passed args does not need to contain the command line tool's name.
+        This is assessed from  `self.cli_main_func`
+        """
+        with patch.object(
+            sys, "argv", [self.file_name] + cli_args
+        ), self.assertRaises(SystemExit) as raise_ctx:
+            self.cli_main_func()  # pylint: disable=not-callable
+
+        self.assertEqual(raise_ctx.exception.code, status)
```

### Comparing `in_toto-1.4.0/tests/runtests.py` & `in_toto-2.0.0/tests/runtests.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,13 +18,13 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Script to search, load and run in-toto tests using the Python `unittest`
   framework.
 """
 
-from unittest import defaultTestLoader, TextTestRunner
 import sys
+from unittest import TextTestRunner, defaultTestLoader
 
 suite = defaultTestLoader.discover(start_dir=".")
 result = TextTestRunner(verbosity=2, buffer=True).run(suite)
 sys.exit(0 if result.wasSuccessful() else 1)
```

### Comparing `in_toto-1.4.0/tests/test_common_args.py` & `in_toto-2.0.0/tests/test_common_args.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,92 +14,103 @@
 <Copyright>
   See LICENSE for licensing information.
 
 <Purpose>
   Test in_toto/common_args.py
 
 """
-import unittest
 import argparse
+import unittest
+
 from in_toto.common_args import (
-  sort_action_groups,
-  title_case_action_groups,
-  KEY_PASSWORD_ARGS,
-  KEY_PASSWORD_KWARGS,
-  parse_password_and_prompt_args,
-  OPTS_TITLE)
+    KEY_PASSWORD_ARGS,
+    KEY_PASSWORD_KWARGS,
+    OPTS_TITLE,
+    parse_password_and_prompt_args,
+    sort_action_groups,
+    title_case_action_groups,
+)
 
 
 class TestCommonArgs(unittest.TestCase):
-  def test_parse_password_and_prompt_args(self):
-    """"Test parse -P/--password optional arg (nargs=?, const=True). """
-    parser = argparse.ArgumentParser()
-    parser.add_argument(*KEY_PASSWORD_ARGS, **KEY_PASSWORD_KWARGS)
-
-    # parameter list | expected result tuple, i.e password, prompt
-    tests = [
-      ([], (None, False)),
-      (["--password"], (None, True)),
-      (["--password", "123456"], ("123456", False)),
-      (["-P"], (None, True)),
-      (["-P", "123456"], ("123456", False))
-    ]
-
-    for idx, (params, expected) in enumerate(tests):
-      result = parse_password_and_prompt_args(parser.parse_args(params))
-      self.assertTupleEqual(result, expected, "(row {})".format(idx))
+    def test_parse_password_and_prompt_args(self):
+        """Test parse -P/--password optional arg (nargs=?, const=True)."""
+        parser = argparse.ArgumentParser()
+        parser.add_argument(*KEY_PASSWORD_ARGS, **KEY_PASSWORD_KWARGS)
+
+        # parameter list | expected result tuple, i.e password, prompt
+        tests = [
+            ([], (None, False)),
+            (["--password"], (None, True)),
+            (["--password", "123456"], ("123456", False)),
+            (["-P"], (None, True)),
+            (["-P", "123456"], ("123456", False)),
+        ]
+
+        for idx, (params, expected) in enumerate(tests):
+            result = parse_password_and_prompt_args(parser.parse_args(params))
+            self.assertTupleEqual(result, expected, "(row {})".format(idx))
 
 
 class TestArgparseActionGroupHelpers(unittest.TestCase):
-  # pylint: disable=protected-access
+    # pylint: disable=protected-access
 
-  def setUp(self):
-    """Create an empty parser and perform some basic assertions prior to
-    testing parser action group (i.e. argument group) helper functions. """
-    # Create empty argument parser
-    self.parser = argparse.ArgumentParser()
-
-    # Assert parser has the protected member "_action_groups" and it is a list
-    # NOTE: argparse could remove this at any time without notice
-    self.assertTrue(type(getattr(self.parser, "_action_groups", None)) == list) # pylint: disable=unidiomatic-typecheck
-
-    # Assert default action groups with default titles' case and default order
-    self.assertListEqual([group.title for group in self.parser._action_groups],
-        ["positional arguments", OPTS_TITLE.lower()])
-
-
-  def test_title_case_action_groups(self):
-    """Test title_case_action_groups title cases action group titles. """
-    # Make titles title-case (default is asserted in setUp)
-    title_case_action_groups(self.parser)
-
-    # Assert successful title-casing
-    self.assertListEqual([group.title for group in self.parser._action_groups],
-        ["Positional Arguments", OPTS_TITLE])
-
-
-  def test_sort_action_groups(self):
-    """Test sort_action_groups sorts action groups by custom title order. """
-    # Create custom order for titles (default is asserted in setUp)
-    custom_order = [OPTS_TITLE.lower(), "positional arguments"]
-    sort_action_groups(self.parser, title_order=custom_order)
-    # Assert successful re-ordering
-    self.assertListEqual([group.title for group in self.parser._action_groups],
-        custom_order)
-
-
-    # Add custom group to parser that exists in most in-toto command line tools
-    self.parser.add_argument_group("required named arguments")
-
-    # Test default custom order of action groups titles (which are title-cased)
-    title_case_action_groups(self.parser)
-    sort_action_groups(self.parser)
-    default_custom_order = ["Required Named Arguments", "Positional Arguments",
-        OPTS_TITLE]
-
-    # Assert successful(title-casing) re-ordering
-    self.assertListEqual([group.title for group in self.parser._action_groups],
-        default_custom_order)
+    def setUp(self):
+        """Create an empty parser and perform some basic assertions prior to
+        testing parser action group (i.e. argument group) helper functions."""
+        # Create empty argument parser
+        self.parser = argparse.ArgumentParser()
+
+        # Assert parser has the protected member "_action_groups" and it is a list
+        # NOTE: argparse could remove this at any time without notice
+        self.assertIsInstance(
+            getattr(self.parser, "_action_groups", None), list
+        )
+
+        # Assert default action groups with default titles' case and default order
+        self.assertListEqual(
+            [group.title for group in self.parser._action_groups],
+            ["positional arguments", OPTS_TITLE.lower()],
+        )
+
+    def test_title_case_action_groups(self):
+        """Test title_case_action_groups title cases action group titles."""
+        # Make titles title-case (default is asserted in setUp)
+        title_case_action_groups(self.parser)
+
+        # Assert successful title-casing
+        self.assertListEqual(
+            [group.title for group in self.parser._action_groups],
+            ["Positional Arguments", OPTS_TITLE],
+        )
+
+    def test_sort_action_groups(self):
+        """Test sort_action_groups sorts action groups by custom title order."""
+        # Create custom order for titles (default is asserted in setUp)
+        custom_order = [OPTS_TITLE.lower(), "positional arguments"]
+        sort_action_groups(self.parser, title_order=custom_order)
+        # Assert successful re-ordering
+        self.assertListEqual(
+            [group.title for group in self.parser._action_groups], custom_order
+        )
+
+        # Add custom group to parser that exists in most in-toto command line tools
+        self.parser.add_argument_group("required named arguments")
+
+        # Test default custom order of action groups titles (which are title-cased)
+        title_case_action_groups(self.parser)
+        sort_action_groups(self.parser)
+        default_custom_order = [
+            "Required Named Arguments",
+            "Positional Arguments",
+            OPTS_TITLE,
+        ]
+
+        # Assert successful(title-casing) re-ordering
+        self.assertListEqual(
+            [group.title for group in self.parser._action_groups],
+            default_custom_order,
+        )
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_in_toto_keygen.py` & `in_toto-2.0.0/tests/test_in_toto_keygen.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,75 +15,84 @@
 
 """
 import sys
 import unittest
 from unittest.mock import patch
 
 from in_toto.in_toto_keygen import main as in_toto_keygen_main
-
 from tests.common import TmpDirMixin
 
 
 class TestInTotoKeyGenTool(unittest.TestCase, TmpDirMixin):
-  """Test in_toto_keygen's main() - requires sys.argv patching; error
-  logs/exits on Exception. """
+    """Test in_toto_keygen's main() - requires sys.argv patching; error
+    logs/exits on Exception."""
+
+    @classmethod
+    def setUpClass(self):
+        self.set_up_test_dir()
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_main_required_args(self):
+        """Test in-toto-keygen CLI tool with required arguments."""
+        args = ["in_toto_keygen.py"]
+
+        with patch.object(sys, "argv", args + ["bob"]), self.assertRaises(
+            SystemExit
+        ):
+            in_toto_keygen_main()
+
+    def test_main_optional_args(self):
+        """Test CLI command keygen with optional arguments."""
+        args = ["in_toto_keygen.py"]
+        password = "123456"
+        with patch.object(sys, "argv", args + ["-p", "bob"]), patch(
+            "getpass.getpass", return_value=password
+        ), self.assertRaises(SystemExit):
+            in_toto_keygen_main()
+        with patch.object(
+            sys, "argv", args + ["-p", "-t", "rsa", "bob"]
+        ), patch("getpass.getpass", return_value=password), self.assertRaises(
+            SystemExit
+        ):
+            in_toto_keygen_main()
+        with patch.object(
+            sys, "argv", args + ["-t", "ed25519", "bob"]
+        ), self.assertRaises(SystemExit):
+            in_toto_keygen_main()
+        with patch.object(
+            sys, "argv", args + ["-t", "ecdsa", "bob"]
+        ), self.assertRaises(SystemExit):
+            in_toto_keygen_main()
+        with patch.object(
+            sys, "argv", args + ["-p", "-t", "ed25519", "bob"]
+        ), patch("getpass.getpass", return_value=password), self.assertRaises(
+            SystemExit
+        ):
+            in_toto_keygen_main()
+        with patch.object(
+            sys, "argv", args + ["-p", "-b", "3072", "bob"]
+        ), patch("getpass.getpass", return_value=password), self.assertRaises(
+            SystemExit
+        ):
+            in_toto_keygen_main()
+
+    def test_main_wrong_args(self):
+        """Test CLI command with missing arguments."""
+        wrong_args_list = [
+            ["in_toto_keygen.py"],
+            ["in_toto_keygen.py", "-r"],
+            ["in_toto_keygen.py", "-p", "-b", "1024", "bob"],
+        ]
+        password = "123456"
+
+        for wrong_args in wrong_args_list:
+            with patch.object(sys, "argv", wrong_args), patch(
+                "getpass.getpass", return_value=password
+            ), self.assertRaises(SystemExit):
+                in_toto_keygen_main()
 
-  @classmethod
-  def setUpClass(self):
-    self.set_up_test_dir()
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def test_main_required_args(self):
-    """Test in-toto-keygen CLI tool with required arguments. """
-    args = ["in_toto_keygen.py"]
-
-    with patch.object(sys, 'argv', args + ["bob"]), \
-      self.assertRaises(SystemExit):
-      in_toto_keygen_main()
-
-
-  def test_main_optional_args(self):
-    """Test CLI command keygen with optional arguments. """
-    args = ["in_toto_keygen.py"]
-    password = "123456"
-    with patch.object(sys, 'argv', args + ["-p", "bob"]), \
-      patch("getpass.getpass", return_value=password), self.assertRaises(
-      SystemExit):
-      in_toto_keygen_main()
-    with patch.object(sys, 'argv', args + ["-p", "-t", "rsa", "bob"]), \
-      patch("getpass.getpass", return_value=password), self.assertRaises(
-      SystemExit):
-      in_toto_keygen_main()
-    with patch.object(sys, 'argv', args + ["-t", "ed25519", "bob"]), \
-      self.assertRaises(SystemExit):
-      in_toto_keygen_main()
-    with patch.object(sys, 'argv', args + ["-t", "ecdsa", "bob"]), \
-      self.assertRaises(SystemExit):
-      in_toto_keygen_main()
-    with patch.object(sys, 'argv', args + ["-p", "-t", "ed25519", "bob"]), \
-      patch("getpass.getpass", return_value=password), self.assertRaises(
-      SystemExit):
-      in_toto_keygen_main()
-    with patch.object(sys, 'argv', args + ["-p", "-b", "3072", "bob"]), \
-      patch("getpass.getpass", return_value=password), self.assertRaises(
-      SystemExit):
-      in_toto_keygen_main()
-
-
-  def test_main_wrong_args(self):
-    """Test CLI command with missing arguments. """
-    wrong_args_list = [
-      ["in_toto_keygen.py"],
-      ["in_toto_keygen.py", "-r"],
-      ["in_toto_keygen.py", "-p", "-b", "1024", "bob"]]
-    password = "123456"
-
-    for wrong_args in wrong_args_list:
-      with patch.object(sys, 'argv', wrong_args), patch("getpass.getpass",
-        return_value=password), self.assertRaises(SystemExit):
-        in_toto_keygen_main()
 
-if __name__ == '__main__':
-  unittest.main()
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_in_toto_mock.py` & `in_toto-2.0.0/tests/test_in_toto_mock.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,89 +16,81 @@
 <Copyright>
   See LICENSE for licensing information.
 
 <Purpose>
   Test in_toto_mock command line tool.
 
 """
+import logging
 import os
 import unittest
-import logging
-
-from in_toto.in_toto_mock import main as in_toto_mock_main
 from pathlib import Path
 
+from in_toto.in_toto_mock import main as in_toto_mock_main
 from tests.common import CliTestCase, TmpDirMixin
 
 # Required to cache and restore default log level
 logger = logging.getLogger("in_toto")
 
 
 class TestInTotoMockTool(CliTestCase, TmpDirMixin):
-  """Test in_toto_mock's main() - requires sys.argv patching; and
-  in_toto_mock- calls runlib and error logs/exits on Exception. """
-  cli_main_func = staticmethod(in_toto_mock_main)
-
-  @classmethod
-  def setUpClass(self):
-    """Create and change into temporary directory,
-    dummy artifact and base arguments. """
-    self.set_up_test_dir()
-
-    # Below tests override the base logger ('in_toto') log level to
-    # `logging.INFO`. We cache the original log level before running the tests
-    # to restore it afterwards.
-    self._base_log_level = logger.level
-
-    self.test_step = "test_step"
-    self.test_link = self.test_step + ".link"
-    self.test_artifact = "test_artifact"
-    Path(self.test_artifact).touch()
-
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-    # Restore log level to what it was before running in-toto-mock
-    logger.setLevel(self._base_log_level)
-
-
-  def tearDown(self):
-    try:
-      os.remove(self.test_link)
-    except OSError:
-      pass
-
-
-  def test_main_required_args(self):
-    """Test CLI command with required arguments. """
-
-    args = ["--name", self.test_step, "--", "python", "--version"]
-    self.assert_cli_sys_exit(args, 0)
-
-    self.assertTrue(os.path.exists(self.test_link))
-
-
-  def test_main_wrong_args(self):
-    """Test CLI command with missing arguments. """
-
-    wrong_args_list = [
-      [],
-      ["--name", "test-step"],
-      ["--", "echo", "blub"]]
-
-    for wrong_args in wrong_args_list:
-      self.assert_cli_sys_exit(wrong_args, 2)
-      self.assertFalse(os.path.exists(self.test_link))
+    """Test in_toto_mock's main() - requires sys.argv patching; and
+    in_toto_mock- calls runlib and error logs/exits on Exception."""
 
+    cli_main_func = staticmethod(in_toto_mock_main)
 
-  def test_main_bad_cmd(self):
-    """Test CLI command with non-existing command. """
-    # TODO: Is it safe to assume this command does not exist, or should we
-    # assert for it?
-    args = ["-n", "bad-command", "--", "ggadsfljasdhlasdfljvzxc"]
-    self.assert_cli_sys_exit(args, 1)
+    @classmethod
+    def setUpClass(self):
+        """Create and change into temporary directory,
+        dummy artifact and base arguments."""
+        self.set_up_test_dir()
+
+        # Below tests override the base logger ('in_toto') log level to
+        # `logging.INFO`. We cache the original log level before running the tests
+        # to restore it afterwards.
+        self._base_log_level = logger.level
+
+        self.test_step = "test_step"
+        self.test_link = self.test_step + ".link"
+        self.test_artifact = "test_artifact"
+        Path(self.test_artifact).touch()
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+        # Restore log level to what it was before running in-toto-mock
+        logger.setLevel(self._base_log_level)
+
+    def tearDown(self):
+        try:
+            os.remove(self.test_link)
+        except OSError:
+            pass
+
+    def test_main_required_args(self):
+        """Test CLI command with required arguments."""
+
+        args = ["--name", self.test_step, "--", "python", "--version"]
+        self.assert_cli_sys_exit(args, 0)
+
+        self.assertTrue(os.path.exists(self.test_link))
+
+    def test_main_wrong_args(self):
+        """Test CLI command with missing arguments."""
+
+        wrong_args_list = [[], ["--name", "test-step"], ["--", "echo", "blub"]]
+
+        for wrong_args in wrong_args_list:
+            self.assert_cli_sys_exit(wrong_args, 2)
+            self.assertFalse(os.path.exists(self.test_link))
+
+    def test_main_bad_cmd(self):
+        """Test CLI command with non-existing command."""
+        # TODO: Is it safe to assume this command does not exist, or should we
+        # assert for it?
+        args = ["-n", "bad-command", "--", "ggadsfljasdhlasdfljvzxc"]
+        self.assert_cli_sys_exit(args, 1)
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_in_toto_run.py` & `in_toto-2.0.0/tests/test_in_toto_run.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,377 +17,503 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Test in_toto_run command line tool.
 
 """
 
-import os
-import unittest
 import glob
+import os
 import tempfile
-
+import unittest
 from pathlib import Path
 from unittest import mock
 
-from in_toto.models.metadata import Metadata, Metablock
+import securesystemslib.interface  # pylint: disable=unused-import
+
 from in_toto.in_toto_run import main as in_toto_run_main
 from in_toto.models.link import FILENAME_FORMAT
-
-from tests.common import CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin
-
-import securesystemslib.interface # pylint: disable=unused-import
+from in_toto.models.metadata import Metablock, Metadata
+from tests.common import CliTestCase, GenKeysMixin, GPGKeysMixin, TmpDirMixin
 
 
 class TestInTotoRunTool(CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin):
-  """Test in_toto_run's main() - requires sys.argv patching; and
-  in_toto_run- calls runlib and error logs/exits on Exception. """
-  cli_main_func = staticmethod(in_toto_run_main)
-
-  @classmethod
-  def setUpClass(self):
-    """Create and change into temporary directory,
-    generate key pair, dummy artifact and base arguments. """
-    self.set_up_test_dir()
-    self.set_up_gpg_keys()
-    self.set_up_keys()
-
-    self.test_step = "test_step"
-    self.test_link_rsa = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.rsa_key_id)
-    self.test_link_ed25519 = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.ed25519_key_id)
-    self.test_link_ecdsa = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.ecdsa_key_id)
-    self.test_link_rsa_enc = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.rsa_key_enc_id)
-    self.test_link_ed25519_enc = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.ed25519_key_enc_id)
-    self.test_link_ecdsa_enc = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.ecdsa_key_enc_id)
-
-    self.test_artifact = "test_artifact"
-    Path(self.test_artifact).touch()
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def tearDown(self):
-    for link in glob.glob("*.link"):
-      os.remove(link)
-
-  def test_main_required_args(self):
-    """Test CLI command with required arguments. """
-
-    args = ["--step-name", self.test_step, "--key", self.rsa_key_path, "--",
-        "python", "--version"]
-
-    self.assert_cli_sys_exit(args, 0)
-    self.assertTrue(os.path.exists(self.test_link_rsa))
-
-
-  def test_main_optional_args(self):
-    """Test CLI command with optional arguments. """
-
-    named_args = ["--step-name", self.test_step, "--key",
-        self.rsa_key_path, "--materials", self.test_artifact, "--products",
-        self.test_artifact, "--record-streams"]
-    positional_args = ["--", "python", "--version"]
-
-    # Test and assert recorded artifacts
-    args1 = named_args + positional_args
-    self.assert_cli_sys_exit(args1, 0)
-    link_metadata = Metablock.load(self.test_link_rsa)
-    self.assertTrue(self.test_artifact in
-        list(link_metadata.signed.materials.keys()))
-    self.assertTrue(self.test_artifact in
-        list(link_metadata.signed.products.keys()))
-
-    # Test and assert exlcuded artifacts
-    args2 = named_args + ["--exclude", "*test*"] + positional_args
-    self.assert_cli_sys_exit(args2, 0)
-    link_metadata = Metablock.load(self.test_link_rsa)
-    self.assertFalse(link_metadata.signed.materials)
-    self.assertFalse(link_metadata.signed.products)
-
-    # Test with base path
-    args3 = named_args + ["--base-path", self.test_dir] + positional_args
-    self.assert_cli_sys_exit(args3, 0)
-    link_metadata = Metablock.load(self.test_link_rsa)
-    self.assertListEqual(list(link_metadata.signed.materials.keys()),
-        [self.test_artifact])
-    self.assertListEqual(list(link_metadata.signed.products.keys()),
-        [self.test_artifact])
-
-    # Test with bogus base path
-    args4 = named_args + ["--base-path", "bogus/path"] + positional_args
-    self.assert_cli_sys_exit(args4, 1)
-
-    # Test with lstrip path
-    strip_prefix = self.test_artifact[:-1]
-    args5 = named_args + ["--lstrip-paths", strip_prefix] + positional_args
-    self.assert_cli_sys_exit(args5, 0)
-    link_metadata = Metablock.load(self.test_link_rsa)
-    self.assertListEqual(list(link_metadata.signed.materials.keys()),
-        [self.test_artifact[len(strip_prefix):]])
-    self.assertListEqual(list(link_metadata.signed.products.keys()),
-        [self.test_artifact[len(strip_prefix):]])
-
-
-  def test_main_with_metadata_directory(self):
-    """Test CLI command with metadata directory. """
-    tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
-    args = ["--step-name", self.test_step, "--key", self.rsa_key_path,
-        "--metadata-directory", tmp_dir, "--", "python", "--version"]
-
-    self.assert_cli_sys_exit(args, 0)
-
-    linkpath = os.path.join(tmp_dir, self.test_link_rsa)
-
-    self.assertTrue(os.path.exists(linkpath))
-
-
-  def test_main_with_unencrypted_ed25519_key(self):
-    """Test CLI command with ed25519 key. """
-    args = ["-n", self.test_step,
-        "--key", self.ed25519_key_path,
-        "--key-type", "ed25519", "--", "ls"]
-
-    self.assert_cli_sys_exit(args, 0)
-    self.assertTrue(os.path.exists(self.test_link_ed25519))
-
-  def test_main_with_unencrypted_ecdsa_key(self):
-    """Test CLI command with ecdsa key. """
-    args = ["-n", self.test_step,
-        "--key", self.ecdsa_key_path,
-        "--key-type", "ecdsa", "--", "ls"]
-
-    self.assert_cli_sys_exit(args, 0)
-    self.assertTrue(os.path.exists(self.test_link_ecdsa))
-
-
-  def test_main_with_encrypted_keys(self):
-    """Test CLI command with encrypted ed25519 key. """
-
-    for key_type, key_path, link_path in [
-        ("rsa", self.rsa_key_enc_path, self.test_link_rsa_enc),
-        ("ed25519", self.ed25519_key_enc_path, self.test_link_ed25519_enc),
-        ("ecdsa", self.ecdsa_key_enc_path, self.test_link_ecdsa_enc)]:
-
-
-      # Define common arguments passed to in in-toto-run below
-      args = [
-          "-n", self.test_step,
-          "--key", key_path,
-          "--key-type", key_type]
-      cmd = ["--", "python", "--version"]
-
-      # Make sure the link file to be generated doesn't already exist
-      self.assertFalse(os.path.exists(link_path))
-
-      # Test 1: Call in-toto-run entering signing key password on prompt
-      with mock.patch('securesystemslib.interface.get_password',
-          return_value=self.key_pw):
-        self.assert_cli_sys_exit(args + ["--password"] + cmd, 0)
-
-      self.assertTrue(os.path.exists(link_path))
-      os.remove(link_path)
-
-      # Test 2: Call in-toto-run passing signing key password
-      self.assert_cli_sys_exit(args + ["--password", self.key_pw] + cmd, 0)
-      self.assertTrue(os.path.exists(link_path))
-      os.remove(link_path)
-
-
-  def test_main_with_specified_gpg_key(self):
-    """Test CLI command with specified gpg key. """
-    args = ["-n", self.test_step,
-            "--gpg", self.gpg_key_85DA58,
-            "--gpg-home", self.gnupg_home, "--", "python", "--version"]
-
-    self.assert_cli_sys_exit(args, 0)
-    link_filename = FILENAME_FORMAT.format(step_name=self.test_step,
-        keyid=self.gpg_key_85DA58)
-
-    self.assertTrue(os.path.exists(link_filename))
-
-
-  def test_main_with_default_gpg_key(self):
-    """Test CLI command with default gpg key. """
-    args = ["-n", self.test_step,
-            "--gpg", "--gpg-home", self.gnupg_home, "--", "python", "--version"]
-
-    self.assert_cli_sys_exit(args, 0)
-
-    link_filename = FILENAME_FORMAT.format(step_name=self.test_step,
-        keyid=self.gpg_key_D924E9)
-
-    self.assertTrue(os.path.exists(link_filename))
-
-
-  def test_main_no_command_arg(self):
-    """Test CLI command with --no-command argument. """
-
-    args = ["in_toto_run.py", "--step-name", self.test_step, "--key",
-        self.rsa_key_path, "--no-command"]
-
-    self.assert_cli_sys_exit(args, 0)
-
-    self.assertTrue(os.path.exists(self.test_link_rsa))
-
-  def test_main_wrong_args(self):
-    """Test CLI command with missing arguments. """
-
-    wrong_args_list = [
-      [],
-      ["--step-name", "some"],
-      ["--key", self.rsa_key_path],
-      ["--", "echo", "blub"],
-      ["--step-name", "test-step", "--key", self.rsa_key_path],
-      ["--step-name", "--", "echo", "blub"],
-      ["--key", self.rsa_key_path, "--", "echo", "blub"],
-      ["--step-name", "test-step", "--key", self.rsa_key_path, "--"],
-      ["--step-name", "test-step",
-           "--key", self.rsa_key_path, "--gpg", "--", "echo", "blub"]
-    ]
-
-    for wrong_args in wrong_args_list:
-      self.assert_cli_sys_exit(wrong_args, 2)
-      self.assertFalse(os.path.exists(self.test_link_rsa))
-
-  def test_main_wrong_key_exits(self):
-    """Test CLI command with wrong key argument, exits and logs error """
-
-    args = ["--step-name", self.test_step, "--key",
-       "non-existing-key", "--", "echo", "test"]
-
-    self.assert_cli_sys_exit(args, 1)
-    self.assertFalse(os.path.exists(self.test_link_rsa))
-
-
-  def test_main_encrypted_key_but_no_pw(self):
-    """Test CLI command exits 1 with encrypted key but no pw. """
-    args = ["-n", self.test_step, "--key", self.rsa_key_enc_path, "-x"]
-    self.assert_cli_sys_exit(args, 1)
-    self.assertFalse(os.path.exists(self.test_link_rsa_enc))
-
-    args = ["-n", self.test_step, "--key", self.ed25519_key_enc_path, "-x"]
-    self.assert_cli_sys_exit(args, 1)
-    self.assertFalse(os.path.exists(self.test_link_ed25519_enc))
-
-
-class TestInTotoRunToolWithDSSE(CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin):
-  """Test in_toto_run's main() with --use-dsse argument - requires sys.argv
-  patching; and in_toto_run- calls runlib and error logs/exits on Exception."""
-  cli_main_func = staticmethod(in_toto_run_main)
-
-  @classmethod
-  def setUpClass(self):
-    """Create and change into temporary directory,
-    generate key pair, dummy artifact and base arguments. """
-    self.set_up_test_dir()
-    self.set_up_gpg_keys()
-    self.set_up_keys()
-
-    self.test_step = "test_step"
-    self.test_link_rsa = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.rsa_key_id)
-    self.test_link_ed25519 = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.ed25519_key_id)
-    self.test_link_rsa_enc = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.rsa_key_enc_id)
-    self.test_link_ed25519_enc = FILENAME_FORMAT.format(
-        step_name=self.test_step, keyid=self.ed25519_key_enc_id)
-
-    self.test_artifact = "test_artifact"
-    Path(self.test_artifact).touch()
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def tearDown(self):
-    for link in glob.glob("*.link"):
-      os.remove(link)
-
-  def test_main_required_args(self):
-    """Test CLI command with required arguments. """
-
-    args = ["--step-name", self.test_step, "--key", self.rsa_key_path,
-        "--use-dsse", "--", "python", "--version"]
-
-    self.assert_cli_sys_exit(args, 0)
-    self.assertTrue(os.path.exists(self.test_link_rsa))
-
-
-  def test_main_optional_args(self):
-    """Test CLI command with optional arguments. """
-
-    named_args = ["--step-name", self.test_step, "--key",
-        self.rsa_key_path, "--materials", self.test_artifact, "--products",
-        self.test_artifact, "--record-streams", "--use-dsse"]
-    positional_args = ["--", "python", "--version"]
-
-    # Test and assert recorded artifacts
-    args1 = named_args + positional_args
-    self.assert_cli_sys_exit(args1, 0)
-    metadata = Metadata.load(self.test_link_rsa)
-    link = metadata.get_payload()
-    self.assertTrue(self.test_artifact in
-        list(link.materials.keys()))
-    self.assertTrue(self.test_artifact in
-        list(link.products.keys()))
-
-    # Test and assert exlcuded artifacts
-    args2 = named_args + ["--exclude", "*test*"] + positional_args
-    self.assert_cli_sys_exit(args2, 0)
-    link = Metadata.load(self.test_link_rsa).get_payload()
-    self.assertFalse(link.materials)
-    self.assertFalse(link.products)
-
-    # Test with base path
-    args3 = named_args + ["--base-path", self.test_dir] + positional_args
-    self.assert_cli_sys_exit(args3, 0)
-    link = Metadata.load(self.test_link_rsa).get_payload()
-    self.assertListEqual(list(link.materials.keys()),
-        [self.test_artifact])
-    self.assertListEqual(list(link.products.keys()),
-        [self.test_artifact])
-
-    # Test with bogus base path
-    args4 = named_args + ["--base-path", "bogus/path"] + positional_args
-    self.assert_cli_sys_exit(args4, 1)
-
-    # Test with lstrip path
-    strip_prefix = self.test_artifact[:-1]
-    args5 = named_args + ["--lstrip-paths", strip_prefix] + positional_args
-    self.assert_cli_sys_exit(args5, 0)
-    link = Metadata.load(self.test_link_rsa).get_payload()
-    self.assertListEqual(list(link.materials.keys()),
-        [self.test_artifact[len(strip_prefix):]])
-    self.assertListEqual(list(link.products.keys()),
-        [self.test_artifact[len(strip_prefix):]])
-
-
-  def test_main_with_default_gpg_key(self):
-    """Test CLI command with default gpg key."""
-    args = ["-n", self.test_step,
-            "--gpg", "--gpg-home", self.gnupg_home, "--use-dsse",
-            "--", "python", "--version"]
-
-    self.assert_cli_sys_exit(args, 1)
-
-
-  def test_main_no_command_arg(self):
-    """Test CLI command with --no-command argument. """
+    """Test in_toto_run's main() - requires sys.argv patching; and
+    in_toto_run- calls runlib and error logs/exits on Exception."""
+
+    cli_main_func = staticmethod(in_toto_run_main)
 
-    args = ["in_toto_run.py", "--step-name", self.test_step, "--key",
-        self.rsa_key_path, "--no-command", "--use-dsse"]
+    @classmethod
+    def setUpClass(self):
+        """Create and change into temporary directory,
+        generate key pair, dummy artifact and base arguments."""
+        self.set_up_test_dir()
+        self.set_up_gpg_keys()
+        self.set_up_keys()
+
+        self.test_step = "test_step"
+        self.test_link_rsa = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.rsa_key_id
+        )
+        self.test_link_ed25519 = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.ed25519_key_id
+        )
+        self.test_link_ecdsa = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.ecdsa_key_id
+        )
+        self.test_link_rsa_enc = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.rsa_key_enc_id
+        )
+        self.test_link_ed25519_enc = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.ed25519_key_enc_id
+        )
+        self.test_link_ecdsa_enc = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.ecdsa_key_enc_id
+        )
+
+        self.test_artifact = "test_artifact"
+        Path(self.test_artifact).touch()
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def tearDown(self):
+        for link in glob.glob("*.link"):
+            os.remove(link)
+
+    def test_main_required_args(self):
+        """Test CLI command with required arguments."""
+
+        args = [
+            "--step-name",
+            self.test_step,
+            "--key",
+            self.rsa_key_path,
+            "--",
+            "python",
+            "--version",
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+        self.assertTrue(os.path.exists(self.test_link_rsa))
+
+    def test_main_optional_args(self):
+        """Test CLI command with optional arguments."""
+
+        named_args = [
+            "--step-name",
+            self.test_step,
+            "--key",
+            self.rsa_key_path,
+            "--materials",
+            self.test_artifact,
+            "--products",
+            self.test_artifact,
+            "--record-streams",
+        ]
+        positional_args = ["--", "python", "--version"]
+
+        # Test and assert recorded artifacts
+        args1 = named_args + positional_args
+        self.assert_cli_sys_exit(args1, 0)
+        link_metadata = Metablock.load(self.test_link_rsa)
+        self.assertTrue(
+            self.test_artifact in list(link_metadata.signed.materials.keys())
+        )
+        self.assertTrue(
+            self.test_artifact in list(link_metadata.signed.products.keys())
+        )
+
+        # Test and assert exlcuded artifacts
+        args2 = named_args + ["--exclude", "*test*"] + positional_args
+        self.assert_cli_sys_exit(args2, 0)
+        link_metadata = Metablock.load(self.test_link_rsa)
+        self.assertFalse(link_metadata.signed.materials)
+        self.assertFalse(link_metadata.signed.products)
+
+        # Test with base path
+        args3 = named_args + ["--base-path", self.test_dir] + positional_args
+        self.assert_cli_sys_exit(args3, 0)
+        link_metadata = Metablock.load(self.test_link_rsa)
+        self.assertListEqual(
+            list(link_metadata.signed.materials.keys()), [self.test_artifact]
+        )
+        self.assertListEqual(
+            list(link_metadata.signed.products.keys()), [self.test_artifact]
+        )
+
+        # Test with bogus base path
+        args4 = named_args + ["--base-path", "bogus/path"] + positional_args
+        self.assert_cli_sys_exit(args4, 1)
+
+        # Test with lstrip path
+        strip_prefix = self.test_artifact[:-1]
+        args5 = named_args + ["--lstrip-paths", strip_prefix] + positional_args
+        self.assert_cli_sys_exit(args5, 0)
+        link_metadata = Metablock.load(self.test_link_rsa)
+        self.assertListEqual(
+            list(link_metadata.signed.materials.keys()),
+            [self.test_artifact[len(strip_prefix) :]],
+        )
+        self.assertListEqual(
+            list(link_metadata.signed.products.keys()),
+            [self.test_artifact[len(strip_prefix) :]],
+        )
+
+    def test_main_with_metadata_directory(self):
+        """Test CLI command with metadata directory."""
+        tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
+        args = [
+            "--step-name",
+            self.test_step,
+            "--key",
+            self.rsa_key_path,
+            "--metadata-directory",
+            tmp_dir,
+            "--",
+            "python",
+            "--version",
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+
+        linkpath = os.path.join(tmp_dir, self.test_link_rsa)
+
+        self.assertTrue(os.path.exists(linkpath))
+
+    def test_main_with_unencrypted_ed25519_key(self):
+        """Test CLI command with ed25519 key."""
+        args = [
+            "-n",
+            self.test_step,
+            "--key",
+            self.ed25519_key_path,
+            "--key-type",
+            "ed25519",
+            "--",
+            "ls",
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+        self.assertTrue(os.path.exists(self.test_link_ed25519))
+
+    def test_main_with_unencrypted_ecdsa_key(self):
+        """Test CLI command with ecdsa key."""
+        args = [
+            "-n",
+            self.test_step,
+            "--key",
+            self.ecdsa_key_path,
+            "--key-type",
+            "ecdsa",
+            "--",
+            "ls",
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+        self.assertTrue(os.path.exists(self.test_link_ecdsa))
+
+    def test_main_with_encrypted_keys(self):
+        """Test CLI command with encrypted ed25519 key."""
+
+        for key_type, key_path, link_path in [
+            ("rsa", self.rsa_key_enc_path, self.test_link_rsa_enc),
+            ("ed25519", self.ed25519_key_enc_path, self.test_link_ed25519_enc),
+            ("ecdsa", self.ecdsa_key_enc_path, self.test_link_ecdsa_enc),
+        ]:
+            # Define common arguments passed to in in-toto-run below
+            args = [
+                "-n",
+                self.test_step,
+                "--key",
+                key_path,
+                "--key-type",
+                key_type,
+            ]
+            cmd = ["--", "python", "--version"]
+
+            # Make sure the link file to be generated doesn't already exist
+            self.assertFalse(os.path.exists(link_path))
+
+            # Test 1: Call in-toto-run entering signing key password on prompt
+            with mock.patch(
+                "securesystemslib.interface.get_password",
+                return_value=self.key_pw,
+            ):
+                self.assert_cli_sys_exit(args + ["--password"] + cmd, 0)
+
+            self.assertTrue(os.path.exists(link_path))
+            os.remove(link_path)
+
+            # Test 2: Call in-toto-run passing signing key password
+            self.assert_cli_sys_exit(
+                args + ["--password", self.key_pw] + cmd, 0
+            )
+            self.assertTrue(os.path.exists(link_path))
+            os.remove(link_path)
+
+    def test_main_with_specified_gpg_key(self):
+        """Test CLI command with specified gpg key."""
+        args = [
+            "-n",
+            self.test_step,
+            "--gpg",
+            self.gpg_key_85DA58,
+            "--gpg-home",
+            self.gnupg_home,
+            "--",
+            "python",
+            "--version",
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+        link_filename = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.gpg_key_85DA58
+        )
+
+        self.assertTrue(os.path.exists(link_filename))
+
+    def test_main_with_default_gpg_key(self):
+        """Test CLI command with default gpg key."""
+        args = [
+            "-n",
+            self.test_step,
+            "--gpg",
+            "--gpg-home",
+            self.gnupg_home,
+            "--",
+            "python",
+            "--version",
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+
+        link_filename = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.gpg_key_D924E9
+        )
+
+        self.assertTrue(os.path.exists(link_filename))
+
+    def test_main_no_command_arg(self):
+        """Test CLI command with --no-command argument."""
+
+        args = [
+            "in_toto_run.py",
+            "--step-name",
+            self.test_step,
+            "--key",
+            self.rsa_key_path,
+            "--no-command",
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+
+        self.assertTrue(os.path.exists(self.test_link_rsa))
+
+    def test_main_wrong_args(self):
+        """Test CLI command with missing arguments."""
+
+        wrong_args_list = [
+            [],
+            ["--step-name", "some"],
+            ["--key", self.rsa_key_path],
+            ["--", "echo", "blub"],
+            ["--step-name", "test-step", "--key", self.rsa_key_path],
+            ["--step-name", "--", "echo", "blub"],
+            ["--key", self.rsa_key_path, "--", "echo", "blub"],
+            ["--step-name", "test-step", "--key", self.rsa_key_path, "--"],
+            [
+                "--step-name",
+                "test-step",
+                "--key",
+                self.rsa_key_path,
+                "--gpg",
+                "--",
+                "echo",
+                "blub",
+            ],
+        ]
+
+        for wrong_args in wrong_args_list:
+            self.assert_cli_sys_exit(wrong_args, 2)
+            self.assertFalse(os.path.exists(self.test_link_rsa))
+
+    def test_main_wrong_key_exits(self):
+        """Test CLI command with wrong key argument, exits and logs error"""
+
+        args = [
+            "--step-name",
+            self.test_step,
+            "--key",
+            "non-existing-key",
+            "--",
+            "echo",
+            "test",
+        ]
+
+        self.assert_cli_sys_exit(args, 1)
+        self.assertFalse(os.path.exists(self.test_link_rsa))
+
+    def test_main_encrypted_key_but_no_pw(self):
+        """Test CLI command exits 1 with encrypted key but no pw."""
+        args = ["-n", self.test_step, "--key", self.rsa_key_enc_path, "-x"]
+        self.assert_cli_sys_exit(args, 1)
+        self.assertFalse(os.path.exists(self.test_link_rsa_enc))
+
+        args = ["-n", self.test_step, "--key", self.ed25519_key_enc_path, "-x"]
+        self.assert_cli_sys_exit(args, 1)
+        self.assertFalse(os.path.exists(self.test_link_ed25519_enc))
+
+
+class TestInTotoRunToolWithDSSE(
+    CliTestCase, TmpDirMixin, GPGKeysMixin, GenKeysMixin
+):
+    """Test in_toto_run's main() with --use-dsse argument - requires sys.argv
+    patching; and in_toto_run- calls runlib and error logs/exits on Exception.
+    """
+
+    cli_main_func = staticmethod(in_toto_run_main)
+
+    @classmethod
+    def setUpClass(self):
+        """Create and change into temporary directory,
+        generate key pair, dummy artifact and base arguments."""
+        self.set_up_test_dir()
+        self.set_up_gpg_keys()
+        self.set_up_keys()
+
+        self.test_step = "test_step"
+        self.test_link_rsa = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.rsa_key_id
+        )
+        self.test_link_ed25519 = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.ed25519_key_id
+        )
+        self.test_link_rsa_enc = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.rsa_key_enc_id
+        )
+        self.test_link_ed25519_enc = FILENAME_FORMAT.format(
+            step_name=self.test_step, keyid=self.ed25519_key_enc_id
+        )
+
+        self.test_artifact = "test_artifact"
+        Path(self.test_artifact).touch()
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def tearDown(self):
+        for link in glob.glob("*.link"):
+            os.remove(link)
+
+    def test_main_required_args(self):
+        """Test CLI command with required arguments."""
+
+        args = [
+            "--step-name",
+            self.test_step,
+            "--key",
+            self.rsa_key_path,
+            "--use-dsse",
+            "--",
+            "python",
+            "--version",
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+        self.assertTrue(os.path.exists(self.test_link_rsa))
+
+    def test_main_optional_args(self):
+        """Test CLI command with optional arguments."""
+
+        named_args = [
+            "--step-name",
+            self.test_step,
+            "--key",
+            self.rsa_key_path,
+            "--materials",
+            self.test_artifact,
+            "--products",
+            self.test_artifact,
+            "--record-streams",
+            "--use-dsse",
+        ]
+        positional_args = ["--", "python", "--version"]
+
+        # Test and assert recorded artifacts
+        args1 = named_args + positional_args
+        self.assert_cli_sys_exit(args1, 0)
+        metadata = Metadata.load(self.test_link_rsa)
+        link = metadata.get_payload()
+        self.assertTrue(self.test_artifact in list(link.materials.keys()))
+        self.assertTrue(self.test_artifact in list(link.products.keys()))
+
+        # Test and assert exlcuded artifacts
+        args2 = named_args + ["--exclude", "*test*"] + positional_args
+        self.assert_cli_sys_exit(args2, 0)
+        link = Metadata.load(self.test_link_rsa).get_payload()
+        self.assertFalse(link.materials)
+        self.assertFalse(link.products)
+
+        # Test with base path
+        args3 = named_args + ["--base-path", self.test_dir] + positional_args
+        self.assert_cli_sys_exit(args3, 0)
+        link = Metadata.load(self.test_link_rsa).get_payload()
+        self.assertListEqual(list(link.materials.keys()), [self.test_artifact])
+        self.assertListEqual(list(link.products.keys()), [self.test_artifact])
+
+        # Test with bogus base path
+        args4 = named_args + ["--base-path", "bogus/path"] + positional_args
+        self.assert_cli_sys_exit(args4, 1)
+
+        # Test with lstrip path
+        strip_prefix = self.test_artifact[:-1]
+        args5 = named_args + ["--lstrip-paths", strip_prefix] + positional_args
+        self.assert_cli_sys_exit(args5, 0)
+        link = Metadata.load(self.test_link_rsa).get_payload()
+        self.assertListEqual(
+            list(link.materials.keys()),
+            [self.test_artifact[len(strip_prefix) :]],
+        )
+        self.assertListEqual(
+            list(link.products.keys()),
+            [self.test_artifact[len(strip_prefix) :]],
+        )
+
+    def test_main_with_default_gpg_key(self):
+        """Test CLI command with default gpg key."""
+        args = [
+            "-n",
+            self.test_step,
+            "--gpg",
+            "--gpg-home",
+            self.gnupg_home,
+            "--use-dsse",
+            "--",
+            "python",
+            "--version",
+        ]
+
+        self.assert_cli_sys_exit(args, 1)
+
+    def test_main_no_command_arg(self):
+        """Test CLI command with --no-command argument."""
+
+        args = [
+            "in_toto_run.py",
+            "--step-name",
+            self.test_step,
+            "--key",
+            self.rsa_key_path,
+            "--no-command",
+            "--use-dsse",
+        ]
 
-    self.assert_cli_sys_exit(args, 0)
+        self.assert_cli_sys_exit(args, 0)
 
-    self.assertTrue(os.path.exists(self.test_link_rsa))
+        self.assertTrue(os.path.exists(self.test_link_rsa))
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_in_toto_verify.py` & `in_toto-2.0.0/tests/test_in_toto_verify.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,428 +18,490 @@
 
 <Purpose>
   Test in_toto_verify command line tool.
 
 """
 
 import os
-import unittest
 import shutil
+import unittest
 
-from in_toto.models.metadata import Metadata
-from in_toto.in_toto_verify import main as in_toto_verify_main
-from securesystemslib.interface import (import_rsa_privatekey_from_file,
-    import_ed25519_privatekey_from_file)
 from securesystemslib.gpg.constants import have_gpg
+from securesystemslib.interface import (
+    import_ed25519_privatekey_from_file,
+    import_rsa_privatekey_from_file,
+)
 from securesystemslib.signer import SSlibSigner
 
-from tests.common import CliTestCase, TmpDirMixin, GPGKeysMixin
-
+from in_toto.in_toto_verify import main as in_toto_verify_main
+from in_toto.models.metadata import Metadata
+from tests.common import CliTestCase, GPGKeysMixin, TmpDirMixin
 
 
 class TestInTotoVerifyTool(CliTestCase, TmpDirMixin):
-  """
-  Tests
-    - in_toto_verify's main() - requires sys.argv patching;
-    - in_toto_verify - calls verifylib.in_toto_verify and error logs/exits
-      in case of a raised Exception.
-
-  Uses in-toto demo supply chain link metadata files and basic layout for
-  verification:
-
-  Copies the basic layout for different test scenarios:
-    - signed layout
-    - multiple signed layout (using two project owner keys)
-  """
-  cli_main_func = staticmethod(in_toto_verify_main)
-
-
-  @classmethod
-  def setUpClass(self):
-    """Creates and changes into temporary directory.
-    Copies demo files to temp dir...
-      - owner/functionary key pairs
-      - *.link metadata files
-      - layout template (not signed, no expiration date)
-      - final product
-
-    ...and dumps various layouts for different test scenarios
+    """
+    Tests
+      - in_toto_verify's main() - requires sys.argv patching;
+      - in_toto_verify - calls verifylib.in_toto_verify and error logs/exits
+        in case of a raised Exception.
+
+    Uses in-toto demo supply chain link metadata files and basic layout for
+    verification:
+
+    Copies the basic layout for different test scenarios:
+      - signed layout
+      - multiple signed layout (using two project owner keys)
     """
 
-    # Find demo files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-    # find where the scripts directory is located.
-    scripts_directory = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "scripts")
-
-    self.set_up_test_dir()
-
-    # Copy demo files to temp dir
-    for fn in os.listdir(demo_files):
-      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
-
-    shutil.copytree(scripts_directory, 'scripts')
-
-    # Load layout template
-    layout_template = Metadata.load("demo.layout.template")
-
-    # Store layout paths to be used in tests
-    self.layout_single_signed_path = "single-signed.layout"
-    self.layout_double_signed_path = "double-signed.layout"
-
-    # Import layout signing keys
-    alice = import_rsa_privatekey_from_file("alice")
-    bob = import_rsa_privatekey_from_file("bob")
-    self.alice_path = "alice.pub"
-    self.bob_path = "bob.pub"
-
-    # dump a single signed layout
-    layout_template.sign(alice)
-    layout_template.dump(self.layout_single_signed_path)
-    # dump a double signed layout
-    layout_template.sign(bob)
-    layout_template.dump(self.layout_double_signed_path)
-
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-
-  def test_main_required_args(self):
-    """Test in-toto-verify CLI tool with required arguments. """
-    args = ["--layout", self.layout_single_signed_path,
-        "--layout-keys", self.alice_path]
-
-    self.assert_cli_sys_exit(args, 0)
-
-
-  def test_main_wrong_args(self):
-    """Test in-toto-verify CLI tool with wrong arguments. """
-    wrong_args_list = [
-      [],
-      ["--layout", self.layout_single_signed_path],
-      ["--key", self.alice_path]]
-
-    for wrong_args in wrong_args_list:
-      self.assert_cli_sys_exit(wrong_args, 2)
-
-
-  def test_main_multiple_keys(self):
-    """Test in-toto-verify CLI tool with multiple keys. """
-    args = ["--layout", self.layout_double_signed_path,
-        "--layout-keys", self.alice_path, self.bob_path]
-    self.assert_cli_sys_exit(args, 0)
-
-
-  def test_main_failing_bad_layout_path(self):
-    """Test in-toto-verify CLI tool with bad layout path. """
-    args = ["-l", "not-a-path-to-a-layout", "-k", self.alice_path]
-    self.assert_cli_sys_exit(args, 1)
-
-
-  def test_main_link_dir(self):
-    """Test in-toto-verify CLI tool with explicit link dir. """
-
-    # Use current working directory explicitly to load links
-    args = ["--layout", self.layout_single_signed_path,
-        "--layout-keys", self.alice_path, "--link-dir", "."]
-    self.assert_cli_sys_exit(args, 0)
+    cli_main_func = staticmethod(in_toto_verify_main)
 
-    # Fail with an explicit link directory, where no links are found
-    args = ["--layout", self.layout_single_signed_path,
-        "--layout-keys", self.alice_path, "--link-dir", "bad-link-dir"]
-    self.assert_cli_sys_exit(args, 1)
+    @classmethod
+    def setUpClass(self):
+        """Creates and changes into temporary directory.
+        Copies demo files to temp dir...
+          - owner/functionary key pairs
+          - *.link metadata files
+          - layout template (not signed, no expiration date)
+          - final product
+
+        ...and dumps various layouts for different test scenarios
+        """
+
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
+        # find where the scripts directory is located.
+        scripts_directory = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "scripts"
+        )
+
+        self.set_up_test_dir()
+
+        # Copy demo files to temp dir
+        for fn in os.listdir(demo_files):
+            shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+        shutil.copytree(scripts_directory, "scripts")
+
+        # Load layout template
+        layout_template = Metadata.load("demo.layout.template")
+
+        # Store layout paths to be used in tests
+        self.layout_single_signed_path = "single-signed.layout"
+        self.layout_double_signed_path = "double-signed.layout"
+
+        # Import layout signing keys
+        alice = import_rsa_privatekey_from_file("alice")
+        bob = import_rsa_privatekey_from_file("bob")
+        self.alice_path = "alice.pub"
+        self.bob_path = "bob.pub"
+
+        # dump a single signed layout
+        layout_template.sign(alice)
+        layout_template.dump(self.layout_single_signed_path)
+        # dump a double signed layout
+        layout_template.sign(bob)
+        layout_template.dump(self.layout_double_signed_path)
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_main_required_args(self):
+        """Test in-toto-verify CLI tool with required arguments."""
+        args = [
+            "--layout",
+            self.layout_single_signed_path,
+            "--layout-keys",
+            self.alice_path,
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+
+    def test_main_wrong_args(self):
+        """Test in-toto-verify CLI tool with wrong arguments."""
+        wrong_args_list = [
+            [],
+            ["--layout", self.layout_single_signed_path],
+            ["--key", self.alice_path],
+        ]
+
+        for wrong_args in wrong_args_list:
+            self.assert_cli_sys_exit(wrong_args, 2)
+
+    def test_main_multiple_keys(self):
+        """Test in-toto-verify CLI tool with multiple keys."""
+        args = [
+            "--layout",
+            self.layout_double_signed_path,
+            "--layout-keys",
+            self.alice_path,
+            self.bob_path,
+        ]
+        self.assert_cli_sys_exit(args, 0)
+
+    def test_main_failing_bad_layout_path(self):
+        """Test in-toto-verify CLI tool with bad layout path."""
+        args = ["-l", "not-a-path-to-a-layout", "-k", self.alice_path]
+        self.assert_cli_sys_exit(args, 1)
+
+    def test_main_link_dir(self):
+        """Test in-toto-verify CLI tool with explicit link dir."""
+
+        # Use current working directory explicitly to load links
+        args = [
+            "--layout",
+            self.layout_single_signed_path,
+            "--layout-keys",
+            self.alice_path,
+            "--link-dir",
+            ".",
+        ]
+        self.assert_cli_sys_exit(args, 0)
+
+        # Fail with an explicit link directory, where no links are found
+        args = [
+            "--layout",
+            self.layout_single_signed_path,
+            "--layout-keys",
+            self.alice_path,
+            "--link-dir",
+            "bad-link-dir",
+        ]
+        self.assert_cli_sys_exit(args, 1)
 
 
 class TestInTotoVerifyToolWithDSSE(CliTestCase, TmpDirMixin):
-  """
-  Tests
-    - in_toto_verify's main() - requires sys.argv patching;
-    - in_toto_verify - calls verifylib.in_toto_verify and error logs/exits
-      in case of a raised Exception.
-
-  Uses in-toto demo supply chain link metadata files and basic layout for
-  verification:
-
-  Copies the basic layout for different test scenarios:
-    - signed layout
-    - multiple signed layout (using two project owner keys)
-  """
-  cli_main_func = staticmethod(in_toto_verify_main)
-
-
-  @classmethod
-  def setUpClass(self):
-    """Creates and changes into temporary directory.
-    Copies demo files to temp dir...
-      - owner/functionary key pairs
-      - *.link metadata files
-      - layout template (not signed, no expiration date)
-      - final product
-
-    ...and dumps various layouts for different test scenarios
     """
-
-    # Find demo files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    # Demo DSSE Metadata Files
-    demo_dsse_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_dsse_files")
-
-    # find where the scripts directory is located.
-    scripts_directory = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "scripts")
-
-    self.set_up_test_dir()
-
-    # Copy demo files to temp dir
-    for fn in os.listdir(demo_files):
-      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
-
-    for fn in os.listdir(demo_dsse_files):
-      shutil.copy(os.path.join(demo_dsse_files, fn), self.test_dir)
-
-    shutil.copytree(scripts_directory, 'scripts')
-
-    # Load layout template
-    layout_template = Metadata.load("demo.layout.template")
-
-    # Store layout paths to be used in tests
-    self.layout_single_signed_path = "single-signed.layout"
-    self.layout_double_signed_path = "double-signed.layout"
-
-    # Import layout signing keys
-    alice = import_rsa_privatekey_from_file("alice")
-    bob = import_rsa_privatekey_from_file("bob")
-    self.alice_path = "alice.pub"
-    self.bob_path = "bob.pub"
-
-    # dump a single signed layout
-    layout_template.create_signature(SSlibSigner(alice))
-    layout_template.dump(self.layout_single_signed_path)
-    # dump a double signed layout
-    layout_template.create_signature(SSlibSigner(bob))
-    layout_template.dump(self.layout_double_signed_path)
-
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-
-  def test_main_required_args(self):
-    """Test in-toto-verify CLI tool with required arguments. """
-    args = ["--layout", self.layout_single_signed_path,
-        "--layout-keys", self.alice_path]
-
-    self.assert_cli_sys_exit(args, 0)
-
-
-  def test_main_multiple_keys(self):
-    """Test in-toto-verify CLI tool with multiple keys. """
-    args = ["--layout", self.layout_double_signed_path,
-        "--layout-keys", self.alice_path, self.bob_path]
-    self.assert_cli_sys_exit(args, 0)
-
-
-  def test_main_link_dir(self):
-    """Test in-toto-verify CLI tool with explicit link dir. """
-
-    # Use current working directory explicitly to load links
-    args = ["--layout", self.layout_single_signed_path,
-        "--layout-keys", self.alice_path, "--link-dir", "."]
-    self.assert_cli_sys_exit(args, 0)
-
-    # Fail with an explicit link directory, where no links are found
-    args = ["--layout", self.layout_single_signed_path,
-        "--layout-keys", self.alice_path, "--link-dir", "bad-link-dir"]
-    self.assert_cli_sys_exit(args, 1)
-
-
-
-class TestInTotoVerifyToolMixedKeys(CliTestCase, TmpDirMixin):
-  """ Tests in-toto-verify like TestInTotoVerifyTool but with
-  both rsa and ed25519 project owner and functionary keys. """
-  cli_main_func = staticmethod(in_toto_verify_main)
-
-
-  @classmethod
-  def setUpClass(self):
-    """Creates and changes into temporary directory.
-    Copies demo files to temp dir...
-      - owner/functionary key pairs
-      - *.link metadata files
-      - layout template (not signed, no expiration date)
-      - final product
-
-    ...and dumps layout for test scenario
+    Tests
+      - in_toto_verify's main() - requires sys.argv patching;
+      - in_toto_verify - calls verifylib.in_toto_verify and error logs/exits
+        in case of a raised Exception.
+
+    Uses in-toto demo supply chain link metadata files and basic layout for
+    verification:
+
+    Copies the basic layout for different test scenarios:
+      - signed layout
+      - multiple signed layout (using two project owner keys)
     """
-    # Find demo files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    scripts_directory = os.path.join(
-      os.path.dirname(os.path.realpath(__file__)), "scripts")
-
-    self.set_up_test_dir()
-
-    # Copy demo files to temp dir
-    for fn in os.listdir(demo_files):
-      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
 
-    shutil.copytree(scripts_directory, 'scripts')
+    cli_main_func = staticmethod(in_toto_verify_main)
 
-    # Load layout template
-    layout_template = Metadata.load("demo.layout.template")
+    @classmethod
+    def setUpClass(self):
+        """Creates and changes into temporary directory.
+        Copies demo files to temp dir...
+          - owner/functionary key pairs
+          - *.link metadata files
+          - layout template (not signed, no expiration date)
+          - final product
+
+        ...and dumps various layouts for different test scenarios
+        """
+
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
+
+        # Demo DSSE Metadata Files
+        demo_dsse_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_dsse_files"
+        )
+
+        # find where the scripts directory is located.
+        scripts_directory = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "scripts"
+        )
+
+        self.set_up_test_dir()
+
+        # Copy demo files to temp dir
+        for fn in os.listdir(demo_files):
+            shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+        for fn in os.listdir(demo_dsse_files):
+            shutil.copy(os.path.join(demo_dsse_files, fn), self.test_dir)
+
+        shutil.copytree(scripts_directory, "scripts")
+
+        # Load layout template
+        layout_template = Metadata.load("demo.layout.template")
+
+        # Store layout paths to be used in tests
+        self.layout_single_signed_path = "single-signed.layout"
+        self.layout_double_signed_path = "double-signed.layout"
+
+        # Import layout signing keys
+        alice = import_rsa_privatekey_from_file("alice")
+        bob = import_rsa_privatekey_from_file("bob")
+        self.alice_path = "alice.pub"
+        self.bob_path = "bob.pub"
+
+        # dump a single signed layout
+        layout_template.create_signature(SSlibSigner(alice))
+        layout_template.dump(self.layout_single_signed_path)
+        # dump a double signed layout
+        layout_template.create_signature(SSlibSigner(bob))
+        layout_template.dump(self.layout_double_signed_path)
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_main_required_args(self):
+        """Test in-toto-verify CLI tool with required arguments."""
+        args = [
+            "--layout",
+            self.layout_single_signed_path,
+            "--layout-keys",
+            self.alice_path,
+        ]
+
+        self.assert_cli_sys_exit(args, 0)
+
+    def test_main_multiple_keys(self):
+        """Test in-toto-verify CLI tool with multiple keys."""
+        args = [
+            "--layout",
+            self.layout_double_signed_path,
+            "--layout-keys",
+            self.alice_path,
+            self.bob_path,
+        ]
+        self.assert_cli_sys_exit(args, 0)
+
+    def test_main_link_dir(self):
+        """Test in-toto-verify CLI tool with explicit link dir."""
+
+        # Use current working directory explicitly to load links
+        args = [
+            "--layout",
+            self.layout_single_signed_path,
+            "--layout-keys",
+            self.alice_path,
+            "--link-dir",
+            ".",
+        ]
+        self.assert_cli_sys_exit(args, 0)
+
+        # Fail with an explicit link directory, where no links are found
+        args = [
+            "--layout",
+            self.layout_single_signed_path,
+            "--layout-keys",
+            self.alice_path,
+            "--link-dir",
+            "bad-link-dir",
+        ]
+        self.assert_cli_sys_exit(args, 1)
 
-    # Store layout paths to be used in tests
-    self.layout_double_signed_path = "double-signed.layout"
-
-    # Import layout signing keys
-    alice = import_rsa_privatekey_from_file("alice")
-    danny = import_ed25519_privatekey_from_file("danny")
-    self.alice_path = "alice.pub"
-    self.danny_path = "danny.pub"
-
-    # dump a double signed layout
-    layout_template.sign(alice)
-    layout_template.sign(danny)
-    layout_template.dump(self.layout_double_signed_path)
 
+class TestInTotoVerifyToolMixedKeys(CliTestCase, TmpDirMixin):
+    """Tests in-toto-verify like TestInTotoVerifyTool but with
+    both rsa and ed25519 project owner and functionary keys."""
 
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
+    cli_main_func = staticmethod(in_toto_verify_main)
 
-  def test_main_multiple_keys(self):
-    """Test in-toto-verify CLI tool with multiple keys. """
-    args = ["--layout", self.layout_double_signed_path,
-       "--layout-keys", self.alice_path, self.danny_path,
-       "--key-types", "rsa", "ed25519"]
-    self.assert_cli_sys_exit(args, 0)
+    @classmethod
+    def setUpClass(self):
+        """Creates and changes into temporary directory.
+        Copies demo files to temp dir...
+          - owner/functionary key pairs
+          - *.link metadata files
+          - layout template (not signed, no expiration date)
+          - final product
+
+        ...and dumps layout for test scenario
+        """
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
+
+        scripts_directory = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "scripts"
+        )
+
+        self.set_up_test_dir()
+
+        # Copy demo files to temp dir
+        for fn in os.listdir(demo_files):
+            shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+        shutil.copytree(scripts_directory, "scripts")
+
+        # Load layout template
+        layout_template = Metadata.load("demo.layout.template")
+
+        # Store layout paths to be used in tests
+        self.layout_double_signed_path = "double-signed.layout"
+
+        # Import layout signing keys
+        alice = import_rsa_privatekey_from_file("alice")
+        danny = import_ed25519_privatekey_from_file("danny")
+        self.alice_path = "alice.pub"
+        self.danny_path = "danny.pub"
+
+        # dump a double signed layout
+        layout_template.sign(alice)
+        layout_template.sign(danny)
+        layout_template.dump(self.layout_double_signed_path)
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_main_multiple_keys(self):
+        """Test in-toto-verify CLI tool with multiple keys."""
+        args = [
+            "--layout",
+            self.layout_double_signed_path,
+            "--layout-keys",
+            self.alice_path,
+            self.danny_path,
+            "--key-types",
+            "rsa",
+            "ed25519",
+        ]
+        self.assert_cli_sys_exit(args, 0)
 
 
 class TestInTotoVerifyToolMixedKeysWithDSSE(CliTestCase, TmpDirMixin):
-  """ Tests in-toto-verify like TestInTotoVerifyTool but with
-  both rsa and ed25519 project owner and functionary keys. """
-  cli_main_func = staticmethod(in_toto_verify_main)
+    """Tests in-toto-verify like TestInTotoVerifyTool but with
+    both rsa and ed25519 project owner and functionary keys."""
 
+    cli_main_func = staticmethod(in_toto_verify_main)
 
-  @classmethod
-  def setUpClass(self):
-    """Creates and changes into temporary directory.
-    Copies demo files to temp dir...
-      - owner/functionary key pairs
-      - *.link metadata files
-      - layout template (not signed, no expiration date)
-      - final product
-
-    ...and dumps layout for test scenario
-    """
-    # Find demo files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    # Demo DSSE Metadata Files
-    demo_dsse_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_dsse_files")
-
-    # find where the scripts directory is located.
-    scripts_directory = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "scripts")
-
-    self.set_up_test_dir()
-
-    # Copy demo files to temp dir
-    for fn in os.listdir(demo_files):
-      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
-
-    for fn in os.listdir(demo_dsse_files):
-      shutil.copy(os.path.join(demo_dsse_files, fn), self.test_dir)
-
-    shutil.copytree(scripts_directory, 'scripts')
-
-    # Load layout template
-    layout_template = Metadata.load("demo.layout.template")
-
-    # Store layout paths to be used in tests
-    self.layout_double_signed_path = "double-signed.layout"
-
-    # Import layout signing keys
-    alice = import_rsa_privatekey_from_file("alice")
-    danny = import_ed25519_privatekey_from_file("danny")
-    self.alice_path = "alice.pub"
-    self.danny_path = "danny.pub"
-
-    # dump a double signed layout
-    layout_template.create_signature(SSlibSigner(alice))
-    layout_template.create_signature(SSlibSigner(danny))
-    layout_template.dump(self.layout_double_signed_path)
-
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def test_main_multiple_keys(self):
-    """Test in-toto-verify CLI tool with multiple keys. """
-    args = ["--layout", self.layout_double_signed_path,
-       "--layout-keys", self.alice_path, self.danny_path,
-       "--key-types", "rsa", "ed25519"]
-    self.assert_cli_sys_exit(args, 0)
+    @classmethod
+    def setUpClass(self):
+        """Creates and changes into temporary directory.
+        Copies demo files to temp dir...
+          - owner/functionary key pairs
+          - *.link metadata files
+          - layout template (not signed, no expiration date)
+          - final product
+
+        ...and dumps layout for test scenario
+        """
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
+
+        # Demo DSSE Metadata Files
+        demo_dsse_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_dsse_files"
+        )
+
+        # find where the scripts directory is located.
+        scripts_directory = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "scripts"
+        )
+
+        self.set_up_test_dir()
+
+        # Copy demo files to temp dir
+        for fn in os.listdir(demo_files):
+            shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+        for fn in os.listdir(demo_dsse_files):
+            shutil.copy(os.path.join(demo_dsse_files, fn), self.test_dir)
+
+        shutil.copytree(scripts_directory, "scripts")
+
+        # Load layout template
+        layout_template = Metadata.load("demo.layout.template")
+
+        # Store layout paths to be used in tests
+        self.layout_double_signed_path = "double-signed.layout"
+
+        # Import layout signing keys
+        alice = import_rsa_privatekey_from_file("alice")
+        danny = import_ed25519_privatekey_from_file("danny")
+        self.alice_path = "alice.pub"
+        self.danny_path = "danny.pub"
+
+        # dump a double signed layout
+        layout_template.create_signature(SSlibSigner(alice))
+        layout_template.create_signature(SSlibSigner(danny))
+        layout_template.dump(self.layout_double_signed_path)
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_main_multiple_keys(self):
+        """Test in-toto-verify CLI tool with multiple keys."""
+        args = [
+            "--layout",
+            self.layout_double_signed_path,
+            "--layout-keys",
+            self.alice_path,
+            self.danny_path,
+            "--key-types",
+            "rsa",
+            "ed25519",
+        ]
+        self.assert_cli_sys_exit(args, 0)
 
 
 @unittest.skipIf(not have_gpg(), "gpg not found")
 class TestInTotoVerifyToolGPG(CliTestCase, TmpDirMixin, GPGKeysMixin):
-  """ Tests in-toto-verify like TestInTotoVerifyTool but with
-  gpg project owner and functionary keys. """
-  cli_main_func = staticmethod(in_toto_verify_main)
-
-
-  @classmethod
-  def setUpClass(self):
-    """Copy test gpg rsa keyring, gpg demo metadata files and demo final
-    product to tmp test dir. """
-    # Copy gpg demo metadata files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files_gpg")
-
-    # find where the scripts directory is located.
-    scripts_directory = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "scripts")
-
-    self.set_up_test_dir()
-    self.set_up_gpg_keys()
-
-    for fn in os.listdir(demo_files):
-      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
-
-    # Change into test dir
-    shutil.copytree(scripts_directory, 'scripts')
-
-    # Sign layout template with gpg key
-    layout_template = Metadata.load("demo.layout.template")
-
-    self.layout_path = "gpg_signed.layout"
-    layout_template.sign_gpg(self.gpg_key_0C8A17, self.gnupg_home)
-    layout_template.dump(self.layout_path)
-
+    """Tests in-toto-verify like TestInTotoVerifyTool but with
+    gpg project owner and functionary keys."""
 
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
+    cli_main_func = staticmethod(in_toto_verify_main)
 
-  def test_gpg_signed_layout_with_gpg_functionary_keys(self):
-    """ Successfully test demo supply chain where the layout lists gpg keys
-    as functionary keys and is signed with a gpg key. """
-    args = ["--layout", self.layout_path,
-            "--gpg", self.gpg_key_0C8A17, "--gpg-home", self.gnupg_home]
+    @classmethod
+    def setUpClass(self):
+        """Copy test gpg rsa keyring, gpg demo metadata files and demo final
+        product to tmp test dir."""
+        # Copy gpg demo metadata files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files_gpg"
+        )
+
+        # find where the scripts directory is located.
+        scripts_directory = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "scripts"
+        )
+
+        self.set_up_test_dir()
+        self.set_up_gpg_keys()
+
+        for fn in os.listdir(demo_files):
+            shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+        # Change into test dir
+        shutil.copytree(scripts_directory, "scripts")
+
+        # Sign layout template with gpg key
+        layout_template = Metadata.load("demo.layout.template")
+
+        self.layout_path = "gpg_signed.layout"
+        layout_template.sign_gpg(self.gpg_key_0C8A17, self.gnupg_home)
+        layout_template.dump(self.layout_path)
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_gpg_signed_layout_with_gpg_functionary_keys(self):
+        """Successfully test demo supply chain where the layout lists gpg keys
+        as functionary keys and is signed with a gpg key."""
+        args = [
+            "--layout",
+            self.layout_path,
+            "--gpg",
+            self.gpg_key_0C8A17,
+            "--gpg-home",
+            self.gnupg_home,
+        ]
 
-    self.assert_cli_sys_exit(args, 0)
+        self.assert_cli_sys_exit(args, 0)
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_log.py` & `in_toto-2.0.0/tests/test_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,30 +16,31 @@
 
 <Purpose>
   Test in_toto/log.py
 
 """
 import logging
 import unittest
+
 import in_toto.log
 
 
 class TestInTotoLogger(unittest.TestCase):
-  def test_set_level_verbose_or_quiet(self):
-    """Test set level convenience method. """
-    logger = in_toto.log.InTotoLogger("test-in-toto-logger")
-
-    # Default level if verbose and quiet are false
-    logger.setLevelVerboseOrQuiet(False, False)
-    self.assertEqual(logger.level, logging.NOTSET)
-
-    # INFO if verbose is true
-    logger.setLevelVerboseOrQuiet(True, False)
-    self.assertEqual(logger.level, logging.INFO)
-
-    # CRITICAL if quiet is true
-    logger.setLevelVerboseOrQuiet(False, True)
-    self.assertEqual(logger.level, logger.QUIET)
+    def test_set_level_verbose_or_quiet(self):
+        """Test set level convenience method."""
+        logger = in_toto.log.InTotoLogger("test-in-toto-logger")
+
+        # Default level if verbose and quiet are false
+        logger.setLevelVerboseOrQuiet(False, False)
+        self.assertEqual(logger.level, logging.NOTSET)
+
+        # INFO if verbose is true
+        logger.setLevelVerboseOrQuiet(True, False)
+        self.assertEqual(logger.level, logging.INFO)
+
+        # CRITICAL if quiet is true
+        logger.setLevelVerboseOrQuiet(False, True)
+        self.assertEqual(logger.level, logger.QUIET)
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_param_substitution.py` & `in_toto-2.0.0/tests/test_param_substitution.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,189 +23,233 @@
 
 """
 
 import os
 import shutil
 import unittest
 
-import in_toto.settings
-from in_toto.models.metadata import Envelope, Metablock
-from in_toto.models.layout import  Layout
-from in_toto.verifylib import in_toto_verify, substitute_parameters
 from securesystemslib.interface import (
+    import_publickeys_from_file,
     import_rsa_privatekey_from_file,
-    import_publickeys_from_file)
+)
 from securesystemslib.signer import SSlibSigner
 
 import in_toto.exceptions
-
+import in_toto.settings
+from in_toto.models.layout import Layout
+from in_toto.models.metadata import Envelope, Metablock
+from in_toto.verifylib import in_toto_verify, substitute_parameters
 from tests.common import TmpDirMixin
 
-class Test_SubstituteArtifacts(unittest.TestCase):
-  """Test parameter substitution on artifact rules. """
-
-  def setUp(self):
-    self.layout = Layout.read({
-        "_type": "layout",
-        "inspect": [{
-          "name": "do-the-thing",
-          "expected_materials": [
-            ["MATCH", "{SOURCE_THING}", "WITH", "MATERIALS", "FROM",
-              "{SOURCE_STEP}"]
-          ],
-          "expected_products": [
-            ["CREATE", "{NEW_THING}"]
-          ]
-        }],
-        "steps": [{
-          "name": "artifacts",
-          "expected_command": [],
-          "expected_materials": [
-            ["MATCH", "{SOURCE_THING}", "WITH", "MATERIALS", "FROM",
-              "{SOURCE_STEP}"]
-          ],
-          "expected_products": [
-            ["CREATE", "{NEW_THING}"]
-          ]
-        }]
-    })
-
-  def test_substitute(self):
-    """Do a simple substitution on the expected_command field"""
-    substitute_parameters(self.layout, {"SOURCE_THING": "vim",
-      "SOURCE_STEP": "source_step", "NEW_THING": "new_thing"})
-    self.assertEqual(self.layout.steps[0].expected_materials[0][1], "vim")
-    self.assertEqual(self.layout.steps[0].expected_materials[0][5], "source_step")
-    self.assertEqual(self.layout.steps[0].expected_products[0][1], "new_thing")
-    self.assertEqual(self.layout.inspect[0].expected_materials[0][1], "vim")
-    self.assertEqual(self.layout.inspect[0].expected_materials[0][5], "source_step")
-    self.assertEqual(self.layout.inspect[0].expected_products[0][1], "new_thing")
-
 
+class Test_SubstituteArtifacts(unittest.TestCase):
+    """Test parameter substitution on artifact rules."""
 
-  def test_substitute_no_var(self):
-    """Raise an error if the parameter is not filled-in"""
-    with self.assertRaises(KeyError):
-      substitute_parameters(self.layout, {})
+    def setUp(self):
+        self.layout = Layout.read(
+            {
+                "_type": "layout",
+                "inspect": [
+                    {
+                        "name": "do-the-thing",
+                        "expected_materials": [
+                            [
+                                "MATCH",
+                                "{SOURCE_THING}",
+                                "WITH",
+                                "MATERIALS",
+                                "FROM",
+                                "{SOURCE_STEP}",
+                            ]
+                        ],
+                        "expected_products": [["CREATE", "{NEW_THING}"]],
+                    }
+                ],
+                "steps": [
+                    {
+                        "name": "artifacts",
+                        "expected_command": [],
+                        "expected_materials": [
+                            [
+                                "MATCH",
+                                "{SOURCE_THING}",
+                                "WITH",
+                                "MATERIALS",
+                                "FROM",
+                                "{SOURCE_STEP}",
+                            ]
+                        ],
+                        "expected_products": [["CREATE", "{NEW_THING}"]],
+                    }
+                ],
+            }
+        )
+
+    def test_substitute(self):
+        """Do a simple substitution on the expected_command field"""
+        substitute_parameters(
+            self.layout,
+            {
+                "SOURCE_THING": "vim",
+                "SOURCE_STEP": "source_step",
+                "NEW_THING": "new_thing",
+            },
+        )
+        self.assertEqual(self.layout.steps[0].expected_materials[0][1], "vim")
+        self.assertEqual(
+            self.layout.steps[0].expected_materials[0][5], "source_step"
+        )
+        self.assertEqual(
+            self.layout.steps[0].expected_products[0][1], "new_thing"
+        )
+        self.assertEqual(self.layout.inspect[0].expected_materials[0][1], "vim")
+        self.assertEqual(
+            self.layout.inspect[0].expected_materials[0][5], "source_step"
+        )
+        self.assertEqual(
+            self.layout.inspect[0].expected_products[0][1], "new_thing"
+        )
+
+    def test_substitute_no_var(self):
+        """Raise an error if the parameter is not filled-in"""
+        with self.assertRaises(KeyError):
+            substitute_parameters(self.layout, {})
 
 
 class Test_SubstituteRunField(unittest.TestCase):
-  """Test substitution on the run field of the layout"""
-
-  def setUp(self):
-    """
-    Create layout with dummy inspection
-    """
-
-    # Create layout with one inspection
-    self.layout = Layout.read({
-        "_type": "layout",
-        "steps": [],
-        "inspect": [{
-          "name": "run-command",
-          "run": ["{COMMAND}"],
-        }]
-      })
-
-  def test_substitute(self):
-    """Check that the substitution is performed on the run field."""
-    substitute_parameters(self.layout, {"COMMAND": "touch"})
-    self.assertEqual(self.layout.inspect[0].run[0], "touch")
+    """Test substitution on the run field of the layout"""
 
+    def setUp(self):
+        """
+        Create layout with dummy inspection
+        """
+
+        # Create layout with one inspection
+        self.layout = Layout.read(
+            {
+                "_type": "layout",
+                "steps": [],
+                "inspect": [
+                    {
+                        "name": "run-command",
+                        "run": ["{COMMAND}"],
+                    }
+                ],
+            }
+        )
+
+    def test_substitute(self):
+        """Check that the substitution is performed on the run field."""
+        substitute_parameters(self.layout, {"COMMAND": "touch"})
+        self.assertEqual(self.layout.inspect[0].run[0], "touch")
 
-  def test_inspection_fail_with_non_zero_retval(self):
-    """Check that the substitution raises TypeError if the key is missing"""
+    def test_inspection_fail_with_non_zero_retval(self):
+        """Check that the substitution raises TypeError if the key is missing"""
 
-    with self.assertRaises(KeyError):
-      substitute_parameters(self.layout, {})
+        with self.assertRaises(KeyError):
+            substitute_parameters(self.layout, {})
 
 
 class Test_SubstituteExpectedCommand(unittest.TestCase):
-  """Test verifylib.verify_command_alignment(command, expected_command)"""
-
-  def setUp(self):
-    # Create layout with one inspection
-    self.layout = Layout.read({
-        "_type": "layout",
-        "inspect": [],
-        "steps": [{
-          "name": "run-command",
-          "expected_command": ["{EDITOR}"],
-        }]})
-
-  def test_substitute(self):
-    """Do a simple substitution on the expected_command field"""
-    substitute_parameters(self.layout, {"EDITOR": "vim"})
-    self.assertEqual(self.layout.steps[0].expected_command[0], "vim")
+    """Test verifylib.verify_command_alignment(command, expected_command)"""
 
+    def setUp(self):
+        # Create layout with one inspection
+        self.layout = Layout.read(
+            {
+                "_type": "layout",
+                "inspect": [],
+                "steps": [
+                    {
+                        "name": "run-command",
+                        "expected_command": ["{EDITOR}"],
+                    }
+                ],
+            }
+        )
+
+    def test_substitute(self):
+        """Do a simple substitution on the expected_command field"""
+        substitute_parameters(self.layout, {"EDITOR": "vim"})
+        self.assertEqual(self.layout.steps[0].expected_command[0], "vim")
 
-  def test_substitute_no_var(self):
-    """Raise an error if the parameter is not filled-in"""
+    def test_substitute_no_var(self):
+        """Raise an error if the parameter is not filled-in"""
 
-    with self.assertRaises(KeyError):
-      substitute_parameters(self.layout, {"NOEDITOR": "vim"})
+        with self.assertRaises(KeyError):
+            substitute_parameters(self.layout, {"NOEDITOR": "vim"})
 
 
 class Test_SubstituteOnVerify(unittest.TestCase, TmpDirMixin):
-  """Test verifylib.verify_command_alignment(command, expected_command)"""
+    """Test verifylib.verify_command_alignment(command, expected_command)"""
 
-  @classmethod
-  def setUpClass(self):
-    # Create layout with one inspection
-    self.layout = Layout.read({
-        "_type": "layout",
-        "inspect": [],
-        "steps": [{
-          "name": "run-command",
-          "expected_command": ["{EDITOR}"],
-        }]
-      })
-
-    # Find demo files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    self.set_up_test_dir()
-
-    # Copy demo files to temp dir
-    for fn in os.listdir(demo_files):
-      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
-
-    # load alice's key
-    self.alice = import_rsa_privatekey_from_file("alice")
-    self.alice_pub_dict = import_publickeys_from_file(
-        ["alice.pub"])
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def test_substitute(self):
-    """Do a simple substitution on the expected_command field"""
-    signed_layout = Metablock(signed=self.layout)
-    signed_layout.sign(self.alice)
-
-    # we will catch a LinkNotFound error because we don't have (and don't need)
-    # the metadata.
-    with self.assertRaises(in_toto.exceptions.LinkNotFoundError):
-      in_toto_verify(signed_layout, self.alice_pub_dict,
-          substitution_parameters={"EDITOR":"vim"})
-
-    self.assertEqual(self.layout.steps[0].expected_command[0], "vim")
-
-  def test_substitute_for_envelope(self):
-    """Do a simple substitution on the expected_command field for DSSE
-    envelope."""
-    signed_layout = Envelope.from_signable(self.layout)
-    signed_layout.create_signature(SSlibSigner(self.alice))
-
-    # we will catch a LinkNotFound error because we don't have (and don't need)
-    # the metadata.
-    with self.assertRaises(in_toto.exceptions.LinkNotFoundError):
-      in_toto_verify(signed_layout, self.alice_pub_dict,
-          substitution_parameters={"EDITOR":"vim"})
+    @classmethod
+    def setUpClass(self):
+        # Create layout with one inspection
+        self.layout = Layout.read(
+            {
+                "_type": "layout",
+                "inspect": [],
+                "steps": [
+                    {
+                        "name": "run-command",
+                        "expected_command": ["{EDITOR}"],
+                    }
+                ],
+            }
+        )
+
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
+
+        self.set_up_test_dir()
+
+        # Copy demo files to temp dir
+        for fn in os.listdir(demo_files):
+            shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+        # load alice's key
+        self.alice = import_rsa_privatekey_from_file("alice")
+        self.alice_pub_dict = import_publickeys_from_file(["alice.pub"])
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_substitute(self):
+        """Do a simple substitution on the expected_command field"""
+        signed_layout = Metablock(signed=self.layout)
+        signed_layout.sign(self.alice)
+
+        # we will catch a LinkNotFound error because we don't have (and don't need)
+        # the metadata.
+        with self.assertRaises(in_toto.exceptions.LinkNotFoundError):
+            in_toto_verify(
+                signed_layout,
+                self.alice_pub_dict,
+                substitution_parameters={"EDITOR": "vim"},
+            )
+
+        self.assertEqual(self.layout.steps[0].expected_command[0], "vim")
+
+    def test_substitute_for_envelope(self):
+        """Do a simple substitution on the expected_command field for DSSE
+        envelope."""
+        signed_layout = Envelope.from_signable(self.layout)
+        signed_layout.create_signature(SSlibSigner(self.alice))
+
+        # we will catch a LinkNotFound error because we don't have (and don't need)
+        # the metadata.
+        with self.assertRaises(in_toto.exceptions.LinkNotFoundError):
+            in_toto_verify(
+                signed_layout,
+                self.alice_pub_dict,
+                substitution_parameters={"EDITOR": "vim"},
+            )
 
-    self.assertEqual(self.layout.steps[0].expected_command[0], "vim")
+        self.assertEqual(self.layout.steps[0].expected_command[0], "vim")
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_rulelib.py` & `in_toto-2.0.0/tests/test_rulelib.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,270 +18,407 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Test artifact rule packing and unpacking.
 
 """
 import unittest
-from in_toto.rulelib import (unpack_rule, pack_rule, pack_rule_data,
-    pack_create_rule, pack_delete_rule, pack_modify_rule, pack_allow_rule,
-    pack_disallow_rule, pack_require_rule)
+
 import securesystemslib.exceptions
 
+from in_toto.rulelib import (
+    pack_allow_rule,
+    pack_create_rule,
+    pack_delete_rule,
+    pack_disallow_rule,
+    pack_modify_rule,
+    pack_require_rule,
+    pack_rule,
+    pack_rule_data,
+    unpack_rule,
+)
+
 
 class TestArtifactRuleUnpack(unittest.TestCase):
-  """Test artifact rule unpacker/syntax checker. """
+    """Test artifact rule unpacker/syntax checker."""
 
-  def test_unpack_rule_not_list(self):
-    """Test rule syntax error, not a list. """
+    def test_unpack_rule_not_list(self):
+        """Test rule syntax error, not a list."""
 
-    rule = "CREATE stuff"
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-  def test_unpack_rule_not_enough_keywords(self):
-    """Test rule syntax error, too little arguments. """
-    rule = ["DELETE"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-  def test_unpack_rule_unknown_rule_type(self):
-    """Test generic rule syntax error, too many arguments. """
-    rule = ["SUBVERT", "foo"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-  def test_unpack_rule_pattern_not_string(self):
-    """Test rule syntax error, pattern not a string. """
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      rule = ["CREATE", {"abc"}]
-      unpack_rule(rule)
-
-  def test_unpack_generic_rule_too_long(self):
-    """Test generic rule syntax error, too many arguments. """
-    rule = ["CREATE", "foo", "pleaze!!"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-  def test_unpack_and_pack_generic_rule(self):
-    """Test generic rule proper packing and unpacking. """
-    rule = ["CREATE", "foo"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 2)
-    self.assertEqual(rule_data["rule_type"], "create")
-    self.assertEqual(rule_data["pattern"], "foo")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_create_rule("foo"))
-
-
-    rule = ["DELETE", "foo"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 2)
-    self.assertEqual(rule_data["rule_type"], "delete")
-    self.assertEqual(rule_data["pattern"], "foo")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_delete_rule("foo"))
-
-
-    rule = ["MODIFY", "foo"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 2)
-    self.assertEqual(rule_data["rule_type"], "modify")
-    self.assertEqual(rule_data["pattern"], "foo")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_modify_rule("foo"))
-
-
-    rule = ["ALLOW", "foo"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 2)
-    self.assertEqual(rule_data["rule_type"], "allow")
-    self.assertEqual(rule_data["pattern"], "foo")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_allow_rule("foo"))
-
-
-    rule = ["DISALLOW", "foo"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 2)
-    self.assertEqual(rule_data["rule_type"], "disallow")
-    self.assertEqual(rule_data["pattern"], "foo")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_disallow_rule("foo"))
-
-    rule = ["REQUIRE", "foo"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 2)
-    self.assertEqual(rule_data["rule_type"], "require")
-    self.assertEqual(rule_data["pattern"], "foo")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_require_rule("foo"))
-
-
-  def test_unpack_and_pack_match_rule(self):
-    """Check match rule proper packing and unpacking. """
-
-    rule = ["MATCH", "foo", "IN", "source-path", "WITH",
-        "PRODUCTS", "IN", "dest-path", "FROM", "step-name"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 6)
-    self.assertEqual(rule_data["rule_type"], "match")
-    self.assertEqual(rule_data["pattern"], "foo")
-    self.assertEqual(rule_data["source_prefix"], "source-path")
-    self.assertEqual(rule_data["dest_prefix"], "dest-path")
-    self.assertEqual(rule_data["dest_type"], "products")
-    self.assertEqual(rule_data["dest_name"], "step-name")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_rule("MATCH", "foo",
-        source_prefix="source-path", dest_type="PRODUCTS",
-        dest_prefix="dest-path", dest_name="step-name"))
-
-
-    rule = ["MATCH", "foo", "IN", "source-path", "WITH",
-        "MATERIALS", "FROM", "step-name"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 6)
-    self.assertEqual(rule_data["rule_type"], "match")
-    self.assertEqual(rule_data["pattern"], "foo")
-    self.assertEqual(rule_data["source_prefix"], "source-path")
-    self.assertEqual(rule_data["dest_prefix"], "")
-    self.assertEqual(rule_data["dest_type"], "materials")
-    self.assertEqual(rule_data["dest_name"], "step-name")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_rule("MATCH", "foo",
-        source_prefix="source-path", dest_type="MATERIALS",
-        dest_name="step-name"))
-
-
-    rule = ["MATCH", "foo", "WITH",
-        "PRODUCTS", "IN", "dest-path", "FROM", "step-name"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 6)
-    self.assertEqual(rule_data["rule_type"], "match")
-    self.assertEqual(rule_data["pattern"], "foo")
-    self.assertEqual(rule_data["source_prefix"], "")
-    self.assertEqual(rule_data["dest_prefix"], "dest-path")
-    self.assertEqual(rule_data["dest_type"], "products")
-    self.assertEqual(rule_data["dest_name"], "step-name")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_rule("MATCH", "foo",
-        dest_type="PRODUCTS", dest_prefix="dest-path", dest_name="step-name"))
-
-    rule = ["MATCH", "foo", "WITH", "PRODUCTS", "FROM", "step-name"]
-    rule_data = unpack_rule(rule)
-    self.assertEqual(len(list(rule_data.keys())), 6)
-    self.assertEqual(rule_data["rule_type"], "match")
-    self.assertEqual(rule_data["pattern"], "foo")
-    self.assertEqual(rule_data["source_prefix"], "")
-    self.assertEqual(rule_data["dest_prefix"], "")
-    self.assertEqual(rule_data["dest_type"], "products")
-    self.assertEqual(rule_data["dest_name"], "step-name")
-
-    self.assertEqual(rule, pack_rule_data(rule_data))
-    self.assertEqual(rule, pack_rule("MATCH", "foo",
-        dest_type="PRODUCTS", dest_name="step-name"))
-
-  def test_pack_rule_wrong_types(self):
-    """Test argument validation for pack_rule. """
-    # pattern must be a string
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      pack_rule("match", None)
-
-    # rule_type must be a string...
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      pack_rule(1, "foo")
-
-    # ... and one of the allowed rule types
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      pack_rule("not-a-rule-type", "foo")
-
-    # For match rules a dest_type must be passed ...
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      pack_rule("match", "foo", dest_name="step-name")
-
-    # ... and be one of materials or products
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      pack_rule("match", "foo", dest_type="not-a-dest-type",
-          dest_name="step-name")
-
-    # For match rules dest_name must be a string ...
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      pack_rule("match", "foo", dest_type="materials",
-          dest_name=1)
-
-    # ... and non-empty
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      pack_rule("match", "foo", dest_type="materials",
-          dest_name="")
-
-    # For match rules, if a source_prefix is passed it must be a string
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      pack_rule("match", "foo", source_prefix=1, dest_type="products",
-          dest_prefix="dest-path", dest_name="step-name")
-
-   # For match rules, if a dest_prefix is passed it must be a string
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      pack_rule("match", "foo", dest_type="products",
-          dest_prefix=["not-a-string"], dest_name="step-name")
-
-
-  def test_unpack_match_rule_wrong_length(self):
-    """Check match rule syntax error, too few or many arguments. """
-
-    rule = ["MATCH", "foo", "WITH", "PRODUCTS", "FROM"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-    rule = ["MATCH", "foo", "WITH", "PRODUCTS", "FROM", "step-name", "really?"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-    rule = ["MATCH", "foo", "IN", "source-path", "WITH",
-        "PRODUCTS", "IN", "dest-path", "FROM", "step-name", "YES, we can!"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-  def test_unpack_match_rule_wrong_types(self):
-    """Check match rule syntax error, wrong data type in variable arguments. """
-    # pattern must be string
-    rule = ["MATCH", ["abc"], "IN", "source-path", "WITH",
-        "PRODUCTS", "IN", "dest-path", "FROM", "step-name"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-    # source path must be a string
-    rule = ["MATCH", "foo", "IN", {"abc": "def"}, "WITH",
-        "PRODUCTS", "IN", "dest-path", "FROM", "step-name"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-    # dest-path must be a string
-    rule = ["MATCH", "foo", "IN", "source-path", "WITH",
-        "PRODUCTS", "IN", 123, "FROM", "step-name"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-    # step-name must be a string
-    rule = ["MATCH", "foo", "IN", "source-path", "WITH",
-        "PRODUCTS", "IN", "dest-path", "FROM", ("456",)]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
-
-  def test_unpack_match_rule_wrong_destination_type(self):
-    """Check match rule syntax error, wrong destination type. """
-    rule = ["MATCH", "foo", "IN", "source-path", "WITH",
-        "PONIES", "IN", "dest-path", "FROM", "step-name"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      unpack_rule(rule)
+        rule = "CREATE stuff"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+    def test_unpack_rule_not_enough_keywords(self):
+        """Test rule syntax error, too little arguments."""
+        rule = ["DELETE"]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+    def test_unpack_rule_unknown_rule_type(self):
+        """Test generic rule syntax error, too many arguments."""
+        rule = ["SUBVERT", "foo"]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+    def test_unpack_rule_pattern_not_string(self):
+        """Test rule syntax error, pattern not a string."""
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            rule = ["CREATE", {"abc"}]
+            unpack_rule(rule)
+
+    def test_unpack_generic_rule_too_long(self):
+        """Test generic rule syntax error, too many arguments."""
+        rule = ["CREATE", "foo", "pleaze!!"]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+    def test_unpack_and_pack_generic_rule(self):
+        """Test generic rule proper packing and unpacking."""
+        rule = ["CREATE", "foo"]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 2)
+        self.assertEqual(rule_data["rule_type"], "create")
+        self.assertEqual(rule_data["pattern"], "foo")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(rule, pack_create_rule("foo"))
+
+        rule = ["DELETE", "foo"]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 2)
+        self.assertEqual(rule_data["rule_type"], "delete")
+        self.assertEqual(rule_data["pattern"], "foo")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(rule, pack_delete_rule("foo"))
+
+        rule = ["MODIFY", "foo"]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 2)
+        self.assertEqual(rule_data["rule_type"], "modify")
+        self.assertEqual(rule_data["pattern"], "foo")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(rule, pack_modify_rule("foo"))
+
+        rule = ["ALLOW", "foo"]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 2)
+        self.assertEqual(rule_data["rule_type"], "allow")
+        self.assertEqual(rule_data["pattern"], "foo")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(rule, pack_allow_rule("foo"))
+
+        rule = ["DISALLOW", "foo"]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 2)
+        self.assertEqual(rule_data["rule_type"], "disallow")
+        self.assertEqual(rule_data["pattern"], "foo")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(rule, pack_disallow_rule("foo"))
+
+        rule = ["REQUIRE", "foo"]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 2)
+        self.assertEqual(rule_data["rule_type"], "require")
+        self.assertEqual(rule_data["pattern"], "foo")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(rule, pack_require_rule("foo"))
+
+    def test_unpack_and_pack_match_rule(self):
+        """Check match rule proper packing and unpacking."""
+
+        rule = [
+            "MATCH",
+            "foo",
+            "IN",
+            "source-path",
+            "WITH",
+            "PRODUCTS",
+            "IN",
+            "dest-path",
+            "FROM",
+            "step-name",
+        ]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 6)
+        self.assertEqual(rule_data["rule_type"], "match")
+        self.assertEqual(rule_data["pattern"], "foo")
+        self.assertEqual(rule_data["source_prefix"], "source-path")
+        self.assertEqual(rule_data["dest_prefix"], "dest-path")
+        self.assertEqual(rule_data["dest_type"], "products")
+        self.assertEqual(rule_data["dest_name"], "step-name")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(
+            rule,
+            pack_rule(
+                "MATCH",
+                "foo",
+                source_prefix="source-path",
+                dest_type="PRODUCTS",
+                dest_prefix="dest-path",
+                dest_name="step-name",
+            ),
+        )
+
+        rule = [
+            "MATCH",
+            "foo",
+            "IN",
+            "source-path",
+            "WITH",
+            "MATERIALS",
+            "FROM",
+            "step-name",
+        ]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 6)
+        self.assertEqual(rule_data["rule_type"], "match")
+        self.assertEqual(rule_data["pattern"], "foo")
+        self.assertEqual(rule_data["source_prefix"], "source-path")
+        self.assertEqual(rule_data["dest_prefix"], "")
+        self.assertEqual(rule_data["dest_type"], "materials")
+        self.assertEqual(rule_data["dest_name"], "step-name")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(
+            rule,
+            pack_rule(
+                "MATCH",
+                "foo",
+                source_prefix="source-path",
+                dest_type="MATERIALS",
+                dest_name="step-name",
+            ),
+        )
+
+        rule = [
+            "MATCH",
+            "foo",
+            "WITH",
+            "PRODUCTS",
+            "IN",
+            "dest-path",
+            "FROM",
+            "step-name",
+        ]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 6)
+        self.assertEqual(rule_data["rule_type"], "match")
+        self.assertEqual(rule_data["pattern"], "foo")
+        self.assertEqual(rule_data["source_prefix"], "")
+        self.assertEqual(rule_data["dest_prefix"], "dest-path")
+        self.assertEqual(rule_data["dest_type"], "products")
+        self.assertEqual(rule_data["dest_name"], "step-name")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(
+            rule,
+            pack_rule(
+                "MATCH",
+                "foo",
+                dest_type="PRODUCTS",
+                dest_prefix="dest-path",
+                dest_name="step-name",
+            ),
+        )
+
+        rule = ["MATCH", "foo", "WITH", "PRODUCTS", "FROM", "step-name"]
+        rule_data = unpack_rule(rule)
+        self.assertEqual(len(list(rule_data.keys())), 6)
+        self.assertEqual(rule_data["rule_type"], "match")
+        self.assertEqual(rule_data["pattern"], "foo")
+        self.assertEqual(rule_data["source_prefix"], "")
+        self.assertEqual(rule_data["dest_prefix"], "")
+        self.assertEqual(rule_data["dest_type"], "products")
+        self.assertEqual(rule_data["dest_name"], "step-name")
+
+        self.assertEqual(rule, pack_rule_data(rule_data))
+        self.assertEqual(
+            rule,
+            pack_rule(
+                "MATCH", "foo", dest_type="PRODUCTS", dest_name="step-name"
+            ),
+        )
+
+    def test_pack_rule_wrong_types(self):
+        """Test argument validation for pack_rule."""
+        # pattern must be a string
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            pack_rule("match", None)
+
+        # rule_type must be a string...
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            pack_rule(1, "foo")
+
+        # ... and one of the allowed rule types
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            pack_rule("not-a-rule-type", "foo")
+
+        # For match rules a dest_type must be passed ...
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            pack_rule("match", "foo", dest_name="step-name")
+
+        # ... and be one of materials or products
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            pack_rule(
+                "match",
+                "foo",
+                dest_type="not-a-dest-type",
+                dest_name="step-name",
+            )
+
+        # For match rules dest_name must be a string ...
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            pack_rule("match", "foo", dest_type="materials", dest_name=1)
+
+        # ... and non-empty
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            pack_rule("match", "foo", dest_type="materials", dest_name="")
+
+        # For match rules, if a source_prefix is passed it must be a string
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            pack_rule(
+                "match",
+                "foo",
+                source_prefix=1,
+                dest_type="products",
+                dest_prefix="dest-path",
+                dest_name="step-name",
+            )
+
+        # For match rules, if a dest_prefix is passed it must be a string
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            pack_rule(
+                "match",
+                "foo",
+                dest_type="products",
+                dest_prefix=["not-a-string"],
+                dest_name="step-name",
+            )
+
+    def test_unpack_match_rule_wrong_length(self):
+        """Check match rule syntax error, too few or many arguments."""
+
+        rule = ["MATCH", "foo", "WITH", "PRODUCTS", "FROM"]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+        rule = [
+            "MATCH",
+            "foo",
+            "WITH",
+            "PRODUCTS",
+            "FROM",
+            "step-name",
+            "really?",
+        ]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+        rule = [
+            "MATCH",
+            "foo",
+            "IN",
+            "source-path",
+            "WITH",
+            "PRODUCTS",
+            "IN",
+            "dest-path",
+            "FROM",
+            "step-name",
+            "YES, we can!",
+        ]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+    def test_unpack_match_rule_wrong_types(self):
+        """Check match rule syntax error, wrong data type in variable arguments."""
+        # pattern must be string
+        rule = [
+            "MATCH",
+            ["abc"],
+            "IN",
+            "source-path",
+            "WITH",
+            "PRODUCTS",
+            "IN",
+            "dest-path",
+            "FROM",
+            "step-name",
+        ]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+        # source path must be a string
+        rule = [
+            "MATCH",
+            "foo",
+            "IN",
+            {"abc": "def"},
+            "WITH",
+            "PRODUCTS",
+            "IN",
+            "dest-path",
+            "FROM",
+            "step-name",
+        ]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+        # dest-path must be a string
+        rule = [
+            "MATCH",
+            "foo",
+            "IN",
+            "source-path",
+            "WITH",
+            "PRODUCTS",
+            "IN",
+            123,
+            "FROM",
+            "step-name",
+        ]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+        # step-name must be a string
+        rule = [
+            "MATCH",
+            "foo",
+            "IN",
+            "source-path",
+            "WITH",
+            "PRODUCTS",
+            "IN",
+            "dest-path",
+            "FROM",
+            ("456",),
+        ]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
+
+    def test_unpack_match_rule_wrong_destination_type(self):
+        """Check match rule syntax error, wrong destination type."""
+        rule = [
+            "MATCH",
+            "foo",
+            "IN",
+            "source-path",
+            "WITH",
+            "PONIES",
+            "IN",
+            "dest-path",
+            "FROM",
+            "step-name",
+        ]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            unpack_rule(rule)
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_runlib.py` & `in_toto-2.0.0/tests/test_runlib.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-#coding=utf-8
+# coding=utf-8
 
 # Copyright New York University and the in-toto contributors
 # SPDX-License-Identifier: Apache-2.0
 
 """
 <Program Name>
   test_runlib.py
@@ -18,1029 +18,1388 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Test runlib functions.
 
 """
 import os
-import unittest
 import shutil
-import tempfile
-import sys
 import stat
 import subprocess
+import sys
+import tempfile
+import unittest
+from pathlib import Path
 
-import in_toto.settings
-import in_toto.exceptions
-from in_toto.models.metadata import Envelope, Metablock
-from in_toto.exceptions import SignatureVerificationError
-from in_toto.runlib import (in_toto_run, in_toto_record_start,
-    in_toto_record_stop, record_artifacts_as_dict, _apply_exclude_patterns,
-    _hash_artifact, _subprocess_run_duplicate_streams)
+import securesystemslib.exceptions
+import securesystemslib.formats
 from securesystemslib.interface import (
     generate_and_write_unencrypted_rsa_keypair,
     import_rsa_privatekey_from_file,
-    import_rsa_publickey_from_file)
-from in_toto.models.link import UNFINISHED_FILENAME_FORMAT, FILENAME_FORMAT
-
-import securesystemslib.formats
-import securesystemslib.exceptions
+    import_rsa_publickey_from_file,
+)
 
+import in_toto.exceptions
+import in_toto.settings
+from in_toto.exceptions import SignatureVerificationError
+from in_toto.models.link import (
+    FILENAME_FORMAT,
+    UNFINISHED_FILENAME_FORMAT,
+    Link,
+)
+from in_toto.models.metadata import Envelope, Metablock
+from in_toto.resolver import FileResolver
+from in_toto.runlib import (
+    _subprocess_run_duplicate_streams,
+    in_toto_match_products,
+    in_toto_record_start,
+    in_toto_record_stop,
+    in_toto_run,
+    record_artifacts_as_dict,
+)
 from tests.common import TmpDirMixin
-from pathlib import Path
 
 
-class Test_ApplyExcludePatterns(unittest.TestCase):
-  """Test _apply_exclude_patterns(names, exclude_patterns) """
+def _apply_exclude_patterns(names, patterns):
+    """Temporary bridge from old `runlib._apply_exclude_patterns` with new
+    `FileResolver._exclude`.
 
-  def test_apply_exclude_explict(self):
-    names = ["foo", "bar", "baz"]
-    patterns = ["foo", "bar"]
-    expected = ["baz"]
-    result = _apply_exclude_patterns(names, patterns)
-    self.assertListEqual(sorted(result), sorted(expected))
-
-  def test_apply_exclude_all(self):
-    names = ["foo", "bar", "baz"]
-    patterns = ["*"]
-    expected = []
-    result = _apply_exclude_patterns(names, patterns)
-    self.assertListEqual(sorted(result), sorted(expected))
-
-  def test_apply_exclude_multiple_star(self):
-    names = ["foo", "bar", "baz"]
-    patterns = ["*a*"]
-    expected = ["foo"]
-    result = _apply_exclude_patterns(names, patterns)
-    self.assertListEqual(result, expected)
-
-  def test_apply_exclude_question_mark(self):
-    names = ["foo", "bazfoo", "barfoo"]
-    patterns = ["ba?foo"]
-    expected = ["foo"]
-    result = _apply_exclude_patterns(names, patterns)
-    self.assertListEqual(result, expected)
-
-  def test_apply_exclude_seq(self):
-    names = ["baxfoo", "bazfoo", "barfoo"]
-    patterns = ["ba[xz]foo"]
-    expected = ["barfoo"]
-    result = _apply_exclude_patterns(names, patterns)
-    self.assertListEqual(result, expected)
-
-  def test_apply_exclude_neg_seq(self):
-    names = ["baxfoo", "bazfoo", "barfoo"]
-    patterns = ["ba[!r]foo"]
-    expected = ["barfoo"]
-    result = _apply_exclude_patterns(names, patterns)
-    self.assertListEqual(result, expected)
+     TODO: Replace tist once resolver interface evolves
+    """
+    return [
+        n
+        for n in names
+        if not FileResolver(exclude_patterns=patterns)._exclude(n)
+    ]
 
 
-class TestRecordArtifactsAsDict(unittest.TestCase, TmpDirMixin):
-  """Test record_artifacts_as_dict(artifacts). """
+class Test_ApplyExcludePatterns(unittest.TestCase):
+    """Test _apply_exclude_patterns(names, exclude_patterns)"""
 
-  @classmethod
-  def setUpClass(self):
-    """Create and change into temp test directory with dummy artifacts.
-    |-- bar
-    |-- foo
-    `-- subdir
-        |-- foosub1
-        |-- foosub2
-        `-- subsubdir
-            `-- foosubsub
-    """
+    def test_apply_exclude_explict(self):
+        names = ["foo", "bar", "baz"]
+        patterns = ["foo", "bar"]
+        expected = ["baz"]
+        result = _apply_exclude_patterns(names, patterns)
+        self.assertListEqual(sorted(result), sorted(expected))
+
+    def test_apply_exclude_all(self):
+        names = ["foo", "bar", "baz"]
+        patterns = ["*"]
+        expected = []
+        result = _apply_exclude_patterns(names, patterns)
+        self.assertListEqual(sorted(result), sorted(expected))
+
+    def test_apply_exclude_multiple_star(self):
+        names = ["foo", "bar", "baz"]
+        patterns = ["*a*"]
+        expected = ["foo"]
+        result = _apply_exclude_patterns(names, patterns)
+        self.assertListEqual(result, expected)
+
+    def test_apply_exclude_question_mark(self):
+        names = ["foo", "bazfoo", "barfoo"]
+        patterns = ["ba?foo"]
+        expected = ["foo"]
+        result = _apply_exclude_patterns(names, patterns)
+        self.assertListEqual(result, expected)
+
+    def test_apply_exclude_seq(self):
+        names = ["baxfoo", "bazfoo", "barfoo"]
+        patterns = ["ba[xz]foo"]
+        expected = ["barfoo"]
+        result = _apply_exclude_patterns(names, patterns)
+        self.assertListEqual(result, expected)
+
+    def test_apply_exclude_neg_seq(self):
+        names = ["baxfoo", "bazfoo", "barfoo"]
+        patterns = ["ba[!r]foo"]
+        expected = ["barfoo"]
+        result = _apply_exclude_patterns(names, patterns)
+        self.assertListEqual(result, expected)
 
-    # Backup and clear user set exclude patterns and base path
-    self.artifact_exclude_orig = in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS
-    self.artifact_base_path_orig = in_toto.settings.ARTIFACT_BASE_PATH
-    in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = []
-    in_toto.settings.ARTIFACT_BASE_PATH = None
-
-    self.set_up_test_dir()
-
-    # Create files on 3 levels
-    os.mkdir("subdir")
-    os.mkdir("subdir/subsubdir")
-
-    self.full_file_path_list = ["foo", "bar", "#esc!", "subdir/foosub1",
-        "subdir/foosub2", "subdir/subsubdir/foosubsub"]
-
-    for path in self.full_file_path_list:
-      with open(path, "w", encoding="utf8") as fp:
-        fp.write(path)
-
-
-  @classmethod
-  def tearDownClass(self):
-    """Change back to working dir, remove temp directory, restore settings. """
-    self.tear_down_test_dir()
-    in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = self.artifact_exclude_orig
-    in_toto.settings.ARTIFACT_BASE_PATH = self.artifact_base_path_orig
-
-  def tearDown(self):
-    """Clear the ARTIFACT_EXLCUDES after every test. """
-    in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = []
-    in_toto.settings.ARTIFACT_BASE_PATH = None
-
-  def test_bad_base_path_setting(self):
-    """Raise exception with bogus base path settings. """
-    for base_path in ["path/does/not/exist", 12345, True]:
-      in_toto.settings.ARTIFACT_BASE_PATH = base_path
-      with self.assertRaises(ValueError):
-        record_artifacts_as_dict(["."])
-      in_toto.settings.ARTIFACT_BASE_PATH = None
-
-      with self.assertRaises(ValueError):
-        record_artifacts_as_dict(["."], base_path=base_path)
-
-
-  def test_base_path_is_child_dir(self):
-    """Test path of recorded artifacts and cd back with child as base."""
-    base_path = "subdir"
-    expected_artifacts = sorted(["foosub1", "foosub2", "subsubdir/foosubsub"])
-
-    in_toto.settings.ARTIFACT_BASE_PATH = base_path
-    artifacts_dict = record_artifacts_as_dict(["."])
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-        expected_artifacts)
-    in_toto.settings.ARTIFACT_BASE_PATH = None
-
-    artifacts_dict = record_artifacts_as_dict(["."], base_path=base_path)
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-        expected_artifacts)
-
-
-  def test_base_path_is_parent_dir(self):
-    """Test path of recorded artifacts and cd back with parent as base. """
-    base_path = ".."
-    expected_artifacts = sorted(["foosub1", "foosub2", "subsubdir/foosubsub"])
-    os.chdir("subdir/subsubdir")
-
-    in_toto.settings.ARTIFACT_BASE_PATH = base_path
-    artifacts_dict = record_artifacts_as_dict(["."])
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-        expected_artifacts)
-    in_toto.settings.ARTIFACT_BASE_PATH = None
-
-    artifacts_dict = record_artifacts_as_dict(["."], base_path=base_path)
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-        expected_artifacts)
-
-    os.chdir(self.test_dir)
-
-
-  def test_lstrip_paths_valid_prefix_directory(self):
-    lstrip_paths = ["subdir/subsubdir/"]
-    expected_artifacts = sorted(["#esc!", "bar", "foo", "subdir/foosub1",
-        "subdir/foosub2", "foosubsub"])
-    artifacts_dict = record_artifacts_as_dict(["."],
-        lstrip_paths=lstrip_paths)
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-        expected_artifacts)
-
-
-  def test_lstrip_paths_substring_prefix_directory(self):
-    lstrip_paths = ["subdir/subsubdir/", "subdir/"]
-    with self.assertRaises(in_toto.exceptions.PrefixError):
-      record_artifacts_as_dict(["."], lstrip_paths=lstrip_paths)
-
-
-  def test_lstrip_paths_non_unique_key(self):
-    os.mkdir("subdir_new")
-    path = "subdir_new/foosub1"
-    shutil.copy("subdir/foosub1", path)
-    lstrip_paths = ["subdir/", "subdir_new/"]
-    with self.assertRaises(in_toto.exceptions.PrefixError):
-      record_artifacts_as_dict(["."], lstrip_paths=lstrip_paths)
-    os.remove(path)
-    os.rmdir("subdir_new")
-
-
-  def test_lstrip_paths_invalid_prefix_directory(self):
-    lstrip_paths = ["not/a/directory/"]
-    expected_artifacts = sorted(["#esc!", "bar", "foo", "subdir/foosub1",
-                                 "subdir/foosub2", "subdir/subsubdir/foosubsub"])
-    artifacts_dict = record_artifacts_as_dict(["."],
-        lstrip_paths=lstrip_paths)
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-                         expected_artifacts)
-
-
-  def test_lstrip_paths_valid_prefix_file(self):
-    lstrip_paths = ["subdir/subsubdir/"]
-    expected_artifacts = sorted(["foosubsub"])
-    artifacts_dict = record_artifacts_as_dict(["./subdir/subsubdir/foosubsub"],
-        lstrip_paths=lstrip_paths)
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-        expected_artifacts)
-
-
-  def test_lstrip_paths_non_unique_key_file(self):
-    os.mkdir("subdir/subsubdir_new")
-    path = "subdir/subsubdir_new/foosubsub"
-    shutil.copy("subdir/subsubdir/foosubsub", path)
-    lstrip_paths = ["subdir/subsubdir/", "subdir/subsubdir_new/"]
-    with self.assertRaises(in_toto.exceptions.PrefixError):
-      record_artifacts_as_dict(["subdir/subsubdir/foosubsub",
-          "subdir/subsubdir_new/foosubsub"], lstrip_paths=lstrip_paths)
-    os.remove(path)
-    os.rmdir("subdir/subsubdir_new")
-
-
-  def test_lstrip_paths_valid_unicode_prefix_file(self):
-    # Try to create a file with unicode character
-    try:
-      os.mkdir("ಠ")
-      path = "ಠ/foo"
-      shutil.copy("foo", path)
-
-      # Attempt to left strip the path now that the file has been created
-      lstrip_paths = ["ಠ/"]
-      expected_artifacts = sorted(["foo"])
-      artifacts_dict = record_artifacts_as_dict(["./ಠ/"],
-          lstrip_paths=lstrip_paths)
-      self.assertListEqual(sorted(list(artifacts_dict.keys())),
-          expected_artifacts)
-      os.remove(path)
-      os.rmdir("ಠ")
-    except OSError:
-      # OS doesn't support unicode explicit files
-      pass
-
-
-  def test_empty_artifacts_list_record_nothing(self):
-    """Empty list passed. Return empty dict. """
-    self.assertDictEqual(record_artifacts_as_dict([]), {})
-
-  def test_not_existing_artifacts_in_list_record_nothing(self):
-    """List with not existing artifact passed. Return empty dict. """
-    self.assertDictEqual(record_artifacts_as_dict(["baz"]), {})
-
-  def test_record_dot_check_files_hash_dict_schema(self):
-    """Traverse dir and subdirs. Record three files. """
-    artifacts_dict = record_artifacts_as_dict(["."])
-
-    for val in list(artifacts_dict.values()):
-      securesystemslib.formats.HASHDICT_SCHEMA.check_match(val)
-
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-      sorted(self.full_file_path_list))
-
-  @staticmethod
-  def _raise_win_dev_mode_error():
-    """If the platform is Windows, raises an error that asks the user if
-    developer mode is activated."""
-    if os.name == "nt":
-      raise IOError("Developer mode is required to work with symlinks on "
-          "Windows. Is it enabled?")
-
-
-  @unittest.skipIf("symlink" not in os.__dict__, "symlink is not supported in this platform")
-  def test_record_symlinked_files(self):
-    """Symlinked files are always recorded. """
-    # Symlinked **files** are always recorded ...
-    link_pairs = [
-      ("foo", "foo_link"),
-      ("subdir/foosub1", "subdir/foosub2_link"),
-      ("subdir/subsubdir/foosubsub", "subdir/subsubdir/foosubsub_link")
-    ]
 
-    # Create links
-    for pair in link_pairs:
-      # We only use the basename of the file (source) as it is on the same
-      # level as the link (target)
-      try:
-        os.symlink(os.path.basename(pair[0]), pair[1])
-      except IOError:
-        TestRecordArtifactsAsDict._raise_win_dev_mode_error()
-        raise
-
-    # Record files and linked files
-    # follow_symlink_dirs does not make a difference as it only concerns linked dirs
-    for follow_symlink_dirs in [True, False]:
-      artifacts_dict = record_artifacts_as_dict(["."],
-          follow_symlink_dirs=follow_symlink_dirs)
-
-      # Test that everything was recorded ...
-      self.assertListEqual(sorted(list(artifacts_dict.keys())),
-          sorted(self.full_file_path_list + [pair[1] for pair in link_pairs]))
-
-      # ... and the hashes of each link/file pair match
-      for pair in link_pairs:
-        self.assertDictEqual(artifacts_dict[pair[0]], artifacts_dict[pair[1]])
-
-    for pair in link_pairs:
-      os.unlink(pair[1])
-
-
-  @unittest.skipIf("symlink" not in os.__dict__, "symlink is not supported in this platform")
-  def test_record_without_dead_symlinks(self):
-    """Dead symlinks are never recorded. """
-
-    # Dead symlinks are never recorded ...
-    links = [
-      "foo_link",
-      "subdir/foosub2_link",
-      "subdir/subsubdir/foosubsub_link"
-    ]
+class TestRecordArtifactsAsDict(unittest.TestCase, TmpDirMixin):
+    """Test record_artifacts_as_dict(artifacts)."""
 
-    # Create dead links
-    for link in links:
-      try:
-        os.symlink("does/not/exist", link)
-      except IOError:
-        TestRecordArtifactsAsDict._raise_win_dev_mode_error()
-        raise
-
-    # Record files without dead links
-    # follow_symlink_dirs does not make a difference as it only concerns linked dirs
-    for follow_symlink_dirs in [True, False]:
-      artifacts_dict = record_artifacts_as_dict(["."],
-          follow_symlink_dirs=follow_symlink_dirs)
-
-      # Test only the files were recorded ...
-      self.assertListEqual(sorted(list(artifacts_dict.keys())),
-          sorted(self.full_file_path_list))
-
-    for link in links:
-      os.unlink(link)
-
-
-  @unittest.skipIf("symlink" not in os.__dict__, "symlink is not supported in this platform")
-  def test_record_follow_symlinked_directories(self):
-    """Record files in symlinked dirs if follow_symlink_dirs is True. """
-
-    try:
-      # Link to subdir
-      os.symlink("subdir", "subdir_link")
-    except IOError:
-      TestRecordArtifactsAsDict._raise_win_dev_mode_error()
-      raise
-
-    link_pairs = [
-      ("subdir/foosub1", "subdir_link/foosub1"),
-      ("subdir/foosub2", "subdir_link/foosub2"),
-      ("subdir/subsubdir/foosubsub", "subdir_link/subsubdir/foosubsub"),
-    ]
+    @classmethod
+    def setUpClass(self):
+        """Create and change into temp test directory with dummy artifacts.
+        |-- bar
+        |-- foo
+        `-- subdir
+            |-- foosub1
+            |-- foosub2
+            `-- subsubdir
+                `-- foosubsub
+        """
+
+        # Backup and clear user set exclude patterns and base path
+        self.artifact_exclude_orig = in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS
+        self.artifact_base_path_orig = in_toto.settings.ARTIFACT_BASE_PATH
+        in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = []
+        in_toto.settings.ARTIFACT_BASE_PATH = None
+
+        self.set_up_test_dir()
+
+        # Create files on 3 levels
+        os.mkdir("subdir")
+        os.mkdir("subdir/subsubdir")
+
+        self.full_file_path_list = [
+            "foo",
+            "bar",
+            "#esc!",
+            "subdir/foosub1",
+            "subdir/foosub2",
+            "subdir/subsubdir/foosubsub",
+        ]
+
+        for path in self.full_file_path_list:
+            with open(path, "w", encoding="utf8") as fp:
+                fp.write(path)
+
+    @classmethod
+    def tearDownClass(self):
+        """Change back to working dir, remove temp directory, restore settings."""
+        self.tear_down_test_dir()
+        in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = self.artifact_exclude_orig
+        in_toto.settings.ARTIFACT_BASE_PATH = self.artifact_base_path_orig
+
+    def tearDown(self):
+        """Clear the ARTIFACT_EXLCUDES after every test."""
+        in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = []
+        in_toto.settings.ARTIFACT_BASE_PATH = None
+
+    def test_bad_base_path_setting(self):
+        """Raise exception with bogus base path settings."""
+        for base_path in ["path/does/not/exist", 12345, True]:
+            in_toto.settings.ARTIFACT_BASE_PATH = base_path
+            with self.assertRaises((OSError, ValueError)):
+                record_artifacts_as_dict(["."])
+            in_toto.settings.ARTIFACT_BASE_PATH = None
+
+            with self.assertRaises((OSError, ValueError)):
+                record_artifacts_as_dict(["."], base_path=base_path)
+
+    def test_base_path_is_child_dir(self):
+        """Test path of recorded artifacts and cd back with child as base."""
+        base_path = "subdir"
+        expected_artifacts = sorted(
+            ["foosub1", "foosub2", "subsubdir/foosubsub"]
+        )
+
+        in_toto.settings.ARTIFACT_BASE_PATH = base_path
+        artifacts_dict = record_artifacts_as_dict(["."])
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())), expected_artifacts
+        )
+        in_toto.settings.ARTIFACT_BASE_PATH = None
+
+        artifacts_dict = record_artifacts_as_dict(["."], base_path=base_path)
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())), expected_artifacts
+        )
+
+    def test_base_path_is_parent_dir(self):
+        """Test path of recorded artifacts and cd back with parent as base."""
+        base_path = ".."
+        expected_artifacts = sorted(
+            ["foosub1", "foosub2", "subsubdir/foosubsub"]
+        )
+        os.chdir("subdir/subsubdir")
+
+        in_toto.settings.ARTIFACT_BASE_PATH = base_path
+        artifacts_dict = record_artifacts_as_dict(["."])
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())), expected_artifacts
+        )
+        in_toto.settings.ARTIFACT_BASE_PATH = None
+
+        artifacts_dict = record_artifacts_as_dict(["."], base_path=base_path)
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())), expected_artifacts
+        )
+
+        os.chdir(self.test_dir)
+
+    def test_lstrip_paths_valid_prefix_directory(self):
+        lstrip_paths = ["subdir/subsubdir/"]
+        expected_artifacts = sorted(
+            [
+                "#esc!",
+                "bar",
+                "foo",
+                "subdir/foosub1",
+                "subdir/foosub2",
+                "foosubsub",
+            ]
+        )
+        artifacts_dict = record_artifacts_as_dict(
+            ["."], lstrip_paths=lstrip_paths
+        )
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())), expected_artifacts
+        )
+
+    def test_lstrip_paths_substring_prefix_directory(self):
+        lstrip_paths = ["subdir/subsubdir/", "subdir/"]
+        with self.assertRaises(in_toto.exceptions.PrefixError):
+            record_artifacts_as_dict(["."], lstrip_paths=lstrip_paths)
+
+    def test_lstrip_paths_non_unique_key(self):
+        os.mkdir("subdir_new")
+        path = "subdir_new/foosub1"
+        shutil.copy("subdir/foosub1", path)
+        lstrip_paths = ["subdir/", "subdir_new/"]
+        with self.assertRaises(in_toto.exceptions.PrefixError):
+            record_artifacts_as_dict(["."], lstrip_paths=lstrip_paths)
+        os.remove(path)
+        os.rmdir("subdir_new")
 
-    # Record with follow_symlink_dirs TRUE
-    artifacts_dict = record_artifacts_as_dict(["."], follow_symlink_dirs=True)
-    # Test that all files were recorded including files in linked subdir ...
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-        sorted(self.full_file_path_list + [pair[1] for pair in link_pairs]))
-
-    # ... and the hashes of each link/file pair match
-    for pair in link_pairs:
-      self.assertDictEqual(artifacts_dict[pair[0]], artifacts_dict[pair[1]])
-
-    # Record with follow_symlink_dirs FALSE (default)
-    artifacts_dict = record_artifacts_as_dict(["."])
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-        sorted(self.full_file_path_list))
-
-    os.unlink("subdir_link")
-
-
-  def test_record_files_and_subdirs(self):
-    """Explicitly record files and subdirs. """
-    artifacts_dict = record_artifacts_as_dict(["foo", "subdir"])
-
-    for val in list(artifacts_dict.values()):
-      securesystemslib.formats.HASHDICT_SCHEMA.check_match(val)
-
-    self.assertListEqual(sorted(list(artifacts_dict.keys())),
-      sorted(["foo", "subdir/foosub1", "subdir/foosub2",
-          "subdir/subsubdir/foosubsub"]))
-
-
-  def test_exclude_patterns(self):
-    """Test excluding artifacts using passed pattern or setting. """
-    excludes_and_results = [
-      # Exclude files containing 'foo' everywhere
-      (["*foo*"], ["bar", "#esc!"]),
-      # Exclude subdirectory and all its contents
-      (["subdir"], ["bar", "foo", "#esc!"]),
-      # Exclude files 'subdir/foosub1' and 'subdir/foosub2'
-      (["*foosub?"], ["bar", "foo", "#esc!", "subdir/subsubdir/foosubsub"]),
-      # Exclude subsubdirectory and its contents
-      (
-        ["*subsubdir"],
-        ["foo", "bar", "#esc!", "subdir/foosub1", "subdir/foosub2"],
-      ),
-      (["/**"], []),
-      (["*sub*"], ["foo", "bar", "#esc!"]),
-      (
-        ["**/subdir/subsubdir"],
-        ["foo", "bar", "#esc!", "subdir/foosub1", "subdir/foosub2"],
-      ),
-      (
-        ["subdir/foo*"],
-        ["bar", "foo", "#esc!", "subdir/subsubdir/foosubsub"],
-      ),
-      (["**/subdir/"], ["bar", "foo", "#esc!"]),
-      (["foo*"], ["bar", "#esc!"]),
-      (
-        ["**/*1"],
-        ["bar", "foo", "#esc!", "subdir/foosub2", "subdir/subsubdir/foosubsub"]
-      ),
-      (["**/*sub?"], ["bar", "foo", "#esc!", "subdir/subsubdir/foosubsub"]),
-      (["**/foo*[1-9]"], ["bar", "foo", "#esc!", "subdir/subsubdir/foosubsub"]),
-      (["**/[a-z][a-z][a-z][a-z][a-z][a-z]/"], ["bar", "foo", "#esc!"]),
-      (["/subdir"], ["foo", "bar", "#esc!"]),
-      (["subdir/"], ["foo", "bar", "#esc!"]),
-      (
-        ["/subdir/subsubdir"],
-        ["foo", "bar", "#esc!", "subdir/foosub1", "subdir/foosub2"],
-      ),
-      (
-        ["subdir/subsubdir/"],
-        ["foo", "bar", "#esc!", "subdir/foosub1", "subdir/foosub2"],
-      ),
-      (
-        ["\#esc*"],  # pylint: disable=W1401
-        ["foo", "bar", "subdir/foosub1", "subdir/foosub2",
-            "subdir/subsubdir/foosubsub"],
-      ),
-      (
-        ["*esc\!"],  # pylint: disable=W1401
-        ["foo", "bar", "subdir/foosub1", "subdir/foosub2",
-            "subdir/subsubdir/foosubsub"],
-      ),
-      (
-        ["/"],
-        ["foo", "bar", "#esc!", "subdir/foosub1", "subdir/foosub2",
-            "subdir/subsubdir/foosubsub"],
-      )
-    ]
+    def test_lstrip_paths_invalid_prefix_directory(self):
+        lstrip_paths = ["not/a/directory/"]
+        expected_artifacts = sorted(
+            [
+                "#esc!",
+                "bar",
+                "foo",
+                "subdir/foosub1",
+                "subdir/foosub2",
+                "subdir/subsubdir/foosubsub",
+            ]
+        )
+        artifacts_dict = record_artifacts_as_dict(
+            ["."], lstrip_paths=lstrip_paths
+        )
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())), expected_artifacts
+        )
+
+    def test_lstrip_paths_valid_prefix_file(self):
+        lstrip_paths = ["subdir/subsubdir/"]
+        expected_artifacts = sorted(["foosubsub"])
+        artifacts_dict = record_artifacts_as_dict(
+            ["./subdir/subsubdir/foosubsub"], lstrip_paths=lstrip_paths
+        )
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())), expected_artifacts
+        )
+
+    def test_lstrip_paths_non_unique_key_file(self):
+        os.mkdir("subdir/subsubdir_new")
+        path = "subdir/subsubdir_new/foosubsub"
+        shutil.copy("subdir/subsubdir/foosubsub", path)
+        lstrip_paths = ["subdir/subsubdir/", "subdir/subsubdir_new/"]
+        with self.assertRaises(in_toto.exceptions.PrefixError):
+            record_artifacts_as_dict(
+                [
+                    "subdir/subsubdir/foosubsub",
+                    "subdir/subsubdir_new/foosubsub",
+                ],
+                lstrip_paths=lstrip_paths,
+            )
+        os.remove(path)
+        os.rmdir("subdir/subsubdir_new")
 
-    for exclude_patterns, expected_results in excludes_and_results:
-      # Exclude via setting
-      in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = exclude_patterns
-      artifacts1 = record_artifacts_as_dict(["."])
-
-      # Exclude via argument
-      in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = None
-      artifacts2 = record_artifacts_as_dict(["."],
-          exclude_patterns=exclude_patterns)
-
-      self.assertTrue(sorted(list(artifacts1)) == sorted(list(artifacts2))
-          == sorted(expected_results))
-
-
-  def test_bad_artifact_exclude_patterns_setting(self):
-    """Raise exception with bogus artifact exclude patterns settings. """
-    for setting in ["not a list of settings", 12345, True]:
-      in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = setting
-      with self.assertRaises(securesystemslib.exceptions.FormatError):
-        record_artifacts_as_dict(["."])
-
-  def test_hash_artifact_passing_algorithm(self):
-    """Test _hash_artifact passing hash algorithm. """
-    self.assertTrue("sha256" in list(_hash_artifact("foo", ["sha256"])))
+    def test_lstrip_paths_valid_unicode_prefix_file(self):
+        # Try to create a file with unicode character
+        try:
+            os.mkdir("ಠ")
+            path = "ಠ/foo"
+            shutil.copy("foo", path)
+
+            # Attempt to left strip the path now that the file has been created
+            lstrip_paths = ["ಠ/"]
+            expected_artifacts = sorted(["foo"])
+            artifacts_dict = record_artifacts_as_dict(
+                ["./ಠ/"], lstrip_paths=lstrip_paths
+            )
+            self.assertListEqual(
+                sorted(list(artifacts_dict.keys())), expected_artifacts
+            )
+            os.remove(path)
+            os.rmdir("ಠ")
+        except OSError:
+            # OS doesn't support unicode explicit files
+            pass
+
+    def test_empty_artifacts_list_record_nothing(self):
+        """Empty list passed. Return empty dict."""
+        self.assertDictEqual(record_artifacts_as_dict([]), {})
+
+    def test_not_existing_artifacts_in_list_record_nothing(self):
+        """List with not existing artifact passed. Return empty dict."""
+        self.assertDictEqual(record_artifacts_as_dict(["baz"]), {})
+
+    def test_record_dot_check_files_hash_dict_schema(self):
+        """Traverse dir and subdirs. Record three files."""
+        artifacts_dict = record_artifacts_as_dict(["."])
+
+        for val in list(artifacts_dict.values()):
+            securesystemslib.formats.HASHDICT_SCHEMA.check_match(val)
+
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())),
+            sorted(self.full_file_path_list),
+        )
+
+    @staticmethod
+    def _raise_win_dev_mode_error():
+        """If the platform is Windows, raises an error that asks the user if
+        developer mode is activated."""
+        if os.name == "nt":
+            raise IOError(
+                "Developer mode is required to work with symlinks on "
+                "Windows. Is it enabled?"
+            )
+
+    @unittest.skipIf(
+        "symlink" not in os.__dict__,
+        "symlink is not supported in this platform",
+    )
+    def test_record_symlinked_files(self):
+        """Symlinked files are always recorded."""
+        # Symlinked **files** are always recorded ...
+        link_pairs = [
+            ("foo", "foo_link"),
+            ("subdir/foosub1", "subdir/foosub2_link"),
+            ("subdir/subsubdir/foosubsub", "subdir/subsubdir/foosubsub_link"),
+        ]
+
+        # Create links
+        for pair in link_pairs:
+            # We only use the basename of the file (source) as it is on the same
+            # level as the link (target)
+            try:
+                os.symlink(os.path.basename(pair[0]), pair[1])
+            except IOError:
+                TestRecordArtifactsAsDict._raise_win_dev_mode_error()
+                raise
+
+        # Record files and linked files
+        # follow_symlink_dirs does not make a difference as it only concerns linked dirs
+        for follow_symlink_dirs in [True, False]:
+            artifacts_dict = record_artifacts_as_dict(
+                ["."], follow_symlink_dirs=follow_symlink_dirs
+            )
+
+            # Test that everything was recorded ...
+            self.assertListEqual(
+                sorted(list(artifacts_dict.keys())),
+                sorted(
+                    self.full_file_path_list + [pair[1] for pair in link_pairs]
+                ),
+            )
+
+            # ... and the hashes of each link/file pair match
+            for pair in link_pairs:
+                self.assertDictEqual(
+                    artifacts_dict[pair[0]], artifacts_dict[pair[1]]
+                )
+
+        for pair in link_pairs:
+            os.unlink(pair[1])
+
+    @unittest.skipIf(
+        "symlink" not in os.__dict__,
+        "symlink is not supported in this platform",
+    )
+    def test_record_without_dead_symlinks(self):
+        """Dead symlinks are never recorded."""
+
+        # Dead symlinks are never recorded ...
+        links = [
+            "foo_link",
+            "subdir/foosub2_link",
+            "subdir/subsubdir/foosubsub_link",
+        ]
+
+        # Create dead links
+        for link in links:
+            try:
+                os.symlink("does/not/exist", link)
+            except IOError:
+                TestRecordArtifactsAsDict._raise_win_dev_mode_error()
+                raise
+
+        # Record files without dead links
+        # follow_symlink_dirs does not make a difference as it only concerns linked dirs
+        for follow_symlink_dirs in [True, False]:
+            artifacts_dict = record_artifacts_as_dict(
+                ["."], follow_symlink_dirs=follow_symlink_dirs
+            )
+
+            # Test only the files were recorded ...
+            self.assertListEqual(
+                sorted(list(artifacts_dict.keys())),
+                sorted(self.full_file_path_list),
+            )
+
+        for link in links:
+            os.unlink(link)
+
+    @unittest.skipIf(
+        "symlink" not in os.__dict__,
+        "symlink is not supported in this platform",
+    )
+    def test_record_follow_symlinked_directories(self):
+        """Record files in symlinked dirs if follow_symlink_dirs is True."""
+
+        try:
+            # Link to subdir
+            os.symlink("subdir", "subdir_link")
+        except IOError:
+            TestRecordArtifactsAsDict._raise_win_dev_mode_error()
+            raise
+
+        link_pairs = [
+            ("subdir/foosub1", "subdir_link/foosub1"),
+            ("subdir/foosub2", "subdir_link/foosub2"),
+            ("subdir/subsubdir/foosubsub", "subdir_link/subsubdir/foosubsub"),
+        ]
+
+        # Record with follow_symlink_dirs TRUE
+        artifacts_dict = record_artifacts_as_dict(
+            ["."], follow_symlink_dirs=True
+        )
+        # Test that all files were recorded including files in linked subdir ...
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())),
+            sorted(self.full_file_path_list + [pair[1] for pair in link_pairs]),
+        )
+
+        # ... and the hashes of each link/file pair match
+        for pair in link_pairs:
+            self.assertDictEqual(
+                artifacts_dict[pair[0]], artifacts_dict[pair[1]]
+            )
+
+        # Record with follow_symlink_dirs FALSE (default)
+        artifacts_dict = record_artifacts_as_dict(["."])
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())),
+            sorted(self.full_file_path_list),
+        )
+
+        os.unlink("subdir_link")
+
+    def test_record_files_and_subdirs(self):
+        """Explicitly record files and subdirs."""
+        artifacts_dict = record_artifacts_as_dict(["foo", "subdir"])
+
+        for val in list(artifacts_dict.values()):
+            securesystemslib.formats.HASHDICT_SCHEMA.check_match(val)
+
+        self.assertListEqual(
+            sorted(list(artifacts_dict.keys())),
+            sorted(
+                [
+                    "foo",
+                    "subdir/foosub1",
+                    "subdir/foosub2",
+                    "subdir/subsubdir/foosubsub",
+                ]
+            ),
+        )
+
+    def test_exclude_patterns(self):
+        """Test excluding artifacts using passed pattern or setting."""
+        excludes_and_results = [
+            # Exclude files containing 'foo' everywhere
+            (["*foo*"], ["bar", "#esc!"]),
+            # Exclude subdirectory and all its contents
+            (["subdir"], ["bar", "foo", "#esc!"]),
+            # Exclude files 'subdir/foosub1' and 'subdir/foosub2'
+            (
+                ["*foosub?"],
+                ["bar", "foo", "#esc!", "subdir/subsubdir/foosubsub"],
+            ),
+            # Exclude subsubdirectory and its contents
+            (
+                ["*subsubdir"],
+                ["foo", "bar", "#esc!", "subdir/foosub1", "subdir/foosub2"],
+            ),
+            (["/**"], []),
+            (["*sub*"], ["foo", "bar", "#esc!"]),
+            (
+                ["**/subdir/subsubdir"],
+                ["foo", "bar", "#esc!", "subdir/foosub1", "subdir/foosub2"],
+            ),
+            (
+                ["subdir/foo*"],
+                ["bar", "foo", "#esc!", "subdir/subsubdir/foosubsub"],
+            ),
+            (["**/subdir/"], ["bar", "foo", "#esc!"]),
+            (["foo*"], ["bar", "#esc!"]),
+            (
+                ["**/*1"],
+                [
+                    "bar",
+                    "foo",
+                    "#esc!",
+                    "subdir/foosub2",
+                    "subdir/subsubdir/foosubsub",
+                ],
+            ),
+            (
+                ["**/*sub?"],
+                ["bar", "foo", "#esc!", "subdir/subsubdir/foosubsub"],
+            ),
+            (
+                ["**/foo*[1-9]"],
+                ["bar", "foo", "#esc!", "subdir/subsubdir/foosubsub"],
+            ),
+            (["**/[a-z][a-z][a-z][a-z][a-z][a-z]/"], ["bar", "foo", "#esc!"]),
+            (["/subdir"], ["foo", "bar", "#esc!"]),
+            (["subdir/"], ["foo", "bar", "#esc!"]),
+            (
+                ["/subdir/subsubdir"],
+                ["foo", "bar", "#esc!", "subdir/foosub1", "subdir/foosub2"],
+            ),
+            (
+                ["subdir/subsubdir/"],
+                ["foo", "bar", "#esc!", "subdir/foosub1", "subdir/foosub2"],
+            ),
+            (
+                ["\#esc*"],  # pylint: disable=W1401
+                [
+                    "foo",
+                    "bar",
+                    "subdir/foosub1",
+                    "subdir/foosub2",
+                    "subdir/subsubdir/foosubsub",
+                ],
+            ),
+            (
+                ["*esc\!"],  # pylint: disable=W1401
+                [
+                    "foo",
+                    "bar",
+                    "subdir/foosub1",
+                    "subdir/foosub2",
+                    "subdir/subsubdir/foosubsub",
+                ],
+            ),
+            (
+                ["/"],
+                [
+                    "foo",
+                    "bar",
+                    "#esc!",
+                    "subdir/foosub1",
+                    "subdir/foosub2",
+                    "subdir/subsubdir/foosubsub",
+                ],
+            ),
+        ]
+
+        for exclude_patterns, expected_results in excludes_and_results:
+            # Exclude via setting
+            in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = exclude_patterns
+            artifacts1 = record_artifacts_as_dict(["."])
+
+            # Exclude via argument
+            in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = None
+            artifacts2 = record_artifacts_as_dict(
+                ["."], exclude_patterns=exclude_patterns
+            )
+
+            self.assertTrue(
+                sorted(list(artifacts1))
+                == sorted(list(artifacts2))
+                == sorted(expected_results)
+            )
+
+    def test_bad_artifact_exclude_patterns_setting(self):
+        """Raise exception with bogus artifact exclude patterns settings."""
+        for setting in ["not a list of settings", 12345, True]:
+            in_toto.settings.ARTIFACT_EXCLUDE_PATTERNS = setting
+            with self.assertRaises(ValueError):
+                record_artifacts_as_dict(["."])
 
 
 class TestLinkCmdExecTimeoutSetting(unittest.TestCase):
-  """Tests LINK_CMD_EXEC_TIMEOUT setting in settings.py file. """
+    """Tests LINK_CMD_EXEC_TIMEOUT setting in settings.py file."""
 
-  def test_timeout_setting(self):
-    # Save the old timeout and make sure it's saved properly
-    timeout_old = in_toto.settings.LINK_CMD_EXEC_TIMEOUT
-
-    # Modify timeout
-    in_toto.settings.LINK_CMD_EXEC_TIMEOUT = 0.1
-
-    # check if exception is raised
-    with self.assertRaises(subprocess.TimeoutExpired):
-      # Call execute_link to see if new timeout is respected
-      in_toto.runlib.execute_link([sys.executable, '-c', 'while True: pass'], True)
-
-    # check if exception is raised
-    with self.assertRaises(subprocess.TimeoutExpired):
-      # Call execute_link to see if new timeout is respected
-      in_toto.runlib.execute_link([sys.executable, '-c', 'while True: pass'], False)
+    def test_timeout_setting(self):
+        # Save the old timeout and make sure it's saved properly
+        timeout_old = in_toto.settings.LINK_CMD_EXEC_TIMEOUT
+
+        # Modify timeout
+        in_toto.settings.LINK_CMD_EXEC_TIMEOUT = 0.1
+
+        # check if exception is raised
+        with self.assertRaises(subprocess.TimeoutExpired):
+            # Call execute_link to see if new timeout is respected
+            in_toto.runlib.execute_link(
+                [sys.executable, "-c", "while True: pass"], True
+            )
+
+        # check if exception is raised
+        with self.assertRaises(subprocess.TimeoutExpired):
+            # Call execute_link to see if new timeout is respected
+            in_toto.runlib.execute_link(
+                [sys.executable, "-c", "while True: pass"], False
+            )
 
-    # Restore original timeout
-    in_toto.settings.LINK_CMD_EXEC_TIMEOUT = timeout_old
+        # Restore original timeout
+        in_toto.settings.LINK_CMD_EXEC_TIMEOUT = timeout_old
 
-class TestSubprocess(unittest.TestCase):
 
-  def test_run_duplicate_streams(self):
-    """Test output indeed duplicated."""
-    # Command that prints 'foo' to stdout and 'bar' to stderr.
-    cmd = [
-      sys.executable,
-      "-c",
-      "import sys; sys.stdout.write('foo'); sys.stderr.write('bar');"
-    ]
+class TestSubprocess(unittest.TestCase):
+    def test_run_duplicate_streams(self):
+        """Test output indeed duplicated."""
+        # Command that prints 'foo' to stdout and 'bar' to stderr.
+        cmd = [
+            sys.executable,
+            "-c",
+            "import sys; sys.stdout.write('foo'); sys.stderr.write('bar');",
+        ]
+
+        # Create and open fake targets for standard streams
+        stdout_fd, stdout_fn = tempfile.mkstemp()
+        stderr_fd, stderr_fn = tempfile.mkstemp()
+        with open(  # pylint: disable=unspecified-encoding
+            stdout_fn, "r"
+        ) as fake_stdout_reader, os.fdopen(
+            stdout_fd, "w"
+        ) as fake_stdout_writer, open(  # pylint: disable=unspecified-encoding
+            stderr_fn, "r"
+        ) as fake_stderr_reader, os.fdopen(
+            stderr_fd, "w"
+        ) as fake_stderr_writer:
+            # Backup original standard streams and redirect to fake targets
+            real_stdout = sys.stdout
+            real_stderr = sys.stderr
+            sys.stdout = fake_stdout_writer
+            sys.stderr = fake_stderr_writer
+
+            # Run command
+            ret_code, ret_out, ret_err = _subprocess_run_duplicate_streams(
+                cmd, 10
+            )
+
+            # Rewind fake standard streams
+            fake_stdout_reader.seek(0)
+            fake_stderr_reader.seek(0)
+
+            # Assert that what was printed and what was returned is correct
+            self.assertTrue(ret_out == fake_stdout_reader.read() == "foo")
+            self.assertTrue(ret_err == fake_stderr_reader.read() == "bar")
+            # Also assert the return value
+            self.assertEqual(ret_code, 0)
+
+            # Restore original streams
+            sys.stdout = real_stdout
+            sys.stderr = real_stderr
+
+        # Remove fake standard streams
+        os.remove(stdout_fn)
+        os.remove(stderr_fn)
+
+    def test_run_duplicate_streams_return_value(self):
+        """Test return code."""
+        cmd = [sys.executable, "-c", "import sys; sys.exit(100)"]
+        ret_code, _, _ = _subprocess_run_duplicate_streams(cmd, 10)
+        self.assertEqual(ret_code, 100)
+
+    def test_run_duplicate_streams_timeout(self):
+        """Test timeout."""
+        cmd = [sys.executable, "-c", "while True: pass"]
+        with self.assertRaises(subprocess.TimeoutExpired):
+            _subprocess_run_duplicate_streams(cmd, timeout=-1)
 
-    # Create and open fake targets for standard streams
-    stdout_fd, stdout_fn = tempfile.mkstemp()
-    stderr_fd, stderr_fn = tempfile.mkstemp()
-    with open(  # pylint: disable=unspecified-encoding
-      stdout_fn, "r"
-    ) as fake_stdout_reader, os.fdopen(
-      stdout_fd, "w"
-    ) as fake_stdout_writer, open(  # pylint: disable=unspecified-encoding
-      stderr_fn, "r"
-    ) as fake_stderr_reader, os.fdopen(
-      stderr_fd, "w"
-    ) as fake_stderr_writer:
-
-      # Backup original standard streams and redirect to fake targets
-      real_stdout = sys.stdout
-      real_stderr = sys.stderr
-      sys.stdout = fake_stdout_writer
-      sys.stderr = fake_stderr_writer
-
-      # Run command
-      ret_code, ret_out, ret_err = _subprocess_run_duplicate_streams(cmd, 10)
-
-      # Rewind fake standard streams
-      fake_stdout_reader.seek(0)
-      fake_stderr_reader.seek(0)
-
-      # Assert that what was printed and what was returned is correct
-      self.assertTrue(ret_out == fake_stdout_reader.read() == "foo")
-      self.assertTrue(ret_err == fake_stderr_reader.read() == "bar")
-      # Also assert the return value
-      self.assertEqual(ret_code, 0)
-
-      # Restore original streams
-      sys.stdout = real_stdout
-      sys.stderr = real_stderr
-
-    # Remove fake standard streams
-    os.remove(stdout_fn)
-    os.remove(stderr_fn)
-
-  def test_run_duplicate_streams_return_value(self):
-    """Test return code."""
-    cmd = [sys.executable, "-c", "import sys; sys.exit(100)"]
-    ret_code, _, _ = _subprocess_run_duplicate_streams(cmd, 10)
-    self.assertEqual(ret_code, 100)
-
-  def test_run_duplicate_streams_timeout(self):
-    """Test timeout."""
-    cmd = [sys.executable,  "-c", "while True: pass"]
-    with self.assertRaises(subprocess.TimeoutExpired ):
-      _subprocess_run_duplicate_streams(cmd, timeout=-1)
 
 class TestInTotoRun(unittest.TestCase, TmpDirMixin):
-  """"
-  Tests runlib.in_toto_run() with different arguments
+    """ "
+    Tests runlib.in_toto_run() with different arguments
 
-  Calls in_toto_run library funtion inside of a temporary directory that
-  contains a test artifact and a test keypair
+    Calls in_toto_run library funtion inside of a temporary directory that
+    contains a test artifact and a test keypair
 
-  If the function does not fail it will dump a test step link metadata file
-  to the temp dir which is removed after every test.
+    If the function does not fail it will dump a test step link metadata file
+    to the temp dir which is removed after every test.
 
-  """
-
-  @classmethod
-  def setUpClass(self):
-    """Create and change into temporary directory, generate key pair and dummy
-    material, read key pair. """
-    self.set_up_test_dir()
-
-    self.step_name = "test_step"
-    self.key_path = "test_key"
-    generate_and_write_unencrypted_rsa_keypair(self.key_path)
-    self.key = import_rsa_privatekey_from_file(self.key_path)
-    self.key_pub = import_rsa_publickey_from_file(self.key_path + ".pub")
-
-    self.test_artifact = "test_artifact"
-    Path(self.test_artifact).touch()
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-
-  def tearDown(self):
-    """Remove link file if it was created. """
-    try:
-      os.remove(FILENAME_FORMAT.format(step_name=self.step_name, keyid=self.key["keyid"]))
-    except OSError:
-      pass
-
-  def test_in_toto_run_verify_signature(self):
-    """Successfully run, verify signed metadata. """
-    link = in_toto_run(self.step_name, None, None,
-        ["python", "--version"], True, self.key)
-    link.verify_signature(self.key)
-
-  def test_in_toto_run_no_signature(self):
-    """Successfully run, verify empty signature field. """
-    link = in_toto_run(self.step_name, None, None, ["python", "--version"])
-    self.assertFalse(len(link.signatures))
-
-  def test_in_toto_run_with_byproduct(self):
-    """Successfully run, verify recorded byproduct. """
-    link = in_toto_run(self.step_name, None, None, ["python", "--version"],
-        record_streams=True)
-
-    # this or clause may seem weird, but given that python 2 prints its version
-    # to stderr while python3 prints it to stdout we check on both (or add a
-    # more verbose if clause)
-    stderr_contents = link.signed.byproducts.get("stderr")
-    stdout_contents = link.signed.byproducts.get("stdout")
-    self.assertTrue("Python" in stderr_contents or "Python" in stdout_contents,
-        msg="\nSTDERR:\n{}\nSTDOUT:\n{}".format(stderr_contents, stdout_contents))
-
-  def test_in_toto_run_without_byproduct(self):
-    """Successfully run, verify byproduct is not recorded. """
-    link = in_toto_run(self.step_name, None, None, ["python", "--version"],
-        record_streams=False)
-    self.assertFalse(len(link.signed.byproducts.get("stdout")))
-
-  def test_in_toto_run_compare_dumped_with_returned_link(self):
-    """Successfully run, compare dumped link is equal to returned link. """
-    link = in_toto_run(self.step_name, [self.test_artifact],
-        [self.test_artifact], ["python", "--version"], True, self.key)
-    link_dump = Metablock.load(
-        FILENAME_FORMAT.format(step_name=self.step_name, keyid=self.key["keyid"]))
-    self.assertEqual(repr(link), repr(link_dump))
-
-  def test_in_toto_run_with_metadata_directory(self):
-    """Successfully run with metadata directory,
-     compare dumped link is equal to returned link"""
-    tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
-    link = in_toto_run(self.step_name, [self.test_artifact],
-        [self.test_artifact], ["python", "--version"], True, self.key,
-        metadata_directory=tmp_dir)
-    file_path = os.path.join(tmp_dir, FILENAME_FORMAT.format(step_name=self.step_name,
-        keyid=self.key["keyid"]))
-    link_dump = Metablock.load(file_path)
-    self.assertEqual(repr(link), repr(link_dump))
-
-  def test_in_toto_run_compare_with_and_without_metadata_directory(self):
-    """Successfully run with and without metadata directory,
-     compare the signed is equal"""
-    tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
-    in_toto_run(self.step_name, [self.test_artifact], [self.test_artifact],
-        ["python", "--version"], True, self.key, metadata_directory=tmp_dir)
-    file_path = os.path.join(tmp_dir, FILENAME_FORMAT.format(step_name=self.step_name,
-        keyid=self.key["keyid"]))
-    link_dump_with_md = Metablock.load(file_path)
-
-    in_toto_run(self.step_name, [self.test_artifact], [self.test_artifact],
-        ["python", "--version"], True, self.key)
-    link_dump_without_md = Metablock.load(
-        FILENAME_FORMAT.format(step_name=self.step_name, keyid=self.key["keyid"]))
-    self.assertEqual(repr(link_dump_with_md.signed),
-        repr(link_dump_without_md.signed))
-
-  def test_in_toto_run_verify_recorded_artifacts(self):
-    """Successfully run, verify properly recorded artifacts. """
-    link = in_toto_run(self.step_name, [self.test_artifact],
-        [self.test_artifact], ["python", "--version"])
-    self.assertEqual(list(link.signed.materials.keys()),
-        list(link.signed.products.keys()), [self.test_artifact])
-
-  def test_in_toto_run_verify_workdir(self):
-    """Successfully run, verify cwd. """
-    link = in_toto_run(self.step_name, [], [], ["python", "--version"],
-        record_environment=True)
-    self.assertEqual(link.signed.environment["workdir"],
-        os.getcwd().replace("\\", "/"))
-
-  def test_normalize_line_endings(self):
-    """Test cross-platform line ending normalization. """
-    paths = []
-    try:
-      # Create three artifacts with same content but different line endings
-      for line_ending in [b"\n", b"\r", b"\r\n"]:
+    """
+
+    @classmethod
+    def setUpClass(self):
+        """Create and change into temporary directory, generate key pair and dummy
+        material, read key pair."""
+        self.set_up_test_dir()
+
+        self.step_name = "test_step"
+        self.key_path = "test_key"
+        generate_and_write_unencrypted_rsa_keypair(self.key_path)
+        self.key = import_rsa_privatekey_from_file(self.key_path)
+        self.key_pub = import_rsa_publickey_from_file(self.key_path + ".pub")
+
+        self.test_artifact = "test_artifact"
+        Path(self.test_artifact).touch()
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def tearDown(self):
+        """Remove link file if it was created."""
+        try:
+            os.remove(
+                FILENAME_FORMAT.format(
+                    step_name=self.step_name, keyid=self.key["keyid"]
+                )
+            )
+        except OSError:
+            pass
+
+    def test_in_toto_run_verify_signature(self):
+        """Successfully run, verify signed metadata."""
+        link = in_toto_run(
+            self.step_name, None, None, ["python", "--version"], True, self.key
+        )
+        link.verify_signature(self.key)
+
+    def test_in_toto_run_no_signature(self):
+        """Successfully run, verify empty signature field."""
+        link = in_toto_run(self.step_name, None, None, ["python", "--version"])
+        self.assertFalse(len(link.signatures))
+
+    def test_in_toto_run_with_byproduct(self):
+        """Successfully run, verify recorded byproduct."""
+        link = in_toto_run(
+            self.step_name,
+            None,
+            None,
+            ["python", "--version"],
+            record_streams=True,
+        )
+
+        # this or clause may seem weird, but given that python 2 prints its version
+        # to stderr while python3 prints it to stdout we check on both (or add a
+        # more verbose if clause)
+        stderr_contents = link.signed.byproducts.get("stderr")
+        stdout_contents = link.signed.byproducts.get("stdout")
+        self.assertTrue(
+            "Python" in stderr_contents or "Python" in stdout_contents,
+            msg="\nSTDERR:\n{}\nSTDOUT:\n{}".format(
+                stderr_contents, stdout_contents
+            ),
+        )
+
+    def test_in_toto_run_without_byproduct(self):
+        """Successfully run, verify byproduct is not recorded."""
+        link = in_toto_run(
+            self.step_name,
+            None,
+            None,
+            ["python", "--version"],
+            record_streams=False,
+        )
+        self.assertFalse(len(link.signed.byproducts.get("stdout")))
+
+    def test_in_toto_run_compare_dumped_with_returned_link(self):
+        """Successfully run, compare dumped link is equal to returned link."""
+        link = in_toto_run(
+            self.step_name,
+            [self.test_artifact],
+            [self.test_artifact],
+            ["python", "--version"],
+            True,
+            self.key,
+        )
+        link_dump = Metablock.load(
+            FILENAME_FORMAT.format(
+                step_name=self.step_name, keyid=self.key["keyid"]
+            )
+        )
+        self.assertEqual(repr(link), repr(link_dump))
+
+    def test_in_toto_run_with_metadata_directory(self):
+        """Successfully run with metadata directory,
+        compare dumped link is equal to returned link"""
+        tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
+        link = in_toto_run(
+            self.step_name,
+            [self.test_artifact],
+            [self.test_artifact],
+            ["python", "--version"],
+            True,
+            self.key,
+            metadata_directory=tmp_dir,
+        )
+        file_path = os.path.join(
+            tmp_dir,
+            FILENAME_FORMAT.format(
+                step_name=self.step_name, keyid=self.key["keyid"]
+            ),
+        )
+        link_dump = Metablock.load(file_path)
+        self.assertEqual(repr(link), repr(link_dump))
+
+    def test_in_toto_run_compare_with_and_without_metadata_directory(self):
+        """Successfully run with and without metadata directory,
+        compare the signed is equal"""
+        tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
+        in_toto_run(
+            self.step_name,
+            [self.test_artifact],
+            [self.test_artifact],
+            ["python", "--version"],
+            True,
+            self.key,
+            metadata_directory=tmp_dir,
+        )
+        file_path = os.path.join(
+            tmp_dir,
+            FILENAME_FORMAT.format(
+                step_name=self.step_name, keyid=self.key["keyid"]
+            ),
+        )
+        link_dump_with_md = Metablock.load(file_path)
+
+        in_toto_run(
+            self.step_name,
+            [self.test_artifact],
+            [self.test_artifact],
+            ["python", "--version"],
+            True,
+            self.key,
+        )
+        link_dump_without_md = Metablock.load(
+            FILENAME_FORMAT.format(
+                step_name=self.step_name, keyid=self.key["keyid"]
+            )
+        )
+        self.assertEqual(
+            repr(link_dump_with_md.signed), repr(link_dump_without_md.signed)
+        )
+
+    def test_in_toto_run_verify_recorded_artifacts(self):
+        """Successfully run, verify properly recorded artifacts."""
+        link = in_toto_run(
+            self.step_name,
+            [self.test_artifact],
+            [self.test_artifact],
+            ["python", "--version"],
+        )
+        self.assertEqual(
+            list(link.signed.materials.keys()),
+            list(link.signed.products.keys()),
+            [self.test_artifact],
+        )
+
+    def test_in_toto_run_verify_workdir(self):
+        """Successfully run, verify cwd."""
+        link = in_toto_run(
+            self.step_name,
+            [],
+            [],
+            ["python", "--version"],
+            record_environment=True,
+        )
+        self.assertEqual(
+            link.signed.environment["workdir"], os.getcwd().replace("\\", "/")
+        )
+
+    def test_normalize_line_endings(self):
+        """Test cross-platform line ending normalization."""
+        paths = []
+        try:
+            # Create three artifacts with same content but different line endings
+            for line_ending in [b"\n", b"\r", b"\r\n"]:
+                fd, path = tempfile.mkstemp()
+                paths.append(path)
+                os.write(fd, b"hello" + line_ending + b"toto")
+                os.close(fd)
+
+            # Call in_toto_run and record artifacts as materials and products
+            # with line ending normalization on
+            link = in_toto_run(
+                self.step_name,
+                paths,
+                paths,
+                ["python", "--version"],
+                normalize_line_endings=True,
+            ).signed
+
+            # Check that all three hashes in materials and products are equal
+            for artifact_dict in [link.materials, link.products]:
+                hash_dicts = list(artifact_dict.values())
+                self.assertTrue(hash_dicts[1:] == hash_dicts[:-1])
+
+        # Clean up
+        finally:
+            for path in paths:
+                os.remove(path)
+
+    def test_in_toto_bad_signing_key_format(self):
+        """Fail run, passed key is not properly formatted."""
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            in_toto_run(
+                self.step_name,
+                None,
+                None,
+                ["python", "--version"],
+                True,
+                "this-is-not-a-key",
+            )
+
+    def test_in_toto_wrong_key(self):
+        """Fail run, passed key is a public key."""
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            in_toto_run(
+                self.step_name,
+                None,
+                None,
+                ["python", "--version"],
+                True,
+                self.key_pub,
+            )
+
+    def test_nonexistent_directory(self):
+        """Fail run, passed metadata_directory not exist."""
+        with self.assertRaises(FileNotFoundError):
+            in_toto_run(
+                self.step_name,
+                None,
+                None,
+                ["python", "--version"],
+                True,
+                self.key,
+                metadata_directory="nonexistentDir",
+            )
+
+    def test_not_a_directory(self):
+        """Fail run, passed metadata_directory is not a directory."""
         fd, path = tempfile.mkstemp()
-        paths.append(path)
-        os.write(fd, b"hello" + line_ending + b"toto")
+        os.write(fd, b"hello in-toto")
         os.close(fd)
-
-      # Call in_toto_run and record artifacts as materials and products
-      # with line ending normalization on
-      link = in_toto_run(self.step_name, paths, paths, ["python", "--version"],
-          normalize_line_endings=True).signed
-
-      # Check that all three hashes in materials and products are equal
-      for artifact_dict in [link.materials, link.products]:
-        hash_dicts = list(artifact_dict.values())
-        self.assertTrue(hash_dicts[1:] == hash_dicts[:-1])
-
-    # Clean up
-    finally:
-      for path in paths:
+        # Windows will raise FileNotFoundError instead of NotADirectoryError
+        with self.assertRaises((NotADirectoryError, FileNotFoundError)):
+            in_toto_run(
+                self.step_name,
+                None,
+                None,
+                ["python", "--version"],
+                True,
+                self.key,
+                metadata_directory=path,
+            )
         os.remove(path)
 
-
-  def test_in_toto_bad_signing_key_format(self):
-    """Fail run, passed key is not properly formatted. """
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      in_toto_run(self.step_name, None, None,
-          ["python", "--version"], True, "this-is-not-a-key")
-
-  def test_in_toto_wrong_key(self):
-    """Fail run, passed key is a public key. """
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      in_toto_run(self.step_name, None, None,
-          ["python", "--version"], True, self.key_pub)
-
-  def test_nonexistent_directory(self):
-    """Fail run, passed metadata_directory not exist. """
-    with self.assertRaises(FileNotFoundError):
-      in_toto_run(self.step_name, None, None, ["python", "--version"],
-          True, self.key, metadata_directory='nonexistentDir')
-
-  def test_not_a_directory(self):
-    """Fail run, passed metadata_directory is not a directory. """
-    fd, path = tempfile.mkstemp()
-    os.write(fd, b"hello in-toto")
-    os.close(fd)
-    # Windows will raise FileNotFoundError instead of NotADirectoryError
-    with self.assertRaises((NotADirectoryError, FileNotFoundError)):
-      in_toto_run(self.step_name, None, None, ["python", "--version"],
-          True, self.key, metadata_directory=path)
-    os.remove(path)
-
-  @unittest.skipIf(os.name == 'nt', "chmod doesn't work properly on Windows")
-  def test_in_toto_read_only_metadata_directory(self):
-    """Fail run, passed metadata directory is read only"""
-    tmp_dir = os.path.realpath(tempfile.mkdtemp())
-    # make the directory read only
-    os.chmod(tmp_dir, stat.S_IREAD)
-    with self.assertRaises(PermissionError):
-      in_toto_run(self.step_name, None, None, ["python", "--version"],
-          True, self.key, metadata_directory=tmp_dir)
-    os.rmdir(tmp_dir)
-
-  def test_in_toto_for_dsse(self):
-    """Test metadata generation using dsse."""
-
-    link_metadata = in_toto_run(self.step_name, None, None,
-        ["python", "--version"], True, self.key, use_dsse=True)
-    self.assertIsInstance(link_metadata, Envelope)
-    link_metadata.verify_signature(self.key)
+    @unittest.skipIf(os.name == "nt", "chmod doesn't work properly on Windows")
+    def test_in_toto_read_only_metadata_directory(self):
+        """Fail run, passed metadata directory is read only"""
+        tmp_dir = os.path.realpath(tempfile.mkdtemp())
+        # make the directory read only
+        os.chmod(tmp_dir, stat.S_IREAD)
+        with self.assertRaises(PermissionError):
+            in_toto_run(
+                self.step_name,
+                None,
+                None,
+                ["python", "--version"],
+                True,
+                self.key,
+                metadata_directory=tmp_dir,
+            )
+        os.rmdir(tmp_dir)
+
+    def test_in_toto_for_dsse(self):
+        """Test metadata generation using dsse."""
+
+        link_metadata = in_toto_run(
+            self.step_name,
+            None,
+            None,
+            ["python", "--version"],
+            True,
+            self.key,
+            use_dsse=True,
+        )
+        self.assertIsInstance(link_metadata, Envelope)
+        link_metadata.verify_signature(self.key)
 
 
 class TestInTotoRecordStart(unittest.TestCase, TmpDirMixin):
-  """"Test in_toto_record_start(step_name, key, material_list). """
+    """ "Test in_toto_record_start(step_name, key, material_list)."""
+
+    @classmethod
+    def setUpClass(self):
+        """Create and change into temporary directory, generate key pair and dummy
+        material, read key pair."""
+        self.set_up_test_dir()
+
+        self.key_path = "test_key"
+        generate_and_write_unencrypted_rsa_keypair(self.key_path)
+        self.key = import_rsa_privatekey_from_file(self.key_path)
+
+        self.step_name = "test_step"
+        self.link_name_unfinished = UNFINISHED_FILENAME_FORMAT.format(
+            step_name=self.step_name, keyid=self.key["keyid"]
+        )
+
+        self.test_material = "test_material"
+        Path(self.test_material).touch()
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_UNFINISHED_FILENAME_FORMAT(self):
+        """Test if the unfinished filname format."""
+        self.assertTrue(
+            self.link_name_unfinished
+            == ".{}.{:.8}.link-unfinished".format(
+                self.step_name, self.key["keyid"]
+            )
+        )
+
+    def test_create_unfinished_metadata_with_expected_material(self):
+        """Test record start creates metadata with expected material."""
+        in_toto_record_start(self.step_name, [self.test_material], self.key)
+        link = Metablock.load(self.link_name_unfinished)
+        self.assertEqual(
+            list(link.signed.materials.keys()), [self.test_material]
+        )
+        os.remove(self.link_name_unfinished)
+
+    def test_create_unfinished_metadata_verify_signature(self):
+        """Test record start creates metadata with expected signature."""
+        in_toto_record_start(self.step_name, [self.test_material], self.key)
+        link = Metablock.load(self.link_name_unfinished)
+        link.verify_signature(self.key)
+        os.remove(self.link_name_unfinished)
+
+    def test_no_key_arguments(self):
+        """Test record start without passing one required key argument."""
+        with self.assertRaises(ValueError):
+            in_toto_record_start(
+                self.step_name,
+                [],
+                signing_key=None,
+                gpg_keyid=None,
+                gpg_use_default=False,
+            )
+
+    def test_create_unfinished_metadata_using_dsse(self):
+        """Test record start creates metadata using dsse."""
+        in_toto_record_start(
+            self.step_name, [self.test_material], self.key, use_dsse=True
+        )
+        link_metadata = Envelope.load(self.link_name_unfinished)
+        link_metadata.verify_signature(self.key)
+        os.remove(self.link_name_unfinished)
 
-  @classmethod
-  def setUpClass(self):
-    """Create and change into temporary directory, generate key pair and dummy
-    material, read key pair. """
-    self.set_up_test_dir()
-
-    self.key_path = "test_key"
-    generate_and_write_unencrypted_rsa_keypair(self.key_path)
-    self.key = import_rsa_privatekey_from_file(self.key_path)
-
-    self.step_name = "test_step"
-    self.link_name_unfinished = UNFINISHED_FILENAME_FORMAT.format(step_name=self.step_name, keyid=self.key["keyid"])
-
-    self.test_material = "test_material"
-    Path(self.test_material).touch()
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def test_UNFINISHED_FILENAME_FORMAT(self):
-    """Test if the unfinished filname format. """
-    self.assertTrue(self.link_name_unfinished ==
-        ".{}.{:.8}.link-unfinished".format(self.step_name, self.key["keyid"]))
-
-  def test_create_unfinished_metadata_with_expected_material(self):
-    """Test record start creates metadata with expected material. """
-    in_toto_record_start(
-        self.step_name, [self.test_material], self.key)
-    link = Metablock.load(self.link_name_unfinished)
-    self.assertEqual(list(link.signed.materials.keys()), [self.test_material])
-    os.remove(self.link_name_unfinished)
-
-  def test_create_unfinished_metadata_verify_signature(self):
-    """Test record start creates metadata with expected signature. """
-    in_toto_record_start(
-        self.step_name, [self.test_material], self.key)
-    link = Metablock.load(self.link_name_unfinished)
-    link.verify_signature(self.key)
-    os.remove(self.link_name_unfinished)
-
-  def test_no_key_arguments(self):
-    """Test record start without passing one required key argument. """
-    with self.assertRaises(ValueError):
-      in_toto_record_start(
-          self.step_name, [], signing_key=None, gpg_keyid=None,
-          gpg_use_default=False)
-
-  def test_create_unfinished_metadata_using_dsse(self):
-    """Test record start creates metadata using dsse."""
-    in_toto_record_start(
-        self.step_name, [self.test_material], self.key, use_dsse=True)
-    link_metadata = Envelope.load(self.link_name_unfinished)
-    link_metadata.verify_signature(self.key)
-    os.remove(self.link_name_unfinished)
 
 class TestInTotoRecordStop(unittest.TestCase, TmpDirMixin):
-  """"Test in_toto_record_stop(step_name, key, product_list). """
+    """ "Test in_toto_record_stop(step_name, key, product_list)."""
+
+    @classmethod
+    def setUpClass(self):
+        """Create and change into temporary directory, generate two key pairs
+        and dummy product."""
+        self.set_up_test_dir()
+
+        self.key_path = "test-key"
+        self.key_path2 = "test-key2"
+        generate_and_write_unencrypted_rsa_keypair(self.key_path)
+        generate_and_write_unencrypted_rsa_keypair(self.key_path2)
+        self.key = import_rsa_privatekey_from_file(self.key_path)
+        self.key2 = import_rsa_privatekey_from_file(self.key_path2)
+
+        self.step_name = "test-step"
+        self.link_name = "{}.{:.8}.link".format(
+            self.step_name, self.key["keyid"]
+        )
+        self.link_name_unfinished = UNFINISHED_FILENAME_FORMAT.format(
+            step_name=self.step_name, keyid=self.key["keyid"]
+        )
+
+        self.test_product = "test_product"
+        Path(self.test_product).touch()
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_create_metadata_with_expected_product(self):
+        """Test record stop records expected product."""
+        in_toto_record_start(self.step_name, [], self.key)
+        in_toto_record_stop(self.step_name, [self.test_product], self.key)
+        link = Metablock.load(self.link_name)
+        self.assertEqual(list(link.signed.products.keys()), [self.test_product])
+        os.remove(self.link_name)
+
+    def test_compare_metadata_with_and_without_metadata_directory(self):
+        """Test record stop with and without metadata directory,
+        compare the expected product"""
+        tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
+        in_toto_record_start(self.step_name, [], self.key)
+        in_toto_record_stop(
+            self.step_name,
+            [self.test_product],
+            self.key,
+            metadata_directory=tmp_dir,
+        )
+        link_path = os.path.join(tmp_dir, self.link_name)
+        link_with_md = Metablock.load(link_path)
+
+        in_toto_record_start(self.step_name, [], self.key)
+        in_toto_record_stop(self.step_name, [self.test_product], self.key)
+        link_without_md = Metablock.load(self.link_name)
+        self.assertEqual(link_with_md.signed, link_without_md.signed)
+        os.remove(link_path)
+        os.remove(self.link_name)
+
+    def test_create_metadata_with_expected_cwd(self):
+        """Test record start/stop run, verify cwd."""
+        in_toto_record_start(
+            self.step_name, [], self.key, record_environment=True
+        )
+        in_toto_record_stop(self.step_name, [self.test_product], self.key)
+        link = Metablock.load(self.link_name)
+        self.assertEqual(
+            link.signed.environment["workdir"], os.getcwd().replace("\\", "/")
+        )
+        os.remove(self.link_name)
+
+    def test_create_metadata_verify_signature(self):
+        """Test record start creates metadata with expected signature."""
+        in_toto_record_start(self.step_name, [], self.key)
+        in_toto_record_stop(self.step_name, [], self.key)
+        link = Metablock.load(self.link_name)
+        link.verify_signature(self.key)
+        os.remove(self.link_name)
+
+    def test_replace_unfinished_metadata(self):
+        """Test record stop removes unfinished file and creates link file."""
+        in_toto_record_start(self.step_name, [], self.key)
+        in_toto_record_stop(self.step_name, [], self.key)
+        with self.assertRaises(IOError):
+            # pylint: disable-next=consider-using-with
+            open(self.link_name_unfinished, "r", encoding="utf8")
+        self.assertTrue(os.path.isfile(self.link_name))
+        os.remove(self.link_name)
+
+    def test_missing_unfinished_file(self):
+        """Test record stop exits on missing unfinished file, no link recorded."""
+        with self.assertRaises(IOError):
+            in_toto_record_stop(self.step_name, [], self.key)
+        with self.assertRaises(IOError):
+            # pylint: disable-next=consider-using-with
+            open(self.link_name, "r", encoding="utf8")
+
+    def test_wrong_signature_in_unfinished_metadata(self):
+        """Test record stop exits on wrong signature, no link recorded."""
+        in_toto_record_start(self.step_name, [], self.key)
+        link_name = UNFINISHED_FILENAME_FORMAT.format(
+            step_name=self.step_name, keyid=self.key["keyid"]
+        )
+        changed_link_name = UNFINISHED_FILENAME_FORMAT.format(
+            step_name=self.step_name, keyid=self.key2["keyid"]
+        )
+        os.rename(link_name, changed_link_name)
+        with self.assertRaises(SignatureVerificationError):
+            in_toto_record_stop(self.step_name, [], self.key2)
+        with self.assertRaises(IOError):
+            # pylint: disable-next=consider-using-with
+            open(self.link_name, "r", encoding="utf8")
+        os.rename(changed_link_name, link_name)
+        os.remove(self.link_name_unfinished)
+
+    def test_no_key_arguments(self):
+        """Test record stop without passing one required key argument."""
+        with self.assertRaises(ValueError):
+            in_toto_record_stop(
+                self.step_name,
+                [],
+                signing_key=None,
+                gpg_keyid=None,
+                gpg_use_default=False,
+            )
+
+    def test_normalize_line_endings(self):
+        """Test cross-platform line ending normalization."""
+        paths = []
+        try:
+            # Create three artifacts with same content but different line endings
+            for line_ending in [b"\n", b"\r", b"\r\n"]:
+                fd, path = tempfile.mkstemp()
+                paths.append(path)
+                os.write(fd, b"hello" + line_ending + b"toto")
+                os.close(fd)
+
+            # Call in_toto_record start and stop and record artifacts as
+            # materials and products with line ending normalization on
+            in_toto_record_start(
+                self.step_name, paths, self.key, normalize_line_endings=True
+            )
+            in_toto_record_stop(
+                self.step_name, paths, self.key, normalize_line_endings=True
+            )
+            link = Metablock.load(self.link_name).signed
+
+            # Check that all three hashes in materials and products are equal
+            for artifact_dict in [link.materials, link.products]:
+                hash_dicts = list(artifact_dict.values())
+                self.assertTrue(hash_dicts[1:] == hash_dicts[:-1])
+
+        # Clean up
+        finally:
+            for path in paths:
+                os.remove(path)
+
+    def test_nonexistent_directory(self):
+        """Test record stop with nonexistent metadata directory"""
+        with self.assertRaises(FileNotFoundError):
+            in_toto_record_start(self.step_name, [], self.key)
+            in_toto_record_stop(
+                self.step_name,
+                [],
+                self.key,
+                metadata_directory="nonexistentDir",
+            )
 
-  @classmethod
-  def setUpClass(self):
-    """Create and change into temporary directory, generate two key pairs
-    and dummy product. """
-    self.set_up_test_dir()
-
-    self.key_path = "test-key"
-    self.key_path2 = "test-key2"
-    generate_and_write_unencrypted_rsa_keypair(self.key_path)
-    generate_and_write_unencrypted_rsa_keypair(self.key_path2)
-    self.key = import_rsa_privatekey_from_file(self.key_path)
-    self.key2 = import_rsa_privatekey_from_file(self.key_path2)
-
-    self.step_name = "test-step"
-    self.link_name = "{}.{:.8}.link".format(self.step_name, self.key["keyid"])
-    self.link_name_unfinished = UNFINISHED_FILENAME_FORMAT.format(
-        step_name=self.step_name, keyid=self.key["keyid"])
-
-    self.test_product = "test_product"
-    Path(self.test_product).touch()
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def test_create_metadata_with_expected_product(self):
-    """Test record stop records expected product. """
-    in_toto_record_start(self.step_name, [], self.key)
-    in_toto_record_stop(self.step_name, [self.test_product], self.key)
-    link = Metablock.load(self.link_name)
-    self.assertEqual(list(link.signed.products.keys()), [self.test_product])
-    os.remove(self.link_name)
-
-  def test_compare_metadata_with_and_without_metadata_directory(self):
-    """Test record stop with and without metadata directory,
-     compare the expected product"""
-    tmp_dir = os.path.realpath(tempfile.mkdtemp(dir=os.getcwd()))
-    in_toto_record_start(self.step_name, [], self.key)
-    in_toto_record_stop(self.step_name, [self.test_product], self.key,
-        metadata_directory=tmp_dir)
-    link_path = os.path.join(tmp_dir, self.link_name)
-    link_with_md = Metablock.load(link_path)
-
-    in_toto_record_start(self.step_name, [], self.key)
-    in_toto_record_stop(self.step_name, [self.test_product], self.key)
-    link_without_md = Metablock.load(self.link_name)
-    self.assertEqual(link_with_md.signed, link_without_md.signed)
-    os.remove(link_path)
-    os.remove(self.link_name)
-
-  def test_create_metadata_with_expected_cwd(self):
-    """Test record start/stop run, verify cwd. """
-    in_toto_record_start(self.step_name, [], self.key, record_environment=True)
-    in_toto_record_stop(self.step_name, [self.test_product], self.key)
-    link = Metablock.load(self.link_name)
-    self.assertEqual(link.signed.environment["workdir"],
-        os.getcwd().replace('\\', '/'))
-    os.remove(self.link_name)
-
-  def test_create_metadata_verify_signature(self):
-    """Test record start creates metadata with expected signature. """
-    in_toto_record_start(self.step_name, [], self.key)
-    in_toto_record_stop(self.step_name, [], self.key)
-    link = Metablock.load(self.link_name)
-    link.verify_signature(self.key)
-    os.remove(self.link_name)
-
-  def test_replace_unfinished_metadata(self):
-    """Test record stop removes unfinished file and creates link file. """
-    in_toto_record_start(self.step_name, [], self.key)
-    in_toto_record_stop(self.step_name, [], self.key)
-    with self.assertRaises(IOError):
-      # pylint: disable-next=consider-using-with
-      open(self.link_name_unfinished, "r", encoding="utf8")
-    self.assertTrue(os.path.isfile(self.link_name))
-    os.remove(self.link_name)
-
-  def test_missing_unfinished_file(self):
-    """Test record stop exits on missing unfinished file, no link recorded. """
-    with self.assertRaises(IOError):
-      in_toto_record_stop(self.step_name, [], self.key)
-    with self.assertRaises(IOError):
-      # pylint: disable-next=consider-using-with
-      open(self.link_name, "r", encoding="utf8")
-
-  def test_wrong_signature_in_unfinished_metadata(self):
-    """Test record stop exits on wrong signature, no link recorded. """
-    in_toto_record_start(self.step_name, [], self.key)
-    link_name = UNFINISHED_FILENAME_FORMAT.format(
-        step_name=self.step_name, keyid=self.key["keyid"])
-    changed_link_name = UNFINISHED_FILENAME_FORMAT.format(
-        step_name=self.step_name, keyid=self.key2["keyid"])
-    os.rename(link_name, changed_link_name)
-    with self.assertRaises(SignatureVerificationError):
-      in_toto_record_stop(self.step_name, [], self.key2)
-    with self.assertRaises(IOError):
-      # pylint: disable-next=consider-using-with
-      open(self.link_name, "r", encoding="utf8")
-    os.rename(changed_link_name, link_name)
-    os.remove(self.link_name_unfinished)
-
-  def test_no_key_arguments(self):
-    """Test record stop without passing one required key argument. """
-    with self.assertRaises(ValueError):
-      in_toto_record_stop(
-          self.step_name, [], signing_key=None, gpg_keyid=None,
-          gpg_use_default=False)
-
-  def test_normalize_line_endings(self):
-    """Test cross-platform line ending normalization. """
-    paths = []
-    try:
-      # Create three artifacts with same content but different line endings
-      for line_ending in [b"\n", b"\r", b"\r\n"]:
+    def test_not_a_directory(self):
+        """Test record stop, passed metadata directory is not a dir"""
         fd, path = tempfile.mkstemp()
-        paths.append(path)
-        os.write(fd, b"hello" + line_ending + b"toto")
+        os.write(fd, b"hello in-toto")
         os.close(fd)
-
-      # Call in_toto_record start and stop and record artifacts as
-      # materials and products with line ending normalization on
-      in_toto_record_start(self.step_name, paths, self.key,
-          normalize_line_endings=True)
-      in_toto_record_stop(self.step_name, paths, self.key,
-          normalize_line_endings=True)
-      link = Metablock.load(self.link_name).signed
-
-      # Check that all three hashes in materials and products are equal
-      for artifact_dict in [link.materials, link.products]:
-        hash_dicts = list(artifact_dict.values())
-        self.assertTrue(hash_dicts[1:] == hash_dicts[:-1])
-
-    # Clean up
-    finally:
-      for path in paths:
+        # Windows will raise FileNotFoundError instead of NotADirectoryError
+        with self.assertRaises((NotADirectoryError, FileNotFoundError)):
+            in_toto_record_start(self.step_name, [], self.key)
+            in_toto_record_stop(
+                self.step_name, [], self.key, metadata_directory=path
+            )
         os.remove(path)
 
-  def test_nonexistent_directory(self):
-    """Test record stop with nonexistent metadata directory"""
-    with self.assertRaises(FileNotFoundError):
-      in_toto_record_start(self.step_name, [], self.key)
-      in_toto_record_stop(self.step_name, [], self.key,
-          metadata_directory='nonexistentDir')
-
-  def test_not_a_directory(self):
-    """Test record stop, passed metadata directory is not a dir"""
-    fd, path = tempfile.mkstemp()
-    os.write(fd, b"hello in-toto")
-    os.close(fd)
-    # Windows will raise FileNotFoundError instead of NotADirectoryError
-    with self.assertRaises((NotADirectoryError, FileNotFoundError)):
-      in_toto_record_start(self.step_name, [], self.key)
-      in_toto_record_stop(self.step_name, [], self.key,
-          metadata_directory=path)
-    os.remove(path)
-
-  @unittest.skipIf(os.name == 'nt', "chmod doesn't work properly on Windows")
-  def test_read_only_metadata_directory(self):
-    """Test record stop with read only metadata directory"""
-    tmp_dir = os.path.realpath(tempfile.mkdtemp())
-    # make the directory read only
-    os.chmod(tmp_dir, stat.S_IREAD)
-    with self.assertRaises(PermissionError):
-      in_toto_record_start(self.step_name, [], self.key)
-      in_toto_record_stop(self.step_name, [], self.key,
-          metadata_directory=tmp_dir)
-    os.rmdir(tmp_dir)
-
-  def test_created_metadata_using_dsse(self):
-    """Test record stop records created metadata with dsse."""
-    in_toto_record_start(self.step_name, [], self.key, use_dsse=True)
-    in_toto_record_stop(self.step_name, [self.test_product], self.key)
-
-    link_metadata = Envelope.load(self.link_name)
-    link_metadata.verify_signature(self.key)
-
-    link = link_metadata.get_payload()
-    self.assertEqual(list(link.products.keys()), [self.test_product])
-    os.remove(self.link_name)
-
-  def test_create_metadata_with_command_byproducts_environment(self):
-    """Test record stop records expected product. """
-    command = ["cp", "src", "dest"]
-    byproducts = {"stdout": "success", "stderr": "errors", "return-value": 0}
-    environment = {
-              "variables": "ENV_NAME=ENV_VALUE",
-              "filesystem": "<filesystem info>",
-              "workdir": "./"
+    @unittest.skipIf(os.name == "nt", "chmod doesn't work properly on Windows")
+    def test_read_only_metadata_directory(self):
+        """Test record stop with read only metadata directory"""
+        tmp_dir = os.path.realpath(tempfile.mkdtemp())
+        # make the directory read only
+        os.chmod(tmp_dir, stat.S_IREAD)
+        with self.assertRaises(PermissionError):
+            in_toto_record_start(self.step_name, [], self.key)
+            in_toto_record_stop(
+                self.step_name, [], self.key, metadata_directory=tmp_dir
+            )
+        os.rmdir(tmp_dir)
+
+    def test_created_metadata_using_dsse(self):
+        """Test record stop records created metadata with dsse."""
+        in_toto_record_start(self.step_name, [], self.key, use_dsse=True)
+        in_toto_record_stop(self.step_name, [self.test_product], self.key)
+
+        link_metadata = Envelope.load(self.link_name)
+        link_metadata.verify_signature(self.key)
+
+        link = link_metadata.get_payload()
+        self.assertEqual(list(link.products.keys()), [self.test_product])
+        os.remove(self.link_name)
+
+    def test_create_metadata_with_command_byproducts_environment(self):
+        """Test record stop records expected product."""
+        command = ["cp", "src", "dest"]
+        byproducts = {
+            "stdout": "success",
+            "stderr": "errors",
+            "return-value": 0,
+        }
+        environment = {
+            "variables": "ENV_NAME=ENV_VALUE",
+            "filesystem": "<filesystem info>",
+            "workdir": "./",
+        }
+
+        in_toto_record_start(
+            self.step_name, [], self.key, record_environment=True
+        )
+        in_toto_record_stop(
+            self.step_name,
+            [self.test_product],
+            self.key,
+            command=command,
+            byproducts=byproducts,
+            environment=environment,
+        )
+        link = Metablock.load(self.link_name)
+        self.assertEqual(link.signed.command, command)
+        self.assertDictEqual(link.signed.byproducts, byproducts)
+        self.assertDictEqual(link.signed.environment, environment)
+        os.remove(self.link_name)
+
+
+class TestInTotoMatchProducts(TmpDirMixin, unittest.TestCase):
+    """Basic tests for in_toto_match_products.
+
+    More comprehensive tests for `record_artifacts_as_dict` args exist above.
+    """
+
+    @classmethod
+    def setUpClass(cls):
+        # Create link with some products and some local artifacts in tmp dir:
+        # - 'foo' is only in products
+        # - 'quux' is not in products
+        # - 'baz' is in both, with different hashes
+        # - 'bar' is in both, with matching hashes
+        cls.set_up_test_dir()  # teardown is called implicitly
+
+        cls.link = Link(
+            products={
+                "foo": {
+                    "sha256": "8a51c03f1ff77c2b8e76da512070c23c5e69813d5c61732b3025199e5f0c14d5"
+                },
+                "bar": {
+                    "sha256": "bb97edb3507a35b119539120526d00da595f14575da261cd856389ecd89d3186"
+                },
+                "baz": {
+                    "sha256": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855"
+                },
             }
+        )
+        Path("bar").touch()
+        Path("baz").touch()
+        Path("quux").touch()
+
+    def test_check(self):
+        """Match local artifacts with link products for different kwargs."""
+        # Test data:
+        # [
+        #   (
+        #     <passed kwargs>,
+        #     <expected return values (only in products, not in products, differ)>
+        #   ),
+        #   ...
+        # ]
+        test_data = [
+            ({}, ({"foo"}, {"quux"}, {"bar"})),
+            (
+                {"exclude_patterns": ["ba*"]},
+                ({"foo", "bar", "baz"}, {"quux"}, set()),
+            ),
+            ({"paths": ["baz"]}, ({"foo", "bar"}, set(), set())),
+            (
+                {
+                    "paths": [str(Path("baz").absolute())],
+                    "lstrip_paths": [
+                        # NOTE: normalize lstrip path to match normalized artifact path
+                        # (see in-toto/in-toto#565)
+                        f"{Path('baz').absolute().parent}/".replace("\\", "/")
+                    ],
+                },
+                ({"foo", "bar"}, set(), set()),
+            ),
+        ]
+
+        for kwargs, expected_return_value in test_data:
+            self.assertTupleEqual(
+                in_toto_match_products(self.link, **kwargs),
+                expected_return_value,
+                f"unexpected result for **kwargs: {kwargs})",
+            )
 
-    in_toto_record_start(self.step_name, [], self.key, record_environment=True)
-    in_toto_record_stop(self.step_name, [self.test_product], self.key, command=command,
-      byproducts=byproducts, environment=environment)
-    link = Metablock.load(self.link_name)
-    self.assertEqual(link.signed.command, command)
-    self.assertDictEqual(link.signed.byproducts, byproducts)
-    self.assertDictEqual(link.signed.environment, environment)
-    os.remove(self.link_name)
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_settings.py` & `in_toto-2.0.0/tests/test_settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,17 +15,19 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Test in_toto/settings.py
 
 """
 import unittest
+
 import in_toto.settings
 
 
 class TestSettings(unittest.TestCase):
-  def test_debug_not_true(self):
-    """in_toto.settings.DEBUG should not be commited with True. """
-    self.assertFalse(in_toto.settings.DEBUG)
+    def test_debug_not_true(self):
+        """in_toto.settings.DEBUG should not be commited with True."""
+        self.assertFalse(in_toto.settings.DEBUG)
+
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/test_verifylib.py` & `in_toto-2.0.0/tests/test_verifylib.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,1673 +30,1793 @@
 import unittest
 from datetime import datetime
 from unittest.mock import patch
 
 import securesystemslib.exceptions
 import securesystemslib.gpg.functions
 from dateutil.relativedelta import relativedelta
-from securesystemslib.interface import (import_publickeys_from_file,
-    import_rsa_privatekey_from_file, import_rsa_publickey_from_file)
+from securesystemslib.gpg.constants import have_gpg
+from securesystemslib.interface import (
+    import_publickeys_from_file,
+    import_rsa_privatekey_from_file,
+    import_rsa_publickey_from_file,
+)
 
 import in_toto.exceptions
 import in_toto.settings
-from in_toto.exceptions import (BadReturnValueError, LayoutExpiredError,
-    RuleVerificationError, ThresholdVerificationError,
-    SignatureVerificationError)
-from in_toto.models.layout import (SUBLAYOUT_LINK_DIR_FORMAT, Inspection,
-    Layout, Step)
+from in_toto.exceptions import (
+    BadReturnValueError,
+    LayoutExpiredError,
+    RuleVerificationError,
+    SignatureVerificationError,
+    ThresholdVerificationError,
+)
+from in_toto.models.layout import (
+    SUBLAYOUT_LINK_DIR_FORMAT,
+    Inspection,
+    Layout,
+    Step,
+)
 from in_toto.models.link import FILENAME_FORMAT, Link
 from in_toto.models.metadata import Metablock
 from in_toto.rulelib import unpack_rule
-from securesystemslib.gpg.constants import have_gpg
-
-from in_toto.verifylib import (_raise_on_bad_retval, get_summary_link,
-    in_toto_verify, load_links_for_layout, run_all_inspections,
-    verify_all_item_rules, verify_allow_rule, verify_command_alignment,
-    verify_create_rule, verify_delete_rule, verify_disallow_rule,
-    verify_item_rules, verify_link_signature_thresholds, verify_match_rule,
-    verify_modify_rule, verify_require_rule, verify_sublayouts,
-    verify_threshold_constraints)
+from in_toto.verifylib import (
+    _raise_on_bad_retval,
+    get_summary_link,
+    in_toto_verify,
+    load_links_for_layout,
+    run_all_inspections,
+    verify_all_item_rules,
+    verify_allow_rule,
+    verify_command_alignment,
+    verify_create_rule,
+    verify_delete_rule,
+    verify_disallow_rule,
+    verify_item_rules,
+    verify_link_signature_thresholds,
+    verify_match_rule,
+    verify_modify_rule,
+    verify_require_rule,
+    verify_sublayouts,
+    verify_threshold_constraints,
+)
 from tests.common import GPGKeysMixin, TmpDirMixin
 
 
 class Test_RaiseOnBadRetval(unittest.TestCase):
-  """Tests internal function that raises an exception if the passed
-  "return_value" is not and integer and not zero. """
+    """Tests internal function that raises an exception if the passed
+    "return_value" is not and integer and not zero."""
 
-  def test_zero_return_value(self):
-    """Don't raise exception on zero return value. """
-    _raise_on_bad_retval(0)
-    _raise_on_bad_retval(0, "command")
-
-  def test_non_int_return_value(self):
-    """Raise exception on non-int return value. """
-    with self.assertRaises(BadReturnValueError):
-      _raise_on_bad_retval("bad retval")
-    with self.assertRaises(BadReturnValueError):
-      _raise_on_bad_retval("bad retval", "bad command")
-
-  def test_non_zero_return_value(self):
-    """Raise exception on non-zero return value. """
-    with self.assertRaises(BadReturnValueError):
-      _raise_on_bad_retval(1)
-    with self.assertRaises(BadReturnValueError):
-      _raise_on_bad_retval(-1, "bad command")
+    def test_zero_return_value(self):
+        """Don't raise exception on zero return value."""
+        _raise_on_bad_retval(0)
+        _raise_on_bad_retval(0, "command")
+
+    def test_non_int_return_value(self):
+        """Raise exception on non-int return value."""
+        with self.assertRaises(BadReturnValueError):
+            _raise_on_bad_retval("bad retval")
+        with self.assertRaises(BadReturnValueError):
+            _raise_on_bad_retval("bad retval", "bad command")
+
+    def test_non_zero_return_value(self):
+        """Raise exception on non-zero return value."""
+        with self.assertRaises(BadReturnValueError):
+            _raise_on_bad_retval(1)
+        with self.assertRaises(BadReturnValueError):
+            _raise_on_bad_retval(-1, "bad command")
 
 
 class TestRunAllInspections(unittest.TestCase, TmpDirMixin):
-  """Test verifylib.run_all_inspections(layout, persist_inspection_links)"""
+    """Test verifylib.run_all_inspections(layout, persist_inspection_links)"""
 
-  @classmethod
-  def setUpClass(self):
-    """
-    Create layout with dummy inpsection.
-    Create and change into temp test directory with dummy artifact."""
+    @classmethod
+    def setUpClass(self):
+        """
+        Create layout with dummy inpsection.
+        Create and change into temp test directory with dummy artifact."""
+
+        # find where the scripts directory is located.
+        scripts_directory = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "scripts"
+        )
+
+        # Create layout with one inspection
+        self.layout = Layout.read(
+            {
+                "_type": "layout",
+                "steps": [],
+                "inspect": [
+                    {
+                        "name": "touch-bar",
+                        "run": [
+                            "python",
+                            os.path.join(scripts_directory, "touch"),
+                            "bar",
+                        ],
+                    }
+                ],
+            }
+        )
 
-    # find where the scripts directory is located.
-    scripts_directory = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "scripts")
-
-    # Create layout with one inspection
-    self.layout = Layout.read({
-        "_type": "layout",
-        "steps": [],
-        "inspect": [{
-          "name": "touch-bar",
-          "run": ["python", os.path.join(scripts_directory, "touch"), "bar"],
-        }]
-      })
-
-    # Create directory where the verification will take place
-    self.set_up_test_dir()
-    with open("foo", "w", encoding="utf8") as f:
-      f.write("foo")
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def test_inpsection_artifacts_with_base_path_ignored(self):
-    """Create new dummy test dir and set as base path, must ignore. """
-    ignore_dir = os.path.realpath(tempfile.mkdtemp())
-    ignore_foo = os.path.join(ignore_dir, "ignore_foo")
-    with open(ignore_foo, "w", encoding="utf8") as f:
-      f.write("ignore foo")
-    in_toto.settings.ARTIFACT_BASE_PATH = ignore_dir
-
-    run_all_inspections(self.layout, True)
-    link = Metablock.load("touch-bar.link")
-    self.assertListEqual(list(link.signed.materials.keys()), ["foo"])
-    self.assertListEqual(sorted(list(link.signed.products.keys())), sorted(["foo", "bar"]))
-
-    in_toto.settings.ARTIFACT_BASE_PATH = None
-    shutil.rmtree(ignore_dir)
-
-  def test_inspection_fail_with_non_zero_retval(self):
-    """Test fail run inspections with non-zero return value. """
-    layout = Layout.read({
-        "_type": "layout",
-        "steps": [],
-        "inspect": [{
-          "name": "non-zero-inspection",
-          "run": ["python", "./scripts/expr", "1", "/", "0"],
-        }]
-    })
-    with self.assertRaises(BadReturnValueError):
-      run_all_inspections(layout, True)
-
-  def test_inspection_persistence_false(self):
-    """Test metadata link file non-persistence"""
-    if os.path.exists("touch-bar.link"):
-      os.remove("touch-bar.link")
-    run_all_inspections(self.layout, False)
-    self.assertFalse(os.path.exists("touch-bar.link"))
-
-  def test_inspeciton_persistence_true(self):
-    run_all_inspections(self.layout, True)
-    self.assertTrue(os.path.exists("touch-bar.link"))
+        # Create directory where the verification will take place
+        self.set_up_test_dir()
+        with open("foo", "w", encoding="utf8") as f:
+            f.write("foo")
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_inpsection_artifacts_with_base_path_ignored(self):
+        """Create new dummy test dir and set as base path, must ignore."""
+        ignore_dir = os.path.realpath(tempfile.mkdtemp())
+        ignore_foo = os.path.join(ignore_dir, "ignore_foo")
+        with open(ignore_foo, "w", encoding="utf8") as f:
+            f.write("ignore foo")
+        in_toto.settings.ARTIFACT_BASE_PATH = ignore_dir
+
+        run_all_inspections(self.layout, True)
+        link = Metablock.load("touch-bar.link")
+        self.assertListEqual(list(link.signed.materials.keys()), ["foo"])
+        self.assertListEqual(
+            sorted(list(link.signed.products.keys())), sorted(["foo", "bar"])
+        )
+
+        in_toto.settings.ARTIFACT_BASE_PATH = None
+        shutil.rmtree(ignore_dir)
+
+    def test_inspection_fail_with_non_zero_retval(self):
+        """Test fail run inspections with non-zero return value."""
+        layout = Layout.read(
+            {
+                "_type": "layout",
+                "steps": [],
+                "inspect": [
+                    {
+                        "name": "non-zero-inspection",
+                        "run": ["python", "./scripts/expr", "1", "/", "0"],
+                    }
+                ],
+            }
+        )
+        with self.assertRaises(BadReturnValueError):
+            run_all_inspections(layout, True)
+
+    def test_inspection_persistence_false(self):
+        """Test metadata link file non-persistence"""
+        if os.path.exists("touch-bar.link"):
+            os.remove("touch-bar.link")
+        run_all_inspections(self.layout, False)
+        self.assertFalse(os.path.exists("touch-bar.link"))
+
+    def test_inspeciton_persistence_true(self):
+        run_all_inspections(self.layout, True)
+        self.assertTrue(os.path.exists("touch-bar.link"))
 
 
 class TestVerifyCommandAlignment(unittest.TestCase):
-  """Test verifylib.verify_command_alignment(command, expected_command)"""
+    """Test verifylib.verify_command_alignment(command, expected_command)"""
 
-  def setUp(self):
-    self.command = ["vi", "file1", "file2"]
+    def setUp(self):
+        self.command = ["vi", "file1", "file2"]
 
-  def test_commands_align(self):
-    """Cmd and expected cmd are equal, passes. """
-    expected_command = ["vi", "file1", "file2"]
-    verify_command_alignment(self.command, expected_command)
-
-  def test_commands_do_not_fully_align_log_warning(self):
-    """Cmd and expected cmd differ slightly. """
-    expected_command = ["/usr/bin/vi", "file1", "file2"]
-
-    with patch("in_toto.verifylib.LOG") as mock_logging:
-      verify_command_alignment(self.command, expected_command)
-      mock_logging.warning.assert_called_with("Run command '{0}'"
-          " differs from expected command '{1}'"
-          .format(self.command, expected_command))
-
-  def test_commands_do_not_align_at_all_log_warning(self):
-    """Cmd and expected cmd differ completely. """
-    expected_command = ["make install"]
-
-    with patch("in_toto.verifylib.LOG") as mock_logging:
-      verify_command_alignment(self.command, expected_command)
-      mock_logging.warning.assert_called_with("Run command '{0}'"
-          " differs from expected command '{1}'"
-          .format(self.command, expected_command))
+    def test_commands_align(self):
+        """Cmd and expected cmd are equal, passes."""
+        expected_command = ["vi", "file1", "file2"]
+        verify_command_alignment(self.command, expected_command)
+
+    def test_commands_do_not_fully_align_log_warning(self):
+        """Cmd and expected cmd differ slightly."""
+        expected_command = ["/usr/bin/vi", "file1", "file2"]
+
+        with patch("in_toto.verifylib.LOG") as mock_logging:
+            verify_command_alignment(self.command, expected_command)
+            mock_logging.warning.assert_called_with(
+                "Run command '{0}'"
+                " differs from expected command '{1}'".format(
+                    self.command, expected_command
+                )
+            )
+
+    def test_commands_do_not_align_at_all_log_warning(self):
+        """Cmd and expected cmd differ completely."""
+        expected_command = ["make install"]
+
+        with patch("in_toto.verifylib.LOG") as mock_logging:
+            verify_command_alignment(self.command, expected_command)
+            mock_logging.warning.assert_called_with(
+                "Run command '{0}'"
+                " differs from expected command '{1}'".format(
+                    self.command, expected_command
+                )
+            )
 
 
 class TestVerifyRule(unittest.TestCase):
-  """Table driven tests for individual rule verification functions. """
+    """Table driven tests for individual rule verification functions."""
+
+    def test_verify_delete_rule(self):
+        """Test verifylib.verify_delete_rule."""
+        test_data_keys = [
+            "rule pattern",
+            "artifact queue",
+            "materials",
+            "products",
+            "expected",
+        ]
+        test_cases = [
+            # Consume deleted artifact
+            ["foo", {"foo"}, {"foo"}, set(), {"foo"}],
+            # Consume multiple deleted artifacts with wildcard
+            ["*", {"foo", "bar"}, {"foo", "bar"}, set(), {"foo", "bar"}],
+            # Don't consume created artifact (in products only)
+            ["foo", {"foo"}, set(), {"foo"}, set()],
+            # Don't consume artifact that's not in materials or products
+            # NOTE: In real life this shouldn't be in the queue either
+            ["foo", {"foo"}, set(), set(), set()],
+            # Don't consume deleted but not queued artifact
+            ["foo", set(), {"foo"}, set(), set()],
+            # Don't consume deleted but not matched artifact
+            ["bar", {"foo"}, {"foo"}, set(), set()],
+        ]
+
+        for i, test_data in enumerate(test_cases):
+            pattern, queue, materials, products, expected = test_data
+            result = verify_delete_rule(pattern, queue, materials, products)
+            self.assertSetEqual(
+                result,
+                expected,
+                "test {}: {}".format(i, dict(zip(test_data_keys, test_data))),
+            )
 
-  def test_verify_delete_rule(self):
-    """Test verifylib.verify_delete_rule. """
-    test_data_keys = [
-        "rule pattern", "artifact queue", "materials", "products", "expected"]
-    test_cases = [
-      # Consume deleted artifact
-      ["foo", {"foo"}, {"foo"}, set(), {"foo"}],
-      # Consume multiple deleted artifacts with wildcard
-      ["*", {"foo", "bar"}, {"foo", "bar"}, set(), {"foo", "bar"}],
-      # Don't consume created artifact (in products only)
-      ["foo", {"foo"}, set(), {"foo"}, set()],
-      # Don't consume artifact that's not in materials or products
-      # NOTE: In real life this shouldn't be in the queue either
-      ["foo", {"foo"}, set(), set(), set()],
-      # Don't consume deleted but not queued artifact
-      ["foo", set(), {"foo"}, set(), set()],
-      # Don't consume deleted but not matched artifact
-      ["bar", {"foo"}, {"foo"}, set(), set()]
-    ]
-
-    for i, test_data in enumerate(test_cases):
-      pattern, queue, materials, products, expected = test_data
-      result = verify_delete_rule(pattern, queue, materials, products)
-      self.assertSetEqual(result, expected,
-          "test {}: {}".format(i, dict(zip(test_data_keys, test_data))))
-
-
-  def test_verify_create_rule(self):
-    """Test verifylib.verify_create_rule. """
-    test_data_keys = [
-        "rule pattern", "artifact queue", "materials", "products", "expected"]
-    test_cases = [
-      # Consume created artifact
-      ["foo", {"foo"}, set(), {"foo"}, {"foo"}],
-      # Consume multiple created artifacts with wildcard
-      ["*", {"foo", "bar"}, set(), {"foo", "bar"}, {"foo", "bar"}],
-      # Don't consume deleted artifact (in materials only)
-      ["foo", {"foo"}, {"foo"}, set(), set()],
-      # Don't consume artifact that's not in materials or products
-      # NOTE: In real life this shouldn't be in the queue either
-      ["foo", {"foo"}, set(), set(), set()],
-      # Don't consume created but not queued artifact
-      ["foo", set(), set(), {"foo"}, set()],
-      # Don't consume created but not matched artifact
-      ["bar", {"foo"}, set(), {"foo"}, set()]
-    ]
-
-    for i, test_data in enumerate(test_cases):
-      pattern, queue, materials, products, expected = test_data
-      result = verify_create_rule(pattern, queue, materials, products)
-      self.assertSetEqual(result, expected,
-          "test {}: {}".format(i, dict(zip(test_data_keys, test_data))))
-
-
-  def test_verify_modify_rule(self):
-    """Test verifylib.verify_modify_rule. """
-    sha_a = "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
-    sha_b = "155c693a6b7481f48626ebfc545f05236df679f0099225d6d0bc472e6dd21155"
-
-    test_data_keys = [
-        "rule pattern", "artifact queue", "materials", "products", "expected"]
-    test_cases = [
-      # Consume modified artifact
-      ["foo", {"foo"}, {"foo": {"sha256": sha_a}}, {"foo": {"sha256": sha_b}},
-          {"foo"}],
-      # Consume multiple modified artifacts with wildcard
-      ["*", {"foo", "bar"},
-          {"foo": {"sha256": sha_a}, "bar": {"sha256": sha_a}},
-          {"foo": {"sha256": sha_b}, "bar": {"sha256": sha_b}},
-          {"foo", "bar"}],
-      # Don't consume unmodified artifact
-      ["foo", {"foo"}, {"foo": {"sha256": sha_a}}, {"foo": {"sha256": sha_a}},
-          set()],
-      # Don't consume artifact that's not in materials or products
-      # NOTE: In real life this shouldn't be in the queue either
-      ["foo", {"foo"}, {}, {}, set()],
-      # Don't consume modified but not queued artifact
-      ["foo", set(), {"foo": {"sha256": sha_a}}, {"foo": {"sha256": sha_b}},
-          set()],
-      # Don't consume modified but not matched artifact
-      ["bar", {"foo"}, {"foo": {"sha256": sha_a}}, {"foo": {"sha256": sha_b}},
-          set()],
-    ]
-
-    for i, test_data in enumerate(test_cases):
-      pattern, queue, materials, products, expected = test_data
-      result = verify_modify_rule(pattern, queue, materials, products)
-      self.assertSetEqual(result, expected,
-          "test {}: {}".format(i, dict(zip(test_data_keys, test_data))))
-
-
-  def test_verify_allow_rule(self):
-    """Test verifylib.verify_allow_rule. """
-    test_data_keys = ["rule pattern", "artifact queue", "expected"]
-    test_cases = [
-      # Consume allowed artifact
-      ["foo", {"foo"}, {"foo"}],
-      # Consume multiple allowed artifacts with wildcard
-      ["*", {"foo", "bar"}, {"foo", "bar"}],
-      # Consume multiple allowed artifacts with wildcard 2
-      ["foo*", {"foo", "foobar", "bar"}, {"foo", "foobar"}],
-      # Don't consume unmatched artifacts
-      ["bar", {"foo"}, set()],
-      # Don't consume artifacts if nothing is in the queue
-      ["foo", set(), set()],
-
-    ]
-    for i, test_data in enumerate(test_cases):
-      pattern, queue, expected = test_data
-      result = verify_allow_rule(pattern, queue)
-      self.assertSetEqual(result, expected,
-          "test {}: {}".format(i, dict(zip(test_data_keys, test_data))))
-
-
-  def test_verify_disallow_rule(self):
-    """Test verifylib.verify_disallow_rule. """
-    test_data_keys = ["rule pattern", "artifact queue"]
-    test_cases = [
-      # Foo disallowed, raise
-      ["foo", {"foo"}, True],
-      # All disallowed, raise
-      ["*", {"foo", "bar"}, True],
-      # Foo disallowed, but only bar there, don't raise
-      ["foo", {"bar"}, False],
-      # All disallowed, but no artifacts, don't raise
-      ["*", {}, False]
-    ]
-
-    for i, test_data in enumerate(test_cases):
-      pattern, queue, should_raise = test_data
-
-      msg = "test {}: {}".format(i, dict(zip(test_data_keys, test_data)))
-      exception = None
-
-      try:
-        verify_disallow_rule(pattern, queue)
-      except RuleVerificationError as e:
-        exception = e
-
-      if should_raise and not exception:
-        self.fail("Expected 'RuleVerificationError'\n{}".format(msg))
-
-      if exception and not should_raise:
-        self.fail("Unexpected {}\n{}".format(exception, msg))
-
-
-  def test_verify_require_rule(self):
-    """Test verifylib.verify_require_rule. """
-    test_data_keys = ["rule pattern", "artifact queue"]
-    test_cases = [
-      # Foo required, pass
-      ["foo", {"foo"}, False],
-      # Foo is required, but only bar there, blow up
-      ["foo", {"bar"}, True],
-      # A pattern is passed, which should be interpreted *literally*
-      ["*", {"*"}, False],
-      ["*", {"foo"}, True]
-      #
-    ]
-
-    for i, test_data in enumerate(test_cases):
-      pattern, queue, should_raise = test_data
-
-      msg = "test {}: {}".format(i, dict(zip(test_data_keys, test_data)))
-      exception = None
-
-      try:
-        verify_require_rule(pattern, queue)
-      except RuleVerificationError as e:
-        exception = e
+    def test_verify_create_rule(self):
+        """Test verifylib.verify_create_rule."""
+        test_data_keys = [
+            "rule pattern",
+            "artifact queue",
+            "materials",
+            "products",
+            "expected",
+        ]
+        test_cases = [
+            # Consume created artifact
+            ["foo", {"foo"}, set(), {"foo"}, {"foo"}],
+            # Consume multiple created artifacts with wildcard
+            ["*", {"foo", "bar"}, set(), {"foo", "bar"}, {"foo", "bar"}],
+            # Don't consume deleted artifact (in materials only)
+            ["foo", {"foo"}, {"foo"}, set(), set()],
+            # Don't consume artifact that's not in materials or products
+            # NOTE: In real life this shouldn't be in the queue either
+            ["foo", {"foo"}, set(), set(), set()],
+            # Don't consume created but not queued artifact
+            ["foo", set(), set(), {"foo"}, set()],
+            # Don't consume created but not matched artifact
+            ["bar", {"foo"}, set(), {"foo"}, set()],
+        ]
+
+        for i, test_data in enumerate(test_cases):
+            pattern, queue, materials, products, expected = test_data
+            result = verify_create_rule(pattern, queue, materials, products)
+            self.assertSetEqual(
+                result,
+                expected,
+                "test {}: {}".format(i, dict(zip(test_data_keys, test_data))),
+            )
 
-      if should_raise and not exception:
-        self.fail("Expected 'RuleVerificationError'\n{}".format(msg))
+    def test_verify_modify_rule(self):
+        """Test verifylib.verify_modify_rule."""
+        sha_a = (
+            "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
+        )
+        sha_b = (
+            "155c693a6b7481f48626ebfc545f05236df679f0099225d6d0bc472e6dd21155"
+        )
 
-      if exception and not should_raise:
-        self.fail("Unexpected {}\n{}".format(exception, msg))
+        test_data_keys = [
+            "rule pattern",
+            "artifact queue",
+            "materials",
+            "products",
+            "expected",
+        ]
+        test_cases = [
+            # Consume modified artifact
+            [
+                "foo",
+                {"foo"},
+                {"foo": {"sha256": sha_a}},
+                {"foo": {"sha256": sha_b}},
+                {"foo"},
+            ],
+            # Consume multiple modified artifacts with wildcard
+            [
+                "*",
+                {"foo", "bar"},
+                {"foo": {"sha256": sha_a}, "bar": {"sha256": sha_a}},
+                {"foo": {"sha256": sha_b}, "bar": {"sha256": sha_b}},
+                {"foo", "bar"},
+            ],
+            # Don't consume unmodified artifact
+            [
+                "foo",
+                {"foo"},
+                {"foo": {"sha256": sha_a}},
+                {"foo": {"sha256": sha_a}},
+                set(),
+            ],
+            # Don't consume artifact that's not in materials or products
+            # NOTE: In real life this shouldn't be in the queue either
+            ["foo", {"foo"}, {}, {}, set()],
+            # Don't consume modified but not queued artifact
+            [
+                "foo",
+                set(),
+                {"foo": {"sha256": sha_a}},
+                {"foo": {"sha256": sha_b}},
+                set(),
+            ],
+            # Don't consume modified but not matched artifact
+            [
+                "bar",
+                {"foo"},
+                {"foo": {"sha256": sha_a}},
+                {"foo": {"sha256": sha_b}},
+                set(),
+            ],
+        ]
+
+        for i, test_data in enumerate(test_cases):
+            pattern, queue, materials, products, expected = test_data
+            result = verify_modify_rule(pattern, queue, materials, products)
+            self.assertSetEqual(
+                result,
+                expected,
+                "test {}: {}".format(i, dict(zip(test_data_keys, test_data))),
+            )
+
+    def test_verify_allow_rule(self):
+        """Test verifylib.verify_allow_rule."""
+        test_data_keys = ["rule pattern", "artifact queue", "expected"]
+        test_cases = [
+            # Consume allowed artifact
+            ["foo", {"foo"}, {"foo"}],
+            # Consume multiple allowed artifacts with wildcard
+            ["*", {"foo", "bar"}, {"foo", "bar"}],
+            # Consume multiple allowed artifacts with wildcard 2
+            ["foo*", {"foo", "foobar", "bar"}, {"foo", "foobar"}],
+            # Don't consume unmatched artifacts
+            ["bar", {"foo"}, set()],
+            # Don't consume artifacts if nothing is in the queue
+            ["foo", set(), set()],
+        ]
+        for i, test_data in enumerate(test_cases):
+            pattern, queue, expected = test_data
+            result = verify_allow_rule(pattern, queue)
+            self.assertSetEqual(
+                result,
+                expected,
+                "test {}: {}".format(i, dict(zip(test_data_keys, test_data))),
+            )
 
+    def test_verify_disallow_rule(self):
+        """Test verifylib.verify_disallow_rule."""
+        test_data_keys = ["rule pattern", "artifact queue"]
+        test_cases = [
+            # Foo disallowed, raise
+            ["foo", {"foo"}, True],
+            # All disallowed, raise
+            ["*", {"foo", "bar"}, True],
+            # Foo disallowed, but only bar there, don't raise
+            ["foo", {"bar"}, False],
+            # All disallowed, but no artifacts, don't raise
+            ["*", {}, False],
+        ]
+
+        for i, test_data in enumerate(test_cases):
+            pattern, queue, should_raise = test_data
+
+            msg = "test {}: {}".format(i, dict(zip(test_data_keys, test_data)))
+            exception = None
+
+            try:
+                verify_disallow_rule(pattern, queue)
+            except RuleVerificationError as e:
+                exception = e
+
+            if should_raise and not exception:
+                self.fail("Expected 'RuleVerificationError'\n{}".format(msg))
+
+            if exception and not should_raise:
+                self.fail("Unexpected {}\n{}".format(exception, msg))
+
+    def test_verify_require_rule(self):
+        """Test verifylib.verify_require_rule."""
+        test_data_keys = ["rule pattern", "artifact queue"]
+        test_cases = [
+            # Foo required, pass
+            ["foo", {"foo"}, False],
+            # Foo is required, but only bar there, blow up
+            ["foo", {"bar"}, True],
+            # A pattern is passed, which should be interpreted *literally*
+            ["*", {"*"}, False],
+            ["*", {"foo"}, True]
+            #
+        ]
+
+        for i, test_data in enumerate(test_cases):
+            pattern, queue, should_raise = test_data
+
+            msg = "test {}: {}".format(i, dict(zip(test_data_keys, test_data)))
+            exception = None
+
+            try:
+                verify_require_rule(pattern, queue)
+            except RuleVerificationError as e:
+                exception = e
+
+            if should_raise and not exception:
+                self.fail("Expected 'RuleVerificationError'\n{}".format(msg))
+
+            if exception and not should_raise:
+                self.fail("Unexpected {}\n{}".format(exception, msg))
 
 
 class TestVerifyMatchRule(unittest.TestCase):
-  """Test verifylib.verify_match_rule(rule, artifact_queue, artifacts, links) """
+    """Test verifylib.verify_match_rule(rule, artifact_queue, artifacts, links)"""
 
-  def setUp(self):
-    """Setup artifact queues, artifacts dictionary and Link dictionary. """
+    def setUp(self):
+        """Setup artifact queues, artifacts dictionary and Link dictionary."""
 
-    # Dummy artifact hashes
-    self.sha256_foo = \
-        "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
-    self.sha256_foobar = \
-        "155c693a6b7481f48626ebfc545f05236df679f0099225d6d0bc472e6dd21155"
-    self.sha256_bar = \
-        "cfdaaf1ab2e4661952a9dec5e8fa3c360c1b06b1a073e8493a7c46d2af8c504b"
-    self.sha256_barfoo = \
-        "2036784917e49b7685c7c17e03ddcae4a063979aa296ee5090b5bb8f8aeafc5d"
-
-    # Link dictionary containing dummy artifacts related to Steps the rule is
-    # matched with (match destination).
-    self.materials = {
-      "foo": {"sha256": self.sha256_foo},
-      "foobar": {"sha256": self.sha256_foobar},
-      "sub/foo": {"sha256": self.sha256_foo},
-      "sub/foobar": {"sha256": self.sha256_foobar},
-      "lib/foo": {"sha256": self.sha256_foo},
-      "lib/foobar": {"sha256": self.sha256_foobar},
-      "lib/build/foo": {"sha256": self.sha256_foo},
-      "lib/build/foobar": {"sha256": self.sha256_foobar},
-    }
-    self.products = {
-      "bar": {"sha256": self.sha256_bar},
-      "barfoo": {"sha256": self.sha256_barfoo},
-      "sub/bar": {"sha256": self.sha256_bar},
-      "sub/barfoo": {"sha256": self.sha256_barfoo},
-      "sub/lib/bar": {"sha256": self.sha256_bar},
-      "sub/lib/barfoo": {"sha256": self.sha256_barfoo},
-      "build/bar": {"sha256": self.sha256_bar},
-      "build/barfoo": {"sha256": self.sha256_barfoo},
-    }
-
-    self.links = {
-        "dest-item": Link(
-            name="dest-item",
-            materials=self.materials,
-            products=self.products
-          ),
-    }
-
-
-  def test_verify_match_rule(self):
-    test_data_keys = [
-        "rule string", "artifacts queue", "source artifacts", "expected"]
-    test_cases = [
-      [
-        # Consume foo matching with dest material foo
-        "MATCH foo WITH MATERIALS FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"foo"}
-      ],
-      [
-        # Consume foo matching with dest product foo
-        "MATCH bar WITH PRODUCTS FROM dest-item",
-        set(self.products.keys()), self.products,
-        {"bar"}
-      ],
-      [
-        # Consume sub/foo matching with dest material foo
-        "MATCH foo IN sub WITH MATERIALS FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"sub/foo"}
-      ],
-      [
-        # Consume sub/foo matching with dest material foo (ignore trailing /)
-        "MATCH foo IN sub/ WITH MATERIALS FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"sub/foo"}
-      ],
-      [
-        # Consume sub/bar matching with dest product bar
-        "MATCH bar IN sub WITH PRODUCTS FROM dest-item",
-        set(self.products.keys()), self.products,
-        {"sub/bar"}
-      ],
-      [
-        # Consume foo matching with dest material sub/foo
-        "MATCH foo WITH MATERIALS IN sub FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"foo"}
-      ],
-      [
-        # Consume bar matching with dest product sub/bar
-        "MATCH bar WITH PRODUCTS IN sub FROM dest-item",
-        set(self.products.keys()), self.products,
-        {"bar"}
-      ],
-      [
-        # Consume bar matching with dest product sub/bar (ignore trailing /)
-        "MATCH bar WITH PRODUCTS IN sub/ FROM dest-item",
-        set(self.products.keys()), self.products,
-        {"bar"}
-      ],
-      [
-        # Consume foo* matching with dest material foo*
-        "MATCH foo* WITH MATERIALS FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"foo", "foobar"}
-      ],
-      [
-        # Consume sub/foo* matching with dest material foo*
-        "MATCH foo* IN sub WITH MATERIALS FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"sub/foo", "sub/foobar"}
-      ],
-      [
-        # Consume bar* matching with dest product bar*
-        "MATCH bar* WITH PRODUCTS FROM dest-item",
-        set(self.products.keys()), self.products,
-        {"bar", "barfoo"}
-      ],
-      [
-        # Consume bar* matching with dest product sub/bar*
-        "MATCH bar* WITH PRODUCTS IN sub FROM dest-item",
-        set(self.products.keys()), self.products,
-        {"bar", "barfoo"}
-      ],
-      [
-        # Don't consume (empty queue)
-        "MATCH foo WITH MATERIALS FROM dest-item",
-        set(), self.materials,
-        set()
-      ],
-      [
-        # Don't consume (no destination artifact)
-        "MATCH foo WITH PRODUCTS FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        set()
-      ],
-      [
-        # Don't consume (non-matching hashes)
-        "MATCH foo WITH MATERIALS FROM dest-item",
-        {"foo"}, {"foo": {"sha256": "deadbeef"}},
-        set()
-      ],
-      [
-        # Don't consume (missing link)
-        "MATCH foo WITH MATERIALS FROM dest-item-missing-link",
-        set(self.materials.keys()), self.materials,
-        set()
-      ],
-      [
-        # Ensures the sub/bar file matches the product file in the sub folder
-        # from the dest-item step.
-        "MATCH bar IN sub WITH PRODUCTS IN sub FROM dest-item",
-        set(self.products.keys()), self.products,
-        {"sub/bar"}
-      ],
-      [
-        # Ensures the sub/bar and sub/barfoo files matches the product
-        # files in the sub folder from the dest-item step.
-        "MATCH bar* IN sub WITH PRODUCTS IN sub/ FROM dest-item",
-        set(self.products.keys()), self.products,
-        {"sub/bar", "sub/barfoo"}
-      ],
-      [
-        # Ensure the sub/bar file matches the product file in the
-        # sub/lib folder from the dest-item step.
-        "MATCH bar IN sub WITH PRODUCTS IN sub/lib FROM dest-item",
-        set(self.products.keys()), self.products,
-        {"sub/bar"}
-      ],
-      [
-        # Do not consume. Missing link
-        "MATCH bar IN sub WITH PRODUCTS IN sub FROM dest-item-missing-link",
-        set(self.products.keys()), self.products,
-        set()
-      ],
-      [
-        # Ensures the sub/foo file matches the material file in the
-        # lib folder from the dest-item step.
-        "MATCH foo IN sub WITH MATERIALS IN lib FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"sub/foo"}
-      ],
-      [
-        # Ensures any sub/foo and sub/foobar files matches material
-        # files in the lib folder from the dest-item step.
-        "MATCH foo* IN sub WITH MATERIALS IN lib/ FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"sub/foo", "sub/foobar"}
-      ],
-      [
-        # Ensures the sub/foo file matches the material files in the lib/build
-        # the lib/build folder from the dest-item step.
-        "MATCH foo IN sub WITH MATERIALS IN lib/build FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"sub/foo"}
-      ],
-      [
-        # Ensures the sub/foo and sub/foobar files matches the material files
-        # in the lib/build folder from the dest-item step.
-        "MATCH foo* IN sub WITH MATERIALS IN lib/build FROM dest-item",
-        set(self.materials.keys()), self.materials,
-        {"sub/foo", "sub/foobar"}
-      ]
-    ]
-
-    for i, test_data in enumerate(test_cases):
-      rule_string, queue, source_artifacts, expected = test_data
-
-      # Generate rule data from rule string
-      rule_data = unpack_rule(shlex.split(rule_string))
-
-      result = verify_match_rule(
-          rule_data, queue, source_artifacts, self.links)
-
-      self.assertSetEqual(result, expected,
-          "'result': {}\n test {}: {}, 'links':{}".format(result,
-          i, dict(zip(test_data_keys, test_data)), self.links))
+        # Dummy artifact hashes
+        self.sha256_foo = (
+            "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
+        )
+        self.sha256_foobar = (
+            "155c693a6b7481f48626ebfc545f05236df679f0099225d6d0bc472e6dd21155"
+        )
+        self.sha256_bar = (
+            "cfdaaf1ab2e4661952a9dec5e8fa3c360c1b06b1a073e8493a7c46d2af8c504b"
+        )
+        self.sha256_barfoo = (
+            "2036784917e49b7685c7c17e03ddcae4a063979aa296ee5090b5bb8f8aeafc5d"
+        )
 
+        # Link dictionary containing dummy artifacts related to Steps the rule is
+        # matched with (match destination).
+        self.materials = {
+            "foo": {"sha256": self.sha256_foo},
+            "foobar": {"sha256": self.sha256_foobar},
+            "sub/foo": {"sha256": self.sha256_foo},
+            "sub/foobar": {"sha256": self.sha256_foobar},
+            "lib/foo": {"sha256": self.sha256_foo},
+            "lib/foobar": {"sha256": self.sha256_foobar},
+            "lib/build/foo": {"sha256": self.sha256_foo},
+            "lib/build/foobar": {"sha256": self.sha256_foobar},
+        }
+        self.products = {
+            "bar": {"sha256": self.sha256_bar},
+            "barfoo": {"sha256": self.sha256_barfoo},
+            "sub/bar": {"sha256": self.sha256_bar},
+            "sub/barfoo": {"sha256": self.sha256_barfoo},
+            "sub/lib/bar": {"sha256": self.sha256_bar},
+            "sub/lib/barfoo": {"sha256": self.sha256_barfoo},
+            "build/bar": {"sha256": self.sha256_bar},
+            "build/barfoo": {"sha256": self.sha256_barfoo},
+        }
+
+        self.links = {
+            "dest-item": Link(
+                name="dest-item",
+                materials=self.materials,
+                products=self.products,
+            ),
+        }
+
+    def test_verify_match_rule(self):
+        test_data_keys = [
+            "rule string",
+            "artifacts queue",
+            "source artifacts",
+            "expected",
+        ]
+        test_cases = [
+            [
+                # Consume foo matching with dest material foo
+                "MATCH foo WITH MATERIALS FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"foo"},
+            ],
+            [
+                # Consume foo matching with dest product foo
+                "MATCH bar WITH PRODUCTS FROM dest-item",
+                set(self.products.keys()),
+                self.products,
+                {"bar"},
+            ],
+            [
+                # Consume sub/foo matching with dest material foo
+                "MATCH foo IN sub WITH MATERIALS FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"sub/foo"},
+            ],
+            [
+                # Consume sub/foo matching with dest material foo (ignore trailing /)
+                "MATCH foo IN sub/ WITH MATERIALS FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"sub/foo"},
+            ],
+            [
+                # Consume sub/bar matching with dest product bar
+                "MATCH bar IN sub WITH PRODUCTS FROM dest-item",
+                set(self.products.keys()),
+                self.products,
+                {"sub/bar"},
+            ],
+            [
+                # Consume foo matching with dest material sub/foo
+                "MATCH foo WITH MATERIALS IN sub FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"foo"},
+            ],
+            [
+                # Consume bar matching with dest product sub/bar
+                "MATCH bar WITH PRODUCTS IN sub FROM dest-item",
+                set(self.products.keys()),
+                self.products,
+                {"bar"},
+            ],
+            [
+                # Consume bar matching with dest product sub/bar (ignore trailing /)
+                "MATCH bar WITH PRODUCTS IN sub/ FROM dest-item",
+                set(self.products.keys()),
+                self.products,
+                {"bar"},
+            ],
+            [
+                # Consume foo* matching with dest material foo*
+                "MATCH foo* WITH MATERIALS FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"foo", "foobar"},
+            ],
+            [
+                # Consume sub/foo* matching with dest material foo*
+                "MATCH foo* IN sub WITH MATERIALS FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"sub/foo", "sub/foobar"},
+            ],
+            [
+                # Consume bar* matching with dest product bar*
+                "MATCH bar* WITH PRODUCTS FROM dest-item",
+                set(self.products.keys()),
+                self.products,
+                {"bar", "barfoo"},
+            ],
+            [
+                # Consume bar* matching with dest product sub/bar*
+                "MATCH bar* WITH PRODUCTS IN sub FROM dest-item",
+                set(self.products.keys()),
+                self.products,
+                {"bar", "barfoo"},
+            ],
+            [
+                # Don't consume (empty queue)
+                "MATCH foo WITH MATERIALS FROM dest-item",
+                set(),
+                self.materials,
+                set(),
+            ],
+            [
+                # Don't consume (no destination artifact)
+                "MATCH foo WITH PRODUCTS FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                set(),
+            ],
+            [
+                # Don't consume (non-matching hashes)
+                "MATCH foo WITH MATERIALS FROM dest-item",
+                {"foo"},
+                {"foo": {"sha256": "deadbeef"}},
+                set(),
+            ],
+            [
+                # Don't consume (missing link)
+                "MATCH foo WITH MATERIALS FROM dest-item-missing-link",
+                set(self.materials.keys()),
+                self.materials,
+                set(),
+            ],
+            [
+                # Ensures the sub/bar file matches the product file in the sub folder
+                # from the dest-item step.
+                "MATCH bar IN sub WITH PRODUCTS IN sub FROM dest-item",
+                set(self.products.keys()),
+                self.products,
+                {"sub/bar"},
+            ],
+            [
+                # Ensures the sub/bar and sub/barfoo files matches the product
+                # files in the sub folder from the dest-item step.
+                "MATCH bar* IN sub WITH PRODUCTS IN sub/ FROM dest-item",
+                set(self.products.keys()),
+                self.products,
+                {"sub/bar", "sub/barfoo"},
+            ],
+            [
+                # Ensure the sub/bar file matches the product file in the
+                # sub/lib folder from the dest-item step.
+                "MATCH bar IN sub WITH PRODUCTS IN sub/lib FROM dest-item",
+                set(self.products.keys()),
+                self.products,
+                {"sub/bar"},
+            ],
+            [
+                # Do not consume. Missing link
+                "MATCH bar IN sub WITH PRODUCTS IN sub FROM dest-item-missing-link",
+                set(self.products.keys()),
+                self.products,
+                set(),
+            ],
+            [
+                # Ensures the sub/foo file matches the material file in the
+                # lib folder from the dest-item step.
+                "MATCH foo IN sub WITH MATERIALS IN lib FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"sub/foo"},
+            ],
+            [
+                # Ensures any sub/foo and sub/foobar files matches material
+                # files in the lib folder from the dest-item step.
+                "MATCH foo* IN sub WITH MATERIALS IN lib/ FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"sub/foo", "sub/foobar"},
+            ],
+            [
+                # Ensures the sub/foo file matches the material files in the lib/build
+                # the lib/build folder from the dest-item step.
+                "MATCH foo IN sub WITH MATERIALS IN lib/build FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"sub/foo"},
+            ],
+            [
+                # Ensures the sub/foo and sub/foobar files matches the material files
+                # in the lib/build folder from the dest-item step.
+                "MATCH foo* IN sub WITH MATERIALS IN lib/build FROM dest-item",
+                set(self.materials.keys()),
+                self.materials,
+                {"sub/foo", "sub/foobar"},
+            ],
+        ]
+
+        for i, test_data in enumerate(test_cases):
+            rule_string, queue, source_artifacts, expected = test_data
+
+            # Generate rule data from rule string
+            rule_data = unpack_rule(shlex.split(rule_string))
+
+            result = verify_match_rule(
+                rule_data, queue, source_artifacts, self.links
+            )
+
+            self.assertSetEqual(
+                result,
+                expected,
+                "'result': {}\n test {}: {}, 'links':{}".format(
+                    result, i, dict(zip(test_data_keys, test_data)), self.links
+                ),
+            )
 
 
 class TestVerifyItemRules(unittest.TestCase):
-  """Test verifylib.verify_item_rules(source_name, source_type, rules, links)"""
+    """Test verifylib.verify_item_rules(source_name, source_type, rules, links)"""
 
-  def setUp(self):
-    self.item_name = "item"
-    self.sha256_1 = \
-        "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
-    self.sha256_2 = \
-        "cfdaaf1ab2e4661952a9dec5e8fa3c360c1b06b1a073e8493a7c46d2af8c504b"
-
-    self.links = {
-      "item": Link(name="item",
-        materials={
-            "foo": {"sha256": self.sha256_1},
-            "foobar": {"sha256": self.sha256_1},
-            "bar": {"sha256": self.sha256_1},
-            "foobarbaz": {"sha256": self.sha256_1}
-        },
-        products={
-            "baz" : {"sha256": self.sha256_1},
-            "foo": {"sha256": self.sha256_1},
-            "bar": {"sha256": self.sha256_2},
-            "foobarbaz": {"sha256": self.sha256_1}
+    def setUp(self):
+        self.item_name = "item"
+        self.sha256_1 = (
+            "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
+        )
+        self.sha256_2 = (
+            "cfdaaf1ab2e4661952a9dec5e8fa3c360c1b06b1a073e8493a7c46d2af8c504b"
+        )
+
+        self.links = {
+            "item": Link(
+                name="item",
+                materials={
+                    "foo": {"sha256": self.sha256_1},
+                    "foobar": {"sha256": self.sha256_1},
+                    "bar": {"sha256": self.sha256_1},
+                    "foobarbaz": {"sha256": self.sha256_1},
+                },
+                products={
+                    "baz": {"sha256": self.sha256_1},
+                    "foo": {"sha256": self.sha256_1},
+                    "bar": {"sha256": self.sha256_2},
+                    "foobarbaz": {"sha256": self.sha256_1},
+                },
+            )
         }
-      )
-    }
 
-  def test_pass_rules_with_each_rule_type(self):
-    """Pass with list of rules of each rule type. """
-    rules = [
-      ["DELETE", "foobar"],
-      ["REQUIRE", "foobarbaz"],
-      ["CREATE", "baz"],
-      ["MODIFY", "bar"],
-      ["MATCH", "foo", "WITH", "MATERIALS", "FROM", "item"], # match with self
-      ["ALLOW", "foobarbaz"],
-      ["DISALLOW", "*"],
-    ]
-    for source_type in ["materials", "products"]:
-      verify_item_rules(self.item_name, source_type, rules, self.links)
-
-  def test_fail_disallow_not_consumed_artifacts(self):
-    """Fail with not consumed artifacts and terminal DISALLOW. """
-    rules = [
-      ["DISALLOW", "*"],
-    ]
-    with self.assertRaises(RuleVerificationError):
-      verify_item_rules(self.item_name, "materials", rules, self.links)
-
-  def test_fail_wrong_source_type(self):
-    """Fail with wrong source_type."""
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      verify_item_rules(self.item_name, "artifacts", [], self.links)
-
-  def test_pass_not_consumed_artifacts(self):
-    """Pass with not consumed artifacts and implicit terminal ALLOW * """
-    verify_item_rules(self.item_name, "materials", [], self.links)
+    def test_pass_rules_with_each_rule_type(self):
+        """Pass with list of rules of each rule type."""
+        rules = [
+            ["DELETE", "foobar"],
+            ["REQUIRE", "foobarbaz"],
+            ["CREATE", "baz"],
+            ["MODIFY", "bar"],
+            [
+                "MATCH",
+                "foo",
+                "WITH",
+                "MATERIALS",
+                "FROM",
+                "item",
+            ],  # match with self
+            ["ALLOW", "foobarbaz"],
+            ["DISALLOW", "*"],
+        ]
+        for source_type in ["materials", "products"]:
+            verify_item_rules(self.item_name, source_type, rules, self.links)
+
+    def test_fail_disallow_not_consumed_artifacts(self):
+        """Fail with not consumed artifacts and terminal DISALLOW."""
+        rules = [
+            ["DISALLOW", "*"],
+        ]
+        with self.assertRaises(RuleVerificationError):
+            verify_item_rules(self.item_name, "materials", rules, self.links)
+
+    def test_fail_wrong_source_type(self):
+        """Fail with wrong source_type."""
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            verify_item_rules(self.item_name, "artifacts", [], self.links)
+
+    def test_pass_not_consumed_artifacts(self):
+        """Pass with not consumed artifacts and implicit terminal ALLOW *"""
+        verify_item_rules(self.item_name, "materials", [], self.links)
 
 
 class TestVerifyAllItemRules(unittest.TestCase):
-  """Test verifylib.verify_all_item_rules(items, links). """
+    """Test verifylib.verify_all_item_rules(items, links)."""
 
-  def setUp(self):
-    """Create a dummy supply chain with two steps one inspection and the
-    according link metadata:
+    def setUp(self):
+        """Create a dummy supply chain with two steps one inspection and the
+        according link metadata:
 
-    write-code (Step) ->  package (step) -> untar (Inspection)
+        write-code (Step) ->  package (step) -> untar (Inspection)
 
-    'write-code' creates an artifact foo
-    'package' creates foo.tar.gz and deletes foo
-    'untar' untars foo.tar.gz which results in foo.tar.gz and foo
+        'write-code' creates an artifact foo
+        'package' creates foo.tar.gz and deletes foo
+        'untar' untars foo.tar.gz which results in foo.tar.gz and foo
 
-    """
+        """
 
-    self.sha256_foo = \
-        "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
-    self.sha256_foo_tar = \
-        "93c3c35a039a6a3d53e81c5dbee4ebb684de57b7c8be11b8739fd35804a0e918"
-
-    self.steps = [
-        Step(name="write-code",
-            expected_products=[
-                ["CREATE", "foo"]
-            ],
-        ),
-        Step(name="package",
-            expected_materials=[
-                ["MATCH", "foo", "WITH", "PRODUCTS", "FROM", "write-code"]
-            ],
-            expected_products=[
-                ["CREATE", "foo.tar.gz"],
-                ["DELETE", "foo"]
-            ],
-        )
-    ]
-
-    self.inspections = [
-        Inspection(name="untar",
-            expected_materials=[
-                ["REQUIRE", "foo.tar.gz"],
-                ["MATCH", "foo.tar.gz", "WITH", "PRODUCTS", "FROM", "package"]
-            ],
-            expected_products=[
-                ["MATCH", "foo", "IN", "dir", "WITH", "PRODUCTS",
-                    "FROM", "write-code"]
-            ]
-        )
-    ]
-
-    self.links = {
-      "write-code" : Link(name="write-code",
-        products={
-            "foo": {
-                "sha256": self.sha256_foo
-            }
-        }
-      ),
-      "package" : Link(name="package",
-        materials={
-            "foo": {
-                "sha256": self.sha256_foo
-            }
-        },
-        products={
-            "foo.tar.gz": {
-                "sha256": self.sha256_foo_tar
-            }
+        self.sha256_foo = (
+            "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
+        )
+        self.sha256_foo_tar = (
+            "93c3c35a039a6a3d53e81c5dbee4ebb684de57b7c8be11b8739fd35804a0e918"
+        )
+
+        self.steps = [
+            Step(
+                name="write-code",
+                expected_products=[["CREATE", "foo"]],
+            ),
+            Step(
+                name="package",
+                expected_materials=[
+                    ["MATCH", "foo", "WITH", "PRODUCTS", "FROM", "write-code"]
+                ],
+                expected_products=[["CREATE", "foo.tar.gz"], ["DELETE", "foo"]],
+            ),
+        ]
+
+        self.inspections = [
+            Inspection(
+                name="untar",
+                expected_materials=[
+                    ["REQUIRE", "foo.tar.gz"],
+                    [
+                        "MATCH",
+                        "foo.tar.gz",
+                        "WITH",
+                        "PRODUCTS",
+                        "FROM",
+                        "package",
+                    ],
+                ],
+                expected_products=[
+                    [
+                        "MATCH",
+                        "foo",
+                        "IN",
+                        "dir",
+                        "WITH",
+                        "PRODUCTS",
+                        "FROM",
+                        "write-code",
+                    ]
+                ],
+            )
+        ]
+
+        self.links = {
+            "write-code": Link(
+                name="write-code", products={"foo": {"sha256": self.sha256_foo}}
+            ),
+            "package": Link(
+                name="package",
+                materials={"foo": {"sha256": self.sha256_foo}},
+                products={"foo.tar.gz": {"sha256": self.sha256_foo_tar}},
+            ),
+            "untar": Link(
+                name="untar",
+                materials={"foo.tar.gz": {"sha256": self.sha256_foo_tar}},
+                products={
+                    "dir/foo": {"sha256": self.sha256_foo},
+                },
+            ),
         }
-      ),
-        "untar" : Link(name="untar",
-          materials={
-              "foo.tar.gz": {
-                  "sha256": self.sha256_foo_tar
-              }
-          },
-          products={
-              "dir/foo": {
-                  "sha256": self.sha256_foo
-              },
-          }
-        )
-    }
-
-  def test_pass_verify_all_step_rules(self):
-    """Pass rule verification for dummy supply chain Steps. """
-    verify_all_item_rules(self.steps, self.links)
-
-  def test_pass_verify_all_inspection_rules(self):
-    """Pass rule verification for dummy supply chain Inspections. """
-    verify_all_item_rules(self.inspections, self.links)
+
+    def test_pass_verify_all_step_rules(self):
+        """Pass rule verification for dummy supply chain Steps."""
+        verify_all_item_rules(self.steps, self.links)
+
+    def test_pass_verify_all_inspection_rules(self):
+        """Pass rule verification for dummy supply chain Inspections."""
+        verify_all_item_rules(self.inspections, self.links)
 
 
 class TestInTotoVerify(unittest.TestCase, TmpDirMixin):
-  """
-  Tests verifylib.in_toto_verify(layout_path, layout_key_paths).
+    """
+    Tests verifylib.in_toto_verify(layout_path, layout_key_paths).
 
-  Uses in-toto demo supply chain link metadata files and basic layout for
-  verification.
+    Uses in-toto demo supply chain link metadata files and basic layout for
+    verification.
 
-  Copies the basic layout for different test scenarios:
-    - single-signed layout
-    - double-signed layout
-    - expired layout
-    - layout with failing link rule
-    - layout with failing step rule
-
-  """
-  @classmethod
-  def setUpClass(self):
-    """Creates and changes into temporary directory.
-    Copies demo files to temp dir...
-      - owner/functionary key pairs
-      - *.link metadata files
-      - layout template (not signed, no expiration date)
-      - final product
+    Copies the basic layout for different test scenarios:
+      - single-signed layout
+      - double-signed layout
+      - expired layout
+      - layout with failing link rule
+      - layout with failing step rule
 
-    ...and dumps various layouts for different test scenarios
     """
 
-    # Find demo files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    # find where the scripts directory is located.
-    scripts_directory = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "scripts")
-
-    # Create and change into temporary directory
-    self.set_up_test_dir()
-
-    # Copy demo files to temp dir
-    for fn in os.listdir(demo_files):
-      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
-
-    # copy scripts over
-    shutil.copytree(scripts_directory, "scripts")
-
-    # Load layout template
-    layout_template = Metablock.load("demo.layout.template")
-
-    # Store various layout paths to be used in tests
-    self.layout_single_signed_path = "single-signed.layout"
-    self.layout_double_signed_path = "double-signed.layout"
-    self.layout_bad_sig = "bad-sig.layout"
-    self.layout_expired_path = "expired.layout"
-    self.layout_failing_step_rule_path = "failing-step-rule.layout"
-    self.layout_failing_inspection_rule_path = "failing-inspection-rule.layout"
-    self.layout_failing_inspection_retval = "failing-inspection-retval.layout"
-    self.layout_no_steps_no_inspections = "no_steps_no_inspections.layout"
-
-    # Import layout signing keys
-    alice = import_rsa_privatekey_from_file("alice")
-    bob = import_rsa_privatekey_from_file("bob")
-    self.alice_path = "alice.pub"
-    self.bob_path = "bob.pub"
-
-    # dump single signed layout
-    layout = copy.deepcopy(layout_template)
-    layout.sign(alice)
-    layout.dump(self.layout_single_signed_path)
-
-    # dump double signed layout
-    layout = copy.deepcopy(layout_template)
-    layout.sign(alice)
-    layout.sign(bob)
-    layout.dump(self.layout_double_signed_path)
-
-    # dump layout with bad signature
-    layout = copy.deepcopy(layout_template)
-    layout.sign(alice)
-    layout.signed.readme = "this breaks the signature"
-    layout.dump(self.layout_bad_sig)
-
-    # dump expired layout
-    layout = copy.deepcopy(layout_template)
-    layout.signed.expires = (datetime.today() +
-        relativedelta(months=-1)).strftime("%Y-%m-%dT%H:%M:%SZ")
-    layout.sign(alice)
-    layout.dump(self.layout_expired_path)
-
-    # dump layout with failing step rule
-    layout = copy.deepcopy(layout_template)
-    layout.signed.steps[0].expected_products.insert(0,
-        ["DISALLOW", "*"])
-    layout.signed.steps[0].expected_products.insert(0,
-        ["MODIFY", "*"])
-    layout.sign(alice)
-    layout.dump(self.layout_failing_step_rule_path)
-
-    # dump layout with failing inspection rule
-    layout = copy.deepcopy(layout_template)
-    layout.signed.inspect[0].expected_materials.insert(0,
-        ["MODIFY", "*"])
-    layout.signed.inspect[0].expected_materials.append(
-        ["DISALLOW", "*"])
-    layout.sign(alice)
-    layout.dump(self.layout_failing_inspection_rule_path)
-
-    # dump layout with failing inspection retval
-    layout = copy.deepcopy(layout_template)
-    layout.signed.inspect[0].run = ["python", "./scripts/expr", "1", "/", "0"]
-    layout.sign(alice)
-    layout.dump(self.layout_failing_inspection_retval)
-
-    # dump empty layout
-    layout = Metablock(signed=Layout())
-    layout.sign(alice)
-    layout.dump(self.layout_no_steps_no_inspections)
-    self.alice = alice
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-
-  def test_verify_passing(self):
-    """Test pass verification of single-signed layout. """
-    layout = Metablock.load(self.layout_single_signed_path)
-    layout_key_dict = import_publickeys_from_file([self.alice_path])
-    in_toto_verify(layout, layout_key_dict)
-
-  def test_verify_passing_double_signed_layout(self):
-    """Test pass verification of double-signed layout. """
-    layout = Metablock.load(self.layout_double_signed_path)
-    layout_key_dict = import_publickeys_from_file([self.alice_path, self.bob_path])
-    in_toto_verify(layout, layout_key_dict)
-
-  def test_verify_passing_empty_layout(self):
-    """Test pass verification of layout without steps or inspections. """
-    layout = Metablock.load(self.layout_no_steps_no_inspections)
-    layout_key_dict = import_publickeys_from_file(
-        [self.alice_path])
-    in_toto_verify(layout, layout_key_dict)
-
-  def test_verify_failing_wrong_key(self):
-    """Test fail verification with wrong layout key. """
-    layout = Metablock.load(self.layout_single_signed_path)
-    layout_key_dict = import_publickeys_from_file([self.bob_path])
-    with self.assertRaises(SignatureVerificationError):
-      in_toto_verify(layout, layout_key_dict)
-
-  def test_verify_failing_bad_signature(self):
-    """Test fail verification with bad layout signature. """
-    layout = Metablock.load(self.layout_bad_sig)
-    layout_key_dict = import_publickeys_from_file([self.alice_path])
-    with self.assertRaises(SignatureVerificationError):
-      in_toto_verify(layout, layout_key_dict)
-
-  def test_verify_failing_layout_expired(self):
-    """Test fail verification with expired layout. """
-    layout = Metablock.load(self.layout_expired_path)
-    layout_key_dict = import_publickeys_from_file([self.alice_path])
-    with self.assertRaises(LayoutExpiredError):
-      in_toto_verify(layout, layout_key_dict)
-
-  def test_verify_failing_link_metadata_files(self):
-    """Test fail verification with link metadata files not found. """
-    os.rename("package.2f89b927.link", "package.link.bak")
-    layout = Metablock.load(self.layout_single_signed_path)
-    layout_key_dict = import_publickeys_from_file([self.alice_path])
-    with self.assertRaises(in_toto.exceptions.LinkNotFoundError):
-      in_toto_verify(layout, layout_key_dict)
-    os.rename("package.link.bak", "package.2f89b927.link")
-
-  def test_verify_failing_inspection_exits_non_zero(self):
-    """Test fail verification with inspection returning non-zero. """
-    layout = Metablock.load(self.layout_failing_inspection_retval)
-    layout_key_dict = import_publickeys_from_file([self.alice_path])
-    with self.assertRaises(BadReturnValueError):
-      in_toto_verify(layout, layout_key_dict)
-
-  def test_verify_failing_step_rules(self):
-    """Test fail verification with failing step artifact rule. """
-    layout = Metablock.load(self.layout_failing_step_rule_path)
-    layout_key_dict = import_publickeys_from_file([self.alice_path])
-    with self.assertRaises(RuleVerificationError):
-      in_toto_verify(layout, layout_key_dict)
-
-  def test_verify_failing_inspection_rules(self):
-    """Test fail verification with failing inspection artifact rule. """
-    layout = Metablock.load(self.layout_failing_inspection_rule_path)
-    layout_key_dict = import_publickeys_from_file([self.alice_path])
-    with self.assertRaises(RuleVerificationError):
-      in_toto_verify(layout, layout_key_dict)
-
-  def test_verify_layout_signatures_fail_with_no_keys(self):
-    """Layout signature verification fails when no keys are passed. """
-    layout_metablock = Metablock(signed=Layout())
-    with self.assertRaises(SignatureVerificationError):
-      in_toto_verify(layout_metablock, {})
-
-  def test_verify_layout_signatures_fail_with_malformed_signature(self):
-    """Layout signature verification fails with malformed signatures. """
-    layout_metablock = Metablock(signed=Layout())
-    signature = layout_metablock.sign(self.alice)
-    pubkey = copy.deepcopy(self.alice)
-    pubkey["keyval"]["private"] = ""
-
-    del signature["sig"]
-    layout_metablock.signed.signatures = [signature]
-    with self.assertRaises(SignatureVerificationError):
-      in_toto_verify(layout_metablock, {self.alice["keyid"]: pubkey})
+    @classmethod
+    def setUpClass(self):
+        """Creates and changes into temporary directory.
+        Copies demo files to temp dir...
+          - owner/functionary key pairs
+          - *.link metadata files
+          - layout template (not signed, no expiration date)
+          - final product
+
+        ...and dumps various layouts for different test scenarios
+        """
+
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
+
+        # find where the scripts directory is located.
+        scripts_directory = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "scripts"
+        )
+
+        # Create and change into temporary directory
+        self.set_up_test_dir()
+
+        # Copy demo files to temp dir
+        for fn in os.listdir(demo_files):
+            shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+        # copy scripts over
+        shutil.copytree(scripts_directory, "scripts")
+
+        # Load layout template
+        layout_template = Metablock.load("demo.layout.template")
+
+        # Store various layout paths to be used in tests
+        self.layout_single_signed_path = "single-signed.layout"
+        self.layout_double_signed_path = "double-signed.layout"
+        self.layout_bad_sig = "bad-sig.layout"
+        self.layout_expired_path = "expired.layout"
+        self.layout_failing_step_rule_path = "failing-step-rule.layout"
+        self.layout_failing_inspection_rule_path = (
+            "failing-inspection-rule.layout"
+        )
+        self.layout_failing_inspection_retval = (
+            "failing-inspection-retval.layout"
+        )
+        self.layout_no_steps_no_inspections = "no_steps_no_inspections.layout"
 
+        # Import layout signing keys
+        alice = import_rsa_privatekey_from_file("alice")
+        bob = import_rsa_privatekey_from_file("bob")
+        self.alice_path = "alice.pub"
+        self.bob_path = "bob.pub"
+
+        # dump single signed layout
+        layout = copy.deepcopy(layout_template)
+        layout.sign(alice)
+        layout.dump(self.layout_single_signed_path)
+
+        # dump double signed layout
+        layout = copy.deepcopy(layout_template)
+        layout.sign(alice)
+        layout.sign(bob)
+        layout.dump(self.layout_double_signed_path)
+
+        # dump layout with bad signature
+        layout = copy.deepcopy(layout_template)
+        layout.sign(alice)
+        layout.signed.readme = "this breaks the signature"
+        layout.dump(self.layout_bad_sig)
+
+        # dump expired layout
+        layout = copy.deepcopy(layout_template)
+        layout.signed.expires = (
+            datetime.today() + relativedelta(months=-1)
+        ).strftime("%Y-%m-%dT%H:%M:%SZ")
+        layout.sign(alice)
+        layout.dump(self.layout_expired_path)
+
+        # dump layout with failing step rule
+        layout = copy.deepcopy(layout_template)
+        layout.signed.steps[0].expected_products.insert(0, ["DISALLOW", "*"])
+        layout.signed.steps[0].expected_products.insert(0, ["MODIFY", "*"])
+        layout.sign(alice)
+        layout.dump(self.layout_failing_step_rule_path)
+
+        # dump layout with failing inspection rule
+        layout = copy.deepcopy(layout_template)
+        layout.signed.inspect[0].expected_materials.insert(0, ["MODIFY", "*"])
+        layout.signed.inspect[0].expected_materials.append(["DISALLOW", "*"])
+        layout.sign(alice)
+        layout.dump(self.layout_failing_inspection_rule_path)
+
+        # dump layout with failing inspection retval
+        layout = copy.deepcopy(layout_template)
+        layout.signed.inspect[0].run = [
+            "python",
+            "./scripts/expr",
+            "1",
+            "/",
+            "0",
+        ]
+        layout.sign(alice)
+        layout.dump(self.layout_failing_inspection_retval)
+
+        # dump empty layout
+        layout = Metablock(signed=Layout())
+        layout.sign(alice)
+        layout.dump(self.layout_no_steps_no_inspections)
+        self.alice = alice
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_verify_passing(self):
+        """Test pass verification of single-signed layout."""
+        layout = Metablock.load(self.layout_single_signed_path)
+        layout_key_dict = import_publickeys_from_file([self.alice_path])
+        in_toto_verify(layout, layout_key_dict)
+
+    def test_verify_passing_double_signed_layout(self):
+        """Test pass verification of double-signed layout."""
+        layout = Metablock.load(self.layout_double_signed_path)
+        layout_key_dict = import_publickeys_from_file(
+            [self.alice_path, self.bob_path]
+        )
+        in_toto_verify(layout, layout_key_dict)
 
+    def test_verify_passing_empty_layout(self):
+        """Test pass verification of layout without steps or inspections."""
+        layout = Metablock.load(self.layout_no_steps_no_inspections)
+        layout_key_dict = import_publickeys_from_file([self.alice_path])
+        in_toto_verify(layout, layout_key_dict)
+
+    def test_verify_failing_wrong_key(self):
+        """Test fail verification with wrong layout key."""
+        layout = Metablock.load(self.layout_single_signed_path)
+        layout_key_dict = import_publickeys_from_file([self.bob_path])
+        with self.assertRaises(SignatureVerificationError):
+            in_toto_verify(layout, layout_key_dict)
+
+    def test_verify_failing_bad_signature(self):
+        """Test fail verification with bad layout signature."""
+        layout = Metablock.load(self.layout_bad_sig)
+        layout_key_dict = import_publickeys_from_file([self.alice_path])
+        with self.assertRaises(SignatureVerificationError):
+            in_toto_verify(layout, layout_key_dict)
+
+    def test_verify_failing_layout_expired(self):
+        """Test fail verification with expired layout."""
+        layout = Metablock.load(self.layout_expired_path)
+        layout_key_dict = import_publickeys_from_file([self.alice_path])
+        with self.assertRaises(LayoutExpiredError):
+            in_toto_verify(layout, layout_key_dict)
+
+    def test_verify_failing_link_metadata_files(self):
+        """Test fail verification with link metadata files not found."""
+        os.rename("package.2f89b927.link", "package.link.bak")
+        layout = Metablock.load(self.layout_single_signed_path)
+        layout_key_dict = import_publickeys_from_file([self.alice_path])
+        with self.assertRaises(in_toto.exceptions.LinkNotFoundError):
+            in_toto_verify(layout, layout_key_dict)
+        os.rename("package.link.bak", "package.2f89b927.link")
+
+    def test_verify_failing_inspection_exits_non_zero(self):
+        """Test fail verification with inspection returning non-zero."""
+        layout = Metablock.load(self.layout_failing_inspection_retval)
+        layout_key_dict = import_publickeys_from_file([self.alice_path])
+        with self.assertRaises(BadReturnValueError):
+            in_toto_verify(layout, layout_key_dict)
+
+    def test_verify_failing_step_rules(self):
+        """Test fail verification with failing step artifact rule."""
+        layout = Metablock.load(self.layout_failing_step_rule_path)
+        layout_key_dict = import_publickeys_from_file([self.alice_path])
+        with self.assertRaises(RuleVerificationError):
+            in_toto_verify(layout, layout_key_dict)
+
+    def test_verify_failing_inspection_rules(self):
+        """Test fail verification with failing inspection artifact rule."""
+        layout = Metablock.load(self.layout_failing_inspection_rule_path)
+        layout_key_dict = import_publickeys_from_file([self.alice_path])
+        with self.assertRaises(RuleVerificationError):
+            in_toto_verify(layout, layout_key_dict)
+
+    def test_verify_layout_signatures_fail_with_no_keys(self):
+        """Layout signature verification fails when no keys are passed."""
+        layout_metablock = Metablock(signed=Layout())
+        with self.assertRaises(SignatureVerificationError):
+            in_toto_verify(layout_metablock, {})
+
+    def test_verify_layout_signatures_fail_with_malformed_signature(self):
+        """Layout signature verification fails with malformed signatures."""
+        layout_metablock = Metablock(signed=Layout())
+        signature = layout_metablock.sign(self.alice)
+        pubkey = copy.deepcopy(self.alice)
+        pubkey["keyval"]["private"] = ""
+
+        del signature["sig"]
+        layout_metablock.signed.signatures = [signature]
+        with self.assertRaises(SignatureVerificationError):
+            in_toto_verify(layout_metablock, {self.alice["keyid"]: pubkey})
 
 
 class TestInTotoVerifyThresholds(unittest.TestCase):
-  """Test verifylib functions related to signature thresholds.
+    """Test verifylib functions related to signature thresholds.
 
     - verifylib.verify_link_signature_thresholds
-    - verifylib.verify_threshold_constraints """
+    - verifylib.verify_threshold_constraints"""
 
+    @classmethod
+    def setUpClass(self):
+        """Load test keys from demo files."""
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
 
-  @classmethod
-  def setUpClass(self):
-    """Load test keys from demo files. """
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    self.alice = import_rsa_privatekey_from_file(
-        os.path.join(demo_files, "alice"))
-    self.alice_pubkey = import_rsa_publickey_from_file(
-        os.path.join(demo_files, "alice.pub"))
-    self.alice_keyid = self.alice["keyid"]
-
-    self.bob = import_rsa_privatekey_from_file(
-        os.path.join(demo_files, "bob"))
-    self.bob_pubkey = import_rsa_publickey_from_file(
-        os.path.join(demo_files, "bob.pub"))
-    self.bob_keyid = self.bob["keyid"]
-
-    self.name = "test"
-    self.foo_hash = \
-        "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
-
-
-  def test_thresholds_skip_unauthorized_links(self):
-    """Ignore links with unauthorized signatures. """
-    # Layout with one step, one authorized functionary and threshold 1
-    layout = Layout(
-        keys={
-          self.bob_keyid: self.bob_pubkey
-        },
-        steps=[
-          Step(
-            name=self.name,
-            pubkeys=[self.bob_keyid])
-          ]
-      )
-
-    # Signed links (one authorized the other one not)
-    link_bob = Metablock(signed=Link(name=self.name))
-    link_bob.sign(self.bob)
-    link_alice = Metablock(signed=Link(name=self.name))
-    link_alice.sign(self.alice)
-
-    # The dictionary of links per step passed to the verify function
-    chain_link_dict = {
-      self.name: {
-        self.bob_keyid: link_bob,
-        self.alice_keyid: link_alice
-      }
-    }
-
-    # The dictionary of links expected to be returned, not containing the
-    # unauthorized link, but enough (threshold) authorized links
-    expected_chain_link_dict = {
-      self.name: {
-        self.bob_keyid: link_bob
-      }
-    }
-    # Verify signatures/thresholds
-    returned_chain_link_dict = verify_link_signature_thresholds(
-        layout, chain_link_dict)
-    # Test that the returned dict is as expected
-    self.assertDictEqual(returned_chain_link_dict, expected_chain_link_dict)
-
-
-  def test_thresholds_skip_links_with_failing_signature(self):
-    """Ignore links with failing signatures. """
-
-    # Layout with one step, two authorized functionaries and threshold 1
-    layout = Layout(
-        keys={
-          self.bob_keyid: self.bob_pubkey,
-          self.alice_keyid: self.alice_pubkey,
-        },
-        steps=[
-          Step(
-            name=self.name,
-            pubkeys=[self.bob_keyid, self.alice_keyid],
-            threshold=1)
-          ]
-        )
-
-    # Authorized links (one signed one not)
-    link_bob = Metablock(signed=Link(name=self.name))
-    link_bob.sign(self.bob)
-    link_alice = Metablock(signed=Link(name=self.name))
-
-    # The dictionary of links per step passed to the verify function
-    chain_link_dict = {
-      self.name: {
-        self.bob_keyid: link_bob,
-        self.alice_keyid: link_alice
-      }
-    }
-
-    # The dictionary of links expected to be returned, not containing the
-    # unauthorized link, but enough (threshold) authorized links
-    expected_chain_link_dict = {
-      self.name: {
-        self.bob_keyid: link_bob
-      }
-    }
-
-    # Verify signatures/thresholds
-    returned_chain_link_dict = verify_link_signature_thresholds(
-        layout, chain_link_dict)
-    # Test that the returned dict is as expected
-    self.assertDictEqual(returned_chain_link_dict, expected_chain_link_dict)
-
-
-  def test_thresholds_fail_with_not_enough_valid_links(self):
-    """ Fail with not enough authorized links. """
-
-    # Layout with one step, two authorized functionaries and threshold 2
-    layout = Layout(
-        keys={
-          self.bob_keyid: self.bob_pubkey,
-          self.alice_keyid: self.alice_pubkey,
-        },
-        steps=[
-          Step(
-            name=self.name,
-            pubkeys=[self.bob_keyid, self.alice_keyid],
-            threshold=2)
-          ]
-        )
-
-    # Only one authorized and validly signed link
-    link_bob = Metablock(signed=Link(name=self.name))
-    link_bob.sign(self.bob)
-
-    # The dictionary of links per step passed to the verify function
-    chain_link_dict = {
-      self.name: {
-        self.bob_keyid: link_bob
-      }
-    }
-
-    # Fail signature threshold verification with not enough links
-    with self.assertRaises(ThresholdVerificationError):
-      verify_link_signature_thresholds(layout, chain_link_dict)
-
-
-  def test_threshold_constraints_fail_with_not_enough_links(self):
-    """ Fail with not enough links. """
-    # Layout with one step and threshold 2
-    layout = Layout(steps=[Step(name=self.name, threshold=2)])
-    # Authorized (unsigned) link
-    # This function does not care for signatures it just verifies if the
-    # different links have recorded the same artifacts. Signature verification
-    # happens earlier in the final product verification (see tests above)
-    link_bob = Metablock(signed=Link(name=self.name))
-
-    chain_link_dict = {
-      self.name: {
-        self.bob_keyid: link_bob,
-      }
-    }
-
-    with self.assertRaises(ThresholdVerificationError):
-      verify_threshold_constraints(layout, chain_link_dict)
-
-
-  def test_threshold_constraints_fail_with_unequal_links(self):
-    """ Test that the links for a step recorded the same artifacts. """
-    # Layout with one step and threshold 2
-    layout = Layout(steps=[Step(name=self.name, threshold=2)])
-    link_bob = Link(
-      name=self.name,
-      materials={
-        "foo": {"sha256": self.foo_hash}
-      }
-    )
-    # Cf. signing comment in test_thresholds_constraints_with_not_enough_links
-    link_alice = Link(name=self.name)
-
-    chain_link_dict = {
-      self.name: {
-        self.bob_keyid: link_bob,
-        self.alice_keyid: link_alice,
-      }
-    }
-
-    with self.assertRaises(ThresholdVerificationError):
-      verify_threshold_constraints(layout, chain_link_dict)
-
-
-
-  def test_threshold_constraints_pas_with_equal_links(self):
-    """ Pass threshold constraint verification with equal links. """
-    # Layout with one step and threshold 2
-    layout = Layout(steps=[Step(name=self.name, threshold=2)])
-    # Two authorized links with equal artifact recordings (materials)
-    # Cf. signing comment in test_thresholds_constraints_with_not_enough_links
-    link_bob = Link(
-      name=self.name,
-      materials={
-        "foo": {"sha256": self.foo_hash}
-      }
-    )
-    link_alice = Link(
-      name=self.name,
-      materials={
-        "foo": {"sha256": self.foo_hash}
-      }
-    )
-
-    chain_link_dict = {
-      self.name: {
-        self.bob_keyid: link_bob,
-        self.alice_keyid: link_alice,
-      }
-    }
+        self.alice = import_rsa_privatekey_from_file(
+            os.path.join(demo_files, "alice")
+        )
+        self.alice_pubkey = import_rsa_publickey_from_file(
+            os.path.join(demo_files, "alice.pub")
+        )
+        self.alice_keyid = self.alice["keyid"]
 
-    verify_threshold_constraints(layout, chain_link_dict)
+        self.bob = import_rsa_privatekey_from_file(
+            os.path.join(demo_files, "bob")
+        )
+        self.bob_pubkey = import_rsa_publickey_from_file(
+            os.path.join(demo_files, "bob.pub")
+        )
+        self.bob_keyid = self.bob["keyid"]
 
+        self.name = "test"
+        self.foo_hash = (
+            "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
+        )
 
+    def test_thresholds_skip_unauthorized_links(self):
+        """Ignore links with unauthorized signatures."""
+        # Layout with one step, one authorized functionary and threshold 1
+        layout = Layout(
+            keys={self.bob_keyid: self.bob_pubkey},
+            steps=[Step(name=self.name, pubkeys=[self.bob_keyid])],
+        )
 
-@unittest.skipIf(not have_gpg(), "gpg not found")
-class TestInTotoVerifyThresholdsGpgSubkeys(
-    unittest.TestCase, TmpDirMixin, GPGKeysMixin):
-  """
-  Test the following 8 scenarios for combinations of link authorization,
-  where a link is either signed by a master or subkey (SIG), and the
-  corresponding step authorizes either the master or subkey (AUTH), and the
-  corresponding top level key in the layout key store is either a master key
-  (bundle, i.e. with subkeys) or a subkey (KEY).
-
-  M ... Masterkey
-  S ... Subkey
-
-  SIG AUTH KEY(bundle)| OK  | Comment
-  ---------------------------------------------------------------
-  M   M    M          | Yes | Normal scenario (*)
-  M   M    S          | No  | Cannot find key in key store + cannot sign (*)
-  M   S    M          | No  | Unallowed trust delegation + cannot sign (*)
-  M   S    S          | No  | Unallowed trust delegation + cannot sign (*)
-  S   M    M          | Yes | Allowed trust delegation
-  S   M    S          | No  | Cannot associate keys
-  S   S    M          | Yes | Can find key in key store
-  S   S    S          | Yes | Generalizes to normal scenario
-
-  (*) NOTE: Master keys with a subkey with signing capability always use that
-  subkey, even if the master keyid is specified and has signing capability.
-
-
-  Plus additional gpg subkey related threshold tests.
-
-  """
-
-  @classmethod
-  def setUpClass(self):
-    self.set_up_test_dir()
-    self.set_up_gpg_keys()
-
-    master_key = securesystemslib.gpg.functions.export_pubkey(
-        self.gpg_key_0C8A17, self.gnupg_home)
-    sub_key = master_key["subkeys"][self.gpg_key_D924E9]
-
-    # We need a gpg key without subkeys to test the normal scenario (M M M),
-    # because keys with signing subkeys always use that subkey for signing.
-    master_key2 = securesystemslib.gpg.functions.export_pubkey(
-        self.gpg_key_768C43, self.gnupg_home)
-
-
-    self.pub_key_dict = {
-      self.gpg_key_0C8A17: master_key,
-      self.gpg_key_D924E9: sub_key,
-      self.gpg_key_768C43: master_key2
-    }
-
-    self.step_name = "name"
-
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def _verify_link_signature_tresholds(self, sig_id, auth_id, key_id):
-    metablock = Metablock(signed=Link(name=self.step_name))
-    metablock.sign_gpg(sig_id, self.gnupg_home)                        # SIG
-
-    chain_link_dict = {
-      self.step_name : {
-        sig_id : metablock                                             # SIG
-      }
-    }
-
-    layout = Layout(
-      steps=[
-        Step(
-            name=self.step_name,
-            pubkeys=[auth_id]                                          # AUTH
-          )
-        ],
-      keys={
-          key_id: self.pub_key_dict[key_id]                            # KEY
+        # Signed links (one authorized the other one not)
+        link_bob = Metablock(signed=Link(name=self.name))
+        link_bob.sign(self.bob)
+        link_alice = Metablock(signed=Link(name=self.name))
+        link_alice.sign(self.alice)
+
+        # The dictionary of links per step passed to the verify function
+        chain_link_dict = {
+            self.name: {self.bob_keyid: link_bob, self.alice_keyid: link_alice}
         }
-      )
-    return layout, chain_link_dict
 
+        # The dictionary of links expected to be returned, not containing the
+        # unauthorized link, but enough (threshold) authorized links
+        expected_chain_link_dict = {self.name: {self.bob_keyid: link_bob}}
+        # Verify signatures/thresholds
+        returned_chain_link_dict = verify_link_signature_thresholds(
+            layout, chain_link_dict
+        )
+        # Test that the returned dict is as expected
+        self.assertDictEqual(returned_chain_link_dict, expected_chain_link_dict)
+
+    def test_thresholds_skip_links_with_failing_signature(self):
+        """Ignore links with failing signatures."""
+
+        # Layout with one step, two authorized functionaries and threshold 1
+        layout = Layout(
+            keys={
+                self.bob_keyid: self.bob_pubkey,
+                self.alice_keyid: self.alice_pubkey,
+            },
+            steps=[
+                Step(
+                    name=self.name,
+                    pubkeys=[self.bob_keyid, self.alice_keyid],
+                    threshold=1,
+                )
+            ],
+        )
 
-  def test_verify_link_signature_thresholds__M_M_M(self):
-    """Normal scenario. """
-    layout, chain_link_dict = self._verify_link_signature_tresholds(
-        self.gpg_key_768C43, self.gpg_key_768C43, self.gpg_key_768C43)
-
-    #print("path: {}".format(os.environ['PATH']))
-    verify_link_signature_thresholds(layout, chain_link_dict)
-
-
-  def test_verify_link_signature_thresholds__M_M_S__M_S_M__M_S_S(self):
-    """Cannot sign with master key if subkey is present. """
-    # The scenarios MMS, MSM, MSS are impossible because we cannot sign
-    # with a master key, if there is a subkey with signing capability
-    # GPG will always use that subkey.
-    # Even if gpg would use the masterkey, these scenarios are not allowed,
-    # see table in docstring of testcase
-    signature = securesystemslib.gpg.functions.create_signature(
-        b"data", self.gpg_key_0C8A17, self.gnupg_home)
-
-    self.assertTrue(signature["keyid"] == self.gpg_key_D924E9)
-
-
-  def test_verify_link_signature_thresholds__S_M_M(self):
-    """Allowed trust delegation. """
-    layout, chain_link_dict = self._verify_link_signature_tresholds(
-        self.gpg_key_D924E9, self.gpg_key_0C8A17, self.gpg_key_0C8A17)
-    verify_link_signature_thresholds(layout, chain_link_dict)
-
-
-  def test_verify_link_signature_thresholds__S_M_S(self):
-    """Cannot associate keys. """
-    layout, chain_link_dict = self._verify_link_signature_tresholds(
-        self.gpg_key_D924E9, self.gpg_key_0C8A17, self.gpg_key_D924E9)
-    with self.assertRaises(ThresholdVerificationError):
-      verify_link_signature_thresholds(layout, chain_link_dict)
-
-
-  def test_verify_link_signature_thresholds__S_S_M(self):
-    """No trust delegation and can find key in key store. """
-    layout, chain_link_dict = self._verify_link_signature_tresholds(
-        self.gpg_key_D924E9, self.gpg_key_D924E9, self.gpg_key_0C8A17)
-    verify_link_signature_thresholds(layout, chain_link_dict)
-
-
-  def test_verify_link_signature_thresholds__S_S_S(self):
-    """Generalizes to normal scenario. """
-    layout, chain_link_dict = self._verify_link_signature_tresholds(
-        self.gpg_key_D924E9, self.gpg_key_D924E9, self.gpg_key_D924E9)
-    verify_link_signature_thresholds(layout, chain_link_dict)
-
-
-  def test_verify_subkey_thresholds(self):
-    """Subkeys of same main key count only once towards threshold. """
-
-    masterkey = "40e692c3ae03f6b88dff95d0d2c9fe930766998d"
-    subkey1 = "35830aa342b9fea0178876b02b25647ff0ef59fe"
-    subkey2 = "732d722578f71a9ec967a64bfead922c91eb7351"
-
-    link1 = Metablock(signed=Link(name=self.step_name))
-    link1.sign_gpg(subkey1, self.gnupg_home)
-    link2 = Metablock(signed=Link(name=self.step_name))
-    link2.sign_gpg(subkey2, self.gnupg_home)
-
-    chain_link_dict = {
-      self.step_name : {
-        subkey1: link1,
-        subkey2: link2
-      }
-    }
-
-    layout = Layout(
-      steps=[
-          Step(name=self.step_name, pubkeys=[masterkey], threshold=2)
-        ],
-      keys={
-          masterkey: securesystemslib.gpg.functions.export_pubkey(
-              masterkey, self.gnupg_home)
+        # Authorized links (one signed one not)
+        link_bob = Metablock(signed=Link(name=self.name))
+        link_bob.sign(self.bob)
+        link_alice = Metablock(signed=Link(name=self.name))
+
+        # The dictionary of links per step passed to the verify function
+        chain_link_dict = {
+            self.name: {self.bob_keyid: link_bob, self.alice_keyid: link_alice}
         }
-      )
-    with self.assertRaises(ThresholdVerificationError):
-      verify_link_signature_thresholds(layout, chain_link_dict)
 
-  def test_verify_thresholds_skip_expired_key(self):
-    """Verify that a link signed with an expired key is skipped.
+        # The dictionary of links expected to be returned, not containing the
+        # unauthorized link, but enough (threshold) authorized links
+        expected_chain_link_dict = {self.name: {self.bob_keyid: link_bob}}
+
+        # Verify signatures/thresholds
+        returned_chain_link_dict = verify_link_signature_thresholds(
+            layout, chain_link_dict
+        )
+        # Test that the returned dict is as expected
+        self.assertDictEqual(returned_chain_link_dict, expected_chain_link_dict)
 
-    NOTE: This test would be a better fit for `TestInTotoVerifyThresholds`,
-    but we make use of `TestInTotoVerifyThresholdsGpgSubkeys`'s gpg setup here.
+    def test_thresholds_fail_with_not_enough_valid_links(self):
+        """Fail with not enough authorized links."""
 
+        # Layout with one step, two authorized functionaries and threshold 2
+        layout = Layout(
+            keys={
+                self.bob_keyid: self.bob_pubkey,
+                self.alice_keyid: self.alice_pubkey,
+            },
+            steps=[
+                Step(
+                    name=self.name,
+                    pubkeys=[self.bob_keyid, self.alice_keyid],
+                    threshold=2,
+                )
+            ],
+        )
+
+        # Only one authorized and validly signed link
+        link_bob = Metablock(signed=Link(name=self.name))
+        link_bob.sign(self.bob)
+
+        # The dictionary of links per step passed to the verify function
+        chain_link_dict = {self.name: {self.bob_keyid: link_bob}}
+
+        # Fail signature threshold verification with not enough links
+        with self.assertRaises(ThresholdVerificationError):
+            verify_link_signature_thresholds(layout, chain_link_dict)
+
+    def test_threshold_constraints_fail_with_not_enough_links(self):
+        """Fail with not enough links."""
+        # Layout with one step and threshold 2
+        layout = Layout(steps=[Step(name=self.name, threshold=2)])
+        # Authorized (unsigned) link
+        # This function does not care for signatures it just verifies if the
+        # different links have recorded the same artifacts. Signature verification
+        # happens earlier in the final product verification (see tests above)
+        link_bob = Metablock(signed=Link(name=self.name))
+
+        chain_link_dict = {
+            self.name: {
+                self.bob_keyid: link_bob,
+            }
+        }
+
+        with self.assertRaises(ThresholdVerificationError):
+            verify_threshold_constraints(layout, chain_link_dict)
+
+    def test_threshold_constraints_fail_with_unequal_links(self):
+        """Test that the links for a step recorded the same artifacts."""
+        # Layout with one step and threshold 2
+        layout = Layout(steps=[Step(name=self.name, threshold=2)])
+        link_bob = Link(
+            name=self.name, materials={"foo": {"sha256": self.foo_hash}}
+        )
+        # Cf. signing comment in test_thresholds_constraints_with_not_enough_links
+        link_alice = Link(name=self.name)
+
+        chain_link_dict = {
+            self.name: {
+                self.bob_keyid: link_bob,
+                self.alice_keyid: link_alice,
+            }
+        }
+
+        with self.assertRaises(ThresholdVerificationError):
+            verify_threshold_constraints(layout, chain_link_dict)
+
+    def test_threshold_constraints_pas_with_equal_links(self):
+        """Pass threshold constraint verification with equal links."""
+        # Layout with one step and threshold 2
+        layout = Layout(steps=[Step(name=self.name, threshold=2)])
+        # Two authorized links with equal artifact recordings (materials)
+        # Cf. signing comment in test_thresholds_constraints_with_not_enough_links
+        link_bob = Link(
+            name=self.name, materials={"foo": {"sha256": self.foo_hash}}
+        )
+        link_alice = Link(
+            name=self.name, materials={"foo": {"sha256": self.foo_hash}}
+        )
+
+        chain_link_dict = {
+            self.name: {
+                self.bob_keyid: link_bob,
+                self.alice_keyid: link_alice,
+            }
+        }
+
+        verify_threshold_constraints(layout, chain_link_dict)
+
+
+@unittest.skipIf(not have_gpg(), "gpg not found")
+class TestInTotoVerifyThresholdsGpgSubkeys(
+    unittest.TestCase, TmpDirMixin, GPGKeysMixin
+):
     """
-    expired_key_id = "e8ac80c924116dabb51d4b987cb07d6d2c199c7c"
-    expired_key = securesystemslib.gpg.functions.export_pubkey(expired_key_id,
-        self.gnupg_home)
-
-    # Chain link dict containing a single link for a single step
-    # The link's signature is (supposedly) signed by an expired key and
-    # hence does not count towards the link threshold as defined in the layout.
-    chain_link_dict = {
-      self.step_name : {
-        expired_key_id: Metablock(
-          signed=Link(name=self.step_name),
-          signatures=[{
-            "keyid": expired_key_id,
-            "other_headers": "deadbeef",
-            "signature": "deadbeef",
-          }])
-      }
-    }
-    layout = Layout(
-      steps=[Step(name=self.step_name, pubkeys=[expired_key_id], threshold=1)],
-      keys={expired_key_id: expired_key}
-    )
-
-    with self.assertRaises(ThresholdVerificationError), \
-        patch("in_toto.verifylib.LOG") as mock_log:
-      verify_link_signature_thresholds(layout, chain_link_dict)
-
-    msg = mock_log.info.call_args[0][0]
-    self.assertTrue("Skipping link" in msg and "expired" in msg,
-        "Unexpected log message: {}".format(msg))
+    Test the following 8 scenarios for combinations of link authorization,
+    where a link is either signed by a master or subkey (SIG), and the
+    corresponding step authorizes either the master or subkey (AUTH), and the
+    corresponding top level key in the layout key store is either a master key
+    (bundle, i.e. with subkeys) or a subkey (KEY).
+
+    M ... Masterkey
+    S ... Subkey
+
+    SIG AUTH KEY(bundle)| OK  | Comment
+    ---------------------------------------------------------------
+    M   M    M          | Yes | Normal scenario (*)
+    M   M    S          | No  | Cannot find key in key store + cannot sign (*)
+    M   S    M          | No  | Unallowed trust delegation + cannot sign (*)
+    M   S    S          | No  | Unallowed trust delegation + cannot sign (*)
+    S   M    M          | Yes | Allowed trust delegation
+    S   M    S          | No  | Cannot associate keys
+    S   S    M          | Yes | Can find key in key store
+    S   S    S          | Yes | Generalizes to normal scenario
+
+    (*) NOTE: Master keys with a subkey with signing capability always use that
+    subkey, even if the master keyid is specified and has signing capability.
+
+
+    Plus additional gpg subkey related threshold tests.
+
+    """
+
+    @classmethod
+    def setUpClass(self):
+        self.set_up_test_dir()
+        self.set_up_gpg_keys()
+
+        master_key = securesystemslib.gpg.functions.export_pubkey(
+            self.gpg_key_0C8A17, self.gnupg_home
+        )
+        sub_key = master_key["subkeys"][self.gpg_key_D924E9]
+
+        # We need a gpg key without subkeys to test the normal scenario (M M M),
+        # because keys with signing subkeys always use that subkey for signing.
+        master_key2 = securesystemslib.gpg.functions.export_pubkey(
+            self.gpg_key_768C43, self.gnupg_home
+        )
+
+        self.pub_key_dict = {
+            self.gpg_key_0C8A17: master_key,
+            self.gpg_key_D924E9: sub_key,
+            self.gpg_key_768C43: master_key2,
+        }
+
+        self.step_name = "name"
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def _verify_link_signature_tresholds(self, sig_id, auth_id, key_id):
+        metablock = Metablock(signed=Link(name=self.step_name))
+        metablock.sign_gpg(sig_id, self.gnupg_home)  # SIG
+
+        chain_link_dict = {self.step_name: {sig_id: metablock}}  # SIG
+
+        layout = Layout(
+            steps=[Step(name=self.step_name, pubkeys=[auth_id])],  # AUTH
+            keys={key_id: self.pub_key_dict[key_id]},  # KEY
+        )
+        return layout, chain_link_dict
+
+    def test_verify_link_signature_thresholds__M_M_M(self):
+        """Normal scenario."""
+        layout, chain_link_dict = self._verify_link_signature_tresholds(
+            self.gpg_key_768C43, self.gpg_key_768C43, self.gpg_key_768C43
+        )
+
+        # print("path: {}".format(os.environ['PATH']))
+        verify_link_signature_thresholds(layout, chain_link_dict)
+
+    def test_verify_link_signature_thresholds__M_M_S__M_S_M__M_S_S(self):
+        """Cannot sign with master key if subkey is present."""
+        # The scenarios MMS, MSM, MSS are impossible because we cannot sign
+        # with a master key, if there is a subkey with signing capability
+        # GPG will always use that subkey.
+        # Even if gpg would use the masterkey, these scenarios are not allowed,
+        # see table in docstring of testcase
+        signature = securesystemslib.gpg.functions.create_signature(
+            b"data", self.gpg_key_0C8A17, self.gnupg_home
+        )
+
+        self.assertTrue(signature["keyid"] == self.gpg_key_D924E9)
+
+    def test_verify_link_signature_thresholds__S_M_M(self):
+        """Allowed trust delegation."""
+        layout, chain_link_dict = self._verify_link_signature_tresholds(
+            self.gpg_key_D924E9, self.gpg_key_0C8A17, self.gpg_key_0C8A17
+        )
+        verify_link_signature_thresholds(layout, chain_link_dict)
+
+    def test_verify_link_signature_thresholds__S_M_S(self):
+        """Cannot associate keys."""
+        layout, chain_link_dict = self._verify_link_signature_tresholds(
+            self.gpg_key_D924E9, self.gpg_key_0C8A17, self.gpg_key_D924E9
+        )
+        with self.assertRaises(ThresholdVerificationError):
+            verify_link_signature_thresholds(layout, chain_link_dict)
+
+    def test_verify_link_signature_thresholds__S_S_M(self):
+        """No trust delegation and can find key in key store."""
+        layout, chain_link_dict = self._verify_link_signature_tresholds(
+            self.gpg_key_D924E9, self.gpg_key_D924E9, self.gpg_key_0C8A17
+        )
+        verify_link_signature_thresholds(layout, chain_link_dict)
+
+    def test_verify_link_signature_thresholds__S_S_S(self):
+        """Generalizes to normal scenario."""
+        layout, chain_link_dict = self._verify_link_signature_tresholds(
+            self.gpg_key_D924E9, self.gpg_key_D924E9, self.gpg_key_D924E9
+        )
+        verify_link_signature_thresholds(layout, chain_link_dict)
+
+    def test_verify_subkey_thresholds(self):
+        """Subkeys of same main key count only once towards threshold."""
+
+        masterkey = "40e692c3ae03f6b88dff95d0d2c9fe930766998d"
+        subkey1 = "35830aa342b9fea0178876b02b25647ff0ef59fe"
+        subkey2 = "732d722578f71a9ec967a64bfead922c91eb7351"
+
+        link1 = Metablock(signed=Link(name=self.step_name))
+        link1.sign_gpg(subkey1, self.gnupg_home)
+        link2 = Metablock(signed=Link(name=self.step_name))
+        link2.sign_gpg(subkey2, self.gnupg_home)
+
+        chain_link_dict = {self.step_name: {subkey1: link1, subkey2: link2}}
+
+        layout = Layout(
+            steps=[Step(name=self.step_name, pubkeys=[masterkey], threshold=2)],
+            keys={
+                masterkey: securesystemslib.gpg.functions.export_pubkey(
+                    masterkey, self.gnupg_home
+                )
+            },
+        )
+        with self.assertRaises(ThresholdVerificationError):
+            verify_link_signature_thresholds(layout, chain_link_dict)
+
+    def test_verify_thresholds_skip_expired_key(self):
+        """Verify that a link signed with an expired key is skipped.
+
+        NOTE: This test would be a better fit for `TestInTotoVerifyThresholds`,
+        but we make use of `TestInTotoVerifyThresholdsGpgSubkeys`'s gpg setup here.
+
+        """
+        expired_key_id = "e8ac80c924116dabb51d4b987cb07d6d2c199c7c"
+        expired_key = securesystemslib.gpg.functions.export_pubkey(
+            expired_key_id, self.gnupg_home
+        )
+
+        # Chain link dict containing a single link for a single step
+        # The link's signature is (supposedly) signed by an expired key and
+        # hence does not count towards the link threshold as defined in the layout.
+        chain_link_dict = {
+            self.step_name: {
+                expired_key_id: Metablock(
+                    signed=Link(name=self.step_name),
+                    signatures=[
+                        {
+                            "keyid": expired_key_id,
+                            "other_headers": "deadbeef",
+                            "signature": "deadbeef",
+                        }
+                    ],
+                )
+            }
+        }
+        layout = Layout(
+            steps=[
+                Step(name=self.step_name, pubkeys=[expired_key_id], threshold=1)
+            ],
+            keys={expired_key_id: expired_key},
+        )
+
+        with self.assertRaises(ThresholdVerificationError), patch(
+            "in_toto.verifylib.LOG"
+        ) as mock_log:
+            verify_link_signature_thresholds(layout, chain_link_dict)
+
+        msg = mock_log.info.call_args[0][0]
+        self.assertTrue(
+            "Skipping link" in msg and "expired" in msg,
+            "Unexpected log message: {}".format(msg),
+        )
 
 
 class TestVerifySublayouts(unittest.TestCase, TmpDirMixin):
-  """Tests verifylib.verify_sublayouts(layout, reduced_chain_link_dict).
-  Call with one-step super layout that has a sublayout (demo layout). """
+    """Tests verifylib.verify_sublayouts(layout, reduced_chain_link_dict).
+    Call with one-step super layout that has a sublayout (demo layout)."""
+
+    @classmethod
+    def setUpClass(self):
+        """Creates and changes into temporary directory and prepares two layouts.
+        The superlayout, which has one step and its sublayout, which is the usual
+        demo layout (write code, package, inspect tar)."""
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
+
+        # find where the scripts directory is located.
+        scripts_directory = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "scripts"
+        )
 
-  @classmethod
-  def setUpClass(self):
-    """Creates and changes into temporary directory and prepares two layouts.
-    The superlayout, which has one step and its sublayout, which is the usual
-    demo layout (write code, package, inspect tar). """
-    # Find demo files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    # find where the scripts directory is located.
-    scripts_directory = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "scripts")
-
-    # Create and change into temporary directory
-    self.set_up_test_dir()
-
-    # Copy demo files to temp dir
-    for fn in os.listdir(demo_files):
-      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
-
-    # copy portable scripts over
-    shutil.copytree(scripts_directory, 'scripts')
-
-    # Import sub layout signing (private) and verifying (public) keys
-    alice = import_rsa_privatekey_from_file("alice")
-    alice_pub = import_rsa_publickey_from_file("alice.pub")
-
-    # From the perspective of the superlayout, the sublayout is treated as
-    # a link corresponding to a step, hence needs a name.
-    sub_layout_name = "sub_layout"
-
-    # Sublayout links are expected in a directory relative to the superlayout's
-    # link directory
-    sub_layout_link_dir = SUBLAYOUT_LINK_DIR_FORMAT.format(
-        name=sub_layout_name, keyid=alice["keyid"])
-
-    for sublayout_link_name in glob.glob("*.link"):
-      dest_path = os.path.join(sub_layout_link_dir, sublayout_link_name)
-      os.renames(sublayout_link_name, dest_path)
-
-
-    # Copy, sign and dump sub layout as link from template
-    layout_template = Metablock.load("demo.layout.template")
-    sub_layout = copy.deepcopy(layout_template)
-    sub_layout_path = FILENAME_FORMAT.format(step_name=sub_layout_name,
-        keyid=alice_pub["keyid"])
-    sub_layout.sign(alice)
-    sub_layout.dump(sub_layout_path)
-
-    # Create super layout that has only one step, the sublayout
-    self.super_layout = Layout()
-    self.super_layout.keys[alice_pub["keyid"]] = alice_pub
-    sub_layout_step = Step(
-        name=sub_layout_name,
-        pubkeys=[alice_pub["keyid"]]
-      )
-    self.super_layout.steps.append(sub_layout_step)
-
-    # Load the super layout links (i.e. the sublayout)
-    self.super_layout_links = load_links_for_layout(self.super_layout, ".")
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-
-  def test_verify_demo_as_sublayout(self):
-    """Test super layout's passing sublayout verification. """
-    verify_sublayouts(
-        self.super_layout, self.super_layout_links, ".")
+        # Create and change into temporary directory
+        self.set_up_test_dir()
 
+        # Copy demo files to temp dir
+        for fn in os.listdir(demo_files):
+            shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+        # copy portable scripts over
+        shutil.copytree(scripts_directory, "scripts")
+
+        # Import sub layout signing (private) and verifying (public) keys
+        alice = import_rsa_privatekey_from_file("alice")
+        alice_pub = import_rsa_publickey_from_file("alice.pub")
+
+        # From the perspective of the superlayout, the sublayout is treated as
+        # a link corresponding to a step, hence needs a name.
+        sub_layout_name = "sub_layout"
+
+        # Sublayout links are expected in a directory relative to the superlayout's
+        # link directory
+        sub_layout_link_dir = SUBLAYOUT_LINK_DIR_FORMAT.format(
+            name=sub_layout_name, keyid=alice["keyid"]
+        )
 
+        for sublayout_link_name in glob.glob("*.link"):
+            dest_path = os.path.join(sub_layout_link_dir, sublayout_link_name)
+            os.renames(sublayout_link_name, dest_path)
+
+        # Copy, sign and dump sub layout as link from template
+        layout_template = Metablock.load("demo.layout.template")
+        sub_layout = copy.deepcopy(layout_template)
+        sub_layout_path = FILENAME_FORMAT.format(
+            step_name=sub_layout_name, keyid=alice_pub["keyid"]
+        )
+        sub_layout.sign(alice)
+        sub_layout.dump(sub_layout_path)
 
+        # Create super layout that has only one step, the sublayout
+        self.super_layout = Layout()
+        self.super_layout.keys[alice_pub["keyid"]] = alice_pub
+        sub_layout_step = Step(
+            name=sub_layout_name, pubkeys=[alice_pub["keyid"]]
+        )
+        self.super_layout.steps.append(sub_layout_step)
+
+        # Load the super layout links (i.e. the sublayout)
+        self.super_layout_links = load_links_for_layout(self.super_layout, ".")
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_verify_demo_as_sublayout(self):
+        """Test super layout's passing sublayout verification."""
+        verify_sublayouts(self.super_layout, self.super_layout_links, ".")
 
 
 class TestInTotoVerifyMultiLevelSublayouts(unittest.TestCase, TmpDirMixin):
-  """Test verifylib.in_toto_verify with multiple levels of sublayouts. """
+    """Test verifylib.in_toto_verify with multiple levels of sublayouts."""
 
-  def test_verify_multi_level_sublayout(self):
-    # Find demo files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    # Create and change into temporary directory
-    self.set_up_test_dir()
-
-    # We don't need to copy the demo files, we just load the keys
-    keys = {}
-    for key_name in ["alice", "bob", "carl"]:
-      keys[key_name + "_priv"] = import_rsa_privatekey_from_file(
-          os.path.join(demo_files, key_name))
-      keys[key_name + "_pub"] = import_rsa_publickey_from_file(
-          os.path.join(demo_files, key_name + ".pub"))
-
-
-    # Create layout hierarchy
-
-    # Root layout
-    # The root layout is the layout that will be passed to `in_toto_verify`
-    # It only has one step which is a sublayout, into which verification
-    # recurses. Only the root layout and root layout verification key will be
-    # passed to verification.
-    root_layout_pub_key_dict = {
-        keys["alice_pub"]["keyid"]: keys["alice_pub"]
-      }
-
-    root_layout_step_name = "delegated-to-bob"
-
-    root_layout = Metablock(signed=Layout(
-        keys={
-          keys["bob_pub"]["keyid"]: keys["bob_pub"]
-        },
-        steps=[
-            Step(
-              name=root_layout_step_name,
-              pubkeys=[
-                keys["bob_pub"]["keyid"]
-              ]
-            )
-          ]
+    def test_verify_multi_level_sublayout(self):
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
         )
-      )
-    root_layout.sign(keys["alice_priv"])
 
+        # Create and change into temporary directory
+        self.set_up_test_dir()
 
-    # Sublayout (first level)
-    # The first level sublayout wil be treated as a link from the
-    # superlayout's perspective and loaded from the current working directory.
-    # The link for the only step of this sublayout will be placed in a
-    # namespaced subdir, that link itself is a sublayout (subsublayout).
-    bobs_layout_name = FILENAME_FORMAT.format(
-        step_name=root_layout_step_name,
-        keyid=keys["bob_pub"]["keyid"])
-
-    bobs_layout_link_dir = SUBLAYOUT_LINK_DIR_FORMAT.format(
-        name=root_layout_step_name,
-        keyid=keys["bob_pub"]["keyid"])
-    os.mkdir(bobs_layout_link_dir)
-
-    bobs_layout_step_name = "delegated-to-carl"
-
-    bobs_layout = Metablock(signed=Layout(
-        keys={
-          keys["carl_pub"]["keyid"]: keys["carl_pub"]
-          },
-        steps=[
-            Step(
-              name=bobs_layout_step_name,
-              pubkeys=[keys["carl_pub"]["keyid"]]
+        # We don't need to copy the demo files, we just load the keys
+        keys = {}
+        for key_name in ["alice", "bob", "carl"]:
+            keys[key_name + "_priv"] = import_rsa_privatekey_from_file(
+                os.path.join(demo_files, key_name)
+            )
+            keys[key_name + "_pub"] = import_rsa_publickey_from_file(
+                os.path.join(demo_files, key_name + ".pub")
+            )
+
+        # Create layout hierarchy
+
+        # Root layout
+        # The root layout is the layout that will be passed to `in_toto_verify`
+        # It only has one step which is a sublayout, into which verification
+        # recurses. Only the root layout and root layout verification key will be
+        # passed to verification.
+        root_layout_pub_key_dict = {
+            keys["alice_pub"]["keyid"]: keys["alice_pub"]
+        }
+
+        root_layout_step_name = "delegated-to-bob"
+
+        root_layout = Metablock(
+            signed=Layout(
+                keys={keys["bob_pub"]["keyid"]: keys["bob_pub"]},
+                steps=[
+                    Step(
+                        name=root_layout_step_name,
+                        pubkeys=[keys["bob_pub"]["keyid"]],
+                    )
+                ],
             )
-          ]
         )
-      )
-    bobs_layout.sign(keys["bob_priv"])
-    bobs_layout.dump(bobs_layout_name)
+        root_layout.sign(keys["alice_priv"])
 
+        # Sublayout (first level)
+        # The first level sublayout wil be treated as a link from the
+        # superlayout's perspective and loaded from the current working directory.
+        # The link for the only step of this sublayout will be placed in a
+        # namespaced subdir, that link itself is a sublayout (subsublayout).
+        bobs_layout_name = FILENAME_FORMAT.format(
+            step_name=root_layout_step_name, keyid=keys["bob_pub"]["keyid"]
+        )
 
-    # Subsublayout (second level)
-    # The subsublayout will be placed in the namespaced link dir
-    # of its superlayout (sublayout from the root layout's perspective), for
-    # for which it serves as link.
-    carls_layout_name = FILENAME_FORMAT.format(
-            step_name=bobs_layout_step_name,
-            keyid=keys["carl_pub"]["keyid"])
+        bobs_layout_link_dir = SUBLAYOUT_LINK_DIR_FORMAT.format(
+            name=root_layout_step_name, keyid=keys["bob_pub"]["keyid"]
+        )
+        os.mkdir(bobs_layout_link_dir)
 
-    carls_layout_path = os.path.join(bobs_layout_link_dir, carls_layout_name)
-    carls_layout = Metablock(signed=Layout())
-    carls_layout.sign(keys["carl_priv"])
-    carls_layout.dump(carls_layout_path)
+        bobs_layout_step_name = "delegated-to-carl"
 
-    in_toto_verify(root_layout, root_layout_pub_key_dict)
+        bobs_layout = Metablock(
+            signed=Layout(
+                keys={keys["carl_pub"]["keyid"]: keys["carl_pub"]},
+                steps=[
+                    Step(
+                        name=bobs_layout_step_name,
+                        pubkeys=[keys["carl_pub"]["keyid"]],
+                    )
+                ],
+            )
+        )
+        bobs_layout.sign(keys["bob_priv"])
+        bobs_layout.dump(bobs_layout_name)
+
+        # Subsublayout (second level)
+        # The subsublayout will be placed in the namespaced link dir
+        # of its superlayout (sublayout from the root layout's perspective), for
+        # for which it serves as link.
+        carls_layout_name = FILENAME_FORMAT.format(
+            step_name=bobs_layout_step_name, keyid=keys["carl_pub"]["keyid"]
+        )
 
-    self.tear_down_test_dir()
+        carls_layout_path = os.path.join(
+            bobs_layout_link_dir, carls_layout_name
+        )
+        carls_layout = Metablock(signed=Layout())
+        carls_layout.sign(keys["carl_priv"])
+        carls_layout.dump(carls_layout_path)
+
+        in_toto_verify(root_layout, root_layout_pub_key_dict)
+
+        self.tear_down_test_dir()
 
 
 class TestSublayoutVerificationMatchRule(unittest.TestCase, TmpDirMixin):
-  """Tests a sublayout and checks if a MATCH rule is successful after sublayout
-  is resolved into a summary link."""
+    """Tests a sublayout and checks if a MATCH rule is successful after sublayout
+    is resolved into a summary link."""
+
+    def test_verify_sublayout_match_rule(self):
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
+
+        script_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "scripts"
+        )
+
+        # Create and change into temporary directory
+        self.set_up_test_dir()
+
+        # We don't need to copy the demo files, we just load the keys
+        keys = {}
+        for key_name in ["alice", "bob"]:
+            keys[key_name + "_priv"] = import_rsa_privatekey_from_file(
+                os.path.join(demo_files, key_name)
+            )
+            keys[key_name + "_pub"] = import_rsa_publickey_from_file(
+                os.path.join(demo_files, key_name + ".pub")
+            )
+
+        # Create layout hierarchy
+
+        # Root layout
+        # The root layout is the layout that will be passed to `in_toto_verify`
+        # It only has one step which is a sublayout, into which verification
+        # recurses. Only the root layout and root layout verification key will be
+        # passed to verification.
+        root_layout_pub_key_dict = {
+            keys["alice_pub"]["keyid"]: keys["alice_pub"]
+        }
+
+        root_layout_step_name = "delegated-to-bob"
+
+        root_layout = Metablock(
+            signed=Layout(
+                keys={keys["bob_pub"]["keyid"]: keys["bob_pub"]},
+                steps=[
+                    Step(
+                        name=root_layout_step_name,
+                        pubkeys=[keys["bob_pub"]["keyid"]],
+                        expected_products=[
+                            [
+                                "MATCH",
+                                "foo.tar.gz",
+                                "WITH",
+                                "PRODUCTS",
+                                "FROM",
+                                root_layout_step_name,
+                            ],
+                            ["DISALLOW", "*"],
+                        ],
+                    )
+                ],
+            )
+        )
+        root_layout.sign(keys["alice_priv"])
+
+        # Sublayout (first level)
+        # The sublayout will be treated as a link from the superlayout's
+        # perspective and loaded from the current working directory. The links for
+        # the steps of this sublayout will be placed in a namespaced subdir.
+        bobs_layout_name = FILENAME_FORMAT.format(
+            step_name=root_layout_step_name, keyid=keys["bob_pub"]["keyid"]
+        )
 
-  def test_verify_sublayout_match_rule(self):
-    # Find demo files
-    demo_files = os.path.join(
-      os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    script_files = os.path.join(
-      os.path.dirname(os.path.realpath(__file__)), "scripts")
-
-    # Create and change into temporary directory
-    self.set_up_test_dir()
-
-    # We don't need to copy the demo files, we just load the keys
-    keys = {}
-    for key_name in ["alice", "bob"]:
-      keys[key_name + "_priv"] = import_rsa_privatekey_from_file(
-        os.path.join(demo_files, key_name))
-      keys[key_name + "_pub"] = import_rsa_publickey_from_file(
-        os.path.join(demo_files, key_name + ".pub"))
-
-    # Create layout hierarchy
-
-    # Root layout
-    # The root layout is the layout that will be passed to `in_toto_verify`
-    # It only has one step which is a sublayout, into which verification
-    # recurses. Only the root layout and root layout verification key will be
-    # passed to verification.
-    root_layout_pub_key_dict = {
-      keys["alice_pub"]["keyid"]: keys["alice_pub"]
-    }
-
-    root_layout_step_name = "delegated-to-bob"
-
-    root_layout = Metablock(signed=Layout(
-      keys={
-        keys["bob_pub"]["keyid"]: keys["bob_pub"]
-      },
-      steps=[
-        Step(
-          name=root_layout_step_name,
-          pubkeys=[
-            keys["bob_pub"]["keyid"]
-          ],
-          expected_products=[["MATCH", "foo.tar.gz", "WITH", "PRODUCTS",
-              "FROM", root_layout_step_name], ["DISALLOW", "*"]]
-        )
-      ]
-    )
-    )
-    root_layout.sign(keys["alice_priv"])
-
-
-    # Sublayout (first level)
-    # The sublayout will be treated as a link from the superlayout's
-    # perspective and loaded from the current working directory. The links for
-    # the steps of this sublayout will be placed in a namespaced subdir.
-    bobs_layout_name = FILENAME_FORMAT.format(
-      step_name=root_layout_step_name,
-      keyid=keys["bob_pub"]["keyid"])
-
-    bobs_layout_link_dir = SUBLAYOUT_LINK_DIR_FORMAT.format(
-      name=root_layout_step_name,
-      keyid=keys["bob_pub"]["keyid"])
-    os.mkdir(bobs_layout_link_dir)
-
-    bobs_layout = Metablock.load(os.path.join(demo_files, "demo.layout.template"))
-    bobs_layout.sign(keys["bob_priv"])
-    bobs_layout.dump(bobs_layout_name)
-    shutil.copy2(os.path.join(demo_files, "write-code.776a00e2.link"), bobs_layout_link_dir)
-    shutil.copy2(os.path.join(demo_files, "package.2f89b927.link"), bobs_layout_link_dir)
-    shutil.copy2(os.path.join(demo_files, "foo.tar.gz"), ".")
-    shutil.copytree(script_files, os.path.join(".", "scripts"))
+        bobs_layout_link_dir = SUBLAYOUT_LINK_DIR_FORMAT.format(
+            name=root_layout_step_name, keyid=keys["bob_pub"]["keyid"]
+        )
+        os.mkdir(bobs_layout_link_dir)
 
-    in_toto_verify(root_layout, root_layout_pub_key_dict)
+        bobs_layout = Metablock.load(
+            os.path.join(demo_files, "demo.layout.template")
+        )
+        bobs_layout.sign(keys["bob_priv"])
+        bobs_layout.dump(bobs_layout_name)
+        shutil.copy2(
+            os.path.join(demo_files, "write-code.776a00e2.link"),
+            bobs_layout_link_dir,
+        )
+        shutil.copy2(
+            os.path.join(demo_files, "package.2f89b927.link"),
+            bobs_layout_link_dir,
+        )
+        shutil.copy2(os.path.join(demo_files, "foo.tar.gz"), ".")
+        shutil.copytree(script_files, os.path.join(".", "scripts"))
 
-    self.tear_down_test_dir()
+        in_toto_verify(root_layout, root_layout_pub_key_dict)
 
+        self.tear_down_test_dir()
 
 
 class TestGetSummaryLink(unittest.TestCase, TmpDirMixin):
-  """Tests verifylib.get_summary_link(layout, reduced_chain_link_dict).
-  Pass two step demo layout and according link files and verify the
-  returned summary link.
-  """
-
-  @classmethod
-  def setUpClass(self):
-    """Creates and changes into temporary directory and prepares two layouts.
-    The superlayout, which has one step and its sublayout, which is the usual
-    demo layout (write code, package, inspect tar). """
-
-    # Find demo files
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "demo_files")
-
-    # Create and change into temporary directory
-    self.set_up_test_dir()
-
-    # Copy demo files to temp dir
-    for fn in os.listdir(demo_files):
-      shutil.copy(os.path.join(demo_files, fn), self.test_dir)
-
-    self.demo_layout = Metablock.load("demo.layout.template")
-    self.code_link = Metablock.load("package.2f89b927.link")
-    self.package_link = Metablock.load("write-code.776a00e2.link")
-    self.demo_links = {
-        "write-code": self.code_link.signed,
-        "package": self.package_link.signed
-      }
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-  def test_get_summary_link_from_demo_layout(self):
-    """Create summary link from demo link files and compare properties. """
-    sum_link = get_summary_link(self.demo_layout.signed, self.demo_links, "")
-
-    self.assertEqual(sum_link._type, self.code_link.signed._type)
-    self.assertEqual(sum_link.name, "")
-    self.assertEqual(sum_link.materials, self.code_link.signed.materials)
-
-    self.assertEqual(sum_link.products, self.package_link.signed.products)
-    self.assertEqual(sum_link.command, self.package_link.signed.command)
-    self.assertEqual(sum_link.byproducts, self.package_link.signed.byproducts)
-    self.assertEqual(sum_link.byproducts.get("return-value"),
-        self.package_link.signed.byproducts.get("return-value"))
+    """Tests verifylib.get_summary_link(layout, reduced_chain_link_dict).
+    Pass two step demo layout and according link files and verify the
+    returned summary link.
+    """
+
+    @classmethod
+    def setUpClass(self):
+        """Creates and changes into temporary directory and prepares two layouts.
+        The superlayout, which has one step and its sublayout, which is the usual
+        demo layout (write code, package, inspect tar)."""
+
+        # Find demo files
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "demo_files"
+        )
 
+        # Create and change into temporary directory
+        self.set_up_test_dir()
+
+        # Copy demo files to temp dir
+        for fn in os.listdir(demo_files):
+            shutil.copy(os.path.join(demo_files, fn), self.test_dir)
+
+        self.demo_layout = Metablock.load("demo.layout.template")
+        self.code_link = Metablock.load("package.2f89b927.link")
+        self.package_link = Metablock.load("write-code.776a00e2.link")
+        self.demo_links = {
+            "write-code": self.code_link.signed,
+            "package": self.package_link.signed,
+        }
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_get_summary_link_from_demo_layout(self):
+        """Create summary link from demo link files and compare properties."""
+        sum_link = get_summary_link(
+            self.demo_layout.signed, self.demo_links, ""
+        )
+
+        self.assertEqual(sum_link._type, self.code_link.signed._type)
+        self.assertEqual(sum_link.name, "")
+        self.assertEqual(sum_link.materials, self.code_link.signed.materials)
+
+        self.assertEqual(sum_link.products, self.package_link.signed.products)
+        self.assertEqual(sum_link.command, self.package_link.signed.command)
+        self.assertEqual(
+            sum_link.byproducts, self.package_link.signed.byproducts
+        )
+        self.assertEqual(
+            sum_link.byproducts.get("return-value"),
+            self.package_link.signed.byproducts.get("return-value"),
+        )
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/demo_dsse_files/demo.layout.template` & `in_toto-2.0.0/tests/demo_dsse_files/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_dsse_files/package.2f89b927.link` & `in_toto-2.0.0/tests/demo_dsse_files/package.2f89b927.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_dsse_files/write-code.776a00e2.link` & `in_toto-2.0.0/tests/demo_dsse_files/write-code.776a00e2.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files/alice` & `in_toto-2.0.0/tests/demo_files/alice`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files/alice.pub` & `in_toto-2.0.0/tests/demo_files/alice.pub`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files/bob` & `in_toto-2.0.0/tests/demo_files/bob`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files/bob.pub` & `in_toto-2.0.0/tests/demo_files/bob.pub`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files/carl` & `in_toto-2.0.0/tests/demo_files/carl`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files/carl.pub` & `in_toto-2.0.0/tests/demo_files/carl.pub`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files/demo.layout.template` & `in_toto-2.0.0/tests/demo_files/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files/package.2f89b927.link` & `in_toto-2.0.0/tests/demo_files/package.2f89b927.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files/write-code.776a00e2.link` & `in_toto-2.0.0/tests/demo_files/write-code.776a00e2.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files_gpg/demo.layout.template` & `in_toto-2.0.0/tests/demo_files_gpg/demo.layout.template`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files_gpg/package.7b3abb26.link` & `in_toto-2.0.0/tests/demo_files_gpg/package.7b3abb26.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/demo_files_gpg/write-code.8288ef56.link` & `in_toto-2.0.0/tests/demo_files_gpg/write-code.8288ef56.link`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh` & `in_toto-2.0.0/tests/gpg_keyrings/dsa/C242A830DAAF1C2BEF604A9EF033A3A3E267B3B1.ssh`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/gpg_keyrings/dsa/pubring.gpg` & `in_toto-2.0.0/tests/gpg_keyrings/dsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/gpg_keyrings/dsa/random_seed` & `in_toto-2.0.0/tests/gpg_keyrings/dsa/random_seed`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/gpg_keyrings/dsa/secring.gpg` & `in_toto-2.0.0/tests/gpg_keyrings/dsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/gpg_keyrings/dsa/trustdb.gpg` & `in_toto-2.0.0/tests/gpg_keyrings/dsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/gpg_keyrings/rsa/pubring.gpg` & `in_toto-2.0.0/tests/gpg_keyrings/rsa/pubring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/gpg_keyrings/rsa/random_seed` & `in_toto-2.0.0/tests/gpg_keyrings/rsa/random_seed`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/gpg_keyrings/rsa/secring.gpg` & `in_toto-2.0.0/tests/gpg_keyrings/rsa/secring.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/gpg_keyrings/rsa/trustdb.gpg` & `in_toto-2.0.0/tests/gpg_keyrings/rsa/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/tests/models/test_common.py` & `in_toto-2.0.0/tests/models/test_common.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,20 +17,23 @@
   See LICENSE for licensing information.
 
 <Purpose>
   Test the Signable and ValidationMixin class functions.
 
 """
 
-import unittest
 import json
+import unittest
+
 from in_toto.models.common import Signable
 
+
 class TestSignable(unittest.TestCase):
-  """ Verifies Signable class. """
+    """Verifies Signable class."""
+
+    def test_load_repr_string_as_json(self):
+        """Test load string returned by `Signable.repr` as JSON"""
+        json.loads(repr(Signable()))
 
-  def test_load_repr_string_as_json(self):
-    """Test load string returned by `Signable.repr` as JSON  """
-    json.loads(repr(Signable()))
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/models/test_envelope.py` & `in_toto-2.0.0/tests/models/test_envelope.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,58 +20,59 @@
   Test in_toto.models.metadata.Envelope class methods.
 
 """
 
 import os
 import unittest
 
-from in_toto.models.metadata import Envelope
 from in_toto.models.layout import Layout
 from in_toto.models.link import Link
-
+from in_toto.models.metadata import Envelope
 from tests.common import TmpDirMixin
 
+
 class TestMetablockValidator(unittest.TestCase, TmpDirMixin):
-  """Test in_toto.models.metadata.Envelope methods. """
+    """Test in_toto.models.metadata.Envelope methods."""
 
-  def test_create_envelope(self):
-    """Test DSSE envelope creation from Link or Layout."""
+    def test_create_envelope(self):
+        """Test DSSE envelope creation from Link or Layout."""
 
-    # Create DSSE Envelope from empty Link.
-    link = Link()
-    env = Envelope.from_signable(link)
+        # Create DSSE Envelope from empty Link.
+        link = Link()
+        env = Envelope.from_signable(link)
 
-    # Verify links.
-    self.assertEqual(env.get_payload(), link)
+        # Verify links.
+        self.assertEqual(env.get_payload(), link)
 
-    # Create DSSE Envelope from empty Layout.
-    layout = Layout()
-    env = Envelope.from_signable(layout)
+        # Create DSSE Envelope from empty Layout.
+        layout = Layout()
+        env = Envelope.from_signable(layout)
 
-    # Verify layouts.
-    self.assertEqual(env.get_payload(), layout)
+        # Verify layouts.
+        self.assertEqual(env.get_payload(), layout)
 
-  def test_load_envelope(self):
-    """Test loading and parsing of in-toto envelope."""
+    def test_load_envelope(self):
+        """Test loading and parsing of in-toto envelope."""
 
-    # Demo DSSE Metadata Files
-    demo_dsse_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "../demo_dsse_files")
+        # Demo DSSE Metadata Files
+        demo_dsse_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "../demo_dsse_files"
+        )
 
-    layout_path = os.path.join(demo_dsse_files, "demo.layout.template")
-    link_path = os.path.join(demo_dsse_files, "package.2f89b927.link")
+        layout_path = os.path.join(demo_dsse_files, "demo.layout.template")
+        link_path = os.path.join(demo_dsse_files, "package.2f89b927.link")
 
-    # Load layout metadata.
-    env = Envelope.load(layout_path)
-    layout = env.get_payload()
+        # Load layout metadata.
+        env = Envelope.load(layout_path)
+        layout = env.get_payload()
 
-    self.assertIsInstance(layout, Layout)
+        self.assertIsInstance(layout, Layout)
 
-    # Load link metadata.
-    env = Envelope.load(link_path)
-    link = env.get_payload()
+        # Load link metadata.
+        env = Envelope.load(link_path)
+        link = env.get_payload()
 
-    self.assertIsInstance(link, Link)
+        self.assertIsInstance(link, Link)
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/models/test_inspection.py` & `in_toto-2.0.0/tests/models/test_inspection.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,55 +18,56 @@
 
 <Purpose>
   Test inspection class functions.
 
 """
 
 import unittest
-from in_toto.models.layout import Inspection
+
 import securesystemslib.exceptions
 
-class TestInspectionValidator(unittest.TestCase):
-  """Test verifylib.verify_delete_rule(rule, artifact_queue) """
+from in_toto.models.layout import Inspection
 
-  def setUp(self):
-    """Populate a base layout that we can use."""
-    self.inspection = Inspection(name="some-inspection")
 
-  def test_wrong_type(self):
-    """Test the type field within Validate()."""
+class TestInspectionValidator(unittest.TestCase):
+    """Test verifylib.verify_delete_rule(rule, artifact_queue)"""
 
-    self.inspection._type = "wrong"
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.inspection._validate_type()
+    def setUp(self):
+        """Populate a base layout that we can use."""
+        self.inspection = Inspection(name="some-inspection")
 
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.inspection.validate()
+    def test_wrong_type(self):
+        """Test the type field within Validate()."""
 
-    self.inspection._type = "inspection"
-    self.inspection._validate_type()
+        self.inspection._type = "wrong"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.inspection._validate_type()
 
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.inspection.validate()
 
-  def test_wrong_run(self):
-    """Test that the run validators catch malformed values."""
+        self.inspection._type = "inspection"
+        self.inspection._validate_type()
 
-    self.inspection.run = -1
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.inspection._validate_run()
+    def test_wrong_run(self):
+        """Test that the run validators catch malformed values."""
 
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.inspection.validate()
+        self.inspection.run = -1
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.inspection._validate_run()
 
-    self.inspection.run = ["somecommand"]
-    self.inspection._validate_run()
-    self.inspection.validate()
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.inspection.validate()
 
+        self.inspection.run = ["somecommand"]
+        self.inspection._validate_run()
+        self.inspection.validate()
 
-  def test_set_run_from_string(self):
-    """Test shelx parse command string to list. """
-    inspection = Inspection()
-    inspection.set_run_from_string("echo 'foo bar'")
-    self.assertListEqual(inspection.run, ["echo", "foo bar"])
+    def test_set_run_from_string(self):
+        """Test shelx parse command string to list."""
+        inspection = Inspection()
+        inspection.set_run_from_string("echo 'foo bar'")
+        self.assertListEqual(inspection.run, ["echo", "foo bar"])
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/models/test_layout.py` & `in_toto-2.0.0/tests/models/test_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,384 +18,371 @@
 
 <Purpose>
   Test layout class functions.
 
 """
 
 import os
-import unittest
 import shutil
+import unittest
+
+import securesystemslib.exceptions
 
-from in_toto.models.layout import Layout, Step, Inspection
-from in_toto.models.metadata import Metablock
-import in_toto.models.link
 import in_toto.exceptions
+import in_toto.models.link
 import in_toto.verifylib
-import securesystemslib.exceptions
+from in_toto.models.layout import Inspection, Layout, Step
+from in_toto.models.metadata import Metablock
+from tests.common import GPGKeysMixin, TmpDirMixin
 
-from tests.common import TmpDirMixin, GPGKeysMixin
 
 class TestLayoutMethods(unittest.TestCase, TmpDirMixin, GPGKeysMixin):
-  """Test Layout methods. """
-
-  @classmethod
-  def setUpClass(self):
-    """Create temporary test directory and copy gpg keychain, and rsa keys from
-    demo files. """
-    demo_files = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)), "..", "demo_files")
-
-    self.set_up_test_dir()
-    self.set_up_gpg_keys()
-
-
-    # Copy keys to temp test dir
-    key_names = ["bob", "bob.pub", "carl.pub"]
-    for name in key_names:
-      shutil.copy(os.path.join(demo_files, name), name)
-
-    self.key_path = os.path.join(self.test_dir, "bob")
-    self.pubkey_path1 = os.path.join(self.test_dir, "bob.pub")
-    self.pubkey_path2 = os.path.join(self.test_dir, "carl.pub")
-
-
-  @classmethod
-  def tearDownClass(self):
-    self.tear_down_test_dir()
-
-
-  def test_set_relative_expiration(self):
-    """Test adding expiration date relative from today. """
-    layout = Layout()
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.set_relative_expiration(days=None, months=0, years=0)
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.set_relative_expiration(days=0, months="", years=0)
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.set_relative_expiration(days=0, months=0, years=[])
-
-    layout.set_relative_expiration(days=1)
-    layout._validate_expires()
-    layout.set_relative_expiration(months=2)
-    layout._validate_expires()
-    layout.set_relative_expiration(years=3)
-    layout._validate_expires()
-    layout.set_relative_expiration(days=3, months=2, years=1)
-    layout._validate_expires()
-
-    # It's possible to add an expiration date in the past
-    layout.set_relative_expiration(days=-3, months=-2, years=-1)
-    layout._validate_expires()
-
-
-  def test_get_step_name_list(self):
-    """Test getting list of step names. """
-    names = ["a", "b", "c"]
-    layout = Layout(steps=[Step(name=name) for name in names])
-    self.assertListEqual(layout.get_step_name_list(), names)
-
-
-  def test_get_step_by_name(self):
-    """Test getting step by name. """
-    names = ["a", "b", "c"]
-    layout = Layout(steps=[Step(name=name) for name in names])
-    self.assertEqual(layout.get_step_by_name("b").name, "b")
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.get_step_by_name(None)
-
-
-  def test_remove_step_by_name(self):
-    """Test removing step by name. """
-    names = ["a", "b", "c"]
-    layout = Layout(steps=[Step(name=name) for name in names])
-
-    self.assertEqual(len(layout.steps), 3)
-    self.assertTrue("b" in layout.get_step_name_list())
-    # Items are only removed if they exist
-    for _ in range(2):
-      layout.remove_step_by_name("b")
-      self.assertEqual(len(layout.steps), 2)
-      self.assertTrue("b" not in layout.get_step_name_list())
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.get_step_by_name([])
-
-
-  def test_get_inspection_name_list(self):
-    """Test getting list of inspection names. """
-    names = ["a", "b", "c"]
-    layout = Layout(inspect=[Inspection(name=name) for name in names])
-    self.assertListEqual(layout.get_inspection_name_list(), names)
-
-
-  def test_get_inspection_by_name(self):
-    """Test getting inspection by name. """
-    names = ["a", "b", "c"]
-    layout = Layout(inspect=[Inspection(name=name) for name in names])
-    self.assertEqual(layout.get_inspection_by_name("b").name, "b")
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.get_inspection_by_name(1)
-
-
-  def test_remove_inspection_by_name(self):
-    """Test removing inspection by name. """
-    names = ["a", "b", "c"]
-    layout = Layout(inspect=[Inspection(name=name) for name in names])
-
-    self.assertEqual(len(layout.inspect), 3)
-    self.assertTrue("b" in layout.get_inspection_name_list())
-    # Items are only removed if they exist
-    for _ in range(2):
-      layout.remove_inspection_by_name("b")
-      self.assertEqual(len(layout.inspect), 2)
-      self.assertTrue("b" not in layout.get_inspection_name_list())
-
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.remove_inspection_by_name(False)
-
-
-  def test_functionary_keys(self):
-    """Test adding and listing functionary keys (securesystemslib and gpg). """
-    layout = Layout()
-    self.assertEqual(len(layout.get_functionary_key_id_list()), 0)
-
-    layout.add_functionary_keys_from_paths([self.pubkey_path1,
-        self.pubkey_path2])
-
-    layout.add_functionary_keys_from_gpg_keyids([self.gpg_key_768C43,
-        self.gpg_key_85DA58], gpg_home=self.gnupg_home)
-
-    layout._validate_keys()
-
-    self.assertEqual(len(layout.get_functionary_key_id_list()), 4)
-
-    # Must be a valid key object
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.add_functionary_key("abcd")
-
-    # Must be pubkey and not private key
-    with self.assertRaises(securesystemslib.exceptions.Error):
-      layout.add_functionary_key_from_path(self.key_path)
-
-    # Must be a valid path
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.add_functionary_key_from_path(123)
-
-    # Must be a valid keyid
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.add_functionary_key_from_gpg_keyid("abcdefg")
-
-    # Must be a list of paths
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.add_functionary_keys_from_paths("abcd")
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.add_functionary_keys_from_paths([1])
-
-    # Must be a list of keyids
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.add_functionary_keys_from_gpg_keyids(None)
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      layout.add_functionary_keys_from_gpg_keyids(["abcdefg"])
+    """Test Layout methods."""
 
+    @classmethod
+    def setUpClass(self):
+        """Create temporary test directory and copy gpg keychain, and rsa keys from
+        demo files."""
+        demo_files = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)), "..", "demo_files"
+        )
+
+        self.set_up_test_dir()
+        self.set_up_gpg_keys()
+
+        # Copy keys to temp test dir
+        key_names = ["bob", "bob.pub", "carl.pub"]
+        for name in key_names:
+            shutil.copy(os.path.join(demo_files, name), name)
+
+        self.key_path = os.path.join(self.test_dir, "bob")
+        self.pubkey_path1 = os.path.join(self.test_dir, "bob.pub")
+        self.pubkey_path2 = os.path.join(self.test_dir, "carl.pub")
+
+    @classmethod
+    def tearDownClass(self):
+        self.tear_down_test_dir()
+
+    def test_set_relative_expiration(self):
+        """Test adding expiration date relative from today."""
+        layout = Layout()
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.set_relative_expiration(days=None, months=0, years=0)
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.set_relative_expiration(days=0, months="", years=0)
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.set_relative_expiration(days=0, months=0, years=[])
+
+        layout.set_relative_expiration(days=1)
+        layout._validate_expires()
+        layout.set_relative_expiration(months=2)
+        layout._validate_expires()
+        layout.set_relative_expiration(years=3)
+        layout._validate_expires()
+        layout.set_relative_expiration(days=3, months=2, years=1)
+        layout._validate_expires()
+
+        # It's possible to add an expiration date in the past
+        layout.set_relative_expiration(days=-3, months=-2, years=-1)
+        layout._validate_expires()
+
+    def test_get_step_name_list(self):
+        """Test getting list of step names."""
+        names = ["a", "b", "c"]
+        layout = Layout(steps=[Step(name=name) for name in names])
+        self.assertListEqual(layout.get_step_name_list(), names)
+
+    def test_get_step_by_name(self):
+        """Test getting step by name."""
+        names = ["a", "b", "c"]
+        layout = Layout(steps=[Step(name=name) for name in names])
+        self.assertEqual(layout.get_step_by_name("b").name, "b")
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.get_step_by_name(None)
+
+    def test_remove_step_by_name(self):
+        """Test removing step by name."""
+        names = ["a", "b", "c"]
+        layout = Layout(steps=[Step(name=name) for name in names])
+
+        self.assertEqual(len(layout.steps), 3)
+        self.assertTrue("b" in layout.get_step_name_list())
+        # Items are only removed if they exist
+        for _ in range(2):
+            layout.remove_step_by_name("b")
+            self.assertEqual(len(layout.steps), 2)
+            self.assertTrue("b" not in layout.get_step_name_list())
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.get_step_by_name([])
+
+    def test_get_inspection_name_list(self):
+        """Test getting list of inspection names."""
+        names = ["a", "b", "c"]
+        layout = Layout(inspect=[Inspection(name=name) for name in names])
+        self.assertListEqual(layout.get_inspection_name_list(), names)
+
+    def test_get_inspection_by_name(self):
+        """Test getting inspection by name."""
+        names = ["a", "b", "c"]
+        layout = Layout(inspect=[Inspection(name=name) for name in names])
+        self.assertEqual(layout.get_inspection_by_name("b").name, "b")
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.get_inspection_by_name(1)
+
+    def test_remove_inspection_by_name(self):
+        """Test removing inspection by name."""
+        names = ["a", "b", "c"]
+        layout = Layout(inspect=[Inspection(name=name) for name in names])
+
+        self.assertEqual(len(layout.inspect), 3)
+        self.assertTrue("b" in layout.get_inspection_name_list())
+        # Items are only removed if they exist
+        for _ in range(2):
+            layout.remove_inspection_by_name("b")
+            self.assertEqual(len(layout.inspect), 2)
+            self.assertTrue("b" not in layout.get_inspection_name_list())
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.remove_inspection_by_name(False)
+
+    def test_functionary_keys(self):
+        """Test adding and listing functionary keys (securesystemslib and gpg)."""
+        layout = Layout()
+        self.assertEqual(len(layout.get_functionary_key_id_list()), 0)
+
+        layout.add_functionary_keys_from_paths(
+            [self.pubkey_path1, self.pubkey_path2]
+        )
+
+        layout.add_functionary_keys_from_gpg_keyids(
+            [self.gpg_key_768C43, self.gpg_key_85DA58], gpg_home=self.gnupg_home
+        )
+
+        layout._validate_keys()
+
+        self.assertEqual(len(layout.get_functionary_key_id_list()), 4)
+
+        # Must be a valid key object
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.add_functionary_key("abcd")
+
+        # Must be pubkey and not private key
+        with self.assertRaises(securesystemslib.exceptions.Error):
+            layout.add_functionary_key_from_path(self.key_path)
+
+        # Must be a valid path
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.add_functionary_key_from_path(123)
+
+        # Must be a valid keyid
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.add_functionary_key_from_gpg_keyid("abcdefg")
+
+        # Must be a list of paths
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.add_functionary_keys_from_paths("abcd")
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.add_functionary_keys_from_paths([1])
+
+        # Must be a list of keyids
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.add_functionary_keys_from_gpg_keyids(None)
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            layout.add_functionary_keys_from_gpg_keyids(["abcdefg"])
 
 
 class TestLayoutValidator(unittest.TestCase):
-  """Test in_toto.models.layout.Layout validators. """
-
-
-  def setUp(self):
-    """Populate a base layout that we can use."""
-    self.layout = Layout()
-    self.layout.expires = '2016-11-18T16:44:55Z'
-
-
-  def test_wrong_type(self):
-    """Test that the type field is validated properly."""
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout._type = "wrong"
-      self.layout._validate_type()
-      self.layout.validate()
-
-    self.layout._type = "layout"
-    self.layout._validate_type()
-
-
-  def test_validate_readme_field(self):
-    """Tests the readme field data type validator. """
-    self.layout.readme = 1
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout._validate_readme()
-
-    self.layout.readme = "This is a test supply chain"
-    self.layout._validate_readme()
-
-
-  def test_wrong_expires(self):
-    """Test the expires field is properly populated."""
-
-    self.layout.expires = ''
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout._validate_expires()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    self.layout.expires = '-1'
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout._validate_expires()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    # notice the wrong month
-    self.layout.expires = '2016-13-18T16:44:55Z'
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout._validate_expires()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    self.layout.expires = '2016-11-18T16:44:55Z'
-    self.layout._validate_expires()
-    self.layout.validate()
-
-
-  def test_wrong_key_dictionary(self):
-    """Test that the keys dictionary is properly populated."""
-    rsa_key_one = securesystemslib.keys.generate_rsa_key()
-    rsa_key_two = securesystemslib.keys.generate_rsa_key()
-
-    # FIXME: attr.ib reutilizes the default dictionary, so future constructor
-    # are not empty...
-    self.layout.keys = {"kek": rsa_key_one}
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout._validate_keys()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    self.layout.keys = {}
-    self.layout.keys[rsa_key_two['keyid']] = "kek"
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout._validate_keys()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    self.layout.keys = {}
-    del rsa_key_one["keyval"]["private"]
-    del rsa_key_two["keyval"]["private"]
-    self.layout.keys[rsa_key_one['keyid']] = rsa_key_one
-    self.layout.keys[rsa_key_two['keyid']] = rsa_key_two
-
-    self.layout._validate_keys()
-    self.layout.validate()
-
-
-  def test_wrong_steps_list(self):
-    """Check that the validate method checks the steps' correctness."""
-    self.layout.steps = "not-a-step"
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    self.layout.steps = ["not-a-step"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    test_step = Step(name="this-is-a-step")
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      test_step.expected_materials = ['this is a malformed step']
-      self.layout.steps = [test_step]
-      self.layout.validate()
-
-    test_step = Step(name="this-is-a-step")
-    test_step.expected_materials = [["CREATE", "foo"]]
-    test_step.threshold = 1
-    self.layout.steps = [test_step]
-    self.layout.validate()
-
-
-  def test_wrong_inspect_list(self):
-    """Check that the validate method checks the inspections' correctness."""
-
-    self.layout.inspect = "not-an-inspection"
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    self.layout.inspect = ["not-an-inspection"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    test_inspection = Inspection(name="this-is-a-step")
-    test_inspection.expected_materials = ['this is a malformed artifact rule']
-    self.layout.inspect = [test_inspection]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    test_inspection = Inspection(name="this-is-a-step")
-    test_inspection.expected_materials = [["CREATE", "foo"]]
-    self.layout.inspect = [test_inspection]
-    self.layout.validate()
-
-
-  def test_repeated_step_names(self):
-    """Check that only unique names exist in the steps and inspect lists"""
-
-    self.layout.steps = [Step(name="name"), Step(name="name")]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    self.layout.steps = [Step(name="name")]
-    self.layout.inspect = [Inspection(name="name")]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.layout.validate()
-
-    self.layout.step = [Step(name="name"), Step(name="othername")]
-    self.layout.inspect = [Inspection(name="thirdname")]
-    self.layout.validate()
-
-
-  def test_import_step_metadata_wrong_type(self):
-    functionary_key = securesystemslib.keys.generate_rsa_key()
-    name = "name"
-
-    # Create and dump a link file with a wrong type
-    link_name = in_toto.models.link.FILENAME_FORMAT.format(
-        step_name=name, keyid=functionary_key["keyid"])
-
-    link_path = os.path.abspath(link_name)
-    link = in_toto.models.link.Link(name=name)
-    metadata = Metablock(signed=link)
-    metadata.signed._type = "wrong-type"
-    metadata.dump(link_path)
-
-    # Add the single step to the test layout and try to read the failing link
-    self.layout.steps.append(Step(
-        name=name, pubkeys=[functionary_key["keyid"]]))
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      in_toto.verifylib.load_links_for_layout(self.layout, ".")
-
-    # Clean up
-    os.remove(link_path)
-
+    """Test in_toto.models.layout.Layout validators."""
 
-  def test_wrong_pubkeys(self):
-    """Check validate pubkeys fails with wrong keys."""
-    # Pubkeys must be lists ...
-    tmp_step = Step()
-    tmp_step.pubkeys = "abcd"
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      tmp_step.validate()
+    def setUp(self):
+        """Populate a base layout that we can use."""
+        self.layout = Layout()
+        self.layout.expires = "2016-11-18T16:44:55Z"
+
+    def test_wrong_type(self):
+        """Test that the type field is validated properly."""
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout._type = "wrong"
+            self.layout._validate_type()
+            self.layout.validate()
+
+        self.layout._type = "layout"
+        self.layout._validate_type()
+
+    def test_validate_readme_field(self):
+        """Tests the readme field data type validator."""
+        self.layout.readme = 1
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout._validate_readme()
+
+        self.layout.readme = "This is a test supply chain"
+        self.layout._validate_readme()
+
+    def test_wrong_expires(self):
+        """Test the expires field is properly populated."""
+
+        self.layout.expires = ""
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout._validate_expires()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        self.layout.expires = "-1"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout._validate_expires()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        # notice the wrong month
+        self.layout.expires = "2016-13-18T16:44:55Z"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout._validate_expires()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        self.layout.expires = "2016-11-18T16:44:55Z"
+        self.layout._validate_expires()
+        self.layout.validate()
+
+    def test_wrong_key_dictionary(self):
+        """Test that the keys dictionary is properly populated."""
+        rsa_key_one = securesystemslib.keys.generate_rsa_key()
+        rsa_key_two = securesystemslib.keys.generate_rsa_key()
+
+        # FIXME: attr.ib reutilizes the default dictionary, so future constructor
+        # are not empty...
+        self.layout.keys = {"kek": rsa_key_one}
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout._validate_keys()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        self.layout.keys = {}
+        self.layout.keys[rsa_key_two["keyid"]] = "kek"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout._validate_keys()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        self.layout.keys = {}
+        del rsa_key_one["keyval"]["private"]
+        del rsa_key_two["keyval"]["private"]
+        self.layout.keys[rsa_key_one["keyid"]] = rsa_key_one
+        self.layout.keys[rsa_key_two["keyid"]] = rsa_key_two
+
+        self.layout._validate_keys()
+        self.layout.validate()
+
+    def test_wrong_steps_list(self):
+        """Check that the validate method checks the steps' correctness."""
+        self.layout.steps = "not-a-step"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        self.layout.steps = ["not-a-step"]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        test_step = Step(name="this-is-a-step")
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            test_step.expected_materials = ["this is a malformed step"]
+            self.layout.steps = [test_step]
+            self.layout.validate()
+
+        test_step = Step(name="this-is-a-step")
+        test_step.expected_materials = [["CREATE", "foo"]]
+        test_step.threshold = 1
+        self.layout.steps = [test_step]
+        self.layout.validate()
+
+    def test_wrong_inspect_list(self):
+        """Check that the validate method checks the inspections' correctness."""
+
+        self.layout.inspect = "not-an-inspection"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        self.layout.inspect = ["not-an-inspection"]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        test_inspection = Inspection(name="this-is-a-step")
+        test_inspection.expected_materials = [
+            "this is a malformed artifact rule"
+        ]
+        self.layout.inspect = [test_inspection]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        test_inspection = Inspection(name="this-is-a-step")
+        test_inspection.expected_materials = [["CREATE", "foo"]]
+        self.layout.inspect = [test_inspection]
+        self.layout.validate()
+
+    def test_repeated_step_names(self):
+        """Check that only unique names exist in the steps and inspect lists"""
+
+        self.layout.steps = [Step(name="name"), Step(name="name")]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        self.layout.steps = [Step(name="name")]
+        self.layout.inspect = [Inspection(name="name")]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.layout.validate()
+
+        self.layout.step = [Step(name="name"), Step(name="othername")]
+        self.layout.inspect = [Inspection(name="thirdname")]
+        self.layout.validate()
+
+    def test_import_step_metadata_wrong_type(self):
+        functionary_key = securesystemslib.keys.generate_rsa_key()
+        name = "name"
+
+        # Create and dump a link file with a wrong type
+        link_name = in_toto.models.link.FILENAME_FORMAT.format(
+            step_name=name, keyid=functionary_key["keyid"]
+        )
+
+        link_path = os.path.abspath(link_name)
+        link = in_toto.models.link.Link(name=name)
+        metadata = Metablock(signed=link)
+        metadata.signed._type = "wrong-type"
+        metadata.dump(link_path)
+
+        # Add the single step to the test layout and try to read the failing link
+        self.layout.steps.append(
+            Step(name=name, pubkeys=[functionary_key["keyid"]])
+        )
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            in_toto.verifylib.load_links_for_layout(self.layout, ".")
+
+        # Clean up
+        os.remove(link_path)
+
+    def test_wrong_pubkeys(self):
+        """Check validate pubkeys fails with wrong keys."""
+        # Pubkeys must be lists ...
+        tmp_step = Step()
+        tmp_step.pubkeys = "abcd"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            tmp_step.validate()
+
+        # ... of keyids (hex schema)
+        tmp_step.pubkeys = ["abcdefg"]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            tmp_step.validate()
 
-    # ... of keyids (hex schema)
-    tmp_step.pubkeys = ["abcdefg"]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      tmp_step.validate()
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/models/test_link.py` & `in_toto-2.0.0/tests/models/test_link.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,106 +18,104 @@
 
 <Purpose>
   Test link class functions.
 
 """
 
 import unittest
-from in_toto.models.link import Link
-from securesystemslib.exceptions import FormatError
-
-class TestLinkValidator(unittest.TestCase):
-  """Test link format validators """
-
-  def test_validate_type(self):
-    """Test `_type` field. Must be "link" """
-    test_link = Link()
-
-    # Good type
-    test_link._type = "link"
-    test_link.validate()
-
-    # Bad type
-    test_link._type = "bad link"
-    with self.assertRaises(FormatError):
-      test_link.validate()
-
-
-  def test_validate_materials(self):
-    """Test `materials` field. Must be a `dict` of HASH_DICTs """
-    test_link = Link()
-
-    # Good materials
-    sha = "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
-    test_link.materials = {"foo": {"sha256": sha}}
-    test_link.validate()
-
-    # Bad materials 1
-    test_link.materials = "not a dict"
-    with self.assertRaises(FormatError):
-      test_link.validate()
-
-    # Bad materials 1
-    test_link.materials = {"not": "a material dict"}
-    with self.assertRaises(FormatError):
-      test_link.validate()
-
 
-  def test_validate_products(self):
-    """Test `products` field. Must be a `dict` of HASH_DICTs """
-    test_link = Link()
-
-    # Good products
-    sha = "cfdaaf1ab2e4661952a9dec5e8fa3c360c1b06b1a073e8493a7c46d2af8c504b"
-    test_link.products = {"bar": {"sha256": sha}}
-    test_link.validate()
-
-    # Bad products 1
-    test_link = Link()
-    test_link.products = "not a dict"
-    with self.assertRaises(FormatError):
-      test_link.validate()
-
-    # Bad products 2
-    test_link.products = {"not": "a product dict"}
-    with self.assertRaises(FormatError):
-      test_link.validate()
-
-
-  def test_validate_byproducts(self):
-    """Test `byproducts` field. Must be a `dict` """
-    test_link = Link()
-    # Good byproducts
-    test_link.byproducts = {}
-    test_link.validate()
-
-    # Bad byproducts
-    test_link.byproducts = "not a dict"
-    with self.assertRaises(FormatError):
-      test_link.validate()
-
-
-  def test_validate_command(self):
-    """Test `command` field. Must be either a `list` """
-    test_link = Link()
-
-    # Good command
-    test_link.command = ["echo", "'good command'"]
-    test_link.validate()
-
-    # Bad command
-    test_link.command = "echo 'bad command'"
-    with self.assertRaises(FormatError):
-      test_link.validate()
+from securesystemslib.exceptions import FormatError
 
+from in_toto.models.link import Link
 
-  def test_validate_environment(self):
-    """Test `environment` field. Must be a `dict` """
-    test_link = Link()
 
-    # good env per default
-    test_link.validate()
+class TestLinkValidator(unittest.TestCase):
+    """Test link format validators"""
 
-    # Bad env
-    test_link.environment = "not a dict"
-    with self.assertRaises(FormatError):
-      test_link.validate()
+    def test_validate_type(self):
+        """Test `_type` field. Must be "link" """
+        test_link = Link()
+
+        # Good type
+        test_link._type = "link"
+        test_link.validate()
+
+        # Bad type
+        test_link._type = "bad link"
+        with self.assertRaises(FormatError):
+            test_link.validate()
+
+    def test_validate_materials(self):
+        """Test `materials` field. Must be a `dict` of HASH_DICTs"""
+        test_link = Link()
+
+        # Good materials
+        sha = "d65165279105ca6773180500688df4bdc69a2c7b771752f0a46ef120b7fd8ec3"
+        test_link.materials = {"foo": {"sha256": sha}}
+        test_link.validate()
+
+        # Bad materials 1
+        test_link.materials = "not a dict"
+        with self.assertRaises(FormatError):
+            test_link.validate()
+
+        # Bad materials 1
+        test_link.materials = {"not": "a material dict"}
+        with self.assertRaises(FormatError):
+            test_link.validate()
+
+    def test_validate_products(self):
+        """Test `products` field. Must be a `dict` of HASH_DICTs"""
+        test_link = Link()
+
+        # Good products
+        sha = "cfdaaf1ab2e4661952a9dec5e8fa3c360c1b06b1a073e8493a7c46d2af8c504b"
+        test_link.products = {"bar": {"sha256": sha}}
+        test_link.validate()
+
+        # Bad products 1
+        test_link = Link()
+        test_link.products = "not a dict"
+        with self.assertRaises(FormatError):
+            test_link.validate()
+
+        # Bad products 2
+        test_link.products = {"not": "a product dict"}
+        with self.assertRaises(FormatError):
+            test_link.validate()
+
+    def test_validate_byproducts(self):
+        """Test `byproducts` field. Must be a `dict`"""
+        test_link = Link()
+        # Good byproducts
+        test_link.byproducts = {}
+        test_link.validate()
+
+        # Bad byproducts
+        test_link.byproducts = "not a dict"
+        with self.assertRaises(FormatError):
+            test_link.validate()
+
+    def test_validate_command(self):
+        """Test `command` field. Must be either a `list`"""
+        test_link = Link()
+
+        # Good command
+        test_link.command = ["echo", "'good command'"]
+        test_link.validate()
+
+        # Bad command
+        test_link.command = "echo 'bad command'"
+        with self.assertRaises(FormatError):
+            test_link.validate()
+
+    def test_validate_environment(self):
+        """Test `environment` field. Must be a `dict`"""
+        test_link = Link()
+
+        # good env per default
+        test_link.validate()
+
+        # Bad env
+        test_link.environment = "not a dict"
+        with self.assertRaises(FormatError):
+            test_link.validate()
```

### Comparing `in_toto-1.4.0/tests/models/test_metadata.py` & `in_toto-2.0.0/tests/models/test_metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,71 +20,74 @@
   Test in_toto.models.metadata.Metablock class methods.
 
 """
 
 import os
 import unittest
 
-from in_toto.models.metadata import Metablock
+from securesystemslib.exceptions import FormatError
+
 from in_toto.models.layout import Layout
 from in_toto.models.link import Link
-from securesystemslib.exceptions import FormatError
+from in_toto.models.metadata import Metablock
+
 
 class TestMetablockValidator(unittest.TestCase):
-  """Test in_toto.models.metadata.Metablock validators. """
+    """Test in_toto.models.metadata.Metablock validators."""
 
-  def test_validate_signed(self):
-    """Test validate Metablock's 'signed' property. """
-    # Valid Layout Metablock
-    metablock = Metablock(signed=Layout())
-    metablock._validate_signed()
-
-    # Valid Link Metablock
-    Metablock(signed=Link())
-    metablock._validate_signed()
-
-
-    # Fail instantiation with empty or invalid signed property
-    # Metablock is validated on instantiation
-    with self.assertRaises(FormatError):
-      Metablock()
-    with self.assertRaises(FormatError):
-      Metablock(signed="not-a-layout-or-link")
-
-
-    # Fail with invalid signed property
-    metablock = Metablock(signed=Layout())
-    metablock.signed._type = "bogus type"
-    with self.assertRaises(FormatError):
-      metablock._validate_signed()
-
-
-  def test_validate_signatures(self):
-    """Test validate Metablock's 'signatures' property. """
-    # An empty signature list is okay
-    metablock = Metablock(signed=Layout())
-    metablock._validate_signatures()
-
-    # Fail with signatures property not a list
-    metablock.signatures = "not-a-signatures-list"
-    with self.assertRaises(FormatError):
-      metablock._validate_signatures()
-
-    # Fail with invalid signature
-    metablock.signatures = []
-    metablock.signatures.append("not-a-signature")
-    with self.assertRaises(FormatError):
-      metablock._validate_signatures()
-
-    # Load signed demo link
-    demo_link_path = os.path.join(os.path.dirname(os.path.realpath(__file__)),
-        "..", "demo_files", "write-code.776a00e2.link")
-
-    metablock = Metablock.load(demo_link_path)
-
-    # Verify that there is a signature and that it is valid
-    self.assertTrue(len(metablock.signatures) > 0)
-    metablock._validate_signatures()
+    def test_validate_signed(self):
+        """Test validate Metablock's 'signed' property."""
+        # Valid Layout Metablock
+        metablock = Metablock(signed=Layout())
+        metablock._validate_signed()
+
+        # Valid Link Metablock
+        Metablock(signed=Link())
+        metablock._validate_signed()
+
+        # Fail instantiation with empty or invalid signed property
+        # Metablock is validated on instantiation
+        with self.assertRaises(FormatError):
+            Metablock()
+        with self.assertRaises(FormatError):
+            Metablock(signed="not-a-layout-or-link")
+
+        # Fail with invalid signed property
+        metablock = Metablock(signed=Layout())
+        metablock.signed._type = "bogus type"
+        with self.assertRaises(FormatError):
+            metablock._validate_signed()
+
+    def test_validate_signatures(self):
+        """Test validate Metablock's 'signatures' property."""
+        # An empty signature list is okay
+        metablock = Metablock(signed=Layout())
+        metablock._validate_signatures()
+
+        # Fail with signatures property not a list
+        metablock.signatures = "not-a-signatures-list"
+        with self.assertRaises(FormatError):
+            metablock._validate_signatures()
+
+        # Fail with invalid signature
+        metablock.signatures = []
+        metablock.signatures.append("not-a-signature")
+        with self.assertRaises(FormatError):
+            metablock._validate_signatures()
+
+        # Load signed demo link
+        demo_link_path = os.path.join(
+            os.path.dirname(os.path.realpath(__file__)),
+            "..",
+            "demo_files",
+            "write-code.776a00e2.link",
+        )
+
+        metablock = Metablock.load(demo_link_path)
+
+        # Verify that there is a signature and that it is valid
+        self.assertTrue(len(metablock.signatures) > 0)
+        metablock._validate_signatures()
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/models/test_signer.py` & `in_toto-2.0.0/tests/models/test_signer.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,146 +18,146 @@
 
 <Purpose>
   Test GPGKey, GPGSigner and GPGSignature class methods.
 """
 
 import unittest
 
-from securesystemslib.gpg.functions import export_pubkey
-from securesystemslib.gpg.constants import have_gpg
 from securesystemslib.exceptions import (
-  UnverifiedSignatureError, VerificationError)
-
-from in_toto.models._signer import (GPGKey, GPGSignature,
-  GPGSigner)
+    UnverifiedSignatureError,
+    VerificationError,
+)
+from securesystemslib.gpg.constants import have_gpg
+from securesystemslib.gpg.functions import export_pubkey
 
+from in_toto.models._signer import GPGKey, GPGSignature, GPGSigner
 from tests.common import GPGKeysMixin, TmpDirMixin
 
 
 @unittest.skipIf(not have_gpg(), "gpg not found")
 class TestLegacyGPGKeyAndSigner(unittest.TestCase, TmpDirMixin, GPGKeysMixin):
-  """Test RSA gpg signature creation and verification."""
+    """Test RSA gpg signature creation and verification."""
 
-  @classmethod
-  def setUpClass(cls):
-    cls.set_up_test_dir()
-    cls.set_up_gpg_keys()
+    @classmethod
+    def setUpClass(cls):
+        cls.set_up_test_dir()
+        cls.set_up_gpg_keys()
 
-    cls.test_data = b"test_data"
-    cls.wrong_data = b"something malicious"
+        cls.test_data = b"test_data"
+        cls.wrong_data = b"something malicious"
 
-    cls.default_keyid = cls.gpg_key_0C8A17
-    cls.signing_subkey_keyid = cls.gpg_key_D924E9
-    cls.expired_keyid = "e8ac80c924116dabb51d4b987cb07d6d2c199c7c"
+        cls.default_keyid = cls.gpg_key_0C8A17
+        cls.signing_subkey_keyid = cls.gpg_key_D924E9
+        cls.expired_keyid = "e8ac80c924116dabb51d4b987cb07d6d2c199c7c"
 
-    cls.default_key_dict = export_pubkey(cls.default_keyid, cls.gnupg_home)
+        cls.default_key_dict = export_pubkey(cls.default_keyid, cls.gnupg_home)
 
-  @classmethod
-  def tearDownClass(cls):
-    cls.tear_down_test_dir()
+    @classmethod
+    def tearDownClass(cls):
+        cls.tear_down_test_dir()
 
-  def test_gpg_sign_and_verify_object_with_default_key(self):
-    """Create and verify a signature using the default key on the keyring."""
+    def test_gpg_sign_and_verify_object_with_default_key(self):
+        """Create and verify a signature using the default key on the keyring."""
 
-    # Create a signature.
-    signer = GPGSigner(homedir=self.gnupg_home)
-    signature = signer.sign(self.test_data)
+        # Create a signature.
+        signer = GPGSigner(homedir=self.gnupg_home)
+        signature = signer.sign(self.test_data)
 
-    # Generate Key from gnupg keyring.
-    key = GPGKey.from_keyring(self.default_keyid, self.gnupg_home)
+        # Generate Key from gnupg keyring.
+        key = GPGKey.from_keyring(self.default_keyid, self.gnupg_home)
 
-    key.verify_signature(signature, self.test_data)
-    with self.assertRaises(UnverifiedSignatureError):
-      key.verify_signature(signature, self.wrong_data)
+        key.verify_signature(signature, self.test_data)
+        with self.assertRaises(UnverifiedSignatureError):
+            key.verify_signature(signature, self.wrong_data)
 
-    # Generate Key from dict.
-    key = GPGKey.from_legacy_dict(self.default_key_dict)
+        # Generate Key from dict.
+        key = GPGKey.from_legacy_dict(self.default_key_dict)
 
-    key.verify_signature(signature, self.test_data)
-    with self.assertRaises(UnverifiedSignatureError):
-      key.verify_signature(signature, self.wrong_data)
+        key.verify_signature(signature, self.test_data)
+        with self.assertRaises(UnverifiedSignatureError):
+            key.verify_signature(signature, self.wrong_data)
 
-  def test_gpg_sign_and_verify_object(self):
-    """Create and verify a signature using the specific key on the keyring."""
+    def test_gpg_sign_and_verify_object(self):
+        """Create and verify a signature using the specific key on the keyring."""
 
-    # Create a signature.
-    signer = GPGSigner(self.signing_subkey_keyid, self.gnupg_home)
-    signature = signer.sign(self.test_data)
+        # Create a signature.
+        signer = GPGSigner(self.signing_subkey_keyid, self.gnupg_home)
+        signature = signer.sign(self.test_data)
 
-    # Generate Key from gnupg keyring.
-    key = GPGKey.from_keyring(self.signing_subkey_keyid, self.gnupg_home)
+        # Generate Key from gnupg keyring.
+        key = GPGKey.from_keyring(self.signing_subkey_keyid, self.gnupg_home)
 
-    key.verify_signature(signature, self.test_data)
-    with self.assertRaises(UnverifiedSignatureError):
-      key.verify_signature(signature, self.wrong_data)
+        key.verify_signature(signature, self.test_data)
+        with self.assertRaises(UnverifiedSignatureError):
+            key.verify_signature(signature, self.wrong_data)
 
-    # Generate Key from dict.
-    key_dict = export_pubkey(self.signing_subkey_keyid, self.gnupg_home)
-    key = GPGKey.from_dict(key_dict["keyid"], key_dict)
+        # Generate Key from dict.
+        key_dict = export_pubkey(self.signing_subkey_keyid, self.gnupg_home)
+        key = GPGKey.from_dict(key_dict["keyid"], key_dict)
 
-    key.verify_signature(signature, self.test_data)
-    with self.assertRaises(UnverifiedSignatureError):
-      key.verify_signature(signature, self.wrong_data)
+        key.verify_signature(signature, self.test_data)
+        with self.assertRaises(UnverifiedSignatureError):
+            key.verify_signature(signature, self.wrong_data)
 
-  def test_verify_using_expired_keyid(self):
-    """Creates and verifies a signature using expired key on the keyring."""
+    def test_verify_using_expired_keyid(self):
+        """Creates and verifies a signature using expired key on the keyring."""
 
-    # Create a signature.
-    signer = GPGSigner(self.signing_subkey_keyid, self.gnupg_home)
-    signature = signer.sign(self.test_data)
+        # Create a signature.
+        signer = GPGSigner(self.signing_subkey_keyid, self.gnupg_home)
+        signature = signer.sign(self.test_data)
 
-    # Verify signature using expired key.
-    key = GPGKey.from_keyring(self.expired_keyid, self.gnupg_home)
-    with self.assertRaises(VerificationError):
-      key.verify_signature(signature, self.test_data)
+        # Verify signature using expired key.
+        key = GPGKey.from_keyring(self.expired_keyid, self.gnupg_home)
+        with self.assertRaises(VerificationError):
+            key.verify_signature(signature, self.test_data)
 
-  def test_gpg_signature_serialization(self):
-    """Tests from_dict and to_dict methods of GPGSignature."""
+    def test_gpg_signature_serialization(self):
+        """Tests from_dict and to_dict methods of GPGSignature."""
 
-    sig_dict = {
-      "keyid": "f4f90403af58eef6",
-      "signature": "c39f86e70e12e70e11d87eb7e3ab7d3b",
-      "other_headers": "d8f8a89b5d71f07b842a",
-    }
+        sig_dict = {
+            "keyid": "f4f90403af58eef6",
+            "signature": "c39f86e70e12e70e11d87eb7e3ab7d3b",
+            "other_headers": "d8f8a89b5d71f07b842a",
+        }
 
-    signature = GPGSignature.from_dict(sig_dict)
-    self.assertEqual(sig_dict, signature.to_dict())
+        signature = GPGSignature.from_dict(sig_dict)
+        self.assertEqual(sig_dict, signature.to_dict())
 
-  def test_gpg_key_serialization(self):
-    """Test to check serialization methods of GPGKey."""
+    def test_gpg_key_serialization(self):
+        """Test to check serialization methods of GPGKey."""
 
-    # Test loading and dumping of GPGKey.
-    key = GPGKey.from_legacy_dict(self.default_key_dict)
-    self.assertEqual(key.to_dict(), self.default_key_dict)
+        # Test loading and dumping of GPGKey.
+        key = GPGKey.from_legacy_dict(self.default_key_dict)
+        self.assertEqual(key.to_dict(), self.default_key_dict)
 
-    # Test loading and dumping of GPGKey from keyring.
-    key = GPGKey.from_keyring(self.default_keyid, self.gnupg_home)
-    self.assertEqual(key.to_dict(), self.default_key_dict)
+        # Test loading and dumping of GPGKey from keyring.
+        key = GPGKey.from_keyring(self.default_keyid, self.gnupg_home)
+        self.assertEqual(key.to_dict(), self.default_key_dict)
 
-  def test_gpg_key_equality(self):
-    """Test to check equality between two GPGKey."""
+    def test_gpg_key_equality(self):
+        """Test to check equality between two GPGKey."""
 
-    # Generate two GPGkey.
-    key1 = GPGKey.from_legacy_dict(self.default_key_dict)
-    key2 = GPGKey.from_legacy_dict(self.default_key_dict)
+        # Generate two GPGkey.
+        key1 = GPGKey.from_legacy_dict(self.default_key_dict)
+        key2 = GPGKey.from_legacy_dict(self.default_key_dict)
 
-    self.assertNotEqual(self.default_key_dict, key1)
-    self.assertEqual(key2, key1)
+        self.assertNotEqual(self.default_key_dict, key1)
+        self.assertEqual(key2, key1)
 
-    # Assert equality of key created from dict of first GPGKey.
-    key2 = GPGKey.from_legacy_dict(key1.to_dict())
-    self.assertEqual(key2, key1)
+        # Assert equality of key created from dict of first GPGKey.
+        key2 = GPGKey.from_legacy_dict(key1.to_dict())
+        self.assertEqual(key2, key1)
 
-    # Assert Inequalities.
-    key2.type = "invalid"
-    self.assertNotEqual(key2, key1)
-    key2.type = key1.type
+        # Assert Inequalities.
+        key2.type = "invalid"
+        self.assertNotEqual(key2, key1)
+        key2.type = key1.type
 
-    key2.subkeys = {}
-    self.assertNotEqual(key2, key1)
-    key2.subkeys = key1.subkeys
+        key2.subkeys = {}
+        self.assertNotEqual(key2, key1)
+        key2.subkeys = key1.subkeys
 
-    key2.keyval = {}
-    self.assertNotEqual(key2, key1)
-    key2.keyval = key1.keyval
+        key2.keyval = {}
+        self.assertNotEqual(key2, key1)
+        key2.keyval = key1.keyval
 
-    self.assertEqual(key2, key1)
+        self.assertEqual(key2, key1)
```

### Comparing `in_toto-1.4.0/tests/models/test_step.py` & `in_toto-2.0.0/tests/models/test_step.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,94 +18,91 @@
 
 <Purpose>
   Test step class functions.
 
 """
 
 import unittest
-from in_toto.models.layout import Step
-import securesystemslib.keys
-import securesystemslib.exceptions
-
-class TestStepValidator(unittest.TestCase):
-  """Test verifylib.verify_delete_rule(rule, artifact_queue) """
-
-
-  def setUp(self):
-    """Populate a base layout that we can use."""
-    self.step = Step(name="this-step")
 
+import securesystemslib.exceptions
+import securesystemslib.keys
 
-  def test_wrong_type(self):
-    """Test the type field within Validate()."""
+from in_toto.models.layout import Step
 
-    self.step._type = "wrong"
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.step._validate_type()
 
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.step.validate()
+class TestStepValidator(unittest.TestCase):
+    """Test verifylib.verify_delete_rule(rule, artifact_queue)"""
 
-    self.step._type = "step"
-    self.step._validate_type()
+    def setUp(self):
+        """Populate a base layout that we can use."""
+        self.step = Step(name="this-step")
 
+    def test_wrong_type(self):
+        """Test the type field within Validate()."""
 
-  def test_wrong_threshold(self):
-    """Test that the threshold value is correctly checked."""
+        self.step._type = "wrong"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.step._validate_type()
 
-    # no, python is not *this* smart
-    self.step.threshold = "Ten"
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.step._validate_threshold()
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.step.validate()
 
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.step.validate()
+        self.step._type = "step"
+        self.step._validate_type()
 
-    self.step.threshold = 10
-    self.step._validate_threshold()
-    self.step.validate()
+    def test_wrong_threshold(self):
+        """Test that the threshold value is correctly checked."""
 
+        # no, python is not *this* smart
+        self.step.threshold = "Ten"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.step._validate_threshold()
 
-  def test_wrong_pubkeys(self):
-    # FIXME: generating keys for each test are expensive processes, maybe we
-    # should have an asset/fixture folder/loader?
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.step.validate()
 
-    rsa_key_one = securesystemslib.keys.generate_rsa_key()
-    rsa_key_two = securesystemslib.keys.generate_rsa_key()
+        self.step.threshold = 10
+        self.step._validate_threshold()
+        self.step.validate()
 
-    self.step.pubkeys = ['bad-keyid']
+    def test_wrong_pubkeys(self):
+        # FIXME: generating keys for each test are expensive processes, maybe we
+        # should have an asset/fixture folder/loader?
 
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.step._validate_pubkeys()
+        rsa_key_one = securesystemslib.keys.generate_rsa_key()
+        rsa_key_two = securesystemslib.keys.generate_rsa_key()
 
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.step.validate()
+        self.step.pubkeys = ["bad-keyid"]
 
-    self.step.pubkeys = [rsa_key_one['keyid'], rsa_key_two['keyid']]
-    self.step._validate_pubkeys()
-    self.step.validate()
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.step._validate_pubkeys()
 
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.step.validate()
 
-  def test_wrong_expected_command(self):
-    """Test that the expected command validator catches malformed ones."""
+        self.step.pubkeys = [rsa_key_one["keyid"], rsa_key_two["keyid"]]
+        self.step._validate_pubkeys()
+        self.step.validate()
 
-    self.step.expected_command = -1
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.step._validate_expected_command()
+    def test_wrong_expected_command(self):
+        """Test that the expected command validator catches malformed ones."""
 
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      self.step.validate()
+        self.step.expected_command = -1
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.step._validate_expected_command()
 
-    self.step.expected_command = ["somecommand"]
-    self.step._validate_expected_command()
-    self.step.validate()
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            self.step.validate()
 
+        self.step.expected_command = ["somecommand"]
+        self.step._validate_expected_command()
+        self.step.validate()
 
-  def test_set_expected_command_from_string(self):
-    """Test shelx parse command string to list. """
-    step = Step()
-    step.set_expected_command_from_string("echo 'foo bar'")
-    self.assertListEqual(step.expected_command, ["echo", "foo bar"])
+    def test_set_expected_command_from_string(self):
+        """Test shelx parse command string to list."""
+        step = Step()
+        step.set_expected_command_from_string("echo 'foo bar'")
+        self.assertListEqual(step.expected_command, ["echo", "foo bar"])
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/models/test_supply_chain_item.py` & `in_toto-2.0.0/tests/models/test_supply_chain_item.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,80 +19,79 @@
 <Purpose>
   Test SupplyChainItem class methods.
   SupplyChainItem is a super class for Steps and Inspections.
 
 """
 import json
 import unittest
-from in_toto.models.layout import SupplyChainItem
-import securesystemslib.exceptions
-
-class TestSupplyChainItem(unittest.TestCase):
-  """Test models.SupplyChainItem. """
-
-
-  def test_wrong_expected_materials(self):
-    """Test that the material rule validators catch malformed ones."""
-    item = SupplyChainItem()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      item.expected_materials = [["NONFOO"]]
-      item._validate_expected_materials()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      item.validate()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      item.expected_materials = "PFF"
-      item._validate_expected_materials()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      item.validate()
 
-    # for more thorough tests, check the test_rulelib.py module
-    item.expected_materials = [["CREATE", "foo"]]
-    item._validate_expected_materials()
-    item.validate()
-
-
-  def test_wrong_expected_products(self):
-    """Test that the product rule validators catch malformed values."""
-    item = SupplyChainItem()
-
-    item.expected_products = [["NONFOO"]]
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      item._validate_expected_products()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      item.validate()
-
-    item.expected_products = "PFF"
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      item._validate_expected_products()
-
-    with self.assertRaises(securesystemslib.exceptions.FormatError):
-      item.validate()
-
-    # for more thorough tests, check the test_rulelib.py module
-    item.expected_products = [["CREATE", "foo"]]
-    item._validate_expected_products()
-    item.validate()
+import securesystemslib.exceptions
 
+from in_toto.models.layout import SupplyChainItem
 
-  def test_repr(self):
-    """Test repr returns a JSON parseable string. """
-    json.loads(repr(SupplyChainItem()))
 
+class TestSupplyChainItem(unittest.TestCase):
+    """Test models.SupplyChainItem."""
 
-  def test_add_rule_from_string(self):
-    """Test that add_rule_from string methods set property correctly. """
-    item = SupplyChainItem()
-    item.add_material_rule_from_string("CREATE foo")
-    self.assertListEqual(item.expected_materials[-1], ["CREATE", "foo"])
-    item.add_product_rule_from_string("ALLOW bar")
-    self.assertListEqual(item.expected_products[-1], ["ALLOW", "bar"])
+    def test_wrong_expected_materials(self):
+        """Test that the material rule validators catch malformed ones."""
+        item = SupplyChainItem()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            item.expected_materials = [["NONFOO"]]
+            item._validate_expected_materials()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            item.validate()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            item.expected_materials = "PFF"
+            item._validate_expected_materials()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            item.validate()
+
+        # for more thorough tests, check the test_rulelib.py module
+        item.expected_materials = [["CREATE", "foo"]]
+        item._validate_expected_materials()
+        item.validate()
+
+    def test_wrong_expected_products(self):
+        """Test that the product rule validators catch malformed values."""
+        item = SupplyChainItem()
+
+        item.expected_products = [["NONFOO"]]
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            item._validate_expected_products()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            item.validate()
+
+        item.expected_products = "PFF"
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            item._validate_expected_products()
+
+        with self.assertRaises(securesystemslib.exceptions.FormatError):
+            item.validate()
+
+        # for more thorough tests, check the test_rulelib.py module
+        item.expected_products = [["CREATE", "foo"]]
+        item._validate_expected_products()
+        item.validate()
+
+    def test_repr(self):
+        """Test repr returns a JSON parseable string."""
+        json.loads(repr(SupplyChainItem()))
+
+    def test_add_rule_from_string(self):
+        """Test that add_rule_from string methods set property correctly."""
+        item = SupplyChainItem()
+        item.add_material_rule_from_string("CREATE foo")
+        self.assertListEqual(item.expected_materials[-1], ["CREATE", "foo"])
+        item.add_product_rule_from_string("ALLOW bar")
+        self.assertListEqual(item.expected_products[-1], ["ALLOW", "bar"])
 
-    item.validate()
+        item.validate()
 
 
 if __name__ == "__main__":
-  unittest.main()
+    unittest.main()
```

### Comparing `in_toto-1.4.0/tests/scripts/expr` & `in_toto-2.0.0/tests/scripts/touch`

 * *Files 9% similar despite different names*

```diff
@@ -22,8 +22,10 @@
   <Author>
     Santiago Torres-Arias <santiago@nyu.edu>
 
   <Date>
     1527623020
 """
 import sys
-sys.exit(1)
+
+open(sys.argv[1], "a+").close()
+sys.exit(0)
```

### Comparing `in_toto-1.4.0/tests/scripts/tar` & `in_toto-2.0.0/tests/scripts/tar`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 
   <Author>
     Santiago Torres-Arias <santiago@nyu.edu>
 
   <Date>
     1527623020
 """
-import tarfile
 import sys
+import tarfile
 
 tarfile.open(sys.argv[2], "r:*").extractall()
 sys.exit(0)
```

### Comparing `in_toto-1.4.0/tests/scripts/touch` & `in_toto-2.0.0/tests/scripts/expr`

 * *Files 12% similar despite different names*

```diff
@@ -23,9 +23,8 @@
     Santiago Torres-Arias <santiago@nyu.edu>
 
   <Date>
     1527623020
 """
 import sys
 
-open(sys.argv[1], "a+").close()
-sys.exit(0)
+sys.exit(1)
```

### Comparing `in_toto-1.4.0/.gitignore` & `in_toto-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/LICENSE` & `in_toto-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `in_toto-1.4.0/README.md` & `in_toto-2.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -146,30 +146,21 @@
 
 ## Specification
 You can read more about how in-toto works by taking a look at the
 [specification](https://github.com/in-toto/docs/blob/master/in-toto-spec.md).
 
 
 ## Security Issues and Bugs
-See [SECURITY.md](https://github.com/in-toto/in-toto/blob/develop/SECURITY.md)
+See [SECURITY.md](SECURITY.md).
 
-## Instructions for Contributors
-Development of in-toto occurs on the "develop" branch of this repository.
-Contributions can be made by submitting GitHub *Pull Requests*. Take a look at
-our [development
-guidelines](https://github.com/secure-systems-lab/lab-guidelines/blob/master/dev-workflow.md)
-for detailed instructions. Submitted code should follow our [style
-guidelines](https://github.com/secure-systems-lab/code-style-guidelines) and
-must be unit tested.
-
-Contributors must also indicate acceptance of the [Developer Certificate of
-Origin (DCO)](https://developercertificate.org/) by appending a `Signed-off-by:
-Your Name <example@domain.com>` to each git commit message (see [`git commit
---signoff`](https://git-scm.com/docs/git-commit#Documentation/git-commit.txt---signoff)).
 
+## Governance and Contributing
+
+For information about in-toto's governance and contributing guidelines, see
+[GOVERNANCE.md](GOVERNANCE.md).
 
 ## Acknowledgments
 This project is managed by Prof. Santiago Torres-Arias at Purdue University.
 It is worked on by many folks in academia and industry, including members of
 the [Secure Systems Lab](https://ssl.engineering.nyu.edu/) at NYU and the
 [NJIT Cybersecurity Research Center](https://centers.njit.edu/cybersecurity).
```

### Comparing `in_toto-1.4.0/pyproject.toml` & `in_toto-2.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Security",
     "Topic :: Software Development",
 ]
 dependencies = [
     "attrs",
     "iso8601",
@@ -57,14 +58,15 @@
 [project.scripts]
 in-toto-keygen = "in_toto.in_toto_keygen:main"
 in-toto-mock = "in_toto.in_toto_mock:main"
 in-toto-record = "in_toto.in_toto_record:main"
 in-toto-run = "in_toto.in_toto_run:main"
 in-toto-sign = "in_toto.in_toto_sign:main"
 in-toto-verify = "in_toto.in_toto_verify:main"
+in-toto-match-products = "in_toto.in_toto_match_products:main"
 
 [project.urls]
 "Bug Reports" = "https://github.com/in-toto/in-toto/issues"
 Homepage = "https://in-toto.io"
 Source = "https://github.com/in-toto/in-toto"
 
 [tool.hatch.version]
@@ -74,7 +76,15 @@
 include = [
     "/in_toto",
     "/tests",
     "/.coveragerc",
     "/tox.ini",
     "/requirements*.txt",
 ]
+
+[tool.black]
+line-length=80
+
+[tool.isort]
+profile="black"
+line_length=80
+known_first_party = ["in_toto"]
```

### Comparing `in_toto-1.4.0/PKG-INFO` & `in_toto-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-toto
-Version: 1.4.0
+Version: 2.0.0
 Summary: A framework to define and secure the integrity of software supply chains
 Project-URL: Bug Reports, https://github.com/in-toto/in-toto/issues
 Project-URL: Homepage, https://in-toto.io
 Project-URL: Source, https://github.com/in-toto/in-toto
 Author-email: "New York University: Secure Systems Lab" <in-toto-dev@googlegroups.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -18,14 +18,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development
 Requires-Python: ~=3.7
 Requires-Dist: attrs
 Requires-Dist: iso8601
 Requires-Dist: pathspec
@@ -183,30 +184,21 @@
 
 ## Specification
 You can read more about how in-toto works by taking a look at the
 [specification](https://github.com/in-toto/docs/blob/master/in-toto-spec.md).
 
 
 ## Security Issues and Bugs
-See [SECURITY.md](https://github.com/in-toto/in-toto/blob/develop/SECURITY.md)
+See [SECURITY.md](SECURITY.md).
 
-## Instructions for Contributors
-Development of in-toto occurs on the "develop" branch of this repository.
-Contributions can be made by submitting GitHub *Pull Requests*. Take a look at
-our [development
-guidelines](https://github.com/secure-systems-lab/lab-guidelines/blob/master/dev-workflow.md)
-for detailed instructions. Submitted code should follow our [style
-guidelines](https://github.com/secure-systems-lab/code-style-guidelines) and
-must be unit tested.
-
-Contributors must also indicate acceptance of the [Developer Certificate of
-Origin (DCO)](https://developercertificate.org/) by appending a `Signed-off-by:
-Your Name <example@domain.com>` to each git commit message (see [`git commit
---signoff`](https://git-scm.com/docs/git-commit#Documentation/git-commit.txt---signoff)).
 
+## Governance and Contributing
+
+For information about in-toto's governance and contributing guidelines, see
+[GOVERNANCE.md](GOVERNANCE.md).
 
 ## Acknowledgments
 This project is managed by Prof. Santiago Torres-Arias at Purdue University.
 It is worked on by many folks in academia and industry, including members of
 the [Secure Systems Lab](https://ssl.engineering.nyu.edu/) at NYU and the
 [NJIT Cybersecurity Research Center](https://centers.njit.edu/cybersecurity).
```

