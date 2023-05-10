# Comparing `tmp/ezmsg-3.3.1.tar.gz` & `tmp/ezmsg-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezmsg-3.3.1.tar", last modified: Thu Apr 13 18:59:02 2023, max compression
+gzip compressed data, was "ezmsg-3.3.2.tar", last modified: Wed May 10 14:07:40 2023, max compression
```

## Comparing `ezmsg-3.3.1.tar` & `ezmsg-3.3.2.tar`

### file list

```diff
@@ -1,124 +1,124 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.974635 ezmsg-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-13 18:58:53.000000 ezmsg-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-13 18:59:02.974635 ezmsg-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-04-13 18:58:53.000000 ezmsg-3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.946634 ezmsg-3.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.954635 ezmsg-3.3.1/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-13 18:58:53.000000 ezmsg-3.3.1/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.958635 ezmsg-3.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_attach.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_count.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_intro.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_normalterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_stop.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-13 18:58:53.000000 ezmsg-3.3.1/examples/ezmsg_toy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.958635 ezmsg-3.3.1/extensions/ezmsg-sigproc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/butterworthfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/decimate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/ewmfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/spectral.py
--rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/synth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/window.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_butterworth.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_downsample.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_window.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-websocket/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-websocket/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/examples/ezmsg_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.962635 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-websocket/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.966635 ezmsg-3.3.1/extensions/ezmsg-zmq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.966635 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-13 18:58:53.000000 ezmsg-3.3.1/extensions/ezmsg-zmq/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.950635 ezmsg-3.3.1/ezmsg/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/core/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/addressable.py
--rw-r--r--   0 runner    (1001) docker     (123)    10343 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/backendprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/backpressure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/graphcontext.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/graphserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/messagecache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/messagemarshal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/netprotocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/pubclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/shmserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/subclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/core/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/debuglog.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/lfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/multiplier.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/testing/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/debuglog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagecodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagegate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagelogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagequeue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messagereplay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/util/messages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/messages/axisarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/util/terminate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.970635 ezmsg-3.3.1/ezmsg/version/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-13 18:58:53.000000 ezmsg-3.3.1/ezmsg/version/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.966635 ezmsg-3.3.1/ezmsg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-13 18:59:02.000000 ezmsg-3.3.1/ezmsg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-13 18:58:53.000000 ezmsg-3.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-13 18:59:02.974635 ezmsg-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 18:58:53.000000 ezmsg-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 18:59:02.974635 ezmsg-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_addressable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_attach.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_axisarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_shm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-13 18:58:53.000000 ezmsg-3.3.1/tests/test_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.898419 ezmsg-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-10 14:07:25.000000 ezmsg-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-10 14:07:40.898419 ezmsg-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-05-10 14:07:25.000000 ezmsg-3.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.870419 ezmsg-3.3.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.874419 ezmsg-3.3.2/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-10 14:07:25.000000 ezmsg-3.3.2/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.878419 ezmsg-3.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-10 14:07:25.000000 ezmsg-3.3.2/examples/ezmsg_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-10 14:07:25.000000 ezmsg-3.3.2/examples/ezmsg_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-10 14:07:25.000000 ezmsg-3.3.2/examples/ezmsg_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-10 14:07:25.000000 ezmsg-3.3.2/examples/ezmsg_intro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-10 14:07:25.000000 ezmsg-3.3.2/examples/ezmsg_normalterm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-10 14:07:25.000000 ezmsg-3.3.2/examples/ezmsg_stop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-05-10 14:07:25.000000 ezmsg-3.3.2/examples/ezmsg_toy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.874419 ezmsg-3.3.2/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.878419 ezmsg-3.3.2/extensions/ezmsg-sigproc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.870419 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.882419 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/butterworthfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/decimate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/ewmfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10100 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/spectral.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12929 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/synth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.882419 ezmsg-3.3.2/extensions/ezmsg-sigproc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/tests/test_butterworth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/tests/test_downsample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/tests/test_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-sigproc/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.882419 ezmsg-3.3.2/extensions/ezmsg-websocket/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.882419 ezmsg-3.3.2/extensions/ezmsg-websocket/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-websocket/examples/ezmsg_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.874419 ezmsg-3.3.2/extensions/ezmsg-websocket/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.882419 ezmsg-3.3.2/extensions/ezmsg-websocket/ezmsg/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-websocket/ezmsg/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-websocket/ezmsg/websocket/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-websocket/ezmsg/websocket/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-websocket/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.882419 ezmsg-3.3.2/extensions/ezmsg-zmq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.874419 ezmsg-3.3.2/extensions/ezmsg-zmq/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.886419 ezmsg-3.3.2/extensions/ezmsg-zmq/ezmsg/zmq/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-zmq/ezmsg/zmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-zmq/ezmsg/zmq/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-zmq/ezmsg/zmq/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-10 14:07:25.000000 ezmsg-3.3.2/extensions/ezmsg-zmq/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.874419 ezmsg-3.3.2/ezmsg/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.890419 ezmsg-3.3.2/ezmsg/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/addressable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/backendprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/backpressure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/graphcontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11078 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/graphserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/messagecache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/messagemarshal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4917 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/netprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/pubclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/shmserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/subclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/core/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.890419 ezmsg-3.3.2/ezmsg/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/testing/debuglog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/testing/lfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/testing/multiplier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/testing/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.894419 ezmsg-3.3.2/ezmsg/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/debuglog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/messagecodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/messagegate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/messagelogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/messagequeue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/messagereplay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.894419 ezmsg-3.3.2/ezmsg/util/messages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/messages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/messages/axisarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/util/terminate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.894419 ezmsg-3.3.2/ezmsg/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 14:07:25.000000 ezmsg-3.3.2/ezmsg/version/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.886419 ezmsg-3.3.2/ezmsg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-10 14:07:40.000000 ezmsg-3.3.2/ezmsg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-10 14:07:40.000000 ezmsg-3.3.2/ezmsg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 14:07:40.000000 ezmsg-3.3.2/ezmsg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 14:07:40.000000 ezmsg-3.3.2/ezmsg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-10 14:07:40.000000 ezmsg-3.3.2/ezmsg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-10 14:07:40.000000 ezmsg-3.3.2/ezmsg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 14:07:25.000000 ezmsg-3.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-10 14:07:40.898419 ezmsg-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 14:07:25.000000 ezmsg-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 14:07:40.898419 ezmsg-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_addressable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_axisarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2445 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_shm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 14:07:25.000000 ezmsg-3.3.2/tests/test_test.py
```

### Comparing `ezmsg-3.3.1/LICENSE` & `ezmsg-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/PKG-INFO` & `ezmsg-3.3.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg
-Version: 3.3.1
+Version: 3.3.2
 Summary: A simple DAG-based computation model
 Home-page: https://github.com/iscoe/ezmsg
 Author: Griffin Milsap
 Author-email: griffin.milsap@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-3.3.1/README.md` & `ezmsg-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/docs/source/conf.py` & `ezmsg-3.3.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/examples/ezmsg_configs.py` & `ezmsg-3.3.2/examples/ezmsg_configs.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/examples/ezmsg_count.py` & `ezmsg-3.3.2/examples/ezmsg_count.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/examples/ezmsg_intro.py` & `ezmsg-3.3.2/examples/ezmsg_intro.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/examples/ezmsg_normalterm.py` & `ezmsg-3.3.2/examples/ezmsg_normalterm.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/examples/ezmsg_stop.py` & `ezmsg-3.3.2/examples/ezmsg_stop.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/examples/ezmsg_toy.py` & `ezmsg-3.3.2/examples/ezmsg_toy.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/butterworthfilter.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/butterworthfilter.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/decimate.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/decimate.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/downsample.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/downsample.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/ewmfilter.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/ewmfilter.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/filter.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 
 class FilterState(ez.State):
     axis: Optional[str] = None
     zi: Optional[np.ndarray] = None
     filt_designed: bool = False
     filt: Optional[FilterCoefficients] = None
