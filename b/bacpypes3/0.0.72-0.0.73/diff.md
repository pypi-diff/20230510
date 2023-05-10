# Comparing `tmp/bacpypes3-0.0.72.tar.gz` & `tmp/bacpypes3-0.0.73.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bacpypes3-0.0.72.tar", last modified: Thu May  4 19:35:47 2023, max compression
+gzip compressed data, was "bacpypes3-0.0.73.tar", last modified: Wed May 10 06:11:40 2023, max compression
```

## Comparing `bacpypes3-0.0.72.tar` & `bacpypes3-0.0.73.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.210466 bacpypes3-0.0.72/
--rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-05-04 19:35:47.210466 bacpypes3-0.0.72/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.72/README.md
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.198466 bacpypes3-0.0.72/bacpypes3/
--rw-rw-r--   0 joel      (1000) joel      (1000)     1370 2023-05-04 14:15:37.000000 bacpypes3-0.0.72/bacpypes3/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    23678 2023-04-21 19:39:28.000000 bacpypes3-0.0.72/bacpypes3/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    56648 2023-01-24 05:27:28.000000 bacpypes3-0.0.72/bacpypes3/apdu.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    32984 2023-04-03 19:01:08.000000 bacpypes3-0.0.72/bacpypes3/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    65777 2023-04-04 12:53:18.000000 bacpypes3-0.0.72/bacpypes3/appservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    21553 2023-03-22 18:04:43.000000 bacpypes3-0.0.72/bacpypes3/argparse.py
--rw-rw-r--   0 joel      (1000) joel      (1000)   106747 2023-04-03 19:42:26.000000 bacpypes3-0.0.72/bacpypes3/basetypes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16150 2023-04-03 15:32:38.000000 bacpypes3-0.0.72/bacpypes3/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.72/bacpypes3/comm.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.72/bacpypes3/console.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    64295 2023-04-07 19:15:02.000000 bacpypes3-0.0.72/bacpypes3/constructeddata.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10883 2023-01-24 13:27:43.000000 bacpypes3-0.0.72/bacpypes3/debugging.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.72/bacpypes3/errors.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.202466 bacpypes3-0.0.72/bacpypes3/ipv4/
--rw-rw-r--   0 joel      (1000) joel      (1000)     9099 2023-01-09 14:29:42.000000 bacpypes3-0.0.72/bacpypes3/ipv4/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.72/bacpypes3/ipv4/app.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.72/bacpypes3/ipv4/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.72/bacpypes3/ipv4/link.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.72/bacpypes3/ipv4/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.202466 bacpypes3-0.0.72/bacpypes3/ipv6/
--rw-rw-r--   0 joel      (1000) joel      (1000)     6298 2023-01-09 14:29:42.000000 bacpypes3-0.0.72/bacpypes3/ipv6/__init__.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.72/bacpypes3/ipv6/bvll.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.72/bacpypes3/ipv6/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.202466 bacpypes3-0.0.72/bacpypes3/json/
--rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.72/bacpypes3/json/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.72/bacpypes3/json/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/bacpypes3/json/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.202466 bacpypes3-0.0.72/bacpypes3/lib/
--rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.72/bacpypes3/lib/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10085 2021-08-04 12:18:07.000000 bacpypes3-0.0.72/bacpypes3/lib/batchread.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.202466 bacpypes3-0.0.72/bacpypes3/local/
--rw-rw-r--   0 joel      (1000) joel      (1000)      381 2023-02-06 04:19:11.000000 bacpypes3-0.0.72/bacpypes3/local/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5393 2023-01-03 14:48:04.000000 bacpypes3-0.0.72/bacpypes3/local/cmd.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18792 2022-11-24 07:17:25.000000 bacpypes3-0.0.72/bacpypes3/local/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.72/bacpypes3/local/device.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4822 2023-02-06 04:19:11.000000 bacpypes3-0.0.72/bacpypes3/local/networkport.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     9811 2022-11-21 19:38:08.000000 bacpypes3-0.0.72/bacpypes3/local/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.72/bacpypes3/local/oos.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    24830 2023-02-06 04:19:11.000000 bacpypes3-0.0.72/bacpypes3/local/schedule.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    76370 2023-04-14 14:22:25.000000 bacpypes3-0.0.72/bacpypes3/netservice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.72/bacpypes3/npdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    93859 2023-04-04 12:10:08.000000 bacpypes3-0.0.72/bacpypes3/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    64688 2023-02-15 17:04:37.000000 bacpypes3-0.0.72/bacpypes3/pdu.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    80966 2023-02-17 06:25:03.000000 bacpypes3-0.0.72/bacpypes3/primitivedata.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.202466 bacpypes3-0.0.72/bacpypes3/rdf/
--rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.72/bacpypes3/rdf/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.72/bacpypes3/rdf/__main__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10595 2023-05-04 14:15:16.000000 bacpypes3-0.0.72/bacpypes3/rdf/core.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    19634 2023-01-27 13:19:10.000000 bacpypes3-0.0.72/bacpypes3/rdf/util.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.202466 bacpypes3-0.0.72/bacpypes3/sc/
--rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/bacpypes3/sc/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/bacpypes3/sc/bvll.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.72/bacpypes3/sc/service.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.206466 bacpypes3-0.0.72/bacpypes3/service/
--rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.72/bacpypes3/service/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    22512 2023-04-03 19:06:43.000000 bacpypes3-0.0.72/bacpypes3/service/cov.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    22741 2023-04-04 12:42:09.000000 bacpypes3-0.0.72/bacpypes3/service/device.py
--rwxrwxr-x   0 joel      (1000) joel      (1000)    31277 2023-04-03 19:49:50.000000 bacpypes3-0.0.72/bacpypes3/service/object.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3884 2023-01-27 13:49:14.000000 bacpypes3-0.0.72/bacpypes3/settings.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.206466 bacpypes3-0.0.72/bacpypes3/vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)    10230 2023-01-24 05:27:28.000000 bacpypes3-0.0.72/bacpypes3/vlan/__init__.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.198466 bacpypes3-0.0.72/bacpypes3.egg-info/
--rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-05-04 19:35:47.000000 bacpypes3-0.0.72/bacpypes3.egg-info/PKG-INFO
--rw-rw-r--   0 joel      (1000) joel      (1000)     2924 2023-05-04 19:35:47.000000 bacpypes3-0.0.72/bacpypes3.egg-info/SOURCES.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-05-04 19:35:47.000000 bacpypes3-0.0.72/bacpypes3.egg-info/dependency_links.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.72/bacpypes3.egg-info/not-zip-safe
--rw-rw-r--   0 joel      (1000) joel      (1000)       16 2023-05-04 19:35:47.000000 bacpypes3-0.0.72/bacpypes3.egg-info/top_level.txt
--rw-rw-r--   0 joel      (1000) joel      (1000)      100 2022-08-22 00:12:37.000000 bacpypes3-0.0.72/pyproject.toml
--rw-rw-r--   0 joel      (1000) joel      (1000)       38 2023-05-04 19:35:47.210466 bacpypes3-0.0.72/setup.cfg
--rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.72/setup.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.206466 bacpypes3-0.0.72/tests/
--rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/clocked_test.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/conftest.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/state_machine.py
--rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_1.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test__template.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.206466 bacpypes3-0.0.72/tests/test_constructed_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_constructed_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_constructed_data/test_any.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_constructed_data/test_array.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_constructed_data/test_choice.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_constructed_data/test_list.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_constructed_data/test_read_property_multiple.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_constructed_data/test_sequence.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_constructed_data/test_sequence_of.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.206466 bacpypes3-0.0.72/tests/test_pdu/
--rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_pdu/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    16509 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_pdu/test_address.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_pdu/test_pci.py
--rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_pdu/test_pdu.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.210466 bacpypes3-0.0.72/tests/test_primitive_data/
--rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_bit_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_boolean.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_character_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2671 2023-02-17 06:25:03.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_date.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_double.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_enumerated.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_integer.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_null.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_object_identifier.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_octet_string.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_real.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_tag.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     2546 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_time.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.72/tests/test_primitive_data/test_unsigned.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.210466 bacpypes3-0.0.72/tests/test_utilities/
--rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_utilities/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_utilities/test_state_machine.py
-drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-04 19:35:47.210466 bacpypes3-0.0.72/tests/test_vlan/
--rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_vlan/__init__.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_vlan/test_ipv4_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_vlan/test_ipv4_router.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/test_vlan/test_network.py
--rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/trapped_classes.py
--rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.72/tests/utilities.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.109958 bacpypes3-0.0.73/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-05-10 06:11:40.109958 bacpypes3-0.0.73/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)      346 2023-03-09 18:20:30.000000 bacpypes3-0.0.73/README.md
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.093958 bacpypes3-0.0.73/bacpypes3/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1370 2023-05-10 06:05:09.000000 bacpypes3-0.0.73/bacpypes3/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    23678 2023-04-21 19:39:28.000000 bacpypes3-0.0.73/bacpypes3/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    56648 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/apdu.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    32984 2023-04-03 19:01:08.000000 bacpypes3-0.0.73/bacpypes3/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    65777 2023-04-04 12:53:18.000000 bacpypes3-0.0.73/bacpypes3/appservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    21553 2023-03-22 18:04:43.000000 bacpypes3-0.0.73/bacpypes3/argparse.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)   109678 2023-05-10 06:07:50.000000 bacpypes3-0.0.73/bacpypes3/basetypes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16150 2023-04-03 15:32:38.000000 bacpypes3-0.0.73/bacpypes3/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7934 2022-11-21 19:40:26.000000 bacpypes3-0.0.73/bacpypes3/comm.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     7128 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/console.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    64295 2023-04-07 19:15:02.000000 bacpypes3-0.0.73/bacpypes3/constructeddata.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10883 2023-01-24 13:27:43.000000 bacpypes3-0.0.73/bacpypes3/debugging.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9685 2023-02-08 13:29:16.000000 bacpypes3-0.0.73/bacpypes3/errors.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/ipv4/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9099 2023-01-09 14:29:42.000000 bacpypes3-0.0.73/bacpypes3/ipv4/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8238 2023-04-22 03:23:44.000000 bacpypes3-0.0.73/bacpypes3/ipv4/app.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    25882 2023-04-21 19:42:07.000000 bacpypes3-0.0.73/bacpypes3/ipv4/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4119 2023-02-12 01:55:32.000000 bacpypes3-0.0.73/bacpypes3/ipv4/link.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    61699 2023-04-21 19:25:10.000000 bacpypes3-0.0.73/bacpypes3/ipv4/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/ipv6/
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6298 2023-01-09 14:29:42.000000 bacpypes3-0.0.73/bacpypes3/ipv6/__init__.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    32041 2023-01-24 14:48:16.000000 bacpypes3-0.0.73/bacpypes3/ipv6/bvll.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    57488 2023-02-01 12:39:44.000000 bacpypes3-0.0.73/bacpypes3/ipv6/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/json/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      102 2023-01-24 13:54:53.000000 bacpypes3-0.0.73/bacpypes3/json/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      132 2022-09-06 15:15:46.000000 bacpypes3-0.0.73/bacpypes3/json/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16743 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/bacpypes3/json/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/lib/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       41 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/lib/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10085 2021-08-04 12:18:07.000000 bacpypes3-0.0.73/bacpypes3/lib/batchread.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.097958 bacpypes3-0.0.73/bacpypes3/local/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      381 2023-02-06 04:19:11.000000 bacpypes3-0.0.73/bacpypes3/local/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5393 2023-01-03 14:48:04.000000 bacpypes3-0.0.73/bacpypes3/local/cmd.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18792 2022-11-24 07:17:25.000000 bacpypes3-0.0.73/bacpypes3/local/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     5769 2023-01-24 13:31:42.000000 bacpypes3-0.0.73/bacpypes3/local/device.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4822 2023-02-06 04:19:11.000000 bacpypes3-0.0.73/bacpypes3/local/networkport.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     9811 2022-11-21 19:38:08.000000 bacpypes3-0.0.73/bacpypes3/local/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1046 2023-01-03 14:48:04.000000 bacpypes3-0.0.73/bacpypes3/local/oos.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    24830 2023-02-06 04:19:11.000000 bacpypes3-0.0.73/bacpypes3/local/schedule.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    76370 2023-04-14 14:22:25.000000 bacpypes3-0.0.73/bacpypes3/netservice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    28240 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/npdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    93858 2023-05-10 06:05:09.000000 bacpypes3-0.0.73/bacpypes3/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    64688 2023-02-15 17:04:37.000000 bacpypes3-0.0.73/bacpypes3/pdu.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    80966 2023-02-17 06:25:03.000000 bacpypes3-0.0.73/bacpypes3/primitivedata.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/bacpypes3/rdf/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      353 2023-01-24 13:54:37.000000 bacpypes3-0.0.73/bacpypes3/rdf/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2022-08-22 23:43:00.000000 bacpypes3-0.0.73/bacpypes3/rdf/__main__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10595 2023-05-04 14:15:16.000000 bacpypes3-0.0.73/bacpypes3/rdf/core.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    19634 2023-01-27 13:19:10.000000 bacpypes3-0.0.73/bacpypes3/rdf/util.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/bacpypes3/sc/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       65 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/bacpypes3/sc/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    33859 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/bacpypes3/sc/bvll.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18081 2023-02-27 03:52:18.000000 bacpypes3-0.0.73/bacpypes3/sc/service.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/bacpypes3/service/
+-rw-rw-r--   0 joel      (1000) joel      (1000)       78 2023-01-24 13:55:00.000000 bacpypes3-0.0.73/bacpypes3/service/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    22512 2023-04-03 19:06:43.000000 bacpypes3-0.0.73/bacpypes3/service/cov.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    22741 2023-04-04 12:42:09.000000 bacpypes3-0.0.73/bacpypes3/service/device.py
+-rwxrwxr-x   0 joel      (1000) joel      (1000)    31277 2023-04-03 19:49:50.000000 bacpypes3-0.0.73/bacpypes3/service/object.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3884 2023-01-27 13:49:14.000000 bacpypes3-0.0.73/bacpypes3/settings.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/bacpypes3/vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10230 2023-01-24 05:27:28.000000 bacpypes3-0.0.73/bacpypes3/vlan/__init__.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.093958 bacpypes3-0.0.73/bacpypes3.egg-info/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      666 2023-05-10 06:11:40.000000 bacpypes3-0.0.73/bacpypes3.egg-info/PKG-INFO
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2924 2023-05-10 06:11:40.000000 bacpypes3-0.0.73/bacpypes3.egg-info/SOURCES.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2023-05-10 06:11:40.000000 bacpypes3-0.0.73/bacpypes3.egg-info/dependency_links.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)        1 2021-06-28 12:41:48.000000 bacpypes3-0.0.73/bacpypes3.egg-info/not-zip-safe
+-rw-rw-r--   0 joel      (1000) joel      (1000)       16 2023-05-10 06:11:40.000000 bacpypes3-0.0.73/bacpypes3.egg-info/top_level.txt
+-rw-rw-r--   0 joel      (1000) joel      (1000)      100 2022-08-22 00:12:37.000000 bacpypes3-0.0.73/pyproject.toml
+-rw-rw-r--   0 joel      (1000) joel      (1000)       38 2023-05-10 06:11:40.109958 bacpypes3-0.0.73/setup.cfg
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1219 2023-05-04 14:51:12.000000 bacpypes3-0.0.73/setup.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.101958 bacpypes3-0.0.73/tests/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      351 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2298 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/clocked_test.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      372 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/conftest.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    49924 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/state_machine.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)      644 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_1.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3054 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test__template.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.105958 bacpypes3-0.0.73/tests/test_constructed_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      247 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2616 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_any.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2526 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_array.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2894 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_choice.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2071 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_list.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4013 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_read_property_multiple.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    10217 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_sequence.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8422 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_constructed_data/test_sequence_of.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.105958 bacpypes3-0.0.73/tests/test_pdu/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      126 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_pdu/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    16509 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_pdu/test_address.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_pdu/test_pci.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)       14 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_pdu/test_pdu.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.105958 bacpypes3-0.0.73/tests/test_primitive_data/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      456 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3309 2023-01-09 14:29:42.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_bit_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2629 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_boolean.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3204 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_character_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2671 2023-02-17 06:25:03.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_date.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2794 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_double.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3266 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_enumerated.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2632 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_integer.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2363 2022-10-03 15:42:31.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_null.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3739 2021-07-22 21:59:33.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_object_identifier.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2775 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_octet_string.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2785 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_real.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     4262 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_tag.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     2546 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_time.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     3588 2021-06-28 12:37:49.000000 bacpypes3-0.0.73/tests/test_primitive_data/test_unsigned.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.105958 bacpypes3-0.0.73/tests/test_utilities/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      130 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_utilities/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    18594 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_utilities/test_state_machine.py
+drwxrwxr-x   0 joel      (1000) joel      (1000)        0 2023-05-10 06:11:40.109958 bacpypes3-0.0.73/tests/test_vlan/
+-rw-rw-r--   0 joel      (1000) joel      (1000)      200 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_vlan/__init__.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8287 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_vlan/test_ipv4_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     6304 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_vlan/test_ipv4_router.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     8904 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/test_vlan/test_network.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)    12098 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/trapped_classes.py
+-rw-rw-r--   0 joel      (1000) joel      (1000)     1397 2023-01-26 13:59:48.000000 bacpypes3-0.0.73/tests/utilities.py
```

### Comparing `bacpypes3-0.0.72/PKG-INFO` & `bacpypes3-0.0.73/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.72
+Version: 0.0.73
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.72/bacpypes3/__init__.py` & `bacpypes3-0.0.73/bacpypes3/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 if _sys.platform not in _supported_platforms:
     _warnings.warn("unsupported platform", RuntimeWarning)
 
 #
 #   Project Metadata
 #
 
