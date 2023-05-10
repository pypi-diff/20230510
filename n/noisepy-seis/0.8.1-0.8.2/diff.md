# Comparing `tmp/noisepy_seis-0.8.1.tar.gz` & `tmp/noisepy_seis-0.8.2.tar.gz`

## Comparing `noisepy_seis-0.8.1.tar` & `noisepy_seis-0.8.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/S0A_download_ASDF_MPI.py
--rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/S0B_to_ASDF.py
--rw-r--r--   0        0        0    13464 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/S1_fft_cc_MPI.py
--rw-r--r--   0        0        0    15939 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/S2_stacking.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/_version.py
--rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/asdfstore.py
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/channelcatalog.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/constants.py
--rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/datatypes.py
--rw-r--r--   0        0        0     7105 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/main.py
--rw-r--r--   0        0        0   112958 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/noise_module.py
--rw-r--r--   0        0        0    35085 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/plotting_modules.py
--rw-r--r--   0        0        0     4937 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/scedc_s3store.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/stores.py
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/utils.py
--rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/application_modules/comp_stacking.py
--rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/application_modules/dispersion_analysis.py
--rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/application_modules/measure_dvv.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/src/noisepy/seis/application_modules/write_sac.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/.gitignore
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/LICENSE
--rw-r--r--   0        0        0     7056 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/README.md
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     9513 2020-02-02 00:00:00.000000 noisepy_seis-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    12029 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/S0A_download_ASDF_MPI.py
+-rw-r--r--   0        0        0     9641 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/S0B_to_ASDF.py
+-rw-r--r--   0        0        0    13464 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/S1_fft_cc_MPI.py
+-rw-r--r--   0        0        0    15939 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/S2_stacking.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/_version.py
+-rw-r--r--   0        0        0     6492 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/asdfstore.py
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/channelcatalog.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/constants.py
+-rw-r--r--   0        0        0     5521 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/datatypes.py
+-rw-r--r--   0        0        0     7274 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/main.py
+-rw-r--r--   0        0        0   112958 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/noise_module.py
+-rw-r--r--   0        0        0    35085 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/plotting_modules.py
+-rw-r--r--   0        0        0     5805 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/scedc_s3store.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/stores.py
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/utils.py
+-rw-r--r--   0        0        0    12253 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/application_modules/comp_stacking.py
+-rw-r--r--   0        0        0     6882 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/application_modules/dispersion_analysis.py
+-rw-r--r--   0        0        0    14886 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/application_modules/measure_dvv.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/src/noisepy/seis/application_modules/write_sac.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/.gitignore
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/LICENSE
+-rw-r--r--   0        0        0     7569 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/README.md
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0    10026 2020-02-02 00:00:00.000000 noisepy_seis-0.8.2/PKG-INFO
```

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/S0A_download_ASDF_MPI.py` & `noisepy_seis-0.8.2/src/noisepy/seis/S0A_download_ASDF_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/S0B_to_ASDF.py` & `noisepy_seis-0.8.2/src/noisepy/seis/S0B_to_ASDF.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/S1_fft_cc_MPI.py` & `noisepy_seis-0.8.2/src/noisepy/seis/S1_fft_cc_MPI.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/S2_stacking.py` & `noisepy_seis-0.8.2/src/noisepy/seis/S2_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/__init__.py` & `noisepy_seis-0.8.2/src/noisepy/seis/__init__.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/asdfstore.py` & `noisepy_seis-0.8.2/src/noisepy/seis/asdfstore.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/channelcatalog.py` & `noisepy_seis-0.8.2/src/noisepy/seis/channelcatalog.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/datatypes.py` & `noisepy_seis-0.8.2/src/noisepy/seis/datatypes.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/main.py` & `noisepy_seis-0.8.2/src/noisepy/seis/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import argparse
 import os
 import typing
 from enum import Enum
 from typing import Any, Callable, List
 
 import obspy
+from datetimerange import DateTimeRange
 
 from .asdfstore import ASDFCCStore, ASDFRawDataStore
 from .channelcatalog import CSVChannelCatalog, XMLStationChannelCatalog
 from .constants import DATE_FORMAT_HELP, STATION_FILE
 from .datatypes import Channel, ConfigParameters
 from .S0A_download_ASDF_MPI import download
 from .S1_fft_cc_MPI import cross_correlate
 from .S2_stacking import stack
 from .scedc_s3store import SCEDCS3DataStore
 from .utils import fs_join, get_filesystem
 
 # Utility running the different steps from the command line. Defines the arguments for each step
 
-default_start_date = "2016_07_01_0_0_0"  # start date of download
-default_end_date = "2016_07_02_0_0_0"  # end date of download
 default_data_path = "Documents/SCAL"
 
 
 class Step(Enum):
     DOWNLOAD = 1
     CROSS_CORRELATE = 2
     STACK = 3
@@ -54,87 +53,94 @@
     if len(sta_list) == 1 and sta_list[0] == "*":
         return lambda ch: True
     else:
         stations = set(sta_list)
         return lambda ch: ch.station.name in stations
 
 
-def create_raw_store(raw_dir: str, sta_list: List[str], xml_path: str):
+def get_date_range(args) -> DateTimeRange:
+    if args.start is None or args.end is None:
+        return None
+    return DateTimeRange(obspy.UTCDateTime(args.start).datetime, obspy.UTCDateTime(args.end).datetime)
+
+
+def create_raw_store(args):
+    stations = args.stations if "stations" in args else []
+    xml_path = args.xml_path if "xml_path" in args else None
+    raw_dir = args.raw_data_path
+
     fs = get_filesystem(raw_dir)
 
     def count(pat):
         return len(fs.glob(fs_join(raw_dir, pat)))
 
     # Use heuristics around which store to use by the files present
     if count("*.h5") > 0:
         return ASDFRawDataStore(raw_dir)
     else:
-        assert count("*.ms") > 0 or count("*.sac") > 0, f"Can not find any .h5, .ms or .sac files in {raw_dir}"
+        # assert count("*.ms") > 0 or count("*.sac") > 0, f"Can not find any .h5, .ms or .sac files in {raw_dir}"
         if xml_path is not None:
             catalog = XMLStationChannelCatalog(xml_path)
         elif os.path.isfile(os.path.join(raw_dir, STATION_FILE)):
             catalog = CSVChannelCatalog(raw_dir)
         else:
             raise ValueError(f"Either an --xml_path argument or a {STATION_FILE} must be provided")
 
-        return SCEDCS3DataStore(raw_dir, catalog, get_channel_filter(sta_list))
+        date_range = get_date_range(args)
+        return SCEDCS3DataStore(raw_dir, catalog, get_channel_filter(stations), date_range)
 
 
 def main(args: typing.Any):
     raw_dir = args.raw_data_path
 
-    def get_raw_store():
-        stations = args.stations if "stations" in args else []
-        xml_path = args.xml_path if "xml_path" in args else None
-        return create_raw_store(raw_dir, stations, xml_path)
-
     def run_cross_correlation():
         ccf_dir = args.ccf_path
         fft_params = initialize_fft_params(raw_dir)
         fft_params.freq_norm = args.freq_norm
         cc_store = ASDFCCStore(ccf_dir)
-        raw_store = get_raw_store()
+        raw_store = create_raw_store(args)
         cross_correlate(raw_store, fft_params, cc_store)
 
     def run_download():
         params = ConfigParameters()
         params.start_date = args.start
         params.end_date = args.end
         params.inc_hours = args.inc_hours
         download(args.raw_data_path, args.channels, args.stations, params)
 
     if args.step == Step.DOWNLOAD:
         run_download()
     if args.step == Step.CROSS_CORRELATE:
         run_cross_correlation()
     if args.step == Step.STACK:
-        raw_store = get_raw_store()
+        raw_store = create_raw_store(args)
         stack(raw_store.get_station_list(), args.ccf_path, args.stack_path, args.method)
     if args.step == Step.ALL:
         run_download()
         run_cross_correlation()
-        raw_store = get_raw_store()
+        raw_store = create_raw_store(args)
         stack(raw_store.get_station_list(), args.ccf_path, args.stack_path, args.method)
 
 
-def add_download_args(down_parser: argparse.ArgumentParser):
-    down_parser.add_argument(
+def add_date_args(parser, required):
+    parser.add_argument(
         "--start",
         type=valid_date,
-        required=True,
+        required=required,
         help="Start date in the format: " + DATE_FORMAT_HELP,
-        default=default_start_date,
     )
-    down_parser.add_argument(
+    parser.add_argument(
         "--end",
         type=valid_date,
-        required=True,
+        required=required,
         help="End date in the format: " + DATE_FORMAT_HELP,
-        default=default_end_date,
     )
+
+
+def add_download_args(down_parser: argparse.ArgumentParser):
     down_parser.add_argument(
         "--channels",
         type=lambda s: s.split(","),
         help="Comma separated list of channels",
         default="BHE,BHN,BHZ",
     )
     down_parser.add_argument("--inc_hours", type=int, default=24, help="Time increment size (hrs)")
@@ -195,18 +201,22 @@
         config_fn(parser)
 
 
 def main_cli():
     parser = argparse.ArgumentParser()
     subparsers = parser.add_subparsers(dest="step", required=True)
     make_step_parser(
-        subparsers, Step.DOWNLOAD, [lambda p: add_paths(p, ["raw_data"]), add_download_args, add_stations_arg]
+        subparsers,
+        Step.DOWNLOAD,
+        [lambda p: add_paths(p, ["raw_data"]), add_download_args, add_stations_arg, lambda p: add_date_args(p, True)],
     )
     make_step_parser(
-        subparsers, Step.CROSS_CORRELATE, [lambda p: add_paths(p, ["raw_data", "ccf"]), add_cc_args, add_stations_arg]
+        subparsers,
+        Step.CROSS_CORRELATE,
+        [lambda p: add_paths(p, ["raw_data", "ccf"]), add_cc_args, add_stations_arg, lambda p: add_date_args(p, False)],
     )
     make_step_parser(subparsers, Step.STACK, [lambda p: add_paths(p, ["raw_data", "stack", "ccf"]), add_stack_args])
     make_step_parser(
         subparsers,
         Step.ALL,
         [
             lambda p: add_paths(p, ["raw_data", "ccf", "stack"]),
```

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/noise_module.py` & `noisepy_seis-0.8.2/src/noisepy/seis/noise_module.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/plotting_modules.py` & `noisepy_seis-0.8.2/src/noisepy/seis/plotting_modules.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/scedc_s3store.py` & `noisepy_seis-0.8.2/src/noisepy/seis/scedc_s3store.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,37 +36,57 @@
     """
 
     # TODO: Support reading directly from the S3 bucket
 
     # for checking the filename has the form: CIGMR__LHN___2022002.ms
     file_re = re.compile(r".*[0-9]{7}\.ms$", re.IGNORECASE)
 
-    def __init__(self, path: str, chan_catalog: ChannelCatalog, channel_filter: Callable[[Channel], bool] = None):
+    def __init__(
+        self,
+        path: str,
+        chan_catalog: ChannelCatalog,
+        ch_filter: Callable[[Channel], bool] = None,
+        date_range: DateTimeRange = None,
+    ):
         """
         Parameters:
             path: path to look for ms files. Can be a local file directory or an s3://... url path
             chan_catalog: ChannelCatalog to retrieve inventory information for the channels
             channel_filter: Function to decide whether a channel should be used or not,
                             if None, all channels are used
         """
         super().__init__()
         self.fs = get_filesystem(path)
-        self.path = path
         self.channel_catalog = chan_catalog
-        if channel_filter is None:
-            channel_filter = lambda s: True  # noqa: E731
-
-        msfiles = [f for f in self.fs.glob(fs_join(path, "*.ms")) if self.file_re.match(f) is not None]
-        # store a dict of {timerange: list of channels}
+        self.path = path
+        self.paths = {}
+        # to store a dict of {timerange: list of channels}
         self.channels = {}
+        if ch_filter is None:
+            ch_filter = lambda s: True  # noqa: E731
+
+        if date_range is None:
+            self._load_channels(self.path, ch_filter)
+        else:
+            dt = date_range.end_datetime - date_range.start_datetime
+            for d in range(0, dt.days):
+                date = date_range.start_datetime + timedelta(days=d)
+                date_path = str(date.year) + "/" + str(date.year) + "_" + str(date.timetuple().tm_yday).zfill(3) + "/"
+                full_path = fs_join(self.path, date_path)
+                self._load_channels(full_path, ch_filter)
+
+    def _load_channels(self, full_path: str, ch_filter: Callable[[Channel], bool]):
+        msfiles = [f for f in self.fs.glob(fs_join(full_path, "*.ms")) if self.file_re.match(f) is not None]
+        logger.info(f"Loading {len(msfiles)} files from {full_path}")
         timespans = []
         for f in msfiles:
             timespan = SCEDCS3DataStore._parse_timespan(f)
+            self.paths[timespan.start_datetime] = full_path
             channel = SCEDCS3DataStore._parse_channel(os.path.basename(f))
-            if not channel_filter(channel):
+            if not ch_filter(channel):
                 continue
             key = str(timespan)  # DataTimeFrame is not hashable
             if key not in self.channels:
                 timespans.append(timespan)
                 self.channels[key] = [channel]
             else:
                 self.channels[key].append(channel)
@@ -83,15 +103,17 @@
 
     def read_data(self, timespan: DateTimeRange, chan: Channel) -> ChannelData:
         # reconstruct the file name from the channel parameters
         chan_str = (
             f"{chan.station.network}{chan.station.name.ljust(5, '_')}{chan.type.name}"
             f"{chan.station.location.ljust(3, '_')}"
         )
-        filename = fs_join(self.path, f"{chan_str}{timespan.start_datetime.strftime('%Y%j')}.ms")
+        filename = fs_join(
+            self.paths[timespan.start_datetime], f"{chan_str}{timespan.start_datetime.strftime('%Y%j')}.ms"
+        )
         if not self.fs.exists(filename):
             logger.warning(f"Could not find file {filename}")
             return ChannelData.empty()
 
         with self.fs.open(filename) as f:
             stream = obspy.read(f)
         return ChannelData(stream)
```

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/stores.py` & `noisepy_seis-0.8.2/src/noisepy/seis/stores.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/utils.py` & `noisepy_seis-0.8.2/src/noisepy/seis/utils.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/application_modules/comp_stacking.py` & `noisepy_seis-0.8.2/src/noisepy/seis/application_modules/comp_stacking.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/application_modules/dispersion_analysis.py` & `noisepy_seis-0.8.2/src/noisepy/seis/application_modules/dispersion_analysis.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/application_modules/measure_dvv.py` & `noisepy_seis-0.8.2/src/noisepy/seis/application_modules/measure_dvv.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/src/noisepy/seis/application_modules/write_sac.py` & `noisepy_seis-0.8.2/src/noisepy/seis/application_modules/write_sac.py`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/.gitignore` & `noisepy_seis-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/LICENSE` & `noisepy_seis-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/README.md` & `noisepy_seis-0.8.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -72,32 +72,37 @@
 
 
 This tutorial presents one simple example of how NoisePy might work! We strongly encourage you to download the NoisePy package and play it on your own! If you have any  comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
 
 Chengxin Jiang (chengxinjiang@gmail.com)
 Marine Denolle (mdenolle@uw.edu).
 
+## Taxonomy
+Taxonomy of the NoisePy variables.
+
+* ``station`` refers to the site that has the seismic instruments that records ground shaking.
+* `` channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
+* ``ista`` is the index name for looping over stations
+
+* ``cc_len`` correlation length, basic window length in seconds
+* ``step`` is the window that get skipped when sliding windows in seconds
+* ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
+* ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
+* ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
+* ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
+
+
+# Acknowledgements
 ## Use this reference when publishing on your work with noisepy
 
 Main code:
 * Jiang, C. and Denolle, M. [NoisePy: a new high-performance python tool for seismic ambient noise seismology.](https://doi.org/10.1785/0220190364) _Seismological Research Letter_ 91, no. 3 (2020): 1853–1866. https://doi.org/10.1785/0220190364
 
 Algorithms used:
 * (data pre-processing) Seats, K. J., Jesse F. L., and German A. P. [Improved ambient noise correlation functions using Welch′ s method.](https://doi.org/10.1111/j.1365-246X.2011.05263.x) _Geophysical Journal International_ 188, no. 2 (2012): 513-523. https://doi.org/10.1111/j.1365-246X.2011.05263.x
 
 * (dv/v in wavelet domain) Yuan, C., Bryan, J. T., and Denolle, M. [Numerical comparison of time-, frequency- and wavelet-domain methods for coda wave interferometry.](https://doi.org/10.1093/gji/ggab140) _Geophysical Journal International_ 226, no. 2 (2021): 828-846. https://doi.org/10.1093/gji/ggab140
 
 * (optimal stacking) Yang X, Bryan J, Okubo K, Jiang C, Clements T, Denolle MA. [Optimal stacking of noise cross-correlation functions/](https://doi.org/10.1093/gji/ggac410) _Geophysical Journal International_. 2023 Mar;232(3):1600-18. https://doi.org/10.1093/gji/ggac410
 
-### Some taxonomy of the NoisePy variables.
-
-
-* ``station`` refers to the site that has the seismic instruments that records ground shaking.
-* `` channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
-* ``ista`` is the index name for looping over stations
 
-* ``cc_len`` correlation length, basic window length in seconds
-* ``step`` is the window that get skipped when sliding windows in seconds
-* ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
-* ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
-* ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
-* ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
+This research received software engineering support from the University of Washington’s Scientific Software Engineering Center ([SSEC](https://escience.washington.edu/software-engineering/ssec/)) supported by Schmidt Futures, as part of the Virtual Institute for Scientific Software (VISS). We would like to acknowledge [Carlos Garcia Jurado Suarez](https://github.com/carlosgjs) and [Nicholas Rich](https://github.com/nrich20) for their collaboration and contributions to the software.
```

### Comparing `noisepy_seis-0.8.1/pyproject.toml` & `noisepy_seis-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `noisepy_seis-0.8.1/PKG-INFO` & `noisepy_seis-0.8.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noisepy-seis
-Version: 0.8.1
+Version: 0.8.2
 Summary: A High-performance Computing Python Package for Ambient Noise Analysis
 Project-URL: Homepage, https://github.com/mdenolle/NoisePy
 Author-email: Marine Denolle <mdenolle@uw.edu>, Chengxin Jiang <chengxin_jiang@fas.harvard.edu>
 License: MIT License
         
         Copyright (c) 2019 Marine Denolle & Chengxin Jiang
         
@@ -124,32 +124,37 @@
 
 
 This tutorial presents one simple example of how NoisePy might work! We strongly encourage you to download the NoisePy package and play it on your own! If you have any  comments and/or suggestions during running the codes, please do not hesitate to contact us through email or open an issue in this github page!
 
 Chengxin Jiang (chengxinjiang@gmail.com)
 Marine Denolle (mdenolle@uw.edu).
 
+## Taxonomy
+Taxonomy of the NoisePy variables.
+
+* ``station`` refers to the site that has the seismic instruments that records ground shaking.
+* `` channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
+* ``ista`` is the index name for looping over stations
+
+* ``cc_len`` correlation length, basic window length in seconds
+* ``step`` is the window that get skipped when sliding windows in seconds
+* ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
+* ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
+* ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
+* ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
+
+
+# Acknowledgements
 ## Use this reference when publishing on your work with noisepy
 
 Main code:
 * Jiang, C. and Denolle, M. [NoisePy: a new high-performance python tool for seismic ambient noise seismology.](https://doi.org/10.1785/0220190364) _Seismological Research Letter_ 91, no. 3 (2020): 1853–1866. https://doi.org/10.1785/0220190364
 
 Algorithms used:
 * (data pre-processing) Seats, K. J., Jesse F. L., and German A. P. [Improved ambient noise correlation functions using Welch′ s method.](https://doi.org/10.1111/j.1365-246X.2011.05263.x) _Geophysical Journal International_ 188, no. 2 (2012): 513-523. https://doi.org/10.1111/j.1365-246X.2011.05263.x
 
 * (dv/v in wavelet domain) Yuan, C., Bryan, J. T., and Denolle, M. [Numerical comparison of time-, frequency- and wavelet-domain methods for coda wave interferometry.](https://doi.org/10.1093/gji/ggab140) _Geophysical Journal International_ 226, no. 2 (2021): 828-846. https://doi.org/10.1093/gji/ggab140
 
 * (optimal stacking) Yang X, Bryan J, Okubo K, Jiang C, Clements T, Denolle MA. [Optimal stacking of noise cross-correlation functions/](https://doi.org/10.1093/gji/ggac410) _Geophysical Journal International_. 2023 Mar;232(3):1600-18. https://doi.org/10.1093/gji/ggac410
 
-### Some taxonomy of the NoisePy variables.
-
-
-* ``station`` refers to the site that has the seismic instruments that records ground shaking.
-* `` channel`` refers to the direction of ground motion investigated for 3 component seismometers. For DAS project, it may refers to the single channel sensors.
-* ``ista`` is the index name for looping over stations
 
-* ``cc_len`` correlation length, basic window length in seconds
-* ``step`` is the window that get skipped when sliding windows in seconds
-* ``smooth_N`` number of points for smoothing the  time or frequency domain discrete arrays.
-* ``maxlag`` maximum length in seconds saved in files in each side of the correlation (save on storage)
-* ``substack,substack_len`` boolean, window length over which to substack the correlation (to save storage or do monitoring), it has to be a multiple of ``cc_len``.
-* ``time_chunk, nchunk`` refers to the time unit that defined a single job. for instace, ``cc_len`` is the correlation length (e.g., 1 hour, 30 min), the overall duration of the experiment is the total length (1 month, 1 year, ...). The time chunk could be 1 day: the code would loop through each cc_len window in a for loop. But each day will be sent as a thread.
+This research received software engineering support from the University of Washington’s Scientific Software Engineering Center ([SSEC](https://escience.washington.edu/software-engineering/ssec/)) supported by Schmidt Futures, as part of the Virtual Institute for Scientific Software (VISS). We would like to acknowledge [Carlos Garcia Jurado Suarez](https://github.com/carlosgjs) and [Nicholas Rich](https://github.com/nrich20) for their collaboration and contributions to the software.
```