-    filt_set: asyncio.Event = asyncio.Event()
+    filt_set: asyncio.Event = field(default_factory=asyncio.Event)
     samp_shape: Optional[Tuple[int, ...]] = None
     fs: Optional[float] = None  # Hz
 
 
 class Filter(ez.Unit):
     SETTINGS: FilterSettingsBase
     STATE: FilterState
```

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/messages.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/messages.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/sampler.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/sampler.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/spectral.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/spectral.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/synth.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/synth.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/ezmsg/sigproc/window.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/ezmsg/sigproc/window.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_butterworth.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/tests/test_butterworth.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_downsample.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/test_window.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/tests/test_window.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-sigproc/tests/util.py` & `ezmsg-3.3.2/extensions/ezmsg-sigproc/tests/util.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-websocket/examples/ezmsg_websocket.py` & `ezmsg-3.3.2/extensions/ezmsg-websocket/examples/ezmsg_websocket.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-websocket/ezmsg/websocket/units.py` & `ezmsg-3.3.2/extensions/ezmsg-websocket/ezmsg/websocket/units.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/extensions/ezmsg-zmq/ezmsg/zmq/units.py` & `ezmsg-3.3.2/extensions/ezmsg-zmq/ezmsg/zmq/units.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,15 @@
         self.socket = self.context.socket(zmq.PUB)
         self.monitor = self.socket.get_monitor_socket()
         ez.logger.debug(f"{self}:binding to {self.SETTINGS.write_addr}")
         self.socket.bind(self.SETTINGS.write_addr)
         self.has_subscribers = False
 
     def shutdown(self) -> None:
+        self.monitor.close()
         self.socket.close()
 
     @ez.task
     async def _socket_monitor(self) -> None:
         while True:
             monitor_result = await self.monitor.poll(100, zmq.POLLIN)
             if monitor_result:
@@ -146,14 +147,15 @@
 
         self.poller = zmq.Poller()
         self.poller.register(self.socket, zmq.POLLIN)
 
         self.socket_open = False
 
     def shutdown(self) -> None:
+        self.monitor.close()
         self.socket.close()
 
     @ez.task
     async def socket_monitor(self) -> None:
         while True:
             monitor_result = await self.monitor.poll(100, zmq.POLLIN)
             if monitor_result:
```

