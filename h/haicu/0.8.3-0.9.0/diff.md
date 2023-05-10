# Comparing `tmp/haicu-0.8.3.tar.gz` & `tmp/haicu-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haicu-0.8.3.tar", last modified: Tue Apr 11 20:11:16 2023, max compression
+gzip compressed data, was "haicu-0.9.0.tar", last modified: Wed May 10 17:20:29 2023, max compression
```

## Comparing `haicu-0.8.3.tar` & `haicu-0.9.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:11:16.250266 haicu-0.8.3/
--rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.8.3/LICENSE
--rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:11:16.250266 haicu-0.8.3/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)     2042 2023-04-11 19:58:00.000000 haicu-0.8.3/README.md
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:11:16.250266 haicu-0.8.3/haicu/
--rw-rw-r--   0 bry       (1000) bry       (1000)        0 2023-03-10 00:08:52.000000 haicu-0.8.3/haicu/__init__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    28509 2023-04-11 20:10:54.000000 haicu-0.8.3/haicu/__main__.py
--rwxrwxr-x   0 bry       (1000) bry       (1000)    12563 2023-04-11 18:21:24.000000 haicu-0.8.3/haicu/format.py
--rw-rw-r--   0 bry       (1000) bry       (1000)    11443 2023-04-11 18:13:59.000000 haicu-0.8.3/haicu/ftdi.py
-drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-04-11 20:11:16.250266 haicu-0.8.3/haicu.egg-info/
--rw-rw-r--   0 bry       (1000) bry       (1000)     3555 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/PKG-INFO
--rw-rw-r--   0 bry       (1000) bry       (1000)      274 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/SOURCES.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/dependency_links.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       50 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/entry_points.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/requires.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-04-11 20:11:16.000000 haicu-0.8.3/haicu.egg-info/top_level.txt
--rw-rw-r--   0 bry       (1000) bry       (1000)      742 2023-04-11 20:11:10.000000 haicu-0.8.3/pyproject.toml
--rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-04-11 20:11:16.250266 haicu-0.8.3/setup.cfg
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 17:20:29.235020 haicu-0.9.0/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     1074 2023-04-11 16:31:08.000000 haicu-0.9.0/LICENSE
+-rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-05-10 17:20:29.235020 haicu-0.9.0/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)     2619 2023-05-09 22:37:20.000000 haicu-0.9.0/README.md
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 17:20:29.235020 haicu-0.9.0/haicu/
+-rw-rw-r--   0 bry       (1000) bry       (1000)       21 2023-05-10 16:32:05.000000 haicu-0.9.0/haicu/__init__.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)       78 2023-05-10 16:43:20.000000 haicu-0.9.0/haicu/__main__.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    22183 2023-05-10 17:05:04.000000 haicu-0.9.0/haicu/format.py
+-rw-rw-r--   0 bry       (1000) bry       (1000)    15626 2023-05-10 17:07:01.000000 haicu-0.9.0/haicu/ftdi.py
+-rwxrwxr-x   0 bry       (1000) bry       (1000)    27584 2023-05-10 17:12:22.000000 haicu-0.9.0/haicu/haicu_ctl.py
+drwxrwxr-x   0 bry       (1000) bry       (1000)        0 2023-05-10 17:20:29.235020 haicu-0.9.0/haicu.egg-info/
+-rw-rw-r--   0 bry       (1000) bry       (1000)     4144 2023-05-10 17:20:29.000000 haicu-0.9.0/haicu.egg-info/PKG-INFO
+-rw-rw-r--   0 bry       (1000) bry       (1000)      293 2023-05-10 17:20:29.000000 haicu-0.9.0/haicu.egg-info/SOURCES.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        1 2023-05-10 17:20:29.000000 haicu-0.9.0/haicu.egg-info/dependency_links.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       51 2023-05-10 17:20:29.000000 haicu-0.9.0/haicu.egg-info/entry_points.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)       29 2023-05-10 17:20:29.000000 haicu-0.9.0/haicu.egg-info/requires.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)        6 2023-05-10 17:20:29.000000 haicu-0.9.0/haicu.egg-info/top_level.txt
+-rw-rw-r--   0 bry       (1000) bry       (1000)      830 2023-05-10 17:19:58.000000 haicu-0.9.0/pyproject.toml
+-rw-rw-r--   0 bry       (1000) bry       (1000)       38 2023-05-10 17:20:29.235020 haicu-0.9.0/setup.cfg
```

### Comparing `haicu-0.8.3/LICENSE` & `haicu-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `haicu-0.8.3/PKG-INFO` & `haicu-0.9.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.8.3
-Summary: package for HAICU
+Version: 0.9.0
+Summary: package for HAICU experiment
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,73 +26,67 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# HAICU
+# HAICU Control Script (haicu-ctl)
 
 ## Overview
 
 Package and command line utility for controlling and sequencing the MLD1200
 
-The available subcommands are:
-
-- `list` - List of available MLD1200 devices
-- `info` - Get full report on MLD1200, all registers and status bits
-- `set` - Allows human-readable setting of register values
-- `upload` - Upload a new sequence into MLD1200 (does not run!)
-- `program` - Upload and start sequence
-- `convert` - Convert derived.txt file into .RLE format
-- `compare` - Compare a derived file to an RLE file
-- `csv` - Future use. Will convert .csv directly to RLE
-- `monitor` - Attach to MLD and log errors
-
-Diagnostic subcommands:
-- `memtest` - Test the selected MLD by writing then reading random values to DDR memory
-- `status` - Low level readback of status registers
-- `control` - Low level read/write of control registers
-- `memory` - Low level read/write of DDR memory
-- `bread` - Low level block read of DDR memory section
-
 ## Installation
 
 The recommended installation method is via pip
 
-  To install:
-    `pip install haicu`
-
-  To upgrade:
+  To install/upgrade:
     `pip install -U haicu`
 
   To run it locally from the source (from the `scripts/haicu` directory):
     `python -m haicu`
 
-## Interactive
+## Usage
+
+Command:
+`haicu-ctl [-h] [--version] [-v] [-l file] [-s SERIAL] [-j] {list,info,set,upload,program,convert,compare}`
 
- Command:
-  `haicu-ctl [-h] [--version] [-v] [-l file] [-s SERIAL] [-j] {list,info,set,upload,program,convert,compare,csv,monitor}`
+Purpose:
+Connects to an MLD1200 device and reads/writes registers, statuses, and memory. Also contains utility functions to create .RLE files for consumption by device.
 
- Purpose:
-  Connects to an MLD1200 device and reads/writes registers, statuses, and memory. Also contains utility functions to create .RLE files for consumption by device.
+Options:
 
- Options:
+`-h` or `--help`
+Print out help for general usage or subcommand. Ie: `haicu-ctl -h` or `haicu-ctl set -h`
 
-  `-h` or `--help`
-  Print out help for general usage or subcommand. Ie: `haicu-ctl -h` or `haicu-ctl reg -h`
+`--version`
+Print out current version
 
-  `--version`
-  Print out current version
+`-v` or `--verbose`
+  Increase logging level, can be used multiple times
 
-  `-v` or `--verbose`
-   Increase logging level, can be used multiple times
+`-l LOG_FILE` or `--log LOG_FILE`
+  Specify log file name, instead of standard naming scheme
 
-  `-l LOG_FILE` or `--log LOG_FILE`
-   Specify log file name, instead of standard naming scheme
+`-s SERIAL` or `--serial SERIAL`
+  Specify serial number of MLD1200 to connect to
 
-  `-s SERIAL` or `--serial SERIAL`
-   Specify serial number of MLD1200 to connect to
+`-j` or `--json`
+  For reads, format output in JSON. Only affects `set` (with no value), `info`, `status`, `control`, `memory`, and `bread`
 
-  `-j` or `--json`
-   For reads, format output in JSON. Only affects `info`, `register`, `memory`, and `bread`
+The available subcommands are:
 
+- `list` - List of available MLD1200 devices
+- `info` - Get full report on MLD1200, all registers and status bits
+- `set <regname> [data]` - Allows human-readable setting of register values. If data is omitted, returns current value in register
+- `upload <file> <section>` - Upload a new sequence into MLD1200 from file. Choose section to load ('left','right','extension'). Does not start sequence.
+- `program [config_file] [--auto/-a]` - Upload and start sequence. Can be passed a path to an INI file, otherwise tries to use 'haicu.ini' in current directory. The '--auto' option auto-reload the sequencer when it finishes, it will then start again on next trigger.
+- `convert <infile> <outfile>` - Convert a derived format file 'infile' into RLE formatted file 'outfile'
+- `compare <derived_file> <rle_file>` - Compare a derived file to an RLE file
+
+Diagnostic subcommands:
+- `memtest` - Test the selected MLD by writing and reading random values to DDR memory
+- `status <addr>` - Low level readback of status register at given address
+- `control <addr> [data]` - Low level read/write of control registers. Omit 'data' to return current value at given address
+- `memory <addr> [data]` - Low level read/write of DDR memory. Omit 'data' to return current value at given address
+- `bread <addr> <count>` - Low level block read of DDR memory section. Reads 'count' words out of DDR started at given address
```