-__version__ = "0.0.72"
+__version__ = "0.0.73"
 __author__ = "Joel Bender"
 __email__ = "joel@carrickbender.com"
 
 #
 #   Settings and Debugging
 #
```

### Comparing `bacpypes3-0.0.72/bacpypes3/__main__.py` & `bacpypes3-0.0.73/bacpypes3/__main__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/apdu.py` & `bacpypes3-0.0.73/bacpypes3/apdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/app.py` & `bacpypes3-0.0.73/bacpypes3/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/appservice.py` & `bacpypes3-0.0.73/bacpypes3/appservice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/argparse.py` & `bacpypes3-0.0.73/bacpypes3/argparse.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/basetypes.py` & `bacpypes3-0.0.73/bacpypes3/basetypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -646,124 +646,186 @@
     abortWindowSizeOutOfRange = 127
     accessDenied = 85
     addressingError = 115
     badDestinationAddress = 86
     badDestinationDeviceId = 87
     badSignature = 88
     badSourceAddress = 89
-    badTimestamp = 90
+    badTimestamp = 90  # removed revision 22
     busy = 82
-    cannotUseKey = 91
-    cannotVerifyMessageId = 92
+    bvlcFunctionUnknown = 143
+    bvlcProprietaryFunctionUnknown = 144
+    cannotUseKey = 91  # removed revision 22
+    cannotVerifyMessageId = 92  # removed revision 22
     characterSetNotSupported = 41
     communicationDisabled = 83
     configurationInProgress = 2