### Comparing `ezmsg-3.3.1/ezmsg/core/__init__.py` & `ezmsg-3.3.2/ezmsg/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/addressable.py` & `ezmsg-3.3.2/ezmsg/core/addressable.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/backend.py` & `ezmsg-3.3.2/ezmsg/core/backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import logging
 import typing
+import enum
 
 from socket import socket
 from multiprocessing import Event, Barrier
 from multiprocessing.synchronize import Event as EventType
 from multiprocessing.synchronize import Barrier as BarrierType
 from multiprocessing.connection import wait, Connection
 
@@ -84,14 +85,18 @@
 
         if connections is not None:
             for from_topic, to_topic in connections:
                 if isinstance(from_topic, Stream):
                     from_topic = from_topic.address
                 if isinstance(to_topic, Stream):
                     to_topic = to_topic.address
+                if isinstance(to_topic, enum.Enum):
+                    to_topic = to_topic.name
+                if isinstance(from_topic, enum.Enum):
+                    from_topic = from_topic.name
                 graph_connections.append((from_topic, to_topic))
 
         def crawl_components(
             component: Component, callback: typing.Callable[[Component], None]
         ) -> None:
             search: typing.List[Component] = [component]
             while len(search):
@@ -102,24 +107,29 @@
         def gather_edges(comp: Component):
             if isinstance(comp, Collection):
                 for from_stream, to_stream in comp.network():
                     if isinstance(from_stream, Stream):
                         from_stream = from_stream.address
                     if isinstance(to_stream, Stream):
                         to_stream = to_stream.address
+                    if isinstance(to_stream, enum.Enum):
+                        to_stream = to_stream.name
+                    if isinstance(from_stream, enum.Enum):
+                        from_stream = from_stream.name
                     graph_connections.append((from_stream, to_stream))
 
         for component in components.values():
             if isinstance(component, Collection):
                 crawl_components(component, gather_edges)
 
         processes = collect_processes(components.values(), process_components)
 
         for component in components.values():
             if isinstance(component, Collection):