### Comparing `haicu-0.8.3/haicu/__main__.py` & `haicu-0.9.0/haicu/haicu_ctl.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/bin/python
 
 import signal
 import argparse
 import sys
 import random
 import time
+import datetime
 import configparser
 import os
 import pprint
-import pkg_resources
 from simplejson import dumps
 from . import ftdi as haicu_ftdi
 from . import format as haicu_format
+from . import __version__ as __version__
 
-VERSION = pkg_resources.get_distribution('haicu').version
+VERSION = __version__
 
 # Table to convert 'get' request name to status register address
 GET_REG_TABLE = {
     'invert_frontpanel': 23,
     'invert_right_address': 22,
     'invert_left_address': 21,
     'invert_tunebox8': 20,
@@ -73,34 +74,49 @@
         self.state = True
 
     def exit(self):
         return self.state
 
 flag = GracefulExiter()
 
+def rmr_register(ftdi_dev, addr, mask, offset, data):
+    init_value = (haicu_ftdi.read_register(ftdi_dev, addr) & ~mask)
+    new_value = (data << offset) & mask
+    haicu_ftdi.write_register(ftdi_dev, addr, new_value | init_value)
+
+def read_masked_register(ftdi_dev, addr, mask, offset):
+    return (haicu_ftdi.read_register(ftdi_dev, addr) & mask) >> offset
+
+def handle_set(name, ftdi_dev, addr, mask, offset, data, json):
+        if(data == None):
+            result = read_masked_register(ftdi_dev, addr, mask, offset)
+            print("0x" + '{:02X}'.format(result)) if(not json) else  print("{\"" + name + "\": 0x" + '{:02X}'.format(result) + "}")
+        else:
+            rmr_register(ftdi_dev, addr, mask, offset, int(data, 0))
+
 def main():
     prog='haicu_ctl'
     parser = argparse.ArgumentParser(prog=prog)
-    parser.add_argument('--version', action='version', version='%(prog)s ' + VERSION)
+    parser.add_argument('--version', action='version', version='%(prog)s ' + str(VERSION))
     parser.add_argument('-v', '--verbose', action='count', default=0, help='Increase logging verbosity, can be repeated')
     parser.add_argument('-l', '--log', metavar='file', help='Log to output file')
     parser.add_argument('-s', '--serial', type=str, default='', help='MLD1200 serial of device to connect')
     parser.add_argument('-j', '--json', default=False, action='store_true', help='Send response as JSON object')
 
-    cmd_parser = parser.add_subparsers(metavar='{list,info,set,upload,program,convert,compare,monitor}', dest="command", description="Valid subcommands", help=" ")
+    cmd_parser = parser.add_subparsers(metavar='{list,info,set,upload,program,convert,compare}', dest="command", description="Valid subcommands", help=" ")
 
     ftdi_list_parser = cmd_parser.add_parser("list", help="List available MLD1200 devices")
     ftdi_list_parser.set_defaults(func=arg_list)
 
     get_parser = cmd_parser.add_parser("info", help="Get status information")
     get_parser.set_defaults(func=arg_info)
 
     set_parser = cmd_parser.add_parser("set", help="Read/Write control value")
     set_parser.set_defaults(func=arg_set)
-    set_parser.add_argument("request", type=str, action=RenameSetChoice, choices=GET_REG_TABLE)
+    set_parser.add_argument("regname", type=str, action=RenameSetChoice, choices=GET_REG_TABLE)
     set_parser.add_argument("data", nargs='?', type=str, help="Value to write")
 
     upload_parser = cmd_parser.add_parser("upload", help="Upload file to memory")
     upload_parser.set_defaults(func=arg_upload)
     upload_parser.add_argument("file", type=str, help="Program file to upload")
     upload_parser.add_argument("section", action=RenameProgramChoice, choices=GET_PROGRAM_TABLE)
 
@@ -115,20 +131,17 @@
     convert_parser.set_defaults(func=arg_convert)
 
     compare_parser = cmd_parser.add_parser("compare", help="Compare derived file to rle")
     compare_parser.add_argument("dfile", type=str, help="Derived file to compare")
     compare_parser.add_argument("rfile", type=str, help="RLE file to compare")
     compare_parser.set_defaults(func=arg_compare)
 
-    csv_parser = cmd_parser.add_parser("csv", help="Parse CSV file")
-    csv_parser.add_argument("csvfile", type=str, help="CSV sum file")
-    csv_parser.set_defaults(func=arg_csv)
-
-    monitor_parser = cmd_parser.add_parser("monitor", help="Monitor MLD1200")
-    monitor_parser.set_defaults(func=arg_monitor)
+    # csv_parser = cmd_parser.add_parser("csv", help="Parse CSV file")
+    # csv_parser.add_argument("csvfile", type=str, help="CSV sum file")
+    # csv_parser.set_defaults(func=arg_csv)
 
     status_parser = cmd_parser.add_parser("status", aliases=['stat'])
     status_parser.set_defaults(func=arg_status)
     status_parser.add_argument("addr", type=str, help="address to read")
 
     reg_parser = cmd_parser.add_parser("control", aliases=['ctrl'])
     reg_parser.set_defaults(func=arg_reg)
@@ -144,14 +157,17 @@
     block_parser.set_defaults(func=arg_block)
     block_parser.add_argument("addr", type=str, help="24-bit address to read")
     block_parser.add_argument("count", type=str, help="Number of words to read")
 
     memtest_parser = cmd_parser.add_parser("memtest")
     memtest_parser.set_defaults(func=arg_memtest)
 
+    stop_parser = cmd_parser.add_parser("stop")
+    stop_parser.set_defaults(func=arg_stop)
+
     args = parser.parse_args()
 
     try:
         ftdi_dev = haicu_ftdi.init(args.serial)
     except:
         print("Device '" + str(args.serial) + "' not found!")
         print()
@@ -164,15 +180,15 @@
 
     args.func(args, ftdi_dev)
 
 def arg_list(args, ftdi_dev):
     print("Available devices:")
     result = haicu_ftdi.list_devices()
     for n, r in enumerate(result):
-        print(str(n+1) + "\t" + str(r[0]) + "\t" + str(r[1]))
+        print(str(n+1) + "\t" + str(r))
 
     if(len(result) == 0):
         print("No devices found")
 
 def arg_memtest(args, ftdi_dev):
     # Generate random data of 'tlen' length
     tlen = 1048576 # number of 32-bit words to transfer
@@ -205,14 +221,18 @@
     for n in range(0, tlen):
         if(result[n] != test_data[n]):
             print("Mismatch at " + str(n) + "\tExpected: " + str(test_data[n]) + " Result: " + str(result[n]))
             sys.exit(-1)
 
     print("Verification Successful")
 
+
+def arg_stop(args, ftdi_dev):
+    haicu_ftdi.write_register(ftdi_dev, 0, 0)
+
 ## Converts status values into human read-able format
 def arg_info(args, ftdi_dev):
     status_resp = haicu_ftdi.gather_status_registers(ftdi_dev)
     control_resp = haicu_ftdi.gather_control_registers(ftdi_dev)
 
     if(not args.json):
         print("Status:")
@@ -222,20 +242,22 @@
         print("\tProgram Active: " + str(status_resp['program_active']))
         print("\tProgram Done: " + str(status_resp['program_done']))
         print("\tProgram Error: " + str(status_resp['program_error']))
         print("\tProgram DDR Load: " + str(status_resp['program_ddr_load']))
         print("\tProgram DDR Lock: " + str(status_resp['program_ddr_lock']))
         print("\tProgram Run Count: " + str(status_resp['program_run_count']))
         print("\tProgram Error Count: " + str(status_resp['program_error_count']))
+        print("\tProgram Run Timer: " + str(status_resp['program_run_timer'] * 10) + " ns")
         print()
         print("\tTrigger Active: " + str(status_resp['trigger_active']))
         print("\tTrigger Counter: " + str(status_resp['trigger_counter']))
-        print("\tExternal Clock Frequency: " + f"{status_resp['external_clock_freq']:.3f}" + " MHz")
+        print("\tExternal Clock Frequency: " + f"{(status_resp['external_clock_freq']/1000000):.3f}" + " MHz")
         print("\tExternal Clock Active: " + str(status_resp['external_clock_active']))
         print("\tExternal Clock Counter: " + str(status_resp['external_clock_counter']))
+        print("\tUptime: " + str(datetime.timedelta(seconds=status_resp['uptime'])))
         print("\tBuildtime: "+ str(status_resp['buildtime']))
         print()
         print("Control:")
         print("\tProgram Load: " + str(control_resp['program_load']))
         print("\tProgram Numwords: " + str(control_resp['program_numwords']))
         print()
         print("\tTrigger Inverted: " + str(control_resp['trigger_invert']))
@@ -267,136 +289,102 @@
         print("\tInvert Left Address: 0x" + f"{(control_resp['invert_left_address']):03X}")
         print("\tInvert Right Address: 0x" + f"{(control_resp['invert_right_address']):03X}")
     else:
         print("{\"status\":" + dumps(status_resp) + ",\"control\":" + dumps(control_resp) + "}")
 
 ## Converts register values into human read-able format
 def arg_set(args, ftdi_dev):
-    addr = args.request
+    addr = args.regname
     if(addr == GET_REG_TABLE["trigger_invert"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 2) & 0xBFFFFFFF
-        value = (int(args.data, 0) & 0x1) << 30
-        haicu_ftdi.write_register(ftdi_dev, 2, value | init_value)
+        handle_set("trigger_invert", ftdi_dev, 2, 0x40000000, 30, args.data, args.json)
 
     if(addr == GET_REG_TABLE["trigger_delay"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 2) & 0xFFFFFF00
-        value = (int(args.data, 0) & 0xFF)
-        haicu_ftdi.write_register(ftdi_dev, 2, value | init_value)
+        handle_set("trigger_delay", ftdi_dev, 2, 0x000000FF, 0, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_tunebox1"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 3) & 0xFFFFFF00
-        value = (int(args.data, 0) & 0xFF)
-        haicu_ftdi.write_register(ftdi_dev, 3, value | init_value)
+        handle_set("enable_tunebox1", ftdi_dev, 3, 0x000000FF, 0, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_tunebox2"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 3) & 0xFFFF00FF
-        value = (int(args.data, 0) & 0xFF) << 8
-        haicu_ftdi.write_register(ftdi_dev, 3, value | init_value)
+        handle_set("enable_tunebox2", ftdi_dev, 3, 0x0000FF00, 8, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_tunebox3"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 3) & 0xFF00FFFF
-        value = (int(args.data, 0) & 0xFF) << 16
-        haicu_ftdi.write_register(ftdi_dev, 3, value | init_value)
+        handle_set("enable_tunebox3", ftdi_dev, 3, 0x00FF0000, 16, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_tunebox4"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 3) & 0x00FFFFFF
-        value = (int(args.data, 0) & 0xFF) << 24
-        haicu_ftdi.write_register(ftdi_dev, 3, value | init_value)
+        handle_set("enable_tunebox4", ftdi_dev, 3, 0xFF000000, 24, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_tunebox5"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 4) & 0xFFFFFF00
-        value = (int(args.data, 0) & 0xFF)
-        haicu_ftdi.write_register(ftdi_dev, 4, value | init_value)
+        handle_set("enable_tunebox5", ftdi_dev, 4, 0x000000FF, 0, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_tunebox6"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 4) & 0xFFFF00FF
-        value = (int(args.data, 0) & 0xFF) << 8
-        haicu_ftdi.write_register(ftdi_dev, 4, value | init_value)
+        handle_set("enable_tunebox6", ftdi_dev, 4, 0x0000FF00, 8, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_tunebox7"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 4) & 0xFF00FFFF
-        value = (int(args.data, 0) & 0xFF) << 16
-        haicu_ftdi.write_register(ftdi_dev, 4, value | init_value)
+        handle_set("enable_tunebox7", ftdi_dev, 4, 0x00FF0000, 16, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_tunebox8"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 4) & 0x00FFFFFF
-        value = (int(args.data, 0) & 0xFF) << 24
-        haicu_ftdi.write_register(ftdi_dev, 4, value | init_value)
+        handle_set("enable_tunebox8", ftdi_dev, 4, 0xFF000000, 24, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_left_address"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 5) & 0xFFFFF000
-        value = (int(args.data, 0) & 0xFFF)
-        haicu_ftdi.write_register(ftdi_dev, 5, value | init_value)
+        handle_set("enable_left_address", ftdi_dev, 5, 0x00000FFF, 0, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_right_address"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 5) & 0xF000FFFF
-        value = (int(args.data, 0) & 0xFFF) << 16
-        haicu_ftdi.write_register(ftdi_dev, 5, value | init_value)
+        handle_set("enable_right_address", ftdi_dev, 5, 0x0FFF0000, 16, args.data, args.json)
 
     if(addr == GET_REG_TABLE["enable_frontpanel"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 5) & 0x0FFF0FFF
-        value1 = (int(args.data, 0) & 0x0F) << 12
-        value2 = (int(args.data, 0) & 0xF0) << 24
-        haicu_ftdi.write_register(ftdi_dev, 5, value1 | value2 | init_value)
+        if(args.data == None):
+            top = read_masked_register(ftdi_dev, 5, 0xF0000000, 28)
+            btm = read_masked_register(ftdi_dev, 5, 0x0000F000, 12)
+            result = (top << 4) | btm
+            print("0x" + '{:02X}'.format(result)) if(not args.json) else print("{\"enable_frontpanel\": 0x" + '{:02X}'.format(result) + "}")
+        else:
+            value = int(args.data, 0) & 0xFF
+            rmr_register(ftdi_dev, 5, 0xF0000000, 28, (value & 0xF0) >> 4)
+            rmr_register(ftdi_dev, 5, 0x0000F000, 12, value & 0x0F)
 
     if(addr == GET_REG_TABLE["invert_tunebox1"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 6) & 0xFFFFFF00
-        value = (int(args.data, 0) & 0xFF)
-        haicu_ftdi.write_register(ftdi_dev, 6, value | init_value)
+        handle_set("invert_tunebox1", ftdi_dev, 6, 0x000000FF, 0, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_tunebox2"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 6) & 0xFFFF00FF
-        value = (int(args.data, 0) & 0xFF) << 8
-        haicu_ftdi.write_register(ftdi_dev, 6, value | init_value)
+        handle_set("invert_tunebox2", ftdi_dev, 6, 0x0000FF00, 8, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_tunebox3"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 6) & 0xFF00FFFF
-        value = (int(args.data, 0) & 0xFF) << 16
-        haicu_ftdi.write_register(ftdi_dev, 6, value | init_value)
+        handle_set("invert_tunebox3", ftdi_dev, 6, 0x00FF0000, 16, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_tunebox4"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 6) & 0x00FFFFFF
-        value = (int(args.data, 0) & 0xFF) << 24
-        haicu_ftdi.write_register(ftdi_dev, 6, value | init_value)
+        handle_set("invert_tunebox4", ftdi_dev, 6, 0xFF000000, 24, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_tunebox5"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 7) & 0xFFFFFF00
-        value = (int(args.data, 0) & 0xFF)
-        haicu_ftdi.write_register(ftdi_dev, 7, value | init_value)
+        handle_set("invert_tunebox5", ftdi_dev, 7, 0x000000FF, 0, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_tunebox6"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 7) & 0xFFFF00FF
-        value = (int(args.data, 0) & 0xFF) << 8
-        haicu_ftdi.write_register(ftdi_dev, 7, value | init_value)
+        handle_set("invert_tunebox6", ftdi_dev, 7, 0x0000FF00, 8, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_tunebox7"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 7) & 0xFF00FFFF
-        value = (int(args.data, 0) & 0xFF) << 16
-        haicu_ftdi.write_register(ftdi_dev, 7, value | init_value)
+        handle_set("invert_tunebox7", ftdi_dev, 7, 0x00FF0000, 16, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_tunebox8"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 7) & 0x00FFFFFF
-        value = (int(args.data, 0) & 0xFF) << 24
-        haicu_ftdi.write_register(ftdi_dev, 7, value | init_value)
+        handle_set("invert_tunebox8", ftdi_dev, 7, 0xFF000000, 24, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_left_address"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 8) & 0xFFFFF000
-        value = (int(args.data, 0) & 0xFFF)
-        haicu_ftdi.write_register(ftdi_dev, 8, value | init_value)
+        handle_set("invert_left_address", ftdi_dev, 8, 0x00000FFF, 0, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_right_address"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 8) & 0xF000FFFF
-        value = (int(args.data, 0) & 0xFFF) << 16
-        haicu_ftdi.write_register(ftdi_dev, 8, value | init_value)
+        handle_set("invert_right_address", ftdi_dev, 8, 0x0FFF0000, 16, args.data, args.json)
 
     if(addr == GET_REG_TABLE["invert_frontpanel"]):
-        init_value = haicu_ftdi.read_register(ftdi_dev, 8) & 0x0FFF0FFF
-        value1 = (int(args.data, 0) & 0x0F) << 12
-        value2 = (int(args.data, 0) & 0xF0) << 24
-        haicu_ftdi.write_register(ftdi_dev, 8, value1 | value2 | init_value)
+        if(args.data == None):
+            top = read_masked_register(ftdi_dev, 8, 0xF0000000, 28)
+            btm = read_masked_register(ftdi_dev, 8, 0x0000F000, 12)
+            result = (top << 4) | btm
+            print("0x" + '{:02X}'.format(result)) if(not args.json) else print("{\"invert_frontpanel\": 0x" + '{:02X}'.format(result) + "}")
+        else:
+            value = int(args.data, 0) & 0xFF
+            rmr_register(ftdi_dev, 8, 0xF0000000, 28, (value & 0xF0) >> 4)
+            rmr_register(ftdi_dev, 8, 0x0000F000, 12, value & 0x0F)
 
 ## Low level status register read
 def arg_status(args, ftdi_dev):
     addr = int(args.addr, 0)
     val = haicu_ftdi.read_status(ftdi_dev, addr)
     if(not args.json):
         if(val != None):
@@ -491,30 +479,30 @@
         sys.exit(-1)
 
     in_name, in_ext = os.path.splitext(args.file)
 
     try:
         if(in_ext.lower() == ".txt"):
             print("Generating RLE from " + args.file)
-            rle = haicu_format.convert_derived2rle(args.file)
+            rle = haicu_format.convert_derived_absolute2rle(args.file)
         elif(in_ext.lower() == ".rle"):
             rle = haicu_format.load_rle_from_file(args.file)
         else:
             print("Invalid filetype " + in_ext + ". Must be .rle or .txt")
             sys.exit(-1)
 
     except:
         if(os.path.exists(args.file)):
             print("Error parsing " + args.file)
         else:
             print("File not found: " + args.file)
             sys.exit(-1)
 
     upload(ftdi_dev, rle, args.section, args.verbose)
-    # haicu_ftdi.write_register(ftdi_dev, 0, 1) # Turn on program load
+
 
 def arg_program(args, ftdi_dev):
     if(not os.path.exists(args.config_file)):
         if(args.verbose > 0):
             print("Config file " + args.config_file + " not found")
         sys.exit(-1)
 
@@ -525,15 +513,15 @@
     in_name, in_ext = os.path.splitext(in_file)
 
     # Load the RLE file
     try:
         if(in_ext.lower() == ".txt"):
             if(args.verbose > 0):
                 print("Generating RLE from " + in_file)
-            rle = haicu_format.convert_derived2rle(in_file)
+            rle = haicu_format.convert_derived_absolute2rle(in_file)
         elif(in_ext.lower() == ".rle"):
             if(args.verbose > 0):
                 print("Loading RLE payload from " + in_file)
             rle = haicu_format.load_rle_from_file(in_file)
         else:
             if(args.verbose > 0):
                 print("Invalid filetype " + in_ext + ". Must be .rle or .txt")
@@ -575,20 +563,19 @@
             # Turn on program load
             val = haicu_ftdi.read_register(dev, 0)
             if(args.auto):
                 val = val | 0x40000000
             haicu_ftdi.write_register(dev, 0, 0x80000000 | val)
         else:
             if(args.verbose > 0):
-                print("No device specified for " + section_name + " section")
+                print("No device specified for " + section_name + " section. Ignoring section in file")
 
         if(args.verbose > 0):
             print()
 
-    monitor(dev_list)
 
 def arg_convert(args, ftdi_dev):
     if(args.verbose > 0):
         print("Converting " + args.infile + " to RLE")
 
     in_name, in_ext = os.path.splitext(args.infile)
     if(in_ext != ".txt"):
@@ -596,49 +583,38 @@
         sys.exit(-1)
 
     out_name, out_ext = os.path.splitext(args.outfile)
     if(out_ext != ".rle"):
         print("Invalid extension, output file must be .rle")
         sys.exit(-1)
 
-    rle = haicu_format.convert_derived2rle(args.infile)
+    rle = haicu_format.convert_derived_absolute2rle(args.infile)
     if(args.verbose > 1):
         pprint.pprint(rle) # Debug print, only useful for tiny derived.txt files
 
     if(args.verbose > 0):
         print("Creating RLE file " + args.outfile)
 
     with open(args.outfile, "wb+") as f:
         for n in range(len(rle)):
             f.write(rle[n])
 
 def arg_compare(args, ftdi_dev):
     # Verification
-    if(haicu_format.match(args.dfile, args.rfile, args.verbose)):
+    if(haicu_format.match(args.dfile, args.rfile)):
         if(args.verbose > 0):
             print("RLE and Derived files match")
     else:
         if(args.verbose > 0):
             print("RLE and Derived files do not match!")
             print()
             sys.exit(-1)
 
-def arg_monitor(args, ftdi_dev):
-    monitor([ftdi_dev])
-
-def arg_csv(args, ftdi_dev):
-    haicu_format.convert_sum_to_obj(args.csvfile)
-
-def monitor(ftdi_dev_list):
-    log = ""
-    while(not flag.state):
-        for ftdi_dev in ftdi_dev_list:
-            log = log + hex(haicu_ftdi.read_status(ftdi_dev, 0)) + "\n"
-
-    print(log)
+# def arg_csv(args, ftdi_dev):
+#     haicu_format.convert_sum_to_obj(args.csvfile)
 
 def upload(ftdi_dev, rle, mld_section, verbose):
     section_name = next(key for key, value in GET_PROGRAM_TABLE.items() if value == mld_section)
 
     if(mld_section >= len(rle)):
         print("MLD section '" + section_name + "' does not exist")
         sys.exit(-1)
@@ -683,9 +659,7 @@
             print("Payload length in bytes: " + str(tlen * 4))
             print("Updating program count register")
 
         haicu_ftdi.write_register(ftdi_dev, 1, tlen) # Load program count
     else:
         print("Verification failed. Null result payload")
 
-if __name__ == "__main__":
-    main()
```

### Comparing `haicu-0.8.3/haicu.egg-info/PKG-INFO` & `haicu-0.9.0/haicu.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: haicu
-Version: 0.8.3
-Summary: package for HAICU
+Version: 0.9.0
+Summary: package for HAICU experiment
 Author-email: Bryerton Shaw <bryerton@triumf.ca>
 Maintainer-email: Bryerton Shaw <bryerton@triumf.ca>
 License: MIT License
         
         Copyright (c) [2023] [Bryerton Shaw]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,73 +26,67 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# HAICU
+# HAICU Control Script (haicu-ctl)
 
 ## Overview
 
 Package and command line utility for controlling and sequencing the MLD1200
 
-The available subcommands are:
-
-- `list` - List of available MLD1200 devices
-- `info` - Get full report on MLD1200, all registers and status bits
-- `set` - Allows human-readable setting of register values
-- `upload` - Upload a new sequence into MLD1200 (does not run!)
-- `program` - Upload and start sequence
-- `convert` - Convert derived.txt file into .RLE format
-- `compare` - Compare a derived file to an RLE file
-- `csv` - Future use. Will convert .csv directly to RLE
-- `monitor` - Attach to MLD and log errors
-
-Diagnostic subcommands:
-- `memtest` - Test the selected MLD by writing then reading random values to DDR memory
-- `status` - Low level readback of status registers
-- `control` - Low level read/write of control registers
-- `memory` - Low level read/write of DDR memory
-- `bread` - Low level block read of DDR memory section
-
 ## Installation
 
 The recommended installation method is via pip
 
-  To install:
-    `pip install haicu`
-
-  To upgrade:
+  To install/upgrade:
     `pip install -U haicu`
 
   To run it locally from the source (from the `scripts/haicu` directory):
     `python -m haicu`
 
-## Interactive
+## Usage
+
+Command:
+`haicu-ctl [-h] [--version] [-v] [-l file] [-s SERIAL] [-j] {list,info,set,upload,program,convert,compare}`
 
- Command:
-  `haicu-ctl [-h] [--version] [-v] [-l file] [-s SERIAL] [-j] {list,info,set,upload,program,convert,compare,csv,monitor}`
+Purpose:
+Connects to an MLD1200 device and reads/writes registers, statuses, and memory. Also contains utility functions to create .RLE files for consumption by device.
 
- Purpose:
-  Connects to an MLD1200 device and reads/writes registers, statuses, and memory. Also contains utility functions to create .RLE files for consumption by device.
+Options:
 
- Options:
+`-h` or `--help`
+Print out help for general usage or subcommand. Ie: `haicu-ctl -h` or `haicu-ctl set -h`
 
-  `-h` or `--help`
-  Print out help for general usage or subcommand. Ie: `haicu-ctl -h` or `haicu-ctl reg -h`
+`--version`
+Print out current version
 
-  `--version`
-  Print out current version
+`-v` or `--verbose`
+  Increase logging level, can be used multiple times
 
-  `-v` or `--verbose`
-   Increase logging level, can be used multiple times
+`-l LOG_FILE` or `--log LOG_FILE`
+  Specify log file name, instead of standard naming scheme
 
-  `-l LOG_FILE` or `--log LOG_FILE`
-   Specify log file name, instead of standard naming scheme
+`-s SERIAL` or `--serial SERIAL`
+  Specify serial number of MLD1200 to connect to
 
-  `-s SERIAL` or `--serial SERIAL`
-   Specify serial number of MLD1200 to connect to
+`-j` or `--json`
+  For reads, format output in JSON. Only affects `set` (with no value), `info`, `status`, `control`, `memory`, and `bread`
 
-  `-j` or `--json`
-   For reads, format output in JSON. Only affects `info`, `register`, `memory`, and `bread`
+The available subcommands are:
 
+- `list` - List of available MLD1200 devices
+- `info` - Get full report on MLD1200, all registers and status bits
+- `set <regname> [data]` - Allows human-readable setting of register values. If data is omitted, returns current value in register
+- `upload <file> <section>` - Upload a new sequence into MLD1200 from file. Choose section to load ('left','right','extension'). Does not start sequence.
+- `program [config_file] [--auto/-a]` - Upload and start sequence. Can be passed a path to an INI file, otherwise tries to use 'haicu.ini' in current directory. The '--auto' option auto-reload the sequencer when it finishes, it will then start again on next trigger.
+- `convert <infile> <outfile>` - Convert a derived format file 'infile' into RLE formatted file 'outfile'
+- `compare <derived_file> <rle_file>` - Compare a derived file to an RLE file
+
+Diagnostic subcommands:
+- `memtest` - Test the selected MLD by writing and reading random values to DDR memory
+- `status <addr>` - Low level readback of status register at given address
+- `control <addr> [data]` - Low level read/write of control registers. Omit 'data' to return current value at given address
+- `memory <addr> [data]` - Low level read/write of DDR memory. Omit 'data' to return current value at given address
+- `bread <addr> <count>` - Low level block read of DDR memory section. Reads 'count' words out of DDR started at given address
```