-    correctKeyRevision = 93
+    correctKeyRevision = 93  # removed revision 22
     covSubscriptionFailed = 43
     datatypeNotSupported = 47
     deleteFdtEntryFailed = 120
+    destinationDeviceIdRequired = 94  # removed revision 22
     deviceBusy = 3
-    destinationDeviceIdRequired = 94
     distributeBroadcastFailed = 121
+    dnsError = 192
+    dnsNameResolutionFailed = 190
+    dnsResolverFailure = 191
+    dnsUnavailable = 189
+    duplicateEntry = 137
     duplicateMessage = 95
     duplicateName = 48
     duplicateObjectId = 49
     dynamicCreationNotSupported = 4
     encryptionNotConfigured = 96
     encryptionRequired = 97
     fileAccessDenied = 5
     fileFull = 128
+    headerEncodingError = 145
+    headerNotUnderstood = 146
+    httpError = 165
+    httpNotAServer = 164
+    httpNoUpgrade = 153
+    httpProxyAuthenticationFailed = 155
+    httpResourceNotLocal = 154
+    httpResponseMissingHeader = 159
+    httpResponseSyntaxError = 157
+    httpResponseTimeout = 156
+    httpResponseValueError = 158
+    httpTemporaryUnavailable = 163
+    httpUnexpectedResponseCode = 152
+    httpUpgradeError = 162
+    httpUpgradeRequired = 161
+    httpWebsocketHeaderError = 160
     inconsistentConfiguration = 129
     inconsistentObjectType = 130
     inconsistentParameters = 7
     inconsistentSelectionCriterion = 8