+
                 def configure_collections(comp: Component):
                     if isinstance(comp, Collection):
                         comp.configure()
 
                 crawl_components(component, configure_collections)
 
         if force_single_process:
@@ -140,33 +150,35 @@
 def run_system(
     system: Collection,
     num_buffers: int = 32,
     init_buf_size: int = DEFAULT_SHM_SIZE,
     backend_process: typing.Type[BackendProcess] = DefaultBackendProcess,
 ) -> None:
     """Deprecated; just use run any component (unit, collection)"""
-    run(SYSTEM = system, backend_process = backend_process)
+    run(SYSTEM=system, backend_process=backend_process)
 
 
 def run(
     components: typing.Optional[typing.Mapping[str, Component]] = None,
     root_name: typing.Optional[str] = None,
     connections: typing.Optional[NetworkDefinition] = None,
     process_components: typing.Optional[typing.Collection[Component]] = None,
     backend_process: typing.Type[BackendProcess] = DefaultBackendProcess,
     graph_address: typing.Optional[AddressType] = None,
     force_single_process: bool = False,
-    **components_kwargs: Component
+    **components_kwargs: Component,
 ) -> None:
     graph_service = GraphService(graph_address)
     shm_service = SHMService()
 
     if components is not None and isinstance(components, Component):
         components = {"SYSTEM": components}
-        logger.warning("Passing a single Component without naming the Component is now Deprecated.")
+        logger.warning(
+            "Passing a single Component without naming the Component is now Deprecated."
+        )
     components = either_dict_or_kwargs(components, components_kwargs, "run")
     if components is None:
         raise ValueError("Must supply at least one component to run")
 
     with new_threaded_event_loop() as loop:
 
         execution_context = ExecutionContext.setup(
@@ -178,18 +190,18 @@
             process_components,
             backend_process,
             force_single_process,
         )
 
         if execution_context is None:
             return
-        
+
         async def create_graph_context() -> GraphContext:
             return await GraphContext(graph_service, shm_service).__aenter__()
-        
+
         async def cleanup_graph(context: GraphContext) -> None:
             await context.__aexit__(None, None, None)
 
         graph_context = asyncio.run_coroutine_threadsafe(
             create_graph_context(), loop
         ).result()
 
@@ -197,15 +209,15 @@
             for edge in execution_context.connections:
                 await graph_context.connect(*edge)
 
         asyncio.run_coroutine_threadsafe(setup_graph(), loop).result()
 
         if len(execution_context.processes) > 1:
             logger.info(f"Running in {len(execution_context.processes)} processes.")
-            
+
         main_process = execution_context.processes[0]
         other_processes = execution_context.processes[1:]
 
         sentinels: typing.Set[typing.Union[Connection, socket, int]] = set()
 
         for proc in other_processes:
             proc.start()
@@ -243,48 +255,45 @@
             asyncio.run_coroutine_threadsafe(
                 cleanup_graph(graph_context), loop
             ).result()
 
 
 def collect_processes(
     collection: typing.Union[Collection, typing.Iterable[Component]],
-    process_components: typing.Optional[typing.Collection[Component]] = None
+    process_components: typing.Optional[typing.Collection[Component]] = None,
 ) -> typing.List[typing.List[Unit]]:
-    
+
     if isinstance(collection, Collection):
         process_units, units = _collect_processes(
-            collection._components.values(), 
-            collection.process_components()
+            collection._components.values(), collection.process_components()
         )
 
     else:
         process_units, units = _collect_processes(
-            collection, 
-            process_components if process_components is not None else tuple()
+            collection,
+            process_components if process_components is not None else tuple(),
         )
 
     if len(units):
-        process_units = [units] + process_units 
+        process_units = [units] + process_units
 
     return process_units
 
 
 def _collect_processes(
-    comps: typing.Iterable[Component],
-    process_components: typing.Collection[Component]
+    comps: typing.Iterable[Component], process_components: typing.Collection[Component]
 ) -> typing.Tuple[typing.List[typing.List[Unit]], typing.List[Unit]]:
     process_units: typing.List[typing.List[Unit]] = []
     units: typing.List[Unit] = []
-    
+
     for comp in comps:
 
         if isinstance(comp, Collection):
             r_process_units, r_units = _collect_processes(
-                comp.components.values(), 
-                comp.process_components()
+                comp.components.values(), comp.process_components()
             )
 
             process_units = process_units + r_process_units
             if comp in process_components:
                 if len(r_units) > 0:
                     process_units = process_units + [r_units]
             else:
```

### Comparing `ezmsg-3.3.1/ezmsg/core/backendprocess.py` & `ezmsg-3.3.2/ezmsg/core/backendprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .unit import Unit, TIMEIT_ATTR, PUBLISHES_ATTR, SUBSCRIBES_ATTR, ZERO_COPY_ATTR
 
 from .graphcontext import GraphContext
 from .graphserver import GraphService
 from .shmserver import SHMService
 from .pubclient import Publisher
 from .subclient import Subscriber
-from .netprotocol import Address
+from .messagecache import MessageCache
 
 from typing import (
     List,
     Dict,
     Callable,
     Any,
     Optional,
@@ -240,14 +240,18 @@
             logger.debug(f"Shutting down Units")
 
             async def shutdown_units() -> None:
                 for unit in self.units:
                     unit.shutdown()
 
             asyncio.run_coroutine_threadsafe(shutdown_units(), loop=loop).result()
+
+            for cache in MessageCache.values():
+                cache.clear()
+
             asyncio.run_coroutine_threadsafe(context.revert(), loop=loop).result()
 
             logger.debug(f"Remaining tasks in event loop = {asyncio.all_tasks(loop)}")
 
             if self.task_finished_ev is not None:
                 logger.debug("Setting task finished event")
                 self.task_finished_ev.set()
```

### Comparing `ezmsg-3.3.1/ezmsg/core/backpressure.py` & `ezmsg-3.3.2/ezmsg/core/backpressure.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/collection.py` & `ezmsg-3.3.2/ezmsg/core/collection.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/command.py` & `ezmsg-3.3.2/ezmsg/core/command.py`

 * *Files 14% similar despite different names*

```diff
@@ -123,25 +123,51 @@
             dag: DAG = await graph_service.dag()
         except (ConnectionRefusedError, ConnectionResetError):
             logger.info(
                 f"GraphServer not running @{graph_address}, or host is refusing connections"
             )
             return
 
+        graph_connections = dag.graph.copy()
+        # Let's eliminate proxy topics, i.e. connections with inputs and outputs.
+        source_nodes = []
+        for node, conns in graph_connections.items():
+            if len(conns) > 0:
+                source_nodes += [node]
+        proxy_topics = []
+        for conns in graph_connections.values():
+            for conn in conns:
+                if conn in source_nodes and conn not in proxy_topics:
+                    proxy_topics += [conn]
+        # Replace Proxy Topics with actual source and downstream
+        for proxy_topic in proxy_topics:
+            downstreams = graph_connections.pop(proxy_topic)
+            logger.info(f"{proxy_topic} downstream connetions: {downstreams}")
+            for node, conns in graph_connections.items():
+                for conn in conns:
+                    if conn == proxy_topic:
+                        new_conns = conns.copy()
+                        new_conns.remove(proxy_topic)
+                        new_conns.union(downstreams)
+                        logger.info(f"Updating connections for {node} from {conns} to {new_conns}")
+                        graph_connections[node] = new_conns
+
+        graph_connections = dag.graph.copy()
         # Let's come up with UUID node names
-        node_map = {name: f'"{str(uuid4())}"' for name in dag.nodes}
+        nodes = set(graph_connections.keys())
+        node_map = {name: f'"{str(uuid4())}"' for name in nodes}
 
         # Construct the graph
         def tree():
             return defaultdict(tree)
 
         graph: defaultdict = tree()
 
         connections = ""
-        for node, conns in dag.graph.items():
+        for node, conns in graph_connections.items():
             subgraph = graph
             path = node.split("/")
             route = path[:-1]
             stream = path[-1]
             for seg in route:
                 subgraph = subgraph[seg]
             subgraph[stream] = node
```

### Comparing `ezmsg-3.3.1/ezmsg/core/component.py` & `ezmsg-3.3.2/ezmsg/core/component.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/dag.py` & `ezmsg-3.3.2/ezmsg/core/dag.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/graphcontext.py` & `ezmsg-3.3.2/ezmsg/core/graphcontext.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/graphserver.py` & `ezmsg-3.3.2/ezmsg/core/graphserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -292,18 +292,10 @@
         await writer.drain()
         await asyncio.sleep(1.0)
         await reader.readexactly(1)
         dag_num_bytes = await read_int(reader)
         dag_bytes = await reader.readexactly(dag_num_bytes)
         dag: DAG = pickle.loads(dag_bytes)
 
-        graphviz_str = "digraph EZ {\n"
-        for node in dag.nodes:
-            graphviz_str += f"\t{node}\n"
-        for node, conns in dag.graph.items():
-            for conn in conns:
-                graphviz_str += f"\t{node}->{conn}\n"
-        graphviz_str += "}"
-
         await asyncio.wait_for(reader.read(1), timeout=timeout)  # Complete
         await close_stream_writer(writer)
         return dag
```

### Comparing `ezmsg-3.3.1/ezmsg/core/message.py` & `ezmsg-3.3.2/ezmsg/core/message.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/messagecache.py` & `ezmsg-3.3.2/ezmsg/core/messagecache.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,10 +65,14 @@
                         raise CacheMiss
                 except UninitializedMemory:
                     raise CacheMiss
 
                 with MessageMarshal.obj_from_mem(mem) as obj:
                     yield obj
 
+    def clear(self):
+        self.cache_id = [None] * self.num_buffers
+        self.cache = [None] * self.num_buffers
+
 
 # NOTE: This should be made thread-safe in the future
 MessageCache: Dict[UUID, Cache] = dict()
```

### Comparing `ezmsg-3.3.1/ezmsg/core/messagemarshal.py` & `ezmsg-3.3.2/ezmsg/core/messagemarshal.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/netprotocol.py` & `ezmsg-3.3.2/ezmsg/core/netprotocol.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/pubclient.py` & `ezmsg-3.3.2/ezmsg/core/pubclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
     _subscriber_tasks: Dict[UUID, "asyncio.Task[None]"]
     _address: Address
     _backpressure: Backpressure
     _num_buffers: int
     _running: asyncio.Event
     _msg_id: int
     _shm: SHMContext
-    _cache: Cache
     _force_tcp: bool
     _last_backpressure_event: float
 
     _shm_service: SHMService
 
     @staticmethod
     def client_type() -> bytes:
@@ -100,16 +99,15 @@
 
         pub._connection_task = asyncio.create_task(serve(), name=f"pub_{str(id)}")
 
         def on_done(_: asyncio.Future) -> None:
             logger.debug("Closing pub server task.")
 
         pub._connection_task.add_done_callback(on_done)
-        pub._cache = Cache(pub._num_buffers)
-        MessageCache[id] = pub._cache
+        MessageCache[id] = Cache(pub._num_buffers)
         await pub._initialized.wait()
         return pub
 
     def __init__(
         self,
         id: UUID,
         topic: str,
@@ -255,39 +253,39 @@
         if not self._backpressure.available(buf_idx):
             delta = time.time() - self._last_backpressure_event
             if BACKPRESSURE_WARNING and (delta > BACKPRESSURE_REFRACTORY):
                 logger.warning(f"{self.topic} under subscriber backpressure!")
             self._last_backpressure_event = time.time()
             await self._backpressure.wait(buf_idx)
 
-        self._cache.put(self._msg_id, obj)
+        MessageCache[self.id].put(self._msg_id, obj)
 
         for sub in list(self._subscribers.values()):
             if not self._force_tcp and sub.id.node == self.id.node:
                 if sub.pid == self.pid:
                     sub.writer.write(Command.TX_LOCAL.value + msg_id_bytes)
 
                 else:
                     try:
                         # Push cache to shm (if not already there)
-                        self._cache.push(self._msg_id, self._shm)
+                        MessageCache[self.id].push(self._msg_id, self._shm)
 
                     except UndersizedMemory as e:
                         new_shm = await self._shm_service.create(
                             self._num_buffers, e.req_size * 2
                         )
 
                         for i in range(self._num_buffers):
                             with self._shm.buffer(i, readonly=True) as from_buf:
                                 with new_shm.buffer(i) as to_buf:
                                     MessageMarshal.copy_obj(from_buf, to_buf)
 
                         self._shm.close()
                         self._shm = new_shm
-                        self._cache.push(self._msg_id, self._shm)
+                        MessageCache[self.id].push(self._msg_id, self._shm)
 
                     sub.writer.write(Command.TX_SHM.value)
                     sub.writer.write(msg_id_bytes)
                     sub.writer.write(encode_str(self._shm.name))
 
             else:
                 with MessageMarshal.serialize(self._msg_id, obj) as ser_obj:
```

### Comparing `ezmsg-3.3.1/ezmsg/core/server.py` & `ezmsg-3.3.2/ezmsg/core/server.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/settings.py` & `ezmsg-3.3.2/ezmsg/core/settings.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/shmserver.py` & `ezmsg-3.3.2/ezmsg/core/shmserver.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/state.py` & `ezmsg-3.3.2/ezmsg/core/state.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/stream.py` & `ezmsg-3.3.2/ezmsg/core/stream.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/subclient.py` & `ezmsg-3.3.2/ezmsg/core/subclient.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/unit.py` & `ezmsg-3.3.2/ezmsg/core/unit.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/core/util.py` & `ezmsg-3.3.2/ezmsg/core/util.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/testing/__init__.py` & `ezmsg-3.3.2/ezmsg/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/testing/lfo.py` & `ezmsg-3.3.2/ezmsg/testing/lfo.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/testing/multiplier.py` & `ezmsg-3.3.2/ezmsg/testing/multiplier.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/util/debuglog.py` & `ezmsg-3.3.2/ezmsg/util/debuglog.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/util/messagecodec.py` & `ezmsg-3.3.2/ezmsg/util/messagecodec.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/util/messagegate.py` & `ezmsg-3.3.2/ezmsg/util/messagegate.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/util/messagelogger.py` & `ezmsg-3.3.2/ezmsg/util/messagelogger.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/util/messagequeue.py` & `ezmsg-3.3.2/ezmsg/util/messagequeue.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/util/messagereplay.py` & `ezmsg-3.3.2/ezmsg/util/messagereplay.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/util/messages/axisarray.py` & `ezmsg-3.3.2/ezmsg/util/messages/axisarray.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/util/rate.py` & `ezmsg-3.3.2/ezmsg/util/rate.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg/util/terminate.py` & `ezmsg-3.3.2/ezmsg/util/terminate.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/ezmsg.egg-info/PKG-INFO` & `ezmsg-3.3.2/ezmsg.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezmsg
-Version: 3.3.1
+Version: 3.3.2
 Summary: A simple DAG-based computation model
 Home-page: https://github.com/iscoe/ezmsg
 Author: Griffin Milsap
 Author-email: griffin.milsap@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `ezmsg-3.3.1/ezmsg.egg-info/SOURCES.txt` & `ezmsg-3.3.2/ezmsg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/setup.cfg` & `ezmsg-3.3.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_addressable.py` & `ezmsg-3.3.2/tests/test_addressable.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_attach.py` & `ezmsg-3.3.2/tests/test_attach.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_axisarray.py` & `ezmsg-3.3.2/tests/test_axisarray.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_connections.py` & `ezmsg-3.3.2/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_dag.py` & `ezmsg-3.3.2/tests/test_dag.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_graph.py` & `ezmsg-3.3.2/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_perf.py` & `ezmsg-3.3.2/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_run.py` & `ezmsg-3.3.2/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_shm.py` & `ezmsg-3.3.2/tests/test_shm.py`

 * *Files identical despite different names*

### Comparing `ezmsg-3.3.1/tests/test_state.py` & `ezmsg-3.3.2/tests/test_state.py`

 * *Files identical despite different names*