-    incorrectKey = 98
+    incorrectKey = 98  # removed revision 22
     internalError = 131
     invalidArrayIndex = 42
     invalidConfigurationData = 46
+    invalidDataEncoding = 142
     invalidDataType = 9
     invalidEventState = 73
     invalidFileAccessMethod = 10
     invalidFileStartPosition = 11
-    invalidKeyData = 99
+    invalidKeyData = 99  # removed revision 22
     invalidParameterDataType = 13
     invalidTag = 57
     invalidTimeStamp = 14
-    keyUpdateInProgress = 100
+    invalidValueInThisState = 138
+    ipAddressNotReachable = 198
+    ipError = 199
+    keyUpdateInProgress = 100  # removed revision 22
     listElementNotFound = 81
+    listItemNotNumbered = 140
+    listItemNotTimestamped = 141
     logBufferFull = 75
     loggedValuePurged = 76
     malformedMessage = 101
+    messageIncomplete = 147
     messageTooLong = 113
     missingRequiredParameter = 16
     networkDown = 58
     noAlarmConfigured = 74
+    nodeDuplicateVmac = 151
     noObjectsOfSpecifiedType = 17
     noPropertySpecified = 77
     noSpaceForObject = 18
     noSpaceToAddListElement = 19
     noSpaceToWriteProperty = 20
-    noVtSessionsAvailable = 21
+    notABacnetScHub = 148
     notConfigured = 132
     notConfiguredForTriggeredLogging = 78
     notCovProperty = 44
-    notKeyServer = 102
+    notKeyServer = 102  # removed revision 22
     notRouterToDnet = 110
+    noVtSessionsAvailable = 21
     objectDeletionNotPermitted = 23
     objectIdentifierAlreadyExists = 24
-    other = 0
     operationalProblem = 25
     optionalFunctionalityNotSupported = 45
+    other = 0
     outOfMemory = 133
     parameterOutOfRange = 80
     passwordFailure = 26
+    payloadExpected = 149
     propertyIsNotAList = 22
     propertyIsNotAnArray = 50
     readAccessDenied = 27
     readBdtFailed = 117
     readFdtFailed = 119
     registerForeignDeviceFailed = 118
     rejectBufferOverflow = 59
     rejectInconsistentParameters = 60
     rejectInvalidParameterDataType = 61
     rejectInvalidTag = 62
     rejectMissingRequiredParameter = 63
+    rejectOther = 69
     rejectParameterOutOfRange = 64
+    rejectProprietary = 68
     rejectTooManyArguments = 65
     rejectUndefinedEnumeration = 66
     rejectUnrecognizedService = 67
-    rejectProprietary = 68
-    rejectOther = 69
     routerBusy = 111
     securityError = 114
     securityNotConfigured = 103
     serviceRequestDenied = 29
     sourceSecurityRequired = 104
     success = 84
+    tcpClosedByLocal = 195
+    tcpClosedOther = 196
+    tcpConnectionRefused = 194
+    tcpConnectTimeout = 193
+    tcpError = 197
     timeout = 30
-    tooManyKeys = 105
+    tleError = 188
+    tlsClientAuthenticationFailed = 182
+    tlsClientCertificateError = 180
+    tlsClientCertificateExpired = 184
+    tlsClientCertificateRevoked = 186
+    tlsServerAuthenticationFailed = 183
+    tlsServerCertificateError = 181
+    tlsServerCertificateExpired = 185
+    tlsServerCertificateRevoked = 187
+    tooManyKeys = 105  # removed revision 22
+    unexpectedData = 150
     unknownAuthenticationType = 106
     unknownDevice = 70
     unknownFileSize = 122
-    unknownKey = 107
-    unknownKeyRevision = 108
+    unknownKey = 107  # removed revision 22
+    unknownKeyRevision = 108  # removed revision 22
     unknownNetworkMessage = 112
     unknownObject = 31
     unknownProperty = 32
-    unknownSubscription = 79
     unknownRoute = 71
-    unknownSourceMessage = 109
+    unknownSourceMessage = 109  # removed revision 22
+    unknownSubscription = 79
     unknownVtClass = 34
     unknownVtSession = 35
     unsupportedObjectType = 36
     valueNotInitialized = 72
     valueOutOfRange = 37
     valueTooLong = 134
     vtSessionAlreadyClosed = 38
     vtSessionTerminationFailure = 39
+    websocketClosedAbnormally = 173
+    websocketClosedByPeer = 169
+    websocketCloseError = 168
+    websocketDataAgainstPolicy = 175
+    websocketDataInconsistent = 174
+    websocketDataNotAccepted = 172
+    websocketEndpointLeaves = 170
+    websocketError = 179
+    websocketExtensionMissing = 177
+    websocketFrameTooLong = 176
+    websocketProtocolError = 171
+    websocketRequestUnavailable = 178
+    websocketSchemeNotSupported = 166
+    websocketUnknownControlMessage = 167
     writeAccessDenied = 40
     writeBdtFailed = 116
 
 
 class EscalatorFault(Enumerated):
     _vendor_range = (1024, 65535)
     controllerFault = 0
@@ -1168,15 +1230,15 @@
     adjustValue = 176
     alarmValue = 6
     alarmValues = 7
     alignIntervals = 193
     all = 8
     allowGroupDelayInhibit = 365
     allWritesSuccessful = 9
-    apduLength = 388
+    apduLength = 399
     apduSegmentTimeout = 10
     apduTimeout = 11
     applicationSoftwareVersion = 12
     archive = 13
     assignedAccessRights = 256
     assignedLandingCalls = 447
     attemptedSamples = 124
@@ -1351,15 +1413,15 @@
     ipDHCPEnable = 402
     ipDHCPLeaseTime = 403
     ipDHCPLeaseTimeRemaining = 404
     ipDHCPServer = 405
     ipDNSServer = 406
     ipSubnetMask = 411
     ipv6Address = 436
-    ipv6AutoAddressingEnabled = 442
+    ipv6AutoAddressingEnable = 442
     ipv6DefaultGateway = 439
     ipv6DHCPLeaseTime = 443
     ipv6DHCPLeaseTimeRemaining = 444
     ipv6DHCPServer = 445
     ipv6DNSServer = 441
     ipv6PrefixLength = 437
     ipv6ZoneIndex = 446
@@ -1492,15 +1554,15 @@
     presentStage = 493
     presentValue = 85
     priority = 86
     priorityArray = 87
     priorityForWriting = 88
     processIdentifier = 89
     processIdentifierFilter = 361
-    profileLocation = 91
+    profileLocation = 485
     profileName = 168
     programChange = 90
     programLocation = 91
     programState = 92
     propertyList = 371
     proportionalConstant = 93
     proportionalConstantUnits = 94
@@ -1695,26 +1757,28 @@
     renewDHCPFailure = 18
     renewFDRegistrationFailure = 19
     restartAutoNegotiationFailure = 20
     restartFailure = 21
     proprietaryCommandFailure = 22
     faultsListed = 23
     referencedObjectFault = 24
+    multiStateOutOfRange = 25
 
 
 class RestartReason(Enumerated):
     _vendor_range = (64, 255)
     unknown = 0
     coldstart = 1
     warmstart = 2
     detectedPowerLost = 3
     detectedPoweredOff = 4
     hardwareWatchdog = 5
     softwareWatchdog = 6
     suspended = 7
+    activateChanges = 8
 
 
 class RouterEntryStatus(Enumerated):
     available = 0
     busy = 1
     disconnected = 2
 
@@ -1884,15 +1948,15 @@
     accessCredential = 32
     accessPoint = 33
     accessRights = 34
     accessUser = 35
     accessZone = 36
     credentialDataInput = 37
     networkPort = 56
-    networkSecurity = 38
+    networkSecurity = 38  # removed revision 22
     bitstringValue = 39
     characterstringValue = 40
     datePatternValue = 41
     dateValue = 42
     datetimePatternValue = 43
     datetimeValue = 44
     integerValue = 45
@@ -1901,14 +1965,22 @@
     positiveIntegerValue = 48
     timePatternValue = 49
     timeValue = 50
     notificationForwarder = 51
     alertEnrollment = 52
     channel = 53
     lightingOutput = 54
+    binaryLightingOutput = 55
+    networkPort = 56
+    elevatorGroup = 57
+    escalator = 58
+    lift = 59
+    staging = 60
+    auditLog = 61
+    auditReporter = 62
 
 
 class PriorityFilter(BitString):
     manualLifeSafety = 0
     automaticLifeSafety = 1
     priority3 = 2
     priority4 = 3
@@ -1970,14 +2042,22 @@
     whoIs = 34
     readRange = 35
     utcTimeSynchronization = 36
     lifeSafetyOperation = 37
     subscribeCOVProperty = 38
     getEventInformation = 39
     writeGroup = 40
+    subscribeCOVPropertyMultiple = 41
+    confirmedCOVNotificationMultiple = 42
+    unconfirmedCOVNotificationMultiple = 43
+    confirmedAuditNotification = 44
+    auditLogQuery = 45
+    unconfirmedAuditNotification = 46
+    whoAmI = 47
+    youAre = 48
 
 
 class StatusFlags(BitString):
     inAlarm = 0
     fault = 1
     overridden = 2
     outOfService = 3
@@ -2207,17 +2287,17 @@
     _order = ("errorClass", "errorCode")
     errorClass = ErrorClass()
     errorCode = ErrorCode()
 
 
 @bacpypes_debugging
 class HostAddress(Choice):
-    none = Null()
-    ipAddress = OctetString()
-    name = CharacterString()
+    none = Null(_context=0)
+    ipAddress = OctetString(_context=1)
+    name = CharacterString(_context=2)
 
     def __init__(
         self,
         arg: Optional[str] = None,
         **kwargs,
     ) -> None:
         if _debug:
@@ -3294,17 +3374,17 @@
     timeDelay = Unsigned(_context=0)
     lowLimit = Unsigned(_context=1)
     highLimit = Unsigned(_context=2)
 
 
 class FDTEntry(Sequence):
     _order = ("bacnetIPAddress", "timeToLive", "remainingTimeToLive")
-    bacnetIPAddress = IPOctetString()
-    timeToLive = Unsigned16()
-    remainingTimeToLive = Unsigned16()
+    bacnetIPAddress = IPOctetString(_context=0)
+    timeToLive = Unsigned16(_context=1)
+    remainingTimeToLive = Unsigned16(_context=2)
 
 
 class ListOfFDTEntry(ListOf(FDTEntry)):
     pass
 
 
 class FaultParameterCharacterString(Sequence):
@@ -3725,18 +3805,19 @@
 class ReadAccessSpecification(Sequence):
     _order = ("objectIdentifier", "listOfPropertyReferences")
     objectIdentifier = ObjectIdentifier(_context=0)
     listOfPropertyReferences = SequenceOf(PropertyReference, _context=1)
 
 
 class RouterEntry(Sequence):
-    _order = ("networkNumber", "macAddress", "status")
-    networkNumber = Unsigned16()
-    macAddress = OctetString()
-    status = RouterEntryStatus()
+    _order = ("networkNumber", "macAddress", "status", "performanceIndex")
+    networkNumber = Unsigned16(_context=0)
+    macAddress = OctetString(_context=1)
+    status = RouterEntryStatus(_context=2)
+    performanceIndex = Unsigned8(_context=3, _optional=True)
 
 
 class SecurityKeySet(Sequence):
     _order = ("keyRevision", "activationTime", "expirationTime", "keyIds")
     keyRevision = Unsigned(_context=0)
     activationTime = DateTime(_context=1)
     expirationTime = DateTime(_context=2)
@@ -3785,16 +3866,16 @@
     limit = Real()
     values = BitString()
     deadband = Real()
 
 
 class VMACEntry(Sequence):
     _order = ("virtualMACAddress", "nativeMACAddress")
-    virtualMACAddress = OctetString()
-    nativeMACAddress = OctetString()
+    virtualMACAddress = OctetString(_context=0)
+    nativeMACAddress = OctetString(_context=1)
 
 
 class VTSession(Sequence):
     _order = ("localVtSessionID", "remoteVtSessionID", "remoteVtAddress")
     localVtSessionID = Unsigned()
     remoteVtSessionID = Unsigned()
     remoteVtAddress = DeviceAddress()
```

### Comparing `bacpypes3-0.0.72/bacpypes3/cmd.py` & `bacpypes3-0.0.73/bacpypes3/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/comm.py` & `bacpypes3-0.0.73/bacpypes3/comm.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/console.py` & `bacpypes3-0.0.73/bacpypes3/console.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/constructeddata.py` & `bacpypes3-0.0.73/bacpypes3/constructeddata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/debugging.py` & `bacpypes3-0.0.73/bacpypes3/debugging.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/errors.py` & `bacpypes3-0.0.73/bacpypes3/errors.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/ipv4/__init__.py` & `bacpypes3-0.0.73/bacpypes3/ipv4/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/ipv4/app.py` & `bacpypes3-0.0.73/bacpypes3/ipv4/app.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/ipv4/bvll.py` & `bacpypes3-0.0.73/bacpypes3/ipv4/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/ipv4/link.py` & `bacpypes3-0.0.73/bacpypes3/ipv4/link.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/ipv4/service.py` & `bacpypes3-0.0.73/bacpypes3/ipv4/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/ipv6/__init__.py` & `bacpypes3-0.0.73/bacpypes3/ipv6/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/ipv6/bvll.py` & `bacpypes3-0.0.73/bacpypes3/ipv6/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/ipv6/service.py` & `bacpypes3-0.0.73/bacpypes3/ipv6/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/json/util.py` & `bacpypes3-0.0.73/bacpypes3/json/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/lib/batchread.py` & `bacpypes3-0.0.73/bacpypes3/lib/batchread.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/local/cmd.py` & `bacpypes3-0.0.73/bacpypes3/local/cmd.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/local/cov.py` & `bacpypes3-0.0.73/bacpypes3/local/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/local/device.py` & `bacpypes3-0.0.73/bacpypes3/local/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/local/networkport.py` & `bacpypes3-0.0.73/bacpypes3/local/networkport.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/local/object.py` & `bacpypes3-0.0.73/bacpypes3/local/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/local/oos.py` & `bacpypes3-0.0.73/bacpypes3/local/oos.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/local/schedule.py` & `bacpypes3-0.0.73/bacpypes3/local/schedule.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/netservice.py` & `bacpypes3-0.0.73/bacpypes3/netservice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/npdu.py` & `bacpypes3-0.0.73/bacpypes3/npdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/object.py` & `bacpypes3-0.0.73/bacpypes3/object.py`

 * *Files 0% similar despite different names*

```diff
@@ -2441,15 +2441,15 @@
     bacnetIPv6Mode: IPMode
     ipv6Address: IPv6OctetString
     ipv6PrefixLength: Unsigned8
     bacnetIPv6UDPPort: Unsigned16
     ipv6DefaultGateway: IPv6OctetString
     bacnetIPv6MulticastAddress: IPv6OctetString
     ipv6DNSServer: ArrayOf(IPv6OctetString)
-    ipv6AutoAddressingEnabled: Boolean
+    ipv6AutoAddressingEnable: Boolean
     ipv6DHCPLeaseTime: Unsigned
     ipv6DHCPLeaseTimeRemaining: Unsigned
     ipv6DHCPServer: IPv6OctetString
     ipv6ZoneIndex: CharacterString
     maxMaster: Unsigned8
     maxInfoFrames: Unsigned8
     slaveProxyEnable: Boolean
```

### Comparing `bacpypes3-0.0.72/bacpypes3/pdu.py` & `bacpypes3-0.0.73/bacpypes3/pdu.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/primitivedata.py` & `bacpypes3-0.0.73/bacpypes3/primitivedata.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/rdf/core.py` & `bacpypes3-0.0.73/bacpypes3/rdf/core.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/rdf/util.py` & `bacpypes3-0.0.73/bacpypes3/rdf/util.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/sc/bvll.py` & `bacpypes3-0.0.73/bacpypes3/sc/bvll.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/sc/service.py` & `bacpypes3-0.0.73/bacpypes3/sc/service.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/service/cov.py` & `bacpypes3-0.0.73/bacpypes3/service/cov.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/service/device.py` & `bacpypes3-0.0.73/bacpypes3/service/device.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/service/object.py` & `bacpypes3-0.0.73/bacpypes3/service/object.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/settings.py` & `bacpypes3-0.0.73/bacpypes3/settings.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3/vlan/__init__.py` & `bacpypes3-0.0.73/bacpypes3/vlan/__init__.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/bacpypes3.egg-info/PKG-INFO` & `bacpypes3-0.0.73/bacpypes3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bacpypes3
-Version: 0.0.72
+Version: 0.0.73
 Summary: BACnet Communications Library
 Home-page: https://github.com/JoelBender/bacpypes3
 Author: Joel Bender
 Author-email: joel@carrickbender.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bacpypes3-0.0.72/bacpypes3.egg-info/SOURCES.txt` & `bacpypes3-0.0.73/bacpypes3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/setup.py` & `bacpypes3-0.0.73/setup.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/clocked_test.py` & `bacpypes3-0.0.73/tests/clocked_test.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/state_machine.py` & `bacpypes3-0.0.73/tests/state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_1.py` & `bacpypes3-0.0.73/tests/test_1.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test__template.py` & `bacpypes3-0.0.73/tests/test__template.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_constructed_data/test_any.py` & `bacpypes3-0.0.73/tests/test_constructed_data/test_any.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_constructed_data/test_array.py` & `bacpypes3-0.0.73/tests/test_constructed_data/test_array.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_constructed_data/test_choice.py` & `bacpypes3-0.0.73/tests/test_constructed_data/test_choice.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_constructed_data/test_list.py` & `bacpypes3-0.0.73/tests/test_constructed_data/test_list.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_constructed_data/test_read_property_multiple.py` & `bacpypes3-0.0.73/tests/test_constructed_data/test_read_property_multiple.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_constructed_data/test_sequence.py` & `bacpypes3-0.0.73/tests/test_constructed_data/test_sequence.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_constructed_data/test_sequence_of.py` & `bacpypes3-0.0.73/tests/test_constructed_data/test_sequence_of.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_pdu/test_address.py` & `bacpypes3-0.0.73/tests/test_pdu/test_address.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_bit_string.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_bit_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_boolean.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_boolean.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_character_string.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_character_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_date.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_date.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_double.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_double.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_enumerated.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_enumerated.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_integer.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_integer.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_null.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_null.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_object_identifier.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_object_identifier.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_octet_string.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_octet_string.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_real.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_real.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_tag.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_tag.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_time.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_time.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_primitive_data/test_unsigned.py` & `bacpypes3-0.0.73/tests/test_primitive_data/test_unsigned.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_utilities/test_state_machine.py` & `bacpypes3-0.0.73/tests/test_utilities/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_vlan/test_ipv4_network.py` & `bacpypes3-0.0.73/tests/test_vlan/test_ipv4_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_vlan/test_ipv4_router.py` & `bacpypes3-0.0.73/tests/test_vlan/test_ipv4_router.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/test_vlan/test_network.py` & `bacpypes3-0.0.73/tests/test_vlan/test_network.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/trapped_classes.py` & `bacpypes3-0.0.73/tests/trapped_classes.py`

 * *Files identical despite different names*

### Comparing `bacpypes3-0.0.72/tests/utilities.py` & `bacpypes3-0.0.73/tests/utilities.py`

 * *Files identical despite different names*

