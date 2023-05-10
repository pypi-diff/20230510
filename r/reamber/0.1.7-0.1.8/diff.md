# Comparing `tmp/reamber-0.1.7.tar.gz` & `tmp/reamber-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reamber-0.1.7.tar", last modified: Tue Aug  9 13:31:26 2022, max compression
+gzip compressed data, was "reamber-0.1.8.tar", max compression
```

## Comparing `reamber-0.1.7.tar` & `reamber-0.1.8.tar`

### file list

```diff
@@ -1,399 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.741988 reamber-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-08-09 13:31:14.000000 reamber-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-08-09 13:31:26.741988 reamber-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1560 2022-08-09 13:31:14.000000 reamber-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.709988 reamber-0.1.7/reamber/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.709988 reamber-0.1.7/reamber/algorithms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.713988 reamber-0.1.7/reamber/algorithms/convert/
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/BMSToOsu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/BMSToQua.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/BMSToSM.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/ConvertBase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/O2JToBMS.py
--rw-r--r--   0 runner    (1001) docker     (121)     1237 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/O2JToOsu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1319 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/O2JToQua.py
--rw-r--r--   0 runner    (1001) docker     (121)     2460 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/O2JToSM.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/OsuToBMS.py
--rw-r--r--   0 runner    (1001) docker     (121)     1804 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/OsuToQua.py
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/OsuToSM.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/QuaToBMS.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/QuaToOsu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/QuaToSM.py
--rw-r--r--   0 runner    (1001) docker     (121)     1355 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/SMToBMS.py
--rw-r--r--   0 runner    (1001) docker     (121)     1561 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/SMToOsu.py
--rw-r--r--   0 runner    (1001) docker     (121)     1956 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/SMToQua.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/convert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.713988 reamber-0.1.7/reamber/algorithms/generate/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/generate/full_ln.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.713988 reamber-0.1.7/reamber/algorithms/osu/
--rw-r--r--   0 runner    (1001) docker     (121)     5417 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/osu/OsuReplayError.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/osu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5917 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/osu/hitsound_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.713988 reamber-0.1.7/reamber/algorithms/pattern/
--rw-r--r--   0 runner    (1001) docker     (121)     5746 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/pattern/Pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/pattern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.713988 reamber-0.1.7/reamber/algorithms/pattern/combos/
--rw-r--r--   0 runner    (1001) docker     (121)     2376 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/pattern/combos/PtnCombo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2517 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/pattern/combos/_PtnCChordStream.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/pattern/combos/_PtnCJack.py
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/pattern/combos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.713988 reamber-0.1.7/reamber/algorithms/pattern/filters/
--rw-r--r--   0 runner    (1001) docker     (121)    10652 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/pattern/filters/PtnFilter.py
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/pattern/filters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.713988 reamber-0.1.7/reamber/algorithms/playField/
--rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/PlayField.py
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.713988 reamber-0.1.7/reamber/algorithms/playField/parts/
--rw-r--r--   0 runner    (1001) docker     (121)     1918 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawBeatLines.py
--rw-r--r--   0 runner    (1001) docker     (121)     1352 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawBpm.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawColumnLines.py
--rw-r--r--   0 runner    (1001) docker     (121)     6809 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawLines.py
--rw-r--r--   0 runner    (1001) docker     (121)     7896 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawNotes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1462 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawOffsets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1545 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawSv.py
--rw-r--r--   0 runner    (1001) docker     (121)      319 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawable.py
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/playField/parts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.713988 reamber-0.1.7/reamber/algorithms/timing/
--rw-r--r--   0 runner    (1001) docker     (121)     5668 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/TimingMap.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.717988 reamber-0.1.7/reamber/algorithms/timing/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      449 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/BpmChangeBase.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/BpmChangeOffset.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/BpmChangeSnap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2185 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/Snapper.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/bpm_changes_offset_to_snap.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/find_lcm.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/from_bpm_changes_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1651 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/from_bpm_changes_snap.py
--rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/reseat_bpm_changes_snap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2779 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/algorithms/timing/utils/snap.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.717988 reamber-0.1.7/reamber/base/
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Bpm.py
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Bpm.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      365 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Hit.py
--rw-r--r--   0 runner    (1001) docker     (121)      120 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Hit.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1680 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Hold.py
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Hold.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10525 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Map.py
--rw-r--r--   0 runner    (1001) docker     (121)     3215 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Map.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5946 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/MapSet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/MapSet.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Note.py
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Note.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6040 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Property.py
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/RAConst.py
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Series.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Timed.py
--rw-r--r--   0 runner    (1001) docker     (121)      559 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/Timed.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      493 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.717988 reamber-0.1.7/reamber/base/lists/
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/BpmList.py
--rw-r--r--   0 runner    (1001) docker     (121)      739 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/BpmList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12540 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/TimedList.py
--rw-r--r--   0 runner    (1001) docker     (121)     3251 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/TimedList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.717988 reamber-0.1.7/reamber/base/lists/notes/
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/notes/HitList.py
--rw-r--r--   0 runner    (1001) docker     (121)      619 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/notes/HitList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     3903 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/notes/HoldList.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/notes/HoldList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/notes/NoteList.py
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/notes/NoteList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/base/lists/notes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.721988 reamber-0.1.7/reamber/bms/
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSBpm.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSBpm.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1643 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSChannel.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSHit.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSHit.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      508 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSHold.py
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSHold.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    19150 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSMap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1919 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSMap.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSMapMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)      570 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSMapMeta.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSNoteMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/BMSNoteMeta.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.721988 reamber-0.1.7/reamber/bms/lists/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/BMSBpmList.py
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/BMSBpmList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/BMSNotePkg.py
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.721988 reamber-0.1.7/reamber/bms/lists/notes/
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/notes/BMSHitList.py
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/notes/BMSHitList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      327 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/notes/BMSHoldList.py
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/notes/BMSHoldList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      280 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/notes/BMSNoteList.py
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/notes/BMSNoteList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/bms/lists/notes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.721988 reamber-0.1.7/reamber/o2jam/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JBpm.py
--rw-r--r--   0 runner    (1001) docker     (121)     9242 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JEventPackage.py
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JHit.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JHit.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JHold.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JHold.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5715 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JMap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1534 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JMap.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JMapSet.py
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JMapSet.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6578 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JMapSetMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JNoteMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)      224 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/O2JNoteMeta.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      509 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.721988 reamber-0.1.7/reamber/o2jam/lists/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/O2JBpmList.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/O2JBpmList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.721988 reamber-0.1.7/reamber/o2jam/lists/notes/
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/notes/O2JHitList.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/notes/O2JHitList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/notes/O2JHoldList.py
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/notes/O2JHoldList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/notes/O2JNoteList.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/notes/O2JNoteList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/o2jam/lists/notes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.725988 reamber-0.1.7/reamber/osu/
--rw-r--r--   0 runner    (1001) docker     (121)     2386 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuBpm.py
--rw-r--r--   0 runner    (1001) docker     (121)      970 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuBpm.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuHit.py
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuHit.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2389 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuHold.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuHold.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4974 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuMap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2650 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuMap.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     7577 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuMapMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)     1884 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuNoteMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuNoteMeta.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuSample.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuSample.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1138 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuSampleSet.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuSv.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuSv.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      758 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/OsuTimingPointMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.725988 reamber-0.1.7/reamber/osu/lists/
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/OsuBpmList.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/OsuBpmList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      598 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/OsuSampleList.py
--rw-r--r--   0 runner    (1001) docker     (121)      575 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/OsuSampleList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/OsuSvList.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/OsuSvList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.725988 reamber-0.1.7/reamber/osu/lists/notes/
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/notes/OsuHitList.py
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/notes/OsuHitList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/notes/OsuHoldList.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/notes/OsuHoldList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/notes/OsuNoteList.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/notes/OsuNoteList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/osu/lists/notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.725988 reamber-0.1.7/reamber/quaver/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaBpm.py
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaBpm.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      918 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaHit.py
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaHit.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaHold.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaHold.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4018 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaMap.py
--rw-r--r--   0 runner    (1001) docker     (121)     1729 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaMap.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaMapMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaNoteMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaNoteMeta.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaSv.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/QuaSv.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      407 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.729988 reamber-0.1.7/reamber/quaver/lists/
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/QuaBpmList.py
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/QuaBpmList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/QuaSvList.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/QuaSvList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/QuaTimedList.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.729988 reamber-0.1.7/reamber/quaver/lists/notes/
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/notes/QuaHitList.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/notes/QuaHitList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/notes/QuaHoldList.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/notes/QuaHoldList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/notes/QuaNoteList.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/notes/QuaNoteList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/quaver/lists/notes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.729988 reamber-0.1.7/reamber/sm/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMBpm.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMBpm.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMConst.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMFake.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMHit.py
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMHold.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMKeySound.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMLift.py
--rw-r--r--   0 runner    (1001) docker     (121)    13557 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMMap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2216 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMMap.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6709 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMMapMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)     2298 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMMapSet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMMapSet.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6610 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMMapSetMeta.py
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMMine.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMRoll.py
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMStop.py
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/SMStop.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.729988 reamber-0.1.7/reamber/sm/lists/
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/SMBpmList.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/SMBpmList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/SMStopList.py
--rw-r--r--   0 runner    (1001) docker     (121)      289 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/SMStopList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/reamber/sm/lists/notes/
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMFakeList.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMFakeList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMHitList.py
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMHitList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMHoldList.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMHoldList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMKeySoundList.py
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMKeySoundList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMLiftList.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMLiftList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMMineList.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMMineList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMNoteList.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMNoteList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      316 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMRollList.py
--rw-r--r--   0 runner    (1001) docker     (121)      251 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/SMRollList.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-08-09 13:31:14.000000 reamber-0.1.7/reamber/sm/lists/notes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.709988 reamber-0.1.7/reamber.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-08-09 13:31:26.000000 reamber-0.1.7/reamber.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11994 2022-08-09 13:31:26.000000 reamber-0.1.7/reamber.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 13:31:26.000000 reamber-0.1.7/reamber.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 13:31:26.000000 reamber-0.1.7/reamber.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-08-09 13:31:26.000000 reamber-0.1.7/reamber.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-09 13:31:26.000000 reamber-0.1.7/reamber.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 13:31:26.741988 reamber-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1242 2022-08-09 13:31:15.000000 reamber-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/algorithm_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/algorithm_tests/convert/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/convert/test_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/algorithm_tests/generate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1604 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/generate/test_full_ln.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/algorithm_tests/osu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/osu/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/algorithm_tests/osu/hitsound_copy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/osu/hitsound_copy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/osu/hitsound_copy/test_hitsound_copy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/algorithm_tests/osu/replay/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/osu/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/osu/replay/test_osu_replay_error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/algorithm_tests/pattern/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1041 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/algorithm_tests/pattern/options/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/options/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1531 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/options/test_chord_filter_option.py
--rw-r--r--   0 runner    (1001) docker     (121)     1644 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/options/test_combo_filter_option.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/options/test_type_filter_option.py
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/test_combo.py
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/test_filter_op.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/test_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/test_pattern.py
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/pattern/test_pattern_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/algorithm_tests/playField/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/playField/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/algorithm_tests/playField/test_playfield.py
--rw-r--r--   0 runner    (1001) docker     (121)     1617 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.733988 reamber-0.1.7/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.737988 reamber-0.1.7/tests/unit_tests/base/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1537 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.737988 reamber-0.1.7/tests/unit_tests/base/inheritance/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/inheritance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      753 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/inheritance/test_map_inherit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/inheritance/test_timed_inherit.py
--rw-r--r--   0 runner    (1001) docker     (121)     1447 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/inheritance/test_timed_list_inherit.py
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_bpm_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_hold.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_hold_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_map_set.py
--rw-r--r--   0 runner    (1001) docker     (121)      935 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_map_stacking.py
--rw-r--r--   0 runner    (1001) docker     (121)      787 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_note_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_series.py
--rw-r--r--   0 runner    (1001) docker     (121)      332 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_timed.py
--rw-r--r--   0 runner    (1001) docker     (121)     2803 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/base/test_timed_list.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.737988 reamber-0.1.7/tests/unit_tests/bms/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.737988 reamber-0.1.7/tests/unit_tests/bms/maps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/maps/test_cold_breath.py
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/maps/test_nhelv.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/maps/test_searoad.py
--rw-r--r--   0 runner    (1001) docker     (121)      500 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/maps/test_super_izanagi.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/maps/test_take.py
--rw-r--r--   0 runner    (1001) docker     (121)      248 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/test_bpm_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/test_hit_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/test_hold_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/bms/test_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.737988 reamber-0.1.7/tests/unit_tests/o2jam/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/o2jam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/o2jam/test_hit_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      325 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/o2jam/test_hold_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2092 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/o2jam/test_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.737988 reamber-0.1.7/tests/unit_tests/osu/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/osu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3453 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/osu/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/osu/test_bpm_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/osu/test_hit_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      915 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/osu/test_hold_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     2558 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/osu/test_map.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/osu/test_sv_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1022 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/osu/test_x_axis_column_conv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.741988 reamber-0.1.7/tests/unit_tests/qua/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/qua/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/qua/test_bpm.py
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/qua/test_bpm_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/qua/test_hit.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/qua/test_hit_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/qua/test_hold.py
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/qua/test_hold_list.py
--rw-r--r--   0 runner    (1001) docker     (121)     1402 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/qua/test_map.py
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/qua/test_sv.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.741988 reamber-0.1.7/tests/unit_tests/sm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.741988 reamber-0.1.7/tests/unit_tests/sm/maps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/maps/test_caravan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/maps/test_escapes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/maps/test_gravity.py
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/maps/test_icfitu.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.741988 reamber-0.1.7/tests/unit_tests/sm/profile/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/profile/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/test_bpm_list.py
--rw-r--r--   0 runner    (1001) docker     (121)      832 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/sm/test_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.741988 reamber-0.1.7/tests/unit_tests/timing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:26.741988 reamber-0.1.7/tests/unit_tests/timing/cases/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/cases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/cases/case.py
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/cases/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/test_b2b_conversion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/test_beat_snap_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/test_from_offset.py
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/test_from_snap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/test_reseat_cases.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-08-09 13:31:15.000000 reamber-0.1.7/tests/unit_tests/timing/test_timing_reseat.py
+-rw-r--r--   0        0        0     1085 2023-04-18 09:51:01.880437 reamber-0.1.8/LICENSE
+-rw-r--r--   0        0        0      541 2023-05-10 08:28:31.758065 reamber-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1658 2023-05-10 08:28:31.732649 reamber-0.1.8/README.md
+-rw-r--r--   0        0        0      142 2023-05-04 05:46:31.859974 reamber-0.1.8/reamber/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:51:01.988949 reamber-0.1.8/reamber/algorithms/__init__.py
+-rw-r--r--   0        0        0       97 2023-05-10 08:28:31.758065 reamber-0.1.8/reamber/algorithms/analysis/__init__.py
+-rw-r--r--   0        0        0     2728 2023-05-10 08:28:31.759071 reamber-0.1.8/reamber/algorithms/analysis/scroll_speed.py
+-rw-r--r--   0        0        0     1197 2023-04-18 09:51:01.993950 reamber-0.1.8/reamber/algorithms/convert/__init__.py
+-rw-r--r--   0        0        0     1392 2023-04-18 09:51:01.989950 reamber-0.1.8/reamber/algorithms/convert/BMSToOsu.py
+-rw-r--r--   0        0        0     1593 2023-04-18 09:51:01.989950 reamber-0.1.8/reamber/algorithms/convert/BMSToQua.py
+-rw-r--r--   0        0        0     1335 2023-04-18 09:51:01.989950 reamber-0.1.8/reamber/algorithms/convert/BMSToSM.py
+-rw-r--r--   0        0        0      759 2023-04-18 09:51:01.989950 reamber-0.1.8/reamber/algorithms/convert/ConvertBase.py
+-rw-r--r--   0        0        0     1712 2023-04-18 09:51:01.990950 reamber-0.1.8/reamber/algorithms/convert/O2JToBMS.py
+-rw-r--r--   0        0        0     1274 2023-04-18 09:51:01.990950 reamber-0.1.8/reamber/algorithms/convert/O2JToOsu.py
+-rw-r--r--   0        0        0     1358 2023-04-18 09:51:01.990950 reamber-0.1.8/reamber/algorithms/convert/O2JToQua.py
+-rw-r--r--   0        0        0     2542 2023-04-18 09:51:01.991950 reamber-0.1.8/reamber/algorithms/convert/O2JToSM.py
+-rw-r--r--   0        0        0     1467 2023-04-18 09:51:01.991950 reamber-0.1.8/reamber/algorithms/convert/OsuToBMS.py
+-rw-r--r--   0        0        0     1858 2023-04-18 09:51:01.991950 reamber-0.1.8/reamber/algorithms/convert/OsuToQua.py
+-rw-r--r--   0        0        0     1836 2023-04-18 09:51:01.991950 reamber-0.1.8/reamber/algorithms/convert/OsuToSM.py
+-rw-r--r--   0        0        0     1494 2023-04-18 09:51:01.992950 reamber-0.1.8/reamber/algorithms/convert/QuaToBMS.py
+-rw-r--r--   0        0        0     1609 2023-04-18 09:51:01.992950 reamber-0.1.8/reamber/algorithms/convert/QuaToOsu.py
+-rw-r--r--   0        0        0     1606 2023-04-18 09:51:01.992950 reamber-0.1.8/reamber/algorithms/convert/QuaToSM.py
+-rw-r--r--   0        0        0     1394 2023-04-18 09:51:01.992950 reamber-0.1.8/reamber/algorithms/convert/SMToBMS.py
+-rw-r--r--   0        0        0     1606 2023-04-18 09:51:01.993950 reamber-0.1.8/reamber/algorithms/convert/SMToOsu.py
+-rw-r--r--   0        0        0     2005 2023-04-18 09:51:01.993950 reamber-0.1.8/reamber/algorithms/convert/SMToQua.py
+-rw-r--r--   0        0        0      165 2023-05-10 08:28:31.759071 reamber-0.1.8/reamber/algorithms/generate/__init__.py
+-rw-r--r--   0        0        0     1725 2023-04-18 09:51:01.994950 reamber-0.1.8/reamber/algorithms/generate/full_ln.py
+-rw-r--r--   0        0        0      102 2023-04-18 09:51:01.993950 reamber-0.1.8/reamber/algorithms/generate/README.md
+-rw-r--r--   0        0        0     1901 2023-05-10 08:28:31.759071 reamber-0.1.8/reamber/algorithms/generate/sv_normalize.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:51:01.995950 reamber-0.1.8/reamber/algorithms/osu/__init__.py
+-rw-r--r--   0        0        0     5692 2023-05-10 08:28:31.760069 reamber-0.1.8/reamber/algorithms/osu/hitsound_copy.py
+-rw-r--r--   0        0        0     8299 2023-05-04 05:45:01.950686 reamber-0.1.8/reamber/algorithms/osu/parse_replay.py
+-rw-r--r--   0        0        0       81 2023-04-18 09:51:01.995950 reamber-0.1.8/reamber/algorithms/pattern/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-18 09:51:01.997949 reamber-0.1.8/reamber/algorithms/pattern/combos/__init__.py
+-rw-r--r--   0        0        0     2589 2023-04-18 09:51:01.996950 reamber-0.1.8/reamber/algorithms/pattern/combos/_PtnCChordStream.py
+-rw-r--r--   0        0        0     1596 2023-04-18 09:51:01.996950 reamber-0.1.8/reamber/algorithms/pattern/combos/_PtnCJack.py
+-rw-r--r--   0        0        0     2442 2023-04-18 09:51:01.996950 reamber-0.1.8/reamber/algorithms/pattern/combos/PtnCombo.py
+-rw-r--r--   0        0        0      178 2023-04-18 09:51:01.997949 reamber-0.1.8/reamber/algorithms/pattern/filters/__init__.py
+-rw-r--r--   0        0        0    10966 2023-04-18 09:51:01.997949 reamber-0.1.8/reamber/algorithms/pattern/filters/PtnFilter.py
+-rw-r--r--   0        0        0     5920 2023-04-18 09:51:01.995950 reamber-0.1.8/reamber/algorithms/pattern/Pattern.py
+-rw-r--r--   0        0        0       89 2023-04-18 09:51:01.998950 reamber-0.1.8/reamber/algorithms/playField/__init__.py
+-rw-r--r--   0        0        0      681 2023-04-18 09:51:02.001950 reamber-0.1.8/reamber/algorithms/playField/parts/__init__.py
+-rw-r--r--   0        0        0      329 2023-04-18 09:51:02.000950 reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawable.py
+-rw-r--r--   0        0        0     1973 2023-04-18 09:51:01.998950 reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawBeatLines.py
+-rw-r--r--   0        0        0     1395 2023-04-18 09:51:01.999950 reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawBpm.py
+-rw-r--r--   0        0        0      892 2023-04-18 09:51:01.999950 reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawColumnLines.py
+-rw-r--r--   0        0        0     6984 2023-04-18 09:51:01.999950 reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawLines.py
+-rw-r--r--   0        0        0     8084 2023-04-18 09:51:02.000950 reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawNotes.py
+-rw-r--r--   0        0        0     1509 2023-04-18 09:51:02.000950 reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawOffsets.py
+-rw-r--r--   0        0        0     1592 2023-04-18 09:51:02.000950 reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawSv.py
+-rw-r--r--   0        0        0     4727 2023-04-18 09:51:01.998950 reamber-0.1.8/reamber/algorithms/playField/PlayField.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:51:02.001950 reamber-0.1.8/reamber/algorithms/timing/__init__.py
+-rw-r--r--   0        0        0     5826 2023-04-18 09:51:02.001950 reamber-0.1.8/reamber/algorithms/timing/TimingMap.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:51:02.002949 reamber-0.1.8/reamber/algorithms/timing/utils/__init__.py
+-rw-r--r--   0        0        0     1425 2023-04-18 09:51:02.003949 reamber-0.1.8/reamber/algorithms/timing/utils/bpm_changes_offset_to_snap.py
+-rw-r--r--   0        0        0      470 2023-04-18 09:51:02.001950 reamber-0.1.8/reamber/algorithms/timing/utils/BpmChangeBase.py
+-rw-r--r--   0        0        0      222 2023-04-18 09:51:02.002949 reamber-0.1.8/reamber/algorithms/timing/utils/BpmChangeOffset.py
+-rw-r--r--   0        0        0      524 2023-04-18 09:51:02.002949 reamber-0.1.8/reamber/algorithms/timing/utils/BpmChangeSnap.py
+-rw-r--r--   0        0        0      123 2023-04-18 09:51:02.003949 reamber-0.1.8/reamber/algorithms/timing/utils/conf.py
+-rw-r--r--   0        0        0     1118 2023-04-18 09:51:02.003949 reamber-0.1.8/reamber/algorithms/timing/utils/find_lcm.py
+-rw-r--r--   0        0        0      413 2023-04-18 09:51:02.003949 reamber-0.1.8/reamber/algorithms/timing/utils/from_bpm_changes_offset.py
+-rw-r--r--   0        0        0     1701 2023-04-18 09:51:02.004949 reamber-0.1.8/reamber/algorithms/timing/utils/from_bpm_changes_snap.py
+-rw-r--r--   0        0        0     3883 2023-04-18 09:51:02.004949 reamber-0.1.8/reamber/algorithms/timing/utils/reseat_bpm_changes_snap.py
+-rw-r--r--   0        0        0     2864 2023-04-18 09:51:02.004949 reamber-0.1.8/reamber/algorithms/timing/utils/snap.py
+-rw-r--r--   0        0        0     2258 2023-04-18 09:51:02.002949 reamber-0.1.8/reamber/algorithms/timing/utils/Snapper.py
+-rw-r--r--   0        0        0       94 2023-05-10 08:28:31.760069 reamber-0.1.8/reamber/algorithms/utils/__init__.py
+-rw-r--r--   0        0        0      929 2023-05-10 08:28:31.761070 reamber-0.1.8/reamber/algorithms/utils/dominant_bpm.py
+-rw-r--r--   0        0        0      506 2023-04-18 09:51:02.009954 reamber-0.1.8/reamber/base/__init__.py
+-rw-r--r--   0        0        0     1752 2023-04-18 09:51:02.005950 reamber-0.1.8/reamber/base/Bpm.py
+-rw-r--r--   0        0        0      530 2023-04-18 09:51:02.005950 reamber-0.1.8/reamber/base/Bpm.pyi
+-rw-r--r--   0        0        0      382 2023-04-18 09:51:02.005950 reamber-0.1.8/reamber/base/Hit.py
+-rw-r--r--   0        0        0      125 2023-04-18 09:51:02.005950 reamber-0.1.8/reamber/base/Hit.pyi
+-rw-r--r--   0        0        0     1748 2023-04-18 09:51:02.006954 reamber-0.1.8/reamber/base/Hold.py
+-rw-r--r--   0        0        0      572 2023-04-18 09:51:02.006954 reamber-0.1.8/reamber/base/Hold.pyi
+-rw-r--r--   0        0        0     2122 2023-04-18 09:51:02.011954 reamber-0.1.8/reamber/base/lists/__init__.py
+-rw-r--r--   0        0        0     3444 2023-04-18 09:51:02.009954 reamber-0.1.8/reamber/base/lists/BpmList.py
+-rw-r--r--   0        0        0      772 2023-04-18 09:51:02.010954 reamber-0.1.8/reamber/base/lists/BpmList.pyi
+-rw-r--r--   0        0        0      215 2023-04-18 09:51:02.012954 reamber-0.1.8/reamber/base/lists/notes/__init__.py
+-rw-r--r--   0        0        0      803 2023-04-18 09:51:02.011954 reamber-0.1.8/reamber/base/lists/notes/HitList.py
+-rw-r--r--   0        0        0      645 2023-04-18 09:51:02.011954 reamber-0.1.8/reamber/base/lists/notes/HitList.pyi
+-rw-r--r--   0        0        0     4021 2023-04-18 09:51:02.011954 reamber-0.1.8/reamber/base/lists/notes/HoldList.py
+-rw-r--r--   0        0        0     1177 2023-04-18 09:51:02.012954 reamber-0.1.8/reamber/base/lists/notes/HoldList.pyi
+-rw-r--r--   0        0        0      369 2023-04-18 09:51:02.012954 reamber-0.1.8/reamber/base/lists/notes/NoteList.py
+-rw-r--r--   0        0        0      423 2023-04-18 09:51:02.012954 reamber-0.1.8/reamber/base/lists/notes/NoteList.pyi
+-rw-r--r--   0        0        0    12962 2023-04-18 09:51:02.010954 reamber-0.1.8/reamber/base/lists/TimedList.py
+-rw-r--r--   0        0        0     3382 2023-04-18 09:51:02.010954 reamber-0.1.8/reamber/base/lists/TimedList.pyi
+-rw-r--r--   0        0        0    10860 2023-04-18 09:51:02.006954 reamber-0.1.8/reamber/base/Map.py
+-rw-r--r--   0        0        0     3341 2023-04-18 09:51:02.006954 reamber-0.1.8/reamber/base/Map.pyi
+-rw-r--r--   0        0        0     6142 2023-04-18 09:51:02.007954 reamber-0.1.8/reamber/base/MapSet.py
+-rw-r--r--   0        0        0     2887 2023-04-18 09:51:02.007954 reamber-0.1.8/reamber/base/MapSet.pyi
+-rw-r--r--   0        0        0      505 2023-04-18 09:51:02.007954 reamber-0.1.8/reamber/base/Note.py
+-rw-r--r--   0        0        0      276 2023-04-18 09:51:02.007954 reamber-0.1.8/reamber/base/Note.pyi
+-rw-r--r--   0        0        0     6240 2023-04-18 09:51:02.008955 reamber-0.1.8/reamber/base/Property.py
+-rw-r--r--   0        0        0     2830 2023-04-18 09:51:02.008955 reamber-0.1.8/reamber/base/RAConst.py
+-rw-r--r--   0        0        0     1372 2023-04-18 09:51:02.008955 reamber-0.1.8/reamber/base/Series.py
+-rw-r--r--   0        0        0      811 2023-04-18 09:51:02.008955 reamber-0.1.8/reamber/base/Timed.py
+-rw-r--r--   0        0        0      583 2023-04-18 09:51:02.009954 reamber-0.1.8/reamber/base/Timed.pyi
+-rw-r--r--   0        0        0      274 2023-04-18 09:51:02.016955 reamber-0.1.8/reamber/bms/__init__.py
+-rw-r--r--   0        0        0      157 2023-04-18 09:51:02.013955 reamber-0.1.8/reamber/bms/BMSBpm.py
+-rw-r--r--   0        0        0      105 2023-04-18 09:51:02.013955 reamber-0.1.8/reamber/bms/BMSBpm.pyi
+-rw-r--r--   0        0        0     1702 2023-04-18 09:51:02.013955 reamber-0.1.8/reamber/bms/BMSChannel.py
+-rw-r--r--   0        0        0      449 2023-04-18 09:51:02.014955 reamber-0.1.8/reamber/bms/BMSHit.py
+-rw-r--r--   0        0        0      266 2023-04-18 09:51:02.014955 reamber-0.1.8/reamber/bms/BMSHit.pyi
+-rw-r--r--   0        0        0      525 2023-04-18 09:51:02.014955 reamber-0.1.8/reamber/bms/BMSHold.py
+-rw-r--r--   0        0        0      283 2023-04-18 09:51:02.014955 reamber-0.1.8/reamber/bms/BMSHold.pyi
+-rw-r--r--   0        0        0    19694 2023-05-10 08:28:31.761070 reamber-0.1.8/reamber/bms/BMSMap.py
+-rw-r--r--   0        0        0     2020 2023-05-10 08:28:31.761070 reamber-0.1.8/reamber/bms/BMSMap.pyi
+-rw-r--r--   0        0        0     1043 2023-04-18 09:51:02.015954 reamber-0.1.8/reamber/bms/BMSMapMeta.py
+-rw-r--r--   0        0        0      595 2023-04-18 09:51:02.016955 reamber-0.1.8/reamber/bms/BMSMapMeta.pyi
+-rw-r--r--   0        0        0      112 2023-04-18 09:51:02.016955 reamber-0.1.8/reamber/bms/BMSNoteMeta.py
+-rw-r--r--   0        0        0      133 2023-04-18 09:51:02.016955 reamber-0.1.8/reamber/bms/BMSNoteMeta.pyi
+-rw-r--r--   0        0        0      925 2023-04-18 09:51:02.016955 reamber-0.1.8/reamber/bms/HEADER_INFO
+-rw-r--r--   0        0        0      148 2023-04-18 09:51:02.018954 reamber-0.1.8/reamber/bms/lists/__init__.py
+-rw-r--r--   0        0        0      241 2023-04-18 09:51:02.017954 reamber-0.1.8/reamber/bms/lists/BMSBpmList.py
+-rw-r--r--   0        0        0      174 2023-04-18 09:51:02.017954 reamber-0.1.8/reamber/bms/lists/BMSBpmList.pyi
+-rw-r--r--   0        0        0     1912 2023-04-18 09:51:02.017954 reamber-0.1.8/reamber/bms/lists/BMSNotePkg.py
+-rw-r--r--   0        0        0      239 2023-04-18 09:51:02.019955 reamber-0.1.8/reamber/bms/lists/notes/__init__.py
+-rw-r--r--   0        0        0      329 2023-04-18 09:51:02.018954 reamber-0.1.8/reamber/bms/lists/notes/BMSHitList.py
+-rw-r--r--   0        0        0      262 2023-04-18 09:51:02.018954 reamber-0.1.8/reamber/bms/lists/notes/BMSHitList.pyi
+-rw-r--r--   0        0        0      338 2023-04-18 09:51:02.018954 reamber-0.1.8/reamber/bms/lists/notes/BMSHoldList.py
+-rw-r--r--   0        0        0      270 2023-04-18 09:51:02.019955 reamber-0.1.8/reamber/bms/lists/notes/BMSHoldList.pyi
+-rw-r--r--   0        0        0      293 2023-04-18 09:51:02.019955 reamber-0.1.8/reamber/bms/lists/notes/BMSNoteList.py
+-rw-r--r--   0        0        0      318 2023-04-18 09:51:02.019955 reamber-0.1.8/reamber/bms/lists/notes/BMSNoteList.pyi
+-rw-r--r--   0        0        0      521 2023-04-18 09:51:02.024465 reamber-0.1.8/reamber/o2jam/__init__.py
+-rw-r--r--   0        0        0       83 2023-04-18 09:51:02.024465 reamber-0.1.8/reamber/o2jam/lists/__init__.py
+-rw-r--r--   0        0        0      245 2023-04-18 09:51:02.026466 reamber-0.1.8/reamber/o2jam/lists/notes/__init__.py
+-rw-r--r--   0        0        0      325 2023-04-18 09:51:02.025465 reamber-0.1.8/reamber/o2jam/lists/notes/O2JHitList.py
+-rw-r--r--   0        0        0      250 2023-04-18 09:51:02.025465 reamber-0.1.8/reamber/o2jam/lists/notes/O2JHitList.pyi
+-rw-r--r--   0        0        0      342 2023-04-18 09:51:02.025465 reamber-0.1.8/reamber/o2jam/lists/notes/O2JHoldList.py
+-rw-r--r--   0        0        0      265 2023-04-18 09:51:02.025465 reamber-0.1.8/reamber/o2jam/lists/notes/O2JHoldList.pyi
+-rw-r--r--   0        0        0      288 2023-04-18 09:51:02.026466 reamber-0.1.8/reamber/o2jam/lists/notes/O2JNoteList.py
+-rw-r--r--   0        0        0      187 2023-04-18 09:51:02.026466 reamber-0.1.8/reamber/o2jam/lists/notes/O2JNoteList.pyi
+-rw-r--r--   0        0        0      243 2023-04-18 09:51:02.024465 reamber-0.1.8/reamber/o2jam/lists/O2JBpmList.py
+-rw-r--r--   0        0        0      176 2023-04-18 09:51:02.024465 reamber-0.1.8/reamber/o2jam/lists/O2JBpmList.pyi
+-rw-r--r--   0        0        0       67 2023-04-18 09:51:02.019955 reamber-0.1.8/reamber/o2jam/O2JBpm.py
+-rw-r--r--   0        0        0     9520 2023-04-18 09:51:02.021460 reamber-0.1.8/reamber/o2jam/O2JEventPackage.py
+-rw-r--r--   0        0        0      474 2023-04-18 09:51:02.021460 reamber-0.1.8/reamber/o2jam/O2JHit.py
+-rw-r--r--   0        0        0      240 2023-04-18 09:51:02.021460 reamber-0.1.8/reamber/o2jam/O2JHit.pyi
+-rw-r--r--   0        0        0      539 2023-04-18 09:51:02.021460 reamber-0.1.8/reamber/o2jam/O2JHold.py
+-rw-r--r--   0        0        0      259 2023-04-18 09:51:02.022465 reamber-0.1.8/reamber/o2jam/O2JHold.pyi
+-rw-r--r--   0        0        0     5874 2023-04-18 09:51:02.022465 reamber-0.1.8/reamber/o2jam/O2JMap.py
+-rw-r--r--   0        0        0     1578 2023-04-18 09:51:02.022465 reamber-0.1.8/reamber/o2jam/O2JMap.pyi
+-rw-r--r--   0        0        0     2116 2023-05-10 08:28:31.762070 reamber-0.1.8/reamber/o2jam/O2JMapSet.py
+-rw-r--r--   0        0        0     1049 2023-05-10 08:28:31.762070 reamber-0.1.8/reamber/o2jam/O2JMapSet.pyi
+-rw-r--r--   0        0        0     6728 2023-04-18 09:51:02.023465 reamber-0.1.8/reamber/o2jam/O2JMapSetMeta.py
+-rw-r--r--   0        0        0      189 2023-04-18 09:51:02.023465 reamber-0.1.8/reamber/o2jam/O2JNoteMeta.py
+-rw-r--r--   0        0        0      237 2023-04-18 09:51:02.023465 reamber-0.1.8/reamber/o2jam/O2JNoteMeta.pyi
+-rw-r--r--   0        0        0      548 2023-04-18 09:51:02.031466 reamber-0.1.8/reamber/osu/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-18 09:51:02.033466 reamber-0.1.8/reamber/osu/lists/__init__.py
+-rw-r--r--   0        0        0      239 2023-04-18 09:51:02.035466 reamber-0.1.8/reamber/osu/lists/notes/__init__.py
+-rw-r--r--   0        0        0     1140 2023-04-18 09:51:02.033466 reamber-0.1.8/reamber/osu/lists/notes/OsuHitList.py
+-rw-r--r--   0        0        0      493 2023-04-18 09:51:02.033466 reamber-0.1.8/reamber/osu/lists/notes/OsuHitList.pyi
+-rw-r--r--   0        0        0      714 2023-04-18 09:51:02.034465 reamber-0.1.8/reamber/osu/lists/notes/OsuHoldList.py
+-rw-r--r--   0        0        0      424 2023-04-18 09:51:02.034465 reamber-0.1.8/reamber/osu/lists/notes/OsuHoldList.pyi
+-rw-r--r--   0        0        0      331 2023-04-18 09:51:02.034465 reamber-0.1.8/reamber/osu/lists/notes/OsuNoteList.py
+-rw-r--r--   0        0        0     1032 2023-04-18 09:51:02.035466 reamber-0.1.8/reamber/osu/lists/notes/OsuNoteList.pyi
+-rw-r--r--   0        0        0      578 2023-04-18 09:51:02.031466 reamber-0.1.8/reamber/osu/lists/OsuBpmList.py
+-rw-r--r--   0        0        0      842 2023-04-18 09:51:02.032466 reamber-0.1.8/reamber/osu/lists/OsuBpmList.pyi
+-rw-r--r--   0        0        0      620 2023-04-18 09:51:02.032466 reamber-0.1.8/reamber/osu/lists/OsuSampleList.py
+-rw-r--r--   0        0        0      602 2023-04-18 09:51:02.032466 reamber-0.1.8/reamber/osu/lists/OsuSampleList.pyi
+-rw-r--r--   0        0        0      580 2023-04-18 09:51:02.032466 reamber-0.1.8/reamber/osu/lists/OsuSvList.py
+-rw-r--r--   0        0        0      974 2023-05-10 08:28:31.763070 reamber-0.1.8/reamber/osu/lists/OsuSvList.pyi
+-rw-r--r--   0        0        0     2454 2023-04-18 09:51:02.027466 reamber-0.1.8/reamber/osu/OsuBpm.py
+-rw-r--r--   0        0        0     1004 2023-04-18 09:51:02.027466 reamber-0.1.8/reamber/osu/OsuBpm.pyi
+-rw-r--r--   0        0        0     2236 2023-04-18 09:51:02.027466 reamber-0.1.8/reamber/osu/OsuHit.py
+-rw-r--r--   0        0        0      967 2023-04-18 09:51:02.027466 reamber-0.1.8/reamber/osu/OsuHit.pyi
+-rw-r--r--   0        0        0     2452 2023-04-18 09:51:02.028465 reamber-0.1.8/reamber/osu/OsuHold.py
+-rw-r--r--   0        0        0     1079 2023-04-18 09:51:02.028465 reamber-0.1.8/reamber/osu/OsuHold.pyi
+-rw-r--r--   0        0        0     5116 2023-04-18 09:51:02.028465 reamber-0.1.8/reamber/osu/OsuMap.py
+-rw-r--r--   0        0        0     2793 2023-05-10 08:28:31.763070 reamber-0.1.8/reamber/osu/OsuMap.pyi
+-rw-r--r--   0        0        0     7803 2023-04-18 09:51:02.029466 reamber-0.1.8/reamber/osu/OsuMapMeta.py
+-rw-r--r--   0        0        0     1945 2023-04-18 09:51:02.029466 reamber-0.1.8/reamber/osu/OsuNoteMeta.py
+-rw-r--r--   0        0        0     1153 2023-04-18 09:51:02.029466 reamber-0.1.8/reamber/osu/OsuNoteMeta.pyi
+-rw-r--r--   0        0        0     1300 2023-04-18 09:51:02.029466 reamber-0.1.8/reamber/osu/OsuSample.py
+-rw-r--r--   0        0        0      862 2023-04-18 09:51:02.030466 reamber-0.1.8/reamber/osu/OsuSample.pyi
+-rw-r--r--   0        0        0     1175 2023-04-18 09:51:02.030466 reamber-0.1.8/reamber/osu/OsuSampleSet.py
+-rw-r--r--   0        0        0     2536 2023-04-18 09:51:02.030466 reamber-0.1.8/reamber/osu/OsuSv.py
+-rw-r--r--   0        0        0     1174 2023-04-18 09:51:02.031466 reamber-0.1.8/reamber/osu/OsuSv.pyi
+-rw-r--r--   0        0        0      786 2023-04-18 09:51:02.031466 reamber-0.1.8/reamber/osu/OsuTimingPointMeta.py
+-rw-r--r--   0        0        0        0 2023-05-04 05:46:31.861060 reamber-0.1.8/reamber/py.typed
+-rw-r--r--   0        0        0      417 2023-04-18 09:51:02.039466 reamber-0.1.8/reamber/quaver/__init__.py
+-rw-r--r--   0        0        0      227 2023-04-18 09:51:02.041466 reamber-0.1.8/reamber/quaver/lists/__init__.py
+-rw-r--r--   0        0        0      248 2023-04-18 09:51:02.043466 reamber-0.1.8/reamber/quaver/lists/notes/__init__.py
+-rw-r--r--   0        0        0     1250 2023-04-18 09:51:02.041466 reamber-0.1.8/reamber/quaver/lists/notes/QuaHitList.py
+-rw-r--r--   0        0        0      383 2023-04-18 09:51:02.041466 reamber-0.1.8/reamber/quaver/lists/notes/QuaHitList.pyi
+-rw-r--r--   0        0        0     1571 2023-04-18 09:51:02.042466 reamber-0.1.8/reamber/quaver/lists/notes/QuaHoldList.py
+-rw-r--r--   0        0        0      382 2023-04-18 09:51:02.042466 reamber-0.1.8/reamber/quaver/lists/notes/QuaHoldList.pyi
+-rw-r--r--   0        0        0      560 2023-04-18 09:51:02.042466 reamber-0.1.8/reamber/quaver/lists/notes/QuaNoteList.py
+-rw-r--r--   0        0        0      548 2023-04-18 09:51:02.043466 reamber-0.1.8/reamber/quaver/lists/notes/QuaNoteList.pyi
+-rw-r--r--   0        0        0      996 2023-04-18 09:51:02.039466 reamber-0.1.8/reamber/quaver/lists/QuaBpmList.py
+-rw-r--r--   0        0        0      367 2023-04-18 09:51:02.040466 reamber-0.1.8/reamber/quaver/lists/QuaBpmList.pyi
+-rw-r--r--   0        0        0     1047 2023-04-18 09:51:02.040466 reamber-0.1.8/reamber/quaver/lists/QuaSvList.py
+-rw-r--r--   0        0        0      501 2023-04-18 09:51:02.040466 reamber-0.1.8/reamber/quaver/lists/QuaSvList.pyi
+-rw-r--r--   0        0        0      358 2023-04-18 09:51:02.041466 reamber-0.1.8/reamber/quaver/lists/QuaTimedList.py
+-rw-r--r--   0        0        0      465 2023-04-18 09:51:02.035466 reamber-0.1.8/reamber/quaver/QuaBpm.py
+-rw-r--r--   0        0        0      210 2023-04-18 09:51:02.036466 reamber-0.1.8/reamber/quaver/QuaBpm.pyi
+-rw-r--r--   0        0        0      949 2023-04-18 09:51:02.036466 reamber-0.1.8/reamber/quaver/QuaHit.py
+-rw-r--r--   0        0        0      392 2023-04-18 09:51:02.036466 reamber-0.1.8/reamber/quaver/QuaHit.pyi
+-rw-r--r--   0        0        0     1079 2023-04-18 09:51:02.036466 reamber-0.1.8/reamber/quaver/QuaHold.py
+-rw-r--r--   0        0        0      412 2023-04-18 09:51:02.037465 reamber-0.1.8/reamber/quaver/QuaHold.pyi
+-rw-r--r--   0        0        0     4139 2023-04-18 09:51:02.037465 reamber-0.1.8/reamber/quaver/QuaMap.py
+-rw-r--r--   0        0        0     1829 2023-05-10 08:28:31.764070 reamber-0.1.8/reamber/quaver/QuaMap.pyi
+-rw-r--r--   0        0        0     4669 2023-04-18 09:51:02.037465 reamber-0.1.8/reamber/quaver/QuaMapMeta.py
+-rw-r--r--   0        0        0      121 2023-04-18 09:51:02.038466 reamber-0.1.8/reamber/quaver/QuaNoteMeta.py
+-rw-r--r--   0        0        0      175 2023-04-18 09:51:02.038466 reamber-0.1.8/reamber/quaver/QuaNoteMeta.pyi
+-rw-r--r--   0        0        0      786 2023-04-18 09:51:02.038466 reamber-0.1.8/reamber/quaver/QuaSv.py
+-rw-r--r--   0        0        0      451 2023-04-18 09:51:02.038466 reamber-0.1.8/reamber/quaver/QuaSv.pyi
+-rw-r--r--   0        0        0      698 2023-04-18 09:51:02.048466 reamber-0.1.8/reamber/sm/__init__.py
+-rw-r--r--   0        0        0     2299 2023-04-18 09:51:02.043466 reamber-0.1.8/reamber/sm/CHART_TYPES
+-rw-r--r--   0        0        0     3129 2023-04-18 09:51:02.043466 reamber-0.1.8/reamber/sm/FILE_FORMAT
+-rw-r--r--   0        0        0      143 2023-04-18 09:51:02.049467 reamber-0.1.8/reamber/sm/lists/__init__.py
+-rw-r--r--   0        0        0      611 2023-04-18 09:51:02.054467 reamber-0.1.8/reamber/sm/lists/notes/__init__.py
+-rw-r--r--   0        0        0      324 2023-04-18 09:51:02.050466 reamber-0.1.8/reamber/sm/lists/notes/SMFakeList.py
+-rw-r--r--   0        0        0      257 2023-04-18 09:51:02.050466 reamber-0.1.8/reamber/sm/lists/notes/SMFakeList.pyi
+-rw-r--r--   0        0        0      318 2023-04-18 09:51:02.050466 reamber-0.1.8/reamber/sm/lists/notes/SMHitList.py
+-rw-r--r--   0        0        0      252 2023-04-18 09:51:02.051467 reamber-0.1.8/reamber/sm/lists/notes/SMHitList.pyi
+-rw-r--r--   0        0        0      327 2023-04-18 09:51:02.051467 reamber-0.1.8/reamber/sm/lists/notes/SMHoldList.py
+-rw-r--r--   0        0        0      260 2023-04-18 09:51:02.051467 reamber-0.1.8/reamber/sm/lists/notes/SMHoldList.pyi
+-rw-r--r--   0        0        0      348 2023-04-18 09:51:02.051467 reamber-0.1.8/reamber/sm/lists/notes/SMKeySoundList.py
+-rw-r--r--   0        0        0      277 2023-04-18 09:51:02.052465 reamber-0.1.8/reamber/sm/lists/notes/SMKeySoundList.pyi
+-rw-r--r--   0        0        0      324 2023-04-18 09:51:02.052465 reamber-0.1.8/reamber/sm/lists/notes/SMLiftList.py
+-rw-r--r--   0        0        0      257 2023-04-18 09:51:02.052465 reamber-0.1.8/reamber/sm/lists/notes/SMLiftList.pyi
+-rw-r--r--   0        0        0      324 2023-04-18 09:51:02.052465 reamber-0.1.8/reamber/sm/lists/notes/SMMineList.py
+-rw-r--r--   0        0        0      257 2023-04-18 09:51:02.052465 reamber-0.1.8/reamber/sm/lists/notes/SMMineList.pyi
+-rw-r--r--   0        0        0      288 2023-04-18 09:51:02.053465 reamber-0.1.8/reamber/sm/lists/notes/SMNoteList.py
+-rw-r--r--   0        0        0      186 2023-04-18 09:51:02.053465 reamber-0.1.8/reamber/sm/lists/notes/SMNoteList.pyi
+-rw-r--r--   0        0        0      327 2023-04-18 09:51:02.053465 reamber-0.1.8/reamber/sm/lists/notes/SMRollList.py
+-rw-r--r--   0        0        0      260 2023-04-18 09:51:02.053465 reamber-0.1.8/reamber/sm/lists/notes/SMRollList.pyi
+-rw-r--r--   0        0        0      229 2023-04-18 09:51:02.048466 reamber-0.1.8/reamber/sm/lists/SMBpmList.py
+-rw-r--r--   0        0        0      163 2023-04-18 09:51:02.049467 reamber-0.1.8/reamber/sm/lists/SMBpmList.pyi
+-rw-r--r--   0        0        0      246 2023-04-18 09:51:02.049467 reamber-0.1.8/reamber/sm/lists/SMStopList.py
+-rw-r--r--   0        0        0      303 2023-04-18 09:51:02.049467 reamber-0.1.8/reamber/sm/lists/SMStopList.pyi
+-rw-r--r--   0        0        0       66 2023-04-18 09:51:02.044465 reamber-0.1.8/reamber/sm/SMBpm.py
+-rw-r--r--   0        0        0       66 2023-04-18 09:51:02.044465 reamber-0.1.8/reamber/sm/SMBpm.pyi
+-rw-r--r--   0        0        0      291 2023-04-18 09:51:02.044465 reamber-0.1.8/reamber/sm/SMConst.py
+-rw-r--r--   0        0        0       67 2023-04-18 09:51:02.044465 reamber-0.1.8/reamber/sm/SMFake.py
+-rw-r--r--   0        0        0       66 2023-04-18 09:51:02.045466 reamber-0.1.8/reamber/sm/SMHit.py
+-rw-r--r--   0        0        0       70 2023-04-18 09:51:02.045466 reamber-0.1.8/reamber/sm/SMHold.py
+-rw-r--r--   0        0        0      164 2023-04-18 09:51:02.045466 reamber-0.1.8/reamber/sm/SMKeySound.py
+-rw-r--r--   0        0        0       67 2023-04-18 09:51:02.045466 reamber-0.1.8/reamber/sm/SMLift.py
+-rw-r--r--   0        0        0    13884 2023-04-18 09:51:02.046466 reamber-0.1.8/reamber/sm/SMMap.py
+-rw-r--r--   0        0        0     2297 2023-04-18 09:51:02.046466 reamber-0.1.8/reamber/sm/SMMap.pyi
+-rw-r--r--   0        0        0     6872 2023-04-18 09:51:02.046466 reamber-0.1.8/reamber/sm/SMMapMeta.py
+-rw-r--r--   0        0        0     2412 2023-05-10 08:28:31.764070 reamber-0.1.8/reamber/sm/SMMapSet.py
+-rw-r--r--   0        0        0     1138 2023-05-10 08:28:31.765070 reamber-0.1.8/reamber/sm/SMMapSet.pyi
+-rw-r--r--   0        0        0     6783 2023-04-18 09:51:02.047466 reamber-0.1.8/reamber/sm/SMMapSetMeta.py
+-rw-r--r--   0        0        0       67 2023-04-18 09:51:02.047466 reamber-0.1.8/reamber/sm/SMMine.py
+-rw-r--r--   0        0        0       72 2023-04-18 09:51:02.047466 reamber-0.1.8/reamber/sm/SMRoll.py
+-rw-r--r--   0        0        0      291 2023-04-18 09:51:02.048466 reamber-0.1.8/reamber/sm/SMStop.py
+-rw-r--r--   0        0        0      248 2023-04-18 09:51:02.048466 reamber-0.1.8/reamber/sm/SMStop.pyi
+-rw-r--r--   0        0        0     3274 1970-01-01 00:00:00.000000 reamber-0.1.8/setup.py
+-rw-r--r--   0        0        0     2366 1970-01-01 00:00:00.000000 reamber-0.1.8/PKG-INFO
```

### Comparing `reamber-0.1.7/README.md` & `reamber-0.1.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-![license](https://img.shields.io/github/license/Eve-ning/reamberPy)
-![dls](https://img.shields.io/pypi/dm/reamber)
-![codecov-coverage](https://img.shields.io/codecov/c/github/Eve-ning/reamberPy)
-![codefactor](https://img.shields.io/codefactor/grade/github/Eve-ning/reamberPy)
-![version](https://img.shields.io/pypi/v/reamber)
-
-# Reamber (Py) 
-
-[:blue_book: Wiki](https://eve-ning.github.io/reamberPy/index.html) & [Getting Started](https://eve-ning.github.io/reamberPy/info/GettingStarted.html)
-
-**Supports Python `3.7`, `3.8`, `3.9`**
-
-`pip install reamber`
-
-------
-
-This is a simple package to handle VSRG files, useful if you'd want to manipulate data
-such as offset, column, bpm, etc.
-
-This doesn't provide complex algorithms, only the base dataclasses and helpful basic
-algorithms
-
-## Migrating to >v0.1.1 Releases
-
-Migrating to `>0.1.1` means spending time updating **a lot** of names.
-
-Major changes in `0.1.1` include many differences in naming. 
-Only update it if you don't plan mind spending time refactoring.
-
-## For Developers
-
-Note that this is still in alpha stage, means a lot of things aren't settled down
-yet. In other words, many function names and references will change without notice.
-
-It is recommended to only build scratch/temp files if you want to utilize this library
-
-## Motivation
-
-A growing amount of osu!mania players are becoming interested in programming.
-The best way to learn is to relate it to something that you're familiar with.
-That's why I'm making a library for most common VSRG (Vertical Scrolling Rhythm Game)
-types.
+![license](https://img.shields.io/github/license/Eve-ning/reamberPy)
+![dls](https://img.shields.io/pypi/dm/reamber)
+![codecov-coverage](https://img.shields.io/codecov/c/github/Eve-ning/reamberPy)
+![codefactor](https://img.shields.io/codefactor/grade/github/Eve-ning/reamberPy)
+![version](https://img.shields.io/pypi/v/reamber)
+
+# Reamber (Py) 
+
+[:blue_book: Wiki](https://eve-ning.github.io/reamberPy/index.html) & [Getting Started](https://eve-ning.github.io/reamberPy/info/GettingStarted.html)
+
+`pip install reamber`
+
+------
+
+VSRG Toolbox for data extraction, manipulation & analysis.
+
+# Features
+
+- Game Support: osu!mania, StepMania, BMS and partially O2Jam files.
+- Algorithms: Map IO, Conversion, Map Image Generation, Pattern Extraction
+- Data Architecture: Pandas DataFrame Integration
+
+> This is built on pandas `DataFrame`, thus, if you need more control, you can 
+retrieve the underlying `DataFrame` via the `.df` property on many reamber classes. 
+
+# Status
+
+This is in alpha, names and references will change without notice.
+We highly recommended to fix version in requirements.
+
+## For Developers, By Developers
+
+A growing amount of osu!mania players are interested in programming.
+The best way to learn is to relate it to something that you're familiar with.
+
+That's why I'm making a library that allows you to tamper with your favorite
+games, and learn on the way.
+
+# Migrating to >v0.1.1 Releases
+
+Migrating to `>0.1.1` means spending time updating **a lot** of names.
+
+Major changes in `0.1.1` include many differences in naming. 
+Only update it if you don't plan mind spending time refactoring.
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/BMSToOsu.py` & `reamber-0.1.8/reamber/algorithms/convert/QuaToOsu.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-from unidecode import unidecode
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.bms.BMSMap import BMSMap
-from reamber.osu.OsuMap import OsuMap
-from reamber.osu.lists.OsuBpmList import OsuBpmList
-from reamber.osu.lists.notes.OsuHitList import OsuHitList
-from reamber.osu.lists.notes.OsuHoldList import OsuHoldList
-
-
-class BMSToOsu(ConvertBase):
-    @classmethod
-    def convert(cls, bms: BMSMap) -> OsuMap:
-        """Converts a BMS map to an osu map"""
-
-        osu = OsuMap()
-        osu.hits = cls.cast(
-            bms.hits, OsuHitList,
-            dict(
-                offset='offset', column='column',
-                hitsound_file=bms.hits.sample.apply(str, args={'ascii'})
-            )
-        )
-        osu.holds = cls.cast(
-            bms.holds, OsuHoldList,
-            dict(
-                offset='offset', column='column', length='length',
-                hitsound_file=bms.holds.sample.apply(str, args={'ascii'})
-            )
-        )
-        osu.bpms = cls.cast(
-            bms.bpms, OsuBpmList,
-            dict(offset='offset', bpm='bpm')
-        )
-
-        osu.title = unidecode(bms.title.decode('sjis'))
-        osu.version = unidecode(bms.version.decode('sjis'))
-        osu.artist = unidecode(bms.artist.decode('sjis'))
-        osu.circle_size = bms.stack().column.max() + 1
-
-        return osu
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.osu.OsuMap import OsuMap
+from reamber.osu.lists.OsuBpmList import OsuBpmList
+from reamber.osu.lists.OsuSvList import OsuSvList
+from reamber.osu.lists.notes.OsuHitList import OsuHitList
+from reamber.osu.lists.notes.OsuHoldList import OsuHoldList
+from reamber.quaver.QuaMap import QuaMap
+from reamber.quaver.QuaMapMeta import QuaMapMode
+
+
+class QuaToOsu(ConvertBase):
+    @classmethod
+    def convert(cls, qua: QuaMap) -> OsuMap:
+        """Converts a Quaver map to an osu map"""
+
+        osu = OsuMap()
+        osu.hits = cls.cast(
+            qua.hits, OsuHitList,
+            dict(offset='offset', column='column')
+        )
+        osu.holds = cls.cast(
+            qua.holds, OsuHoldList,
+            dict(offset='offset', column='column', length='length')
+        )
+        osu.bpms = cls.cast(
+            qua.bpms, OsuBpmList,
+            dict(offset='offset', bpm='bpm')
+        )
+        osu.svs = cls.cast(
+            qua.svs, OsuSvList,
+            dict(offset='offset', multiplier='multiplier')
+        )
+
+        osu.background_file_name = qua.background_file
+        osu.circle_size = QuaMapMode.get_keys(qua.mode)
+        osu.title = qua.title
+        osu.title_unicode = qua.title
+        osu.artist = qua.artist
+        osu.artist_unicode = qua.artist
+        osu.audio_file_name = qua.audio_file
+        osu.creator = qua.creator
+        osu.version = qua.difficulty_name
+        osu.preview_time = qua.song_preview_time
+        osu.tags = qua.tags
+
+        return osu
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/BMSToQua.py` & `reamber-0.1.8/reamber/algorithms/convert/BMSToQua.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from unidecode import unidecode
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.bms.BMSMap import BMSMap
-from reamber.quaver.QuaMap import QuaMap
-from reamber.quaver.QuaMapMeta import QuaMapMode
-from reamber.quaver.lists import QuaBpmList
-from reamber.quaver.lists.notes.QuaHitList import QuaHitList
-from reamber.quaver.lists.notes.QuaHoldList import QuaHoldList
-
-
-class BMSToQua(ConvertBase):
-    @classmethod
-    def convert(cls, bms: BMSMap, raise_bad_mode: bool = True) -> QuaMap:
-        """Converts a BMS to a Qua Map
-
-        Args
-            bms: BMS Map
-            raise_bad_mode: Raises if Quaver can't support this key mode
-        """
-
-        qua = QuaMap()
-        qua.hits = cls.cast(
-            bms.hits, QuaHitList, dict(offset='offset', column='column')
-        )
-        qua.holds = cls.cast(
-            bms.holds, QuaHoldList,
-            dict(offset='offset', column='column', length='length')
-        )
-        qua.bpms = cls.cast(
-            bms.bpms, QuaBpmList,
-            dict(offset='offset', bpm='bpm')
-        )
-
-        qua.title = unidecode(bms.title.decode('sjis'))
-        qua.mode = QuaMapMode.get_mode(int(bms.stack().column.max() + 1))
-        qua.difficulty_name = unidecode(bms.version.decode('sjis'))
-        qua.artist = unidecode(bms.artist.decode('sjis'))
-
-        if raise_bad_mode and not qua.mode:
-            raise ValueError(
-                f"Keys {int(bms.stack().column.max() + 1)} isn't supported"
-                f"by Quaver."
-            )
-
-        return qua
+from unidecode import unidecode
+
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.bms.BMSMap import BMSMap
+from reamber.quaver.QuaMap import QuaMap
+from reamber.quaver.QuaMapMeta import QuaMapMode
+from reamber.quaver.lists import QuaBpmList
+from reamber.quaver.lists.notes.QuaHitList import QuaHitList
+from reamber.quaver.lists.notes.QuaHoldList import QuaHoldList
+
+
+class BMSToQua(ConvertBase):
+    @classmethod
+    def convert(cls, bms: BMSMap, raise_bad_mode: bool = True) -> QuaMap:
+        """Converts a BMS to a Qua Map
+
+        Args
+            bms: BMS Map
+            raise_bad_mode: Raises if Quaver can't support this key mode
+        """
+
+        qua = QuaMap()
+        qua.hits = cls.cast(
+            bms.hits, QuaHitList, dict(offset='offset', column='column')
+        )
+        qua.holds = cls.cast(
+            bms.holds, QuaHoldList,
+            dict(offset='offset', column='column', length='length')
+        )
+        qua.bpms = cls.cast(
+            bms.bpms, QuaBpmList,
+            dict(offset='offset', bpm='bpm')
+        )
+
+        qua.title = unidecode(bms.title.decode('sjis'))
+        qua.mode = QuaMapMode.get_mode(int(bms.stack().column.max() + 1))
+        qua.difficulty_name = unidecode(bms.version.decode('sjis'))
+        qua.artist = unidecode(bms.artist.decode('sjis'))
+
+        if raise_bad_mode and not qua.mode:
+            raise ValueError(
+                f"Keys {int(bms.stack().column.max() + 1)} isn't supported"
+                f"by Quaver."
+            )
+
+        return qua
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/BMSToSM.py` & `reamber-0.1.8/reamber/algorithms/convert/BMSToSM.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from unidecode import unidecode
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.bms.BMSMap import BMSMap
-from reamber.sm.SMMap import SMMap
-from reamber.sm.SMMapMeta import SMMapChartTypes
-from reamber.sm.SMMapSet import SMMapSet
-from reamber.sm.lists.SMBpmList import SMBpmList
-from reamber.sm.lists.notes.SMHitList import SMHitList
-from reamber.sm.lists.notes.SMHoldList import SMHoldList
-
-
-class BMSToSM(ConvertBase):
-    @classmethod
-    def convert(cls, bms: BMSMap) -> SMMapSet:
-        """Converts a Mapset to multiple SM maps"""
-
-        sm = SMMap()
-        sm.hits = cls.cast(
-            bms.hits, SMHitList, dict(offset='offset', column='column')
-        )
-        sm.holds = cls.cast(
-            bms.holds, SMHoldList,
-            dict(offset='offset', column='column', length='length')
-        )
-        sm.bpms = cls.cast(
-            bms.bpms, SMBpmList, dict(offset='offset', bpm='bpm')
-        )
-
-        sm.description = unidecode(bms.version.decode('sjis'))
-        sm.chart_type = SMMapChartTypes.get_type(bms.stack().column.max() + 1)
-        sms = SMMapSet()
-        sms.maps = [sm]
-
-        sms.title = unidecode(bms.title.decode('sjis'))
-        sms.artist = unidecode(bms.artist.decode('sjis'))
-        sms.offset = 0.0
-
-        return sms
+from unidecode import unidecode
+
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.bms.BMSMap import BMSMap
+from reamber.sm.SMMap import SMMap
+from reamber.sm.SMMapMeta import SMMapChartTypes
+from reamber.sm.SMMapSet import SMMapSet
+from reamber.sm.lists.SMBpmList import SMBpmList
+from reamber.sm.lists.notes.SMHitList import SMHitList
+from reamber.sm.lists.notes.SMHoldList import SMHoldList
+
+
+class BMSToSM(ConvertBase):
+    @classmethod
+    def convert(cls, bms: BMSMap) -> SMMapSet:
+        """Converts a Mapset to multiple SM maps"""
+
+        sm = SMMap()
+        sm.hits = cls.cast(
+            bms.hits, SMHitList, dict(offset='offset', column='column')
+        )
+        sm.holds = cls.cast(
+            bms.holds, SMHoldList,
+            dict(offset='offset', column='column', length='length')
+        )
+        sm.bpms = cls.cast(
+            bms.bpms, SMBpmList, dict(offset='offset', bpm='bpm')
+        )
+
+        sm.description = unidecode(bms.version.decode('sjis'))
+        sm.chart_type = SMMapChartTypes.get_type(bms.stack().column.max() + 1)
+        sms = SMMapSet()
+        sms.maps = [sm]
+
+        sms.title = unidecode(bms.title.decode('sjis'))
+        sms.artist = unidecode(bms.artist.decode('sjis'))
+        sms.offset = 0.0
+
+        return sms
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/O2JToBMS.py` & `reamber-0.1.8/reamber/algorithms/convert/O2JToBMS.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import codecs
-from typing import List
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.bms.BMSMap import BMSMap
-from reamber.bms.lists.BMSBpmList import BMSBpmList
-from reamber.bms.lists.notes.BMSHitList import BMSHitList
-from reamber.bms.lists.notes.BMSHoldList import BMSHoldList
-from reamber.o2jam.O2JMapSet import O2JMapSet
-
-
-class O2JToBMS(ConvertBase):
-    @classmethod
-    def convert(cls, o2js: O2JMapSet, move_right_by: int = 1) -> List[BMSMap]:
-        """Converts a Mapset to multiple BMS maps
-
-        Note:
-            Column 0 is the scratch.
-
-            Thus, converting 7k with ``moveRightBy == 1`` to remove the
-            first column scratch
-
-        Args:
-            o2js: O2Jam Mapset
-            move_right_by: Moves every column to the right by
-        """
-
-        bmss: List[BMSMap] = []
-        for o2j in o2js:
-            bms = BMSMap()
-            bms.hits = cls.cast(
-                o2j.hits, BMSHitList, dict(offset='offset', column='column')
-            )
-            bms.holds = cls.cast(
-                o2j.holds, BMSHoldList,
-                dict(offset='offset', column='column', length='length')
-            )
-            bms.bpms = cls.cast(
-                o2j.bpms, BMSBpmList, dict(offset='offset', bpm='bpm')
-            )
-            bms.stack().column += move_right_by
-
-            bms.title = codecs.encode(o2js.title, encoding='shift_jis')
-            bms.artist = codecs.encode(o2js.artist, encoding='shift_jis')
-            bms.version = codecs.encode(
-                f"{o2js.level_name(o2j)}", encoding='shift_jis'
-            )
-
-            bmss.append(bms)
-        return bmss
+import codecs
+from typing import List
+
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.bms.BMSMap import BMSMap
+from reamber.bms.lists.BMSBpmList import BMSBpmList
+from reamber.bms.lists.notes.BMSHitList import BMSHitList
+from reamber.bms.lists.notes.BMSHoldList import BMSHoldList
+from reamber.o2jam.O2JMapSet import O2JMapSet
+
+
+class O2JToBMS(ConvertBase):
+    @classmethod
+    def convert(cls, o2js: O2JMapSet, move_right_by: int = 1) -> List[BMSMap]:
+        """Converts a Mapset to multiple BMS maps
+
+        Note:
+            Column 0 is the scratch.
+
+            Thus, converting 7k with ``moveRightBy == 1`` to remove the
+            first column scratch
+
+        Args:
+            o2js: O2Jam Mapset
+            move_right_by: Moves every column to the right by
+        """
+
+        bmss: List[BMSMap] = []
+        for o2j in o2js:
+            bms = BMSMap()
+            bms.hits = cls.cast(
+                o2j.hits, BMSHitList, dict(offset='offset', column='column')
+            )
+            bms.holds = cls.cast(
+                o2j.holds, BMSHoldList,
+                dict(offset='offset', column='column', length='length')
+            )
+            bms.bpms = cls.cast(
+                o2j.bpms, BMSBpmList, dict(offset='offset', bpm='bpm')
+            )
+            bms.stack().column += move_right_by
+
+            bms.title = codecs.encode(o2js.title, encoding='shift_jis')
+            bms.artist = codecs.encode(o2js.artist, encoding='shift_jis')
+            bms.version = codecs.encode(
+                f"{o2js.level_name(o2j)}", encoding='shift_jis'
+            )
+
+            bmss.append(bms)
+        return bmss
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/O2JToOsu.py` & `reamber-0.1.8/reamber/algorithms/convert/SMToOsu.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,37 +1,45 @@
-from typing import List
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.o2jam.O2JMapSet import O2JMapSet
-from reamber.osu.OsuMap import OsuMap
-from reamber.osu.lists.OsuBpmList import OsuBpmList
-from reamber.osu.lists.notes.OsuHitList import OsuHitList
-from reamber.osu.lists.notes.OsuHoldList import OsuHoldList
-
-
-class O2JToOsu(ConvertBase):
-    @classmethod
-    def convert(cls, o2js: O2JMapSet) -> List[OsuMap]:
-        """Converts a Mapset to multiple Osu maps"""
-
-        osus: List[OsuMap] = []
-        for o2j in o2js:
-            osu = OsuMap()
-            osu.hits = cls.cast(
-                o2j.hits, OsuHitList, dict(offset='offset', column='column')
-            )
-            osu.holds = cls.cast(
-                o2j.holds, OsuHoldList,
-                dict(offset='offset', column='column', length='length')
-            )
-            osu.bpms = cls.cast(
-                o2j.bpms, OsuBpmList, dict(offset='offset', bpm='bpm')
-            )
-
-            osu.title = o2js.title
-            osu.artist = o2js.artist
-            osu.creator = o2js.creator
-            osu.version = f"Level {o2js.level_name(o2j)}"
-            osu.circle_size = 7
-            osus.append(osu)
-
-        return osus
+from typing import List
+
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.osu.OsuMap import OsuMap
+from reamber.osu.lists.OsuBpmList import OsuBpmList
+from reamber.osu.lists.notes.OsuHitList import OsuHitList
+from reamber.osu.lists.notes.OsuHoldList import OsuHoldList
+from reamber.sm.SMMapSet import SMMapSet
+
+
+class SMToOsu(ConvertBase):
+    @classmethod
+    def convert(cls, sms: SMMapSet) -> List[OsuMap]:
+        """Converts a SMMapset to possibly multiple osu maps"""
+
+        # I haven't tested with non 4 keys, so it might explode :(
+
+        osus: List[OsuMap] = []
+        for sm in sms:
+            osu = OsuMap()
+            osu.hits = cls.cast(
+                sm.hits, OsuHitList,
+                dict(offset='offset', column='column')
+            )
+            osu.holds = cls.cast(
+                sm.holds, OsuHoldList,
+                dict(offset='offset', column='column', length='length')
+            )
+            osu.bpms = cls.cast(
+                sm.bpms, OsuBpmList,
+                dict(offset='offset', bpm='bpm')
+            )
+
+            osu.background_file_name = sms.background
+            osu.title = sms.title
+            osu.title_unicode = sms.title_translit
+            osu.artist = sms.artist
+            osu.artist_unicode = sms.artist_translit
+            osu.audio_file_name = sms.music
+            osu.creator = sms.credit
+            osu.version = f"{sm.difficulty} {sm.difficulty_val}"
+            osu.preview_time = int(sms.sample_start)
+
+            osus.append(osu)
+        return osus
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/O2JToQua.py` & `reamber-0.1.8/reamber/algorithms/convert/O2JToQua.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from typing import List
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.o2jam.O2JMapSet import O2JMapSet
-from reamber.quaver.QuaMap import QuaMap
-from reamber.quaver.QuaMapMeta import QuaMapMode
-from reamber.quaver.lists.QuaBpmList import QuaBpmList
-from reamber.quaver.lists.notes.QuaHitList import QuaHitList
-from reamber.quaver.lists.notes.QuaHoldList import QuaHoldList
-
-
-class O2JToQua(ConvertBase):
-    @classmethod
-    def convert(cls, o2js: O2JMapSet) -> List[QuaMap]:
-        """Converts a Mapset to multiple Quaver maps"""
-
-        quas: List[QuaMap] = []
-        for o2j in o2js:
-            qua = QuaMap()
-            qua.hits = cls.cast(
-                o2j.hits, QuaHitList, dict(offset='offset', column='column')
-            )
-            qua.holds = cls.cast(
-                o2j.holds, QuaHoldList,
-                dict(offset='offset', column='column', length='length')
-            )
-            qua.bpms = cls.cast(
-                o2j.bpms, QuaBpmList, dict(offset='offset', bpm='bpm')
-            )
-
-            qua.title = o2js.title
-            qua.artist = o2js.artist
-            qua.creator = o2js.creator
-            qua.mode = QuaMapMode.KEYS_7
-            qua.difficulty_name = f"Level {o2js.level_name(o2j)}"
-
-            quas.append(qua)
-
-        return quas
+from typing import List
+
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.o2jam.O2JMapSet import O2JMapSet
+from reamber.quaver.QuaMap import QuaMap
+from reamber.quaver.QuaMapMeta import QuaMapMode
+from reamber.quaver.lists.QuaBpmList import QuaBpmList
+from reamber.quaver.lists.notes.QuaHitList import QuaHitList
+from reamber.quaver.lists.notes.QuaHoldList import QuaHoldList
+
+
+class O2JToQua(ConvertBase):
+    @classmethod
+    def convert(cls, o2js: O2JMapSet) -> List[QuaMap]:
+        """Converts a Mapset to multiple Quaver maps"""
+
+        quas: List[QuaMap] = []
+        for o2j in o2js:
+            qua = QuaMap()
+            qua.hits = cls.cast(
+                o2j.hits, QuaHitList, dict(offset='offset', column='column')
+            )
+            qua.holds = cls.cast(
+                o2j.holds, QuaHoldList,
+                dict(offset='offset', column='column', length='length')
+            )
+            qua.bpms = cls.cast(
+                o2j.bpms, QuaBpmList, dict(offset='offset', bpm='bpm')
+            )
+
+            qua.title = o2js.title
+            qua.artist = o2js.artist
+            qua.creator = o2js.creator
+            qua.mode = QuaMapMode.KEYS_7
+            qua.difficulty_name = f"Level {o2js.level_name(o2j)}"
+
+            quas.append(qua)
+
+        return quas
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/O2JToSM.py` & `reamber-0.1.8/reamber/algorithms/convert/O2JToSM.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from typing import List
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.o2jam.O2JMapSet import O2JMapSet
-from reamber.sm import SMMap
-from reamber.sm.SMMapMeta import SMMapChartTypes
-from reamber.sm.SMMapSet import SMMapSet
-from reamber.sm.lists.SMBpmList import SMBpmList
-from reamber.sm.lists.notes.SMHitList import SMHitList
-from reamber.sm.lists.notes.SMHoldList import SMHoldList
-
-
-class O2JToSM(ConvertBase):
-    @classmethod
-    def convert(cls, o2js: O2JMapSet) -> List[SMMapSet]:
-        """Converts a Mapset to multiple SM maps
-
-        Notes:
-            As bpms may not be consistent, a list of SMSet would be generated.
-            If you're certain to merge, use convert_merge.
-        """
-
-        smss = []
-
-        for o2j in o2js:
-            sms = SMMapSet()
-            sm = SMMap()
-            sm.hits = cls.cast(
-                o2j.hits, SMHitList, dict(offset='offset', column='column')
-            )
-            sm.holds = cls.cast(
-                o2j.holds, SMHoldList,
-                dict(offset='offset', column='column', length='length')
-            )
-            sm.bpms = cls.cast(o2j.bpms, SMBpmList,
-                               dict(offset='offset', bpm='bpm'))
-            sm.chart_type = SMMapChartTypes.get_type(
-                o2j.stack().column.max() + 1)
-
-            sms.maps = [sm]
-
-            sms.title = o2js.title
-            sms.artist = o2js.artist
-            sms.credit = o2js.creator
-            sms.offset = 0.0
-
-            smss.append(sms)
-
-        return smss
-
-    @classmethod
-    def convert_merge(cls, o2js: O2JMapSet) -> SMMapSet:
-        """Converts a Mapset to a single SM mapset.
-
-        Notes
-            If the bpms aren't consistent, this creates a corrupted SMMapSet.
-        """
-
-        sms = SMMapSet()
-
-        for o2j in o2js:
-            sms = SMMapSet()
-            sm = SMMap()
-            sm.hits = cls.cast(
-                o2j.hits, SMHitList, dict(offset='offset', column='column')
-            )
-            sm.holds = cls.cast(
-                o2j.holds, SMHoldList,
-                dict(offset='offset', column='column', length='length')
-            )
-            sm.bpms = cls.cast(
-                o2j.bpms, SMBpmList, dict(offset='offset', bpm='bpm')
-            )
-
-            sms.maps.append(sm)
-
-        sms.title = o2js.title
-        sms.artist = o2js.artist
-        sms.credit = o2js.creator
-        sms.offset = 0.0
-
-        return sms
+from typing import List
+
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.o2jam.O2JMapSet import O2JMapSet
+from reamber.sm import SMMap
+from reamber.sm.SMMapMeta import SMMapChartTypes
+from reamber.sm.SMMapSet import SMMapSet
+from reamber.sm.lists.SMBpmList import SMBpmList
+from reamber.sm.lists.notes.SMHitList import SMHitList
+from reamber.sm.lists.notes.SMHoldList import SMHoldList
+
+
+class O2JToSM(ConvertBase):
+    @classmethod
+    def convert(cls, o2js: O2JMapSet) -> List[SMMapSet]:
+        """Converts a Mapset to multiple SM maps
+
+        Notes:
+            As bpms may not be consistent, a list of SMSet would be generated.
+            If you're certain to merge, use convert_merge.
+        """
+
+        smss = []
+
+        for o2j in o2js:
+            sms = SMMapSet()
+            sm = SMMap()
+            sm.hits = cls.cast(
+                o2j.hits, SMHitList, dict(offset='offset', column='column')
+            )
+            sm.holds = cls.cast(
+                o2j.holds, SMHoldList,
+                dict(offset='offset', column='column', length='length')
+            )
+            sm.bpms = cls.cast(o2j.bpms, SMBpmList,
+                               dict(offset='offset', bpm='bpm'))
+            sm.chart_type = SMMapChartTypes.get_type(
+                o2j.stack().column.max() + 1)
+
+            sms.maps = [sm]
+
+            sms.title = o2js.title
+            sms.artist = o2js.artist
+            sms.credit = o2js.creator
+            sms.offset = 0.0
+
+            smss.append(sms)
+
+        return smss
+
+    @classmethod
+    def convert_merge(cls, o2js: O2JMapSet) -> SMMapSet:
+        """Converts a Mapset to a single SM mapset.
+
+        Notes
+            If the bpms aren't consistent, this creates a corrupted SMMapSet.
+        """
+
+        sms = SMMapSet()
+
+        for o2j in o2js:
+            sms = SMMapSet()
+            sm = SMMap()
+            sm.hits = cls.cast(
+                o2j.hits, SMHitList, dict(offset='offset', column='column')
+            )
+            sm.holds = cls.cast(
+                o2j.holds, SMHoldList,
+                dict(offset='offset', column='column', length='length')
+            )
+            sm.bpms = cls.cast(
+                o2j.bpms, SMBpmList, dict(offset='offset', bpm='bpm')
+            )
+
+            sms.maps.append(sm)
+
+        sms.title = o2js.title
+        sms.artist = o2js.artist
+        sms.credit = o2js.creator
+        sms.offset = 0.0
+
+        return sms
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/OsuToBMS.py` & `reamber-0.1.8/reamber/algorithms/convert/QuaToBMS.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,47 @@
-import codecs
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.bms.BMSMap import BMSMap
-from reamber.bms.lists.BMSBpmList import BMSBpmList
-from reamber.bms.lists.notes.BMSHitList import BMSHitList
-from reamber.bms.lists.notes.BMSHoldList import BMSHoldList
-from reamber.osu.OsuMap import OsuMap
-
-
-class OsuToBMS(ConvertBase):
-    @classmethod
-    def convert(cls, osu: OsuMap, move_right_by: int = 0) -> BMSMap:
-        """Converts osu to a BMS map
-
-        Note:
-            Column 0 is the scratch.
-
-            Thus, converting 7k with ``moveRightBy == 1`` to remove the
-            first column scratch
-
-        Args:
-            osu: Osu Map
-            move_right_by: Moves every column to the right by
-        """
-
-        bms = BMSMap()
-        bms.hits = cls.cast(
-            osu.hits, BMSHitList, dict(offset='offset', column='column')
-        )
-        bms.holds = cls.cast(
-            osu.holds, BMSHoldList,
-            dict(offset='offset', column='column', length='length')
-        )
-        bms.bpms = cls.cast(
-            osu.bpms, BMSBpmList,
-            dict(offset='offset', bpm='bpm')
-        )
-
-        bms.stack().column += move_right_by
-
-        bms.title = codecs.encode(osu.title, encoding='shift_jis')
-        bms.artist = codecs.encode(osu.artist, encoding='shift_jis')
-        bms.version = codecs.encode(osu.version, encoding='shift_jis')
-
-        return bms
+import codecs
+
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.bms.BMSMap import BMSMap
+from reamber.bms.lists.BMSBpmList import BMSBpmList
+from reamber.bms.lists.notes.BMSHitList import BMSHitList
+from reamber.bms.lists.notes.BMSHoldList import BMSHoldList
+from reamber.quaver.QuaMap import QuaMap
+
+
+class QuaToBMS(ConvertBase):
+    @classmethod
+    def convert(cls, qua: QuaMap, move_right_by: int = 0) -> BMSMap:
+        """Converts qua to a BMS map
+
+        Note:
+            Column 0 is the scratch.
+
+            Thus, converting 7k with ``moveRightBy == 1`` to remove the
+            first column scratch
+
+        Args:
+            qua: Quaver Map
+            move_right_by: Moves every column to the right by
+        """
+
+        bms = BMSMap()
+        bms.hits = cls.cast(
+            qua.hits, BMSHitList,
+            dict(offset='offset', column='column')
+        )
+        bms.holds = cls.cast(
+            qua.holds, BMSHoldList,
+            dict(offset='offset', column='column', length='length')
+        )
+        bms.bpms = cls.cast(
+            qua.bpms, BMSBpmList,
+            dict(offset='offset', bpm='bpm')
+        )
+
+        bms.stack().column += move_right_by
+
+        bms.title = codecs.encode(qua.title, encoding='shift_jis')
+        bms.artist = codecs.encode(qua.artist, encoding='shift_jis')
+        bms.version = codecs.encode(qua.difficulty_name, encoding='shift_jis')
+
+        return bms
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/OsuToQua.py` & `reamber-0.1.8/reamber/algorithms/convert/OsuToQua.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.osu.OsuMap import OsuMap
-from reamber.quaver.QuaMap import QuaMap
-from reamber.quaver.QuaMapMeta import QuaMapMode
-from reamber.quaver.lists import QuaBpmList
-from reamber.quaver.lists import QuaSvList
-from reamber.quaver.lists.notes.QuaHitList import QuaHitList
-from reamber.quaver.lists.notes.QuaHoldList import QuaHoldList
-
-
-class OsuToQua(ConvertBase):
-    @classmethod
-    def convert(cls, osu: OsuMap, raise_bad_mode: bool = True) -> QuaMap:
-        """Converts Osu to a Qua Map
-
-        Args:
-            osu: Osu Map
-            raise_bad_mode: Raises if Quaver can't support this key mode
-        """
-
-        qua = QuaMap()
-        qua.hits = cls.cast(
-            osu.hits, QuaHitList, dict(offset='offset', column='column')
-        )
-        qua.holds = cls.cast(
-            osu.holds, QuaHoldList,
-            dict(offset='offset', column='column', length='length')
-        )
-        qua.bpms = cls.cast(
-            osu.bpms, QuaBpmList,
-            dict(offset='offset', bpm='bpm')
-        )
-        qua.sv = cls.cast(
-            osu.svs, QuaSvList,
-            dict(offset='offset', multiplier='multiplier')
-        )
-
-        qua.audio_file = osu.audio_file_name
-        qua.title = osu.title
-        qua.mode = QuaMapMode.get_mode(int(osu.circle_size))
-        qua.artist = osu.artist
-        qua.creator = osu.creator
-        qua.tags = osu.tags
-        qua.difficulty_name = osu.version
-        qua.background_file = osu.background_file_name
-        qua.song_preview_time = osu.preview_time
-
-        if raise_bad_mode and not qua.mode:
-            raise ValueError(
-                f"Keys {int(osu.stack().column.max() + 1)} isn't supported"
-                f"by Quaver."
-            )
-
-        return qua
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.osu.OsuMap import OsuMap
+from reamber.quaver.QuaMap import QuaMap
+from reamber.quaver.QuaMapMeta import QuaMapMode
+from reamber.quaver.lists import QuaBpmList
+from reamber.quaver.lists import QuaSvList
+from reamber.quaver.lists.notes.QuaHitList import QuaHitList
+from reamber.quaver.lists.notes.QuaHoldList import QuaHoldList
+
+
+class OsuToQua(ConvertBase):
+    @classmethod
+    def convert(cls, osu: OsuMap, raise_bad_mode: bool = True) -> QuaMap:
+        """Converts Osu to a Qua Map
+
+        Args:
+            osu: Osu Map
+            raise_bad_mode: Raises if Quaver can't support this key mode
+        """
+
+        qua = QuaMap()
+        qua.hits = cls.cast(
+            osu.hits, QuaHitList, dict(offset='offset', column='column')
+        )
+        qua.holds = cls.cast(
+            osu.holds, QuaHoldList,
+            dict(offset='offset', column='column', length='length')
+        )
+        qua.bpms = cls.cast(
+            osu.bpms, QuaBpmList,
+            dict(offset='offset', bpm='bpm')
+        )
+        qua.sv = cls.cast(
+            osu.svs, QuaSvList,
+            dict(offset='offset', multiplier='multiplier')
+        )
+
+        qua.audio_file = osu.audio_file_name
+        qua.title = osu.title
+        qua.mode = QuaMapMode.get_mode(int(osu.circle_size))
+        qua.artist = osu.artist
+        qua.creator = osu.creator
+        qua.tags = osu.tags
+        qua.difficulty_name = osu.version
+        qua.background_file = osu.background_file_name
+        qua.song_preview_time = osu.preview_time
+
+        if raise_bad_mode and not qua.mode:
+            raise ValueError(
+                f"Keys {int(osu.stack().column.max() + 1)} isn't supported"
+                f"by Quaver."
+            )
+
+        return qua
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/OsuToSM.py` & `reamber-0.1.8/reamber/algorithms/convert/OsuToSM.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.osu.OsuMap import OsuMap
-from reamber.sm.SMMap import SMMap
-from reamber.sm.SMMapMeta import SMMapChartTypes
-from reamber.sm.SMMapSet import SMMapSet
-from reamber.sm.lists.SMBpmList import SMBpmList
-from reamber.sm.lists.notes.SMHitList import SMHitList
-from reamber.sm.lists.notes.SMHoldList import SMHoldList
-
-
-class OsuToSM(ConvertBase):
-    @classmethod
-    def convert(cls, osu: OsuMap, raise_bad_mode: bool = True) -> SMMapSet:
-        """Converts Osu to a SMMapset Obj
-
-        Args:
-            osu: Osu Map
-            raise_bad_mode: Raises if SM can't support this key mode
-        """
-
-        sm = SMMap()
-
-        sm.hits = cls.cast(
-            osu.hits, SMHitList,
-            dict(offset='offset', column='column')
-        )
-        sm.holds = cls.cast(
-            osu.holds, SMHoldList,
-            dict(offset='offset', column='column', length='length')
-        )
-        sm.bpms = cls.cast(
-            osu.bpms, SMBpmList,
-            dict(offset='offset', bpm='bpm')
-        )
-
-        sms = SMMapSet()
-
-        sms.maps = [sm]
-
-        sms.music = osu.audio_file_name
-        sms.title = osu.title
-        sms.title_translit = osu.title_unicode
-        sms.artist = osu.artist
-        sms.artist_translit = osu.artist_unicode
-        sms.credit = osu.creator
-        sms.background = osu.background_file_name
-        sms.sample_start = osu.preview_time
-        sms.sample_length = 10
-        sms.offset = 0.0
-
-        sm.chart_type = SMMapChartTypes.get_type(osu.stack().column.max() + 1)
-
-        if raise_bad_mode and not sm.chart_type:
-            raise ValueError(
-                f"Keys {int(sm.stack().column.max() + 1)} isn't supported"
-            )
-
-        return sms
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.osu.OsuMap import OsuMap
+from reamber.sm.SMMap import SMMap
+from reamber.sm.SMMapMeta import SMMapChartTypes
+from reamber.sm.SMMapSet import SMMapSet
+from reamber.sm.lists.SMBpmList import SMBpmList
+from reamber.sm.lists.notes.SMHitList import SMHitList
+from reamber.sm.lists.notes.SMHoldList import SMHoldList
+
+
+class OsuToSM(ConvertBase):
+    @classmethod
+    def convert(cls, osu: OsuMap, raise_bad_mode: bool = True) -> SMMapSet:
+        """Converts Osu to a SMMapset Obj
+
+        Args:
+            osu: Osu Map
+            raise_bad_mode: Raises if SM can't support this key mode
+        """
+
+        sm = SMMap()
+
+        sm.hits = cls.cast(
+            osu.hits, SMHitList,
+            dict(offset='offset', column='column')
+        )
+        sm.holds = cls.cast(
+            osu.holds, SMHoldList,
+            dict(offset='offset', column='column', length='length')
+        )
+        sm.bpms = cls.cast(
+            osu.bpms, SMBpmList,
+            dict(offset='offset', bpm='bpm')
+        )
+
+        sms = SMMapSet()
+
+        sms.maps = [sm]
+
+        sms.music = osu.audio_file_name
+        sms.title = osu.title
+        sms.title_translit = osu.title_unicode
+        sms.artist = osu.artist
+        sms.artist_translit = osu.artist_unicode
+        sms.credit = osu.creator
+        sms.background = osu.background_file_name
+        sms.sample_start = osu.preview_time
+        sms.sample_length = 10
+        sms.offset = 0.0
+
+        sm.chart_type = SMMapChartTypes.get_type(osu.stack().column.max() + 1)
+
+        if raise_bad_mode and not sm.chart_type:
+            raise ValueError(
+                f"Keys {int(sm.stack().column.max() + 1)} isn't supported"
+            )
+
+        return sms
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/QuaToSM.py` & `reamber-0.1.8/reamber/algorithms/convert/QuaToSM.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.quaver.QuaMap import QuaMap
-from reamber.sm.SMMap import SMMap
-from reamber.sm.SMMapMeta import SMMapChartTypes
-from reamber.sm.SMMapSet import SMMapSet
-from reamber.sm.lists.SMBpmList import SMBpmList
-from reamber.sm.lists.notes.SMHitList import SMHitList
-from reamber.sm.lists.notes.SMHoldList import SMHoldList
-
-
-class QuaToSM(ConvertBase):
-    @classmethod
-    def convert(cls, qua: QuaMap) -> SMMapSet:
-        """Converts a Quaver map to a SMMapset Obj
-
-        Notes:
-             Each Quaver map will make a separate mapset
-        """
-
-        sm = SMMap()
-        sm.hits = cls.cast(
-            qua.hits, SMHitList,
-            dict(offset='offset', column='column')
-        )
-        sm.holds = cls.cast(
-            qua.holds, SMHoldList,
-            dict(offset='offset', column='column', length='length')
-        )
-        sm.bpms = cls.cast(
-            qua.bpms, SMBpmList,
-            dict(offset='offset', bpm='bpm')
-        )
-        sm.chart_type = SMMapChartTypes.get_type(qua.stack().column.max() + 1)
-
-        sms = SMMapSet()
-
-        sms.maps = [sm]
-
-        sms.music = qua.audio_file
-
-        sms.title = qua.title
-        sms.title_translit = qua.title
-        sms.artist = qua.artist
-        sms.artist_translit = qua.artist
-        sms.credit = qua.creator
-        sms.background = qua.background_file
-        sms.sample_start = qua.song_preview_time
-        sms.sample_length = 10
-        sms.offset = qua.stack().offset.min()
-
-        return sms
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.quaver.QuaMap import QuaMap
+from reamber.sm.SMMap import SMMap
+from reamber.sm.SMMapMeta import SMMapChartTypes
+from reamber.sm.SMMapSet import SMMapSet
+from reamber.sm.lists.SMBpmList import SMBpmList
+from reamber.sm.lists.notes.SMHitList import SMHitList
+from reamber.sm.lists.notes.SMHoldList import SMHoldList
+
+
+class QuaToSM(ConvertBase):
+    @classmethod
+    def convert(cls, qua: QuaMap) -> SMMapSet:
+        """Converts a Quaver map to a SMMapset Obj
+
+        Notes:
+             Each Quaver map will make a separate mapset
+        """
+
+        sm = SMMap()
+        sm.hits = cls.cast(
+            qua.hits, SMHitList,
+            dict(offset='offset', column='column')
+        )
+        sm.holds = cls.cast(
+            qua.holds, SMHoldList,
+            dict(offset='offset', column='column', length='length')
+        )
+        sm.bpms = cls.cast(
+            qua.bpms, SMBpmList,
+            dict(offset='offset', bpm='bpm')
+        )
+        sm.chart_type = SMMapChartTypes.get_type(qua.stack().column.max() + 1)
+
+        sms = SMMapSet()
+
+        sms.maps = [sm]
+
+        sms.music = qua.audio_file
+
+        sms.title = qua.title
+        sms.title_translit = qua.title
+        sms.artist = qua.artist
+        sms.artist_translit = qua.artist
+        sms.credit = qua.creator
+        sms.background = qua.background_file
+        sms.sample_start = qua.song_preview_time
+        sms.sample_length = 10
+        sms.offset = qua.stack().offset.min()
+
+        return sms
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/SMToBMS.py` & `reamber-0.1.8/reamber/algorithms/convert/SMToBMS.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import codecs
-from typing import List
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.bms.BMSMap import BMSMap
-from reamber.bms.lists.BMSBpmList import BMSBpmList
-from reamber.bms.lists.notes.BMSHitList import BMSHitList
-from reamber.bms.lists.notes.BMSHoldList import BMSHoldList
-from reamber.sm.SMMapSet import SMMapSet
-
-
-class SMToBMS(ConvertBase):
-    @classmethod
-    def convert(cls, sms: SMMapSet) -> List[BMSMap]:
-        """Converts a Mapset to multiple BMS maps"""
-
-        bmss: List[BMSMap] = []
-        for sm in sms:
-            bms = BMSMap()
-            bms.hits = cls.cast(
-                sm.hits, BMSHitList,
-                dict(offset='offset', column='column')
-            )
-            bms.holds = cls.cast(
-                sm.holds, BMSHoldList,
-                dict(offset='offset', column='column', length='length')
-            )
-            bms.bpms = cls.cast(
-                sm.bpms, BMSBpmList,
-                dict(offset='offset', bpm='bpm')
-            )
-
-            bms.title = codecs.encode(sms.title, encoding='shift_jis')
-            bms.artist = codecs.encode(sms.artist, encoding='shift_jis')
-            bms.version = codecs.encode(f"{sm.difficulty} {sm.difficulty_val}",
-                                        encoding='shift_jis')
-
-            bmss.append(bms)
-        return bmss
+import codecs
+from typing import List
+
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.bms.BMSMap import BMSMap
+from reamber.bms.lists.BMSBpmList import BMSBpmList
+from reamber.bms.lists.notes.BMSHitList import BMSHitList
+from reamber.bms.lists.notes.BMSHoldList import BMSHoldList
+from reamber.sm.SMMapSet import SMMapSet
+
+
+class SMToBMS(ConvertBase):
+    @classmethod
+    def convert(cls, sms: SMMapSet) -> List[BMSMap]:
+        """Converts a Mapset to multiple BMS maps"""
+
+        bmss: List[BMSMap] = []
+        for sm in sms:
+            bms = BMSMap()
+            bms.hits = cls.cast(
+                sm.hits, BMSHitList,
+                dict(offset='offset', column='column')
+            )
+            bms.holds = cls.cast(
+                sm.holds, BMSHoldList,
+                dict(offset='offset', column='column', length='length')
+            )
+            bms.bpms = cls.cast(
+                sm.bpms, BMSBpmList,
+                dict(offset='offset', bpm='bpm')
+            )
+
+            bms.title = codecs.encode(sms.title, encoding='shift_jis')
+            bms.artist = codecs.encode(sms.artist, encoding='shift_jis')
+            bms.version = codecs.encode(f"{sm.difficulty} {sm.difficulty_val}",
+                                        encoding='shift_jis')
+
+            bmss.append(bms)
+        return bmss
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/SMToQua.py` & `reamber-0.1.8/reamber/algorithms/convert/SMToQua.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from typing import List
-
-from reamber.algorithms.convert.ConvertBase import ConvertBase
-from reamber.quaver.QuaMap import QuaMap
-from reamber.quaver.QuaMapMeta import QuaMapMode
-from reamber.quaver.lists.QuaBpmList import QuaBpmList
-from reamber.quaver.lists.notes.QuaHitList import QuaHitList
-from reamber.quaver.lists.notes.QuaHoldList import QuaHoldList
-from reamber.sm.SMMapMeta import SMMapChartTypes
-from reamber.sm.SMMapSet import SMMapSet
-
-
-class SMToQua(ConvertBase):
-    @classmethod
-    def convert(cls, sms: SMMapSet, raise_bad_mode: bool = True)\
-        -> List[QuaMap]:
-        """Converts a SMMapset to possibly multiple quaver maps
-
-        Args:
-            sms: Stepmania Mapset
-            raise_bad_mode: Raises if Quaver can't support this key mode
-        """
-
-        quas: List[QuaMap] = []
-        for sm in sms:
-            qua = QuaMap()
-            qua.hits = cls.cast(sm.hits, QuaHitList,
-                                dict(offset='offset', column='column'))
-            qua.holds = cls.cast(sm.holds, QuaHoldList,
-                                 dict(offset='offset', column='column',
-                                      length='length'))
-            qua.bpms = cls.cast(sm.bpms, QuaBpmList,
-                                dict(offset='offset', bpm='bpm'))
-
-            qua.background_file = sms.background
-            qua.title = sms.title
-            qua.artist = sms.artist
-            qua.mode = QuaMapMode.get_mode(
-                int(SMMapChartTypes.get_keys(sm.chart_type)))
-            qua.audio_file = sms.music
-            qua.creator = sms.credit
-            qua.difficulty_name = f"{sm.difficulty} {sm.difficulty_val}"
-            qua.song_preview_time = int(sms.sample_start)
-            if raise_bad_mode and not qua.mode:
-                raise ValueError(
-                    f"Keys {int(sm.stack().column.max() + 1)} isn't supported."
-                )
-            quas.append(qua)
-        return quas
+from typing import List
+
+from reamber.algorithms.convert.ConvertBase import ConvertBase
+from reamber.quaver.QuaMap import QuaMap
+from reamber.quaver.QuaMapMeta import QuaMapMode
+from reamber.quaver.lists.QuaBpmList import QuaBpmList
+from reamber.quaver.lists.notes.QuaHitList import QuaHitList
+from reamber.quaver.lists.notes.QuaHoldList import QuaHoldList
+from reamber.sm.SMMapMeta import SMMapChartTypes
+from reamber.sm.SMMapSet import SMMapSet
+
+
+class SMToQua(ConvertBase):
+    @classmethod
+    def convert(cls, sms: SMMapSet, raise_bad_mode: bool = True)\
+        -> List[QuaMap]:
+        """Converts a SMMapset to possibly multiple quaver maps
+
+        Args:
+            sms: Stepmania Mapset
+            raise_bad_mode: Raises if Quaver can't support this key mode
+        """
+
+        quas: List[QuaMap] = []
+        for sm in sms:
+            qua = QuaMap()
+            qua.hits = cls.cast(sm.hits, QuaHitList,
+                                dict(offset='offset', column='column'))
+            qua.holds = cls.cast(sm.holds, QuaHoldList,
+                                 dict(offset='offset', column='column',
+                                      length='length'))
+            qua.bpms = cls.cast(sm.bpms, QuaBpmList,
+                                dict(offset='offset', bpm='bpm'))
+
+            qua.background_file = sms.background
+            qua.title = sms.title
+            qua.artist = sms.artist
+            qua.mode = QuaMapMode.get_mode(
+                int(SMMapChartTypes.get_keys(sm.chart_type)))
+            qua.audio_file = sms.music
+            qua.creator = sms.credit
+            qua.difficulty_name = f"{sm.difficulty} {sm.difficulty_val}"
+            qua.song_preview_time = int(sms.sample_start)
+            if raise_bad_mode and not qua.mode:
+                raise ValueError(
+                    f"Keys {int(sm.stack().column.max() + 1)} isn't supported."
+                )
+            quas.append(qua)
+        return quas
```

### Comparing `reamber-0.1.7/reamber/algorithms/convert/__init__.py` & `reamber-0.1.8/reamber/algorithms/convert/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from reamber.algorithms.convert.BMSToOsu import BMSToOsu
-from reamber.algorithms.convert.BMSToQua import BMSToQua
-from reamber.algorithms.convert.BMSToSM import BMSToSM
-from reamber.algorithms.convert.O2JToBMS import O2JToBMS
-from reamber.algorithms.convert.O2JToOsu import O2JToOsu
-from reamber.algorithms.convert.O2JToQua import O2JToQua
-from reamber.algorithms.convert.O2JToSM import O2JToSM
-from reamber.algorithms.convert.OsuToBMS import OsuToBMS
-from reamber.algorithms.convert.OsuToQua import OsuToQua
-from reamber.algorithms.convert.OsuToSM import OsuToSM
-from reamber.algorithms.convert.QuaToBMS import QuaToBMS
-from reamber.algorithms.convert.QuaToOsu import QuaToOsu
-from reamber.algorithms.convert.QuaToSM import QuaToSM
-from reamber.algorithms.convert.SMToBMS import SMToBMS
-from reamber.algorithms.convert.SMToOsu import SMToOsu
-from reamber.algorithms.convert.SMToQua import SMToQua
-
-__all__ = [
-    "BMSToOsu",
-    "BMSToQua",
-    "BMSToSM",
-    "O2JToOsu",
-    "O2JToQua",
-    "O2JToSM",
-    "O2JToBMS",
-    "OsuToBMS",
-    "OsuToQua",
-    "OsuToSM",
-    "QuaToBMS",
-    "QuaToOsu",
-    "QuaToSM",
-    "SMToBMS",
-    "SMToOsu",
-    "SMToQua",
-]
+from reamber.algorithms.convert.BMSToOsu import BMSToOsu
+from reamber.algorithms.convert.BMSToQua import BMSToQua
+from reamber.algorithms.convert.BMSToSM import BMSToSM
+from reamber.algorithms.convert.O2JToBMS import O2JToBMS
+from reamber.algorithms.convert.O2JToOsu import O2JToOsu
+from reamber.algorithms.convert.O2JToQua import O2JToQua
+from reamber.algorithms.convert.O2JToSM import O2JToSM
+from reamber.algorithms.convert.OsuToBMS import OsuToBMS
+from reamber.algorithms.convert.OsuToQua import OsuToQua
+from reamber.algorithms.convert.OsuToSM import OsuToSM
+from reamber.algorithms.convert.QuaToBMS import QuaToBMS
+from reamber.algorithms.convert.QuaToOsu import QuaToOsu
+from reamber.algorithms.convert.QuaToSM import QuaToSM
+from reamber.algorithms.convert.SMToBMS import SMToBMS
+from reamber.algorithms.convert.SMToOsu import SMToOsu
+from reamber.algorithms.convert.SMToQua import SMToQua
+
+__all__ = [
+    "BMSToOsu",
+    "BMSToQua",
+    "BMSToSM",
+    "O2JToOsu",
+    "O2JToQua",
+    "O2JToSM",
+    "O2JToBMS",
+    "OsuToBMS",
+    "OsuToQua",
+    "OsuToSM",
+    "QuaToBMS",
+    "QuaToOsu",
+    "QuaToSM",
+    "SMToBMS",
+    "SMToOsu",
+    "SMToQua",
+]
```

### Comparing `reamber-0.1.7/reamber/algorithms/generate/full_ln.py` & `reamber-0.1.8/reamber/algorithms/generate/full_ln.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-from typing import TypeVar
-
-import numpy as np
-
-from reamber.base.Map import Map
-from reamber.base.lists.notes.HitList import HitList
-from reamber.base.lists.notes.HoldList import HoldList
-
-MapType = TypeVar('MapType', bound=Map)
-
-
-def full_ln(m: MapType,
-            gap: float = 150,
-            ln_as_hit_thres: float = 100) -> MapType:
-    """ Makes map Full LN
-
-    Args:
-        m: Map to make Full LN
-        gap: Gap between a HoldTail and the next Note
-        ln_as_hit_thres: Threshold before an ln is converted to a hit.
-    """
-
-    m = m.deepcopy()
-    df = m.stack((HitList, HoldList))._stacked
-    dfgs = df.loc[:, ['offset', 'column', 'length']] \
-        .sort_values(['offset']).groupby('column')
-
-    holds = []
-    hits = []
-    # For each column, we populate self.hits and holds for from_dict init.
-    for _, dfg in dfgs:
-        dfg['diff'] = dfg['offset'].diff().shift(-1)
-
-        for offset, column, length, diff in dfg.itertuples(index=False):
-            inv_length = diff - gap
-            if np.isnan(diff):
-                if np.isnan(length):
-                    hits.append(dict(offset=offset, column=column))
-                else:
-                    holds.append(dict(
-                        offset=offset, column=column, length=length
-                    ))
-                continue
-            if inv_length >= ln_as_hit_thres:
-                holds.append(dict(
-                    offset=offset, column=column, length=inv_length
-                ))
-            else:
-                hits.append(dict(offset=offset, column=column))
-
-    m.hits = type(m.hits).from_dict(hits)
-    m.holds = type(m.holds).from_dict(holds)
-    return m
+from typing import TypeVar
+
+import numpy as np
+
+from reamber.base.Map import Map
+from reamber.base.lists.notes.HitList import HitList
+from reamber.base.lists.notes.HoldList import HoldList
+
+MapType = TypeVar('MapType', bound=Map)
+
+
+def full_ln(m: MapType,
+            gap: float = 150,
+            ln_as_hit_thres: float = 100) -> MapType:
+    """ Makes map Full LN
+
+    Args:
+        m: Map to make Full LN
+        gap: Gap between a HoldTail and the next Note
+        ln_as_hit_thres: Threshold before an ln is converted to a hit.
+    """
+
+    m = m.deepcopy()
+    df = m.stack((HitList, HoldList))._stacked
+    dfgs = df.loc[:, ['offset', 'column', 'length']] \
+        .sort_values(['offset']).groupby('column')
+
+    holds = []
+    hits = []
+    # For each column, we populate self.hits and holds for from_dict init.
+    for _, dfg in dfgs:
+        dfg['diff'] = dfg['offset'].diff().shift(-1)
+
+        for offset, column, length, diff in dfg.itertuples(index=False):
+            inv_length = diff - gap
+            if np.isnan(diff):
+                if np.isnan(length):
+                    hits.append(dict(offset=offset, column=column))
+                else:
+                    holds.append(dict(
+                        offset=offset, column=column, length=length
+                    ))
+                continue
+            if inv_length >= ln_as_hit_thres:
+                holds.append(dict(
+                    offset=offset, column=column, length=inv_length
+                ))
+            else:
+                hits.append(dict(offset=offset, column=column))
+
+    m.hits = type(m.hits).from_dict(hits)
+    m.holds = type(m.holds).from_dict(holds)
+    return m
```

### Comparing `reamber-0.1.7/reamber/algorithms/osu/hitsound_copy.py` & `reamber-0.1.8/reamber/algorithms/osu/hitsound_copy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,153 +1,145 @@
-import logging
-from copy import deepcopy
-
-import numpy as np
-import pandas as pd
-
-from reamber.osu.OsuMap import OsuMap
-from reamber.osu.OsuSample import OsuSample
-
-log = logging.getLogger(__name__)
-
-
-def hitsound_copy(m_from: OsuMap, m_to: OsuMap,
-                  inplace: bool = False) -> OsuMap:
-    """Copies the hitsound from mFrom to mTo
-
-    Args:
-        inplace: Whether to just modify this instance or return a modified copy
-        m_from: The map you want to copy from
-        m_to: The map you want to copy to, it doesn't mutate this.
-    :return: A copy of mTo with the copied hitsounds.
-    """
-    df_from = pd.concat([i.df for i in m_from.notes], sort=False)
-    df_from = df_from.drop(['column', 'length'], axis='columns',
-                           errors='ignore')
-    df_from = df_from[(df_from['addition_set'] != 0) |
-                      (df_from['custom_set'] != 0) |
-                      (df_from['hitsound_set'] != 0) |
-                      (df_from['sample_set'] != 0) |
-                      (df_from['hitsound_file'] != "")]
-    df_from: pd.DataFrame
-    df_from = df_from.sort_values('offset').reset_index(drop=True)
-
-    HITSOUND_CLAP = 2
-    HITSOUND_FINISH = 4
-    HITSOUND_WHISTLE = 8
-
-    # Before we group, we want to split the hitsound_file to clap,
-    # finish and whistle (2, 4, 8)
-    df_from['hitsound_clap'] \
-        = np.where(df_from['hitsound_set'] & HITSOUND_CLAP == HITSOUND_CLAP,
-                   HITSOUND_CLAP, 0)
-    df_from['hitsound_finish'] \
-        = np.where(
-        df_from['hitsound_set'] & HITSOUND_FINISH == HITSOUND_FINISH,
-        HITSOUND_FINISH, 0)
-    df_from['hitsound_whistle'] \
-        = np.where(
-        df_from['hitsound_set'] & HITSOUND_WHISTLE == HITSOUND_WHISTLE,
-        HITSOUND_WHISTLE, 0)
-
-    df_from = df_from.drop('hitsound_set', axis='columns')
-    df_from = df_from.groupby('offset')
-
-    # We'll just get the mTo data then export it again
-    df = pd.concat([i.df for i in m_to.notes], sort=False)
-    df = df.sort_values('offset').reset_index(drop=True)
-    df_to_offsets = df['offset']
-
-    # We grab a deepCopy if not inplace
-    m_to_copy = m_to if inplace else deepcopy(m_to)
-    m_to_copy.reset_samples()
-
-    # The idea is to loop through unique offsets
-    # where there's hitsounds/samples
-    # For each offset, we group by the volume,
-    # because we can snap multiple default samples if we just specify 1 volume
-
-    # e.g. < (C)lap (F)inish (W)histle >
-    # C F W  Vol | C F W  Vol
-    # 1 0 0  20  | 1 1 1  20
-    # 0 1 0  20  | 1 0 0  30
-    # 0 0 1  20  | 0 1 1  40
-    # 1 0 0  30  | CUSTOM 20
-    # 0 1 1  40  |
-    # CUSTOM 20  |
-
-    for offset, offset_group in df_from:
-        # You cannot have hitsound Files and the default hitsounds together
-        # We find out which indexes match on the df we want to copy to
-        slot_indexes = list(
-            (df_to_offsets == offset)[df_to_offsets == offset].index)
-        slot = 0  # Indicates the snap on "TO" we're looking at right now
-        slot_max = len(slot_indexes)  # The maximum slots
-
-        offset_group: pd.DataFrame
-        v_groups = offset_group.groupby('volume', as_index=False) \
-            .agg({'hitsound_file': ';'.join,
-                  'hitsound_clap': 'sum',
-                  'hitsound_finish': 'sum',
-                  'hitsound_whistle': 'sum'})
-        v_groups: pd.DataFrame
-
-        for _, v_group in v_groups.iterrows():  # v_group -> Volume Group
-            volume = v_group['volume']
-            claps = int(v_group['hitsound_clap'] / HITSOUND_CLAP)
-            finishes = int(v_group['hitsound_finish'] / HITSOUND_FINISH)
-            whistles = int(v_group['hitsound_whistle'] / HITSOUND_WHISTLE)
-            hitsound_files = [file for file in
-                              v_group['hitsound_file'].split(';') if
-                              len(file) > 0]
-
-            samples = max(claps, finishes, whistles)
-            for _ in range(samples):
-                # We loop through the default C F W samples here
-                if slot == slot_max:
-                    log.debug(
-                        f"No snap to place hitsound {slot} > {slot_max}, "
-                        f"dropping hitsound at {offset}"
-                    )
-                    break
-
-                val = 0
-                if claps:
-                    claps -= 1
-                    val += HITSOUND_CLAP
-                if finishes:
-                    finishes -= 1
-                    val += HITSOUND_FINISH
-                if whistles:
-                    whistles -= 1
-                    val += HITSOUND_WHISTLE
-
-                log.debug(f"Slotted Hitsound {val} at {offset} vol {volume}")
-                df.at[slot_indexes[slot], 'hitsound_set'] = val
-                df.at[
-                    slot_indexes[slot], 'volume'] = volume if volume > 0 else 0
-                slot += 1
-
-            for file in hitsound_files:
-                # We loop through the custom sample here
-                if slot == slot_max:
-                    log.debug(
-                        f"No snap to place hitsound {slot} > {slot_max}, "
-                        f"sampling {file} at {offset}"
-                    )
-                    m_to_copy.samples = m_to_copy.samples.append(
-                        OsuSample(offset=offset, sample_file=file,
-                                  volume=volume))
-                    break
-                log.debug(f"Slotted Hitsound {file} at {offset} vol {volume}")
-                df.at[slot_indexes[slot], 'hitsound_file'] = file
-                df.at[
-                    slot_indexes[slot], 'volume'] = volume if volume > 0 else 0
-                slot += 1
-
-    if 'length' in df:
-        m_to_copy.holds.df = df[~np.isnan(df.length)]
-        m_to_copy.hits.df = df[np.isnan(df.length)].drop('length', axis=1)
-    else:
-        m_to_copy.hits.df = df
-
-    return None if inplace else m_to_copy
+import logging
+from copy import deepcopy
+
+import numpy as np
+import pandas as pd
+
+from reamber.osu.OsuMap import OsuMap
+from reamber.osu.OsuSample import OsuSample
+
+log = logging.getLogger(__name__)
+
+
+def hitsound_copy(osu_src: OsuMap, osu_tgt: OsuMap) -> OsuMap:
+    """ Copies the hitsound from source to target
+
+    Args:
+        osu_src: The map you want to copy from
+        osu_tgt: The map you want to copy to, it doesn't mutate this.
+
+    Returns:
+         A copy of target with the copied hitsounds.
+    """
+    df_src = pd.concat([i.df for i in osu_src.notes], sort=False)
+    df_src = df_src.drop(['column', 'length'], axis='columns', errors='ignore')
+    df_src = df_src[(df_src['addition_set'] != 0) |
+                    (df_src['custom_set'] != 0) |
+                    (df_src['hitsound_set'] != 0) |
+                    (df_src['sample_set'] != 0) |
+                    (df_src['hitsound_file'] != "")]
+    df_src: pd.DataFrame
+    df_src = df_src.sort_values('offset').reset_index(drop=True)
+
+    HS_CLAP = 2
+    HS_FINISH = 4
+    HS_WHISTLE = 8
+
+    # Before we group, we want to split the hitsound_file to clap,
+    # finish and whistle (2, 4, 8)
+    df_src['hitsound_clap'] \
+        = np.where(df_src['hitsound_set'] & HS_CLAP == HS_CLAP, HS_CLAP, 0)
+    df_src['hitsound_finish'] \
+        = np.where(df_src['hitsound_set'] & HS_FINISH == HS_FINISH, HS_FINISH, 0)
+    df_src['hitsound_whistle'] \
+        = np.where(df_src['hitsound_set'] & HS_WHISTLE == HS_WHISTLE, HS_WHISTLE, 0)
+
+    df_src = df_src.drop('hitsound_set', axis='columns')
+    df_src = df_src.groupby('offset')
+
+    # We'll just get the target data then export it again
+    df = pd.concat([i.df for i in osu_tgt.notes], sort=False)
+    df = df.sort_values('offset').reset_index(drop=True)
+    df_to_offsets = df['offset']
+
+    osu_tgt = deepcopy(osu_tgt)
+    osu_tgt.reset_samples()
+
+    # The idea is to loop through unique offsets
+    # where there's hitsounds/samples
+    # For each offset, we group by the volume,
+    # because we can snap multiple default samples if we just specify 1 volume
+
+    # e.g. < (C)lap (F)inish (W)histle >
+    # C F W  Vol | C F W  Vol
+    # 1 0 0  20  | 1 1 1  20
+    # 0 1 0  20  | 1 0 0  30
+    # 0 0 1  20  | 0 1 1  40
+    # 1 0 0  30  | CUSTOM 20
+    # 0 1 1  40  |
+    # CUSTOM 20  |
+
+    for offset, offset_group in df_src:
+        # You cannot have hitsound Files and the default hitsounds together
+        # We find out which indexes match on the df we want to copy to
+        slot_indexes = list(
+            (df_to_offsets == offset)[df_to_offsets == offset].index)
+        slot = 0  # Indicates the snap on "TO" we're looking at right now
+        slot_max = len(slot_indexes)  # The maximum slots
+
+        offset_group: pd.DataFrame
+        v_groups = offset_group.groupby('volume', as_index=False) \
+            .agg({'hitsound_file': ';'.join,
+                  'hitsound_clap': 'sum',
+                  'hitsound_finish': 'sum',
+                  'hitsound_whistle': 'sum'})
+        v_groups: pd.DataFrame
+
+        for _, v_group in v_groups.iterrows():  # v_group -> Volume Group
+            volume = v_group['volume']
+            claps = int(v_group['hitsound_clap'] / HS_CLAP)
+            finishes = int(v_group['hitsound_finish'] / HS_FINISH)
+            whistles = int(v_group['hitsound_whistle'] / HS_WHISTLE)
+            hitsound_files = [file for file in
+                              v_group['hitsound_file'].split(';') if
+                              len(file) > 0]
+
+            samples = max(claps, finishes, whistles)
+            for _ in range(samples):
+                # We loop through the default C F W samples here
+                if slot == slot_max:
+                    log.debug(
+                        f"No snap to place hitsound {slot} > {slot_max}, "
+                        f"dropping hitsound at {offset}"
+                    )
+                    break
+
+                val = 0
+                if claps:
+                    claps -= 1
+                    val += HS_CLAP
+                if finishes:
+                    finishes -= 1
+                    val += HS_FINISH
+                if whistles:
+                    whistles -= 1
+                    val += HS_WHISTLE
+
+                log.debug(f"Slotted Hitsound {val} at {offset} vol {volume}")
+                df.at[slot_indexes[slot], 'hitsound_set'] = val
+                df.at[slot_indexes[slot], 'volume'] = volume if volume > 0 else 0
+                slot += 1
+
+            for file in hitsound_files:
+                # We loop through the custom sample here
+                if slot == slot_max:
+                    log.debug(
+                        f"No snap to place hitsound {slot} > {slot_max}, "
+                        f"sampling {file} at {offset}"
+                    )
+                    osu_tgt.samples = osu_tgt.samples.append(
+                        OsuSample(offset=offset, sample_file=file,
+                                  volume=volume))
+                    break
+                log.debug(f"Slotted Hitsound {file} at {offset} vol {volume}")
+                df.at[slot_indexes[slot], 'hitsound_file'] = file
+                df.at[slot_indexes[slot], 'volume'] = volume if volume > 0 else 0
+                slot += 1
+
+    if 'length' in df:
+        osu_tgt.holds.df = df[~np.isnan(df.length)]
+        osu_tgt.hits.df = df[np.isnan(df.length)].drop('length', axis=1)
+    else:
+        # Unsure if this is replicable, however, we'll just leave it as is
+        osu_tgt.hits.df = df
+
+    return osu_tgt
```

### Comparing `reamber-0.1.7/reamber/algorithms/pattern/Pattern.py` & `reamber-0.1.8/reamber/algorithms/pattern/Pattern.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,174 +1,174 @@
-from __future__ import annotations
-
-from bisect import bisect_left, bisect_right
-from typing import List, Type
-
-import numpy as np
-import pandas as pd
-
-from reamber.base.Hold import Hold, HoldTail
-from reamber.base.lists.notes import HoldList
-from reamber.base.lists.notes.NoteList import NoteList
-
-
-class Pattern:
-    def __init__(self,
-                 cols: List[int],
-                 offsets: List[float],
-                 types: List[Type]):
-        """Initializes the Pattern structure
-
-        Examples:
-
-            ``type`` is a singular object type like ``OsuHit``, ``QuaHold``.
-
-            The end of an LN must be ``HoldTail``.
-
-            >>> from reamber.base.Hit import Hit
-            ... from reamber.base.Hold import Hold, HoldTail
-            ... columns = [0, 1, 1, 2, 2, 3]
-            ... offsets = [0, 0, 100, 100, 200, 200]
-            ... types = [Hit, Hit, Hit, Hold, HoldTail, Hit]
-            ... p = Pattern(columns, offsets, types)
-        """
-
-        self.df = pd.DataFrame(
-            {'column': cols, 'offset': offsets, 'type': types}
-        ).sort_values('offset', ignore_index=True)
-
-    @staticmethod
-    def from_note_lists(note_lists: List[NoteList],
-                        include_tails: bool = True) -> Pattern:
-        """Creates a Pattern Class from a List of Note Lists
-
-        Args:
-            note_lists: Note Lists to add, E.g. QuaHitList, BMSHoldList
-            include_tails: Whether to include tails in pattern discovery
-
-        Notes:
-            You can create it from any subclass of a NoteList,
-
-        Examples:
-            >>> from reamber.osu.OsuMap import OsuMap
-            >>> m = OsuMap.read_file(...)
-            >>> p = Pattern.from_note_lists([m.hits, m.holds])
-        """
-
-        note_lists = filter(lambda x: len(x) > 0, note_lists)
-        cols: List[int] = []
-        offsets: List[float] = []
-        types: List[type] = []
-
-        for nl in note_lists:
-            count: int = len(nl)
-
-            nl_type: type = type(nl[0])
-            nl_cols: List[int] = nl.column.tolist()
-            nl_offsets: List[float] = nl.offset.tolist()
-
-            cols.extend(nl_cols)
-            offsets.extend(nl_offsets)
-            types.extend([nl_type, ] * count)
-
-            if include_tails and issubclass(nl_type, Hold):
-                nl: HoldList
-                cols.extend(nl_cols)
-                offsets.extend(nl.tail_offset)
-                types.extend([HoldTail, ] * count)
-
-        return Pattern(cols=cols, offsets=offsets, types=types)
-
-    def __len__(self):
-        return len(self.df)
-
-    def group(self,
-              v_window: float = 50.0,
-              h_window: None | int = None,
-              avoid_jack=True) -> List[np.ndarray]:
-        """Groups the package horizontally and vertically
-
-        Notes:
-            Having a large v_window causes overlapping groups.
-
-        Args:
-            v_window: Vertical Window to check (Offsets)
-            h_window: Horizontal Window to check (Columns).
-                If None, all columns will be grouped.
-            avoid_jack: Whether a group can have duplicate columns.
-        """
-
-        if v_window < 0:
-            raise ValueError("Vertical Window cannot be negative")
-
-        if h_window is not None and h_window < 0:
-            raise ValueError("Horizontal Window cannot be negative, "
-                             "use None to group all columns.")
-
-        # The objects already in a group
-        is_grouped = np.zeros(len(self), dtype=bool)
-        df_groups = []
-
-        ar = self.df.to_records(index=False)
-
-        for ix, col, offset, *_ in self.df.itertuples():
-            if is_grouped[ix]: continue  # Skip all children of a group
-
-            ar_ungrouped = ar[~is_grouped]
-            mask = self.v_mask(ar_ungrouped, offset, v_window, avoid_jack)
-            if h_window is not None:
-                mask &= self.h_mask(ar_ungrouped, col, h_window)
-
-            # Mark current group as grouped
-            # Mask is a subset of all False in is_grouped, we select all False
-            #  from is_grouped
-            is_grouped[~is_grouped] |= mask
-            df_groups.append(ar_ungrouped[mask])
-
-        return df_groups
-
-    @staticmethod
-    def v_mask(ar: np.ndarray, offset: int, v_window: float,
-               avoid_jack: bool) -> np.ndarray:
-        """Get filtered vertical mask of offset
-
-        Args:
-            ar: np.ndarray to mask
-            offset: The reference offset to scan from
-            v_window: The size of the scan
-            avoid_jack: Whether to avoid repeated columns in the mask
-        """
-        offsets = ar['offset']
-        cols = ar['column'].tolist()
-        mask = np.zeros(len(ar), dtype=bool)
-
-        # Look for objects in [offset, offset + v_window]
-
-        start = bisect_left(offsets, offset)
-        end = bisect_right(offsets, offset + v_window, lo=start)
-
-        if start != end:
-            if avoid_jack:
-                # To avoid jacks, a column appears only once
-                # Take 1st occurrence and discard the rest
-                cols_ = cols[start:end]
-                mask_ixs = np.array([cols_.index(i) for i in set(cols_)]) \
-                           + start
-                mask[mask_ixs] = True
-            else:
-                mask[start:end] = True
-        return mask
-
-    @staticmethod
-    def h_mask(ar: np.ndarray, column: int, h_window: int) -> np.ndarray:
-        """Get the filtered horizontal mask of column
-
-        Args:
-            ar: np.ndarray to mask
-            column: Column reference
-            h_window: Size of horizontal window
-        """
-
-        mask = np.zeros(len(ar), bool)
-        mask[abs(column - ar['column']) <= h_window] = True
-
-        return mask
+from __future__ import annotations
+
+from bisect import bisect_left, bisect_right
+from typing import List, Type
+
+import numpy as np
+import pandas as pd
+
+from reamber.base.Hold import Hold, HoldTail
+from reamber.base.lists.notes import HoldList
+from reamber.base.lists.notes.NoteList import NoteList
+
+
+class Pattern:
+    def __init__(self,
+                 cols: List[int],
+                 offsets: List[float],
+                 types: List[Type]):
+        """Initializes the Pattern structure
+
+        Examples:
+
+            ``type`` is a singular object type like ``OsuHit``, ``QuaHold``.
+
+            The end of an LN must be ``HoldTail``.
+
+            >>> from reamber.base.Hit import Hit
+            ... from reamber.base.Hold import Hold, HoldTail
+            ... columns = [0, 1, 1, 2, 2, 3]
+            ... offsets = [0, 0, 100, 100, 200, 200]
+            ... types = [Hit, Hit, Hit, Hold, HoldTail, Hit]
+            ... p = Pattern(columns, offsets, types)
+        """
+
+        self.df = pd.DataFrame(
+            {'column': cols, 'offset': offsets, 'type': types}
+        ).sort_values('offset', ignore_index=True)
+
+    @staticmethod
+    def from_note_lists(note_lists: List[NoteList],
+                        include_tails: bool = True) -> Pattern:
+        """Creates a Pattern Class from a List of Note Lists
+
+        Args:
+            note_lists: Note Lists to add, E.g. QuaHitList, BMSHoldList
+            include_tails: Whether to include tails in pattern discovery
+
+        Notes:
+            You can create it from any subclass of a NoteList,
+
+        Examples:
+            >>> from reamber.osu.OsuMap import OsuMap
+            >>> m = OsuMap.read_file(...)
+            >>> p = Pattern.from_note_lists([m.hits, m.holds])
+        """
+
+        note_lists = filter(lambda x: len(x) > 0, note_lists)
+        cols: List[int] = []
+        offsets: List[float] = []
+        types: List[type] = []
+
+        for nl in note_lists:
+            count: int = len(nl)
+
+            nl_type: type = type(nl[0])
+            nl_cols: List[int] = nl.column.tolist()
+            nl_offsets: List[float] = nl.offset.tolist()
+
+            cols.extend(nl_cols)
+            offsets.extend(nl_offsets)
+            types.extend([nl_type, ] * count)
+
+            if include_tails and issubclass(nl_type, Hold):
+                nl: HoldList
+                cols.extend(nl_cols)
+                offsets.extend(nl.tail_offset)
+                types.extend([HoldTail, ] * count)
+
+        return Pattern(cols=cols, offsets=offsets, types=types)
+
+    def __len__(self):
+        return len(self.df)
+
+    def group(self,
+              v_window: float = 50.0,
+              h_window: None | int = None,
+              avoid_jack=True) -> List[np.ndarray]:
+        """Groups the package horizontally and vertically
+
+        Notes:
+            Having a large v_window causes overlapping groups.
+
+        Args:
+            v_window: Vertical Window to check (Offsets)
+            h_window: Horizontal Window to check (Columns).
+                If None, all columns will be grouped.
+            avoid_jack: Whether a group can have duplicate columns.
+        """
+
+        if v_window < 0:
+            raise ValueError("Vertical Window cannot be negative")
+
+        if h_window is not None and h_window < 0:
+            raise ValueError("Horizontal Window cannot be negative, "
+                             "use None to group all columns.")
+
+        # The objects already in a group
+        is_grouped = np.zeros(len(self), dtype=bool)
+        df_groups = []
+
+        ar = self.df.to_records(index=False)
+
+        for ix, col, offset, *_ in self.df.itertuples():
+            if is_grouped[ix]: continue  # Skip all children of a group
+
+            ar_ungrouped = ar[~is_grouped]
+            mask = self.v_mask(ar_ungrouped, offset, v_window, avoid_jack)
+            if h_window is not None:
+                mask &= self.h_mask(ar_ungrouped, col, h_window)
+
+            # Mark current group as grouped
+            # Mask is a subset of all False in is_grouped, we select all False
+            #  from is_grouped
+            is_grouped[~is_grouped] |= mask
+            df_groups.append(ar_ungrouped[mask])
+
+        return df_groups
+
+    @staticmethod
+    def v_mask(ar: np.ndarray, offset: int, v_window: float,
+               avoid_jack: bool) -> np.ndarray:
+        """Get filtered vertical mask of offset
+
+        Args:
+            ar: np.ndarray to mask
+            offset: The reference offset to scan from
+            v_window: The size of the scan
+            avoid_jack: Whether to avoid repeated columns in the mask
+        """
+        offsets = ar['offset']
+        cols = ar['column'].tolist()
+        mask = np.zeros(len(ar), dtype=bool)
+
+        # Look for objects in [offset, offset + v_window]
+
+        start = bisect_left(offsets, offset)
+        end = bisect_right(offsets, offset + v_window, lo=start)
+
+        if start != end:
+            if avoid_jack:
+                # To avoid jacks, a column appears only once
+                # Take 1st occurrence and discard the rest
+                cols_ = cols[start:end]
+                mask_ixs = np.array([cols_.index(i) for i in set(cols_)]) \
+                           + start
+                mask[mask_ixs] = True
+            else:
+                mask[start:end] = True
+        return mask
+
+    @staticmethod
+    def h_mask(ar: np.ndarray, column: int, h_window: int) -> np.ndarray:
+        """Get the filtered horizontal mask of column
+
+        Args:
+            ar: np.ndarray to mask
+            column: Column reference
+            h_window: Size of horizontal window
+        """
+
+        mask = np.zeros(len(ar), bool)
+        mask[abs(column - ar['column']) <= h_window] = True
+
+        return mask
```

### Comparing `reamber-0.1.7/reamber/algorithms/pattern/combos/PtnCombo.py` & `reamber-0.1.8/reamber/algorithms/pattern/combos/PtnCombo.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import List, Callable
-
-import numpy as np
-from numpy.lib.stride_tricks import sliding_window_view
-
-from reamber.algorithms.pattern.combos._PtnCChordStream import _PtnCChordStream
-from reamber.algorithms.pattern.combos._PtnCJack import _PtnCJack
-
-
-@dataclass
-class PtnCombo(_PtnCChordStream,
-               _PtnCJack):
-    groups: List[np.ndarray] = field(default_factory=lambda: [])
-
-    def combinations(
-        self, size=2, make_size2=False,
-        chord_filter: Callable[[np.ndarray], bool] = None,
-        combo_filter: Callable[[np.ndarray], np.ndarray[bool]] = None,
-        type_filter: Callable[[np.ndarray], np.ndarray[bool]] = None
-    ) -> List[np.ndarray]:
-        """Gets all combinations of n-size groups with filters
-
-        Args:
-            size: The size of each combination.
-            make_size2: Whether to fold any size > 2 combinations into pairs
-            chord_filter: A chord size filter. Can be generated from
-                PtnFilterChord.filter
-            combo_filter: A combination filter. Can be generated from
-                PtnFilterCombo.filter
-            type_filter: A type filter. Can be generated from
-                PtnFilterType.filter"""
-
-        # Chunks are groups of groups
-        chunks = []
-
-        for i, j in zip(
-            range(0, len(self.groups) - size + 1),  # [0, Groups - Size]
-            range(size, len(self.groups) + 1)  # [Size, Groups]
-        ):
-            chunk = self.groups[i:j]
-
-            if (
-                chord_filter is None or
-                chord_filter(np.array([i.shape[0] for i in chunk]))
-            ):
-                chunks.append(chunk)
-
-        combo_list: List = []
-
-        for chunk in chunks:
-            # This gets all combinations of the list of groups in the chunk
-            combos = np.asarray(np.meshgrid(*chunk)).T.reshape(-1, size)
-            if combo_filter: combos = combos[combo_filter(combos['column'])]
-            if type_filter:  combos = combos[type_filter(combos['type'])]
-
-            combo_list.append(combos)
-
-        combo_list = [_ for _ in combo_list if _.size != 0]
-        if make_size2:
-            return [sliding_window_view(ar, [ar.shape[0], 2]).reshape(-1, 2)
-                    for ar in combo_list]
-        else:
-            return combo_list
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import List, Callable
+
+import numpy as np
+from numpy.lib.stride_tricks import sliding_window_view
+
+from reamber.algorithms.pattern.combos._PtnCChordStream import _PtnCChordStream
+from reamber.algorithms.pattern.combos._PtnCJack import _PtnCJack
+
+
+@dataclass
+class PtnCombo(_PtnCChordStream,
+               _PtnCJack):
+    groups: List[np.ndarray] = field(default_factory=lambda: [])
+
+    def combinations(
+        self, size=2, make_size2=False,
+        chord_filter: Callable[[np.ndarray], bool] = None,
+        combo_filter: Callable[[np.ndarray], np.ndarray[bool]] = None,
+        type_filter: Callable[[np.ndarray], np.ndarray[bool]] = None
+    ) -> List[np.ndarray]:
+        """Gets all combinations of n-size groups with filters
+
+        Args:
+            size: The size of each combination.
+            make_size2: Whether to fold any size > 2 combinations into pairs
+            chord_filter: A chord size filter. Can be generated from
+                PtnFilterChord.filter
+            combo_filter: A combination filter. Can be generated from
+                PtnFilterCombo.filter
+            type_filter: A type filter. Can be generated from
+                PtnFilterType.filter"""
+
+        # Chunks are groups of groups
+        chunks = []
+
+        for i, j in zip(
+            range(0, len(self.groups) - size + 1),  # [0, Groups - Size]
+            range(size, len(self.groups) + 1)  # [Size, Groups]
+        ):
+            chunk = self.groups[i:j]
+
+            if (
+                chord_filter is None or
+                chord_filter(np.array([i.shape[0] for i in chunk]))
+            ):
+                chunks.append(chunk)
+
+        combo_list: List = []
+
+        for chunk in chunks:
+            # This gets all combinations of the list of groups in the chunk
+            combos = np.asarray(np.meshgrid(*chunk)).T.reshape(-1, size)
+            if combo_filter: combos = combos[combo_filter(combos['column'])]
+            if type_filter:  combos = combos[type_filter(combos['type'])]
+
+            combo_list.append(combos)
+
+        combo_list = [_ for _ in combo_list if _.size != 0]
+        if make_size2:
+            return [sliding_window_view(ar, [ar.shape[0], 2]).reshape(-1, 2)
+                    for ar in combo_list]
+        else:
+            return combo_list
```

### Comparing `reamber-0.1.7/reamber/algorithms/pattern/combos/_PtnCChordStream.py` & `reamber-0.1.8/reamber/algorithms/pattern/combos/_PtnCChordStream.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-from __future__ import annotations
-
-from abc import abstractmethod
-from typing import TYPE_CHECKING, List
-
-import numpy as np
-
-from reamber.algorithms.pattern.filters.PtnFilter import PtnFilterType, \
-    PtnFilterCombo, PtnFilterChord
-from reamber.base.Hold import HoldTail
-
-if TYPE_CHECKING:
-    from reamber.algorithms.pattern.combos import PtnCombo
-
-
-class _PtnCChordStream:
-    """Fragment of PtnCombo"""
-
-    @abstractmethod
-    def combinations(self, *args, **kwargs): ...
-
-    def template_chord_stream(self: 'PtnCombo',
-                              primary: int, secondary: int,
-                              keys: int,
-                              and_lower: bool = False,
-                              include_jack: bool = False) -> List[np.ndarray]:
-        """A template for chordstream filtering
-
-        Notes:
-            Primary & Secondary are the size of each chord.
-            Jacks are automatically excluded unless specified.
-
-            All chord sizes below it are also included if ``andBelow is True``
-
-        Examples:
-            a Jumpstream has ``primary=2, secondary=1``
-
-            a Handstream detection can use
-            - ``primary=3, secondary=2, and_lower=True``.
-
-            and_lower implies accepting
-            - ``primary=2, secondary=2``
-            - ``primary=2, secondary=1``,
-            - ``primary=1, secondary=1``.
-
-        Args:
-            primary: The primary chord size for each chord stream.
-            secondary: The secondary chord size for each chord stream.
-            keys: The keys of the map, used to detect pattern limits.
-            and_lower: Whether to include lower size chords or not
-            include_jack: Whether to include jackstreams or not
-        """
-
-        return self.combinations(
-            size=2,
-            make_size2=True,
-            chord_filter=PtnFilterChord.create(
-                [[primary, secondary]], keys=keys,
-                options=PtnFilterChord.Option.ANY_ORDER |
-                        PtnFilterChord.Option.AND_LOWER if and_lower else 0,
-                exclude=False
-            ).filter,
-            combo_filter=PtnFilterCombo.create(
-                [[0, 0]], keys=keys,
-                options=PtnFilterCombo.Option.REPEAT,
-                exclude=True).filter if not include_jack else None,
-            type_filter=PtnFilterType.create(
-                [[HoldTail, object]],
-                options=PtnFilterType.Option.ANY_ORDER,
-                exclude=True
-            ).filter
-        )
+from __future__ import annotations
+
+from abc import abstractmethod
+from typing import TYPE_CHECKING, List
+
+import numpy as np
+
+from reamber.algorithms.pattern.filters.PtnFilter import PtnFilterType, \
+    PtnFilterCombo, PtnFilterChord
+from reamber.base.Hold import HoldTail
+
+if TYPE_CHECKING:
+    from reamber.algorithms.pattern.combos import PtnCombo
+
+
+class _PtnCChordStream:
+    """Fragment of PtnCombo"""
+
+    @abstractmethod
+    def combinations(self, *args, **kwargs): ...
+
+    def template_chord_stream(self: 'PtnCombo',
+                              primary: int, secondary: int,
+                              keys: int,
+                              and_lower: bool = False,
+                              include_jack: bool = False) -> List[np.ndarray]:
+        """A template for chordstream filtering
+
+        Notes:
+            Primary & Secondary are the size of each chord.
+            Jacks are automatically excluded unless specified.
+
+            All chord sizes below it are also included if ``andBelow is True``
+
+        Examples:
+            a Jumpstream has ``primary=2, secondary=1``
+
+            a Handstream detection can use
+            - ``primary=3, secondary=2, and_lower=True``.
+
+            and_lower implies accepting
+            - ``primary=2, secondary=2``
+            - ``primary=2, secondary=1``,
+            - ``primary=1, secondary=1``.
+
+        Args:
+            primary: The primary chord size for each chord stream.
+            secondary: The secondary chord size for each chord stream.
+            keys: The keys of the map, used to detect pattern limits.
+            and_lower: Whether to include lower size chords or not
+            include_jack: Whether to include jackstreams or not
+        """
+
+        return self.combinations(
+            size=2,
+            make_size2=True,
+            chord_filter=PtnFilterChord.create(
+                [[primary, secondary]], keys=keys,
+                options=PtnFilterChord.Option.ANY_ORDER |
+                        PtnFilterChord.Option.AND_LOWER if and_lower else 0,
+                exclude=False
+            ).filter,
+            combo_filter=PtnFilterCombo.create(
+                [[0, 0]], keys=keys,
+                options=PtnFilterCombo.Option.REPEAT,
+                exclude=True).filter if not include_jack else None,
+            type_filter=PtnFilterType.create(
+                [[HoldTail, object]],
+                options=PtnFilterType.Option.ANY_ORDER,
+                exclude=True
+            ).filter
+        )
```

### Comparing `reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawBeatLines.py` & `reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawBeatLines.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,55 +1,55 @@
-from __future__ import annotations
-
-from typing import List, Dict
-
-from reamber.algorithms.playField import PlayField
-from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
-from reamber.base.RAConst import RAConst
-
-
-class PFDrawBeatLines(PFDrawable):
-
-    def __init__(self,
-                 divisions: List = (1, 2, 4),
-                 default_color: str = "#666666",
-                 division_colors: Dict = None):
-        """Draws beat lines by division specified
-
-        Supported Default Snap Colors: 1, 2, 3, 4, 5, 6, 8, 12, 16, 24, 32.
-
-        The colors can be found in RAConst.
-
-        You can specify non-default snaps (including floats) and your custom
-        division_colors.
-
-        The new colors will override the default colors if they overlap.
-
-        Args:
-            divisions: Draws the 1/n lines in the field
-            default_color: Default color for unsupported snap colors
-            division_colors: A custom color dictionary to use.
-                A template can be found in RAConst.DIVISION_COLORS.
-        """
-        self.divisions = divisions
-        self.default_color = default_color
-        self.division_colors = {**RAConst.DIVISION_COLORS, **division_colors} \
-            if division_colors else RAConst.DIVISION_COLORS
-
-    def draw(self, pf: PlayField) -> PlayField:
-        """Refer to __init__"""
-
-        # Draw it from most to least common, else it'll overlap incorrectly
-        for division in sorted(self.divisions, reverse=True):
-
-            color = self.division_colors.get(division, self.default_color)
-            for beat in pf.m.bpms.snap_offsets(
-                nths=division,
-                last_offset=pf.m.stack().offset.max()
-            ):
-                pf.canvas_draw.line([
-                    pf.get_pos(beat),
-                    pf.get_pos(beat, pf.keys)
-                ],
-                    fill=color)
-
-        return pf
+from __future__ import annotations
+
+from typing import List, Dict
+
+from reamber.algorithms.playField import PlayField
+from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
+from reamber.base.RAConst import RAConst
+
+
+class PFDrawBeatLines(PFDrawable):
+
+    def __init__(self,
+                 divisions: List = (1, 2, 4),
+                 default_color: str = "#666666",
+                 division_colors: Dict = None):
+        """Draws beat lines by division specified
+
+        Supported Default Snap Colors: 1, 2, 3, 4, 5, 6, 8, 12, 16, 24, 32.
+
+        The colors can be found in RAConst.
+
+        You can specify non-default snaps (including floats) and your custom
+        division_colors.
+
+        The new colors will override the default colors if they overlap.
+
+        Args:
+            divisions: Draws the 1/n lines in the field
+            default_color: Default color for unsupported snap colors
+            division_colors: A custom color dictionary to use.
+                A template can be found in RAConst.DIVISION_COLORS.
+        """
+        self.divisions = divisions
+        self.default_color = default_color
+        self.division_colors = {**RAConst.DIVISION_COLORS, **division_colors} \
+            if division_colors else RAConst.DIVISION_COLORS
+
+    def draw(self, pf: PlayField) -> PlayField:
+        """Refer to __init__"""
+
+        # Draw it from most to least common, else it'll overlap incorrectly
+        for division in sorted(self.divisions, reverse=True):
+
+            color = self.division_colors.get(division, self.default_color)
+            for beat in pf.m.bpms.snap_offsets(
+                nths=division,
+                last_offset=pf.m.stack().offset.max()
+            ):
+                pf.canvas_draw.line([
+                    pf.get_pos(beat),
+                    pf.get_pos(beat, pf.keys)
+                ],
+                    fill=color)
+
+        return pf
```

### Comparing `reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawBpm.py` & `reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawSv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,43 +1,47 @@
-from __future__ import annotations
-
-from reamber.algorithms.playField import PlayField
-from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
-
-
-class PFDrawBpm(PFDrawable):
-
-    def __init__(self,
-                 decimal_places: int = 2,
-                 color: str = "#cf6b4a",
-                 x_offset: int = 0,
-                 y_offset: int = 0):
-        """Draws Bpms on the field
-
-        Args:
-            decimal_places: The number of decimal places to display
-            color: The color of the text
-            x_offset: Padding from the right
-            y_offset: Padding from the bottom
-        """
-        self.x_offset = x_offset
-        self.y_offset = y_offset
-        self.decimal_places = decimal_places
-        self.color = color
-
-    # noinspection DuplicatedCode
-    def draw(self, pf: PlayField) -> PlayField:
-        """Refer to __init__"""
-        for bpm in pf.m.bpms:
-            txt = f"{float(bpm.bpm):.{self.decimal_places}f}"
-            w, h = pf.canvas_draw.textsize(txt)
-
-            pf.canvas_draw.text(
-                xy=pf.get_pos(bpm.offset,
-                              column=pf.keys,
-                              x_offset=self.x_offset,
-                              y_offset=self.y_offset - h / 2),
-                text=txt,
-                fill=self.color
-            )
-
-        return pf
+from __future__ import annotations
+
+from reamber.algorithms.playField import PlayField
+from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
+from reamber.osu.OsuMap import OsuMap
+from reamber.quaver.QuaMap import QuaMap
+
+
+class PFDrawSv(PFDrawable):
+
+    def __init__(self,
+                 decimal_places: int = 2,
+                 color: str = "#4ef279",
+                 x_offset: int = 0,
+                 y_offset: int = 0):
+        """Draws Svs on the field, only works with maps that have svs
+
+        Args:
+            decimal_places: The number of decimal places to display
+            color: The color of the text
+            x_offset: Padding from the right
+            y_offset: The offset to move the text
+        """
+        self.x_offset = x_offset
+        self.y_offset = y_offset
+        self.decimal_places = decimal_places
+        self.color = color
+
+    def draw(self, pf: PlayField) -> PlayField:
+        """Refer to __init__"""
+        assert isinstance(pf.m, OsuMap) or isinstance(pf.m, QuaMap), \
+            "Only sv maps are supported."
+
+        for sv in pf.m.svs:
+            txt = f"{sv.multiplier:.{self.decimal_places}f}"
+            _, h = pf.canvas_draw.textsize(txt)
+
+            pf.canvas_draw.text(
+                xy=pf.get_pos(sv.offset,
+                              column=pf.keys,
+                              x_offset=self.x_offset,
+                              y_offset=self.y_offset - h / 2),
+                text=txt,
+                fill=self.color
+            )
+
+        return pf
```

### Comparing `reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawLines.py` & `reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawLines.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from typing import List, Tuple, Callable
-
-import numpy as np
-
-from reamber.algorithms.playField import PlayField
-from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
-
-
-@dataclass
-class PFLine:
-    """A dataclass holding the coordinates for PFDrawLines Generation"""
-    col_from: int
-    col_to: int
-    offset_from: float
-    offset_to: float
-
-
-class PFDrawLines(PFDrawable):
-
-    def __init__(self,
-                 lines: List[PFLine],
-                 color: Callable[[int, float], str | Tuple] =
-                 lambda x, y: "#999999",
-                 width: Callable[[int, float], int] = lambda x, y: 1):
-        """The draws listed lines on the field
-
-        Args:
-            lines: The lines to draw
-            color: The lambda to determine color.
-                func(colDifference, offsetDifference) -> str or rgba Tuple
-            width: The lambda to determine width.
-                func(colDifference, offsetDifference) -> int
-        """
-        self.lines = lines
-        self.color = color
-        self.width = width
-
-    class Colors:
-        BLUE = {"from_rgb": (79, 103, 255), "to_rgb": (161, 255, 239)}
-        ORANGE = {"from_rgb": (255, 167, 43), "to_rgb": (255, 197, 115)}
-        GREEN = {"from_rgb": (15, 255, 47), "to_rgb": (133, 255, 149)}
-        PINK = {"from_rgb": (247, 64, 202), "to_rgb": (255, 130, 224)}
-        RED = {"from_rgb": (255, 28, 28), "to_rgb": (255, 148, 148)}
-        PURPLE = {"from_rgb": (177, 51, 255), "to_rgb": (220, 163, 255)}
-
-    @staticmethod
-    def color_lambda(
-        keys,
-        from_rgb: Tuple[int, int, int] = (79, 103, 255),
-        to_rgb: Tuple[int, int, int] = (161, 255, 239),
-        nearest: float = 100,
-        furthest: float = 1000
-    ) -> Callable[[int, float], Tuple[int, int, int, int]]:
-        """Creates a quick lambda for color
-
-        This can be used in PFDrawLines(color=PFDrawLines.color_lambda(...))
-
-        Args:
-            keys: Keys of the map
-            from_rgb: Color when the column difference is the smallest
-            to_rgb: Color when the column difference is the largest
-            nearest: The largest distance where the color is from_rgb
-            furthest: The smallest distance where the color is to_rgb
-
-        Returns:
-             Callable used by DrawLines and returns a RGBA Tuple
-        """
-
-        def func(col: int, offset: float) -> Tuple[int, int, int, int]:
-            clamp = max(nearest, min(furthest, abs(offset)))
-            offset_factor = 1 - (clamp - nearest) / (furthest - nearest)
-            col_factor = 1 - abs(col) / (keys - 1)
-            new_rgb = np.asarray(to_rgb) + \
-                      (np.asarray(from_rgb) - np.asarray(to_rgb)) * \
-                      offset_factor * col_factor
-            new_rgb = (*new_rgb.astype(int),
-                       int(255 * offset_factor * col_factor))
-            # noinspection PyTypeChecker
-            return new_rgb
-
-        return func
-
-    @staticmethod
-    def width_lambda(keys,
-                     from_width: int = 5,
-                     to_width: int = 1,
-                     nearest: float = 100,
-                     furthest: float = 1000) -> Callable[[int, float], int]:
-        """Creates a quick lambda for color
-
-        This can be used in PFDrawLines(color=PFDrawLines.width_lambda(...))
-
-        Returns the expected width
-
-        Args:
-            keys: Keys of the map. (m.notes.maxColumn() + 1)
-            from_width: Width when the column difference is the smallest
-            to_width: Width when the column difference is the largest
-            nearest: The largest distance where the color is from_rgb
-            furthest: The smallest distance where the color is to_rgb
-        """
-
-        def func(col: int, offset: float) -> int:
-            clamp = max(nearest, min(furthest, abs(offset)))
-            offset_factor = 1 - (clamp - nearest) / (furthest - nearest)
-            col_factor = 1 - abs(col) / (keys - 1)
-            return int(to_width + (
-                from_width - to_width) * offset_factor * col_factor)
-
-        return func
-
-    def draw(self, pf: PlayField) -> PlayField:
-        """Refer to __init__"""
-
-        for line in self.lines:
-            pf.canvas_draw.line(
-                [
-                    pf.get_pos(
-                        column=line.col_from,
-                        offset=line.offset_from,
-                        x_offset=pf.note_width / 2,
-                        y_offset=-pf.hit_height / 2),
-                    pf.get_pos(
-                        column=line.col_to,
-                        offset=line.offset_to,
-                        x_offset=pf.note_width / 2,
-                        y_offset=-pf.hit_height / 2)
-                ],
-                fill=self.color(line.col_to - line.col_from,
-                                line.offset_to - line.offset_from),
-                width=self.width(line.col_to - line.col_from,
-                                 line.offset_to - line.offset_from)
-            )
-
-        return pf
-
-    @staticmethod
-    def from_combo(combo: np.ndarray,
-                   keys: int,
-                   from_rgb: Tuple[int, int, int],
-                   to_rgb: Tuple[int, int, int],
-                   from_width=5,
-                   to_width=1,
-                   nearest: float = 50,
-                   furthest: float = 300) -> PFDrawLines:
-        """Draw combination lines on the PF
-
-        Args:
-            combo:
-            keys: The keys of the map, used to detect pattern limits.
-            from_rgb: Color when the column/offset difference is the smallest
-            to_rgb: Color when the column/offset difference is the largest
-            from_width: Width when the column difference is the smallest
-            to_width: Width when the column difference is the largest
-            nearest: The largest distance where the color is from_rgb
-            furthest: The smallest distance where the color is to_rgb
-        """
-
-        return PFDrawLines(
-            [*[PFLine(i['column'][0], i['column'][1],
-                      i['offset'][0], i['offset'][1])
-               for i in combo]],
-            color=PFDrawLines.color_lambda(keys,
-                                           from_rgb=from_rgb,
-                                           to_rgb=to_rgb,
-                                           nearest=nearest,
-                                           furthest=furthest),
-            width=PFDrawLines.width_lambda(keys,
-                                           from_width=from_width,
-                                           to_width=to_width,
-                                           nearest=nearest,
-                                           furthest=furthest))
+from __future__ import annotations
+
+from dataclasses import dataclass
+from typing import List, Tuple, Callable
+
+import numpy as np
+
+from reamber.algorithms.playField import PlayField
+from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
+
+
+@dataclass
+class PFLine:
+    """A dataclass holding the coordinates for PFDrawLines Generation"""
+    col_from: int
+    col_to: int
+    offset_from: float
+    offset_to: float
+
+
+class PFDrawLines(PFDrawable):
+
+    def __init__(self,
+                 lines: List[PFLine],
+                 color: Callable[[int, float], str | Tuple] =
+                 lambda x, y: "#999999",
+                 width: Callable[[int, float], int] = lambda x, y: 1):
+        """The draws listed lines on the field
+
+        Args:
+            lines: The lines to draw
+            color: The lambda to determine color.
+                func(colDifference, offsetDifference) -> str or rgba Tuple
+            width: The lambda to determine width.
+                func(colDifference, offsetDifference) -> int
+        """
+        self.lines = lines
+        self.color = color
+        self.width = width
+
+    class Colors:
+        BLUE = {"from_rgb": (79, 103, 255), "to_rgb": (161, 255, 239)}
+        ORANGE = {"from_rgb": (255, 167, 43), "to_rgb": (255, 197, 115)}
+        GREEN = {"from_rgb": (15, 255, 47), "to_rgb": (133, 255, 149)}
+        PINK = {"from_rgb": (247, 64, 202), "to_rgb": (255, 130, 224)}
+        RED = {"from_rgb": (255, 28, 28), "to_rgb": (255, 148, 148)}
+        PURPLE = {"from_rgb": (177, 51, 255), "to_rgb": (220, 163, 255)}
+
+    @staticmethod
+    def color_lambda(
+        keys,
+        from_rgb: Tuple[int, int, int] = (79, 103, 255),
+        to_rgb: Tuple[int, int, int] = (161, 255, 239),
+        nearest: float = 100,
+        furthest: float = 1000
+    ) -> Callable[[int, float], Tuple[int, int, int, int]]:
+        """Creates a quick lambda for color
+
+        This can be used in PFDrawLines(color=PFDrawLines.color_lambda(...))
+
+        Args:
+            keys: Keys of the map
+            from_rgb: Color when the column difference is the smallest
+            to_rgb: Color when the column difference is the largest
+            nearest: The largest distance where the color is from_rgb
+            furthest: The smallest distance where the color is to_rgb
+
+        Returns:
+             Callable used by DrawLines and returns a RGBA Tuple
+        """
+
+        def func(col: int, offset: float) -> Tuple[int, int, int, int]:
+            clamp = max(nearest, min(furthest, abs(offset)))
+            offset_factor = 1 - (clamp - nearest) / (furthest - nearest)
+            col_factor = 1 - abs(col) / (keys - 1)
+            new_rgb = np.asarray(to_rgb) + \
+                      (np.asarray(from_rgb) - np.asarray(to_rgb)) * \
+                      offset_factor * col_factor
+            new_rgb = (*new_rgb.astype(int),
+                       int(255 * offset_factor * col_factor))
+            # noinspection PyTypeChecker
+            return new_rgb
+
+        return func
+
+    @staticmethod
+    def width_lambda(keys,
+                     from_width: int = 5,
+                     to_width: int = 1,
+                     nearest: float = 100,
+                     furthest: float = 1000) -> Callable[[int, float], int]:
+        """Creates a quick lambda for color
+
+        This can be used in PFDrawLines(color=PFDrawLines.width_lambda(...))
+
+        Returns the expected width
+
+        Args:
+            keys: Keys of the map. (m.notes.maxColumn() + 1)
+            from_width: Width when the column difference is the smallest
+            to_width: Width when the column difference is the largest
+            nearest: The largest distance where the color is from_rgb
+            furthest: The smallest distance where the color is to_rgb
+        """
+
+        def func(col: int, offset: float) -> int:
+            clamp = max(nearest, min(furthest, abs(offset)))
+            offset_factor = 1 - (clamp - nearest) / (furthest - nearest)
+            col_factor = 1 - abs(col) / (keys - 1)
+            return int(to_width + (
+                from_width - to_width) * offset_factor * col_factor)
+
+        return func
+
+    def draw(self, pf: PlayField) -> PlayField:
+        """Refer to __init__"""
+
+        for line in self.lines:
+            pf.canvas_draw.line(
+                [
+                    pf.get_pos(
+                        column=line.col_from,
+                        offset=line.offset_from,
+                        x_offset=pf.note_width / 2,
+                        y_offset=-pf.hit_height / 2),
+                    pf.get_pos(
+                        column=line.col_to,
+                        offset=line.offset_to,
+                        x_offset=pf.note_width / 2,
+                        y_offset=-pf.hit_height / 2)
+                ],
+                fill=self.color(line.col_to - line.col_from,
+                                line.offset_to - line.offset_from),
+                width=self.width(line.col_to - line.col_from,
+                                 line.offset_to - line.offset_from)
+            )
+
+        return pf
+
+    @staticmethod
+    def from_combo(combo: np.ndarray,
+                   keys: int,
+                   from_rgb: Tuple[int, int, int],
+                   to_rgb: Tuple[int, int, int],
+                   from_width=5,
+                   to_width=1,
+                   nearest: float = 50,
+                   furthest: float = 300) -> PFDrawLines:
+        """Draw combination lines on the PF
+
+        Args:
+            combo:
+            keys: The keys of the map, used to detect pattern limits.
+            from_rgb: Color when the column/offset difference is the smallest
+            to_rgb: Color when the column/offset difference is the largest
+            from_width: Width when the column difference is the smallest
+            to_width: Width when the column difference is the largest
+            nearest: The largest distance where the color is from_rgb
+            furthest: The smallest distance where the color is to_rgb
+        """
+
+        return PFDrawLines(
+            [*[PFLine(i['column'][0], i['column'][1],
+                      i['offset'][0], i['offset'][1])
+               for i in combo]],
+            color=PFDrawLines.color_lambda(keys,
+                                           from_rgb=from_rgb,
+                                           to_rgb=to_rgb,
+                                           nearest=nearest,
+                                           furthest=furthest),
+            width=PFDrawLines.width_lambda(keys,
+                                           from_width=from_width,
+                                           to_width=to_width,
+                                           nearest=nearest,
+                                           furthest=furthest))
```

### Comparing `reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawNotes.py` & `reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawNotes.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,188 +1,188 @@
-from __future__ import annotations
-
-from PIL import Image, ImageDraw
-
-from reamber.algorithms.playField import PlayField
-from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
-
-
-class PFDrawNotes(PFDrawable):
-    COL_DICT = [[0],
-                [1, 0],
-                [0, 2, 0],
-                [0, 1, 1, 0],
-                [0, 1, 2, 1, 0],
-                [0, 1, 0, 0, 1, 0],
-                [0, 1, 0, 2, 0, 1, 0],
-                [0, 1, 0, 1, 1, 0, 1, 0],
-                [0, 1, 0, 1, 2, 1, 0, 1, 0],
-                [0, 1, 0, 1, 0, 0, 1, 0, 1, 0],
-                [0, 1, 0, 1, 0, 2, 0, 1, 0, 1, 0],
-                [0, 1, 0, 1, 0, 1, 1, 0, 1, 0, 1, 0],
-                [0, 1, 0, 1, 0, 1, 2, 1, 0, 1, 0, 1, 0],
-                [0, 1, 0, 1, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0],
-                [0, 1, 0, 1, 0, 1, 0, 2, 0, 1, 0, 1, 0, 1, 0],
-                [0, 1, 0, 1, 0, 1, 0, 1, 1, 0, 1, 0, 1, 0, 1, 0],
-                [0, 1, 0, 1, 0, 1, 0, 1, 2, 1, 0, 1, 0, 1, 0, 1, 0],
-                [0, 1, 0, 1, 0, 1, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0, 1, 0]]
-
-    def __init__(self,
-                 img0_outline_color: str = "#47fcff",
-                 img0_fill_color: str = "#28b5b8",
-                 img1_outline_color: str = "#ffffff",
-                 img1_fill_color: str = "#c2c2c2",
-                 img2_outline_color: str = "#f8ff30",
-                 img2_fill_color: str = "#adb31e",
-                 outline_width: int = 2):
-        """The draws all the notes on the field
-
-        The color used for each column is specified in the COL_DICT
-
-        Args:
-            img0_outline_color: The color to outline the first note image
-            img0_fill_color: The color to fill the first note image
-            img1_outline_color: The color to outline the second note image
-            img1_fill_color: The color to fill the second note image
-            img2_outline_color: The color to outline the third note image
-            img2_fill_color: The color to fill the third note image
-            outline_width: The width of each outline. 0 for no outline
-        """
-        self.outline_width = outline_width
-        self.img0_outline_color = img0_outline_color
-        self.img0_fill_color = img0_fill_color
-        self.img1_outline_color = img1_outline_color
-        self.img1_fill_color = img1_fill_color
-        self.img2_outline_color = img2_outline_color
-        self.img2_fill_color = img2_fill_color
-
-    def draw(self, pf: PlayField) -> PlayField:
-        """Refer to __init__"""
-
-        imgs = [self._create_note_set(pf=pf, fill_color=self.img0_fill_color,
-                                      outline_color=self.img0_outline_color,
-                                      width=self.outline_width),
-                self._create_note_set(pf=pf, fill_color=self.img1_fill_color,
-                                      outline_color=self.img1_outline_color,
-                                      width=self.outline_width),
-                self._create_note_set(pf=pf, fill_color=self.img2_fill_color,
-                                      outline_color=self.img2_outline_color,
-                                      width=self.outline_width)]
-
-        self._draw_hits(imgs, pf)
-        self._draw_holds(imgs, pf)
-
-        return pf
-
-    def _draw_hits(self, imgs, pf: PlayField):
-        for hit in pf.m.hits:
-            hit_img = imgs[self.COL_DICT[int(pf.keys) - 1][int(hit.column)]][
-                'hit']
-            pf.canvas.paste(hit_img,
-                            pf.get_pos(hit.offset, hit.column,
-                                       y_offset=-pf.hit_height),
-                            hit_img)
-
-    def _draw_holds(self, imgs, pf: PlayField):
-        for hold in pf.m.holds:
-            hold_head_img = \
-                imgs[self.COL_DICT[int(pf.keys) - 1]
-                [int(hold.column)]]['holdH']
-
-            # DRAWS THE HEAD
-            pf.canvas.paste(
-                hold_head_img,
-                pf.get_pos(hold.offset, hold.column, y_offset=-pf.hold_height),
-                hold_head_img
-            )
-
-            hold_tail_img = \
-                imgs[self.COL_DICT[int(pf.keys) - 1]
-                [int(hold.column)]]['holdT']
-
-            # DRAWS THE TAIL
-            pf.canvas.paste(hold_tail_img,
-                            pf.get_pos(hold.tail_offset, hold.column,
-                                       y_offset=-pf.hold_height),
-                            hold_tail_img)
-
-            # DRAWS THE BODY
-            hold_img_height = int(hold.length / pf.duration_per_px) \
-                              - pf.hold_height + pf.HOLD_RESIZE_BUFFER
-
-            # If too short we don't draw it
-            if hold_img_height > 0:
-                hold_img = \
-                    imgs[self.COL_DICT[int(pf.keys) - 1]
-                    [int(hold.column)]]['holdB'].resize(
-                        (pf.note_width, hold_img_height)
-                    )
-
-                pf.canvas.paste(hold_img,
-                                pf.get_pos(hold.tail_offset, hold.column),
-                                hold_img)
-
-    @staticmethod
-    def _create_hit(pf: PlayField, fill_color, outline_color, width=4):
-        img = Image.new(mode='RGBA', size=(pf.note_width, pf.hit_height),
-                        color=(0, 0, 0, 0))
-        draw = ImageDraw.Draw(img)
-        path = [(0, 0),
-                (0, pf.hit_height - 1),
-                (pf.note_width - 1, pf.hit_height - 1),
-                (pf.note_width - 1, 0),
-                (0, 0)]
-        draw.polygon(path, fill=fill_color)
-        draw.line(path, fill=outline_color, width=width)
-        return img
-
-    @staticmethod
-    def _create_hold_head(pf: PlayField, fill_color, outline_color, width=4):
-        img = Image.new(mode='RGBA', size=(pf.note_width, pf.hold_height),
-                        color=(0, 0, 0, 0))
-        draw = ImageDraw.Draw(img)
-        path = [(0, 0),
-                (int(pf.note_width * 1 / 3), pf.hold_height - int(width / 2)),
-                (int(pf.note_width * 2 / 3), pf.hold_height - int(width / 2)),
-                (pf.note_width - 1, 0)]
-
-        draw.polygon(path, fill=fill_color)
-        draw.line(path, fill=outline_color, width=width)
-        return img
-
-    @staticmethod
-    def _create_hold_body(pf: PlayField, fill_color, outline_color, width=4):
-        img = Image.new(mode='RGBA', size=(pf.note_width, pf.hold_height),
-                        color=(0, 0, 0, 0))
-        draw = ImageDraw.Draw(img)
-        draw.polygon([(0, 0),
-                      (0, pf.note_width - 1),
-                      (pf.note_width - 1, pf.hit_height - 1),
-                      (pf.note_width - 1, 0)],
-                     fill=fill_color)
-        draw.line([(0, 0),
-                   (0, pf.hold_height)],
-                  fill=outline_color, width=width)
-        draw.line([(pf.note_width - 2, 0),
-                   (pf.note_width - 2, pf.hold_height)],
-                  fill=outline_color, width=width)
-        return img
-
-    @classmethod
-    def _create_hold_tail(cls, pf: PlayField, fill_color, outline_color,
-                          width=4):
-        """It's just the inverted head"""
-        return cls._create_hold_head(pf, fill_color, outline_color,
-                                     width).transpose(Image.FLIP_TOP_BOTTOM)
-
-    @classmethod
-    def _create_note_set(cls, pf: PlayField, fill_color, outline_color,
-                         width=4):
-        return {
-            'hit': cls._create_hit(pf, fill_color, outline_color, width),
-            'holdH': cls._create_hold_head(pf, fill_color, outline_color,
-                                           width),
-            'holdB': cls._create_hold_body(pf, fill_color, outline_color,
-                                           width),
-            'holdT': cls._create_hold_tail(pf, fill_color, outline_color,
-                                           width)
-        }
+from __future__ import annotations
+
+from PIL import Image, ImageDraw
+
+from reamber.algorithms.playField import PlayField
+from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
+
+
+class PFDrawNotes(PFDrawable):
+    COL_DICT = [[0],
+                [1, 0],
+                [0, 2, 0],
+                [0, 1, 1, 0],
+                [0, 1, 2, 1, 0],
+                [0, 1, 0, 0, 1, 0],
+                [0, 1, 0, 2, 0, 1, 0],
+                [0, 1, 0, 1, 1, 0, 1, 0],
+                [0, 1, 0, 1, 2, 1, 0, 1, 0],
+                [0, 1, 0, 1, 0, 0, 1, 0, 1, 0],
+                [0, 1, 0, 1, 0, 2, 0, 1, 0, 1, 0],
+                [0, 1, 0, 1, 0, 1, 1, 0, 1, 0, 1, 0],
+                [0, 1, 0, 1, 0, 1, 2, 1, 0, 1, 0, 1, 0],
+                [0, 1, 0, 1, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0],
+                [0, 1, 0, 1, 0, 1, 0, 2, 0, 1, 0, 1, 0, 1, 0],
+                [0, 1, 0, 1, 0, 1, 0, 1, 1, 0, 1, 0, 1, 0, 1, 0],
+                [0, 1, 0, 1, 0, 1, 0, 1, 2, 1, 0, 1, 0, 1, 0, 1, 0],
+                [0, 1, 0, 1, 0, 1, 0, 1, 0, 0, 1, 0, 1, 0, 1, 0, 1, 0]]
+
+    def __init__(self,
+                 img0_outline_color: str = "#47fcff",
+                 img0_fill_color: str = "#28b5b8",
+                 img1_outline_color: str = "#ffffff",
+                 img1_fill_color: str = "#c2c2c2",
+                 img2_outline_color: str = "#f8ff30",
+                 img2_fill_color: str = "#adb31e",
+                 outline_width: int = 2):
+        """The draws all the notes on the field
+
+        The color used for each column is specified in the COL_DICT
+
+        Args:
+            img0_outline_color: The color to outline the first note image
+            img0_fill_color: The color to fill the first note image
+            img1_outline_color: The color to outline the second note image
+            img1_fill_color: The color to fill the second note image
+            img2_outline_color: The color to outline the third note image
+            img2_fill_color: The color to fill the third note image
+            outline_width: The width of each outline. 0 for no outline
+        """
+        self.outline_width = outline_width
+        self.img0_outline_color = img0_outline_color
+        self.img0_fill_color = img0_fill_color
+        self.img1_outline_color = img1_outline_color
+        self.img1_fill_color = img1_fill_color
+        self.img2_outline_color = img2_outline_color
+        self.img2_fill_color = img2_fill_color
+
+    def draw(self, pf: PlayField) -> PlayField:
+        """Refer to __init__"""
+
+        imgs = [self._create_note_set(pf=pf, fill_color=self.img0_fill_color,
+                                      outline_color=self.img0_outline_color,
+                                      width=self.outline_width),
+                self._create_note_set(pf=pf, fill_color=self.img1_fill_color,
+                                      outline_color=self.img1_outline_color,
+                                      width=self.outline_width),
+                self._create_note_set(pf=pf, fill_color=self.img2_fill_color,
+                                      outline_color=self.img2_outline_color,
+                                      width=self.outline_width)]
+
+        self._draw_hits(imgs, pf)
+        self._draw_holds(imgs, pf)
+
+        return pf
+
+    def _draw_hits(self, imgs, pf: PlayField):
+        for hit in pf.m.hits:
+            hit_img = imgs[self.COL_DICT[int(pf.keys) - 1][int(hit.column)]][
+                'hit']
+            pf.canvas.paste(hit_img,
+                            pf.get_pos(hit.offset, hit.column,
+                                       y_offset=-pf.hit_height),
+                            hit_img)
+
+    def _draw_holds(self, imgs, pf: PlayField):
+        for hold in pf.m.holds:
+            hold_head_img = \
+                imgs[self.COL_DICT[int(pf.keys) - 1]
+                [int(hold.column)]]['holdH']
+
+            # DRAWS THE HEAD
+            pf.canvas.paste(
+                hold_head_img,
+                pf.get_pos(hold.offset, hold.column, y_offset=-pf.hold_height),
+                hold_head_img
+            )
+
+            hold_tail_img = \
+                imgs[self.COL_DICT[int(pf.keys) - 1]
+                [int(hold.column)]]['holdT']
+
+            # DRAWS THE TAIL
+            pf.canvas.paste(hold_tail_img,
+                            pf.get_pos(hold.tail_offset, hold.column,
+                                       y_offset=-pf.hold_height),
+                            hold_tail_img)
+
+            # DRAWS THE BODY
+            hold_img_height = int(hold.length / pf.duration_per_px) \
+                              - pf.hold_height + pf.HOLD_RESIZE_BUFFER
+
+            # If too short we don't draw it
+            if hold_img_height > 0:
+                hold_img = \
+                    imgs[self.COL_DICT[int(pf.keys) - 1]
+                    [int(hold.column)]]['holdB'].resize(
+                        (pf.note_width, hold_img_height)
+                    )
+
+                pf.canvas.paste(hold_img,
+                                pf.get_pos(hold.tail_offset, hold.column),
+                                hold_img)
+
+    @staticmethod
+    def _create_hit(pf: PlayField, fill_color, outline_color, width=4):
+        img = Image.new(mode='RGBA', size=(pf.note_width, pf.hit_height),
+                        color=(0, 0, 0, 0))
+        draw = ImageDraw.Draw(img)
+        path = [(0, 0),
+                (0, pf.hit_height - 1),
+                (pf.note_width - 1, pf.hit_height - 1),
+                (pf.note_width - 1, 0),
+                (0, 0)]
+        draw.polygon(path, fill=fill_color)
+        draw.line(path, fill=outline_color, width=width)
+        return img
+
+    @staticmethod
+    def _create_hold_head(pf: PlayField, fill_color, outline_color, width=4):
+        img = Image.new(mode='RGBA', size=(pf.note_width, pf.hold_height),
+                        color=(0, 0, 0, 0))
+        draw = ImageDraw.Draw(img)
+        path = [(0, 0),
+                (int(pf.note_width * 1 / 3), pf.hold_height - int(width / 2)),
+                (int(pf.note_width * 2 / 3), pf.hold_height - int(width / 2)),
+                (pf.note_width - 1, 0)]
+
+        draw.polygon(path, fill=fill_color)
+        draw.line(path, fill=outline_color, width=width)
+        return img
+
+    @staticmethod
+    def _create_hold_body(pf: PlayField, fill_color, outline_color, width=4):
+        img = Image.new(mode='RGBA', size=(pf.note_width, pf.hold_height),
+                        color=(0, 0, 0, 0))
+        draw = ImageDraw.Draw(img)
+        draw.polygon([(0, 0),
+                      (0, pf.note_width - 1),
+                      (pf.note_width - 1, pf.hit_height - 1),
+                      (pf.note_width - 1, 0)],
+                     fill=fill_color)
+        draw.line([(0, 0),
+                   (0, pf.hold_height)],
+                  fill=outline_color, width=width)
+        draw.line([(pf.note_width - 2, 0),
+                   (pf.note_width - 2, pf.hold_height)],
+                  fill=outline_color, width=width)
+        return img
+
+    @classmethod
+    def _create_hold_tail(cls, pf: PlayField, fill_color, outline_color,
+                          width=4):
+        """It's just the inverted head"""
+        return cls._create_hold_head(pf, fill_color, outline_color,
+                                     width).transpose(Image.FLIP_TOP_BOTTOM)
+
+    @classmethod
+    def _create_note_set(cls, pf: PlayField, fill_color, outline_color,
+                         width=4):
+        return {
+            'hit': cls._create_hit(pf, fill_color, outline_color, width),
+            'holdH': cls._create_hold_head(pf, fill_color, outline_color,
+                                           width),
+            'holdB': cls._create_hold_body(pf, fill_color, outline_color,
+                                           width),
+            'holdT': cls._create_hold_tail(pf, fill_color, outline_color,
+                                           width)
+        }
```

### Comparing `reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawOffsets.py` & `reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawOffsets.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-from __future__ import annotations
-
-import numpy as np
-
-from reamber.algorithms.playField import PlayField
-from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
-
-
-class PFDrawOffsets(PFDrawable):
-
-    def __init__(self,
-                 decimal_places: int = 2,
-                 color: str = "#CCCCCC",
-                 x_offset: int = 0,
-                 y_offset: int = 0,
-                 interval: float = 10000):
-        """Draws Bpms on the field
-
-        Args:
-            decimal_places: Decimal places to display
-            color: The color of the text
-            x_offset: Padding from the right
-            y_offset: Padding from the top
-            interval: MS Time between labels
-        """
-        self.x_offset = x_offset
-        self.y_offset = y_offset
-        self.decimal_places = decimal_places
-        self.color = color
-        self.interval = interval
-
-    def draw(self, pf: PlayField) -> PlayField:
-        """Refer to __init__"""
-        for offset in np.arange(0, pf.end, self.interval):
-            txt = f"{offset:.{self.decimal_places}f}"
-            w, h = pf.canvas_draw.textsize(txt)
-
-            pf.canvas_draw.text(
-                xy=pf.get_pos(offset,
-                              column=pf.keys,
-                              x_offset=self.x_offset,
-                              y_offset=self.y_offset - h / 2),
-                text=txt,
-                fill=self.color
-            )
-
-        return pf
+from __future__ import annotations
+
+import numpy as np
+
+from reamber.algorithms.playField import PlayField
+from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
+
+
+class PFDrawOffsets(PFDrawable):
+
+    def __init__(self,
+                 decimal_places: int = 2,
+                 color: str = "#CCCCCC",
+                 x_offset: int = 0,
+                 y_offset: int = 0,
+                 interval: float = 10000):
+        """Draws Bpms on the field
+
+        Args:
+            decimal_places: Decimal places to display
+            color: The color of the text
+            x_offset: Padding from the right
+            y_offset: Padding from the top
+            interval: MS Time between labels
+        """
+        self.x_offset = x_offset
+        self.y_offset = y_offset
+        self.decimal_places = decimal_places
+        self.color = color
+        self.interval = interval
+
+    def draw(self, pf: PlayField) -> PlayField:
+        """Refer to __init__"""
+        for offset in np.arange(0, pf.end, self.interval):
+            txt = f"{offset:.{self.decimal_places}f}"
+            w, h = pf.canvas_draw.textsize(txt)
+
+            pf.canvas_draw.text(
+                xy=pf.get_pos(offset,
+                              column=pf.keys,
+                              x_offset=self.x_offset,
+                              y_offset=self.y_offset - h / 2),
+                text=txt,
+                fill=self.color
+            )
+
+        return pf
```

### Comparing `reamber-0.1.7/reamber/algorithms/playField/parts/PFDrawSv.py` & `reamber-0.1.8/reamber/algorithms/playField/parts/PFDrawBpm.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,47 +1,43 @@
-from __future__ import annotations
-
-from reamber.algorithms.playField import PlayField
-from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
-from reamber.osu.OsuMap import OsuMap
-from reamber.quaver.QuaMap import QuaMap
-
-
-class PFDrawSv(PFDrawable):
-
-    def __init__(self,
-                 decimal_places: int = 2,
-                 color: str = "#4ef279",
-                 x_offset: int = 0,
-                 y_offset: int = 0):
-        """Draws Svs on the field, only works with maps that have svs
-
-        Args:
-            decimal_places: The number of decimal places to display
-            color: The color of the text
-            x_offset: Padding from the right
-            y_offset: The offset to move the text
-        """
-        self.x_offset = x_offset
-        self.y_offset = y_offset
-        self.decimal_places = decimal_places
-        self.color = color
-
-    def draw(self, pf: PlayField) -> PlayField:
-        """Refer to __init__"""
-        assert isinstance(pf.m, OsuMap) or isinstance(pf.m, QuaMap), \
-            "Only sv maps are supported."
-
-        for sv in pf.m.svs:
-            txt = f"{sv.multiplier:.{self.decimal_places}f}"
-            _, h = pf.canvas_draw.textsize(txt)
-
-            pf.canvas_draw.text(
-                xy=pf.get_pos(sv.offset,
-                              column=pf.keys,
-                              x_offset=self.x_offset,
-                              y_offset=self.y_offset - h / 2),
-                text=txt,
-                fill=self.color
-            )
-
-        return pf
+from __future__ import annotations
+
+from reamber.algorithms.playField import PlayField
+from reamber.algorithms.playField.parts.PFDrawable import PFDrawable
+
+
+class PFDrawBpm(PFDrawable):
+
+    def __init__(self,
+                 decimal_places: int = 2,
+                 color: str = "#cf6b4a",
+                 x_offset: int = 0,
+                 y_offset: int = 0):
+        """Draws Bpms on the field
+
+        Args:
+            decimal_places: The number of decimal places to display
+            color: The color of the text
+            x_offset: Padding from the right
+            y_offset: Padding from the bottom
+        """
+        self.x_offset = x_offset
+        self.y_offset = y_offset
+        self.decimal_places = decimal_places
+        self.color = color
+
+    # noinspection DuplicatedCode
+    def draw(self, pf: PlayField) -> PlayField:
+        """Refer to __init__"""
+        for bpm in pf.m.bpms:
+            txt = f"{float(bpm.bpm):.{self.decimal_places}f}"
+            w, h = pf.canvas_draw.textsize(txt)
+
+            pf.canvas_draw.text(
+                xy=pf.get_pos(bpm.offset,
+                              column=pf.keys,
+                              x_offset=self.x_offset,
+                              y_offset=self.y_offset - h / 2),
+                text=txt,
+                fill=self.color
+            )
+
+        return pf
```

### Comparing `reamber-0.1.7/reamber/algorithms/playField/parts/__init__.py` & `reamber-0.1.8/reamber/algorithms/playField/parts/__init__.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from reamber.algorithms.playField.parts.PFDrawBeatLines import PFDrawBeatLines
-from reamber.algorithms.playField.parts.PFDrawBpm import PFDrawBpm
-from reamber.algorithms.playField.parts.PFDrawColumnLines import \
-    PFDrawColumnLines
-from reamber.algorithms.playField.parts.PFDrawLines import PFDrawLines, PFLine
-from reamber.algorithms.playField.parts.PFDrawNotes import PFDrawNotes
-from reamber.algorithms.playField.parts.PFDrawOffsets import PFDrawOffsets
-from reamber.algorithms.playField.parts.PFDrawSv import PFDrawSv
-
-__all__ = ['PFDrawSv', 'PFDrawNotes', 'PFDrawBpm', 'PFDrawColumnLines',
-           'PFDrawBeatLines', 'PFDrawLines', 'PFLine', 'PFDrawOffsets']
+from reamber.algorithms.playField.parts.PFDrawBeatLines import PFDrawBeatLines
+from reamber.algorithms.playField.parts.PFDrawBpm import PFDrawBpm
+from reamber.algorithms.playField.parts.PFDrawColumnLines import \
+    PFDrawColumnLines
+from reamber.algorithms.playField.parts.PFDrawLines import PFDrawLines, PFLine
+from reamber.algorithms.playField.parts.PFDrawNotes import PFDrawNotes
+from reamber.algorithms.playField.parts.PFDrawOffsets import PFDrawOffsets
+from reamber.algorithms.playField.parts.PFDrawSv import PFDrawSv
+
+__all__ = ['PFDrawSv', 'PFDrawNotes', 'PFDrawBpm', 'PFDrawColumnLines',
+           'PFDrawBeatLines', 'PFDrawLines', 'PFLine', 'PFDrawOffsets']
```

### Comparing `reamber-0.1.7/reamber/algorithms/timing/utils/Snapper.py` & `reamber-0.1.8/reamber/algorithms/timing/utils/Snapper.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from __future__ import annotations
-
-from bisect import bisect_left
-from fractions import Fraction
-from typing import Iterable
-
-import numpy as np
-
-from reamber.algorithms.timing.utils.conf import DEFAULT_DIVISIONS
-
-
-def snap(value: float,
-         divisions: Iterable[int] = DEFAULT_DIVISIONS) -> Fraction:
-    """Snaps float value to closest division.
-
-    Args:
-        value: Value to snap
-        divisions: Divisions to accept
-    """
-    return Snapper(divisions=divisions).snap(value)
-
-
-class Snapper:
-    def __init__(self, divisions: Iterable[int] = DEFAULT_DIVISIONS):
-        """Initialize Snapper with defined divisions
-
-        Args:
-            divisions: Divisions acceptable when snapping
-        """
-        divisions = np.asarray(divisions)
-        max_slots = max(divisions)
-
-        # Creates the division triangle
-        den, num = np.indices([max_slots, max_slots])
-        den += 1
-        ar = num / den
-
-        ar[np.triu_indices(ar.shape[0], 1)] = np.nan
-        ar[1:, 0] = np.nan
-        # Prunes the repeated slots
-        visited = set()
-        for i in range(1, max_slots):
-            for j in range(1, i + 1):
-                if ar[i, j] in visited:
-                    ar[i, j] = np.nan
-                else:
-                    visited.add(ar[i, j])
-
-        # Add numerator & denominator
-        ar = np.stack([ar, num, den])
-        ar = ar[:, ~np.isnan(ar[0])].T
-        sorter = ar[:, 0].argsort()
-
-        # Add the case for 1/1 so that 0.9999... matches that
-        ar = np.vstack([ar[sorter], [1, 1, 1]])
-
-        self.val = ar[:, 0]
-        self.num = ar[:, 1]
-        self.den = ar[:, 2]
-
-    def snap(self, beat: float) -> Fraction:
-        """Snaps beat to nearest division"""
-        quo, rem = beat // 1, beat % 1
-        ix = bisect_left(self.val, rem)
-
-        # Bisect Left gets the next value
-        # E.g. [0, 0.5], bisect_left(ar, 0.0001) = 1, bisect_left(ar, 0) = 0,
-        if ix != 0:
-            left_diff, right_diff = \
-                rem - self.val[ix - 1], self.val[ix] - rem
-            if left_diff < right_diff:
-                ix -= 1
-        return Fraction(int(self.num[ix]), int(self.den[ix])) + Fraction(quo)
+from __future__ import annotations
+
+from bisect import bisect_left
+from fractions import Fraction
+from typing import Iterable
+
+import numpy as np
+
+from reamber.algorithms.timing.utils.conf import DEFAULT_DIVISIONS
+
+
+def snap(value: float,
+         divisions: Iterable[int] = DEFAULT_DIVISIONS) -> Fraction:
+    """Snaps float value to closest division.
+
+    Args:
+        value: Value to snap
+        divisions: Divisions to accept
+    """
+    return Snapper(divisions=divisions).snap(value)
+
+
+class Snapper:
+    def __init__(self, divisions: Iterable[int] = DEFAULT_DIVISIONS):
+        """Initialize Snapper with defined divisions
+
+        Args:
+            divisions: Divisions acceptable when snapping
+        """
+        divisions = np.asarray(divisions)
+        max_slots = max(divisions)
+
+        # Creates the division triangle
+        den, num = np.indices([max_slots, max_slots])
+        den += 1
+        ar = num / den
+
+        ar[np.triu_indices(ar.shape[0], 1)] = np.nan
+        ar[1:, 0] = np.nan
+        # Prunes the repeated slots
+        visited = set()
+        for i in range(1, max_slots):
+            for j in range(1, i + 1):
+                if ar[i, j] in visited:
+                    ar[i, j] = np.nan
+                else:
+                    visited.add(ar[i, j])
+
+        # Add numerator & denominator
+        ar = np.stack([ar, num, den])
+        ar = ar[:, ~np.isnan(ar[0])].T
+        sorter = ar[:, 0].argsort()
+
+        # Add the case for 1/1 so that 0.9999... matches that
+        ar = np.vstack([ar[sorter], [1, 1, 1]])
+
+        self.val = ar[:, 0]
+        self.num = ar[:, 1]
+        self.den = ar[:, 2]
+
+    def snap(self, beat: float) -> Fraction:
+        """Snaps beat to nearest division"""
+        quo, rem = beat // 1, beat % 1
+        ix = bisect_left(self.val, rem)
+
+        # Bisect Left gets the next value
+        # E.g. [0, 0.5], bisect_left(ar, 0.0001) = 1, bisect_left(ar, 0) = 0,
+        if ix != 0:
+            left_diff, right_diff = \
+                rem - self.val[ix - 1], self.val[ix] - rem
+            if left_diff < right_diff:
+                ix -= 1
+        return Fraction(int(self.num[ix]), int(self.den[ix])) + Fraction(quo)
```

### Comparing `reamber-0.1.7/reamber/algorithms/timing/utils/bpm_changes_offset_to_snap.py` & `reamber-0.1.8/reamber/algorithms/timing/utils/bpm_changes_offset_to_snap.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from __future__ import annotations
-
-from typing import List
-
-from reamber.algorithms.timing.utils.BpmChangeOffset import BpmChangeOffset
-from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
-from reamber.algorithms.timing.utils.Snapper import Snapper
-from reamber.algorithms.timing.utils.snap import Snap
-
-
-def bpm_changes_offset_to_snap(bco_s: List[BpmChangeOffset],
-                               snapper: Snapper) -> List[BpmChangeSnap]:
-    """Creates Timing Map from bpm changes in offset
-
-    Args:
-        bco_s: BpmChange as Offsets to convert
-        snapper: Snapping helper to snap offsets.
-    """
-    bco_s.sort(key=lambda x: x.offset)
-    parent_bco = bco_s[0]
-
-    prev_snap = Snap(0, 0, parent_bco.metronome)
-    bcs_s: List[BpmChangeSnap] = [
-        BpmChangeSnap(bco_s[0].bpm,
-                      bco_s[0].metronome,
-                      snap=prev_snap)
-    ]
-    for parent_bco, child_bco in zip(bco_s[:-1], bco_s[1:]):
-        snap = Snap.from_offset(child_bco.offset,
-                                parent_bco,
-                                bcs_s[-1],
-                                snapper)
-        snap.metronome = child_bco.metronome
-        bcs_s.append(
-            BpmChangeSnap(
-                bpm=child_bco.bpm,
-                metronome=child_bco.metronome,
-                snap=snap
-            )
-        )
-
-    return bcs_s
+from __future__ import annotations
+
+from typing import List
+
+from reamber.algorithms.timing.utils.BpmChangeOffset import BpmChangeOffset
+from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
+from reamber.algorithms.timing.utils.Snapper import Snapper
+from reamber.algorithms.timing.utils.snap import Snap
+
+
+def bpm_changes_offset_to_snap(bco_s: List[BpmChangeOffset],
+                               snapper: Snapper) -> List[BpmChangeSnap]:
+    """Creates Timing Map from bpm changes in offset
+
+    Args:
+        bco_s: BpmChange as Offsets to convert
+        snapper: Snapping helper to snap offsets.
+    """
+    bco_s.sort(key=lambda x: x.offset)
+    parent_bco = bco_s[0]
+
+    prev_snap = Snap(0, 0, parent_bco.metronome)
+    bcs_s: List[BpmChangeSnap] = [
+        BpmChangeSnap(bco_s[0].bpm,
+                      bco_s[0].metronome,
+                      snap=prev_snap)
+    ]
+    for parent_bco, child_bco in zip(bco_s[:-1], bco_s[1:]):
+        snap = Snap.from_offset(child_bco.offset,
+                                parent_bco,
+                                bcs_s[-1],
+                                snapper)
+        snap.metronome = child_bco.metronome
+        bcs_s.append(
+            BpmChangeSnap(
+                bpm=child_bco.bpm,
+                metronome=child_bco.metronome,
+                snap=snap
+            )
+        )
+
+    return bcs_s
```

### Comparing `reamber-0.1.7/reamber/algorithms/timing/utils/reseat_bpm_changes_snap.py` & `reamber-0.1.8/reamber/algorithms/timing/utils/reseat_bpm_changes_snap.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,110 +1,110 @@
-from __future__ import annotations
-
-from copy import deepcopy
-from typing import List
-
-from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
-from reamber.algorithms.timing.utils.snap import Snap
-
-
-def reseat_bpm_changes_snap(
-    bcs_s: List[BpmChangeSnap],
-    extend_threshold: float = 0.001
-) -> List[BpmChangeSnap]:
-    """Force all bpm changes to be on metronome
-
-    Notes:
-        The case where extend is used.
-        BPM 60000, Offset 0     , Metronome 4
-        BPM 60000, Offset 4.0001, Metronome 4
-
-        Instead of adding a BPM on Offset 4, we simply change the first BPM.
-        This prevents the case of a super high bpm.
-
-    Args:
-        bcs_s: Bpm Changes to reseat
-        extend_threshold: Fraction of Measure to accept extending a late BPM
-
-    Notes:
-        1st BPM Change MUST be on Measure, Beat, Slot 0.
-    """
-    bcs_s = deepcopy(bcs_s)
-    bcs_s.sort(key=lambda x: x.snap)
-
-    offset = 0
-    offsets = [0, ]
-    for bcs_0, bcs_1 in zip(bcs_s[:-1], bcs_s[1:]):
-        diff = (bcs_1.snap - bcs_0.snap).offset(bcs_0)
-        offset += diff
-        offsets.append(offset)
-
-    i = 0
-    measure = 0
-
-    while i != len(bcs_s) - 1:
-        bcs_0, bcs_1 = bcs_s[i], bcs_s[i + 1]
-        offset_0, offset_1 = offsets[i], offsets[i + 1]
-        offset_diff = offset_1 - offset_0
-        measure_diff = offset_diff / bcs_0.measure_length
-        beat_diff = offset_diff / bcs_0.beat_length
-        beat_diff_quo = beat_diff // 1
-        beat_diff_rem = beat_diff % 1
-        measure_diff_quo = measure_diff // 1
-        measure_diff_rem = measure_diff % 1
-        measure += measure_diff_quo
-
-        # BCS_0 is guaranteed to be on a measure.
-        # Extend case, see docstring
-        if 0 < measure_diff_rem <= extend_threshold:
-            # Extend by nudging bpm
-            bcs = BpmChangeSnap(bcs_0.bpm / (measure_diff_rem + 1),
-                                bcs_0.metronome,
-                                Snap(measure - 1, 0, bcs_0.metronome))
-            offset = (measure_diff_quo - 1) * bcs_0.measure_length + offset_0
-            if measure_diff_quo == 1:
-                bcs_s[i] = bcs
-                offsets[i] = offset
-            else:
-                measure -= 1
-                bcs_s.insert(i + 1, bcs)
-                offsets.insert(i + 1, offset)
-
-        # Extend case, see docstring
-        elif 0 < beat_diff_rem <= extend_threshold:
-            # Check if it's possible to extend by changing metronome
-            metronome = beat_diff_quo % bcs_0.metronome
-            bcs = BpmChangeSnap(
-                bcs_0.bpm / ((beat_diff_rem + metronome) / metronome),
-                metronome,
-                Snap(measure, 0, metronome)
-            )
-            offset = offset_1 - metronome * bcs_0.beat_length
-
-            if measure_diff_quo == 0:
-                # Modify prev bpm
-                bcs_s[i] = bcs
-                offsets[i] = offset
-                measure += 1
-            else:
-                bcs_s.insert(i + 1, bcs)
-                offsets.insert(i + 1, offset)
-
-        elif measure_diff_rem > extend_threshold:
-            # This means it's not possible to simply extend
-            bcs = BpmChangeSnap(bcs_0.bpm / measure_diff_rem,
-                                bcs_0.metronome,
-                                Snap(measure, 0, bcs_0.metronome))
-            offset = measure_diff_quo * bcs_0.measure_length + offset_0
-            if measure_diff_quo == 0:
-                bcs_s[i] = bcs
-                offsets[i] = offset
-                measure += 1
-            else:
-                bcs_s.insert(i + 1, bcs)
-                offsets.insert(i + 1, offset)
-
-        bcs_s[i + 1].snap.measure = measure
-        bcs_s[i + 1].snap.beat = 0
-        i += 1
-
-    return bcs_s
+from __future__ import annotations
+
+from copy import deepcopy
+from typing import List
+
+from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
+from reamber.algorithms.timing.utils.snap import Snap
+
+
+def reseat_bpm_changes_snap(
+    bcs_s: List[BpmChangeSnap],
+    extend_threshold: float = 0.001
+) -> List[BpmChangeSnap]:
+    """Force all bpm changes to be on metronome
+
+    Notes:
+        The case where extend is used.
+        BPM 60000, Offset 0     , Metronome 4
+        BPM 60000, Offset 4.0001, Metronome 4
+
+        Instead of adding a BPM on Offset 4, we simply change the first BPM.
+        This prevents the case of a super high bpm.
+
+    Args:
+        bcs_s: Bpm Changes to reseat
+        extend_threshold: Fraction of Measure to accept extending a late BPM
+
+    Notes:
+        1st BPM Change MUST be on Measure, Beat, Slot 0.
+    """
+    bcs_s = deepcopy(bcs_s)
+    bcs_s.sort(key=lambda x: x.snap)
+
+    offset = 0
+    offsets = [0, ]
+    for bcs_0, bcs_1 in zip(bcs_s[:-1], bcs_s[1:]):
+        diff = (bcs_1.snap - bcs_0.snap).offset(bcs_0)
+        offset += diff
+        offsets.append(offset)
+
+    i = 0
+    measure = 0
+
+    while i != len(bcs_s) - 1:
+        bcs_0, bcs_1 = bcs_s[i], bcs_s[i + 1]
+        offset_0, offset_1 = offsets[i], offsets[i + 1]
+        offset_diff = offset_1 - offset_0
+        measure_diff = offset_diff / bcs_0.measure_length
+        beat_diff = offset_diff / bcs_0.beat_length
+        beat_diff_quo = beat_diff // 1
+        beat_diff_rem = beat_diff % 1
+        measure_diff_quo = measure_diff // 1
+        measure_diff_rem = measure_diff % 1
+        measure += measure_diff_quo
+
+        # BCS_0 is guaranteed to be on a measure.
+        # Extend case, see docstring
+        if 0 < measure_diff_rem <= extend_threshold:
+            # Extend by nudging bpm
+            bcs = BpmChangeSnap(bcs_0.bpm / (measure_diff_rem + 1),
+                                bcs_0.metronome,
+                                Snap(measure - 1, 0, bcs_0.metronome))
+            offset = (measure_diff_quo - 1) * bcs_0.measure_length + offset_0
+            if measure_diff_quo == 1:
+                bcs_s[i] = bcs
+                offsets[i] = offset
+            else:
+                measure -= 1
+                bcs_s.insert(i + 1, bcs)
+                offsets.insert(i + 1, offset)
+
+        # Extend case, see docstring
+        elif 0 < beat_diff_rem <= extend_threshold:
+            # Check if it's possible to extend by changing metronome
+            metronome = beat_diff_quo % bcs_0.metronome
+            bcs = BpmChangeSnap(
+                bcs_0.bpm / ((beat_diff_rem + metronome) / metronome),
+                metronome,
+                Snap(measure, 0, metronome)
+            )
+            offset = offset_1 - metronome * bcs_0.beat_length
+
+            if measure_diff_quo == 0:
+                # Modify prev bpm
+                bcs_s[i] = bcs
+                offsets[i] = offset
+                measure += 1
+            else:
+                bcs_s.insert(i + 1, bcs)
+                offsets.insert(i + 1, offset)
+
+        elif measure_diff_rem > extend_threshold:
+            # This means it's not possible to simply extend
+            bcs = BpmChangeSnap(bcs_0.bpm / measure_diff_rem,
+                                bcs_0.metronome,
+                                Snap(measure, 0, bcs_0.metronome))
+            offset = measure_diff_quo * bcs_0.measure_length + offset_0
+            if measure_diff_quo == 0:
+                bcs_s[i] = bcs
+                offsets[i] = offset
+                measure += 1
+            else:
+                bcs_s.insert(i + 1, bcs)
+                offsets.insert(i + 1, offset)
+
+        bcs_s[i + 1].snap.measure = measure
+        bcs_s[i + 1].snap.beat = 0
+        i += 1
+
+    return bcs_s
```

### Comparing `reamber-0.1.7/reamber/algorithms/timing/utils/snap.py` & `reamber-0.1.8/reamber/algorithms/timing/utils/snap.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from fractions import Fraction
-from functools import total_ordering
-from typing import TYPE_CHECKING
-
-from reamber.algorithms.timing.utils.BpmChangeBase import BpmChangeBase
-from reamber.algorithms.timing.utils.BpmChangeOffset import BpmChangeOffset
-from reamber.algorithms.timing.utils.Snapper import Snapper
-
-if TYPE_CHECKING:
-    from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
-
-
-@total_ordering
-@dataclass(unsafe_hash=True)
-class Snap:
-    measure: int
-    beat: Fraction | float
-    # If metronome is none, don't correct anything
-    metronome: Fraction | float | None
-
-    def __post_init__(self):
-        if self.metronome is None: return
-        if self.measure < 0:
-            self.beat += self.measure * self.metronome
-        if (self.beat < 0) or (self.beat >= self.metronome):
-            self.measure += self.beat // self.metronome
-            self.beat %= Fraction(self.metronome)
-
-        if (self.beat < 0) or (self.measure < 0):
-            raise ValueError("Failed to yield positive Snap")
-
-        self.beat = Fraction(self.beat)
-
-    def __eq__(self, other: Snap):
-        return self.measure == other.measure and self.beat == other.beat
-
-    def __lt__(self, other: Snap):
-        return self.measure < other.measure or \
-               (self.measure == other.measure and self.beat < other.beat)
-
-    def __sub__(self, other: Snap):
-        return Snap(
-            self.measure - other.measure,
-            self.beat - other.beat,
-            other.metronome
-        )
-
-    def __add__(self, other: Snap):
-        return Snap(
-            self.measure + other.measure,
-            self.beat + other.beat,
-            self.metronome
-        )
-
-    def offset(self, bpm_active: BpmChangeBase):
-        return (
-            bpm_active.measure_length * self.measure +
-            bpm_active.beat_length * self.beat
-        )
-
-    @staticmethod
-    def from_offset(offset: float,
-                    bco: BpmChangeOffset,
-                    bcs: BpmChangeSnap,
-                    snapper: Snapper) -> Snap:
-        """Calculate Snap from offset
-
-        Args:
-            offset: Offset to calculate from
-            bco: The current active BpmChangeOffset
-            bcs: The current active BpmChangeSnap
-            snapper: Snapper helper instance
-        """
-        offset_del = offset - bco.offset
-        measure = int(offset_del // bco.measure_length)
-        offset_del -= measure * bco.measure_length
-        beat = snapper.snap(offset_del / bco.beat_length)
-        return Snap(measure + bcs.snap.measure,
-                    beat + bcs.snap.beat, bco.metronome)
-
-    def __repr__(self):
-        return f"{self.measure}.{self.beat} / {self.metronome}"
+from __future__ import annotations
+
+from dataclasses import dataclass
+from fractions import Fraction
+from functools import total_ordering
+from typing import TYPE_CHECKING
+
+from reamber.algorithms.timing.utils.BpmChangeBase import BpmChangeBase
+from reamber.algorithms.timing.utils.BpmChangeOffset import BpmChangeOffset
+from reamber.algorithms.timing.utils.Snapper import Snapper
+
+if TYPE_CHECKING:
+    from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
+
+
+@total_ordering
+@dataclass(unsafe_hash=True)
+class Snap:
+    measure: int
+    beat: Fraction | float
+    # If metronome is none, don't correct anything
+    metronome: Fraction | float | None
+
+    def __post_init__(self):
+        if self.metronome is None: return
+        if self.measure < 0:
+            self.beat += self.measure * self.metronome
+        if (self.beat < 0) or (self.beat >= self.metronome):
+            self.measure += self.beat // self.metronome
+            self.beat %= Fraction(self.metronome)
+
+        if (self.beat < 0) or (self.measure < 0):
+            raise ValueError("Failed to yield positive Snap")
+
+        self.beat = Fraction(self.beat)
+
+    def __eq__(self, other: Snap):
+        return self.measure == other.measure and self.beat == other.beat
+
+    def __lt__(self, other: Snap):
+        return self.measure < other.measure or \
+               (self.measure == other.measure and self.beat < other.beat)
+
+    def __sub__(self, other: Snap):
+        return Snap(
+            self.measure - other.measure,
+            self.beat - other.beat,
+            other.metronome
+        )
+
+    def __add__(self, other: Snap):
+        return Snap(
+            self.measure + other.measure,
+            self.beat + other.beat,
+            self.metronome
+        )
+
+    def offset(self, bpm_active: BpmChangeBase):
+        return (
+            bpm_active.measure_length * self.measure +
+            bpm_active.beat_length * self.beat
+        )
+
+    @staticmethod
+    def from_offset(offset: float,
+                    bco: BpmChangeOffset,
+                    bcs: BpmChangeSnap,
+                    snapper: Snapper) -> Snap:
+        """Calculate Snap from offset
+
+        Args:
+            offset: Offset to calculate from
+            bco: The current active BpmChangeOffset
+            bcs: The current active BpmChangeSnap
+            snapper: Snapper helper instance
+        """
+        offset_del = offset - bco.offset
+        measure = int(offset_del // bco.measure_length)
+        offset_del -= measure * bco.measure_length
+        beat = snapper.snap(offset_del / bco.beat_length)
+        return Snap(measure + bcs.snap.measure,
+                    beat + bcs.snap.beat, bco.metronome)
+
+    def __repr__(self):
+        return f"{self.measure}.{self.beat} / {self.metronome}"
```

### Comparing `reamber-0.1.7/reamber/base/Bpm.py` & `reamber-0.1.8/reamber/base/Bpm.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from __future__ import annotations
-
-from reamber.base.Property import item_props
-from reamber.base.RAConst import RAConst
-from reamber.base.Timed import Timed
-
-
-@item_props()
-class Bpm(Timed):
-    """A non-playable timed object indicating tempo of the map.
-
-    Notes:
-        This should not be used directly, instead, use subclassed Bpm classes
-        specific for games. Such as ``OsuBpm`` or ``QuaBpm``.
-
-    Examples:
-
-        >>> b = Bpm(offset=1000, bpm=200, metronome=4)
-        >>> b.offset, b.bpm, b.metronome
-        (1000, 200, 4)
-
-        >>> b.beat_length
-        300.0
-
-        >>> b.metronome_length
-        1200.0
-    """
-
-    _props = dict(bpm=['float', 0.0],
-                  metronome=['float', 4.0])
-
-    def __init__(self, offset: float, bpm: float, metronome: float = 4,
-                 **kwargs):
-        """Initializer
-
-        Args:
-            offset: offset in ms
-            bpm: BPM in beats per minute
-            metronome: Metronome, can be float
-        """
-        super().__init__(offset=offset, bpm=bpm, metronome=metronome, **kwargs)
-
-    @property
-    def beat_length(self) -> float:
-        """Get duration of each beat in ms
-
-        Examples:
-
-            >>> Bpm(offset=0, bpm=200, metronome=4).beat_length
-            300.0
-        """
-        return RAConst.min_to_msec(1.0 / self.bpm)
-
-    @property
-    def metronome_length(self) -> float:
-        """Get duration of each metronome in ms
-
-        Notes:
-            This is simply the ``beat_length`` * ``metronome``
-
-        Examples:
-
-            >>> Bpm(offset=0, bpm=200, metronome=4).metronome_length
-            1200.0
-        """
-        return self.beat_length * self.metronome
+from __future__ import annotations
+
+from reamber.base.Property import item_props
+from reamber.base.RAConst import RAConst
+from reamber.base.Timed import Timed
+
+
+@item_props()
+class Bpm(Timed):
+    """A non-playable timed object indicating tempo of the map.
+
+    Notes:
+        This should not be used directly, instead, use subclassed Bpm classes
+        specific for games. Such as ``OsuBpm`` or ``QuaBpm``.
+
+    Examples:
+
+        >>> b = Bpm(offset=1000, bpm=200, metronome=4)
+        >>> b.offset, b.bpm, b.metronome
+        (1000, 200, 4)
+
+        >>> b.beat_length
+        300.0
+
+        >>> b.metronome_length
+        1200.0
+    """
+
+    _props = dict(bpm=['float', 0.0],
+                  metronome=['float', 4.0])
+
+    def __init__(self, offset: float, bpm: float, metronome: float = 4,
+                 **kwargs):
+        """Initializer
+
+        Args:
+            offset: offset in ms
+            bpm: BPM in beats per minute
+            metronome: Metronome, can be float
+        """
+        super().__init__(offset=offset, bpm=bpm, metronome=metronome, **kwargs)
+
+    @property
+    def beat_length(self) -> float:
+        """Get duration of each beat in ms
+
+        Examples:
+
+            >>> Bpm(offset=0, bpm=200, metronome=4).beat_length
+            300.0
+        """
+        return RAConst.min_to_msec(1.0 / self.bpm)
+
+    @property
+    def metronome_length(self) -> float:
+        """Get duration of each metronome in ms
+
+        Notes:
+            This is simply the ``beat_length`` * ``metronome``
+
+        Examples:
+
+            >>> Bpm(offset=0, bpm=200, metronome=4).metronome_length
+            1200.0
+        """
+        return self.beat_length * self.metronome
```

### Comparing `reamber-0.1.7/reamber/base/Hold.py` & `reamber-0.1.8/reamber/base/Hold.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from __future__ import annotations
-
-from reamber.base.Note import Note
-from reamber.base.Property import item_props
-
-
-@item_props()
-class HoldTail(Note):
-    """A dummy class for tail detection APIs
-
-    ``HoldTail`` is entirely independent of ``Hold``.
-
-    Notes:
-        This is currently only used in the ``Pattern`` algorithm
-    """
-
-    _props = dict(length=['float', 0.0])
-
-    def __init__(self, offset: float, column: int, length: float, **kwargs):
-        """Initializer
-
-        Args:
-            offset: Offset in ms
-            column: Column of Tail, should be same as ``Hold``
-            length: Length of Hold, should be same as ``Hold``
-        """
-        super().__init__(offset=offset, column=column, length=length, **kwargs)
-
-
-@item_props()
-class Hold(Note):
-    """A held timed object with a length.
-
-    Notes:
-        We only store the length, the tail offset is calculated.
-        We inherit ``Note`` instead of ``Hit``
-
-    Examples:
-
-        >>> h = Hold(offset=1000, column=1, length=1000)
-        >>> h.tail_offset
-        2000
-    """
-
-    _props = dict(length=['float', 0.0])
-
-    def __init__(self, offset: float, column: int, length: float, **kwargs):
-        """Initializer
-
-        Args:
-            offset: Offset in ms
-            column: Column
-            length: Length in ms
-        """
-        super().__init__(offset=offset, column=column, length=length, **kwargs)
-
-    @property
-    def tail_offset(self) -> float:
-        """Offset of the tail in ms
-
-        Notes:
-            This is simply ``offset`` + ``length``
-
-        Returns:
-            ``float`` of Tail offset in ms
-
-        """
-        return self.offset + self.length
+from __future__ import annotations
+
+from reamber.base.Note import Note
+from reamber.base.Property import item_props
+
+
+@item_props()
+class HoldTail(Note):
+    """A dummy class for tail detection APIs
+
+    ``HoldTail`` is entirely independent of ``Hold``.
+
+    Notes:
+        This is currently only used in the ``Pattern`` algorithm
+    """
+
+    _props = dict(length=['float', 0.0])
+
+    def __init__(self, offset: float, column: int, length: float, **kwargs):
+        """Initializer
+
+        Args:
+            offset: Offset in ms
+            column: Column of Tail, should be same as ``Hold``
+            length: Length of Hold, should be same as ``Hold``
+        """
+        super().__init__(offset=offset, column=column, length=length, **kwargs)
+
+
+@item_props()
+class Hold(Note):
+    """A held timed object with a length.
+
+    Notes:
+        We only store the length, the tail offset is calculated.
+        We inherit ``Note`` instead of ``Hit``
+
+    Examples:
+
+        >>> h = Hold(offset=1000, column=1, length=1000)
+        >>> h.tail_offset
+        2000
+    """
+
+    _props = dict(length=['float', 0.0])
+
+    def __init__(self, offset: float, column: int, length: float, **kwargs):
+        """Initializer
+
+        Args:
+            offset: Offset in ms
+            column: Column
+            length: Length in ms
+        """
+        super().__init__(offset=offset, column=column, length=length, **kwargs)
+
+    @property
+    def tail_offset(self) -> float:
+        """Offset of the tail in ms
+
+        Notes:
+            This is simply ``offset`` + ``length``
+
+        Returns:
+            ``float`` of Tail offset in ms
+
+        """
+        return self.offset + self.length
```

### Comparing `reamber-0.1.7/reamber/base/Hold.pyi` & `reamber-0.1.8/reamber/base/Hold.pyi`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from __future__ import annotations
-
-from reamber.base.Note import Note
-
-
-class HoldTail(Note):
-
-    def __init__(self, offset: float, column: int, length: float, **kwargs): ...
-    @property
-    def length(self) -> float: ...
-    @length.setter
-    def length(self, val) -> None: ...
-
-
-class Hold(Note):
-
-    def __init__(self, offset: float, column: int, length: float, **kwargs): ...
-    @property
-    def length(self) -> float: ...
-    @length.setter
-    def length(self, val) -> None: ...
-    @property
-    def tail_offset(self) -> float: ...
-
+from __future__ import annotations
+
+from reamber.base.Note import Note
+
+
+class HoldTail(Note):
+
+    def __init__(self, offset: float, column: int, length: float, **kwargs): ...
+    @property
+    def length(self) -> float: ...
+    @length.setter
+    def length(self, val) -> None: ...
+
+
+class Hold(Note):
+
+    def __init__(self, offset: float, column: int, length: float, **kwargs): ...
+    @property
+    def length(self) -> float: ...
+    @length.setter
+    def length(self, val) -> None: ...
+    @property
+    def tail_offset(self) -> float: ...
+
```

### Comparing `reamber-0.1.7/reamber/base/Map.py` & `reamber-0.1.8/reamber/base/Map.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,335 +1,335 @@
-from __future__ import annotations
-
-import datetime
-from copy import deepcopy
-from dataclasses import dataclass, field
-from typing import List, Dict, Type, Generic, Tuple
-from typing import TypeVar
-
-import pandas as pd
-from pandas.core.indexing import _LocIndexer
-
-from reamber.base.Property import stack_props, map_props
-from reamber.base.lists.BpmList import BpmList
-from reamber.base.lists.TimedList import TimedList
-from reamber.base.lists.notes.HitList import HitList
-from reamber.base.lists.notes.HoldList import HoldList
-from reamber.base.lists.notes.NoteList import NoteList
-
-NoteListT = TypeVar('NoteListT', bound=NoteList)
-HitListT = TypeVar('HitListT', bound=HitList)
-HoldListT = TypeVar('HoldListT', bound=HoldList)
-BpmListT = TypeVar('BpmListT', bound=BpmList)
-
-T = TypeVar('T', bound=TimedList)
-
-
-@dataclass
-@map_props()
-class Map(Generic[NoteListT, HitListT, HoldListT, BpmListT]):
-    """This class should be inherited by all Map Objects
-
-    They must inherit the data method, which extracts all data they hold.
-    They are also assumed to be a TimedList.
-    """
-
-    _props = dict(hits=HitList, holds=HoldList, bpms=BpmList)
-
-    # objs is the objects of the class, it MUST be defined,
-    # and must have defaults as ([]).
-    objs: Dict[str, TimedList] = \
-        field(init=False,
-              default_factory=
-              lambda: dict(
-                  hits=HitList([]),
-                  holds=HoldList([]),
-                  bpms=BpmList([]))
-              )
-
-    def __getitem__(self, item: Type[T]) -> List[Type[T]]:
-        li = [o for o in self.objs.values() if isinstance(o, item)]
-        if li:
-            return li
-        else:
-            raise IndexError(f"Object of type {item} does not exist.")
-
-    def __setitem__(self, key: T, value: List[Type[T]]):
-        this = self.__getitem__(key)
-        assert len(this) == len(
-            value), "The lengths of the set and get must be the same."
-        for i in range(len(this)):
-            # noinspection PyTypeChecker
-            this[i] = value[i]
-
-    @property
-    def notes(self):
-        return self[NoteList]
-
-    # noinspection PyUnresolvedReferences
-    @notes.setter
-    def notes(self, val):
-        for i in range(len(val)):
-            self[NoteList][i] = val[i]
-
-    def deepcopy(self) -> Map:
-        """Returns a deep copy of itself"""
-        return deepcopy(self)
-
-    # @abstractmethod
-    def metadata(self, unicode=True, **kwargs) -> str:
-        """Grabs the map metadata
-
-        Notes:
-            This doesn't try to convert unicode to ascii.
-        Args:
-            unicode: Whether to use unicode if available.
-
-        Returns:
-            A string containing the metadata
-        """
-        ...
-
-    def describe(self,
-                 rounding: int = 2,
-                 unicode: bool = False,
-                 **kwargs) -> str:
-        """Describes the map's attributes as a short summary
-
-        Examples:
-
-            >>> from reamber.base import Hit, Bpm
-            >>> bpms = [Bpm(offset=1000, bpm=120)]
-            >>> hits = [Hit(offset=1000, column=1),
-            ...         Hit(offset=2000, column=2)]
-            >>> m = Map()
-            >>> m.hits = HitList(hits)
-            >>> m.bpms = BpmList(bpms)
-            >>> m.describe() # doctest: +ELLIPSIS
-            "..."
-
-        Args:
-            rounding: The decimal rounding
-            unicode: Whether to use unicode if available.
-        """
-
-        first = min([nl.first_offset() for nl in self[NoteList] if nl])
-        last = max([nl.last_offset() for nl in self[NoteList] if nl])
-
-        out = f"Average BPM: " \
-              f"{round(self[BpmList][0].ave_bpm(last), rounding)}\n" \
-              f"Map Length: " \
-              f"{datetime.timedelta(milliseconds=last - first)}\n" \
-              f"{self.metadata(unicode=unicode, **kwargs)} + \n\n" \
-              f"--- Notes ---\n"
-
-        for n in self[NoteList]:
-            n: TimedList
-            out += f"{n.__class__.__name__}\n" \
-                   f"{n.df.columns}\n" \
-                   f"{n.df.describe()}\n\n"
-        return out
-
-    def rate(self, by: float) -> Map:
-        """Changes the rate of the map
-
-        Examples:
-            The following will uprate the map by 10%
-
-            >>> Map().rate(1.1) # doctest: +ELLIPSIS
-            Map(...)
-
-        Args:
-            by: The rate.
-        """
-
-        copy = self.deepcopy()
-        stack = copy.stack()
-        stack.offset /= by
-        stack.bpm *= by
-        stack.length /= by
-        return copy
-
-    @stack_props()
-    class Stacker:
-        """Stacking merges multiple ``TimedList`` to map operations on them.
-
-        The internal data class is a ``pd.DataFrame``.
-
-        Examples:
-
-            >>> from reamber.base import Hit
-            >>> hits = [Hit(offset=1000, column=1),
-            ...         Hit(offset=2000, column=2)]
-            >>> m = Map()
-            >>> m.hits = HitList(hits)
-            >>> stack = m.stack()
-
-            Multiply all offsets in the map by 2
-
-            >>> stack.offset *= 2
-            >>> stack.offset.tolist()
-            [2000.0, 4000.0]
-
-            Or if you do it inline,
-
-            >>> m.stack().offset *= 2
-            >>> m.hits.offset.tolist()
-            [4000.0, 8000.0]
-
-            Notice that ``stack`` changes the map directly by reference.
-
-            If the property, like ``column``, doesn't exist for ``Bpm``,
-            it will simply skip it for ``Bpm``.
-
-            However, all properties must exist at least once.
-
-            For example,
-
-            >>> try:
-            ...     stack.does_not_exist *= 2
-            ... except Excepti  on:
-            ...     print("No such property")
-            No such property
-
-            The internal data class is a ``pd.DataFrame``:
-
-            >>> hits = [Hit(offset=1000, column=1),
-            ...         Hit(offset=2000, column=2),
-            ...         Hit(offset=3000, column=3)]
-            >>> m = Map()
-            >>> m.hits = HitList(hits)
-            >>> stack = m.stack()
-            >>> stack.offset[stack.column < 2].tolist()
-            [1000.0]
-
-            >>> stack.offset[stack.column > 1].tolist()
-            [2000.0, 3000.0]
-
-            If you need more conditions, use ``loc``
-        """
-
-        """We concat all dfs and do operations on the joined df. 
-        However, concat of dfs will always be deep copied.
-        Thus, any updates to the concat needs to update the original list 
-        
-        LISTS ---STACK---> COPY ---> STACKED
-          +---------- REFERENCE ---> UNSTACKED  
-        
-        To do so, we track of the links between unstacked and stacked by ix.
-        
-        IXS        |         |          |    |     |
-        UNSTACKED  [........] [........] [..] [....]
-        STACKED    [...............................]
-        
-        So any operation will affect the stacked, 
-        any mutation will call _update, updating unstacked.
-        
-        """
-
-        _ixs: List[int]
-        _unstacked: List[TimedList]
-
-        # This is concat of all lists, making common ops possible.
-        _stacked: pd.DataFrame
-
-        def __init__(self, objs: List[TimedList]):
-            ixs: List = [0]
-            for obj in objs:
-                ixs.append(ixs[-1] + len(obj))
-            self._ixs = ixs
-            self._unstacked = objs
-            self._stacked = pd.concat(
-                [v.df for v in self._unstacked]
-            ).reset_index()
-
-        @property
-        def loc(self) -> StackerLocIndexer:
-            """Loc is used when basic indexing is insufficient.
-
-            Notes:
-                This is similar to how ``pandas`` uses ``loc``.
-                You may assume the same syntax.
-
-            Examples:
-                >>> from reamber.base import Hit
-                >>> hits = [Hit(offset=1000, column=1),
-                ...         Hit(offset=2000, column=2),
-                ...         Hit(offset=3000, column=3)]
-                >>> m = Map()
-                >>> m.hits = HitList(hits)
-                >>> stack = m.stack()
-
-                >>> stack.loc[stack.offset > 1000, 'column'] += 1
-                >>> m.hits.column.tolist()
-                [1.0, 3.0, 4.0]
-
-                >>> stack.loc[
-                ...     (stack.column == 1) & (stack.offset <= 1000),
-                ...     ['offset']
-                ... ] *= 2
-                >>> m.hits.offset.tolist()
-                [2000.0, 2000.0, 3000.0]
-
-            """
-            return self.StackerLocIndexer(self._stacked.loc, self)
-
-        def _update(self):
-            for obj, ix_i, ix_j in zip(
-                self._unstacked, self._ixs[:-1], self._ixs[1:]
-            ):
-                obj.df = self._stacked[obj.df.columns].iloc[ix_i:ix_j]
-
-        def __getitem__(self, item):
-            return self._stacked[item]
-
-        def __setitem__(self, key, value):
-            self._stacked[key] = value
-            self._update()
-
-        _props = ['offset', 'column', 'length', 'bpm', 'metronome']
-
-        @dataclass
-        class StackerLocIndexer:
-            """Class generated with ``Stacker.loc``
-
-            Notes:
-                See Documentation in ``Stacker.loc`` on usage.
-            """
-            loc: _LocIndexer
-            stacker: Map.Stacker
-
-            def __setitem__(self, key, value):
-                self.loc.__setitem__(key, value)
-                self.stacker._update()
-
-            def __getitem__(self, item):
-                return self.loc.__getitem__(item)
-
-    def stack(self, include_types: Tuple[Type[T]] = None) -> Stacker:
-        """Stacks map and includes specific columns
-
-        Examples:
-            This will generate a stacker ``stack``
-
-            >>> from reamber.base import Hit
-            >>> hits = [Hit(offset=1000, column=1),
-            ...         Hit(offset=2000, column=2),
-            ...         Hit(offset=3000, column=3)]
-            >>> m = Map()
-            >>> m.hits = HitList(hits)
-            >>> m.stack() # doctest: +ELLIPSIS
-            <Map.Map.Stacker ...>
-
-        Returns:
-            A ``Map.Stacker`` instance. This is a pass by reference.
-            Thus, modifications on the stack will change the map directly.
-
-        """
-
-        if include_types is None:
-            objs = [v for v in self.objs.values()]
-        else:
-            # noinspection PyTypeHints
-            objs = [v for v in self.objs.values()
-                    if isinstance(v, include_types)]
-        return self.Stacker(objs)
+from __future__ import annotations
+
+import datetime
+from copy import deepcopy
+from dataclasses import dataclass, field
+from typing import List, Dict, Type, Generic, Tuple
+from typing import TypeVar
+
+import pandas as pd
+from pandas.core.indexing import _LocIndexer
+
+from reamber.base.Property import stack_props, map_props
+from reamber.base.lists.BpmList import BpmList
+from reamber.base.lists.TimedList import TimedList
+from reamber.base.lists.notes.HitList import HitList
+from reamber.base.lists.notes.HoldList import HoldList
+from reamber.base.lists.notes.NoteList import NoteList
+
+NoteListT = TypeVar('NoteListT', bound=NoteList)
+HitListT = TypeVar('HitListT', bound=HitList)
+HoldListT = TypeVar('HoldListT', bound=HoldList)
+BpmListT = TypeVar('BpmListT', bound=BpmList)
+
+T = TypeVar('T', bound=TimedList)
+
+
+@dataclass
+@map_props()
+class Map(Generic[NoteListT, HitListT, HoldListT, BpmListT]):
+    """This class should be inherited by all Map Objects
+
+    They must inherit the data method, which extracts all data they hold.
+    They are also assumed to be a TimedList.
+    """
+
+    _props = dict(hits=HitList, holds=HoldList, bpms=BpmList)
+
+    # objs is the objects of the class, it MUST be defined,
+    # and must have defaults as ([]).
+    objs: Dict[str, TimedList] = \
+        field(init=False,
+              default_factory=
+              lambda: dict(
+                  hits=HitList([]),
+                  holds=HoldList([]),
+                  bpms=BpmList([]))
+              )
+
+    def __getitem__(self, item: Type[T]) -> List[Type[T]]:
+        li = [o for o in self.objs.values() if isinstance(o, item)]
+        if li:
+            return li
+        else:
+            raise IndexError(f"Object of type {item} does not exist.")
+
+    def __setitem__(self, key: T, value: List[Type[T]]):
+        this = self.__getitem__(key)
+        assert len(this) == len(
+            value), "The lengths of the set and get must be the same."
+        for i in range(len(this)):
+            # noinspection PyTypeChecker
+            this[i] = value[i]
+
+    @property
+    def notes(self):
+        return self[NoteList]
+
+    # noinspection PyUnresolvedReferences
+    @notes.setter
+    def notes(self, val):
+        for i in range(len(val)):
+            self[NoteList][i] = val[i]
+
+    def deepcopy(self) -> Map:
+        """Returns a deep copy of itself"""
+        return deepcopy(self)
+
+    # @abstractmethod
+    def metadata(self, unicode=True, **kwargs) -> str:
+        """Grabs the map metadata
+
+        Notes:
+            This doesn't try to convert unicode to ascii.
+        Args:
+            unicode: Whether to use unicode if available.
+
+        Returns:
+            A string containing the metadata
+        """
+        ...
+
+    def describe(self,
+                 rounding: int = 2,
+                 unicode: bool = False,
+                 **kwargs) -> str:
+        """Describes the map's attributes as a short summary
+
+        Examples:
+
+            >>> from reamber.base import Hit, Bpm
+            >>> bpms = [Bpm(offset=1000, bpm=120)]
+            >>> hits = [Hit(offset=1000, column=1),
+            ...         Hit(offset=2000, column=2)]
+            >>> m = Map()
+            >>> m.hits = HitList(hits)
+            >>> m.bpms = BpmList(bpms)
+            >>> m.describe() # doctest: +ELLIPSIS
+            "..."
+
+        Args:
+            rounding: The decimal rounding
+            unicode: Whether to use unicode if available.
+        """
+
+        first = min([nl.first_offset() for nl in self[NoteList] if nl])
+        last = max([nl.last_offset() for nl in self[NoteList] if nl])
+
+        out = f"Average BPM: " \
+              f"{round(self[BpmList][0].ave_bpm(last), rounding)}\n" \
+              f"Map Length: " \
+              f"{datetime.timedelta(milliseconds=last - first)}\n" \
+              f"{self.metadata(unicode=unicode, **kwargs)} + \n\n" \
+              f"--- Notes ---\n"
+
+        for n in self[NoteList]:
+            n: TimedList
+            out += f"{n.__class__.__name__}\n" \
+                   f"{n.df.columns}\n" \
+                   f"{n.df.describe()}\n\n"
+        return out
+
+    def rate(self, by: float) -> Map:
+        """Changes the rate of the map
+
+        Examples:
+            The following will uprate the map by 10%
+
+            >>> Map().rate(1.1) # doctest: +ELLIPSIS
+            Map(...)
+
+        Args:
+            by: The rate.
+        """
+
+        copy = self.deepcopy()
+        stack = copy.stack()
+        stack.offset /= by
+        stack.bpm *= by
+        stack.length /= by
+        return copy
+
+    @stack_props()
+    class Stacker:
+        """Stacking merges multiple ``TimedList`` to map operations on them.
+
+        The internal data class is a ``pd.DataFrame``.
+
+        Examples:
+
+            >>> from reamber.base import Hit
+            >>> hits = [Hit(offset=1000, column=1),
+            ...         Hit(offset=2000, column=2)]
+            >>> m = Map()
+            >>> m.hits = HitList(hits)
+            >>> stack = m.stack()
+
+            Multiply all offsets in the map by 2
+
+            >>> stack.offset *= 2
+            >>> stack.offset.tolist()
+            [2000.0, 4000.0]
+
+            Or if you do it inline,
+
+            >>> m.stack().offset *= 2
+            >>> m.hits.offset.tolist()
+            [4000.0, 8000.0]
+
+            Notice that ``stack`` changes the map directly by reference.
+
+            If the property, like ``column``, doesn't exist for ``Bpm``,
+            it will simply skip it for ``Bpm``.
+
+            However, all properties must exist at least once.
+
+            For example,
+
+            >>> try:
+            ...     stack.does_not_exist *= 2
+            ... except Excepti  on:
+            ...     print("No such property")
+            No such property
+
+            The internal data class is a ``pd.DataFrame``:
+
+            >>> hits = [Hit(offset=1000, column=1),
+            ...         Hit(offset=2000, column=2),
+            ...         Hit(offset=3000, column=3)]
+            >>> m = Map()
+            >>> m.hits = HitList(hits)
+            >>> stack = m.stack()
+            >>> stack.offset[stack.column < 2].tolist()
+            [1000.0]
+
+            >>> stack.offset[stack.column > 1].tolist()
+            [2000.0, 3000.0]
+
+            If you need more conditions, use ``loc``
+        """
+
+        """We concat all dfs and do operations on the joined df. 
+        However, concat of dfs will always be deep copied.
+        Thus, any updates to the concat needs to update the original list 
+        
+        LISTS ---STACK---> COPY ---> STACKED
+          +---------- REFERENCE ---> UNSTACKED  
+        
+        To do so, we track of the links between unstacked and stacked by ix.
+        
+        IXS        |         |          |    |     |
+        UNSTACKED  [........] [........] [..] [....]
+        STACKED    [...............................]
+        
+        So any operation will affect the stacked, 
+        any mutation will call _update, updating unstacked.
+        
+        """
+
+        _ixs: List[int]
+        _unstacked: List[TimedList]
+
+        # This is concat of all lists, making common ops possible.
+        _stacked: pd.DataFrame
+
+        def __init__(self, objs: List[TimedList]):
+            ixs: List = [0]
+            for obj in objs:
+                ixs.append(ixs[-1] + len(obj))
+            self._ixs = ixs
+            self._unstacked = objs
+            self._stacked = pd.concat(
+                [v.df for v in self._unstacked]
+            ).reset_index()
+
+        @property
+        def loc(self) -> StackerLocIndexer:
+            """Loc is used when basic indexing is insufficient.
+
+            Notes:
+                This is similar to how ``pandas`` uses ``loc``.
+                You may assume the same syntax.
+
+            Examples:
+                >>> from reamber.base import Hit
+                >>> hits = [Hit(offset=1000, column=1),
+                ...         Hit(offset=2000, column=2),
+                ...         Hit(offset=3000, column=3)]
+                >>> m = Map()
+                >>> m.hits = HitList(hits)
+                >>> stack = m.stack()
+
+                >>> stack.loc[stack.offset > 1000, 'column'] += 1
+                >>> m.hits.column.tolist()
+                [1.0, 3.0, 4.0]
+
+                >>> stack.loc[
+                ...     (stack.column == 1) & (stack.offset <= 1000),
+                ...     ['offset']
+                ... ] *= 2
+                >>> m.hits.offset.tolist()
+                [2000.0, 2000.0, 3000.0]
+
+            """
+            return self.StackerLocIndexer(self._stacked.loc, self)
+
+        def _update(self):
+            for obj, ix_i, ix_j in zip(
+                self._unstacked, self._ixs[:-1], self._ixs[1:]
+            ):
+                obj.df = self._stacked[obj.df.columns].iloc[ix_i:ix_j]
+
+        def __getitem__(self, item):
+            return self._stacked[item]
+
+        def __setitem__(self, key, value):
+            self._stacked[key] = value
+            self._update()
+
+        _props = ['offset', 'column', 'length', 'bpm', 'metronome']
+
+        @dataclass
+        class StackerLocIndexer:
+            """Class generated with ``Stacker.loc``
+
+            Notes:
+                See Documentation in ``Stacker.loc`` on usage.
+            """
+            loc: _LocIndexer
+            stacker: Map.Stacker
+
+            def __setitem__(self, key, value):
+                self.loc.__setitem__(key, value)
+                self.stacker._update()
+
+            def __getitem__(self, item):
+                return self.loc.__getitem__(item)
+
+    def stack(self, include_types: Tuple[Type[T]] = None) -> Stacker:
+        """Stacks map and includes specific columns
+
+        Examples:
+            This will generate a stacker ``stack``
+
+            >>> from reamber.base import Hit
+            >>> hits = [Hit(offset=1000, column=1),
+            ...         Hit(offset=2000, column=2),
+            ...         Hit(offset=3000, column=3)]
+            >>> m = Map()
+            >>> m.hits = HitList(hits)
+            >>> m.stack() # doctest: +ELLIPSIS
+            <Map.Map.Stacker ...>
+
+        Returns:
+            A ``Map.Stacker`` instance. This is a pass by reference.
+            Thus, modifications on the stack will change the map directly.
+
+        """
+
+        if include_types is None:
+            objs = [v for v in self.objs.values()]
+        else:
+            # noinspection PyTypeHints
+            objs = [v for v in self.objs.values()
+                    if isinstance(v, include_types)]
+        return self.Stacker(objs)
```

### Comparing `reamber-0.1.7/reamber/base/Map.pyi` & `reamber-0.1.8/reamber/base/Map.pyi`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import List, TypeVar, Generic, Dict, Type, Tuple
-
-import pandas as pd
-from pandas.core.indexing import _LocIndexer
-
-from reamber.base.lists.BpmList import BpmList
-from reamber.base.lists.TimedList import TimedList
-from reamber.base.lists.notes.HitList import HitList
-from reamber.base.lists.notes.HoldList import HoldList
-from reamber.base.lists.notes.NoteList import NoteList
-
-NoteListT = TypeVar('NoteListT', bound=NoteList)
-HitListT = TypeVar('HitListT', bound=HitList)
-HoldListT = TypeVar('HoldListT', bound=HoldList)
-BpmListT = TypeVar('BpmListT', bound=BpmList)
-
-T = TypeVar('T', bound=TimedList)
-
-
-@dataclass
-class Map(Generic[NoteListT, HitListT, HoldListT, BpmListT]):
-    """This class should be inherited by all Map Objects
-
-    They must inherit the data method, which extracts all data they hold.
-    They are also assumed to be a TimedList.
-    """
-
-    objs: Dict[str, TimedList] = field(default_factory=lambda: [])
-
-    def __getitem__(self, item: Type[T]) -> List[Type[T]]: ...
-
-    def __setitem__(self, key: T, value: List[Type[T]]): ...
-
-    @property
-    def hits(self) -> HitListT: ...
-
-    @hits.setter
-    def hits(self, val) -> None: ...
-
-    @property
-    def holds(self) -> HoldListT: ...
-
-    @holds.setter
-    def holds(self, val) -> None: ...
-
-    @property
-    def bpms(self) -> BpmListT: ...
-
-    @bpms.setter
-    def bpms(self, val) -> None: ...
-
-    @property
-    def notes(self) -> List[NoteListT]: ...
-
-    @notes.setter
-    def notes(self, val: List[NoteListT]) -> None: ...
-
-    def deepcopy(self) -> Map: ...
-
-    def metadata(self, unicode=True, **kwargs) -> str: ...
-
-    def describe(self, rounding: int = 2, **kwargs) -> str: ...
-
-    def rate(self, by: float) -> Map: ...
-
-    class Stacker:
-        _ixs: List[int]
-        _unstacked: List[TimedList]
-
-        # The stacked property is a concat of all lists, this makes the common ops possible.
-        _stacked: pd.DataFrame
-
-        def __init__(self, objs: List[TimedList]): ...
-
-        def _update(self): ...
-
-        def __getitem__(self, item): ...
-
-        def __setitem__(self, key, value): ...
-
-        @property
-        def offset(self) -> pd.Series: ...
-
-        @offset.setter
-        def offset(self, val: pd.Series): ...
-
-        @property
-        def column(self) -> pd.Series: ...
-
-        @column.setter
-        def column(self, val: pd.Series): ...
-
-        @property
-        def length(self) -> pd.Series: ...
-
-        @length.setter
-        def length(self, val: pd.Series): ...
-
-        @property
-        def bpm(self) -> pd.Series: ...
-
-        @bpm.setter
-        def bpm(self, val: pd.Series): ...
-
-        @property
-        def metronome(self) -> pd.Series: ...
-
-        @metronome.setter
-        def metronome(self, val: pd.Series): ...
-
-        @property
-        def loc(self) -> Map.Stacker.StackerLocIndexer: ...
-
-        @dataclass
-        class StackerLocIndexer:
-            loc: _LocIndexer
-            stacker: Map.Stacker
-
-            def __setitem__(self, key, value): ...
-
-            def __getitem__(self, item): ...
-
-    def stack(self, include_types: Tuple[Type[T]] = None) -> Stacker: ...
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import List, TypeVar, Generic, Dict, Type, Tuple
+
+import pandas as pd
+from pandas.core.indexing import _LocIndexer
+
+from reamber.base.lists.BpmList import BpmList
+from reamber.base.lists.TimedList import TimedList
+from reamber.base.lists.notes.HitList import HitList
+from reamber.base.lists.notes.HoldList import HoldList
+from reamber.base.lists.notes.NoteList import NoteList
+
+NoteListT = TypeVar('NoteListT', bound=NoteList)
+HitListT = TypeVar('HitListT', bound=HitList)
+HoldListT = TypeVar('HoldListT', bound=HoldList)
+BpmListT = TypeVar('BpmListT', bound=BpmList)
+
+T = TypeVar('T', bound=TimedList)
+
+
+@dataclass
+class Map(Generic[NoteListT, HitListT, HoldListT, BpmListT]):
+    """This class should be inherited by all Map Objects
+
+    They must inherit the data method, which extracts all data they hold.
+    They are also assumed to be a TimedList.
+    """
+
+    objs: Dict[str, TimedList] = field(default_factory=lambda: [])
+
+    def __getitem__(self, item: Type[T]) -> List[Type[T]]: ...
+
+    def __setitem__(self, key: T, value: List[Type[T]]): ...
+
+    @property
+    def hits(self) -> HitListT: ...
+
+    @hits.setter
+    def hits(self, val) -> None: ...
+
+    @property
+    def holds(self) -> HoldListT: ...
+
+    @holds.setter
+    def holds(self, val) -> None: ...
+
+    @property
+    def bpms(self) -> BpmListT: ...
+
+    @bpms.setter
+    def bpms(self, val) -> None: ...
+
+    @property
+    def notes(self) -> List[NoteListT]: ...
+
+    @notes.setter
+    def notes(self, val: List[NoteListT]) -> None: ...
+
+    def deepcopy(self) -> Map: ...
+
+    def metadata(self, unicode=True, **kwargs) -> str: ...
+
+    def describe(self, rounding: int = 2, **kwargs) -> str: ...
+
+    def rate(self, by: float) -> Map: ...
+
+    class Stacker:
+        _ixs: List[int]
+        _unstacked: List[TimedList]
+
+        # The stacked property is a concat of all lists, this makes the common ops possible.
+        _stacked: pd.DataFrame
+
+        def __init__(self, objs: List[TimedList]): ...
+
+        def _update(self): ...
+
+        def __getitem__(self, item): ...
+
+        def __setitem__(self, key, value): ...
+
+        @property
+        def offset(self) -> pd.Series: ...
+
+        @offset.setter
+        def offset(self, val: pd.Series): ...
+
+        @property
+        def column(self) -> pd.Series: ...
+
+        @column.setter
+        def column(self, val: pd.Series): ...
+
+        @property
+        def length(self) -> pd.Series: ...
+
+        @length.setter
+        def length(self, val: pd.Series): ...
+
+        @property
+        def bpm(self) -> pd.Series: ...
+
+        @bpm.setter
+        def bpm(self, val: pd.Series): ...
+
+        @property
+        def metronome(self) -> pd.Series: ...
+
+        @metronome.setter
+        def metronome(self, val: pd.Series): ...
+
+        @property
+        def loc(self) -> Map.Stacker.StackerLocIndexer: ...
+
+        @dataclass
+        class StackerLocIndexer:
+            loc: _LocIndexer
+            stacker: Map.Stacker
+
+            def __setitem__(self, key, value): ...
+
+            def __getitem__(self, item): ...
+
+    def stack(self, include_types: Tuple[Type[T]] = None) -> Stacker: ...
```

### Comparing `reamber-0.1.7/reamber/base/MapSet.py` & `reamber-0.1.8/reamber/base/MapSet.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,196 +1,196 @@
-from __future__ import annotations
-
-from copy import deepcopy
-from dataclasses import dataclass, field
-from typing import List, Iterator, TypeVar, Union, Any, Generic, Type
-
-import pandas as pd
-
-from reamber.base.Map import Map
-from reamber.base.Property import stack_props
-from reamber.base.lists import TimedList
-
-NoteListT = TypeVar('NoteListT')
-HitListT = TypeVar('HitListT')
-HoldListT = TypeVar('HoldListT')
-BpmListT = TypeVar('BpmListT')
-MapT = TypeVar('MapT')
-
-T = TypeVar('T', bound=TimedList)
-
-
-@dataclass
-class MapSet(Generic[NoteListT, HitListT, HoldListT, BpmListT, MapT]):
-    maps: List[MapT[NoteListT, HitListT, HoldListT, BpmListT]] = field(
-        default_factory=lambda: []
-    )
-
-    def __init__(self,
-                 maps: List[MapT[NoteListT, HitListT, HoldListT, BpmListT]]):
-        self.maps = maps
-
-    def __iter__(self) -> Iterator[MapT]:
-        for m in self.maps:
-            yield m
-
-    def items(self):
-        for m in self.maps:
-            yield m.__class__, m
-
-    def __getitem__(self, item: Type[T] | int) -> List[Type[T]]:
-        if isinstance(item, type):
-            return [m[item][0] for m in self.maps]
-        else:
-            return self.maps[item]
-
-    def __setitem__(self, key: Union[Any, type], value):
-        this = self[key]
-        if len(this) != len(value):
-            raise ValueError("Length to set mismatched.")
-        for i in range(len(this)): this[i] = value[i]
-
-    def deepcopy(self):
-        """Returns a deep copy of itself"""
-        return deepcopy(self)
-
-    def describe(self, rounding: int = 2, unicode: bool = False) -> List[str]:
-        """Describes the map's attributes as a short summary
-
-        Examples:
-            >>> from reamber.base import Hit, Bpm
-            >>> from reamber.base.lists import BpmList
-            >>> from reamber.base.lists.notes import HitList
-            >>> bpms = [Bpm(offset=1000, bpm=120)]
-            >>> hits = [Hit(offset=1000, column=1),
-            ...         Hit(offset=2000, column=2)]
-            >>> m = Map()
-            ... m.hits = HitList(hits)
-            ... m.bpms = BpmList(bpms)
-            >>> MapSet([m, m]).describe() # doctest: +ELLIPSIS
-            ["...", "..."]
-
-            .. code-block::
-
-                Average BPM: 120.0
-                Map Length: 0:00:01
-
-                --- Notes ---
-                HitList
-                Index(['offset', 'column'], dtype='object')
-                ...
-
-                HoldList
-                Index(['length', 'column', 'offset'], dtype='object')
-                ...
-
-        Args:
-            rounding: The decimal rounding
-            unicode: Whether to use unicode if available.
-        """
-
-        return [m.describe(rounding=rounding, unicode=unicode, s=self)
-                for m in self]
-
-    def rate(self, by: float) -> MapSet:
-        """Changes the rate of the map
-
-        Examples:
-            The following will uprate the map by 10%
-
-            >>> MapSet([]).rate(1.1) # doctest: +ELLIPSIS
-            MapSet(...)
-
-        Args:
-            by: The rate.
-        """
-        copy = self.deepcopy()
-        copy.maps = [m.rate(by=by) for m in copy.maps]
-        return copy
-
-    # noinspection DuplicatedCode,PyUnresolvedReferences
-    @stack_props()
-    class Stacker:
-        """Stacking merges multiple ``TimedList`` to map operations on them.
-
-        Notes:
-            Unlike ``Map.Stacker`` this doesn't support conditional indexing.
-
-        Examples:
-
-            >>> from reamber.base.lists import BpmList
-            >>> from reamber.base.lists.notes import HitList
-            >>> from reamber.base import Hit
-            >>> hits = [Hit(offset=1000, column=1),
-            ...         Hit(offset=2000, column=2)]
-            >>> m = Map()
-            >>> m.hits = HitList(hits)
-            >>> ms = MapSet([m, m.deepcopy()])
-            >>> stack = ms.stack()
-
-            Multiply all offsets in the map by 2
-
-            ``stack.offset`` is a ``pd.DataFrame``.
-
-            ``iloc[0]`` yields the first map offsets
-
-            >>> stack.offset *= 2
-            >>> stack.offset.iloc[0].tolist()
-            [2000.0, 4000.0]
-
-            Or if you do it inline,
-
-            ``ms[0]`` yields the first map
-
-            >>> ms.stack().offset *= 2
-            >>> ms[0].hits.offset.tolist()
-            [4000.0, 8000.0]
-
-            Notice that ``stack`` changes the map directly by reference.
-
-            If the property, like ``column``, doesn't exist for ``Bpm``,
-            it will simply skip it for ``Bpm``.
-
-            However, all properties must exist at least once.
-
-        """
-
-        """See Map.stack for details"""
-
-        stackers: List[Map.Stacker]
-
-        # noinspection PyProtectedMember
-        def __init__(self, stackers: List[Map.Stacker]):
-            self.stackers = stackers
-
-        def __getitem__(self, item):
-            return pd.DataFrame([i[item] for i in self.stackers])
-
-        def __setitem__(self, key, value):
-            for s, i in zip(self.stackers, value.iloc):
-                s[key] = i
-
-        _props = ['offset', 'column', 'length', 'bpm', 'metronome']
-
-    def stack(self):
-        """Stacks map and includes specific columns
-
-        Examples:
-
-            This will generate a stacker ``stack``
-
-            >>> from reamber.base import Hit
-            >>> from reamber.base.lists.notes import HitList
-            >>> hits = [Hit(offset=1000, column=1),
-            ...         Hit(offset=2000, column=2),
-            ...         Hit(offset=3000, column=3)]
-            >>> m = Map()
-            >>> m.hits = HitList(hits)
-            >>> MapSet([m, m.deepcopy()]).stack() # doctest: +ELLIPSIS
-            <MapSet.MapSet.Stacker ...>
-
-        Returns:
-            A ``MapSet.Stacker`` instance. This is a pass by reference.
-            Thus, modifications on the stack will change the map directly.
-
-        """
-        return self.Stacker([_.stack() for _ in self])
+from __future__ import annotations
+
+from copy import deepcopy
+from dataclasses import dataclass, field
+from typing import List, Iterator, TypeVar, Union, Any, Generic, Type
+
+import pandas as pd
+
+from reamber.base.Map import Map
+from reamber.base.Property import stack_props
+from reamber.base.lists import TimedList
+
+NoteListT = TypeVar('NoteListT')
+HitListT = TypeVar('HitListT')
+HoldListT = TypeVar('HoldListT')
+BpmListT = TypeVar('BpmListT')
+MapT = TypeVar('MapT')
+
+T = TypeVar('T', bound=TimedList)
+
+
+@dataclass
+class MapSet(Generic[NoteListT, HitListT, HoldListT, BpmListT, MapT]):
+    maps: List[MapT[NoteListT, HitListT, HoldListT, BpmListT]] = field(
+        default_factory=lambda: []
+    )
+
+    def __init__(self,
+                 maps: List[MapT[NoteListT, HitListT, HoldListT, BpmListT]]):
+        self.maps = maps
+
+    def __iter__(self) -> Iterator[MapT]:
+        for m in self.maps:
+            yield m
+
+    def items(self):
+        for m in self.maps:
+            yield m.__class__, m
+
+    def __getitem__(self, item: Type[T] | int) -> List[Type[T]]:
+        if isinstance(item, type):
+            return [m[item][0] for m in self.maps]
+        else:
+            return self.maps[item]
+
+    def __setitem__(self, key: Union[Any, type], value):
+        this = self[key]
+        if len(this) != len(value):
+            raise ValueError("Length to set mismatched.")
+        for i in range(len(this)): this[i] = value[i]
+
+    def deepcopy(self):
+        """Returns a deep copy of itself"""
+        return deepcopy(self)
+
+    def describe(self, rounding: int = 2, unicode: bool = False) -> List[str]:
+        """Describes the map's attributes as a short summary
+
+        Examples:
+            >>> from reamber.base import Hit, Bpm
+            >>> from reamber.base.lists import BpmList
+            >>> from reamber.base.lists.notes import HitList
+            >>> bpms = [Bpm(offset=1000, bpm=120)]
+            >>> hits = [Hit(offset=1000, column=1),
+            ...         Hit(offset=2000, column=2)]
+            >>> m = Map()
+            ... m.hits = HitList(hits)
+            ... m.bpms = BpmList(bpms)
+            >>> MapSet([m, m]).describe() # doctest: +ELLIPSIS
+            ["...", "..."]
+
+            .. code-block::
+
+                Average BPM: 120.0
+                Map Length: 0:00:01
+
+                --- Notes ---
+                HitList
+                Index(['offset', 'column'], dtype='object')
+                ...
+
+                HoldList
+                Index(['length', 'column', 'offset'], dtype='object')
+                ...
+
+        Args:
+            rounding: The decimal rounding
+            unicode: Whether to use unicode if available.
+        """
+
+        return [m.describe(rounding=rounding, unicode=unicode, s=self)
+                for m in self]
+
+    def rate(self, by: float) -> MapSet:
+        """Changes the rate of the map
+
+        Examples:
+            The following will uprate the map by 10%
+
+            >>> MapSet([]).rate(1.1) # doctest: +ELLIPSIS
+            MapSet(...)
+
+        Args:
+            by: The rate.
+        """
+        copy = self.deepcopy()
+        copy.maps = [m.rate(by=by) for m in copy.maps]
+        return copy
+
+    # noinspection DuplicatedCode,PyUnresolvedReferences
+    @stack_props()
+    class Stacker:
+        """Stacking merges multiple ``TimedList`` to map operations on them.
+
+        Notes:
+            Unlike ``Map.Stacker`` this doesn't support conditional indexing.
+
+        Examples:
+
+            >>> from reamber.base.lists import BpmList
+            >>> from reamber.base.lists.notes import HitList
+            >>> from reamber.base import Hit
+            >>> hits = [Hit(offset=1000, column=1),
+            ...         Hit(offset=2000, column=2)]
+            >>> m = Map()
+            >>> m.hits = HitList(hits)
+            >>> ms = MapSet([m, m.deepcopy()])
+            >>> stack = ms.stack()
+
+            Multiply all offsets in the map by 2
+
+            ``stack.offset`` is a ``pd.DataFrame``.
+
+            ``iloc[0]`` yields the first map offsets
+
+            >>> stack.offset *= 2
+            >>> stack.offset.iloc[0].tolist()
+            [2000.0, 4000.0]
+
+            Or if you do it inline,
+
+            ``ms[0]`` yields the first map
+
+            >>> ms.stack().offset *= 2
+            >>> ms[0].hits.offset.tolist()
+            [4000.0, 8000.0]
+
+            Notice that ``stack`` changes the map directly by reference.
+
+            If the property, like ``column``, doesn't exist for ``Bpm``,
+            it will simply skip it for ``Bpm``.
+
+            However, all properties must exist at least once.
+
+        """
+
+        """See Map.stack for details"""
+
+        stackers: List[Map.Stacker]
+
+        # noinspection PyProtectedMember
+        def __init__(self, stackers: List[Map.Stacker]):
+            self.stackers = stackers
+
+        def __getitem__(self, item):
+            return pd.DataFrame([i[item] for i in self.stackers])
+
+        def __setitem__(self, key, value):
+            for s, i in zip(self.stackers, value.iloc):
+                s[key] = i
+
+        _props = ['offset', 'column', 'length', 'bpm', 'metronome']
+
+    def stack(self):
+        """Stacks map and includes specific columns
+
+        Examples:
+
+            This will generate a stacker ``stack``
+
+            >>> from reamber.base import Hit
+            >>> from reamber.base.lists.notes import HitList
+            >>> hits = [Hit(offset=1000, column=1),
+            ...         Hit(offset=2000, column=2),
+            ...         Hit(offset=3000, column=3)]
+            >>> m = Map()
+            >>> m.hits = HitList(hits)
+            >>> MapSet([m, m.deepcopy()]).stack() # doctest: +ELLIPSIS
+            <MapSet.MapSet.Stacker ...>
+
+        Returns:
+            A ``MapSet.Stacker`` instance. This is a pass by reference.
+            Thus, modifications on the stack will change the map directly.
+
+        """
+        return self.Stacker([_.stack() for _ in self])
```

### Comparing `reamber-0.1.7/reamber/base/MapSet.pyi` & `reamber-0.1.8/reamber/base/MapSet.pyi`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,104 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import List, Iterator, TypeVar, Union, Any, Generator, Tuple, \
-    overload, Generic, Type, Sequence
-
-import numpy as np
-import pandas as pd
-
-from reamber.base.Map import Map
-from reamber.base.lists import TimedList
-from reamber.base.lists.BpmList import BpmList
-from reamber.base.lists.notes.HitList import HitList
-from reamber.base.lists.notes.HoldList import HoldList
-from reamber.base.lists.notes.NoteList import NoteList
-
-NoteListT = TypeVar('NoteListT', bound=NoteList)
-HitListT = TypeVar('HitListT', bound=HitList)
-HoldListT = TypeVar('HoldListT', bound=HoldList)
-BpmListT = TypeVar('BpmListT', bound=BpmList)
-MapT = TypeVar('MapT', bound=Map)
-
-T = TypeVar('T', bound=TimedList)
-TSlice = TypeVar('TSlice', bound=Sequence)
-
-
-@dataclass
-class MapSet(Generic[NoteListT, HitListT, HoldListT, BpmListT, MapT]):
-    maps: List[MapT[NoteListT, HitListT, HoldListT, BpmListT]] = field(
-        default_factory=lambda: [])
-
-    def __init__(self, maps: List[
-        Map[NoteListT, HitListT, HoldListT, BpmListT]]): ...
-
-    def __iter__(self) -> Iterator[Map]: ...
-
-    def items(self) -> Generator[Tuple[type, Map]]: ...
-
-    @overload
-    def __getitem__(self, item: Type[T]) -> List[Type[T]]: ...
-
-    @overload
-    def __getitem__(self, item: slice) -> List[Map]: ...
-
-    @overload
-    def __getitem__(self, item: int) -> Map: ...
-
-    def __getitem__(self, item: int | slice | Type[T]) -> Map: Map | Sequence[
-        Map] | List[Type[T]]
-
-    def __setitem__(self, key: Union[Any, type], value): ...
-
-    def deepcopy(self) -> MapSet: ...
-
-    def describe(self, rounding: int = 2, unicode: bool = False) -> List[
-        str]: ...
-
-    def rate(self, by: float) -> MapSet: ...
-
-    class Stacker:
-        _ixs: np.ndarray
-        _unstacked: List[List[TimedList]]
-        _stacked: pd.DataFrame
-        _stacks: List
-
-        def __init__(self, maps: List[Map]): ...
-
-        def _update(self): ...
-
-        def __getitem__(self, item): ...
-
-        def __setitem__(self, key, value): ...
-
-        @property
-        def offset(self) -> pd.Series: ...
-
-        @offset.setter
-        def offset(self, val: pd.Series): ...
-
-        @property
-        def column(self) -> pd.Series: ...
-
-        @column.setter
-        def column(self, val: pd.Series): ...
-
-        @property
-        def length(self) -> pd.Series: ...
-
-        @length.setter
-        def length(self, val: pd.Series): ...
-
-        @property
-        def bpm(self) -> pd.Series: ...
-
-        @bpm.setter
-        def bpm(self, val: pd.Series): ...
-
-        @property
-        def metronome(self) -> pd.Series: ...
-
-        @metronome.setter
-        def metronome(self, val: pd.Series): ...
-
-    def stack(self) -> Stacker: ...
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import List, Iterator, TypeVar, Union, Any, Generator, Tuple, \
+    overload, Generic, Type, Sequence
+
+import numpy as np
+import pandas as pd
+
+from reamber.base.Map import Map
+from reamber.base.lists import TimedList
+from reamber.base.lists.BpmList import BpmList
+from reamber.base.lists.notes.HitList import HitList
+from reamber.base.lists.notes.HoldList import HoldList
+from reamber.base.lists.notes.NoteList import NoteList
+
+NoteListT = TypeVar('NoteListT', bound=NoteList)
+HitListT = TypeVar('HitListT', bound=HitList)
+HoldListT = TypeVar('HoldListT', bound=HoldList)
+BpmListT = TypeVar('BpmListT', bound=BpmList)
+MapT = TypeVar('MapT', bound=Map)
+
+T = TypeVar('T', bound=TimedList)
+TSlice = TypeVar('TSlice', bound=Sequence)
+
+
+@dataclass
+class MapSet(Generic[NoteListT, HitListT, HoldListT, BpmListT, MapT]):
+    maps: List[MapT[NoteListT, HitListT, HoldListT, BpmListT]] = field(
+        default_factory=lambda: [])
+
+    def __init__(self, maps: List[
+        Map[NoteListT, HitListT, HoldListT, BpmListT]]): ...
+
+    def __iter__(self) -> Iterator[Map]: ...
+
+    def items(self) -> Generator[Tuple[type, Map]]: ...
+
+    @overload
+    def __getitem__(self, item: Type[T]) -> List[Type[T]]: ...
+
+    @overload
+    def __getitem__(self, item: slice) -> List[Map]: ...
+
+    @overload
+    def __getitem__(self, item: int) -> Map: ...
+
+    def __getitem__(self, item: int | slice | Type[T]) -> Map: Map | Sequence[
+        Map] | List[Type[T]]
+
+    def __setitem__(self, key: Union[Any, type], value): ...
+
+    def deepcopy(self) -> MapSet: ...
+
+    def describe(self, rounding: int = 2, unicode: bool = False) -> List[
+        str]: ...
+
+    def rate(self, by: float) -> MapSet: ...
+
+    class Stacker:
+        _ixs: np.ndarray
+        _unstacked: List[List[TimedList]]
+        _stacked: pd.DataFrame
+        _stacks: List
+
+        def __init__(self, maps: List[Map]): ...
+
+        def _update(self): ...
+
+        def __getitem__(self, item): ...
+
+        def __setitem__(self, key, value): ...
+
+        @property
+        def offset(self) -> pd.Series: ...
+
+        @offset.setter
+        def offset(self, val: pd.Series): ...
+
+        @property
+        def column(self) -> pd.Series: ...
+
+        @column.setter
+        def column(self, val: pd.Series): ...
+
+        @property
+        def length(self) -> pd.Series: ...
+
+        @length.setter
+        def length(self, val: pd.Series): ...
+
+        @property
+        def bpm(self) -> pd.Series: ...
+
+        @bpm.setter
+        def bpm(self, val: pd.Series): ...
+
+        @property
+        def metronome(self) -> pd.Series: ...
+
+        @metronome.setter
+        def metronome(self, val: pd.Series): ...
+
+    def stack(self) -> Stacker: ...
```

### Comparing `reamber-0.1.7/reamber/base/RAConst.py` & `reamber-0.1.8/reamber/base/RAConst.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-class RAConst:
-    """This class holds all constants that can be used throughout the program
-
-    The class defines a helper classes to convert in units
-
-    Examples:
-
-        >>> RAConst.hr_to_min(10)
-        600.0
-
-        >>> RAConst.min_to_sec(10)
-        600.0
-
-        >>> RAConst.sec_to_msec(10)
-        10000.0
-
-        >>> RAConst.sec_to_hr(60 * 60)
-        1.0
-
-    Notes:
-        This also defines division classes, used in PlayField::
-
-             {1: "#969696",
-              2: "#b02323",
-              3: "#8a23b0",
-              4: "#2399b0",
-              5: "#ffdfbd",
-              6: "#b02378",
-              8: "#b06c23",
-              12: "#23b09d",
-              16: "#3db023",
-              24: "#94b023",
-              32: "#23b052"}
-
-    """
-
-    HR_TO_MIN   : float = 60.0
-    HR_TO_SEC   : float = 60.0 * 60.0
-    HR_TO_MSEC  : float = 60.0 * 60.0 * 1000.0
-    MIN_TO_HR   : float = 1.0 / 60.0
-    MIN_TO_SEC  : float = 60.0
-    MIN_TO_MSEC : float = 60.0 * 1000.0
-    SEC_TO_HR   : float = 1.0 / (60.0 * 60.0)
-    SEC_TO_MIN  : float = 1.0 / 60.0
-    SEC_TO_MSEC : float = 1000.0
-    MSEC_TO_HR  : float = 1.0 / (60.0 * 60.0 * 1000.0)
-    MSEC_TO_MIN : float = 1.0 / (60.0 * 1000.0)
-    MSEC_TO_SEC : float = 1.0 / 1000.0
-
-    @staticmethod
-    def hr_to_min(hours): return float(hours * RAConst.HR_TO_MIN)
-    @staticmethod
-    def hr_to_sec(hours): return float(hours * RAConst.HR_TO_SEC)
-    @staticmethod
-    def hr_to_msec(hours): return float(hours * RAConst.HR_TO_MSEC)
-    @staticmethod
-    def min_to_hr(mins): return float(mins * RAConst.MIN_TO_HR)
-    @staticmethod
-    def min_to_sec(mins): return float(mins * RAConst.MIN_TO_SEC)
-    @staticmethod
-    def min_to_msec(mins): return float(mins * RAConst.MIN_TO_MSEC)
-    @staticmethod
-    def sec_to_hr(secs): return float(secs * RAConst.SEC_TO_HR)
-    @staticmethod
-    def sec_to_min(secs): return float(secs * RAConst.SEC_TO_MIN)
-    @staticmethod
-    def sec_to_msec(secs): return float(secs * RAConst.SEC_TO_MSEC)
-    @staticmethod
-    def msec_to_hr(msecs): return float(msecs * RAConst.MSEC_TO_HR)
-    @staticmethod
-    def msec_to_min(msecs): return float(msecs * RAConst.MSEC_TO_MIN)
-    @staticmethod
-    def msec_to_sec(msecs): return float(msecs * RAConst.MSEC_TO_SEC)
-
-    # These are the colors to indicate snapping. Used for PlayField
-    DIVISION_COLORS = {1: "#969696"
-                     , 2: "#b02323"
-                     , 3: "#8a23b0"
-                     , 4: "#2399b0"
-                     , 5: "#ffdfbd"
-                     , 6: "#b02378"
-                     , 8: "#b06c23"
-                     , 12: "#23b09d"
-                     , 16: "#3db023"
-                     , 24: "#94b023"
-                     , 32: "#23b052"}
+class RAConst:
+    """This class holds all constants that can be used throughout the program
+
+    The class defines a helper classes to convert in units
+
+    Examples:
+
+        >>> RAConst.hr_to_min(10)
+        600.0
+
+        >>> RAConst.min_to_sec(10)
+        600.0
+
+        >>> RAConst.sec_to_msec(10)
+        10000.0
+
+        >>> RAConst.sec_to_hr(60 * 60)
+        1.0
+
+    Notes:
+        This also defines division classes, used in PlayField::
+
+             {1: "#969696",
+              2: "#b02323",
+              3: "#8a23b0",
+              4: "#2399b0",
+              5: "#ffdfbd",
+              6: "#b02378",
+              8: "#b06c23",
+              12: "#23b09d",
+              16: "#3db023",
+              24: "#94b023",
+              32: "#23b052"}
+
+    """
+
+    HR_TO_MIN   : float = 60.0
+    HR_TO_SEC   : float = 60.0 * 60.0
+    HR_TO_MSEC  : float = 60.0 * 60.0 * 1000.0
+    MIN_TO_HR   : float = 1.0 / 60.0
+    MIN_TO_SEC  : float = 60.0
+    MIN_TO_MSEC : float = 60.0 * 1000.0
+    SEC_TO_HR   : float = 1.0 / (60.0 * 60.0)
+    SEC_TO_MIN  : float = 1.0 / 60.0
+    SEC_TO_MSEC : float = 1000.0
+    MSEC_TO_HR  : float = 1.0 / (60.0 * 60.0 * 1000.0)
+    MSEC_TO_MIN : float = 1.0 / (60.0 * 1000.0)
+    MSEC_TO_SEC : float = 1.0 / 1000.0
+
+    @staticmethod
+    def hr_to_min(hours): return float(hours * RAConst.HR_TO_MIN)
+    @staticmethod
+    def hr_to_sec(hours): return float(hours * RAConst.HR_TO_SEC)
+    @staticmethod
+    def hr_to_msec(hours): return float(hours * RAConst.HR_TO_MSEC)
+    @staticmethod
+    def min_to_hr(mins): return float(mins * RAConst.MIN_TO_HR)
+    @staticmethod
+    def min_to_sec(mins): return float(mins * RAConst.MIN_TO_SEC)
+    @staticmethod
+    def min_to_msec(mins): return float(mins * RAConst.MIN_TO_MSEC)
+    @staticmethod
+    def sec_to_hr(secs): return float(secs * RAConst.SEC_TO_HR)
+    @staticmethod
+    def sec_to_min(secs): return float(secs * RAConst.SEC_TO_MIN)
+    @staticmethod
+    def sec_to_msec(secs): return float(secs * RAConst.SEC_TO_MSEC)
+    @staticmethod
+    def msec_to_hr(msecs): return float(msecs * RAConst.MSEC_TO_HR)
+    @staticmethod
+    def msec_to_min(msecs): return float(msecs * RAConst.MSEC_TO_MIN)
+    @staticmethod
+    def msec_to_sec(msecs): return float(msecs * RAConst.MSEC_TO_SEC)
+
+    # These are the colors to indicate snapping. Used for PlayField
+    DIVISION_COLORS = {1: "#969696"
+                     , 2: "#b02323"
+                     , 3: "#8a23b0"
+                     , 4: "#2399b0"
+                     , 5: "#ffdfbd"
+                     , 6: "#b02378"
+                     , 8: "#b06c23"
+                     , 12: "#23b09d"
+                     , 16: "#3db023"
+                     , 24: "#94b023"
+                     , 32: "#23b052"}
```

### Comparing `reamber-0.1.7/reamber/base/Series.py` & `reamber-0.1.8/reamber/base/Series.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from __future__ import annotations
-
-from copy import deepcopy
-
-import numpy as np
-import pandas as pd
-
-
-class Series:
-    data: pd.Series
-
-    def __init__(self, **kwargs):
-        """If init from same class, we use kwarg to bypass the init"""
-        self.data = pd.Series(data=kwargs)
-
-    def __repr__(self):
-        return self.data.__repr__()
-
-    @staticmethod
-    def _from_series_allowed_names():
-        """Args not in list will be excluded in from_series"""
-        return []
-
-    @classmethod
-    def from_series(cls, data: pd.Series):
-        """An alternative __init__: Uses Series' to_dict as __init__ arguments
-
-        Notes:
-            Works by checking if data has column names in __init__ signature
-            _from_series_allowed_names.
-        """
-        try:
-            return cls(
-                **{k: v for k, v in data.to_dict().items() if k in
-                   cls._from_series_allowed_names()}
-            )
-        except TypeError as e:
-            raise TypeError(
-                f"from_series call is missing arguments: {e.args}. "
-                f"Make sure that those columns exist."
-            )
-
-    def __eq__(self, other: Series):
-        return np.all(self.data == other.data)
-
-    def deepcopy(self):
-        """Returns a deep copy of itself"""
-        return deepcopy(self)
+from __future__ import annotations
+
+from copy import deepcopy
+
+import numpy as np
+import pandas as pd
+
+
+class Series:
+    data: pd.Series
+
+    def __init__(self, **kwargs):
+        """If init from same class, we use kwarg to bypass the init"""
+        self.data = pd.Series(data=kwargs)
+
+    def __repr__(self):
+        return self.data.__repr__()
+
+    @staticmethod
+    def _from_series_allowed_names():
+        """Args not in list will be excluded in from_series"""
+        return []
+
+    @classmethod
+    def from_series(cls, data: pd.Series):
+        """An alternative __init__: Uses Series' to_dict as __init__ arguments
+
+        Notes:
+            Works by checking if data has column names in __init__ signature
+            _from_series_allowed_names.
+        """
+        try:
+            return cls(
+                **{k: v for k, v in data.to_dict().items() if k in
+                   cls._from_series_allowed_names()}
+            )
+        except TypeError as e:
+            raise TypeError(
+                f"from_series call is missing arguments: {e.args}. "
+                f"Make sure that those columns exist."
+            )
+
+    def __eq__(self, other: Series):
+        return np.all(self.data == other.data)
+
+    def deepcopy(self):
+        """Returns a deep copy of itself"""
+        return deepcopy(self)
```

### Comparing `reamber-0.1.7/reamber/base/lists/BpmList.py` & `reamber-0.1.8/reamber/base/lists/BpmList.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,92 +1,92 @@
-from __future__ import annotations
-
-from typing import TypeVar
-
-import numpy as np
-
-from reamber.algorithms.timing.TimingMap import TimingMap
-from reamber.algorithms.timing.utils.BpmChangeOffset import BpmChangeOffset
-from reamber.base.Bpm import Bpm
-from reamber.base.Property import list_props
-from reamber.base.lists.TimedList import TimedList
-
-Item = TypeVar('Item')
-
-
-@list_props(Bpm)
-class BpmList(TimedList[Item]):
-    def current_bpm(self, offset: float, sort=True, delta=0.1) -> Bpm:
-        """Finds the current BPM of the offset
-
-        Args:
-            offset: Offset to find associated bpm
-            sort: Whether to sort the bpm implicitly. IT MUST BE SORTED!
-            delta: A buffer for rounding errors
-
-        Returns:
-            The Bpm Class.
-        """
-
-        bpms = self.sorted() if sort else self
-        # noinspection PyTypeChecker
-        ix = int((np.sum((bpms.offset - offset - delta) <= 0)) - 1)
-        if ix < 0: raise IndexError(
-            f"Offset {offset} does not have a Bpm Associated with it.")
-        return bpms[ix]
-
-    def snap_offsets(self, nths: float = 1.0,
-                     last_offset: float = None) -> np.ndarray:
-        """Gets all of the nth snap offsets
-
-        For example::
-
-            SEC     1   2   3   4   5   6   7   8   9   10  11  12  13  14  ...
-            BPM     15                          7.5                         ...
-            SNAP    4/4 1/4 2/4 3/4 4/4 1/4 2/4 4/4 1/8 2/8 3/8 4/8 5/8 6/8 ...
-            BEAT    1               2           3
-            nths=1  ^               ^           ^
-            nths=2  ^       ^       ^       ^   ^               ^
-            nths=4  ^   ^   ^   ^   ^   ^   ^   ^       ^       ^       ^
-            nths=8  ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^   ^   ^   ^   ^   ^   ^
-
-        * Note: 15 BPM = 1 Beat per 4 seconds, 7.5 = 1 Beat per 8 seconds
-
-        The `^` indicates what offsets will be returned.
-
-        Args:
-            nths: Specifies the beat's snap, 1 = "1st"s, 4 = "4th"s, 16 = "16th"s
-            last_offset: The last offset to consider, if None, it uses the last BPM
-        """
-        bpm_list = self.deepcopy()
-
-        # BPM doesn't matter for the last.
-        if last_offset: bpm_list = bpm_list.append(Bpm(last_offset, bpm=0))
-
-        offsets = []
-        for i, j in zip(bpm_list[:-1], bpm_list[1:]):
-            offset_diff = j.offset - i.offset
-            nth_diff = i.beat_length / nths
-            offsets.append(np.arange(0, offset_diff, nth_diff) + i.offset)
-        return np.concatenate(offsets)
-
-    def to_timing_map(self) -> TimingMap:
-        return TimingMap.from_bpm_changes_offset(
-            bpm_changes_offset=[
-                BpmChangeOffset(b, m, o)
-                for b, m, o in zip(self.bpm, self.metronome, self.offset)
-            ]
-        )
-
-    def ave_bpm(self, last_offset: float = None) -> float:
-        """Calculates the average Bpm.
-
-        Args:
-            last_offset: If specified, this offset is used to
-                terminate activity, else use the last note offset.
-
-        Returns:
-            ``float`` of average BPM.
-        """
-        last_offset = last_offset if last_offset else self.last_offset()
-        sum_prod = np.sum(self.bpm * np.diff(self.offset, append=last_offset))
-        return sum_prod / (last_offset - self.first_offset())
+from __future__ import annotations
+
+from typing import TypeVar
+
+import numpy as np
+
+from reamber.algorithms.timing.TimingMap import TimingMap
+from reamber.algorithms.timing.utils.BpmChangeOffset import BpmChangeOffset
+from reamber.base.Bpm import Bpm
+from reamber.base.Property import list_props
+from reamber.base.lists.TimedList import TimedList
+
+Item = TypeVar('Item')
+
+
+@list_props(Bpm)
+class BpmList(TimedList[Item]):
+    def current_bpm(self, offset: float, sort=True, delta=0.1) -> Bpm:
+        """Finds the current BPM of the offset
+
+        Args:
+            offset: Offset to find associated bpm
+            sort: Whether to sort the bpm implicitly. IT MUST BE SORTED!
+            delta: A buffer for rounding errors
+
+        Returns:
+            The Bpm Class.
+        """
+
+        bpms = self.sorted() if sort else self
+        # noinspection PyTypeChecker
+        ix = int((np.sum((bpms.offset - offset - delta) <= 0)) - 1)
+        if ix < 0: raise IndexError(
+            f"Offset {offset} does not have a Bpm Associated with it.")
+        return bpms[ix]
+
+    def snap_offsets(self, nths: float = 1.0,
+                     last_offset: float = None) -> np.ndarray:
+        """Gets all of the nth snap offsets
+
+        For example::
+
+            SEC     1   2   3   4   5   6   7   8   9   10  11  12  13  14  ...
+            BPM     15                          7.5                         ...
+            SNAP    4/4 1/4 2/4 3/4 4/4 1/4 2/4 4/4 1/8 2/8 3/8 4/8 5/8 6/8 ...
+            BEAT    1               2           3
+            nths=1  ^               ^           ^
+            nths=2  ^       ^       ^       ^   ^               ^
+            nths=4  ^   ^   ^   ^   ^   ^   ^   ^       ^       ^       ^
+            nths=8  ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^ ^   ^   ^   ^   ^   ^   ^
+
+        * Note: 15 BPM = 1 Beat per 4 seconds, 7.5 = 1 Beat per 8 seconds
+
+        The `^` indicates what offsets will be returned.
+
+        Args:
+            nths: Specifies the beat's snap, 1 = "1st"s, 4 = "4th"s, 16 = "16th"s
+            last_offset: The last offset to consider, if None, it uses the last BPM
+        """
+        bpm_list = self.deepcopy()
+
+        # BPM doesn't matter for the last.
+        if last_offset: bpm_list = bpm_list.append(Bpm(last_offset, bpm=0))
+
+        offsets = []
+        for i, j in zip(bpm_list[:-1], bpm_list[1:]):
+            offset_diff = j.offset - i.offset
+            nth_diff = i.beat_length / nths
+            offsets.append(np.arange(0, offset_diff, nth_diff) + i.offset)
+        return np.concatenate(offsets)
+
+    def to_timing_map(self) -> TimingMap:
+        return TimingMap.from_bpm_changes_offset(
+            bpm_changes_offset=[
+                BpmChangeOffset(b, m, o)
+                for b, m, o in zip(self.bpm, self.metronome, self.offset)
+            ]
+        )
+
+    def ave_bpm(self, last_offset: float = None) -> float:
+        """Calculates the average Bpm.
+
+        Args:
+            last_offset: If specified, this offset is used to
+                terminate activity, else use the last note offset.
+
+        Returns:
+            ``float`` of average BPM.
+        """
+        last_offset = last_offset if last_offset else self.last_offset()
+        sum_prod = np.sum(self.bpm * np.diff(self.offset, append=last_offset))
+        return sum_prod / (last_offset - self.first_offset())
```

### Comparing `reamber-0.1.7/reamber/base/lists/BpmList.pyi` & `reamber-0.1.8/reamber/base/lists/BpmList.pyi`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from __future__ import annotations
-
-from typing import TypeVar
-
-import pandas as pd
-
-from reamber.algorithms.timing.TimingMap import TimingMap
-from reamber.base.lists.TimedList import TimedList
-
-Item = TypeVar('Item')
-
-
-class BpmList(TimedList[Item]):
-    def current_bpm(self, offset: float, sort=True) -> Item: ...
-
-    @property
-    def bpm(self) -> pd.Series: ...
-
-    @bpm.setter
-    def bpm(self, val): ...
-
-    @property
-    def metronome(self): ...
-
-    @metronome.setter
-    def metronome(self, val): ...
-
-    def snap_offsets(self, nths: float = 1.0,
-                     last_offset: float = None) -> np.ndarray: ...
-
-    def to_timing_map(self) -> TimingMap: ...
-
-    def ave_bpm(self, last_offset: float = None) -> float: ...
+from __future__ import annotations
+
+from typing import TypeVar
+
+import pandas as pd
+
+from reamber.algorithms.timing.TimingMap import TimingMap
+from reamber.base.lists.TimedList import TimedList
+
+Item = TypeVar('Item')
+
+
+class BpmList(TimedList[Item]):
+    def current_bpm(self, offset: float, sort=True) -> Item: ...
+
+    @property
+    def bpm(self) -> pd.Series: ...
+
+    @bpm.setter
+    def bpm(self, val): ...
+
+    @property
+    def metronome(self): ...
+
+    @metronome.setter
+    def metronome(self, val): ...
+
+    def snap_offsets(self, nths: float = 1.0,
+                     last_offset: float = None) -> np.ndarray: ...
+
+    def to_timing_map(self) -> TimingMap: ...
+
+    def ave_bpm(self, last_offset: float = None) -> float: ...
```

### Comparing `reamber-0.1.7/reamber/base/lists/__init__.py` & `reamber-0.1.8/reamber/base/lists/__init__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-"""The purpose of having separate classes for these objects is to facilitate
-functions that deal with the whole list
-
-Note: If it's possible to classify a certain object under notes or
-
-E.g.
-Instead of having to do a for loop to shift offset ...
-    for obj in map:
-        obj.offset += 100
-
-We can just call a function
-    map.notes.add_offset(100)
-
-There are also other helper classifiers such as MapDataFrame, which indicates
-that the class can be coerced into a pandas DataFrame.
-
-Convention
-When inheriting from this, place everything in lists package.
-Names inheriting should be plural, to be clear
-Also, inherit from the List[Obj] with the appropriate __init__
-
-E.g. class BpmList(List[Bpm], TimedList, ...)
-        def __init__(self, *args):
-            list.__init__(self, *args)
-
-Unlike most things in the repository, this is not a @dataclass
-
-"""
-
-import reamber.base.lists.notes
-from reamber.base.lists.BpmList import BpmList
-from reamber.base.lists.TimedList import TimedList
-
-__all__ = ['BpmList', 'TimedList', 'notes']
-
-"""Instructions on subclassing
-
-Whenever you want to create a class that inherits from this, there are a few 
-things to take note of
-
-1.1 Inherit from List[Obj]
-1.2 You need to declare the def __init__ for initialization of List
-    This is the generic way to do it
-        def __init__(self, *args):
-            list.__init__(self, *args)
-
-2.1 Union of List
-    Consider this
-    svs: Union[OsuSvList, List[OsuSv]] = 
-        field(default_factory=lambda: OsuSvList())
-    
-    Union here is required else PyCharm will complain that you cannot allocate
-        a List[OsuSv] to svs
-    
-    Of course it's not valid, that's where _recast comes into play
-    
-2.2 _recast
-    In the base class, __post_init__ will call _recast after initializing.
-    You just need to override _recast.
-    I made it a separate function because there may be multiple 
-        super().__post_init__ s
-    
-    def _recast(self) -> None:
-        super()._recast()  # Remember to call the super
-        self.svs = OsuSvList(self.svs)
-
-"""
+"""The purpose of having separate classes for these objects is to facilitate
+functions that deal with the whole list
+
+Note: If it's possible to classify a certain object under notes or
+
+E.g.
+Instead of having to do a for loop to shift offset ...
+    for obj in map:
+        obj.offset += 100
+
+We can just call a function
+    map.notes.add_offset(100)
+
+There are also other helper classifiers such as MapDataFrame, which indicates
+that the class can be coerced into a pandas DataFrame.
+
+Convention
+When inheriting from this, place everything in lists package.
+Names inheriting should be plural, to be clear
+Also, inherit from the List[Obj] with the appropriate __init__
+
+E.g. class BpmList(List[Bpm], TimedList, ...)
+        def __init__(self, *args):
+            list.__init__(self, *args)
+
+Unlike most things in the repository, this is not a @dataclass
+
+"""
+
+import reamber.base.lists.notes
+from reamber.base.lists.BpmList import BpmList
+from reamber.base.lists.TimedList import TimedList
+
+__all__ = ['BpmList', 'TimedList', 'notes']
+
+"""Instructions on subclassing
+
+Whenever you want to create a class that inherits from this, there are a few 
+things to take note of
+
+1.1 Inherit from List[Obj]
+1.2 You need to declare the def __init__ for initialization of List
+    This is the generic way to do it
+        def __init__(self, *args):
+            list.__init__(self, *args)
+
+2.1 Union of List
+    Consider this
+    svs: Union[OsuSvList, List[OsuSv]] = 
+        field(default_factory=lambda: OsuSvList())
+    
+    Union here is required else PyCharm will complain that you cannot allocate
+        a List[OsuSv] to svs
+    
+    Of course it's not valid, that's where _recast comes into play
+    
+2.2 _recast
+    In the base class, __post_init__ will call _recast after initializing.
+    You just need to override _recast.
+    I made it a separate function because there may be multiple 
+        super().__post_init__ s
+    
+    def _recast(self) -> None:
+        super()._recast()  # Remember to call the super
+        self.svs = OsuSvList(self.svs)
+
+"""
```

### Comparing `reamber-0.1.7/reamber/base/lists/notes/HitList.pyi` & `reamber-0.1.8/reamber/base/lists/notes/HitList.pyi`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-from __future__ import annotations
-
-from typing import List, Union, overload, Any
-
-import pandas as pd
-
-from reamber.base.Hit import Hit
-from reamber.base.lists.notes.NoteList import NoteList
-
-
-
-class HitList(NoteList[Hit]):
-
-    def __init__(self, objs: Union[List[Hit], Hit, pd.DataFrame]): ...
-
-    @property
-    def _item_class(self) -> type: ...
-
-    @overload
-    def __getitem__(self, item: slice) -> HitList: ...
-    @overload
-    def __getitem__(self, item: list) -> HitList: ...
-    @overload
-    def __getitem__(self, item: Any) -> HitList: ...
-    @overload
-    def __getitem__(self, item: int) -> Hit: ...
+from __future__ import annotations
+
+from typing import List, Union, overload, Any
+
+import pandas as pd
+
+from reamber.base.Hit import Hit
+from reamber.base.lists.notes.NoteList import NoteList
+
+
+
+class HitList(NoteList[Hit]):
+
+    def __init__(self, objs: Union[List[Hit], Hit, pd.DataFrame]): ...
+
+    @property
+    def _item_class(self) -> type: ...
+
+    @overload
+    def __getitem__(self, item: slice) -> HitList: ...
+    @overload
+    def __getitem__(self, item: list) -> HitList: ...
+    @overload
+    def __getitem__(self, item: Any) -> HitList: ...
+    @overload
+    def __getitem__(self, item: int) -> Hit: ...
```

### Comparing `reamber-0.1.7/reamber/base/lists/notes/HoldList.py` & `reamber-0.1.8/reamber/base/lists/notes/HoldList.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-from __future__ import annotations
-
-import warnings
-from typing import Tuple, TypeVar
-
-import pandas as pd
-
-from reamber.base.Hold import Hold
-from reamber.base.Property import list_props
-from reamber.base.lists.notes.NoteList import NoteList
-
-Item = TypeVar('Item', bound=Hold)
-
-
-@list_props(Hold)
-class HoldList(NoteList[Item]):
-
-    def last_offset(self) -> float:
-        """Get Last Note Offset. This includes the tail"""
-        return max(self.offset + self.length)
-
-    def first_last_offset(self) -> Tuple[float, float]:
-        """Get First and Last Note Offset. This includes the tail"""
-        return self.first_offset(), self.last_offset()
-
-    @property
-    def head_offset(self) -> pd.Series:
-        """Alias to self.offsets"""
-        return self.offset
-
-    @property
-    def tail_offset(self) -> pd.Series:
-        """Adds the offset to the length. """
-        return self.offset + self.length
-
-    def after(self,
-              offset: float,
-              include_end: bool = False,
-              include_tail: bool = False) -> HoldList:
-        """Trims the list to after specified offset
-
-        Notes:
-            This assumes that the length > 0. If negative
-            length are present then this will not work.
-
-            If the long note is partially within the bounds,
-            include tail will keep it.
-            E.g.       Trim <-----------
-                         [--+--]
-                            <-----------
-
-        Args:
-            offset: The lower bound in milliseconds
-            include_end: Whether to include the end
-            include_tail: Whether to include tail
-        """
-        if any(self.length < 0) and include_tail:
-            warnings.warn(
-                "after with include_tail does not work properly for "
-                "negative length"
-            )
-
-        if include_end:
-            # noinspection PyTypeChecker
-            return self[
-                self.offset + (self.length if include_tail else 0) >= offset]
-        else:
-            # noinspection PyTypeChecker
-            return self[
-                self.offset + (self.length if include_tail else 0) > offset]
-
-    def before(self,
-               offset: float,
-               include_end: bool = False,
-               include_head: bool = True) -> HoldList:
-        """Trims the list to after specified offset
-
-        Notes:
-            This assumes that the length > 0. If negative length are present
-            then this will not work.
-
-            If the long note is partially within the bounds,
-             include head will keep it.
-
-            E.g. -----------> Trim
-                         [--+--]
-                 ----------->
-
-        Args:
-            offset: The lower bound in milliseconds
-            include_end: Whether to include the end
-            include_head: Whether to include head
-        """
-        if any(self.length < 0) and not include_head:
-            warnings.warn(
-                "before without include_head does not work properly "
-                "for negative length."
-            )
-
-        if include_end:
-            # noinspection PyTypeChecker
-            return self[self.offset + (
-                self.length if not include_head else 0) <= offset]
-        else:
-            # noinspection PyTypeChecker
-            return self[self.offset + (
-                self.length if not include_head else 0) < offset]
-
-    def between(self,
-                lower_bound: float,
-                upper_bound: float,
-                include_ends: Tuple[bool, bool] = (True, False),
-                include_head: bool = True,
-                include_tail: bool = False) -> HoldList:
-        return self.after(lower_bound, include_end=include_ends[0],
-                          include_tail=include_tail) \
-            .before(upper_bound, include_end=include_ends[1],
-                    include_head=include_head)
+from __future__ import annotations
+
+import warnings
+from typing import Tuple, TypeVar
+
+import pandas as pd
+
+from reamber.base.Hold import Hold
+from reamber.base.Property import list_props
+from reamber.base.lists.notes.NoteList import NoteList
+
+Item = TypeVar('Item', bound=Hold)
+
+
+@list_props(Hold)
+class HoldList(NoteList[Item]):
+
+    def last_offset(self) -> float:
+        """Get Last Note Offset. This includes the tail"""
+        return max(self.offset + self.length)
+
+    def first_last_offset(self) -> Tuple[float, float]:
+        """Get First and Last Note Offset. This includes the tail"""
+        return self.first_offset(), self.last_offset()
+
+    @property
+    def head_offset(self) -> pd.Series:
+        """Alias to self.offsets"""
+        return self.offset
+
+    @property
+    def tail_offset(self) -> pd.Series:
+        """Adds the offset to the length. """
+        return self.offset + self.length
+
+    def after(self,
+              offset: float,
+              include_end: bool = False,
+              include_tail: bool = False) -> HoldList:
+        """Trims the list to after specified offset
+
+        Notes:
+            This assumes that the length > 0. If negative
+            length are present then this will not work.
+
+            If the long note is partially within the bounds,
+            include tail will keep it.
+            E.g.       Trim <-----------
+                         [--+--]
+                            <-----------
+
+        Args:
+            offset: The lower bound in milliseconds
+            include_end: Whether to include the end
+            include_tail: Whether to include tail
+        """
+        if any(self.length < 0) and include_tail:
+            warnings.warn(
+                "after with include_tail does not work properly for "
+                "negative length"
+            )
+
+        if include_end:
+            # noinspection PyTypeChecker
+            return self[
+                self.offset + (self.length if include_tail else 0) >= offset]
+        else:
+            # noinspection PyTypeChecker
+            return self[
+                self.offset + (self.length if include_tail else 0) > offset]
+
+    def before(self,
+               offset: float,
+               include_end: bool = False,
+               include_head: bool = True) -> HoldList:
+        """Trims the list to after specified offset
+
+        Notes:
+            This assumes that the length > 0. If negative length are present
+            then this will not work.
+
+            If the long note is partially within the bounds,
+             include head will keep it.
+
+            E.g. -----------> Trim
+                         [--+--]
+                 ----------->
+
+        Args:
+            offset: The lower bound in milliseconds
+            include_end: Whether to include the end
+            include_head: Whether to include head
+        """
+        if any(self.length < 0) and not include_head:
+            warnings.warn(
+                "before without include_head does not work properly "
+                "for negative length."
+            )
+
+        if include_end:
+            # noinspection PyTypeChecker
+            return self[self.offset + (
+                self.length if not include_head else 0) <= offset]
+        else:
+            # noinspection PyTypeChecker
+            return self[self.offset + (
+                self.length if not include_head else 0) < offset]
+
+    def between(self,
+                lower_bound: float,
+                upper_bound: float,
+                include_ends: Tuple[bool, bool] = (True, False),
+                include_head: bool = True,
+                include_tail: bool = False) -> HoldList:
+        return self.after(lower_bound, include_end=include_ends[0],
+                          include_tail=include_tail) \
+            .before(upper_bound, include_end=include_ends[1],
+                    include_head=include_head)
```

### Comparing `reamber-0.1.7/reamber/base/lists/notes/HoldList.pyi` & `reamber-0.1.8/reamber/base/lists/notes/HoldList.pyi`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from __future__ import annotations
-
-from typing import Tuple, Union, Any
-
-import pandas as pd
-
-from reamber.base import Hold
-from reamber.base.lists.notes.NoteList import NoteList
-
-
-class HoldList(NoteList[Hold]):
-
-    @staticmethod
-    def _default() -> dict: ...
-
-    @property
-    def length(self) -> Union[pd.Series, Any]: ...
-
-    @length.setter
-    def length(self, val): ...
-
-    def last_offset(self) -> float: ...
-
-    def first_last_offset(self) -> Tuple[float, float]: ...
-
-    @property
-    def head_offset(self) -> pd.Series: ...
-
-    @property
-    def tail_offset(self) -> pd.Series: ...
-
-    def after(self, offset: float, include_end: bool = False,
-              include_tail: bool = False) -> HoldList: ...
-
-    def before(self, offset: float, include_end: bool = False,
-               include_head: bool = True) -> HoldList: ...
-
-    def between(self, lower_bound: float, upper_bound: float,
-                include_ends: Tuple[bool, bool] = (True, False),
-                include_head: bool = True,
-                include_tail: bool = False) -> HoldList: ...
-
-    @property
-    def _item_class(self) -> type: ...
+from __future__ import annotations
+
+from typing import Tuple, Union, Any
+
+import pandas as pd
+
+from reamber.base import Hold
+from reamber.base.lists.notes.NoteList import NoteList
+
+
+class HoldList(NoteList[Hold]):
+
+    @staticmethod
+    def _default() -> dict: ...
+
+    @property
+    def length(self) -> Union[pd.Series, Any]: ...
+
+    @length.setter
+    def length(self, val): ...
+
+    def last_offset(self) -> float: ...
+
+    def first_last_offset(self) -> Tuple[float, float]: ...
+
+    @property
+    def head_offset(self) -> pd.Series: ...
+
+    @property
+    def tail_offset(self) -> pd.Series: ...
+
+    def after(self, offset: float, include_end: bool = False,
+              include_tail: bool = False) -> HoldList: ...
+
+    def before(self, offset: float, include_end: bool = False,
+               include_head: bool = True) -> HoldList: ...
+
+    def between(self, lower_bound: float, upper_bound: float,
+                include_ends: Tuple[bool, bool] = (True, False),
+                include_head: bool = True,
+                include_tail: bool = False) -> HoldList: ...
+
+    @property
+    def _item_class(self) -> type: ...
```

### Comparing `reamber-0.1.7/reamber/bms/BMSChannel.py` & `reamber-0.1.8/reamber/bms/BMSChannel.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-class BMSChannel:
-    # The value can be 1A, 1B ... 1Z, but so far I haven't seen any?
-    # If there is a need, I can change this.
-
-    TIME_SIG = b'02'
-    BPM_CHANGE = b'03'
-    EXBPM_CHANGE = b'08'
-
-    _HEADER = {
-        # b'01':"SAMPLE", Sample not supported
-        TIME_SIG: "TIME_SIG",
-        BPM_CHANGE: "BPM_CHANGE",
-        EXBPM_CHANGE: "EXBPM_CHANGE",
-        # b'09':"STOP", Stops not supported
-    }
-
-    BMS = {**_HEADER,
-           b'11': 0, b'21': 7,
-           b'12': 1, b'22': 8,
-           b'13': 2, b'23': 9,
-           b'14': 3, b'24': 10,
-           b'15': 4, b'25': 11,
-           b'16': 5, b'26': 12,
-           b'17': 6, b'27': 13}
-    BME = {**_HEADER,
-           b'16': 0, b'21': 8,
-           b'11': 1, b'22': 9,
-           b'12': 2, b'23': 10,
-           b'13': 3, b'24': 11,
-           b'14': 4, b'25': 12,
-           b'15': 5, b'28': 13,
-           b'18': 6, b'29': 14,
-           b'19': 7, b'26': 15}
-    PMS = {**_HEADER,
-           b'11': 0,
-           b'12': 1,
-           b'13': 2,
-           b'14': 3,
-           b'15': 4,
-           b'22': 5,
-           b'23': 6,
-           b'24': 7,
-           b'25': 8}
-    PMS_BME = {**_HEADER,
-               b'11': 0, b'21': 9,
-               b'12': 1, b'22': 10,
-               b'13': 2, b'23': 11,
-               b'14': 3, b'24': 12,
-               b'15': 4, b'25': 13,
-               b'18': 5, b'28': 14,
-               b'19': 6, b'29': 15,
-               b'16': 7, b'26': 16,
-               b'17': 8, b'27': 17}
-    PMS_5B = {**_HEADER,
-              b'13': 0,
-              b'14': 1,
-              b'15': 2,
-              b'22': 3,
-              b'23': 4}
+class BMSChannel:
+    # The value can be 1A, 1B ... 1Z, but so far I haven't seen any?
+    # If there is a need, I can change this.
+
+    TIME_SIG = b'02'
+    BPM_CHANGE = b'03'
+    EXBPM_CHANGE = b'08'
+
+    _HEADER = {
+        # b'01':"SAMPLE", Sample not supported
+        TIME_SIG: "TIME_SIG",
+        BPM_CHANGE: "BPM_CHANGE",
+        EXBPM_CHANGE: "EXBPM_CHANGE",
+        # b'09':"STOP", Stops not supported
+    }
+
+    BMS = {**_HEADER,
+           b'11': 0, b'21': 7,
+           b'12': 1, b'22': 8,
+           b'13': 2, b'23': 9,
+           b'14': 3, b'24': 10,
+           b'15': 4, b'25': 11,
+           b'16': 5, b'26': 12,
+           b'17': 6, b'27': 13}
+    BME = {**_HEADER,
+           b'16': 0, b'21': 8,
+           b'11': 1, b'22': 9,
+           b'12': 2, b'23': 10,
+           b'13': 3, b'24': 11,
+           b'14': 4, b'25': 12,
+           b'15': 5, b'28': 13,
+           b'18': 6, b'29': 14,
+           b'19': 7, b'26': 15}
+    PMS = {**_HEADER,
+           b'11': 0,
+           b'12': 1,
+           b'13': 2,
+           b'14': 3,
+           b'15': 4,
+           b'22': 5,
+           b'23': 6,
+           b'24': 7,
+           b'25': 8}
+    PMS_BME = {**_HEADER,
+               b'11': 0, b'21': 9,
+               b'12': 1, b'22': 10,
+               b'13': 2, b'23': 11,
+               b'14': 3, b'24': 12,
+               b'15': 4, b'25': 13,
+               b'18': 5, b'28': 14,
+               b'19': 6, b'29': 15,
+               b'16': 7, b'26': 16,
+               b'17': 8, b'27': 17}
+    PMS_5B = {**_HEADER,
+              b'13': 0,
+              b'14': 1,
+              b'15': 2,
+              b'22': 3,
+              b'23': 4}
```

### Comparing `reamber-0.1.7/reamber/bms/BMSMap.py` & `reamber-0.1.8/reamber/bms/BMSMap.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,504 +1,505 @@
-from __future__ import annotations
-
-import logging
-import warnings
-from codecs import encode, open as codecs_open
-from collections import namedtuple
-from dataclasses import dataclass, field
-from fractions import Fraction
-from typing import List, Dict
-
-import pandas as pd
-from numpy import base_repr
-
-from reamber.algorithms.timing import TimingMap
-from reamber.algorithms.timing.utils.BpmChangeOffset import BpmChangeOffset
-from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
-from reamber.algorithms.timing.utils.Snapper import Snapper
-from reamber.algorithms.timing.utils.find_lcm import find_lcm
-from reamber.algorithms.timing.utils.snap import Snap
-from reamber.base.Map import Map
-from reamber.base.Property import map_props, stack_props
-from reamber.base.lists.TimedList import TimedList
-from reamber.bms import BMSHit, BMSHold
-from reamber.bms.BMSBpm import BMSBpm
-from reamber.bms.BMSChannel import BMSChannel
-from reamber.bms.BMSMapMeta import BMSMapMeta
-from reamber.bms.lists import BMSBpmList
-from reamber.bms.lists.notes import BMSNoteList, BMSHitList, BMSHoldList
-
-MERGE_DELTA = 0.0001
-
-log = logging.getLogger(__name__)
-ENCODING = "shift_jis"
-
-DEFAULT_METRONOME = 4
-MAX_KEYS = 18
-
-
-@map_props()
-@dataclass
-class BMSMap(Map[BMSNoteList, BMSHitList, BMSHoldList, BMSBpmList],
-             BMSMapMeta):
-    objs: Dict[str, TimedList] = \
-        field(init=False,
-              default_factory=lambda: dict(hits=BMSHitList([]),
-                                           holds=BMSHoldList([]),
-                                           bpms=BMSBpmList([])))
-
-    @staticmethod
-    def read(lines: List[str],
-             note_channel_config: dict = BMSChannel.BME) -> BMSMap:
-        """Reads from a list of strings
-
-        Notes:
-            Channel config determines channel-column mapping
-
-        Args:
-            lines: List of strings from the file
-            note_channel_config: Get this config from reamber.bms.BMSChannel
-                If unsure, use the default BME.
-        """
-
-        header = {}
-        notes = []
-        bms = BMSMap()
-
-        lines = [line.strip() for line in lines]  # Redundancy for safety
-
-        for line in lines:
-            # Check if it's a command
-            if line.startswith('#'):
-                # We split it by b' '.
-                # If it's size == 2, then it's a header metadata
-                # Else, it may be an unfilled header or a note data.
-
-                # Sometimes titles have spaces, so we split maximum of once.
-                line_split = line.encode('shift_jis').strip().split(b' ', 1)
-
-                if len(line_split) == 2:
-                    # Header Metadata (Filled)
-                    log.debug(f"Add {line_split[0][1:]}: "
-                              f"{line_split[1]} header entry")
-
-                    # [1:] Remove the #
-                    header[line_split[0][1:]] = line_split[1]
-
-                elif len(line_split) == 1:
-                    # ASCII for numbers
-                    if ord('0') <= line_split[0][1] <= ord('9'):
-                        # Is note
-                        command, data = line_split[0].split(b':')
-                        measure = command[1:4]
-                        channel = command[4:6]
-                        sequence = data
-
-                        log.debug(f"Added {measure}, {channel}, "
-                                  f"{sequence} note entry")
-
-                        notes.append(dict(measure=measure, channel=channel,
-                                          sequence=sequence))
-
-        bms._read_file_header(header)
-        bms._read_notes(notes, note_channel_config)
-        return bms
-
-    @staticmethod
-    def read_file(file_path: str,
-                  note_channel_config: dict = BMSChannel.BME) -> BMSMap:
-        """Reads the file
-
-        Notes:
-            Channel config determines channel-column mapping
-
-        Args:
-            file_path: Path to file
-            note_channel_config: Get this config from reamber.bms.BMSChannel
-                If unsure, use the default BME.
-        """
-        with codecs_open(file_path, mode="r", encoding=ENCODING) as f:
-            lines = [line.strip() for line in f.readlines()]
-
-        return BMSMap.read(lines, note_channel_config=note_channel_config)
-
-    def write(self,
-              note_channel_config: dict = BMSChannel.BME,
-              no_sample_default: bytes = b'01') -> bytes:
-        b = b''
-        b += self._write_file_header()
-        b += b'\r\n' * 2
-        b += self._write_notes(note_channel_config=note_channel_config,
-                               no_sample_default=no_sample_default)
-        return b
-
-    def write_file(self, file_path: str,
-                   note_channel_config: dict = BMSChannel.BME,
-                   no_sample_default: bytes = b'01'):
-        """Writes the notes according to self data
-
-        Args:
-            file_path: Path to write to
-            note_channel_config: The config from BMSChannel
-            no_sample_default: The default byte to use when there's no sample
-        """
-        with open(file_path, "wb+") as f:
-            f.write(self.write(note_channel_config=note_channel_config,
-                               no_sample_default=no_sample_default))
-
-    def _read_file_header(self, data: dict):
-        self.artist = data.get(b'ARTIST', "")
-        self.title = data.get(b'TITLE', "")
-        self.version = data.get(b'PLAYLEVEL', "")
-        self.ln_end_channel = data.get(b'LNOBJ', b'')
-
-        # We cannot pop during a loop, so we save the keys then pop later.
-        to_pop = []
-        for k, v in data.items():
-            if k.upper().startswith(b'BPM') and len(k) == 5:
-                self.exbpms[k[3:]] = float(v)
-                to_pop.append(k)
-
-        for k, v in data.items():
-            if k.upper().startswith(b'WAV'):
-                self.samples[k[-2:]] = v
-                to_pop.append(k)
-
-        for k in to_pop:
-            data.pop(k)
-
-        # We do this to go in-line with the 
-        # temporary measure property assigned in _readNotes.
-        bpm = BMSBpm(0, bpm=float(data.pop(b'BPM')))
-
-        log.debug(f"Added initial BPM {bpm.bpm}")
-        self.bpms = self.bpms.append(bpm)
-
-        self.misc = data
-
-    def _write_file_header(self) -> bytes:
-        # May need to change all header stuff to a byte string first.
-
-        # noinspection PyTypeChecker
-        title = b"#TITLE " + (encode(self.title, ENCODING)
-                              if not isinstance(self.title,
-                                                bytes) else self.title)
-
-        # noinspection PyTypeChecker
-        artist = b"#ARTIST " + (encode(self.artist, ENCODING)
-                                if not isinstance(self.artist,
-                                                  bytes) else self.artist)
-
-        bpm = b"#BPM " + encode(str(self.bpms[0].bpm), ENCODING)
-
-        # noinspection PyTypeChecker
-        play_level = b"#PLAYLEVEL " + (
-            encode(self.version)
-            if not isinstance(self.version, bytes) else self.version
-        )
-        misc = []
-        for k, v in self.misc.items():
-            k = encode(k, ENCODING) if not isinstance(k, bytes) else k
-            v = encode(v, ENCODING) if not isinstance(v, bytes) else v
-            misc.append(b'#' + k + b' ' + v)
-
-        ln_obj = b''
-        if self.ln_end_channel:
-            # noinspection PyTypeChecker
-            ln_obj = b"#LNOBJ " + (
-                encode(self.ln_end_channel, ENCODING)
-                if not isinstance(self.ln_end_channel, bytes)
-                else self.ln_end_channel
-            )
-
-        assert len(self.bpms) < 35 * 36 + 35, \
-            f"The writer doesn't support more than {35 * 36 + 35} BPMs."
-
-        exbpms = []
-        for e, b in enumerate(self.bpms, 1):
-            exbpms.append(b'#BPM' + bytes(base_repr(e, 36).zfill(2), 'ascii') +
-                          b' ' + bytes(f"{b.bpm:.3f}", 'ascii'))
-
-        wavs = []
-        for k, v in self.samples.items():
-            k = encode(k, ENCODING) if not isinstance(k, bytes) else k
-            v = encode(v, ENCODING) if not isinstance(v, bytes) else v
-            wavs.append(b'#WAV' + k + b' ' + v)
-
-        return b'\r\n'.join(
-            [title, artist, bpm, play_level, *misc, ln_obj, *exbpms, *wavs]
-        )
-
-    def _read_notes(self, data: List[dict], config: dict):
-        """The data will be in the format [{measure, channel, seq}, ...]
-
-        This function helps .read
-        """
-
-        Hit = namedtuple('Hit', ['sample', 'snap'])
-        Hold = namedtuple('Hold', ['hit', 'sample', 'snap'])
-
-        bcs_s = [
-            BpmChangeSnap(
-                self.bpms[0].bpm, DEFAULT_METRONOME,
-                Snap(0, 0, DEFAULT_METRONOME),
-            )
-        ]
-        hits = [[] for _ in range(MAX_KEYS)]
-        holds = [[] for _ in range(MAX_KEYS)]
-        time_sig = {}
-
-        # The time_sig channel call does not sustain for more than 1 measure.
-        # Hence, if the time_sig changes, it's only for that measure.
-        # Thus, if the time_sig changes, it'll need correction
-        # for the next measure if needed.
-
-        config_rev = {v: k for k, v in config.items()}
-        for d in data:
-            measure = int(d['measure'])
-            channel = d['channel']
-            sequence = d['sequence']
-            pairs = [sequence[i:i + 2] for i in range(0, len(sequence), 2)]
-
-            if channel == config_rev['TIME_SIG']:
-                # Time Signatures always appear before BPM Changes
-                metronome = float(sequence) * DEFAULT_METRONOME
-                time_sig[measure] = metronome
-            else:
-                division = len(sequence) // 2
-
-                # If the latest BPM is of the same measure,
-                # this indicates that a TIME_SIG happened on the same measure
-                # We will force the current measure to use the changed time sig
-                metronome = time_sig.get(measure, DEFAULT_METRONOME)
-                for i, pair in enumerate(pairs):
-                    if pair == b'00' or pair == b'0': continue
-
-                    beat = Fraction(i, division) * metronome
-                    if channel in (config_rev['BPM_CHANGE'],
-                                   config_rev['EXBPM_CHANGE']):
-                        new_bpm = (
-                            int(pair, 16)
-                            if channel == config_rev['BPM_CHANGE']
-                            else float(self.exbpms[pair])
-                        )
-                        bcs_s.append(
-                            BpmChangeSnap(
-                                bpm=new_bpm,
-                                snap=Snap(measure, beat, metronome),
-                                metronome=metronome)
-                        )
-                    elif channel in config.keys():
-                        column = int(config[channel])
-
-                        if pair == self.ln_end_channel:
-                            try:
-                                # Yield LN Head from Hits
-                                prev_hit = hits[column].pop(-1)
-                                holds[column].append(
-                                    Hold(hit=prev_hit, sample=prev_hit.sample,
-                                         snap=Snap(measure, beat, None))
-                                )
-                            except IndexError:
-                                raise Exception(f"Failed to match LN Tail on "
-                                                f"Column {column}.")
-                        else:
-                            # Else it's a note
-                            sample = self.samples.get(pair, b'')
-                            hits[column].append(
-                                Hit(sample=sample,
-                                    snap=Snap(measure, beat, None))
-                            )
-        #
-        # measures = [*time_sig.keys(), -1]
-        # for measure0, measure1 in zip(measures[:-1], measures[1:]):
-        #     if measure1 - measure0 != 1:
-        #         time_sig[measure0 + 1] = DEFAULT_METRONOME
-        #
-        # for measure, metronome in sorted(time_sig.items(),
-        #                                  key=lambda x: x[0]):
-        #     bcs_measure = []
-        #     bcs_last_ix = 0
-        #     for e, bcs in enumerate(bcs_s):
-        #         if bcs.snap.measure == measure:
-        #             bcs_measure.append(bcs)
-        #         elif bcs.snap.measure > measure:
-        #             bcs_last_ix = e
-        #             break
-        #
-        #     for bcs in bcs_measure:
-        #         bcs.metronome = metronome
-        #         bcs.snap.metronome = metronome
-        # if not bcs_measure:
-        #     if bcs_last_ix == 0:
-        #         continue
-        #     bcs_prev = bcs_s[bcs_last_ix - 1]
-        #     bcs_s.insert(
-        #         bcs_last_ix,
-        #         BpmChangeSnap(bcs_prev.bpm, metronome,
-        #                       Snap(measure, 0, metronome))
-        #     )
-
-        if (
-            len(bcs_s) > 1 and
-            bcs_s[1].snap.measure == 0 and
-            bcs_s[1].snap.beat == 0
-        ):
-            # Special case:
-            # A Measure 0 Beat 0 BPM Change: overriding the global BPM
-            bcs_s.pop(0)
-
-        # Here we have to correct the lack of default metronome resets.
-        # The problem is that BMS' time sig changes are only for the current
-        # measure, on the contrary, we assume it carries forward to the next
-        # measures.
-        # The algorithm loops all changes and adds a time sig
-        # change if the prev is non-normal and the current is lacking a reset
-
-        bcs_s.sort(key=lambda x: x.snap)
-
-        tm = TimingMap.from_bpm_changes_snap(
-            initial_offset=0, bcs_s=bcs_s, reseat=False
-        )
-
-        if any(hits):
-            cols, samples, snaps = list(
-                zip(*[(k, h.sample, h.snap)
-                      for k, hits_col in enumerate(hits)
-                      for h in hits_col])
-            )
-
-            # TODO: Change offsets to accept multiple args to optimize this
-
-            offsets = tm.offsets(snaps)
-
-            self.hits = BMSHitList([
-                BMSHit(sample=sample, offset=offset, column=col)
-                for col, sample, offset in zip(cols, samples, offsets)
-            ])
-        else:
-            self.hits = BMSHitList([])
-
-        if any(holds):
-            cols, samples, snaps_head, snaps_tail = \
-                list(zip(*[(k, h.sample, h.hit.snap, h.snap)
-                           for k, holds_col in enumerate(holds)
-                           for h in holds_col]))
-            offsets_head = tm.offsets(snaps_head)
-            offsets_tail = tm.offsets(snaps_tail)
-
-            self.holds = BMSHoldList(
-                [BMSHold(sample=sample, offset=head_offset, column=col,
-                         length=tail_offset - head_offset)
-                 for sample, col, head_offset, tail_offset in
-                 zip(samples, cols, offsets_head, offsets_tail)]
-            )
-        else:
-            self.holds = BMSHoldList([])
-
-        tm = tm.reseat()
-        self.bpms = BMSBpmList(
-            [BMSBpm(offset=b.offset, bpm=b.bpm, metronome=b.metronome)
-             for b in tm.bpm_changes_offset]
-        )
-
-    def _write_notes(self,
-                     note_channel_config: dict,
-                     no_sample_default: bytes = b'01'):
-        """Writes the notes according to self data
-
-        Args:
-            note_channel_config: The config from BMSChannel
-            no_sample_default: The default byte to use when there's no sample
-        """
-        warnings.warn("Maps with many BPM Changes will likely break this.")
-
-        tm = TimingMap.from_bpm_changes_offset([
-            BpmChangeOffset(bpm=b.bpm, metronome=b.metronome,
-                            offset=b.offset) for b in self.bpms])
-
-        sample_map = {v: k for k, v in self.samples.items()}
-        channel_map = {v: k for k, v in note_channel_config.items()}
-
-        metronome_changes = [b for b in self.bpms if b.metronome != 4]
-
-        """Find the objects we want to snap here"""
-        snapper = Snapper()
-        hits = [
-            (snap, channel_map[column],
-             sample_map.get(sample, no_sample_default))
-            for snap, column, sample in
-            zip(tm.snaps(self.hits.offset, snapper),
-                self.hits.column, self.hits.sample)
-        ]
-
-        hold_heads = [
-            (snap, channel_map[column],
-             sample_map.get(sample, no_sample_default))
-            for snap, column, sample in
-            zip(tm.snaps(self.holds.offset, snapper),
-                self.holds.column, self.holds.sample)
-        ]
-
-        hold_tails = [
-            (snap, channel_map[column], self.ln_end_channel)
-            for snap, column in
-            zip(tm.snaps(self.holds.tail_offset, snapper),
-                self.holds.column)
-        ]
-
-        # BPM Changes
-        bpms = [(snap,
-                 channel_map["EXBPM_CHANGE"],
-                 bytes(base_repr(e + 1, 36).zfill(2), 'ascii'))
-                for e, snap in enumerate(tm.snaps(self.bpms.offset, snapper))]
-
-        # Metronome Changes
-        time_sigs = [
-            (snap,
-             channel_map["TIME_SIG"],
-             bytes(f"{float(m.metronome) / DEFAULT_METRONOME:.4f}", 'ascii'))
-            for snap, m in
-            zip(tm.snaps([m.offset for m in metronome_changes], snapper),
-                metronome_changes)
-        ]
-
-        df = pd.DataFrame(
-            [*hits, *hold_heads, *hold_tails, *bpms, *time_sigs],
-            columns=['snap', 'channel', 'value']
-        )
-        df['measure'] = [i.measure for i in df['snap']]
-        df['den'] = [i.beat.denominator * i.metronome for i in df['snap']]
-        df['num'] = [i.beat.numerator for i in df['snap']]
-        df['den'] = df['den'].astype(int)
-        df['num'] = df['num'].astype(int)
-        df = df.drop(['snap'], axis=1)
-        df['new_den'] = 0
-        for (measure, channel), dfg in df.groupby(['measure', 'channel']):
-            df.loc[(df.measure == measure) & (df.channel == channel),
-                   'new_den'] = find_lcm(dfg['den'].tolist(), 100)
-        df.num *= df.new_den / df.den
-        df = df.drop(['den'], axis=1)
-
-        # Generate the lines here
-        df = df.sort_values('channel')
-        dfgs = df.groupby(['measure', 'channel', 'new_den'])
-        lines = []
-        for (measure, channel, den), dfg in dfgs:
-            line = bytes(f'#{int(measure):03}', 'ascii') + channel + b':'
-            seq = [b'00'] * den
-            for _, row in dfg.iterrows():
-                seq[int(row['num'])] = row['value']
-            line += b''.join(seq)
-            lines.append(line)
-
-        return b'\r\n'.join(lines)
-
-    # noinspection PyMethodOverriding
-    def metadata(self, **kwargs) -> str:
-        """Grabs the map metadata"""
-        fmt = "{} - {}, {}"
-        return fmt.format(self.artist, self.title, self.version)
-
-    @stack_props()
-    class Stacker(Map.Stacker):
-        _props = ["sample"]
+from __future__ import annotations
+
+import logging
+import warnings
+from codecs import encode, open as codecs_open
+from collections import namedtuple
+from dataclasses import dataclass, field
+from fractions import Fraction
+from pathlib import Path
+from typing import List, Dict
+
+import pandas as pd
+from numpy import base_repr
+
+from reamber.algorithms.timing import TimingMap
+from reamber.algorithms.timing.utils.BpmChangeOffset import BpmChangeOffset
+from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
+from reamber.algorithms.timing.utils.Snapper import Snapper
+from reamber.algorithms.timing.utils.find_lcm import find_lcm
+from reamber.algorithms.timing.utils.snap import Snap
+from reamber.base.Map import Map
+from reamber.base.Property import map_props, stack_props
+from reamber.base.lists.TimedList import TimedList
+from reamber.bms import BMSHit, BMSHold
+from reamber.bms.BMSBpm import BMSBpm
+from reamber.bms.BMSChannel import BMSChannel
+from reamber.bms.BMSMapMeta import BMSMapMeta
+from reamber.bms.lists import BMSBpmList
+from reamber.bms.lists.notes import BMSNoteList, BMSHitList, BMSHoldList
+
+MERGE_DELTA = 0.0001
+
+log = logging.getLogger(__name__)
+ENCODING = "shift_jis"
+
+DEFAULT_METRONOME = 4
+MAX_KEYS = 18
+
+
+@map_props()
+@dataclass
+class BMSMap(Map[BMSNoteList, BMSHitList, BMSHoldList, BMSBpmList],
+             BMSMapMeta):
+    objs: Dict[str, TimedList] = \
+        field(init=False,
+              default_factory=lambda: dict(hits=BMSHitList([]),
+                                           holds=BMSHoldList([]),
+                                           bpms=BMSBpmList([])))
+
+    @staticmethod
+    def read(lines: List[str],
+             note_channel_config: dict = BMSChannel.BME) -> BMSMap:
+        """Reads from a list of strings
+
+        Notes:
+            Channel config determines channel-column mapping
+
+        Args:
+            lines: List of strings from the file
+            note_channel_config: Get this config from reamber.bms.BMSChannel
+                If unsure, use the default BME.
+        """
+
+        header = {}
+        notes = []
+        bms = BMSMap()
+
+        lines = [line.strip() for line in lines]  # Redundancy for safety
+
+        for line in lines:
+            # Check if it's a command
+            if line.startswith('#'):
+                # We split it by b' '.
+                # If it's size == 2, then it's a header metadata
+                # Else, it may be an unfilled header or a note data.
+
+                # Sometimes titles have spaces, so we split maximum of once.
+                line_split = line.encode('shift_jis').strip().split(b' ', 1)
+
+                if len(line_split) == 2:
+                    # Header Metadata (Filled)
+                    log.debug(f"Add {line_split[0][1:]}: "
+                              f"{line_split[1]} header entry")
+
+                    # [1:] Remove the #
+                    header[line_split[0][1:]] = line_split[1]
+
+                elif len(line_split) == 1:
+                    # ASCII for numbers
+                    if ord('0') <= line_split[0][1] <= ord('9'):
+                        # Is note
+                        command, data = line_split[0].split(b':')
+                        measure = command[1:4]
+                        channel = command[4:6]
+                        sequence = data
+
+                        log.debug(f"Added {measure}, {channel}, "
+                                  f"{sequence} note entry")
+
+                        notes.append(dict(measure=measure, channel=channel,
+                                          sequence=sequence))
+
+        bms._read_file_header(header)
+        bms._read_notes(notes, note_channel_config)
+        return bms
+
+    @staticmethod
+    def read_file(file_path: str | Path,
+                  note_channel_config: dict = BMSChannel.BME) -> BMSMap:
+        """Reads the file
+
+        Notes:
+            Channel config determines channel-column mapping
+
+        Args:
+            file_path: Path to file
+            note_channel_config: Get this config from reamber.bms.BMSChannel
+                If unsure, use the default BME.
+        """
+        with codecs_open(file_path, mode="r", encoding=ENCODING) as f:
+            lines = [line.strip() for line in f.readlines()]
+
+        return BMSMap.read(lines, note_channel_config=note_channel_config)
+
+    def write(self,
+              note_channel_config: dict = BMSChannel.BME,
+              no_sample_default: bytes = b'01') -> bytes:
+        b = b''
+        b += self._write_file_header()
+        b += b'\r\n' * 2
+        b += self._write_notes(note_channel_config=note_channel_config,
+                               no_sample_default=no_sample_default)
+        return b
+
+    def write_file(self, file_path: str | Path,
+                   note_channel_config: dict = BMSChannel.BME,
+                   no_sample_default: bytes = b'01'):
+        """Writes the notes according to self data
+
+        Args:
+            file_path: Path to write to
+            note_channel_config: The config from BMSChannel
+            no_sample_default: The default byte to use when there's no sample
+        """
+        with open(file_path, "wb+") as f:
+            f.write(self.write(note_channel_config=note_channel_config,
+                               no_sample_default=no_sample_default))
+
+    def _read_file_header(self, data: dict):
+        self.artist = data.get(b'ARTIST', "")
+        self.title = data.get(b'TITLE', "")
+        self.version = data.get(b'PLAYLEVEL', "")
+        self.ln_end_channel = data.get(b'LNOBJ', b'')
+
+        # We cannot pop during a loop, so we save the keys then pop later.
+        to_pop = []
+        for k, v in data.items():
+            if k.upper().startswith(b'BPM') and len(k) == 5:
+                self.exbpms[k[3:]] = float(v)
+                to_pop.append(k)
+
+        for k, v in data.items():
+            if k.upper().startswith(b'WAV'):
+                self.samples[k[-2:]] = v
+                to_pop.append(k)
+
+        for k in to_pop:
+            data.pop(k)
+
+        # We do this to go in-line with the 
+        # temporary measure property assigned in _readNotes.
+        bpm = BMSBpm(0, bpm=float(data.pop(b'BPM')))
+
+        log.debug(f"Added initial BPM {bpm.bpm}")
+        self.bpms = self.bpms.append(bpm)
+
+        self.misc = data
+
+    def _write_file_header(self) -> bytes:
+        # May need to change all header stuff to a byte string first.
+
+        # noinspection PyTypeChecker
+        title = b"#TITLE " + (encode(self.title, ENCODING)
+                              if not isinstance(self.title,
+                                                bytes) else self.title)
+
+        # noinspection PyTypeChecker
+        artist = b"#ARTIST " + (encode(self.artist, ENCODING)
+                                if not isinstance(self.artist,
+                                                  bytes) else self.artist)
+
+        bpm = b"#BPM " + encode(str(self.bpms[0].bpm), ENCODING)
+
+        # noinspection PyTypeChecker
+        play_level = b"#PLAYLEVEL " + (
+            encode(self.version)
+            if not isinstance(self.version, bytes) else self.version
+        )
+        misc = []
+        for k, v in self.misc.items():
+            k = encode(k, ENCODING) if not isinstance(k, bytes) else k
+            v = encode(v, ENCODING) if not isinstance(v, bytes) else v
+            misc.append(b'#' + k + b' ' + v)
+
+        ln_obj = b''
+        if self.ln_end_channel:
+            # noinspection PyTypeChecker
+            ln_obj = b"#LNOBJ " + (
+                encode(self.ln_end_channel, ENCODING)
+                if not isinstance(self.ln_end_channel, bytes)
+                else self.ln_end_channel
+            )
+
+        assert len(self.bpms) < 35 * 36 + 35, \
+            f"The writer doesn't support more than {35 * 36 + 35} BPMs."
+
+        exbpms = []
+        for e, b in enumerate(self.bpms, 1):
+            exbpms.append(b'#BPM' + bytes(base_repr(e, 36).zfill(2), 'ascii') +
+                          b' ' + bytes(f"{b.bpm:.3f}", 'ascii'))
+
+        wavs = []
+        for k, v in self.samples.items():
+            k = encode(k, ENCODING) if not isinstance(k, bytes) else k
+            v = encode(v, ENCODING) if not isinstance(v, bytes) else v
+            wavs.append(b'#WAV' + k + b' ' + v)
+
+        return b'\r\n'.join(
+            [title, artist, bpm, play_level, *misc, ln_obj, *exbpms, *wavs]
+        )
+
+    def _read_notes(self, data: List[dict], config: dict):
+        """The data will be in the format [{measure, channel, seq}, ...]
+
+        This function helps .read
+        """
+
+        Hit = namedtuple('Hit', ['sample', 'snap'])
+        Hold = namedtuple('Hold', ['hit', 'sample', 'snap'])
+
+        bcs_s = [
+            BpmChangeSnap(
+                self.bpms[0].bpm, DEFAULT_METRONOME,
+                Snap(0, 0, DEFAULT_METRONOME),
+            )
+        ]
+        hits = [[] for _ in range(MAX_KEYS)]
+        holds = [[] for _ in range(MAX_KEYS)]
+        time_sig = {}
+
+        # The time_sig channel call does not sustain for more than 1 measure.
+        # Hence, if the time_sig changes, it's only for that measure.
+        # Thus, if the time_sig changes, it'll need correction
+        # for the next measure if needed.
+
+        config_rev = {v: k for k, v in config.items()}
+        for d in data:
+            measure = int(d['measure'])
+            channel = d['channel']
+            sequence = d['sequence']
+            pairs = [sequence[i:i + 2] for i in range(0, len(sequence), 2)]
+
+            if channel == config_rev['TIME_SIG']:
+                # Time Signatures always appear before BPM Changes
+                metronome = float(sequence) * DEFAULT_METRONOME
+                time_sig[measure] = metronome
+            else:
+                division = len(sequence) // 2
+
+                # If the latest BPM is of the same measure,
+                # this indicates that a TIME_SIG happened on the same measure
+                # We will force the current measure to use the changed time sig
+                metronome = time_sig.get(measure, DEFAULT_METRONOME)
+                for i, pair in enumerate(pairs):
+                    if pair == b'00' or pair == b'0': continue
+
+                    beat = Fraction(i, division) * metronome
+                    if channel in (config_rev['BPM_CHANGE'],
+                                   config_rev['EXBPM_CHANGE']):
+                        new_bpm = (
+                            int(pair, 16)
+                            if channel == config_rev['BPM_CHANGE']
+                            else float(self.exbpms[pair])
+                        )
+                        bcs_s.append(
+                            BpmChangeSnap(
+                                bpm=new_bpm,
+                                snap=Snap(measure, beat, metronome),
+                                metronome=metronome)
+                        )
+                    elif channel in config.keys():
+                        column = int(config[channel])
+
+                        if pair == self.ln_end_channel:
+                            try:
+                                # Yield LN Head from Hits
+                                prev_hit = hits[column].pop(-1)
+                                holds[column].append(
+                                    Hold(hit=prev_hit, sample=prev_hit.sample,
+                                         snap=Snap(measure, beat, None))
+                                )
+                            except IndexError:
+                                raise Exception(f"Failed to match LN Tail on "
+                                                f"Column {column}.")
+                        else:
+                            # Else it's a note
+                            sample = self.samples.get(pair, b'')
+                            hits[column].append(
+                                Hit(sample=sample,
+                                    snap=Snap(measure, beat, None))
+                            )
+        #
+        # measures = [*time_sig.keys(), -1]
+        # for measure0, measure1 in zip(measures[:-1], measures[1:]):
+        #     if measure1 - measure0 != 1:
+        #         time_sig[measure0 + 1] = DEFAULT_METRONOME
+        #
+        # for measure, metronome in sorted(time_sig.items(),
+        #                                  key=lambda x: x[0]):
+        #     bcs_measure = []
+        #     bcs_last_ix = 0
+        #     for e, bcs in enumerate(bcs_s):
+        #         if bcs.snap.measure == measure:
+        #             bcs_measure.append(bcs)
+        #         elif bcs.snap.measure > measure:
+        #             bcs_last_ix = e
+        #             break
+        #
+        #     for bcs in bcs_measure:
+        #         bcs.metronome = metronome
+        #         bcs.snap.metronome = metronome
+        # if not bcs_measure:
+        #     if bcs_last_ix == 0:
+        #         continue
+        #     bcs_prev = bcs_s[bcs_last_ix - 1]
+        #     bcs_s.insert(
+        #         bcs_last_ix,
+        #         BpmChangeSnap(bcs_prev.bpm, metronome,
+        #                       Snap(measure, 0, metronome))
+        #     )
+
+        if (
+            len(bcs_s) > 1 and
+            bcs_s[1].snap.measure == 0 and
+            bcs_s[1].snap.beat == 0
+        ):
+            # Special case:
+            # A Measure 0 Beat 0 BPM Change: overriding the global BPM
+            bcs_s.pop(0)
+
+        # Here we have to correct the lack of default metronome resets.
+        # The problem is that BMS' time sig changes are only for the current
+        # measure, on the contrary, we assume it carries forward to the next
+        # measures.
+        # The algorithm loops all changes and adds a time sig
+        # change if the prev is non-normal and the current is lacking a reset
+
+        bcs_s.sort(key=lambda x: x.snap)
+
+        tm = TimingMap.from_bpm_changes_snap(
+            initial_offset=0, bcs_s=bcs_s, reseat=False
+        )
+
+        if any(hits):
+            cols, samples, snaps = list(
+                zip(*[(k, h.sample, h.snap)
+                      for k, hits_col in enumerate(hits)
+                      for h in hits_col])
+            )
+
+            # TODO: Change offsets to accept multiple args to optimize this
+
+            offsets = tm.offsets(snaps)
+
+            self.hits = BMSHitList([
+                BMSHit(sample=sample, offset=offset, column=col)
+                for col, sample, offset in zip(cols, samples, offsets)
+            ])
+        else:
+            self.hits = BMSHitList([])
+
+        if any(holds):
+            cols, samples, snaps_head, snaps_tail = \
+                list(zip(*[(k, h.sample, h.hit.snap, h.snap)
+                           for k, holds_col in enumerate(holds)
+                           for h in holds_col]))
+            offsets_head = tm.offsets(snaps_head)
+            offsets_tail = tm.offsets(snaps_tail)
+
+            self.holds = BMSHoldList(
+                [BMSHold(sample=sample, offset=head_offset, column=col,
+                         length=tail_offset - head_offset)
+                 for sample, col, head_offset, tail_offset in
+                 zip(samples, cols, offsets_head, offsets_tail)]
+            )
+        else:
+            self.holds = BMSHoldList([])
+
+        tm = tm.reseat()
+        self.bpms = BMSBpmList(
+            [BMSBpm(offset=b.offset, bpm=b.bpm, metronome=b.metronome)
+             for b in tm.bpm_changes_offset]
+        )
+
+    def _write_notes(self,
+                     note_channel_config: dict,
+                     no_sample_default: bytes = b'01'):
+        """Writes the notes according to self data
+
+        Args:
+            note_channel_config: The config from BMSChannel
+            no_sample_default: The default byte to use when there's no sample
+        """
+        warnings.warn("Maps with many BPM Changes will likely break this.")
+
+        tm = TimingMap.from_bpm_changes_offset([
+            BpmChangeOffset(bpm=b.bpm, metronome=b.metronome,
+                            offset=b.offset) for b in self.bpms])
+
+        sample_map = {v: k for k, v in self.samples.items()}
+        channel_map = {v: k for k, v in note_channel_config.items()}
+
+        metronome_changes = [b for b in self.bpms if b.metronome != 4]
+
+        """Find the objects we want to snap here"""
+        snapper = Snapper()
+        hits = [
+            (snap, channel_map[column],
+             sample_map.get(sample, no_sample_default))
+            for snap, column, sample in
+            zip(tm.snaps(self.hits.offset, snapper),
+                self.hits.column, self.hits.sample)
+        ]
+
+        hold_heads = [
+            (snap, channel_map[column],
+             sample_map.get(sample, no_sample_default))
+            for snap, column, sample in
+            zip(tm.snaps(self.holds.offset, snapper),
+                self.holds.column, self.holds.sample)
+        ]
+
+        hold_tails = [
+            (snap, channel_map[column], self.ln_end_channel)
+            for snap, column in
+            zip(tm.snaps(self.holds.tail_offset, snapper),
+                self.holds.column)
+        ]
+
+        # BPM Changes
+        bpms = [(snap,
+                 channel_map["EXBPM_CHANGE"],
+                 bytes(base_repr(e + 1, 36).zfill(2), 'ascii'))
+                for e, snap in enumerate(tm.snaps(self.bpms.offset, snapper))]
+
+        # Metronome Changes
+        time_sigs = [
+            (snap,
+             channel_map["TIME_SIG"],
+             bytes(f"{float(m.metronome) / DEFAULT_METRONOME:.4f}", 'ascii'))
+            for snap, m in
+            zip(tm.snaps([m.offset for m in metronome_changes], snapper),
+                metronome_changes)
+        ]
+
+        df = pd.DataFrame(
+            [*hits, *hold_heads, *hold_tails, *bpms, *time_sigs],
+            columns=['snap', 'channel', 'value']
+        )
+        df['measure'] = [i.measure for i in df['snap']]
+        df['den'] = [i.beat.denominator * i.metronome for i in df['snap']]
+        df['num'] = [i.beat.numerator for i in df['snap']]
+        df['den'] = df['den'].astype(int)
+        df['num'] = df['num'].astype(int)
+        df = df.drop(['snap'], axis=1)
+        df['new_den'] = 0
+        for (measure, channel), dfg in df.groupby(['measure', 'channel']):
+            df.loc[(df.measure == measure) & (df.channel == channel),
+                   'new_den'] = find_lcm(dfg['den'].tolist(), 100)
+        df.num *= df.new_den / df.den
+        df = df.drop(['den'], axis=1)
+
+        # Generate the lines here
+        df = df.sort_values('channel')
+        dfgs = df.groupby(['measure', 'channel', 'new_den'])
+        lines = []
+        for (measure, channel, den), dfg in dfgs:
+            line = bytes(f'#{int(measure):03}', 'ascii') + channel + b':'
+            seq = [b'00'] * den
+            for _, row in dfg.iterrows():
+                seq[int(row['num'])] = row['value']
+            line += b''.join(seq)
+            lines.append(line)
+
+        return b'\r\n'.join(lines)
+
+    # noinspection PyMethodOverriding
+    def metadata(self, **kwargs) -> str:
+        """Grabs the map metadata"""
+        fmt = "{} - {}, {}"
+        return fmt.format(self.artist, self.title, self.version)
+
+    @stack_props()
+    class Stacker(Map.Stacker):
+        _props = ["sample"]
```

### Comparing `reamber-0.1.7/reamber/bms/lists/BMSNotePkg.py` & `reamber-0.1.8/reamber/bms/lists/BMSNotePkg.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-from __future__ import annotations
-
-from typing import Dict, overload
-
-from reamber.bms.lists.notes.BMSHitList import BMSHitList
-from reamber.bms.lists.notes.BMSHoldList import BMSHoldList
-from reamber.bms.lists.notes.BMSNoteList import BMSNoteList
-
-
-class BMSNotePkg:
-    """This package holds both the hits and holds for each BMSMap"""
-
-    @overload
-    def __init__(self):
-        ...
-
-    @overload
-    def __init__(self, data_dict: Dict[str, BMSNoteList]):
-        ...
-
-    @overload
-    def __init__(self, hits: BMSHitList, holds: BMSHoldList):
-        ...
-
-    def __init__(self, data_dict=None, hits=None, holds=None):
-        """Initialize a package,
-
-        Can initialize with either overloaded method.
-
-        Args:
-            data_dict: The data dictionary,  it'll be directly assigned to
-                data_dict. The names must explicitly match
-            hits: The hits as a BMSHitList
-            holds: The holds as a BMSHoldList
-        """
-        if data_dict is not None:
-            self.data_dict = data_dict
-        elif hits is not None:
-            self.data_dict = {'hits': hits, 'holds': holds}
-        else:
-            self.data_dict: Dict[str, BMSNoteList] = {
-                'hits': BMSHitList(),
-                'holds': BMSHoldList()
-            }
-
-    def __iter__(self):
-        """Yields the Dictionary item by item"""
-        yield from self.data_dict
-
-    def data(self) -> Dict[str, BMSNoteList]:
-        """Returns the data dictionary of lists"""
-        return self.data_dict
-
-    # noinspection PyTypeChecker
-    def hits(self) -> BMSHitList:
-        """Returns the hitList from the dictionary"""
-        return self.data_dict['hits']
-
-    # noinspection PyTypeChecker
-    def holds(self) -> BMSHoldList:
-        """Returns the holdList from the dictionary"""
-        return self.data_dict['holds']
+from __future__ import annotations
+
+from typing import Dict, overload
+
+from reamber.bms.lists.notes.BMSHitList import BMSHitList
+from reamber.bms.lists.notes.BMSHoldList import BMSHoldList
+from reamber.bms.lists.notes.BMSNoteList import BMSNoteList
+
+
+class BMSNotePkg:
+    """This package holds both the hits and holds for each BMSMap"""
+
+    @overload
+    def __init__(self):
+        ...
+
+    @overload
+    def __init__(self, data_dict: Dict[str, BMSNoteList]):
+        ...
+
+    @overload
+    def __init__(self, hits: BMSHitList, holds: BMSHoldList):
+        ...
+
+    def __init__(self, data_dict=None, hits=None, holds=None):
+        """Initialize a package,
+
+        Can initialize with either overloaded method.
+
+        Args:
+            data_dict: The data dictionary,  it'll be directly assigned to
+                data_dict. The names must explicitly match
+            hits: The hits as a BMSHitList
+            holds: The holds as a BMSHoldList
+        """
+        if data_dict is not None:
+            self.data_dict = data_dict
+        elif hits is not None:
+            self.data_dict = {'hits': hits, 'holds': holds}
+        else:
+            self.data_dict: Dict[str, BMSNoteList] = {
+                'hits': BMSHitList(),
+                'holds': BMSHoldList()
+            }
+
+    def __iter__(self):
+        """Yields the Dictionary item by item"""
+        yield from self.data_dict
+
+    def data(self) -> Dict[str, BMSNoteList]:
+        """Returns the data dictionary of lists"""
+        return self.data_dict
+
+    # noinspection PyTypeChecker
+    def hits(self) -> BMSHitList:
+        """Returns the hitList from the dictionary"""
+        return self.data_dict['hits']
+
+    # noinspection PyTypeChecker
+    def holds(self) -> BMSHoldList:
+        """Returns the holdList from the dictionary"""
+        return self.data_dict['holds']
```

### Comparing `reamber-0.1.7/reamber/o2jam/O2JEventPackage.py` & `reamber-0.1.8/reamber/o2jam/O2JEventPackage.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,278 +1,278 @@
-"""EventPackage in OJN stores BPM, Notes, Measure Changes and AutoPlays.
-
-For each level (easy, normal, hard), the number of packages are specified.
-Each package header defines the number of events that will occur after it.
-
-By knowing the count of events and the location of the note, we find the offset
-
-Consider this::
-
-            P E P E E E E P E E P E P E E E E E E E E
-    Events  1   4         2     1   8
-    Snap      1   1 2 3 4   1 2   1   1 2 3 4 5 6 7 8
-    Measure 0   1         1     2   2
-    Note      ^       ^       ^   ^               ^
-
-We can find the note offsets by calculating the offset from a BPM List and
- taking a fraction of the beat by looking at the snap.
-
-Notice that some snaps have no data in them, these are useful to "pad" these
-notes into place if they have a complex snap.
-
-There are more specifications on other data decryption in open2jam_.
-
-_open2jam: https://open2jam.wordpress.com/
-
-"""
-
-from __future__ import annotations
-
-import logging
-from collections import deque
-from dataclasses import dataclass, field
-from struct import unpack
-from typing import List, Union, Dict
-
-from reamber.o2jam.O2JBpm import O2JBpm
-from reamber.o2jam.O2JHit import O2JHit
-from reamber.o2jam.O2JHold import O2JHold
-
-log = logging.getLogger(__name__)
-
-
-class O2JConst:
-    # These data are required to find out which notes are hits and holds
-    HIT_BYTES: bytes = b'\x00'
-    HOLD_HEAD_BYTES: bytes = b'\x02'
-    HOLD_TAIL_BYTES: bytes = b'\x03'
-
-
-class O2JNoteChannel:
-    MEASURE_FRACTION: int = 0
-    BPM_CHANGE: int = 1
-    COL_1: int = 2
-    COL_2: int = 3
-    COL_3: int = 4
-    COL_4: int = 5
-    COL_5: int = 6
-    COL_6: int = 7
-    COL_7: int = 8
-    COL_RANGE: range = range(2, 9)
-    AUTOPLAY_1: int = 9
-    AUTOPLAY_2: int = 10
-    AUTOPLAY_3: int = 11
-    AUTOPLAY_4: int = 12
-    AUTOPLAY_5: int = 13
-    AUTOPLAY_6: int = 14
-    AUTOPLAY_7: int = 15
-    AUTOPLAY_8: int = 16
-    AUTOPLAY_9: int = 17
-    AUTOPLAY_10: int = 18
-    AUTOPLAY_11: int = 19
-    AUTOPLAY_12: int = 20
-    AUTOPLAY_13: int = 21
-    AUTOPLAY_14: int = 22
-    AUTOPLAY_RANGE: range = range(9, 23)
-    # Is there more?
-    # Don't worry about the size of this obj, all of them are static.
-
-
-@dataclass
-class O2JEventMeasureChange:
-    """Determines the length of a measure
-
-    Notes:
-        When the channel is 0(fractional measure), the 4 bytes are a float,
-
-    Examples:
-        If 0.75, this measure be only 75% long
-    """
-
-    frac_length: float = 1.0
-
-
-@dataclass
-class O2JEventPackage:
-    measure: int = 0  # Len 4 (Int)
-    channel: int = -1  # Len 2 (Short)
-
-    # There's a Len 2 (Short) indicating how many events there are.
-    # Then it's followed by that amount of events.
-    events: List[Union[O2JBpm, O2JHit, O2JHold, O2JEventMeasureChange]] = \
-        field(default_factory=lambda: [])
-
-    @staticmethod
-    def read_event_packages(data: bytes, lvl_pkg_counts: List[int]) \
-        -> List[List[O2JEventPackage]]:
-        """Reads all events, data found after the metadata
-
-        Args:
-            lvl_pkg_counts: The count of pkgs per level
-            data: All the event data in bytes.
-        """
-
-        # Don't think we can get all the offsets of notes,
-        # we'll firstly find their measures, then calculate offsets separately.
-        # I have doubts because of bpm changes
-
-        # Thus, read LNs in a different loop, not dynamically like stepmania.
-
-        # Additional variables
-        # O2JHit.measure
-        # O2JHold.measure
-        # O2JHold.tailMeasure
-
-        lvls: List[List[O2JEventPackage]] = []
-        data_q = deque(data)
-
-        # Column, Offset
-        hold_buffer: Dict[int, O2JHold] = {}
-
-        # For each level, we read the amount of packages
-        for lvl_pkg_count in lvl_pkg_counts:
-            log.debug(f"Loading New Level with {lvl_pkg_count} Packages")
-            # noinspection PyTypeChecker
-            lvl_pkg: List[O2JEventPackage] = [None] * lvl_pkg_count
-            for pkg_e in range(0, lvl_pkg_count):
-                if len(data_q) == 0: break
-                pkg = O2JEventPackage()
-                pkg_data = []
-                for _ in range(8):
-                    pkg_data.append(data_q.popleft())
-
-                pkg.measure = unpack("<i", bytes(pkg_data[0:4]))[0]
-                pkg.channel = unpack("<h", bytes(pkg_data[4:6]))[0]
-                event_count = unpack("<h", bytes(pkg_data[6:8]))[0]
-
-                events_data = []
-                for i in range(4 * event_count):
-                    events_data.append(data_q.popleft())
-                events_data = bytes(events_data)
-
-                if pkg.channel in O2JNoteChannel.COL_RANGE:
-                    pkg.events += O2JEventPackage.read_events_note(
-                        events_data,
-                        pkg.channel - 2,
-                        # Package CHN - 2 is the column
-                        hold_buffer,
-                        pkg.measure
-                    )
-                elif pkg.channel == O2JNoteChannel.BPM_CHANGE:
-                    pkg.events += O2JEventPackage.read_events_bpm(
-                        events_data,
-                        pkg.measure
-                    )
-                elif pkg.channel == O2JNoteChannel.MEASURE_FRACTION:
-                    measure_frac = O2JEventPackage.read_events_measure(
-                        events_data
-                    )
-                    pkg.events.append(O2JEventMeasureChange(measure_frac))
-                lvl_pkg[pkg_e] = pkg
-            lvls.append(lvl_pkg)
-        return lvls
-
-    @staticmethod
-    def read_events_measure(events_data: bytes) -> float:
-        """Reads the fractional measure data.
-
-        Notes:
-            This may not work as intended,
-            there's no ojn files to test this feature.
-
-        Args:
-            events_data: The 4 byte data point to unpack.
-
-        Returns:
-            Returns a float indicating the fraction of the measure.
-        """
-        log.warning(
-            "Fractional measure isn't confidently implemented, "
-            "conversion may fail."
-        )
-        return unpack("<f", events_data[0:4])[0]
-
-    @staticmethod
-    def read_events_bpm(data: bytes, curr_measure: float) -> List[O2JBpm]:
-        """Reads the event's bpms.
-
-        Like Notes, this can have disabled points where Bpm == 0,
-         that means there's no bpm there.
-
-        This is under the presumption that Bpm == 0 is not supported at all.
-
-        Args:
-            data: The bytes to unpack.
-            curr_measure: The current measure, used to calculate offset later.
-
-        Returns:
-            Returns a List of Bpm Points found.
-        """
-        event_count = len(data) // 4
-        bpms = []
-
-        for i in range(event_count):
-            bpm = unpack("<f", data[i * 4:(i + 1) * 4])[0]
-            if bpm == 0: continue
-            log.debug(f"Add BPM {bpm} @ {curr_measure + i / event_count}")
-            bpm = O2JBpm(bpm=bpm, offset=0)
-            bpm.measure = curr_measure + i / event_count
-            bpms.append(bpm)
-
-        return bpms
-
-    @staticmethod
-    def read_events_note(data: bytes, column: int,
-                         hold_buffer: Dict[int, O2JHold],
-                         curr_measure: float) -> List[Union[O2JHit, O2JHold]]:
-        """Reads the event's notes.
-
-        This can have disabled points dictated by the first 2 bytes
-         (see: 'enabled')
-
-        Args:
-            data: The bytes to unpack.
-            column: Current column
-            hold_buffer: The hold buffer, this acts like a static variable to
-             facilitate head and tail matching.
-            curr_measure: The current measure, used to calculate offset later.
-
-        Returns:
-            Returns a List of Bpm Points found.
-        """
-
-        notes = []
-
-        event_count = len(data) // 4
-
-        for i in range(event_count):
-            enabled = unpack("<h", bytes(data[0 + i * 4:2 + i * 4]))[0]
-            if enabled == 0: continue
-
-            sub_measure = i / event_count + curr_measure
-            volume_pan = int.from_bytes(
-                unpack("<s", data[2 + i * 4:3 + i * 4])[0], 'little'
-            )
-            volume, pan = volume_pan // 16, volume_pan % 16
-            note_type = unpack("<c", data[3 + i * 4:4 + i * 4])[0]
-
-            log.debug(f"Event Data: {data[0 + i * 4:4 + i * 4]}")
-
-            if note_type == O2JConst.HIT_BYTES:
-                hit = O2JHit(volume=volume, pan=pan, offset=0, column=column)
-                hit.measure = sub_measure
-                notes.append(hit)
-                log.debug(f"Appended Note {column} at {sub_measure}")
-
-            elif note_type == O2JConst.HOLD_HEAD_BYTES:
-                hold = O2JHold(volume=volume, pan=pan, column=column,
-                               length=-1, offset=0)
-                hold.measure = sub_measure
-                hold_buffer[column] = hold
-
-            elif note_type == O2JConst.HOLD_TAIL_BYTES:
-                hold = hold_buffer.pop(column)
-                hold.tail_measure = sub_measure
-                notes.append(hold)
-                log.debug(f"Appended LNote {column} at {sub_measure}, "
-                          f"Tail:{hold.tail_measure}")
-        return notes
+"""EventPackage in OJN stores BPM, Notes, Measure Changes and AutoPlays.
+
+For each level (easy, normal, hard), the number of packages are specified.
+Each package header defines the number of events that will occur after it.
+
+By knowing the count of events and the location of the note, we find the offset
+
+Consider this::
+
+            P E P E E E E P E E P E P E E E E E E E E
+    Events  1   4         2     1   8
+    Snap      1   1 2 3 4   1 2   1   1 2 3 4 5 6 7 8
+    Measure 0   1         1     2   2
+    Note      ^       ^       ^   ^               ^
+
+We can find the note offsets by calculating the offset from a BPM List and
+ taking a fraction of the beat by looking at the snap.
+
+Notice that some snaps have no data in them, these are useful to "pad" these
+notes into place if they have a complex snap.
+
+There are more specifications on other data decryption in open2jam_.
+
+_open2jam: https://open2jam.wordpress.com/
+
+"""
+
+from __future__ import annotations
+
+import logging
+from collections import deque
+from dataclasses import dataclass, field
+from struct import unpack
+from typing import List, Union, Dict
+
+from reamber.o2jam.O2JBpm import O2JBpm
+from reamber.o2jam.O2JHit import O2JHit
+from reamber.o2jam.O2JHold import O2JHold
+
+log = logging.getLogger(__name__)
+
+
+class O2JConst:
+    # These data are required to find out which notes are hits and holds
+    HIT_BYTES: bytes = b'\x00'
+    HOLD_HEAD_BYTES: bytes = b'\x02'
+    HOLD_TAIL_BYTES: bytes = b'\x03'
+
+
+class O2JNoteChannel:
+    MEASURE_FRACTION: int = 0
+    BPM_CHANGE: int = 1
+    COL_1: int = 2
+    COL_2: int = 3
+    COL_3: int = 4
+    COL_4: int = 5
+    COL_5: int = 6
+    COL_6: int = 7
+    COL_7: int = 8
+    COL_RANGE: range = range(2, 9)
+    AUTOPLAY_1: int = 9
+    AUTOPLAY_2: int = 10
+    AUTOPLAY_3: int = 11
+    AUTOPLAY_4: int = 12
+    AUTOPLAY_5: int = 13
+    AUTOPLAY_6: int = 14
+    AUTOPLAY_7: int = 15
+    AUTOPLAY_8: int = 16
+    AUTOPLAY_9: int = 17
+    AUTOPLAY_10: int = 18
+    AUTOPLAY_11: int = 19
+    AUTOPLAY_12: int = 20
+    AUTOPLAY_13: int = 21
+    AUTOPLAY_14: int = 22
+    AUTOPLAY_RANGE: range = range(9, 23)
+    # Is there more?
+    # Don't worry about the size of this obj, all of them are static.
+
+
+@dataclass
+class O2JEventMeasureChange:
+    """Determines the length of a measure
+
+    Notes:
+        When the channel is 0(fractional measure), the 4 bytes are a float,
+
+    Examples:
+        If 0.75, this measure be only 75% long
+    """
+
+    frac_length: float = 1.0
+
+
+@dataclass
+class O2JEventPackage:
+    measure: int = 0  # Len 4 (Int)
+    channel: int = -1  # Len 2 (Short)
+
+    # There's a Len 2 (Short) indicating how many events there are.
+    # Then it's followed by that amount of events.
+    events: List[Union[O2JBpm, O2JHit, O2JHold, O2JEventMeasureChange]] = \
+        field(default_factory=lambda: [])
+
+    @staticmethod
+    def read_event_packages(data: bytes, lvl_pkg_counts: List[int]) \
+        -> List[List[O2JEventPackage]]:
+        """Reads all events, data found after the metadata
+
+        Args:
+            lvl_pkg_counts: The count of pkgs per level
+            data: All the event data in bytes.
+        """
+
+        # Don't think we can get all the offsets of notes,
+        # we'll firstly find their measures, then calculate offsets separately.
+        # I have doubts because of bpm changes
+
+        # Thus, read LNs in a different loop, not dynamically like stepmania.
+
+        # Additional variables
+        # O2JHit.measure
+        # O2JHold.measure
+        # O2JHold.tailMeasure
+
+        lvls: List[List[O2JEventPackage]] = []
+        data_q = deque(data)
+
+        # Column, Offset
+        hold_buffer: Dict[int, O2JHold] = {}
+
+        # For each level, we read the amount of packages
+        for lvl_pkg_count in lvl_pkg_counts:
+            log.debug(f"Loading New Level with {lvl_pkg_count} Packages")
+            # noinspection PyTypeChecker
+            lvl_pkg: List[O2JEventPackage] = [None] * lvl_pkg_count
+            for pkg_e in range(0, lvl_pkg_count):
+                if len(data_q) == 0: break
+                pkg = O2JEventPackage()
+                pkg_data = []
+                for _ in range(8):
+                    pkg_data.append(data_q.popleft())
+
+                pkg.measure = unpack("<i", bytes(pkg_data[0:4]))[0]
+                pkg.channel = unpack("<h", bytes(pkg_data[4:6]))[0]
+                event_count = unpack("<h", bytes(pkg_data[6:8]))[0]
+
+                events_data = []
+                for i in range(4 * event_count):
+                    events_data.append(data_q.popleft())
+                events_data = bytes(events_data)
+
+                if pkg.channel in O2JNoteChannel.COL_RANGE:
+                    pkg.events += O2JEventPackage.read_events_note(
+                        events_data,
+                        pkg.channel - 2,
+                        # Package CHN - 2 is the column
+                        hold_buffer,
+                        pkg.measure
+                    )
+                elif pkg.channel == O2JNoteChannel.BPM_CHANGE:
+                    pkg.events += O2JEventPackage.read_events_bpm(
+                        events_data,
+                        pkg.measure
+                    )
+                elif pkg.channel == O2JNoteChannel.MEASURE_FRACTION:
+                    measure_frac = O2JEventPackage.read_events_measure(
+                        events_data
+                    )
+                    pkg.events.append(O2JEventMeasureChange(measure_frac))
+                lvl_pkg[pkg_e] = pkg
+            lvls.append(lvl_pkg)
+        return lvls
+
+    @staticmethod
+    def read_events_measure(events_data: bytes) -> float:
+        """Reads the fractional measure data.
+
+        Notes:
+            This may not work as intended,
+            there's no ojn files to test this feature.
+
+        Args:
+            events_data: The 4 byte data point to unpack.
+
+        Returns:
+            Returns a float indicating the fraction of the measure.
+        """
+        log.warning(
+            "Fractional measure isn't confidently implemented, "
+            "conversion may fail."
+        )
+        return unpack("<f", events_data[0:4])[0]
+
+    @staticmethod
+    def read_events_bpm(data: bytes, curr_measure: float) -> List[O2JBpm]:
+        """Reads the event's bpms.
+
+        Like Notes, this can have disabled points where Bpm == 0,
+         that means there's no bpm there.
+
+        This is under the presumption that Bpm == 0 is not supported at all.
+
+        Args:
+            data: The bytes to unpack.
+            curr_measure: The current measure, used to calculate offset later.
+
+        Returns:
+            Returns a List of Bpm Points found.
+        """
+        event_count = len(data) // 4
+        bpms = []
+
+        for i in range(event_count):
+            bpm = unpack("<f", data[i * 4:(i + 1) * 4])[0]
+            if bpm == 0: continue
+            log.debug(f"Add BPM {bpm} @ {curr_measure + i / event_count}")
+            bpm = O2JBpm(bpm=bpm, offset=0)
+            bpm.measure = curr_measure + i / event_count
+            bpms.append(bpm)
+
+        return bpms
+
+    @staticmethod
+    def read_events_note(data: bytes, column: int,
+                         hold_buffer: Dict[int, O2JHold],
+                         curr_measure: float) -> List[Union[O2JHit, O2JHold]]:
+        """Reads the event's notes.
+
+        This can have disabled points dictated by the first 2 bytes
+         (see: 'enabled')
+
+        Args:
+            data: The bytes to unpack.
+            column: Current column
+            hold_buffer: The hold buffer, this acts like a static variable to
+             facilitate head and tail matching.
+            curr_measure: The current measure, used to calculate offset later.
+
+        Returns:
+            Returns a List of Bpm Points found.
+        """
+
+        notes = []
+
+        event_count = len(data) // 4
+
+        for i in range(event_count):
+            enabled = unpack("<h", bytes(data[0 + i * 4:2 + i * 4]))[0]
+            if enabled == 0: continue
+
+            sub_measure = i / event_count + curr_measure
+            volume_pan = int.from_bytes(
+                unpack("<s", data[2 + i * 4:3 + i * 4])[0], 'little'
+            )
+            volume, pan = volume_pan // 16, volume_pan % 16
+            note_type = unpack("<c", data[3 + i * 4:4 + i * 4])[0]
+
+            log.debug(f"Event Data: {data[0 + i * 4:4 + i * 4]}")
+
+            if note_type == O2JConst.HIT_BYTES:
+                hit = O2JHit(volume=volume, pan=pan, offset=0, column=column)
+                hit.measure = sub_measure
+                notes.append(hit)
+                log.debug(f"Appended Note {column} at {sub_measure}")
+
+            elif note_type == O2JConst.HOLD_HEAD_BYTES:
+                hold = O2JHold(volume=volume, pan=pan, column=column,
+                               length=-1, offset=0)
+                hold.measure = sub_measure
+                hold_buffer[column] = hold
+
+            elif note_type == O2JConst.HOLD_TAIL_BYTES:
+                hold = hold_buffer.pop(column)
+                hold.tail_measure = sub_measure
+                notes.append(hold)
+                log.debug(f"Appended LNote {column} at {sub_measure}, "
+                          f"Tail:{hold.tail_measure}")
+        return notes
```

### Comparing `reamber-0.1.7/reamber/o2jam/O2JHold.py` & `reamber-0.1.8/reamber/o2jam/O2JHold.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from reamber.base import item_props
-from reamber.base.Hold import Hold
-from reamber.o2jam.O2JNoteMeta import O2JNoteMeta
-
-
-@item_props()
-class O2JHold(Hold, O2JNoteMeta):
-
-    def __init__(self,
-                 offset: float,
-                 column: int,
-                 length: float,
-                 volume: int = 0,
-                 pan: int = 8,
-                 **kwargs):
-        super().__init__(
-            offset=offset, column=column, length=length, volume=volume,
-            pan=pan, **kwargs
-        )
+from reamber.base import item_props
+from reamber.base.Hold import Hold
+from reamber.o2jam.O2JNoteMeta import O2JNoteMeta
+
+
+@item_props()
+class O2JHold(Hold, O2JNoteMeta):
+
+    def __init__(self,
+                 offset: float,
+                 column: int,
+                 length: float,
+                 volume: int = 0,
+                 pan: int = 8,
+                 **kwargs):
+        super().__init__(
+            offset=offset, column=column, length=length, volume=volume,
+            pan=pan, **kwargs
+        )
```

### Comparing `reamber-0.1.7/reamber/o2jam/O2JMap.py` & `reamber-0.1.8/reamber/o2jam/O2JMap.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,159 +1,159 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import List, Dict, TYPE_CHECKING
-
-from reamber.base.Map import Map
-from reamber.base.Property import map_props
-from reamber.base.RAConst import RAConst
-from reamber.base.lists import TimedList
-from reamber.o2jam.O2JBpm import O2JBpm
-from reamber.o2jam.O2JEventPackage import O2JEventPackage
-from reamber.o2jam.O2JHit import O2JHit
-from reamber.o2jam.O2JHold import O2JHold
-from reamber.o2jam.lists.O2JBpmList import O2JBpmList
-from reamber.o2jam.lists.notes import O2JNoteList
-from reamber.o2jam.lists.notes.O2JHitList import O2JHitList
-from reamber.o2jam.lists.notes.O2JHoldList import O2JHoldList
-
-if TYPE_CHECKING:
-    from reamber.o2jam.O2JMapSet import O2JMapSet
-
-import logging
-
-log = logging.getLogger(__name__)
-
-
-@map_props()
-@dataclass
-class O2JMap(Map[O2JNoteList, O2JHitList, O2JHoldList, O2JBpmList]):
-    """This holds a single level of a .ojn file out of a total of three.
-
-    This class only holds the data of notes and bpms. The rest can be found in
-    the parent O2JMapSet instance.
-
-    We won't support OJM, see why in O2JMapSet. """
-
-    objs: Dict[str, TimedList] = \
-        field(init=False,
-              default_factory=lambda: dict(hits=O2JHitList([]),
-                                           holds=O2JHoldList([]),
-                                           bpms=O2JBpmList([])))
-
-    # noinspection PyUnresolvedReferences
-    @staticmethod
-    def read_pkgs(pkgs: List[O2JEventPackage], init_bpm: float) -> O2JMap:
-        """Reads a level/map package and returns a O2JMap
-
-        Args:
-            pkgs: Packages read to be parsed
-            init_bpm: Initial bpm for the map from the metadata
-        """
-
-        """
-        We get unique measures from notes then find the offsets via bpm:
-        
-        We drop them into the events_note_dict:
-        { 10: 300, 12: 5000 }
-
-        Then we loop through the notes to obtain the correct offsets.
-
-        We do this because we don't want to separate and pair the LNs again 
-        since we have to go through this algorithm by a sorted offset.
-        """
-        events = [event for pkg in pkgs for event in pkg.events]
-        events.sort(key=lambda x: x.measure)
-
-        notes = [e for e in events if not isinstance(e, O2JBpm)]
-        note_measures = {note.measure for note in notes} | \
-                        {note.tail_measure for note in notes if
-                         isinstance(note, O2JHold)}
-        note_measures = sorted(note_measures)
-        note_measure_dict = {}
-
-        bpms = [e for e in events if isinstance(e, O2JBpm)]
-
-        offset = 0
-        measure = 0
-        bpm_ix = -1
-        bpm_val = init_bpm
-
-        next_bpm_measure = bpms[0].measure if len(bpms) > 0 else None
-        for note_measure in note_measures:
-            if not next_bpm_measure:
-
-                while note_measure > next_bpm_measure:
-                    bpm_ix += 1
-                    bpm = bpms[bpm_ix]
-                    # Update offset
-                    offset += RAConst.min_to_msec(
-                        (bpm.measure - measure) * 4 / bpm_val
-                    )
-                    bpm.offset = offset
-                    measure = bpm.measure
-                    bpm_val = bpm.bpm
-
-                    # Check if next one is available
-                    if bpm_ix + 1 == len(bpms):
-                        next_bpm_measure = None
-                        break
-                    else:
-                        next_bpm_measure = bpm.measure
-
-            # We add it into the measure: offset dictionary.
-            note_measure_dict[note_measure] = \
-                offset + \
-                RAConst.min_to_msec(4 * (note_measure - measure) / bpm_val)
-
-        # We then assign all the offsets here
-        for note in notes:
-            note.offset = note_measure_dict[note.measure]
-            if isinstance(note, O2JHold):  # Special case for LN.
-                note.length = note_measure_dict[note.tail_measure] - \
-                              note.offset
-
-        # We add the missing first BPM here
-        bpms.insert(0, O2JBpm(offset=0, bpm=init_bpm))
-        m = O2JMap()
-        m.hits = O2JHitList([n for n in notes if isinstance(n, O2JHit)])
-        m.holds = O2JHoldList([n for n in notes if isinstance(n, O2JHold)])
-        m.bpms = O2JBpmList(bpms)
-        return m
-
-    # noinspection PyMethodOverriding
-    # Class requires set to operate
-    def metadata(self, s: O2JMapSet, unicode=True) -> str:
-        """Grabs the map metadata
-
-        Notes:
-            This doesn't try to convert unicode to ascii.
-
-        Args:
-            s: The Map Set Object, required for additional metadata info.
-            unicode: Whether to use unicode if available.
-
-        Returns:
-            A string containing the metadata
-        """
-
-        fmt = "{} - {}, {} ({})"
-
-        try:
-            return fmt.format(s.artist.strip(), s.title,
-                              f"Level {s.level_name(self)}", s.creator)
-        except IndexError:
-            return fmt.format(s.artist, s.title, "Cannot determine level",
-                              s.creator)
-
-    # noinspection PyMethodOverriding
-    def describe(self, s: O2JMapSet, rounding: int = 2,
-                 unicode: bool = False) -> str:
-        """Describes the map's attributes as a short summary
-
-        Args:
-            s: The Map Set Object, required for additional metadata info.
-            rounding: The decimal rounding
-            unicode: Whether to attempt to get the non-unicode or unicode.
-                Doesn't attempt to translate.
-        """
-        return super().describe(rounding=rounding, unicode=unicode, s=s)
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import List, Dict, TYPE_CHECKING
+
+from reamber.base.Map import Map
+from reamber.base.Property import map_props
+from reamber.base.RAConst import RAConst
+from reamber.base.lists import TimedList
+from reamber.o2jam.O2JBpm import O2JBpm
+from reamber.o2jam.O2JEventPackage import O2JEventPackage
+from reamber.o2jam.O2JHit import O2JHit
+from reamber.o2jam.O2JHold import O2JHold
+from reamber.o2jam.lists.O2JBpmList import O2JBpmList
+from reamber.o2jam.lists.notes import O2JNoteList
+from reamber.o2jam.lists.notes.O2JHitList import O2JHitList
+from reamber.o2jam.lists.notes.O2JHoldList import O2JHoldList
+
+if TYPE_CHECKING:
+    from reamber.o2jam.O2JMapSet import O2JMapSet
+
+import logging
+
+log = logging.getLogger(__name__)
+
+
+@map_props()
+@dataclass
+class O2JMap(Map[O2JNoteList, O2JHitList, O2JHoldList, O2JBpmList]):
+    """This holds a single level of a .ojn file out of a total of three.
+
+    This class only holds the data of notes and bpms. The rest can be found in
+    the parent O2JMapSet instance.
+
+    We won't support OJM, see why in O2JMapSet. """
+
+    objs: Dict[str, TimedList] = \
+        field(init=False,
+              default_factory=lambda: dict(hits=O2JHitList([]),
+                                           holds=O2JHoldList([]),
+                                           bpms=O2JBpmList([])))
+
+    # noinspection PyUnresolvedReferences
+    @staticmethod
+    def read_pkgs(pkgs: List[O2JEventPackage], init_bpm: float) -> O2JMap:
+        """Reads a level/map package and returns a O2JMap
+
+        Args:
+            pkgs: Packages read to be parsed
+            init_bpm: Initial bpm for the map from the metadata
+        """
+
+        """
+        We get unique measures from notes then find the offsets via bpm:
+        
+        We drop them into the events_note_dict:
+        { 10: 300, 12: 5000 }
+
+        Then we loop through the notes to obtain the correct offsets.
+
+        We do this because we don't want to separate and pair the LNs again 
+        since we have to go through this algorithm by a sorted offset.
+        """
+        events = [event for pkg in pkgs for event in pkg.events]
+        events.sort(key=lambda x: x.measure)
+
+        notes = [e for e in events if not isinstance(e, O2JBpm)]
+        note_measures = {note.measure for note in notes} | \
+                        {note.tail_measure for note in notes if
+                         isinstance(note, O2JHold)}
+        note_measures = sorted(note_measures)
+        note_measure_dict = {}
+
+        bpms = [e for e in events if isinstance(e, O2JBpm)]
+
+        offset = 0
+        measure = 0
+        bpm_ix = -1
+        bpm_val = init_bpm
+
+        next_bpm_measure = bpms[0].measure if len(bpms) > 0 else None
+        for note_measure in note_measures:
+            if not next_bpm_measure:
+
+                while note_measure > next_bpm_measure:
+                    bpm_ix += 1
+                    bpm = bpms[bpm_ix]
+                    # Update offset
+                    offset += RAConst.min_to_msec(
+                        (bpm.measure - measure) * 4 / bpm_val
+                    )
+                    bpm.offset = offset
+                    measure = bpm.measure
+                    bpm_val = bpm.bpm
+
+                    # Check if next one is available
+                    if bpm_ix + 1 == len(bpms):
+                        next_bpm_measure = None
+                        break
+                    else:
+                        next_bpm_measure = bpm.measure
+
+            # We add it into the measure: offset dictionary.
+            note_measure_dict[note_measure] = \
+                offset + \
+                RAConst.min_to_msec(4 * (note_measure - measure) / bpm_val)
+
+        # We then assign all the offsets here
+        for note in notes:
+            note.offset = note_measure_dict[note.measure]
+            if isinstance(note, O2JHold):  # Special case for LN.
+                note.length = note_measure_dict[note.tail_measure] - \
+                              note.offset
+
+        # We add the missing first BPM here
+        bpms.insert(0, O2JBpm(offset=0, bpm=init_bpm))
+        m = O2JMap()
+        m.hits = O2JHitList([n for n in notes if isinstance(n, O2JHit)])
+        m.holds = O2JHoldList([n for n in notes if isinstance(n, O2JHold)])
+        m.bpms = O2JBpmList(bpms)
+        return m
+
+    # noinspection PyMethodOverriding
+    # Class requires set to operate
+    def metadata(self, s: O2JMapSet, unicode=True) -> str:
+        """Grabs the map metadata
+
+        Notes:
+            This doesn't try to convert unicode to ascii.
+
+        Args:
+            s: The Map Set Object, required for additional metadata info.
+            unicode: Whether to use unicode if available.
+
+        Returns:
+            A string containing the metadata
+        """
+
+        fmt = "{} - {}, {} ({})"
+
+        try:
+            return fmt.format(s.artist.strip(), s.title,
+                              f"Level {s.level_name(self)}", s.creator)
+        except IndexError:
+            return fmt.format(s.artist, s.title, "Cannot determine level",
+                              s.creator)
+
+    # noinspection PyMethodOverriding
+    def describe(self, s: O2JMapSet, rounding: int = 2,
+                 unicode: bool = False) -> str:
+        """Describes the map's attributes as a short summary
+
+        Args:
+            s: The Map Set Object, required for additional metadata info.
+            rounding: The decimal rounding
+            unicode: Whether to attempt to get the non-unicode or unicode.
+                Doesn't attempt to translate.
+        """
+        return super().describe(rounding=rounding, unicode=unicode, s=s)
```

### Comparing `reamber-0.1.7/reamber/o2jam/O2JMap.pyi` & `reamber-0.1.8/reamber/o2jam/O2JMap.pyi`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import List, Dict, TYPE_CHECKING
-
-from reamber.base.Map import Map
-from reamber.base.lists import TimedList
-from reamber.o2jam.O2JEventPackage import O2JEventPackage
-from reamber.o2jam.lists.O2JBpmList import O2JBpmList
-from reamber.o2jam.lists.notes import O2JNoteList
-from reamber.o2jam.lists.notes.O2JHitList import O2JHitList
-from reamber.o2jam.lists.notes.O2JHoldList import O2JHoldList
-
-if TYPE_CHECKING:
-    from reamber.o2jam.O2JMapSet import O2JMapSet
-
-import logging
-
-log = logging.getLogger(__name__)
-
-
-@dataclass
-class O2JMap(Map[O2JNoteList, O2JHitList, O2JHoldList, O2JBpmList]):
-    """This holds a single level of a .ojn file out of a total of three.
-
-    This class only holds the data of notes and bpms. The rest can be found in the parent O2JMapSet instance.
-
-    We won't support OJM, see why in O2JMapSet. """
-
-    objs: Dict[str, TimedList] = \
-        field(init=False,
-              default_factory=lambda: dict(hits=O2JHitList([]),
-                                           holds=O2JHoldList([]),
-                                           bpms=O2JBpmList([])))
-
-    @staticmethod
-    def read_pkgs(pkgs: List[O2JEventPackage], init_bpm: float) -> O2JMap: ...
-
-    # noinspection PyMethodOverriding
-    def metadata(self, s: O2JMapSet, unicode=True, **kwargs) -> str: ...
-
-    # noinspection PyMethodOverriding
-    def describe(self, s: O2JMapSet, rounding: int = 2,
-                 unicode: bool = False) -> str: ...
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import List, Dict, TYPE_CHECKING
+
+from reamber.base.Map import Map
+from reamber.base.lists import TimedList
+from reamber.o2jam.O2JEventPackage import O2JEventPackage
+from reamber.o2jam.lists.O2JBpmList import O2JBpmList
+from reamber.o2jam.lists.notes import O2JNoteList
+from reamber.o2jam.lists.notes.O2JHitList import O2JHitList
+from reamber.o2jam.lists.notes.O2JHoldList import O2JHoldList
+
+if TYPE_CHECKING:
+    from reamber.o2jam.O2JMapSet import O2JMapSet
+
+import logging
+
+log = logging.getLogger(__name__)
+
+
+@dataclass
+class O2JMap(Map[O2JNoteList, O2JHitList, O2JHoldList, O2JBpmList]):
+    """This holds a single level of a .ojn file out of a total of three.
+
+    This class only holds the data of notes and bpms. The rest can be found in the parent O2JMapSet instance.
+
+    We won't support OJM, see why in O2JMapSet. """
+
+    objs: Dict[str, TimedList] = \
+        field(init=False,
+              default_factory=lambda: dict(hits=O2JHitList([]),
+                                           holds=O2JHoldList([]),
+                                           bpms=O2JBpmList([])))
+
+    @staticmethod
+    def read_pkgs(pkgs: List[O2JEventPackage], init_bpm: float) -> O2JMap: ...
+
+    # noinspection PyMethodOverriding
+    def metadata(self, s: O2JMapSet, unicode=True, **kwargs) -> str: ...
+
+    # noinspection PyMethodOverriding
+    def describe(self, s: O2JMapSet, rounding: int = 2,
+                 unicode: bool = False) -> str: ...
```

### Comparing `reamber-0.1.7/reamber/o2jam/O2JMapSet.pyi` & `reamber-0.1.8/reamber/o2jam/O2JMapSet.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,34 @@
-from __future__ import annotations
-
-import logging
-from dataclasses import dataclass
-from typing import Iterator, List
-
-from reamber.base.MapSet import MapSet
-from reamber.o2jam.O2JMap import O2JMap
-from reamber.o2jam.O2JMapSetMeta import O2JMapSetMeta
-from reamber.o2jam.lists.O2JBpmList import O2JBpmList
-from reamber.o2jam.lists.notes import O2JHitList
-from reamber.o2jam.lists.notes.O2JHoldList import O2JHoldList
-from reamber.o2jam.lists.notes.O2JNoteList import O2JNoteList
-
-log = logging.getLogger(__name__)
-
-
-@dataclass
-class O2JMapSet(MapSet[O2JNoteList, O2JHitList,
-                       O2JHoldList, O2JBpmList, O2JMap], O2JMapSetMeta):
-    def __iter__(self) -> Iterator[O2JMap]: ...
-
-    def level_name(self, o2j: O2JMap) -> int: ...
-
-    @staticmethod
-    def read(b: bytes) -> O2JMapSet: ...
-
-    @staticmethod
-    def read_file(file_path: str) -> O2JMapSet: ...
-
-    class Stacker(MapSet.Stacker): ...
-
-    def stack(self, include: List[str] = None) -> Stacker: ...
+from __future__ import annotations
+
+import logging
+from dataclasses import dataclass
+from pathlib import Path
+from typing import Iterator, List
+
+from reamber.base.MapSet import MapSet
+from reamber.o2jam.O2JMap import O2JMap
+from reamber.o2jam.O2JMapSetMeta import O2JMapSetMeta
+from reamber.o2jam.lists.O2JBpmList import O2JBpmList
+from reamber.o2jam.lists.notes import O2JHitList
+from reamber.o2jam.lists.notes.O2JHoldList import O2JHoldList
+from reamber.o2jam.lists.notes.O2JNoteList import O2JNoteList
+
+log = logging.getLogger(__name__)
+
+
+@dataclass
+class O2JMapSet(MapSet[O2JNoteList, O2JHitList,
+                       O2JHoldList, O2JBpmList, O2JMap], O2JMapSetMeta):
+    def __iter__(self) -> Iterator[O2JMap]: ...
+
+    def level_name(self, o2j: O2JMap) -> int: ...
+
+    @staticmethod
+    def read(b: bytes) -> O2JMapSet: ...
+
+    @staticmethod
+    def read_file(file_path: str | Path) -> O2JMapSet: ...
+
+    class Stacker(MapSet.Stacker): ...
+
+    def stack(self, include: List[str] = None) -> Stacker: ...
```

### Comparing `reamber-0.1.7/reamber/o2jam/O2JMapSetMeta.py` & `reamber-0.1.8/reamber/o2jam/O2JMapSetMeta.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-"""This holds the metadata for the O2Jam Map Set
-
-Directly inherited by O2JMapSet to allow access to all the extra metadata
-"""
-
-import struct
-from dataclasses import dataclass, field
-from typing import List
-
-
-class O2JMapGenre:
-    """This is a class of static variables that indicate the genre of the song"""
-    BALLAD: int = 0
-    ROCK: int = 1
-    DANCE: int = 2
-    TECHNO: int = 3
-    HIP_HOP: int = 4
-    SOUL_R_B: int = 5
-    JAZZ: int = 6
-    FUNK: int = 7
-    CLASSICAL: int = 8
-    TRADITIONAL: int = 9
-    ETC: int = 10
-
-
-@dataclass
-class O2JMapSetMeta:
-    """This class contains the readable metadata of the map
-
-    This can be extracted from the first 300 bytes of every ojn file."""
-
-    #                                                             # FORMAT
-    song_id: int = 0  # INT
-    signature: str = ""  # CHAR[4]
-    encode_version: float = 0.0  # FLOAT
-    genre: int = 0  # INT
-    bpm: float = 0.0  # FLOAT
-    level: List[int] = field(default_factory=list)  # SHORT[4]
-    event_count: List[int] = field(default_factory=list)  # INT[3]
-    note_count: List[int] = field(default_factory=list)  # INT[3]
-    measure_count: List[int] = field(default_factory=list)  # INT[3]
-    package_count: List[int] = field(default_factory=list)  # INT[3]
-    old_encode_version: int = 0  # SHORT
-    old_song_id: int = 0  # SHORT
-    old_genre: bytes = b""  # CHAR[20]
-    bmp_size: int = 0  # INT
-    old_file_version: int = 0  # INT
-    title: str = ""  # CHAR[64]
-    artist: str = ""  # CHAR[32]
-    creator: str = ""  # CHAR[32]
-    ojm_file: str = ""  # CHAR[32]
-    cover_size: int = 0  # INT
-    duration: List[int] = field(default_factory=list)  # INT[3]
-    note_offset: List[int] = field(default_factory=list)  # INT[3]
-    cover_offset: int = 0  # INT
-
-    BYTE_COUNT = [1, 4, 1, 1, 1, 4, 3, 3, 3, 3, 1, 1, 20, 1, 1, 64, 32, 32, 32,
-                  1, 3, 3, 1]
-    BYTE_SIZES = [4, 4, 4, 4, 4, 8, 12, 12, 12, 12, 2, 2, 20, 4, 4, 64, 32, 32,
-                  32, 4, 12, 12, 4]
-    BYTE_FORMATS = ["i", "s", "f", "i", "f", "h", "i", "i", "i", "i", "h", "h",
-                    "s", "i", "i", "s", "s", "s", "s", "i", "i", "i", "i"]
-
-    def read_meta(self, metadata: bytes):
-        """Reads the metadata of the map
-
-        Args:
-            metadata: The first 300 bytes go here
-        """
-        meta_fields: List = []
-        ix_start = 0
-        for fmt, size, count in zip(O2JMapSetMeta.BYTE_FORMATS,
-                                    O2JMapSetMeta.BYTE_SIZES,
-                                    O2JMapSetMeta.BYTE_COUNT):
-            meta_field = []
-            fmt_size = int(size / count)
-            for _ in range(count):
-                meta_field.append(
-                    struct.unpack("<" + fmt,
-                                  metadata[ix_start:ix_start + fmt_size])[0]
-                )
-                ix_start += fmt_size
-            meta_fields.append(meta_field)
-
-        def decode_replace(b: bytes):
-            return (b"".join(filter(lambda x: x != b'\x00', b))
-                    .decode("ascii", errors='ignore'))
-
-        self.song_id = meta_fields[0][0]
-        self.signature = decode_replace(meta_fields[1])
-        self.encode_version = meta_fields[2][0]
-        self.genre = meta_fields[3][0]
-        self.bpm = meta_fields[4][0]
-        self.level = meta_fields[5]
-        self.event_count = meta_fields[6]
-        self.note_count = meta_fields[7]
-        self.measure_count = meta_fields[8]
-        self.package_count = meta_fields[9]
-        self.old_encode_version = meta_fields[10][0]
-        self.old_song_id = meta_fields[11][0]
-        self.old_genre = b"".join(meta_fields[12])
-        self.bmp_size = meta_fields[13][0]
-        self.old_file_version = meta_fields[14][0]
-        self.title = decode_replace(meta_fields[15])
-        self.artist = decode_replace(meta_fields[16])
-        self.creator = decode_replace(meta_fields[17])
-        self.ojm_file = decode_replace(meta_fields[18])
-        self.cover_size = meta_fields[19][0]
-        self.duration = meta_fields[20]
-        self.note_offset = meta_fields[21]
-        self.cover_offset = meta_fields[22][0]
-
-    def write_meta(self, f) -> bytes:
-        """Unimplemented, writes the metadata of a ojn file
-
-        I don't think I'll implement this unless there's clear support on this
-        """
-        pass
-        # need to verify all byte sizes on export
-        # f.write(struct.pack("<i", self.songId                            ))
-        # f.write(bytes(self.signature, encoding='ascii'                   ))
-        # f.write(struct.pack("<f", self.encodeVersion                     ))
-        # f.write(struct.pack("<i", self.genre                             ))
-        # f.write(struct.pack("<f", self.bpm                               ))
-        # for level in self.level:
-        #     f.write(struct.pack("<h", level                              ))
-        # for eventCount in self.eventCount:
-        #     f.write(struct.pack("<i", eventCount                         ))
-        # for noteCount in self.noteCount:
-        #     f.write(struct.pack("<i", noteCount                          ))
-        # for measureCount in self.measureCount:
-        #     f.write(struct.pack("<i", measureCount                       ))
-        # for packageCount in self.packageCount:
-        #     f.write(struct.pack("<i", packageCount                       ))
-        # f.write(struct.pack("<h", self.oldEncodeVersion                  ))
-        # f.write(struct.pack("<h", self.oldSongId                         ))
-        # f.write(self.oldGenre                                             )
-        # f.write(struct.pack("<i", self.bmpSize                           ))
-        # f.write(struct.pack("<i", self.oldFileVersion                    ))
-        # # TO#DO: Need to verify length. Fly Magpie is 63, expect 64 bytes
-        # f.write(bytes(self.title, encoding='ascii')                       )
-        # f.write(struct.pack("<s", bytes(self.artist, encoding='ascii')   ))
-        # f.write(struct.pack("<s", bytes(self.creator, encoding='ascii')  ))
-        # f.write(struct.pack("<s", bytes(self.ojmFile, encoding='ascii')  ))
-        # f.write(struct.pack("<i", self.coverSize                         ))
-        # for duration in self.duration:
-        #     f.write(struct.pack("<i", self.duration                      ))
-        # for noteOffset in self.noteOffset:
-        #     f.write(struct.pack("<i", noteOffset                         ))
-        # f.write(struct.pack("<i", self.coverOffset                       ))
+"""This holds the metadata for the O2Jam Map Set
+
+Directly inherited by O2JMapSet to allow access to all the extra metadata
+"""
+
+import struct
+from dataclasses import dataclass, field
+from typing import List
+
+
+class O2JMapGenre:
+    """This is a class of static variables that indicate the genre of the song"""
+    BALLAD: int = 0
+    ROCK: int = 1
+    DANCE: int = 2
+    TECHNO: int = 3
+    HIP_HOP: int = 4
+    SOUL_R_B: int = 5
+    JAZZ: int = 6
+    FUNK: int = 7
+    CLASSICAL: int = 8
+    TRADITIONAL: int = 9
+    ETC: int = 10
+
+
+@dataclass
+class O2JMapSetMeta:
+    """This class contains the readable metadata of the map
+
+    This can be extracted from the first 300 bytes of every ojn file."""
+
+    #                                                             # FORMAT
+    song_id: int = 0  # INT
+    signature: str = ""  # CHAR[4]
+    encode_version: float = 0.0  # FLOAT
+    genre: int = 0  # INT
+    bpm: float = 0.0  # FLOAT
+    level: List[int] = field(default_factory=list)  # SHORT[4]
+    event_count: List[int] = field(default_factory=list)  # INT[3]
+    note_count: List[int] = field(default_factory=list)  # INT[3]
+    measure_count: List[int] = field(default_factory=list)  # INT[3]
+    package_count: List[int] = field(default_factory=list)  # INT[3]
+    old_encode_version: int = 0  # SHORT
+    old_song_id: int = 0  # SHORT
+    old_genre: bytes = b""  # CHAR[20]
+    bmp_size: int = 0  # INT
+    old_file_version: int = 0  # INT
+    title: str = ""  # CHAR[64]
+    artist: str = ""  # CHAR[32]
+    creator: str = ""  # CHAR[32]
+    ojm_file: str = ""  # CHAR[32]
+    cover_size: int = 0  # INT
+    duration: List[int] = field(default_factory=list)  # INT[3]
+    note_offset: List[int] = field(default_factory=list)  # INT[3]
+    cover_offset: int = 0  # INT
+
+    BYTE_COUNT = [1, 4, 1, 1, 1, 4, 3, 3, 3, 3, 1, 1, 20, 1, 1, 64, 32, 32, 32,
+                  1, 3, 3, 1]
+    BYTE_SIZES = [4, 4, 4, 4, 4, 8, 12, 12, 12, 12, 2, 2, 20, 4, 4, 64, 32, 32,
+                  32, 4, 12, 12, 4]
+    BYTE_FORMATS = ["i", "s", "f", "i", "f", "h", "i", "i", "i", "i", "h", "h",
+                    "s", "i", "i", "s", "s", "s", "s", "i", "i", "i", "i"]
+
+    def read_meta(self, metadata: bytes):
+        """Reads the metadata of the map
+
+        Args:
+            metadata: The first 300 bytes go here
+        """
+        meta_fields: List = []
+        ix_start = 0
+        for fmt, size, count in zip(O2JMapSetMeta.BYTE_FORMATS,
+                                    O2JMapSetMeta.BYTE_SIZES,
+                                    O2JMapSetMeta.BYTE_COUNT):
+            meta_field = []
+            fmt_size = int(size / count)
+            for _ in range(count):
+                meta_field.append(
+                    struct.unpack("<" + fmt,
+                                  metadata[ix_start:ix_start + fmt_size])[0]
+                )
+                ix_start += fmt_size
+            meta_fields.append(meta_field)
+
+        def decode_replace(b: bytes):
+            return (b"".join(filter(lambda x: x != b'\x00', b))
+                    .decode("ascii", errors='ignore'))
+
+        self.song_id = meta_fields[0][0]
+        self.signature = decode_replace(meta_fields[1])
+        self.encode_version = meta_fields[2][0]
+        self.genre = meta_fields[3][0]
+        self.bpm = meta_fields[4][0]
+        self.level = meta_fields[5]
+        self.event_count = meta_fields[6]
+        self.note_count = meta_fields[7]
+        self.measure_count = meta_fields[8]
+        self.package_count = meta_fields[9]
+        self.old_encode_version = meta_fields[10][0]
+        self.old_song_id = meta_fields[11][0]
+        self.old_genre = b"".join(meta_fields[12])
+        self.bmp_size = meta_fields[13][0]
+        self.old_file_version = meta_fields[14][0]
+        self.title = decode_replace(meta_fields[15])
+        self.artist = decode_replace(meta_fields[16])
+        self.creator = decode_replace(meta_fields[17])
+        self.ojm_file = decode_replace(meta_fields[18])
+        self.cover_size = meta_fields[19][0]
+        self.duration = meta_fields[20]
+        self.note_offset = meta_fields[21]
+        self.cover_offset = meta_fields[22][0]
+
+    def write_meta(self, f) -> bytes:
+        """Unimplemented, writes the metadata of a ojn file
+
+        I don't think I'll implement this unless there's clear support on this
+        """
+        pass
+        # need to verify all byte sizes on export
+        # f.write(struct.pack("<i", self.songId                            ))
+        # f.write(bytes(self.signature, encoding='ascii'                   ))
+        # f.write(struct.pack("<f", self.encodeVersion                     ))
+        # f.write(struct.pack("<i", self.genre                             ))
+        # f.write(struct.pack("<f", self.bpm                               ))
+        # for level in self.level:
+        #     f.write(struct.pack("<h", level                              ))
+        # for eventCount in self.eventCount:
+        #     f.write(struct.pack("<i", eventCount                         ))
+        # for noteCount in self.noteCount:
+        #     f.write(struct.pack("<i", noteCount                          ))
+        # for measureCount in self.measureCount:
+        #     f.write(struct.pack("<i", measureCount                       ))
+        # for packageCount in self.packageCount:
+        #     f.write(struct.pack("<i", packageCount                       ))
+        # f.write(struct.pack("<h", self.oldEncodeVersion                  ))
+        # f.write(struct.pack("<h", self.oldSongId                         ))
+        # f.write(self.oldGenre                                             )
+        # f.write(struct.pack("<i", self.bmpSize                           ))
+        # f.write(struct.pack("<i", self.oldFileVersion                    ))
+        # # TO#DO: Need to verify length. Fly Magpie is 63, expect 64 bytes
+        # f.write(bytes(self.title, encoding='ascii')                       )
+        # f.write(struct.pack("<s", bytes(self.artist, encoding='ascii')   ))
+        # f.write(struct.pack("<s", bytes(self.creator, encoding='ascii')  ))
+        # f.write(struct.pack("<s", bytes(self.ojmFile, encoding='ascii')  ))
+        # f.write(struct.pack("<i", self.coverSize                         ))
+        # for duration in self.duration:
+        #     f.write(struct.pack("<i", self.duration                      ))
+        # for noteOffset in self.noteOffset:
+        #     f.write(struct.pack("<i", noteOffset                         ))
+        # f.write(struct.pack("<i", self.coverOffset                       ))
```

### Comparing `reamber-0.1.7/reamber/osu/OsuBpm.py` & `reamber-0.1.8/reamber/osu/OsuBpm.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-from __future__ import annotations
-
-from reamber.base import item_props
-from reamber.base.Bpm import Bpm
-from reamber.osu.OsuSampleSet import OsuSampleSet
-from reamber.osu.OsuTimingPointMeta import OsuTimingPointMeta
-
-
-@item_props()
-class OsuBpm(OsuTimingPointMeta, Bpm):
-
-    def __init__(self,
-                 offset: float,
-                 bpm: float,
-                 metronome: int = 4,
-                 sample_set: int = OsuSampleSet.AUTO,
-                 sample_set_index: int = 0,
-                 volume: int = 50,
-                 kiai: bool = False,
-                 **kwargs):
-        super().__init__(
-            offset=offset, bpm=bpm, metronome=metronome, sample_set=sample_set,
-            sample_set_index=sample_set_index, volume=volume, kiai=kiai,
-            **kwargs
-        )
-
-    @staticmethod
-    def code_to_value(code: float) -> float:
-        """Converts .osu format to actual Bpm"""
-        try:
-            return 60000.0 / code
-        except ZeroDivisionError:
-            raise ZeroDivisionError("BPM cannot be infinite.")
-
-    @staticmethod
-    def value_to_code(value: float) -> float:
-        """Converts actual Bpm .osu format"""
-        try:
-            return 60000.0 / value
-        except ZeroDivisionError:
-            raise ZeroDivisionError("BPM cannot be exactly 0.")
-
-    @staticmethod
-    def read_string(s: str, as_dict: bool = False) -> OsuBpm:
-        """Reads a single line under the [TimingPoints] Label. """
-        if not OsuTimingPointMeta.is_timing_point(s):
-            raise ValueError(f"Bad OsuBpm format: {s}")
-
-        s_comma = s.split(",")
-        d = dict(offset=float(s_comma[0]),
-                 bpm=OsuBpm.code_to_value(float(s_comma[1])),
-                 metronome=int(s_comma[2]),
-                 sample_set=int(s_comma[3]),
-                 sample_set_index=int(s_comma[4]),
-                 volume=int(s_comma[5]),
-                 kiai=bool(int(s_comma[7])))
-        return d if as_dict else OsuBpm(**d)
-    def write_string(self) -> str:
-        """Writes a .osu writable string"""
-
-        return f"{self.offset}," \
-               f"{self.value_to_code(self.bpm)}," \
-               f"{int(self.metronome)}," \
-               f"{int(self.sample_set)}," \
-               f"{int(self.sample_set_index)}," \
-               f"{int(self.volume)}," \
-               f"{1}," \
-               f"{int(self.kiai)}"
+from __future__ import annotations
+
+from reamber.base import item_props
+from reamber.base.Bpm import Bpm
+from reamber.osu.OsuSampleSet import OsuSampleSet
+from reamber.osu.OsuTimingPointMeta import OsuTimingPointMeta
+
+
+@item_props()
+class OsuBpm(OsuTimingPointMeta, Bpm):
+
+    def __init__(self,
+                 offset: float,
+                 bpm: float,
+                 metronome: int = 4,
+                 sample_set: int = OsuSampleSet.AUTO,
+                 sample_set_index: int = 0,
+                 volume: int = 50,
+                 kiai: bool = False,
+                 **kwargs):
+        super().__init__(
+            offset=offset, bpm=bpm, metronome=metronome, sample_set=sample_set,
+            sample_set_index=sample_set_index, volume=volume, kiai=kiai,
+            **kwargs
+        )
+
+    @staticmethod
+    def code_to_value(code: float) -> float:
+        """Converts .osu format to actual Bpm"""
+        try:
+            return 60000.0 / code
+        except ZeroDivisionError:
+            raise ZeroDivisionError("BPM cannot be infinite.")
+
+    @staticmethod
+    def value_to_code(value: float) -> float:
+        """Converts actual Bpm .osu format"""
+        try:
+            return 60000.0 / value
+        except ZeroDivisionError:
+            raise ZeroDivisionError("BPM cannot be exactly 0.")
+
+    @staticmethod
+    def read_string(s: str, as_dict: bool = False) -> OsuBpm:
+        """Reads a single line under the [TimingPoints] Label. """
+        if not OsuTimingPointMeta.is_timing_point(s):
+            raise ValueError(f"Bad OsuBpm format: {s}")
+
+        s_comma = s.split(",")
+        d = dict(offset=float(s_comma[0]),
+                 bpm=OsuBpm.code_to_value(float(s_comma[1])),
+                 metronome=int(s_comma[2]),
+                 sample_set=int(s_comma[3]),
+                 sample_set_index=int(s_comma[4]),
+                 volume=int(s_comma[5]),
+                 kiai=bool(int(s_comma[7])))
+        return d if as_dict else OsuBpm(**d)
+    def write_string(self) -> str:
+        """Writes a .osu writable string"""
+
+        return f"{self.offset}," \
+               f"{self.value_to_code(self.bpm)}," \
+               f"{int(self.metronome)}," \
+               f"{int(self.sample_set)}," \
+               f"{int(self.sample_set_index)}," \
+               f"{int(self.volume)}," \
+               f"{1}," \
+               f"{int(self.kiai)}"
```

### Comparing `reamber-0.1.7/reamber/osu/OsuBpm.pyi` & `reamber-0.1.8/reamber/osu/OsuSv.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,42 @@
-from __future__ import annotations
-
-from typing import overload, Dict
-
-from reamber.base.Bpm import Bpm
-from reamber.osu.OsuSampleSet import OsuSampleSet
-from reamber.osu.OsuTimingPointMeta import OsuTimingPointMeta
-
-
-class OsuBpm(OsuTimingPointMeta, Bpm):
-
-    def __init__(self, offset: float, bpm: float, metronome: int = 4,
-                 sample_set: int = OsuSampleSet.AUTO,
-                 sample_set_index: int = 0, volume: int = 50,
-                 kiai: bool = False, **kwargs): ...
-
-    @staticmethod
-    def code_to_value(code: float) -> float: ...
-
-    @staticmethod
-    def value_to_code(value: float) -> float: ...
-
-    @staticmethod
-    @overload
-    def read_string(s: str, as_dict: bool = False) -> OsuBpm: ...
-
-    @staticmethod
-    @overload
-    def read_string(s: str, as_dict: bool = True) -> Dict[str]: ...
-
-    @staticmethod
-    def read_string(s: str, as_dict: bool = True) -> OsuBpm or Dict[str]: ...
-
-    def write_string(self) -> str: ...
+from __future__ import annotations
+
+from typing import overload, Dict
+
+import pandas as pd
+
+from reamber.base.Timed import Timed
+from reamber.osu.OsuSampleSet import OsuSampleSet
+from reamber.osu.OsuTimingPointMeta import OsuTimingPointMeta
+
+
+class OsuSv(OsuTimingPointMeta, Timed):
+
+    def __init__(self, offset: float, multiplier: float = 1.0,
+                 metronome: int = 4, sample_set: int = OsuSampleSet.AUTO,
+                 sample_set_index: int = 0, volume: int = 50,
+                 kiai: bool = False, **kwargs): ...
+
+    @staticmethod
+    def code_to_value(code: float) -> float: ...
+
+    @staticmethod
+    def value_to_code(value: float) -> float: ...
+
+    @staticmethod
+    @overload
+    def read_string(s: str, as_dict: bool = False) -> OsuSv: ...
+
+    @staticmethod
+    @overload
+    def read_string(s: str, as_dict: bool = True) -> Dict[str]: ...
+
+    @staticmethod
+    def read_string(s: str, as_dict: bool = True) -> OsuSv or Dict[str]: ...
+
+    def write_string(self) -> str: ...
+
+    @property
+    def multiplier(self) -> pd.Series: ...
+
+    @multiplier.setter
+    def multiplier(self, val) -> None: ...
```

### Comparing `reamber-0.1.7/reamber/osu/OsuHit.py` & `reamber-0.1.8/reamber/osu/OsuHold.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-from __future__ import annotations
-
-from reamber.base import item_props
-from reamber.base.Hit import Hit
-from reamber.osu.OsuNoteMeta import OsuNoteMeta
-from reamber.osu.OsuSampleSet import OsuSampleSet
-
-
-@item_props()
-class OsuHit(Hit, OsuNoteMeta):
-
-    def __init__(self,
-                 offset: float,
-                 column: int,
-                 hitsound_set: int = OsuSampleSet.AUTO,
-                 sample_set: int = OsuSampleSet.AUTO,
-                 addition_set: int = OsuSampleSet.AUTO,
-                 custom_set: int = 0,
-                 volume: int = 0,
-                 hitsound_file: str = "",
-                 **kwargs):
-        super().__init__(
-            offset=offset, column=column, hitsound_set=hitsound_set,
-            sample_set=sample_set, addition_set=addition_set,
-            custom_set=custom_set, volume=volume,
-            hitsound_file=hitsound_file, **kwargs
-        )
-
-    @staticmethod
-    def read_string(s: str, keys: int, as_dict: bool = False) -> OsuHit:
-        """Reads a single line under the [HitObject] Label"""
-
-        if not OsuNoteMeta.is_hit(s):
-            raise ValueError(f"Bad OsuHit Format. {s}")
-
-        s_comma = s.split(",")
-        s_colon = s_comma[-1].split(":")
-
-        d = dict(
-            offset=float(s_comma[2]),
-            column=OsuNoteMeta.x_axis_to_column(int(s_comma[0]), keys),
-            hitsound_set=int(s_comma[4]),
-            sample_set=int(s_colon[0]),
-            addition_set=int(s_colon[1]),
-            custom_set=int(s_colon[2]),
-            volume=int(s_colon[3]),
-            hitsound_file=s_colon[4]
-        )
-        return d if as_dict else OsuHit(**d)
-
-    def write_string(self, keys: int) -> str:
-        """Exports a .osu writable string"""
-        return f"{OsuNoteMeta.column_to_x_axis(self.column, keys=keys)}," \
-               f"{192}," \
-               f"{int(self.offset)}," \
-               f"{1}," \
-               f"{int(self.hitsound_set)}," \
-               f"{int(self.sample_set)}:" \
-               f"{int(self.addition_set)}:" \
-               f"{int(self.custom_set)}:" \
-               f"{int(self.volume)}:" \
-               f"{self.hitsound_file}"
+from __future__ import annotations
+
+from reamber.base import item_props
+from reamber.base.Hold import Hold
+from reamber.osu.OsuNoteMeta import OsuNoteMeta
+from reamber.osu.OsuSampleSet import OsuSampleSet
+
+
+@item_props()
+class OsuHold(Hold, OsuNoteMeta):
+    def __init__(self,
+                 offset: float,
+                 column: int,
+                 length: float,
+                 hitsound_set: int = OsuSampleSet.AUTO,
+                 sample_set: int = OsuSampleSet.AUTO,
+                 addition_set: int = OsuSampleSet.AUTO,
+                 custom_set: int = OsuSampleSet.AUTO,
+                 volume: int = 0,
+                 hitsound_file: str = "",
+                 **kwargs):
+        super().__init__(
+            offset=offset, column=column, length=length,
+            hitsound_set=hitsound_set,
+            sample_set=sample_set, addition_set=addition_set,
+            custom_set=custom_set,
+            volume=volume, hitsound_file=hitsound_file, **kwargs
+        )
+
+    @staticmethod
+    def read_string(s: str, keys: int, as_dict: bool = False) -> OsuHold:
+        """Reads a single line under the [HitObjects] Label"""
+
+        if not OsuNoteMeta.is_hold(s):
+            raise ValueError(f"Bad OsuHold Format. {s}")
+
+        s_comma = s.split(",")
+        s_colon = s_comma[-1].split(":")
+
+        d = dict(offset=float(s_comma[2]),
+                 column=OsuNoteMeta.x_axis_to_column(int(s_comma[0]), keys),
+                 length=float(s_colon[0]) - float(s_comma[2]),
+                 hitsound_set=int(s_comma[4]),
+                 sample_set=int(s_colon[1]),
+                 addition_set=int(s_colon[2]),
+                 custom_set=int(s_colon[3]),
+                 volume=int(s_colon[4]),
+                 hitsound_file=s_colon[5])
+        return d if as_dict else OsuHold(**d)
+
+    def write_string(self, keys: int) -> str:
+        """Exports a .osu writable string"""
+        return f"{OsuNoteMeta.column_to_x_axis(self.column, keys=keys)}," \
+               f"{192}," \
+               f"{int(self.offset)}," \
+               f"{128}," \
+               f"{int(self.hitsound_set)}," \
+               f"{int(self.offset + self.length)}:" \
+               f"{int(self.sample_set)}:" \
+               f"{int(self.addition_set)}:" \
+               f"{int(self.custom_set)}:" \
+               f"{int(self.volume)}:" \
+               f"{self.hitsound_file}"
```

### Comparing `reamber-0.1.7/reamber/osu/OsuHold.py` & `reamber-0.1.8/reamber/osu/OsuHit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,62 @@
-from __future__ import annotations
-
-from reamber.base import item_props
-from reamber.base.Hold import Hold
-from reamber.osu.OsuNoteMeta import OsuNoteMeta
-from reamber.osu.OsuSampleSet import OsuSampleSet
-
-
-@item_props()
-class OsuHold(Hold, OsuNoteMeta):
-    def __init__(self,
-                 offset: float,
-                 column: int,
-                 length: float,
-                 hitsound_set: int = OsuSampleSet.AUTO,
-                 sample_set: int = OsuSampleSet.AUTO,
-                 addition_set: int = OsuSampleSet.AUTO,
-                 custom_set: int = OsuSampleSet.AUTO,
-                 volume: int = 0,
-                 hitsound_file: str = "",
-                 **kwargs):
-        super().__init__(
-            offset=offset, column=column, length=length,
-            hitsound_set=hitsound_set,
-            sample_set=sample_set, addition_set=addition_set,
-            custom_set=custom_set,
-            volume=volume, hitsound_file=hitsound_file, **kwargs
-        )
-
-    @staticmethod
-    def read_string(s: str, keys: int, as_dict: bool = False) -> OsuHold:
-        """Reads a single line under the [HitObjects] Label"""
-
-        if not OsuNoteMeta.is_hold(s):
-            raise ValueError(f"Bad OsuHold Format. {s}")
-
-        s_comma = s.split(",")
-        s_colon = s_comma[-1].split(":")
-
-        d = dict(offset=float(s_comma[2]),
-                 column=OsuNoteMeta.x_axis_to_column(int(s_comma[0]), keys),
-                 length=float(s_colon[0]) - float(s_comma[2]),
-                 hitsound_set=int(s_comma[4]),
-                 sample_set=int(s_colon[1]),
-                 addition_set=int(s_colon[2]),
-                 custom_set=int(s_colon[3]),
-                 volume=int(s_colon[4]),
-                 hitsound_file=s_colon[5])
-        return d if as_dict else OsuHold(**d)
-
-    def write_string(self, keys: int) -> str:
-        """Exports a .osu writable string"""
-        return f"{OsuNoteMeta.column_to_x_axis(self.column, keys=keys)}," \
-               f"{192}," \
-               f"{int(self.offset)}," \
-               f"{128}," \
-               f"{int(self.hitsound_set)}," \
-               f"{int(self.offset + self.length)}:" \
-               f"{int(self.sample_set)}:" \
-               f"{int(self.addition_set)}:" \
-               f"{int(self.custom_set)}:" \
-               f"{int(self.volume)}:" \
-               f"{self.hitsound_file}"
+from __future__ import annotations
+
+from reamber.base import item_props
+from reamber.base.Hit import Hit
+from reamber.osu.OsuNoteMeta import OsuNoteMeta
+from reamber.osu.OsuSampleSet import OsuSampleSet
+
+
+@item_props()
+class OsuHit(Hit, OsuNoteMeta):
+
+    def __init__(self,
+                 offset: float,
+                 column: int,
+                 hitsound_set: int = OsuSampleSet.AUTO,
+                 sample_set: int = OsuSampleSet.AUTO,
+                 addition_set: int = OsuSampleSet.AUTO,
+                 custom_set: int = 0,
+                 volume: int = 0,
+                 hitsound_file: str = "",
+                 **kwargs):
+        super().__init__(
+            offset=offset, column=column, hitsound_set=hitsound_set,
+            sample_set=sample_set, addition_set=addition_set,
+            custom_set=custom_set, volume=volume,
+            hitsound_file=hitsound_file, **kwargs
+        )
+
+    @staticmethod
+    def read_string(s: str, keys: int, as_dict: bool = False) -> OsuHit:
+        """Reads a single line under the [HitObject] Label"""
+
+        if not OsuNoteMeta.is_hit(s):
+            raise ValueError(f"Bad OsuHit Format. {s}")
+
+        s_comma = s.split(",")
+        s_colon = s_comma[-1].split(":")
+
+        d = dict(
+            offset=float(s_comma[2]),
+            column=OsuNoteMeta.x_axis_to_column(int(s_comma[0]), keys),
+            hitsound_set=int(s_comma[4]),
+            sample_set=int(s_colon[0]),
+            addition_set=int(s_colon[1]),
+            custom_set=int(s_colon[2]),
+            volume=int(s_colon[3]),
+            hitsound_file=s_colon[4]
+        )
+        return d if as_dict else OsuHit(**d)
+
+    def write_string(self, keys: int) -> str:
+        """Exports a .osu writable string"""
+        return f"{OsuNoteMeta.column_to_x_axis(self.column, keys=keys)}," \
+               f"{192}," \
+               f"{int(self.offset)}," \
+               f"{1}," \
+               f"{int(self.hitsound_set)}," \
+               f"{int(self.sample_set)}:" \
+               f"{int(self.addition_set)}:" \
+               f"{int(self.custom_set)}:" \
+               f"{int(self.volume)}:" \
+               f"{self.hitsound_file}"
```

### Comparing `reamber-0.1.7/reamber/osu/OsuMap.pyi` & `reamber-0.1.8/reamber/osu/OsuMap.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,101 +1,102 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from typing import List, Union, Tuple, TypeVar, Type
-
-import pandas as pd
-
-from reamber.base.Map import Map
-from reamber.base.lists.TimedList import TimedList
-from reamber.osu.OsuMapMeta import OsuMapMeta
-from reamber.osu.lists.OsuBpmList import OsuBpmList
-from reamber.osu.lists.OsuSvList import OsuSvList
-from reamber.osu.lists.notes.OsuHitList import OsuHitList
-from reamber.osu.lists.notes.OsuHoldList import OsuHoldList
-from reamber.osu.lists.notes.OsuNoteList import OsuNoteList
-
-T = TypeVar('T', bound=TimedList)
-
-
-@dataclass
-class OsuMap(Map[OsuNoteList, OsuHitList, OsuHoldList, OsuBpmList],
-             OsuMapMeta):
-
-    @property
-    def svs(self) -> OsuSvList: ...
-
-    @svs.setter
-    def svs(self, val) -> None: ...
-
-    def reset_samples(self, notes=True, samples=True) -> None: ...
-
-    @staticmethod
-    def read(lines: List[str]) -> OsuMap: ...
-
-    @staticmethod
-    def read_file(file_path: str) -> OsuMap: ...
-
-    def write(self) -> List[str]: ...
-
-    def write_file(self, file_path="") -> None: ...
-
-    def _read_file_metadata(self, lines: List[str]): ...
-
-    def _read_file_timing_points(self, lines: Union[List[str], str]): ...
-
-    def _read_file_hit_objects(self, lines: Union[List[str], str]): ...
-
-    def metadata(self, unicode=True, **kwargs) -> str: ...
-
-    def rate(self, by: float) -> OsuMap: ...
-
-    class Stacker(Map.Stacker):
-        @property
-        def hitsound_set(self) -> pd.Series: ...
-
-        @hitsound_set.setter
-        def hitsound_set(self, val) -> None: ...
-
-        @property
-        def sample_set(self) -> pd.Series: ...
-
-        @sample_set.setter
-        def sample_set(self, val) -> None: ...
-
-        @property
-        def addition_set(self) -> pd.Series: ...
-
-        @addition_set.setter
-        def addition_set(self, val) -> None: ...
-
-        @property
-        def custom_set(self) -> pd.Series: ...
-
-        @custom_set.setter
-        def custom_set(self, val) -> None: ...
-
-        @property
-        def volume(self) -> pd.Series: ...
-
-        @volume.setter
-        def volume(self, val) -> None: ...
-
-        @property
-        def hitsound_file(self) -> pd.Series: ...
-
-        @hitsound_file.setter
-        def hitsound_file(self, val) -> None: ...
-
-        @property
-        def sample_set_index(self) -> pd.Series: ...
-
-        @sample_set_index.setter
-        def sample_set_index(self, val) -> None: ...
-
-        @property
-        def kiai(self) -> pd.Series: ...
-
-        @kiai.setter
-        def kiai(self, val) -> None: ...
-
-    def stack(self, include_types: Tuple[Type[T]] = None) -> Stacker: ...
+from __future__ import annotations
+
+from dataclasses import dataclass
+from pathlib import Path
+from typing import List, Union, Tuple, TypeVar, Type
+
+import pandas as pd
+
+from reamber.base.Map import Map
+from reamber.base.lists.TimedList import TimedList
+from reamber.osu.OsuMapMeta import OsuMapMeta
+from reamber.osu.lists.OsuBpmList import OsuBpmList
+from reamber.osu.lists.OsuSvList import OsuSvList
+from reamber.osu.lists.notes.OsuHitList import OsuHitList
+from reamber.osu.lists.notes.OsuHoldList import OsuHoldList
+from reamber.osu.lists.notes.OsuNoteList import OsuNoteList
+
+T = TypeVar('T', bound=TimedList)
+
+
+@dataclass
+class OsuMap(Map[OsuNoteList, OsuHitList, OsuHoldList, OsuBpmList],
+             OsuMapMeta):
+
+    @property
+    def svs(self) -> OsuSvList: ...
+
+    @svs.setter
+    def svs(self, val) -> None: ...
+
+    def reset_samples(self, notes=True, samples=True) -> None: ...
+
+    @staticmethod
+    def read(lines: List[str]) -> OsuMap: ...
+
+    @staticmethod
+    def read_file(file_path: str | Path) -> OsuMap: ...
+
+    def write(self) -> List[str]: ...
+
+    def write_file(self, file_path: str | Path) -> None: ...
+
+    def _read_file_metadata(self, lines: List[str]): ...
+
+    def _read_file_timing_points(self, lines: Union[List[str], str]): ...
+
+    def _read_file_hit_objects(self, lines: Union[List[str], str]): ...
+
+    def metadata(self, unicode=True, **kwargs) -> str: ...
+
+    def rate(self, by: float) -> OsuMap: ...
+
+    class Stacker(Map.Stacker):
+        @property
+        def hitsound_set(self) -> pd.Series: ...
+
+        @hitsound_set.setter
+        def hitsound_set(self, val) -> None: ...
+
+        @property
+        def sample_set(self) -> pd.Series: ...
+
+        @sample_set.setter
+        def sample_set(self, val) -> None: ...
+
+        @property
+        def addition_set(self) -> pd.Series: ...
+
+        @addition_set.setter
+        def addition_set(self, val) -> None: ...
+
+        @property
+        def custom_set(self) -> pd.Series: ...
+
+        @custom_set.setter
+        def custom_set(self, val) -> None: ...
+
+        @property
+        def volume(self) -> pd.Series: ...
+
+        @volume.setter
+        def volume(self, val) -> None: ...
+
+        @property
+        def hitsound_file(self) -> pd.Series: ...
+
+        @hitsound_file.setter
+        def hitsound_file(self, val) -> None: ...
+
+        @property
+        def sample_set_index(self) -> pd.Series: ...
+
+        @sample_set_index.setter
+        def sample_set_index(self, val) -> None: ...
+
+        @property
+        def kiai(self) -> pd.Series: ...
+
+        @kiai.setter
+        def kiai(self, val) -> None: ...
+
+    def stack(self, include_types: Tuple[Type[T]] = None) -> Stacker: ...
```

### Comparing `reamber-0.1.7/reamber/osu/OsuMapMeta.py` & `reamber-0.1.8/reamber/osu/OsuMapMeta.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,224 +1,224 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import List
-
-from unidecode import unidecode
-
-from reamber.osu.OsuSampleSet import OsuSampleSet
-from reamber.osu.lists.OsuSampleList import OsuSampleList
-
-
-class OsuMapMode:
-    """This determines the mode of the map.
-
-    Note that only MANIA is supported for now.
-    """
-    STANDARD: int = 0
-    TAIKO: int = 1
-    CATCH: int = 2
-    MANIA: int = 3
-
-
-@dataclass
-class OsuMapMetaGeneral:
-    """All meta under [General] """
-
-    audio_file_name: str = ""
-    audio_lead_in: int = 0
-    preview_time: int = -1
-    countdown: bool = False
-    sample_set: int = OsuSampleSet.AUTO
-    stack_leniency: float = 0.7
-    mode: int = OsuMapMode.MANIA
-    letterbox_in_breaks: bool = False
-    special_style: bool = False
-    widescreen_storyboard: bool = True
-
-
-@dataclass
-class OsuMapMetaEditor:
-    """All meta under [Editor] """
-
-    distance_spacing: float = 4
-    beat_divisor: int = 4
-    grid_size: int = 8
-    timeline_zoom: float = 0.3
-
-
-@dataclass
-class OsuMapMetaMetadata:
-    """All meta under [Metadata] """
-
-    title: str = ""
-    title_unicode: str = ""
-    artist: str = ""
-    artist_unicode: str = ""
-    creator: str = ""
-    version: str = ""
-    source: str = ""
-    tags: List[str] = ""
-    beatmap_id: int = 0
-    beatmap_set_id: int = -1
-
-
-@dataclass
-class OsuMapMetaDifficulty:
-    """All meta under [Difficulty] """
-
-    hp_drain_rate: float = 5.0
-    circle_size: float = 4.0
-    overall_difficulty: float = 5.0
-    approach_rate: float = 5.0
-    slider_multiplier: float = 1.4
-    slider_tick_rate: int = 1
-
-
-@dataclass
-class OsuMapMetaEvents:
-    """All meta under [Events], Excludes Storyboard. """
-
-    background_file_name: str = ""
-    samples: OsuSampleList = field(default_factory=lambda: OsuSampleList([]))
-
-
-@dataclass
-class OsuMapMeta(OsuMapMetaGeneral,
-                 OsuMapMetaEditor,
-                 OsuMapMetaMetadata,
-                 OsuMapMetaDifficulty,
-                 OsuMapMetaEvents):
-    def _read_meta_string_list(self, lines: List[str]):
-        """Reads everything Meta"""
-        for e, line in enumerate(lines):
-            if line == "":
-                continue
-            k, *v = line.split(":")
-            if v: v = v[0]
-            if k == "AudioFilename":
-                self.audio_file_name = v.strip()
-            elif k == "AudioLeadIn":
-                self.audio_lead_in = int(v)
-            elif k == "PreviewTime":
-                self.preview_time = int(v)
-            elif k == "Countdown":
-                self.countdown = bool(int(v))
-            elif k == "SampleSet":
-                self.sample_set = OsuSampleSet.from_string(v.strip())
-            elif k == "StackLeniency":
-                self.stack_leniency = float(v)
-            elif k == "Mode":
-                self.mode = int(v)
-            elif k == "LetterboxInBreaks":
-                self.letterbox_in_breaks = bool(int(v))
-            elif k == "SpecialStyle":
-                self.special_style = bool(int(v))
-            elif k == "WidescreenStoryboard":
-                self.widescreen_storyboard = bool(int(v))
-            elif k == "DistanceSpacing":
-                self.distance_spacing = float(v)
-            elif k == "BeatDivisor":
-                self.beat_divisor = int(v)
-            elif k == "GridSize":
-                self.grid_size = int(v)
-            elif k == "TimelineZoom":
-                self.timeline_zoom = float(v)
-            elif k == "Title":
-                self.title = v.strip()
-            elif k == "TitleUnicode":
-                self.title_unicode = v.strip()
-            elif k == "Artist":
-                self.artist = v.strip()
-            elif k == "ArtistUnicode":
-                self.artist_unicode = v.strip()
-            elif k == "Creator":
-                self.creator = v.strip()
-            elif k == "Version":
-                self.version = v.strip()
-            elif k == "Source":
-                self.source = v.strip()
-            elif k == "Tags":
-                self.tags = [i.strip() for i in v.split(" ") if i]
-            elif k == "BeatmapID":
-                self.beatmap_id = int(v)
-            elif k == "BeatmapSetID":
-                self.beatmap_set_id = int(v)
-            elif k == "HPDrainRate":
-                self.hp_drain_rate = float(v)
-            elif k == "CircleSize":
-                self.circle_size = float(v)
-            elif k == "OverallDifficulty":
-                self.overall_difficulty = float(v)
-            elif k == "ApproachRate":
-                self.approach_rate = float(v)
-            elif k == "SliderMultiplier":
-                self.slider_multiplier = float(v)
-            elif k == "SliderTickRate":
-                self.slider_tick_rate = int(v)
-
-            if k == "//Background and Video events":
-                line = lines[e + 1]
-                self.background_file_name = \
-                    line[line.find('"') + 1:line.rfind('"')]
-
-            if k == "//Storyboard Sound Samples":
-                self.samples = OsuSampleList.read(
-                    [line for line in lines[e + 1:] if
-                     line.startswith('Sample')]
-                )
-
-    def write_meta_string_list(self) -> List[str]:
-        """Writes everything Meta"""
-        return [
-            "osu file format v14",
-            "",
-            "[General]",
-            f"AudioFilename: {self.audio_file_name}",
-            f"AudioLeadIn: {self.audio_lead_in:g}",
-            f"PreviewTime: {int(self.preview_time)}",
-            f"Countdown: {int(self.countdown)}",
-            f"SampleSet: {OsuSampleSet.to_string(self.sample_set)}",
-            f"StackLeniency: {self.stack_leniency}",
-            f"Mode: {self.mode}",
-            f"LetterboxInBreaks: {int(self.letterbox_in_breaks)}",
-            f"SpecialStyle: {int(self.special_style)}",
-            f"WidescreenStoryboard: {int(self.widescreen_storyboard)}",
-            "",
-            "[Editor]",
-            f"DistanceSpacing: {self.distance_spacing:g}",
-            f"BeatDivisor: {self.beat_divisor:g}",
-            f"GridSize: {self.grid_size:g}",
-            f"TimelineZoom: {self.timeline_zoom:g}",
-            "",
-            "[Metadata]",
-            f"Title:{unidecode(self.title)}",
-            f"TitleUnicode:{self.title_unicode}",
-            f"Artist:{unidecode(self.artist)}",
-            f"ArtistUnicode:{self.artist_unicode}",
-            f"Creator:{self.creator}",
-            f"Version:{self.version}",
-            f"Source:{self.source}",
-            f"Tags:{' '.join(self.tags)}",
-            f"BeatmapID:{self.beatmap_id}",
-            f"BeatmapSetID:{self.beatmap_set_id}",
-            "",
-            "[Difficulty]",
-            f"HPDrainRate:{self.hp_drain_rate:g}",
-            f"CircleSize:{self.circle_size:g}",
-            f"OverallDifficulty:{self.overall_difficulty:g}",
-            f"ApproachRate:{self.approach_rate:g}",
-            f"SliderMultiplier:{self.slider_multiplier:g}",
-            f"SliderTickRate:{self.slider_tick_rate:g}",
-            "",
-            "[Events]",
-            "//Background and Video events",
-            f"0,0,\"{self.background_file_name}\",0,0",
-            "//Break Periods",
-            "//Storyboard Layer 0 (Background)",
-            "//Storyboard Layer 1 (Fail)",
-            "//Storyboard Layer 2 (Pass)",
-            "//Storyboard Layer 3 (Foreground)",
-            "//Storyboard Layer 4 (Overlay)",
-            "//Storyboard Sound Samples",
-            *[sample.write_string() for sample in self.samples]
-        ]
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import List
+
+from unidecode import unidecode
+
+from reamber.osu.OsuSampleSet import OsuSampleSet
+from reamber.osu.lists.OsuSampleList import OsuSampleList
+
+
+class OsuMapMode:
+    """This determines the mode of the map.
+
+    Note that only MANIA is supported for now.
+    """
+    STANDARD: int = 0
+    TAIKO: int = 1
+    CATCH: int = 2
+    MANIA: int = 3
+
+
+@dataclass
+class OsuMapMetaGeneral:
+    """All meta under [General] """
+
+    audio_file_name: str = ""
+    audio_lead_in: int = 0
+    preview_time: int = -1
+    countdown: bool = False
+    sample_set: int = OsuSampleSet.AUTO
+    stack_leniency: float = 0.7
+    mode: int = OsuMapMode.MANIA
+    letterbox_in_breaks: bool = False
+    special_style: bool = False
+    widescreen_storyboard: bool = True
+
+
+@dataclass
+class OsuMapMetaEditor:
+    """All meta under [Editor] """
+
+    distance_spacing: float = 4
+    beat_divisor: int = 4
+    grid_size: int = 8
+    timeline_zoom: float = 0.3
+
+
+@dataclass
+class OsuMapMetaMetadata:
+    """All meta under [Metadata] """
+
+    title: str = ""
+    title_unicode: str = ""
+    artist: str = ""
+    artist_unicode: str = ""
+    creator: str = ""
+    version: str = ""
+    source: str = ""
+    tags: List[str] = ""
+    beatmap_id: int = 0
+    beatmap_set_id: int = -1
+
+
+@dataclass
+class OsuMapMetaDifficulty:
+    """All meta under [Difficulty] """
+
+    hp_drain_rate: float = 5.0
+    circle_size: float = 4.0
+    overall_difficulty: float = 5.0
+    approach_rate: float = 5.0
+    slider_multiplier: float = 1.4
+    slider_tick_rate: int = 1
+
+
+@dataclass
+class OsuMapMetaEvents:
+    """All meta under [Events], Excludes Storyboard. """
+
+    background_file_name: str = ""
+    samples: OsuSampleList = field(default_factory=lambda: OsuSampleList([]))
+
+
+@dataclass
+class OsuMapMeta(OsuMapMetaGeneral,
+                 OsuMapMetaEditor,
+                 OsuMapMetaMetadata,
+                 OsuMapMetaDifficulty,
+                 OsuMapMetaEvents):
+    def _read_meta_string_list(self, lines: List[str]):
+        """Reads everything Meta"""
+        for e, line in enumerate(lines):
+            if line == "":
+                continue
+            k, *v = line.split(":")
+            if v: v = v[0]
+            if k == "AudioFilename":
+                self.audio_file_name = v.strip()
+            elif k == "AudioLeadIn":
+                self.audio_lead_in = int(v)
+            elif k == "PreviewTime":
+                self.preview_time = int(v)
+            elif k == "Countdown":
+                self.countdown = bool(int(v))
+            elif k == "SampleSet":
+                self.sample_set = OsuSampleSet.from_string(v.strip())
+            elif k == "StackLeniency":
+                self.stack_leniency = float(v)
+            elif k == "Mode":
+                self.mode = int(v)
+            elif k == "LetterboxInBreaks":
+                self.letterbox_in_breaks = bool(int(v))
+            elif k == "SpecialStyle":
+                self.special_style = bool(int(v))
+            elif k == "WidescreenStoryboard":
+                self.widescreen_storyboard = bool(int(v))
+            elif k == "DistanceSpacing":
+                self.distance_spacing = float(v)
+            elif k == "BeatDivisor":
+                self.beat_divisor = int(v)
+            elif k == "GridSize":
+                self.grid_size = int(v)
+            elif k == "TimelineZoom":
+                self.timeline_zoom = float(v)
+            elif k == "Title":
+                self.title = v.strip()
+            elif k == "TitleUnicode":
+                self.title_unicode = v.strip()
+            elif k == "Artist":
+                self.artist = v.strip()
+            elif k == "ArtistUnicode":
+                self.artist_unicode = v.strip()
+            elif k == "Creator":
+                self.creator = v.strip()
+            elif k == "Version":
+                self.version = v.strip()
+            elif k == "Source":
+                self.source = v.strip()
+            elif k == "Tags":
+                self.tags = [i.strip() for i in v.split(" ") if i]
+            elif k == "BeatmapID":
+                self.beatmap_id = int(v)
+            elif k == "BeatmapSetID":
+                self.beatmap_set_id = int(v)
+            elif k == "HPDrainRate":
+                self.hp_drain_rate = float(v)
+            elif k == "CircleSize":
+                self.circle_size = float(v)
+            elif k == "OverallDifficulty":
+                self.overall_difficulty = float(v)
+            elif k == "ApproachRate":
+                self.approach_rate = float(v)
+            elif k == "SliderMultiplier":
+                self.slider_multiplier = float(v)
+            elif k == "SliderTickRate":
+                self.slider_tick_rate = float(v)
+
+            if k == "//Background and Video events":
+                line = lines[e + 1]
+                self.background_file_name = \
+                    line[line.find('"') + 1:line.rfind('"')]
+
+            if k == "//Storyboard Sound Samples":
+                self.samples = OsuSampleList.read(
+                    [line for line in lines[e + 1:] if
+                     line.startswith('Sample')]
+                )
+
+    def write_meta_string_list(self) -> List[str]:
+        """Writes everything Meta"""
+        return [
+            "osu file format v14",
+            "",
+            "[General]",
+            f"AudioFilename: {self.audio_file_name}",
+            f"AudioLeadIn: {self.audio_lead_in:g}",
+            f"PreviewTime: {int(self.preview_time)}",
+            f"Countdown: {int(self.countdown)}",
+            f"SampleSet: {OsuSampleSet.to_string(self.sample_set)}",
+            f"StackLeniency: {self.stack_leniency}",
+            f"Mode: {self.mode}",
+            f"LetterboxInBreaks: {int(self.letterbox_in_breaks)}",
+            f"SpecialStyle: {int(self.special_style)}",
+            f"WidescreenStoryboard: {int(self.widescreen_storyboard)}",
+            "",
+            "[Editor]",
+            f"DistanceSpacing: {self.distance_spacing:g}",
+            f"BeatDivisor: {self.beat_divisor:g}",
+            f"GridSize: {self.grid_size:g}",
+            f"TimelineZoom: {self.timeline_zoom:g}",
+            "",
+            "[Metadata]",
+            f"Title:{unidecode(self.title)}",
+            f"TitleUnicode:{self.title_unicode}",
+            f"Artist:{unidecode(self.artist)}",
+            f"ArtistUnicode:{self.artist_unicode}",
+            f"Creator:{self.creator}",
+            f"Version:{self.version}",
+            f"Source:{self.source}",
+            f"Tags:{' '.join(self.tags)}",
+            f"BeatmapID:{self.beatmap_id}",
+            f"BeatmapSetID:{self.beatmap_set_id}",
+            "",
+            "[Difficulty]",
+            f"HPDrainRate:{self.hp_drain_rate:g}",
+            f"CircleSize:{self.circle_size:g}",
+            f"OverallDifficulty:{self.overall_difficulty:g}",
+            f"ApproachRate:{self.approach_rate:g}",
+            f"SliderMultiplier:{self.slider_multiplier:g}",
+            f"SliderTickRate:{self.slider_tick_rate:g}",
+            "",
+            "[Events]",
+            "//Background and Video events",
+            f"0,0,\"{self.background_file_name}\",0,0",
+            "//Break Periods",
+            "//Storyboard Layer 0 (Background)",
+            "//Storyboard Layer 1 (Fail)",
+            "//Storyboard Layer 2 (Pass)",
+            "//Storyboard Layer 3 (Foreground)",
+            "//Storyboard Layer 4 (Overlay)",
+            "//Storyboard Sound Samples",
+            *[sample.write_string() for sample in self.samples]
+        ]
```

### Comparing `reamber-0.1.7/reamber/osu/OsuNoteMeta.pyi` & `reamber-0.1.8/reamber/osu/OsuNoteMeta.pyi`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-class OsuNoteMeta:
-    @staticmethod
-    def x_axis_to_column(x_axis: float, keys: int,
-                         clip: bool = True) -> int: ...
-
-    @staticmethod
-    def column_to_x_axis(column: float, keys: int) -> int: ...
-
-    def reset_samples(self) -> None: ...
-
-    @staticmethod
-    def is_hit(s: str) -> bool: ...
-
-    @staticmethod
-    def is_hold(s: str) -> bool: ...
-
-    @property
-    def hitsound_set(self) -> int: ...
-
-    @hitsound_set.setter
-    def hitsound_set(self, val) -> None: ...
-
-    @property
-    def sample_set(self) -> int: ...
-
-    @sample_set.setter
-    def sample_set(self, val) -> None: ...
-
-    @property
-    def addition_set(self) -> int: ...
-
-    @addition_set.setter
-    def addition_set(self, val) -> None: ...
-
-    @property
-    def custom_set(self) -> int: ...
-
-    @custom_set.setter
-    def custom_set(self, val) -> None: ...
-
-    @property
-    def volume(self) -> int: ...
-
-    @volume.setter
-    def volume(self, val) -> None: ...
-
-    @property
-    def hitsound_file(self) -> str: ...
-
-    @hitsound_file.setter
-    def hitsound_file(self, val) -> None: ...
+class OsuNoteMeta:
+    @staticmethod
+    def x_axis_to_column(x_axis: float, keys: int,
+                         clip: bool = True) -> int: ...
+
+    @staticmethod
+    def column_to_x_axis(column: float, keys: int) -> int: ...
+
+    def reset_samples(self) -> None: ...
+
+    @staticmethod
+    def is_hit(s: str) -> bool: ...
+
+    @staticmethod
+    def is_hold(s: str) -> bool: ...
+
+    @property
+    def hitsound_set(self) -> int: ...
+
+    @hitsound_set.setter
+    def hitsound_set(self, val) -> None: ...
+
+    @property
+    def sample_set(self) -> int: ...
+
+    @sample_set.setter
+    def sample_set(self, val) -> None: ...
+
+    @property
+    def addition_set(self) -> int: ...
+
+    @addition_set.setter
+    def addition_set(self, val) -> None: ...
+
+    @property
+    def custom_set(self) -> int: ...
+
+    @custom_set.setter
+    def custom_set(self, val) -> None: ...
+
+    @property
+    def volume(self) -> int: ...
+
+    @volume.setter
+    def volume(self, val) -> None: ...
+
+    @property
+    def hitsound_file(self) -> str: ...
+
+    @hitsound_file.setter
+    def hitsound_file(self, val) -> None: ...
```

### Comparing `reamber-0.1.7/reamber/osu/OsuSample.py` & `reamber-0.1.8/reamber/osu/OsuSample.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-from __future__ import annotations
-
-from reamber.base import item_props
-from reamber.base.Timed import Timed
-
-
-@item_props()
-class OsuSample(Timed):
-    """Osu Samples are autoplay hitsounds. Under [Events]
-
-    Not to be confused w/ OsuSampleSet, a class of static variables
-    """
-
-    _props = dict(sample_file=['str', ''],
-                  volume=['int', 50])
-
-    def __init__(self,
-                 offset: float,
-                 sample_file: str = '',
-                 volume: int = 70,
-                 **kwargs):
-        super().__init__(offset=offset, sample_file=sample_file, volume=volume,
-                         **kwargs)
-
-    @staticmethod
-    def read_string(s: str, as_dict: bool = False) -> OsuSample:
-        """Reads the string as a sample"""
-        s_comma = s.split(",")
-        try:
-            d = dict(offset=float(s_comma[1]),
-                     sample_file=s_comma[3],
-                     volume=int(s_comma[4]))
-            return d if as_dict else OsuSample(**d)
-        except IndexError as e:
-            raise ValueError(f"Bad OsuSample format. {s}, {e.args}")
-
-    def write_string(self) -> str:
-        """Exports the sample as a string"""
-        return f"Sample,{int(self.offset)},0,{self.sample_file},{self.volume}"
+from __future__ import annotations
+
+from reamber.base import item_props
+from reamber.base.Timed import Timed
+
+
+@item_props()
+class OsuSample(Timed):
+    """Osu Samples are autoplay hitsounds. Under [Events]
+
+    Not to be confused w/ OsuSampleSet, a class of static variables
+    """
+
+    _props = dict(sample_file=['str', ''],
+                  volume=['int', 50])
+
+    def __init__(self,
+                 offset: float,
+                 sample_file: str = '',
+                 volume: int = 70,
+                 **kwargs):
+        super().__init__(offset=offset, sample_file=sample_file, volume=volume,
+                         **kwargs)
+
+    @staticmethod
+    def read_string(s: str, as_dict: bool = False) -> OsuSample:
+        """Reads the string as a sample"""
+        s_comma = s.split(",")
+        try:
+            d = dict(offset=float(s_comma[1]),
+                     sample_file=s_comma[3],
+                     volume=int(s_comma[4]))
+            return d if as_dict else OsuSample(**d)
+        except IndexError as e:
+            raise ValueError(f"Bad OsuSample format. {s}, {e.args}")
+
+    def write_string(self) -> str:
+        """Exports the sample as a string"""
+        return f"Sample,{int(self.offset)},0,{self.sample_file},{self.volume}"
```

### Comparing `reamber-0.1.7/reamber/osu/OsuSample.pyi` & `reamber-0.1.8/reamber/osu/OsuSample.pyi`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from __future__ import annotations
-
-from typing import Dict, overload
-
-from reamber.base.Timed import Timed
-
-
-class OsuSample(Timed):
-    def __init__(self, offset: float, sample_file: str = '', volume: int = 70,
-                 **kwargs): ...
-
-    @staticmethod
-    @overload
-    def read_string(s: str, as_dict: bool = False) -> OsuSample: ...
-
-    @staticmethod
-    @overload
-    def read_string(s: str, as_dict: bool = True) -> Dict[str]: ...
-
-    @staticmethod
-    def read_string(s: str, as_dict: bool = True) -> OsuSample or Dict[
-        str]: ...
-
-    def write_string(self) -> str: ...
-
-    @property
-    def sample_file(self) -> str: ...
-
-    @sample_file.setter
-    def sample_file(self, val) -> None: ...
-
-    @property
-    def volume(self) -> str: ...
-
-    @volume.setter
-    def volume(self, val) -> None: ...
+from __future__ import annotations
+
+from typing import Dict, overload
+
+from reamber.base.Timed import Timed
+
+
+class OsuSample(Timed):
+    def __init__(self, offset: float, sample_file: str = '', volume: int = 70,
+                 **kwargs): ...
+
+    @staticmethod
+    @overload
+    def read_string(s: str, as_dict: bool = False) -> OsuSample: ...
+
+    @staticmethod
+    @overload
+    def read_string(s: str, as_dict: bool = True) -> Dict[str]: ...
+
+    @staticmethod
+    def read_string(s: str, as_dict: bool = True) -> OsuSample or Dict[
+        str]: ...
+
+    def write_string(self) -> str: ...
+
+    @property
+    def sample_file(self) -> str: ...
+
+    @sample_file.setter
+    def sample_file(self, val) -> None: ...
+
+    @property
+    def volume(self) -> str: ...
+
+    @volume.setter
+    def volume(self, val) -> None: ...
```

### Comparing `reamber-0.1.7/reamber/osu/OsuSampleSet.py` & `reamber-0.1.8/reamber/osu/OsuSampleSet.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-class OsuSampleSet:
-    """Osu SampleSet are an "enum" of available hitsounds.
-
-    Not to be confused with OsuSample, a class for samples under [Events]
-    """
-    AUTO: int = 0
-    NORMAL: int = 1
-    SOFT: int = 2
-    DRUM: int = 3
-
-    @staticmethod
-    def to_string(sample_set: int) -> str:
-        """Converts an int to a string representing SampleSet"""
-        if sample_set == OsuSampleSet.AUTO:
-            return "None"
-        elif sample_set == OsuSampleSet.NORMAL:
-            return "Normal"
-        elif sample_set == OsuSampleSet.SOFT:
-            return "Soft"
-        elif sample_set == OsuSampleSet.DRUM:
-            return "Drum"
-        else:
-            return "Invalid"
-
-    @staticmethod
-    def from_string(sample_set: str) -> int:
-        """Converts a SampleSet string to an int"""
-        if sample_set == "None":
-            return OsuSampleSet.AUTO
-        elif sample_set == "Normal":
-            return OsuSampleSet.NORMAL
-        elif sample_set == "Soft":
-            return OsuSampleSet.SOFT
-        elif sample_set == "Drum":
-            return OsuSampleSet.DRUM
-        else:
-            return -1
+class OsuSampleSet:
+    """Osu SampleSet are an "enum" of available hitsounds.
+
+    Not to be confused with OsuSample, a class for samples under [Events]
+    """
+    AUTO: int = 0
+    NORMAL: int = 1
+    SOFT: int = 2
+    DRUM: int = 3
+
+    @staticmethod
+    def to_string(sample_set: int) -> str:
+        """Converts an int to a string representing SampleSet"""
+        if sample_set == OsuSampleSet.AUTO:
+            return "None"
+        elif sample_set == OsuSampleSet.NORMAL:
+            return "Normal"
+        elif sample_set == OsuSampleSet.SOFT:
+            return "Soft"
+        elif sample_set == OsuSampleSet.DRUM:
+            return "Drum"
+        else:
+            return "Invalid"
+
+    @staticmethod
+    def from_string(sample_set: str) -> int:
+        """Converts a SampleSet string to an int"""
+        if sample_set == "None":
+            return OsuSampleSet.AUTO
+        elif sample_set == "Normal":
+            return OsuSampleSet.NORMAL
+        elif sample_set == "Soft":
+            return OsuSampleSet.SOFT
+        elif sample_set == "Drum":
+            return OsuSampleSet.DRUM
+        else:
+            return -1
```

### Comparing `reamber-0.1.7/reamber/osu/OsuTimingPointMeta.py` & `reamber-0.1.8/reamber/osu/OsuTimingPointMeta.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from reamber.base.Property import item_props
-
-class OsuTimingPointType:
-    SV: int = 0
-    Bpm: int = 1
-
-@item_props()
-class OsuTimingPointMeta:
-    """Holds all metadata for every timing point object"""
-
-    _props = dict(sample_set=['int', 0],
-                  sample_set_index=['int', 0],
-                  volume=['int', 0],
-                  kiai=['bool', False])
-
-    @staticmethod
-    def is_timing_point(s: str) -> bool:
-        """If string is a Timing Point/Bpm Obj"""
-        t = s.split(",")
-        if len(t) != 8: return False
-        return t[6] == "1"
-
-    @staticmethod
-    def is_slider_velocity(s: str) -> bool:
-        """If string is a SV Obj"""
-        t = s.split(",")
-        if len(t) != 8: return False
-        return t[6] == "0"
+from reamber.base.Property import item_props
+
+class OsuTimingPointType:
+    SV: int = 0
+    Bpm: int = 1
+
+@item_props()
+class OsuTimingPointMeta:
+    """Holds all metadata for every timing point object"""
+
+    _props = dict(sample_set=['int', 0],
+                  sample_set_index=['int', 0],
+                  volume=['int', 0],
+                  kiai=['bool', False])
+
+    @staticmethod
+    def is_timing_point(s: str) -> bool:
+        """If string is a Timing Point/Bpm Obj"""
+        t = s.split(",")
+        if len(t) != 8: return False
+        return t[6] == "1"
+
+    @staticmethod
+    def is_slider_velocity(s: str) -> bool:
+        """If string is a SV Obj"""
+        t = s.split(",")
+        if len(t) != 8: return False
+        return t[6] == "0"
```

### Comparing `reamber-0.1.7/reamber/osu/__init__.py` & `reamber-0.1.8/reamber/osu/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from reamber.osu.OsuBpm import OsuBpm
-from reamber.osu.OsuHit import OsuHit
-from reamber.osu.OsuHold import OsuHold
-from reamber.osu.OsuMap import OsuMap
-from reamber.osu.OsuMapMeta import OsuMapMeta
-from reamber.osu.OsuNoteMeta import OsuNoteMeta
-from reamber.osu.OsuSampleSet import OsuSampleSet
-from reamber.osu.OsuSv import OsuSv
-from reamber.osu.OsuTimingPointMeta import OsuTimingPointMeta
-
-__all__ = ['OsuBpm', 'OsuHit', 'OsuNoteMeta', 'OsuHold', 'OsuMap',
-           'OsuMapMeta', 'OsuSampleSet', 'OsuTimingPointMeta', 'OsuSv']
+from reamber.osu.OsuBpm import OsuBpm
+from reamber.osu.OsuHit import OsuHit
+from reamber.osu.OsuHold import OsuHold
+from reamber.osu.OsuMap import OsuMap
+from reamber.osu.OsuMapMeta import OsuMapMeta
+from reamber.osu.OsuNoteMeta import OsuNoteMeta
+from reamber.osu.OsuSampleSet import OsuSampleSet
+from reamber.osu.OsuSv import OsuSv
+from reamber.osu.OsuTimingPointMeta import OsuTimingPointMeta
+
+__all__ = ['OsuBpm', 'OsuHit', 'OsuNoteMeta', 'OsuHold', 'OsuMap',
+           'OsuMapMeta', 'OsuSampleSet', 'OsuTimingPointMeta', 'OsuSv']
```

### Comparing `reamber-0.1.7/reamber/osu/lists/OsuSampleList.py` & `reamber-0.1.8/reamber/osu/lists/OsuSampleList.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from __future__ import annotations
-
-from typing import List
-
-import pandas as pd
-
-from reamber.base.Property import list_props
-from reamber.base.lists.TimedList import TimedList
-from reamber.osu.OsuSample import OsuSample
-
-
-@list_props(OsuSample)
-class OsuSampleList(TimedList[OsuSample]):
-    @staticmethod
-    def read(strings: List[str]) -> OsuSampleList:
-        return OsuSampleList(
-            pd.DataFrame(
-                [OsuSample.read_string(s, True) for s in strings]
-            ) if strings else [])
-
-    def write(self) -> List[str]:
-        return [h.write_string() for h in self]
+from __future__ import annotations
+
+from typing import List
+
+import pandas as pd
+
+from reamber.base.Property import list_props
+from reamber.base.lists.TimedList import TimedList
+from reamber.osu.OsuSample import OsuSample
+
+
+@list_props(OsuSample)
+class OsuSampleList(TimedList[OsuSample]):
+    @staticmethod
+    def read(strings: List[str]) -> OsuSampleList:
+        return OsuSampleList(
+            pd.DataFrame(
+                [OsuSample.read_string(s, True) for s in strings]
+            ) if strings else [])
+
+    def write(self) -> List[str]:
+        return [h.write_string() for h in self]
```

### Comparing `reamber-0.1.7/reamber/osu/lists/OsuSampleList.pyi` & `reamber-0.1.8/reamber/osu/lists/OsuSampleList.pyi`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from __future__ import annotations
-
-from typing import List
-
-import pandas as pd
-
-from reamber.base.lists.TimedList import TimedList
-from reamber.osu.OsuSample import OsuSample
-
-
-class OsuSampleList(TimedList[OsuSample]):
-    @staticmethod
-    def read(strings: List[str]) -> OsuSampleList: ...
-
-    def write(self) -> List[str]: ...
-
-    @property
-    def sample_file(self) -> pd.Series: ...
-
-    @sample_file.setter
-    def sample_file(self, val) -> None: ...
-
-    @property
-    def volume(self) -> pd.Series: ...
-
-    @volume.setter
-    def volume(self, val) -> None: ...
+from __future__ import annotations
+
+from typing import List
+
+import pandas as pd
+
+from reamber.base.lists.TimedList import TimedList
+from reamber.osu.OsuSample import OsuSample
+
+
+class OsuSampleList(TimedList[OsuSample]):
+    @staticmethod
+    def read(strings: List[str]) -> OsuSampleList: ...
+
+    def write(self) -> List[str]: ...
+
+    @property
+    def sample_file(self) -> pd.Series: ...
+
+    @sample_file.setter
+    def sample_file(self, val) -> None: ...
+
+    @property
+    def volume(self) -> pd.Series: ...
+
+    @volume.setter
+    def volume(self, val) -> None: ...
```

### Comparing `reamber-0.1.7/reamber/osu/lists/OsuSvList.py` & `reamber-0.1.8/reamber/osu/lists/OsuSvList.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from __future__ import annotations
-
-from typing import List
-
-import pandas as pd
-
-from reamber.base.Property import list_props
-from reamber.base.lists.TimedList import TimedList
-from reamber.osu.OsuSv import OsuSv
-
-
-@list_props(OsuSv)
-class OsuSvList(TimedList[OsuSv]):
-
-    @staticmethod
-    def read(strings: List[str]) -> OsuSvList:
-        return OsuSvList(pd.DataFrame(
-            [OsuSv.read_string(s, as_dict=True) for s in
-             strings]) if strings else [])
-
-    def write(self) -> List[str]:
-        return [h.write_string() for h in self]
+from __future__ import annotations
+
+from typing import List
+
+import pandas as pd
+
+from reamber.base.Property import list_props
+from reamber.base.lists.TimedList import TimedList
+from reamber.osu.OsuSv import OsuSv
+
+
+@list_props(OsuSv)
+class OsuSvList(TimedList[OsuSv]):
+
+    @staticmethod
+    def read(strings: List[str]) -> OsuSvList:
+        return OsuSvList(pd.DataFrame(
+            [OsuSv.read_string(s, as_dict=True) for s in
+             strings]) if strings else [])
+
+    def write(self) -> List[str]:
+        return [h.write_string() for h in self]
```

### Comparing `reamber-0.1.7/reamber/osu/lists/notes/OsuHitList.py` & `reamber-0.1.8/reamber/osu/lists/notes/OsuHitList.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-from __future__ import annotations
-
-from typing import List
-
-import pandas as pd
-
-from reamber.base.Property import list_props
-from reamber.base.lists.notes.HitList import HitList
-from reamber.osu.OsuHit import OsuHit
-from reamber.osu.lists.notes.OsuNoteList import OsuNoteList
-
-
-@list_props(OsuHit)
-class OsuHitList(HitList[OsuHit], OsuNoteList[OsuHit]):
-
-    @staticmethod
-    def read(strings: List[str], keys: int) -> OsuHitList:
-        return OsuHitList(pd.DataFrame(
-            [OsuHit.read_string(s, keys, True) for s in
-             strings]) if strings else [])
-
-    def write(self, keys: int) -> List[str]:
-        return [h.write_string(keys) for h in self]
-
-    @staticmethod
-    def read_editor_string(s: str) -> OsuHitList:
-        """Reads an editor string, must be of the correct format.
-
-        Notes:
-            i.e. XX:XX:XXX(OFFSET|COL, OFFSET|COL, ...) -
-        """
-        return OsuHitList(
-            [OsuHit(offset=float(note.split("|")[0]),
-                    column=int(note.split("|")[1]))
-             for note in s[s.find("(") + 1: s.find(")")].split(",")]
-        )
+from __future__ import annotations
+
+from typing import List
+
+import pandas as pd
+
+from reamber.base.Property import list_props
+from reamber.base.lists.notes.HitList import HitList
+from reamber.osu.OsuHit import OsuHit
+from reamber.osu.lists.notes.OsuNoteList import OsuNoteList
+
+
+@list_props(OsuHit)
+class OsuHitList(HitList[OsuHit], OsuNoteList[OsuHit]):
+
+    @staticmethod
+    def read(strings: List[str], keys: int) -> OsuHitList:
+        return OsuHitList(pd.DataFrame(
+            [OsuHit.read_string(s, keys, True) for s in
+             strings]) if strings else [])
+
+    def write(self, keys: int) -> List[str]:
+        return [h.write_string(keys) for h in self]
+
+    @staticmethod
+    def read_editor_string(s: str) -> OsuHitList:
+        """Reads an editor string, must be of the correct format.
+
+        Notes:
+            i.e. XX:XX:XXX(OFFSET|COL, OFFSET|COL, ...) -
+        """
+        return OsuHitList(
+            [OsuHit(offset=float(note.split("|")[0]),
+                    column=int(note.split("|")[1]))
+             for note in s[s.find("(") + 1: s.find(")")].split(",")]
+        )
```

### Comparing `reamber-0.1.7/reamber/osu/lists/notes/OsuHoldList.py` & `reamber-0.1.8/reamber/osu/lists/notes/OsuHoldList.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-from __future__ import annotations
-
-from typing import List
-
-import pandas as pd
-
-from reamber.base.Property import list_props
-from reamber.base.lists.notes.HoldList import HoldList
-from reamber.osu.OsuHold import OsuHold
-from reamber.osu.lists.notes.OsuNoteList import OsuNoteList
-
-
-@list_props(OsuHold)
-class OsuHoldList(HoldList[OsuHold], OsuNoteList[OsuHold]):
-
-    @staticmethod
-    def read(strings: List[str], keys: int) -> OsuHoldList:
-        return OsuHoldList(pd.DataFrame(
-            [OsuHold.read_string(s, keys, as_dict=True) for s in
-             strings]) if strings else [])
-
-    def write(self, keys: int) -> List[str]:
-        return [h.write_string(keys) for h in self]
+from __future__ import annotations
+
+from typing import List
+
+import pandas as pd
+
+from reamber.base.Property import list_props
+from reamber.base.lists.notes.HoldList import HoldList
+from reamber.osu.OsuHold import OsuHold
+from reamber.osu.lists.notes.OsuNoteList import OsuNoteList
+
+
+@list_props(OsuHold)
+class OsuHoldList(HoldList[OsuHold], OsuNoteList[OsuHold]):
+
+    @staticmethod
+    def read(strings: List[str], keys: int) -> OsuHoldList:
+        return OsuHoldList(pd.DataFrame(
+            [OsuHold.read_string(s, keys, as_dict=True) for s in
+             strings]) if strings else [])
+
+    def write(self, keys: int) -> List[str]:
+        return [h.write_string(keys) for h in self]
```

### Comparing `reamber-0.1.7/reamber/osu/lists/notes/OsuNoteList.pyi` & `reamber-0.1.8/reamber/osu/lists/notes/OsuNoteList.pyi`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-from __future__ import annotations
-
-from abc import ABC
-from typing import TypeVar
-
-import pandas as pd
-
-from reamber.base.lists.notes.NoteList import NoteList
-
-Item = TypeVar('Item')
-
-
-class OsuNoteList(NoteList[Item], ABC):
-    @property
-    def hitsound_set(self) -> pd.Series: ...
-
-    @hitsound_set.setter
-    def hitsound_set(self, val) -> None: ...
-
-    @property
-    def sample_set(self) -> pd.Series: ...
-
-    @sample_set.setter
-    def sample_set(self, val) -> None: ...
-
-    @property
-    def addition_set(self) -> pd.Series: ...
-
-    @addition_set.setter
-    def addition_set(self, val) -> None: ...
-
-    @property
-    def custom_set(self) -> pd.Series: ...
-
-    @custom_set.setter
-    def custom_set(self, val) -> None: ...
-
-    @property
-    def volume(self) -> pd.Series: ...
-
-    @volume.setter
-    def volume(self, val) -> None: ...
-
-    @property
-    def hitsound_file(self) -> pd.Series: ...
-
-    @hitsound_file.setter
-    def hitsound_file(self, val) -> None: ...
+from __future__ import annotations
+
+from abc import ABC
+from typing import TypeVar
+
+import pandas as pd
+
+from reamber.base.lists.notes.NoteList import NoteList
+
+Item = TypeVar('Item')
+
+
+class OsuNoteList(NoteList[Item], ABC):
+    @property
+    def hitsound_set(self) -> pd.Series: ...
+
+    @hitsound_set.setter
+    def hitsound_set(self, val) -> None: ...
+
+    @property
+    def sample_set(self) -> pd.Series: ...
+
+    @sample_set.setter
+    def sample_set(self, val) -> None: ...
+
+    @property
+    def addition_set(self) -> pd.Series: ...
+
+    @addition_set.setter
+    def addition_set(self, val) -> None: ...
+
+    @property
+    def custom_set(self) -> pd.Series: ...
+
+    @custom_set.setter
+    def custom_set(self, val) -> None: ...
+
+    @property
+    def volume(self) -> pd.Series: ...
+
+    @volume.setter
+    def volume(self, val) -> None: ...
+
+    @property
+    def hitsound_file(self) -> pd.Series: ...
+
+    @hitsound_file.setter
+    def hitsound_file(self, val) -> None: ...
```

### Comparing `reamber-0.1.7/reamber/quaver/QuaHit.py` & `reamber-0.1.8/reamber/quaver/QuaHit.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from typing import Dict, List, Any
-
-import pandas as pd
-
-from reamber.base import item_props
-from reamber.base.Hit import Hit
-from reamber.quaver.QuaNoteMeta import QuaNoteMeta
-
-
-@item_props()
-class QuaHit(Hit, QuaNoteMeta):
-
-    def __init__(self,
-                 offset: float,
-                 column: int,
-                 keysounds: List[str],
-                 **kwargs):
-        super().__init__(
-            offset=offset, column=column, keysounds=keysounds, **kwargs
-        )
-
-    def to_yaml(self) -> Dict[str, Any]:
-        return dict(StartTime=int(self.offset), Lane=int(self.column + 1),
-                    KeySounds=self.keysounds)
-
-    @staticmethod
-    def from_yaml(d: Dict[str, Any]):
-        s = pd.Series(dict(offset=d.get('StartTime', 0),
-                           column=d.get('Lane', 1) - 1,
-                           keysounds=d.get('KeySounds', [])))
-        return QuaHit.from_series(s)
+from typing import Dict, List, Any
+
+import pandas as pd
+
+from reamber.base import item_props
+from reamber.base.Hit import Hit
+from reamber.quaver.QuaNoteMeta import QuaNoteMeta
+
+
+@item_props()
+class QuaHit(Hit, QuaNoteMeta):
+
+    def __init__(self,
+                 offset: float,
+                 column: int,
+                 keysounds: List[str],
+                 **kwargs):
+        super().__init__(
+            offset=offset, column=column, keysounds=keysounds, **kwargs
+        )
+
+    def to_yaml(self) -> Dict[str, Any]:
+        return dict(StartTime=int(self.offset), Lane=int(self.column + 1),
+                    KeySounds=self.keysounds)
+
+    @staticmethod
+    def from_yaml(d: Dict[str, Any]):
+        s = pd.Series(dict(offset=d.get('StartTime', 0),
+                           column=d.get('Lane', 1) - 1,
+                           keysounds=d.get('KeySounds', [])))
+        return QuaHit.from_series(s)
```

### Comparing `reamber-0.1.7/reamber/quaver/QuaMapMeta.py` & `reamber-0.1.8/reamber/quaver/QuaMapMeta.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from dataclasses import dataclass, field
-from typing import List, Dict
-
-
-class QuaMapMode:
-    """Lists all available Quaver Key modes.
-
-    Though easy to implement the rest of the keys here
-    """
-
-    KEYS_4: str = "Keys4"
-    KEYS_7: str = "Keys7"
-    KEYS_8: str = "Keys8"  # Not officially supported yet.
-
-    @staticmethod
-    def get_keys(s: str) -> int:
-        """Gets the keys as integer instead of string"""
-        if s == QuaMapMode.KEYS_4:
-            return 4
-        elif s == QuaMapMode.KEYS_7:
-            return 7
-        elif s == QuaMapMode.KEYS_8:
-            return 8
-        else:
-            return -1
-
-    @staticmethod
-    def get_mode(i: int) -> str:
-        """Gets the keys as string instead of int"""
-        if i == 4:
-            return QuaMapMode.KEYS_4
-        elif i == 7:
-            return QuaMapMode.KEYS_7
-        elif i == 8:
-            return QuaMapMode.KEYS_8
-        else:
-            return ""
-
-
-@dataclass
-class QuaMapMeta:
-    audio_file: str = ""
-    song_preview_time: int = 0
-    background_file: str = ""
-    banner_file: str = ""
-    genre: str = ""
-    bpm_does_not_affect_scroll_velocity: bool = True
-    initial_scroll_velocity: float = ""
-    has_scratch_key: bool = True
-    map_id: int = -1
-    map_set_id: int = -1
-    mode: str = QuaMapMode.KEYS_4
-    title: str = ""
-    artist: str = ""
-    source: str = ""
-    tags: List[str] = field(default_factory=lambda: [])
-    creator: str = ""
-    difficulty_name: str = ""
-    description: str = ""
-    editor_layers: List[str] = field(default_factory=lambda: [])
-    custom_audio_samples: List[str] = field(default_factory=lambda: [])
-    sound_effects: List[str] = field(default_factory=lambda: [])
-
-    def _read_metadata(self, d: Dict):
-        """Reads the Metadata dict from the YAML read"""
-        self.audio_file = d.get('AudioFile', self.audio_file)
-        self.song_preview_time = d.get('SongPreviewTime',
-                                       self.song_preview_time)
-        self.background_file = d.get('BackgroundFile', self.background_file)
-        self.banner_file = d.get('BannerFile', self.banner_file)
-        self.genre = d.get('Genre', self.genre)
-        self.bpm_does_not_affect_scroll_velocity = d.get(
-            'BPMDoesNotAffectScrollVelocity',
-            self.bpm_does_not_affect_scroll_velocity)
-        self.initial_scroll_velocity = d.get('InitialScrollVelocity',
-                                             self.initial_scroll_velocity)
-        self.has_scratch_key = d.get('HasScratchKey', self.has_scratch_key)
-        self.map_id = d.get('MapId', self.map_id)
-        self.map_set_id = d.get('MapSetId', self.map_set_id)
-        self.mode = d.get('Mode', self.mode)
-        self.title = d.get('Title', self.title)
-        self.artist = d.get('Artist', self.artist)
-        self.source = d.get('Source', self.source)
-        # Tags are sep by " "
-        self.tags = [i for i in d.get('Tags', "").split(" ") if i]
-        self.creator = d.get('Creator', self.creator)
-        self.difficulty_name = d.get('DifficultyName', self.difficulty_name)
-        self.description = d.get('Description', self.description)
-        self.editor_layers = d.get('EditorLayers', self.editor_layers)
-        self.custom_audio_samples = d.get('CustomAudioSamples',
-                                          self.custom_audio_samples)
-        self.sound_effects = d.get('SoundEffects', self.sound_effects)
-
-    def _write_meta(self) -> Dict:
-        """Writes the metadata as a Dictionary and returns it"""
-        return {
-            'AudioFile': self.audio_file,
-            'SongPreviewTime': self.song_preview_time,
-            'BackgroundFile': self.background_file,
-            'BannerFile': self.banner_file,
-            'Genre': self.genre,
-            'BPMDoesNotAffectScrollVelocity':
-                self.bpm_does_not_affect_scroll_velocity,
-            'InitialScrollVelocity': self.initial_scroll_velocity,
-            'HasScratchKey': self.has_scratch_key,
-            'MapId': self.map_id,
-            'MapSetId': self.map_set_id,
-            'Mode': self.mode,
-            'Title': self.title,
-            'Artist': self.artist,
-            'Source': self.source,
-            'Tags': " ".join(self.tags),
-            'Creator': self.creator,
-            'DifficultyName': self.difficulty_name,
-            'Description': self.description,
-            'EditorLayers': self.editor_layers,
-            'CustomAudioSamples': self.custom_audio_samples,
-            'SoundEffects': self.sound_effects,
-        }
+from dataclasses import dataclass, field
+from typing import List, Dict
+
+
+class QuaMapMode:
+    """Lists all available Quaver Key modes.
+
+    Though easy to implement the rest of the keys here
+    """
+
+    KEYS_4: str = "Keys4"
+    KEYS_7: str = "Keys7"
+    KEYS_8: str = "Keys8"  # Not officially supported yet.
+
+    @staticmethod
+    def get_keys(s: str) -> int:
+        """Gets the keys as integer instead of string"""
+        if s == QuaMapMode.KEYS_4:
+            return 4
+        elif s == QuaMapMode.KEYS_7:
+            return 7
+        elif s == QuaMapMode.KEYS_8:
+            return 8
+        else:
+            return -1
+
+    @staticmethod
+    def get_mode(i: int) -> str:
+        """Gets the keys as string instead of int"""
+        if i == 4:
+            return QuaMapMode.KEYS_4
+        elif i == 7:
+            return QuaMapMode.KEYS_7
+        elif i == 8:
+            return QuaMapMode.KEYS_8
+        else:
+            return ""
+
+
+@dataclass
+class QuaMapMeta:
+    audio_file: str = ""
+    song_preview_time: int = 0
+    background_file: str = ""
+    banner_file: str = ""
+    genre: str = ""
+    bpm_does_not_affect_scroll_velocity: bool = True
+    initial_scroll_velocity: float = ""
+    has_scratch_key: bool = True
+    map_id: int = -1
+    map_set_id: int = -1
+    mode: str = QuaMapMode.KEYS_4
+    title: str = ""
+    artist: str = ""
+    source: str = ""
+    tags: List[str] = field(default_factory=lambda: [])
+    creator: str = ""
+    difficulty_name: str = ""
+    description: str = ""
+    editor_layers: List[str] = field(default_factory=lambda: [])
+    custom_audio_samples: List[str] = field(default_factory=lambda: [])
+    sound_effects: List[str] = field(default_factory=lambda: [])
+
+    def _read_metadata(self, d: Dict):
+        """Reads the Metadata dict from the YAML read"""
+        self.audio_file = d.get('AudioFile', self.audio_file)
+        self.song_preview_time = d.get('SongPreviewTime',
+                                       self.song_preview_time)
+        self.background_file = d.get('BackgroundFile', self.background_file)
+        self.banner_file = d.get('BannerFile', self.banner_file)
+        self.genre = d.get('Genre', self.genre)
+        self.bpm_does_not_affect_scroll_velocity = d.get(
+            'BPMDoesNotAffectScrollVelocity',
+            self.bpm_does_not_affect_scroll_velocity)
+        self.initial_scroll_velocity = d.get('InitialScrollVelocity',
+                                             self.initial_scroll_velocity)
+        self.has_scratch_key = d.get('HasScratchKey', self.has_scratch_key)
+        self.map_id = d.get('MapId', self.map_id)
+        self.map_set_id = d.get('MapSetId', self.map_set_id)
+        self.mode = d.get('Mode', self.mode)
+        self.title = d.get('Title', self.title)
+        self.artist = d.get('Artist', self.artist)
+        self.source = d.get('Source', self.source)
+        # Tags are sep by " "
+        self.tags = [i for i in d.get('Tags', "").split(" ") if i]
+        self.creator = d.get('Creator', self.creator)
+        self.difficulty_name = d.get('DifficultyName', self.difficulty_name)
+        self.description = d.get('Description', self.description)
+        self.editor_layers = d.get('EditorLayers', self.editor_layers)
+        self.custom_audio_samples = d.get('CustomAudioSamples',
+                                          self.custom_audio_samples)
+        self.sound_effects = d.get('SoundEffects', self.sound_effects)
+
+    def _write_meta(self) -> Dict:
+        """Writes the metadata as a Dictionary and returns it"""
+        return {
+            'AudioFile': self.audio_file,
+            'SongPreviewTime': self.song_preview_time,
+            'BackgroundFile': self.background_file,
+            'BannerFile': self.banner_file,
+            'Genre': self.genre,
+            'BPMDoesNotAffectScrollVelocity':
+                self.bpm_does_not_affect_scroll_velocity,
+            'InitialScrollVelocity': self.initial_scroll_velocity,
+            'HasScratchKey': self.has_scratch_key,
+            'MapId': self.map_id,
+            'MapSetId': self.map_set_id,
+            'Mode': self.mode,
+            'Title': self.title,
+            'Artist': self.artist,
+            'Source': self.source,
+            'Tags': " ".join(self.tags),
+            'Creator': self.creator,
+            'DifficultyName': self.difficulty_name,
+            'Description': self.description,
+            'EditorLayers': self.editor_layers,
+            'CustomAudioSamples': self.custom_audio_samples,
+            'SoundEffects': self.sound_effects,
+        }
```

### Comparing `reamber-0.1.7/reamber/quaver/lists/QuaBpmList.py` & `reamber-0.1.8/reamber/quaver/lists/QuaBpmList.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from __future__ import annotations
-
-from typing import List, Dict, Any
-
-import pandas as pd
-
-from reamber.base.Property import list_props
-from reamber.base.lists.BpmList import BpmList
-from reamber.quaver.QuaBpm import QuaBpm
-from reamber.quaver.lists.QuaTimedList import QuaTimedList
-
-
-@list_props(QuaBpm)
-class QuaBpmList(BpmList[QuaBpm], QuaTimedList[QuaBpm]):
-
-    @staticmethod
-    def from_yaml(dicts: List[Dict[str, Any]]) -> QuaBpmList:
-        df = pd.DataFrame(dicts)
-        df = df.rename(dict(StartTime='offset', Bpm='bpm'), axis=1)
-        df = df.reindex(df.columns.union(['offset', 'bpm'], sort=False),
-                        axis=1)
-        df.offset = df.offset.fillna(0)
-        df.bpm = df.bpm.fillna(120)
-        return QuaBpmList(df)
-
-    def to_yaml(self):
-        return self.df.astype(dict(offset=int, bpm=float)) \
-            .rename(dict(offset='StartTime', bpm='Bpm'), axis=1) \
-            .drop('metronome', axis=1).to_dict('records')
+from __future__ import annotations
+
+from typing import List, Dict, Any
+
+import pandas as pd
+
+from reamber.base.Property import list_props
+from reamber.base.lists.BpmList import BpmList
+from reamber.quaver.QuaBpm import QuaBpm
+from reamber.quaver.lists.QuaTimedList import QuaTimedList
+
+
+@list_props(QuaBpm)
+class QuaBpmList(BpmList[QuaBpm], QuaTimedList[QuaBpm]):
+
+    @staticmethod
+    def from_yaml(dicts: List[Dict[str, Any]]) -> QuaBpmList:
+        df = pd.DataFrame(dicts)
+        df = df.rename(dict(StartTime='offset', Bpm='bpm'), axis=1)
+        df = df.reindex(df.columns.union(['offset', 'bpm'], sort=False),
+                        axis=1)
+        df.offset = df.offset.fillna(0)
+        df.bpm = df.bpm.fillna(120)
+        return QuaBpmList(df)
+
+    def to_yaml(self):
+        return self.df.astype(dict(offset=int, bpm=float)) \
+            .rename(dict(offset='StartTime', bpm='Bpm'), axis=1) \
+            .drop('metronome', axis=1).to_dict('records')
```

### Comparing `reamber-0.1.7/reamber/quaver/lists/QuaSvList.py` & `reamber-0.1.8/reamber/quaver/lists/QuaSvList.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from __future__ import annotations
-
-from typing import List, Dict, Any
-
-import pandas as pd
-
-from reamber.base.Property import list_props
-from reamber.base.lists.TimedList import TimedList
-from reamber.quaver.QuaSv import QuaSv
-
-
-@list_props(QuaSv)
-class QuaSvList(TimedList[QuaSv]):
-    @staticmethod
-    def from_yaml(dicts: List[Dict[str, Any]]) -> QuaSvList:
-        df = pd.DataFrame(dicts)
-        df = df.rename(dict(StartTime='offset', Multiplier='multiplier'),
-                       axis=1)
-        df = df.reindex(df.columns.union(['offset', 'multiplier'], sort=False),
-                        axis=1)
-        df.offset = df.offset.fillna(0)
-        df.multiplier = df.multiplier.fillna(120)
-        return QuaSvList(df)
-
-    def to_yaml(self):
-        df = self.df.copy()
-        return (
-            df.astype(
-                dict(offset=int, multiplier=float)
-            ).rename(
-                dict(offset='StartTime', multiplier='Multiplier'), axis=1
-            ).to_dict('records')
-        )
+from __future__ import annotations
+
+from typing import List, Dict, Any
+
+import pandas as pd
+
+from reamber.base.Property import list_props
+from reamber.base.lists.TimedList import TimedList
+from reamber.quaver.QuaSv import QuaSv
+
+
+@list_props(QuaSv)
+class QuaSvList(TimedList[QuaSv]):
+    @staticmethod
+    def from_yaml(dicts: List[Dict[str, Any]]) -> QuaSvList:
+        df = pd.DataFrame(dicts)
+        df = df.rename(dict(StartTime='offset', Multiplier='multiplier'),
+                       axis=1)
+        df = df.reindex(df.columns.union(['offset', 'multiplier'], sort=False),
+                        axis=1)
+        df.offset = df.offset.fillna(0)
+        df.multiplier = df.multiplier.fillna(120)
+        return QuaSvList(df)
+
+    def to_yaml(self):
+        df = self.df.copy()
+        return (
+            df.astype(
+                dict(offset=int, multiplier=float)
+            ).rename(
+                dict(offset='StartTime', multiplier='Multiplier'), axis=1
+            ).to_dict('records')
+        )
```

### Comparing `reamber-0.1.7/reamber/quaver/lists/notes/QuaNoteList.py` & `reamber-0.1.8/reamber/quaver/lists/notes/QuaNoteList.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from __future__ import annotations
-
-from abc import ABC, abstractmethod
-from typing import TypeVar, List, Dict, Any
-
-from reamber.base.Property import list_props
-from reamber.base.lists.notes.NoteList import NoteList
-from reamber.quaver.QuaHit import QuaHit
-from reamber.quaver.lists.QuaTimedList import QuaTimedList
-
-Item = TypeVar('Item', bound=QuaHit)
-
-@list_props(QuaHit)
-class QuaNoteList(NoteList[Item], QuaTimedList[Item], ABC):
-
-    @staticmethod
-    @abstractmethod
-    def from_yaml(dicts: List[Dict[str, Any]]) -> QuaNoteList: ...
+from __future__ import annotations
+
+from abc import ABC, abstractmethod
+from typing import TypeVar, List, Dict, Any
+
+from reamber.base.Property import list_props
+from reamber.base.lists.notes.NoteList import NoteList
+from reamber.quaver.QuaHit import QuaHit
+from reamber.quaver.lists.QuaTimedList import QuaTimedList
+
+Item = TypeVar('Item', bound=QuaHit)
+
+@list_props(QuaHit)
+class QuaNoteList(NoteList[Item], QuaTimedList[Item], ABC):
+
+    @staticmethod
+    @abstractmethod
+    def from_yaml(dicts: List[Dict[str, Any]]) -> QuaNoteList: ...
```

### Comparing `reamber-0.1.7/reamber/quaver/lists/notes/QuaNoteList.pyi` & `reamber-0.1.8/reamber/quaver/lists/notes/QuaNoteList.pyi`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from __future__ import annotations
-
-from abc import ABC, abstractmethod
-from typing import TypeVar, List, Dict, Any
-
-import pandas as pd
-
-from reamber.base.lists.notes.NoteList import NoteList
-from reamber.quaver import QuaHit
-from reamber.quaver.lists import QuaTimedList
-
-Item = TypeVar('Item', bound=QuaHit)
-
-class QuaNoteList(NoteList[Item], QuaTimedList[Item], ABC):
-    def to_yaml(self) -> List[Dict[str, Any]]: ...
-
-    @staticmethod
-    @abstractmethod
-    def from_yaml(dicts: List[Dict[str, Any]]) -> QuaNoteList: ...
+from __future__ import annotations
+
+from abc import ABC, abstractmethod
+from typing import TypeVar, List, Dict, Any
+
+import pandas as pd
+
+from reamber.base.lists.notes.NoteList import NoteList
+from reamber.quaver import QuaHit
+from reamber.quaver.lists import QuaTimedList
+
+Item = TypeVar('Item', bound=QuaHit)
+
+class QuaNoteList(NoteList[Item], QuaTimedList[Item], ABC):
+    def to_yaml(self) -> List[Dict[str, Any]]: ...
+
+    @staticmethod
+    @abstractmethod
+    def from_yaml(dicts: List[Dict[str, Any]]) -> QuaNoteList: ...
```

### Comparing `reamber-0.1.7/reamber/sm/SMMap.pyi` & `reamber-0.1.8/reamber/sm/SMMap.pyi`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-from __future__ import annotations
-
-from dataclasses import dataclass, field
-from typing import List, Dict, TYPE_CHECKING
-
-from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
-from reamber.base.Map import Map
-from reamber.base.lists import TimedList
-from reamber.sm.SMMapMeta import SMMapMeta
-from reamber.sm.lists.SMBpmList import SMBpmList
-from reamber.sm.lists.SMStopList import SMStopList
-from reamber.sm.lists.notes import SMNoteList, SMHitList, SMHoldList, \
-    SMFakeList, SMLiftList, SMKeySoundList, \
-    SMMineList, SMRollList
-
-if TYPE_CHECKING:
-    from reamber.sm.SMMapSet import SMMapSet
-
-@dataclass
-class SMMap(Map[SMNoteList, SMHitList, SMHoldList, SMBpmList], SMMapMeta):
-    objs: Dict[str, TimedList] = field(init=False,
-                                       default_factory=...)
-
-    @property
-    def fakes(self) -> SMFakeList: ...
-
-    @fakes.setter
-    def fakes(self, val) -> None: ...
-
-    @property
-    def lifts(self) -> SMLiftList: ...
-
-    @lifts.setter
-    def lifts(self, val) -> None: ...
-
-    @property
-    def keysounds(self) -> SMKeySoundList: ...
-
-    @keysounds.setter
-    def keysounds(self, val) -> None: ...
-
-    @property
-    def mines(self) -> SMMineList: ...
-
-    @mines.setter
-    def mines(self, val) -> None: ...
-
-    @property
-    def rolls(self) -> SMRollList: ...
-
-    @rolls.setter
-    def rolls(self, val) -> None: ...
-
-    @property
-    def stops(self) -> SMStopList: ...
-
-    @stops.setter
-    def stops(self, val) -> None: ...
-
-    @staticmethod
-    def read(s: str,
-             bcs_s: List[BpmChangeSnap],
-             initial_offset: float,
-             stops: SMStopList) -> SMMap: ...
-
-    def write(self) -> List[str]: ...
-
-    def _read_notes(self,
-                    note_data: str,
-                    initial_offset: float,
-                    bcs_s: List[BpmChangeSnap],
-                    stops: SMStopList): ...
-
-    # noinspection PyMethodOverriding
-    def metadata(self, s: SMMapSet, unicode=True) -> str: ...
-
-    # noinspection PyMethodOverriding
-    def describe(self, s: SMMapSet, rounding: int = 2,
-                 unicode: bool = False) -> str: ...
-
-    def rate(self, by: float, inplace: bool = False) -> SMMap: ...
+from __future__ import annotations
+
+from dataclasses import dataclass, field
+from typing import List, Dict, TYPE_CHECKING
+
+from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
+from reamber.base.Map import Map
+from reamber.base.lists import TimedList
+from reamber.sm.SMMapMeta import SMMapMeta
+from reamber.sm.lists.SMBpmList import SMBpmList
+from reamber.sm.lists.SMStopList import SMStopList
+from reamber.sm.lists.notes import SMNoteList, SMHitList, SMHoldList, \
+    SMFakeList, SMLiftList, SMKeySoundList, \
+    SMMineList, SMRollList
+
+if TYPE_CHECKING:
+    from reamber.sm.SMMapSet import SMMapSet
+
+@dataclass
+class SMMap(Map[SMNoteList, SMHitList, SMHoldList, SMBpmList], SMMapMeta):
+    objs: Dict[str, TimedList] = field(init=False,
+                                       default_factory=...)
+
+    @property
+    def fakes(self) -> SMFakeList: ...
+
+    @fakes.setter
+    def fakes(self, val) -> None: ...
+
+    @property
+    def lifts(self) -> SMLiftList: ...
+
+    @lifts.setter
+    def lifts(self, val) -> None: ...
+
+    @property
+    def keysounds(self) -> SMKeySoundList: ...
+
+    @keysounds.setter
+    def keysounds(self, val) -> None: ...
+
+    @property
+    def mines(self) -> SMMineList: ...
+
+    @mines.setter
+    def mines(self, val) -> None: ...
+
+    @property
+    def rolls(self) -> SMRollList: ...
+
+    @rolls.setter
+    def rolls(self, val) -> None: ...
+
+    @property
+    def stops(self) -> SMStopList: ...
+
+    @stops.setter
+    def stops(self, val) -> None: ...
+
+    @staticmethod
+    def read(s: str,
+             bcs_s: List[BpmChangeSnap],
+             initial_offset: float,
+             stops: SMStopList) -> SMMap: ...
+
+    def write(self) -> List[str]: ...
+
+    def _read_notes(self,
+                    note_data: str,
+                    initial_offset: float,
+                    bcs_s: List[BpmChangeSnap],
+                    stops: SMStopList): ...
+
+    # noinspection PyMethodOverriding
+    def metadata(self, s: SMMapSet, unicode=True) -> str: ...
+
+    # noinspection PyMethodOverriding
+    def describe(self, s: SMMapSet, rounding: int = 2,
+                 unicode: bool = False) -> str: ...
+
+    def rate(self, by: float, inplace: bool = False) -> SMMap: ...
```

### Comparing `reamber-0.1.7/reamber/sm/SMMapMeta.py` & `reamber-0.1.8/reamber/sm/SMMapMeta.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,163 +1,163 @@
-from dataclasses import dataclass, field
-from typing import List
-
-
-class SMMapDifficulty:
-    BEGINNER: str = "Beginner"
-    EASY: str = "Easy"
-    MEDIUM: str = "Medium"
-    HARD: str = "Hard"
-    CHALLENGE: str = "Challenge"
-    EDIT: str = "Edit"
-
-
-class SMMapChartTypes:
-    # Full Description in CHART_TYPES
-    DANCE_SINGLE: str = "dance-single"  # Your normal 4 panel dance mode.
-    DANCE_DOUBLE: str = "dance-double"  # Both P1 & P2 pads are used for one player.
-    DANCE_SOLO: str = "dance-solo"  # 4-panel, except with additional top-left and top-right columns.
-    DANCE_COUPLE: str = "dance-couple"  # One chart, but P1 & P2 have different steps.
-    DANCE_THREEPANEL: str = "dance-threepanel"  # Like Single, but the down arrow isn't used.
-    DANCE_ROUTINE: str = "dance-routine"  # It's like Couple in that it's for two players
-    PUMP_SINGLE: str = "pump-single"  # Single, 5-panel pad.
-    PUMP_HALFDOUBLE: str = "pump-halfdouble"  # Uses only six panels in the middle of the pad
-    PUMP_DOUBLE: str = "pump-double"  # Same as Dance.
-    PUMP_COUPLE: str = "pump-couple"  # Same as Dance.
-    PUMP_ROUTINE: str = "pump-routine"  # Same as Dance.
-    KB7_SINGLE: str = "kb7-single"  # Standard kb7 layout
-    KICKBOX_HUMAN: str = "kickbox-human"  # 4key
-    KICKBOX_QUADARM: str = "kickbox-quadarm"  # 4key
-    KICKBOX_INSECT: str = "kickbox-insect"  # 6key
-    KICKBOX_ARACHNID: str = "kickbox-arachnid"  # 8key
-    PARA_SINGLE: str = "para-single"  # 5key.
-    BM_SINGLE5: str = "bm-single5"  # 5+1key game mode
-    BM_VERSUS5: str = "bm-versus5"  # Unknown, might be the beat equivalent to Couple?
-    BM_DOUBLE5: str = "bm-double5"  # Both sides are used.
-    BM_SINGLE7: str = "bm-single7"  # 7+1key game mode
-    BM_DOUBLE7: str = "bm-double7"  # Both sides are used.
-    BM_VERSUS7: str = "bm-versus7"  # Unknown (see versus5)
-    EZ2_SINGLE: str = "ez2-single"  # 1 pad
-    EZ2_DOUBLE: str = "ez2-double"  # 2 pad
-    EZ2_REAL: str = "ez2-real"  # Divides the hand sensors into upper and lower halves.
-    PNM_FIVE: str = "pnm-five"  # 5key game mode.
-    PNM_NINE: str = "pnm-nine"  # 9key game mode.
-    TECHNO_SINGLE4: str = "techno-single4"  # Identical to dance_single
-    TECHNO_SINGLE5: str = "techno-single5"  # Identical to pump_single
-    TECHNO_SINGLE8: str = "techno-single8"  # eight panels are used: ⬅⬇⬆➡↙↘↗↖
-    TECHNO_DOUBLE4: str = "techno-double4"  # Identical to dance_double
-    TECHNO_DOUBLE5: str = "techno-double5"  # Identical to pump_double
-    TECHNO_DOUBLE8: str = "techno-double8"  # 16 panels (doubles)
-    DS3DDX_SINGLE: str = "ds3ddx-single"  # 4key + 4hand...
-    MANIAX_SINGLE: str = "maniax-single"  # 4key
-    MANIAX_DOUBLE: str = "maniax-double"  # 8key
-
-    @staticmethod
-    def get_keys(chart: str) -> int or None:
-        if chart == SMMapChartTypes.DANCE_SINGLE:
-            return 4
-        elif chart == SMMapChartTypes.DANCE_DOUBLE:
-            return 8
-        elif chart == SMMapChartTypes.DANCE_SOLO:
-            return 6
-        elif chart == SMMapChartTypes.DANCE_COUPLE:
-            return 4
-        elif chart == SMMapChartTypes.DANCE_THREEPANEL:
-            return 3
-        elif chart == SMMapChartTypes.DANCE_ROUTINE:
-            return 8
-        elif chart == SMMapChartTypes.PUMP_SINGLE:
-            return None
-        elif chart == SMMapChartTypes.PUMP_HALFDOUBLE:
-            return None
-        elif chart == SMMapChartTypes.PUMP_DOUBLE:
-            return None
-        elif chart == SMMapChartTypes.PUMP_COUPLE:
-            return None
-        elif chart == SMMapChartTypes.PUMP_ROUTINE:
-            return None
-        elif chart == SMMapChartTypes.KB7_SINGLE:
-            return 7
-        elif chart == SMMapChartTypes.KICKBOX_HUMAN:
-            return None
-        elif chart == SMMapChartTypes.KICKBOX_QUADARM:
-            return None
-        elif chart == SMMapChartTypes.KICKBOX_INSECT:
-            return None
-        elif chart == SMMapChartTypes.KICKBOX_ARACHNID:
-            return None
-        elif chart == SMMapChartTypes.PARA_SINGLE:
-            return None
-        elif chart == SMMapChartTypes.BM_SINGLE5:
-            return None
-        elif chart == SMMapChartTypes.BM_VERSUS5:
-            return None
-        elif chart == SMMapChartTypes.BM_DOUBLE5:
-            return None
-        elif chart == SMMapChartTypes.BM_SINGLE7:
-            return None
-        elif chart == SMMapChartTypes.BM_DOUBLE7:
-            return None
-        elif chart == SMMapChartTypes.BM_VERSUS7:
-            return None
-        elif chart == SMMapChartTypes.EZ2_SINGLE:
-            return None
-        elif chart == SMMapChartTypes.EZ2_DOUBLE:
-            return None
-        elif chart == SMMapChartTypes.EZ2_REAL:
-            return None
-        elif chart == SMMapChartTypes.PNM_FIVE:
-            return None
-        elif chart == SMMapChartTypes.PNM_NINE:
-            return None
-        elif chart == SMMapChartTypes.TECHNO_SINGLE4:
-            return None
-        elif chart == SMMapChartTypes.TECHNO_SINGLE5:
-            return None
-        elif chart == SMMapChartTypes.TECHNO_SINGLE8:
-            return None
-        elif chart == SMMapChartTypes.TECHNO_DOUBLE4:
-            return None
-        elif chart == SMMapChartTypes.TECHNO_DOUBLE5:
-            return None
-        elif chart == SMMapChartTypes.TECHNO_DOUBLE8:
-            return None
-        elif chart == SMMapChartTypes.DS3DDX_SINGLE:
-            return None
-        elif chart == SMMapChartTypes.MANIAX_SINGLE:
-            return None
-        elif chart == SMMapChartTypes.MANIAX_DOUBLE:
-            return None
-
-    @staticmethod
-    def get_type(keys: int) -> str or None:
-        """Attempts to find the most suitable chart Type"""
-
-        if keys == 4:
-            return SMMapChartTypes.DANCE_SINGLE
-        elif keys == 8:
-            return SMMapChartTypes.DANCE_DOUBLE
-        elif keys == 6:
-            return SMMapChartTypes.DANCE_SOLO
-        elif keys == 3:
-            return SMMapChartTypes.DANCE_THREEPANEL
-        elif keys == 7:
-            return SMMapChartTypes.KB7_SINGLE
-        else:
-            return ""
-
-
-@dataclass
-class SMMapMeta:
-    chart_type: str = SMMapChartTypes.DANCE_SINGLE
-    description: str = ""
-    difficulty: str = SMMapDifficulty.EASY
-    difficulty_val: int = 1
-    groove_radar: List[float] = \
-        field(default_factory=lambda: [0.0, 0.0, 0.0, 0.0, 0.0])
-
-    def _read_note_metadata(self, metadata: List[str]):
-        self.chart_type = metadata[0].strip()
-        self.description = metadata[1].strip()
-        self.difficulty = metadata[2].strip()
-        self.difficulty_val = int(metadata[3].strip())
-        self.groove_radar = [float(x) for x in metadata[4].strip().split(",")]
+from dataclasses import dataclass, field
+from typing import List
+
+
+class SMMapDifficulty:
+    BEGINNER: str = "Beginner"
+    EASY: str = "Easy"
+    MEDIUM: str = "Medium"
+    HARD: str = "Hard"
+    CHALLENGE: str = "Challenge"
+    EDIT: str = "Edit"
+
+
+class SMMapChartTypes:
+    # Full Description in CHART_TYPES
+    DANCE_SINGLE: str = "dance-single"  # Your normal 4 panel dance mode.
+    DANCE_DOUBLE: str = "dance-double"  # Both P1 & P2 pads are used for one player.
+    DANCE_SOLO: str = "dance-solo"  # 4-panel, except with additional top-left and top-right columns.
+    DANCE_COUPLE: str = "dance-couple"  # One chart, but P1 & P2 have different steps.
+    DANCE_THREEPANEL: str = "dance-threepanel"  # Like Single, but the down arrow isn't used.
+    DANCE_ROUTINE: str = "dance-routine"  # It's like Couple in that it's for two players
+    PUMP_SINGLE: str = "pump-single"  # Single, 5-panel pad.
+    PUMP_HALFDOUBLE: str = "pump-halfdouble"  # Uses only six panels in the middle of the pad
+    PUMP_DOUBLE: str = "pump-double"  # Same as Dance.
+    PUMP_COUPLE: str = "pump-couple"  # Same as Dance.
+    PUMP_ROUTINE: str = "pump-routine"  # Same as Dance.
+    KB7_SINGLE: str = "kb7-single"  # Standard kb7 layout
+    KICKBOX_HUMAN: str = "kickbox-human"  # 4key
+    KICKBOX_QUADARM: str = "kickbox-quadarm"  # 4key
+    KICKBOX_INSECT: str = "kickbox-insect"  # 6key
+    KICKBOX_ARACHNID: str = "kickbox-arachnid"  # 8key
+    PARA_SINGLE: str = "para-single"  # 5key.
+    BM_SINGLE5: str = "bm-single5"  # 5+1key game mode
+    BM_VERSUS5: str = "bm-versus5"  # Unknown, might be the beat equivalent to Couple?
+    BM_DOUBLE5: str = "bm-double5"  # Both sides are used.
+    BM_SINGLE7: str = "bm-single7"  # 7+1key game mode
+    BM_DOUBLE7: str = "bm-double7"  # Both sides are used.
+    BM_VERSUS7: str = "bm-versus7"  # Unknown (see versus5)
+    EZ2_SINGLE: str = "ez2-single"  # 1 pad
+    EZ2_DOUBLE: str = "ez2-double"  # 2 pad
+    EZ2_REAL: str = "ez2-real"  # Divides the hand sensors into upper and lower halves.
+    PNM_FIVE: str = "pnm-five"  # 5key game mode.
+    PNM_NINE: str = "pnm-nine"  # 9key game mode.
+    TECHNO_SINGLE4: str = "techno-single4"  # Identical to dance_single
+    TECHNO_SINGLE5: str = "techno-single5"  # Identical to pump_single
+    TECHNO_SINGLE8: str = "techno-single8"  # eight panels are used: ⬅⬇⬆➡↙↘↗↖
+    TECHNO_DOUBLE4: str = "techno-double4"  # Identical to dance_double
+    TECHNO_DOUBLE5: str = "techno-double5"  # Identical to pump_double
+    TECHNO_DOUBLE8: str = "techno-double8"  # 16 panels (doubles)
+    DS3DDX_SINGLE: str = "ds3ddx-single"  # 4key + 4hand...
+    MANIAX_SINGLE: str = "maniax-single"  # 4key
+    MANIAX_DOUBLE: str = "maniax-double"  # 8key
+
+    @staticmethod
+    def get_keys(chart: str) -> int or None:
+        if chart == SMMapChartTypes.DANCE_SINGLE:
+            return 4
+        elif chart == SMMapChartTypes.DANCE_DOUBLE:
+            return 8
+        elif chart == SMMapChartTypes.DANCE_SOLO:
+            return 6
+        elif chart == SMMapChartTypes.DANCE_COUPLE:
+            return 4
+        elif chart == SMMapChartTypes.DANCE_THREEPANEL:
+            return 3
+        elif chart == SMMapChartTypes.DANCE_ROUTINE:
+            return 8
+        elif chart == SMMapChartTypes.PUMP_SINGLE:
+            return None
+        elif chart == SMMapChartTypes.PUMP_HALFDOUBLE:
+            return None
+        elif chart == SMMapChartTypes.PUMP_DOUBLE:
+            return None
+        elif chart == SMMapChartTypes.PUMP_COUPLE:
+            return None
+        elif chart == SMMapChartTypes.PUMP_ROUTINE:
+            return None
+        elif chart == SMMapChartTypes.KB7_SINGLE:
+            return 7
+        elif chart == SMMapChartTypes.KICKBOX_HUMAN:
+            return None
+        elif chart == SMMapChartTypes.KICKBOX_QUADARM:
+            return None
+        elif chart == SMMapChartTypes.KICKBOX_INSECT:
+            return None
+        elif chart == SMMapChartTypes.KICKBOX_ARACHNID:
+            return None
+        elif chart == SMMapChartTypes.PARA_SINGLE:
+            return None
+        elif chart == SMMapChartTypes.BM_SINGLE5:
+            return None
+        elif chart == SMMapChartTypes.BM_VERSUS5:
+            return None
+        elif chart == SMMapChartTypes.BM_DOUBLE5:
+            return None
+        elif chart == SMMapChartTypes.BM_SINGLE7:
+            return None
+        elif chart == SMMapChartTypes.BM_DOUBLE7:
+            return None
+        elif chart == SMMapChartTypes.BM_VERSUS7:
+            return None
+        elif chart == SMMapChartTypes.EZ2_SINGLE:
+            return None
+        elif chart == SMMapChartTypes.EZ2_DOUBLE:
+            return None
+        elif chart == SMMapChartTypes.EZ2_REAL:
+            return None
+        elif chart == SMMapChartTypes.PNM_FIVE:
+            return None
+        elif chart == SMMapChartTypes.PNM_NINE:
+            return None
+        elif chart == SMMapChartTypes.TECHNO_SINGLE4:
+            return None
+        elif chart == SMMapChartTypes.TECHNO_SINGLE5:
+            return None
+        elif chart == SMMapChartTypes.TECHNO_SINGLE8:
+            return None
+        elif chart == SMMapChartTypes.TECHNO_DOUBLE4:
+            return None
+        elif chart == SMMapChartTypes.TECHNO_DOUBLE5:
+            return None
+        elif chart == SMMapChartTypes.TECHNO_DOUBLE8:
+            return None
+        elif chart == SMMapChartTypes.DS3DDX_SINGLE:
+            return None
+        elif chart == SMMapChartTypes.MANIAX_SINGLE:
+            return None
+        elif chart == SMMapChartTypes.MANIAX_DOUBLE:
+            return None
+
+    @staticmethod
+    def get_type(keys: int) -> str or None:
+        """Attempts to find the most suitable chart Type"""
+
+        if keys == 4:
+            return SMMapChartTypes.DANCE_SINGLE
+        elif keys == 8:
+            return SMMapChartTypes.DANCE_DOUBLE
+        elif keys == 6:
+            return SMMapChartTypes.DANCE_SOLO
+        elif keys == 3:
+            return SMMapChartTypes.DANCE_THREEPANEL
+        elif keys == 7:
+            return SMMapChartTypes.KB7_SINGLE
+        else:
+            return ""
+
+
+@dataclass
+class SMMapMeta:
+    chart_type: str = SMMapChartTypes.DANCE_SINGLE
+    description: str = ""
+    difficulty: str = SMMapDifficulty.EASY
+    difficulty_val: int = 1
+    groove_radar: List[float] = \
+        field(default_factory=lambda: [0.0, 0.0, 0.0, 0.0, 0.0])
+
+    def _read_note_metadata(self, metadata: List[str]):
+        self.chart_type = metadata[0].strip()
+        self.description = metadata[1].strip()
+        self.difficulty = metadata[2].strip()
+        self.difficulty_val = int(metadata[3].strip())
+        self.groove_radar = [float(x) for x in metadata[4].strip().split(",")]
```

### Comparing `reamber-0.1.7/reamber/sm/SMMapSet.py` & `reamber-0.1.8/reamber/sm/SMMapSet.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,74 +1,75 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from typing import List
-
-from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
-from reamber.base.MapSet import MapSet
-from reamber.sm.SMMap import SMMap
-from reamber.sm.SMMapSetMeta import SMMapSetMeta
-from reamber.sm.lists import SMStopList
-from reamber.sm.lists.SMBpmList import SMBpmList
-from reamber.sm.lists.notes import SMNoteList, SMHitList, SMHoldList
-
-
-@dataclass
-class SMMapSet(MapSet[SMNoteList, SMHitList, SMHoldList, SMBpmList, SMMap],
-               SMMapSetMeta):
-
-    @staticmethod
-    def read(lines: str | list[str]) -> SMMapSet:
-        """Reads a .sm file"""
-        ms = SMMapSet()
-        lines = "\n".join(lines) if isinstance(lines, list) else lines
-        file_spl = [i.strip() for i in lines.split(";")]
-        metadata = []
-        maps = []
-        for token in file_spl:
-            if "#NOTES:" in token:
-                maps.append(token)
-            else:
-                metadata.append(token)
-
-        bcs_s, stops = ms._read_metadata(metadata)
-        ms._read_maps(maps=maps, bcs_s=bcs_s, stops=stops)
-        return ms
-
-    @staticmethod
-    def read_file(file_path: str) -> SMMapSet:
-        """Reads a .sm file as a Mapset"""
-        with open(file_path, "r", encoding="utf8") as f:
-            file = f.read()
-
-        return SMMapSet.read(file)
-
-    def write(self) -> str:
-        """Writes as a list[str] """
-        m = self._write_metadata()
-
-        for map in self.maps:
-            m.extend(map.write())
-        return "\n".join(m)
-
-    def write_file(self, file_path: str):
-        """Writes the file to file_path specified"""
-        with open(file_path, "w+", encoding="utf8") as f:
-            f.write(self.write())
-
-    def _read_maps(self,
-                   maps: List[str],
-                   bcs_s: List[BpmChangeSnap],
-                   stops: SMStopList):
-        self.maps = [
-            SMMap.read(s=map_str, bcs_s=bcs_s, stops=stops,
-                       initial_offset=self.offset)
-            for map_str in maps
-        ]
-
-    def rate(self, by: float) -> SMMapSet:
-        """Changes the rate of the map"""
-        sms = super(SMMapSet, self).rate(by=by)
-        sms.sample_start /= by
-        sms.sample_length /= by
-
-        return sms
+from __future__ import annotations
+
+from dataclasses import dataclass
+from pathlib import Path
+from typing import List
+
+from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
+from reamber.base.MapSet import MapSet
+from reamber.sm.SMMap import SMMap
+from reamber.sm.SMMapSetMeta import SMMapSetMeta
+from reamber.sm.lists import SMStopList
+from reamber.sm.lists.SMBpmList import SMBpmList
+from reamber.sm.lists.notes import SMNoteList, SMHitList, SMHoldList
+
+
+@dataclass
+class SMMapSet(MapSet[SMNoteList, SMHitList, SMHoldList, SMBpmList, SMMap],
+               SMMapSetMeta):
+
+    @staticmethod
+    def read(lines: str | list[str]) -> SMMapSet:
+        """Reads a .sm file"""
+        ms = SMMapSet()
+        lines = "\n".join(lines) if isinstance(lines, list) else lines
+        file_spl = [i.strip() for i in lines.split(";")]
+        metadata = []
+        maps = []
+        for token in file_spl:
+            if "#NOTES:" in token:
+                maps.append(token)
+            else:
+                metadata.append(token)
+
+        bcs_s, stops = ms._read_metadata(metadata)
+        ms._read_maps(maps=maps, bcs_s=bcs_s, stops=stops)
+        return ms
+
+    @staticmethod
+    def read_file(file_path: str | Path) -> SMMapSet:
+        """Reads a .sm file as a Mapset"""
+        with open(file_path, "r", encoding="utf8") as f:
+            file = f.read()
+
+        return SMMapSet.read(file)
+
+    def write(self) -> str:
+        """Writes as a list[str] """
+        m = self._write_metadata()
+
+        for map in self.maps:
+            m.extend(map.write())
+        return "\n".join(m)
+
+    def write_file(self, file_path: str | Path):
+        """Writes the file to file_path specified"""
+        with open(file_path, "w+", encoding="utf8") as f:
+            f.write(self.write())
+
+    def _read_maps(self,
+                   maps: List[str],
+                   bcs_s: List[BpmChangeSnap],
+                   stops: SMStopList):
+        self.maps = [
+            SMMap.read(s=map_str, bcs_s=bcs_s, stops=stops,
+                       initial_offset=self.offset)
+            for map_str in maps
+        ]
+
+    def rate(self, by: float) -> SMMapSet:
+        """Changes the rate of the map"""
+        sms = super(SMMapSet, self).rate(by=by)
+        sms.sample_start /= by
+        sms.sample_length /= by
+
+        return sms
```

### Comparing `reamber-0.1.7/reamber/sm/SMMapSet.pyi` & `reamber-0.1.8/reamber/sm/SMMapSet.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from __future__ import annotations
-
-from dataclasses import dataclass
-from typing import List, Iterator
-
-from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
-from reamber.base.MapSet import MapSet
-from reamber.sm.SMMap import SMMap
-from reamber.sm.SMMapSetMeta import SMMapSetMeta
-from reamber.sm.lists import SMStopList
-from reamber.sm.lists.SMBpmList import SMBpmList
-from reamber.sm.lists.notes import SMNoteList, SMHitList, SMHoldList
-
-
-@dataclass
-class SMMapSet(MapSet[SMNoteList, SMHitList, SMHoldList, SMBpmList, SMMap],
-               SMMapSetMeta):
-
-    def __iter__(self) -> Iterator[SMMap]: ...
-
-    @staticmethod
-    def read(lines: str | List[str]) -> SMMapSet: ...
-
-    @staticmethod
-    def read_file(file_path: str) -> SMMapSet: ...
-
-    def write(self) -> str: ...
-
-    def write_file(self, file_path: str): ...
-
-    def _read_maps(self, maps: List[str],
-                   bcs_s: List[BpmChangeSnap],
-                   stops: SMStopList): ...
-
-    # noinspection PyTypeChecker
-    def rate(self, by: float) -> SMMapSet: ...
+from __future__ import annotations
+
+from dataclasses import dataclass
+from pathlib import Path
+from typing import List, Iterator
+
+from reamber.algorithms.timing.utils.BpmChangeSnap import BpmChangeSnap
+from reamber.base.MapSet import MapSet
+from reamber.sm.SMMap import SMMap
+from reamber.sm.SMMapSetMeta import SMMapSetMeta
+from reamber.sm.lists import SMStopList
+from reamber.sm.lists.SMBpmList import SMBpmList
+from reamber.sm.lists.notes import SMNoteList, SMHitList, SMHoldList
+
+
+@dataclass
+class SMMapSet(MapSet[SMNoteList, SMHitList, SMHoldList, SMBpmList, SMMap],
+               SMMapSetMeta):
+
+    def __iter__(self) -> Iterator[SMMap]: ...
+
+    @staticmethod
+    def read(lines: str | List[str]) -> SMMapSet: ...
+
+    @staticmethod
+    def read_file(file_path: str | Path) -> SMMapSet: ...
+
+    def write(self) -> str: ...
+
+    def write_file(self, file_path: str | Path): ...
+
+    def _read_maps(self, maps: List[str],
+                   bcs_s: List[BpmChangeSnap],
+                   stops: SMStopList): ...
+
+    # noinspection PyTypeChecker
+    def rate(self, by: float) -> SMMapSet: ...
```

### Comparing `reamber-0.1.7/reamber/sm/__init__.py` & `reamber-0.1.8/reamber/sm/__init__.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from reamber.sm.SMBpm import SMBpm
-from reamber.sm.SMFake import SMFake
-from reamber.sm.SMHit import SMHit
-from reamber.sm.SMHold import SMHold
-from reamber.sm.SMKeySound import SMKeySound
-from reamber.sm.SMLift import SMLift
-from reamber.sm.SMMap import SMMap
-from reamber.sm.SMMapMeta import SMMapMeta
-from reamber.sm.SMMapSet import SMMapSet
-from reamber.sm.SMMapSetMeta import SMMapSetMeta
-from reamber.sm.SMMine import SMMine
-from reamber.sm.SMRoll import SMRoll
-from reamber.sm.SMStop import SMStop
-
-__all__ = ['SMMapSetMeta', 'SMRoll', 'SMHold', 'SMMapSet', 'SMMine', 'SMLift',
-           'SMMapMeta', 'SMKeySound', 'SMFake', 'SMStop', 'SMHit', 'SMMap',
-           'SMBpm']
+from reamber.sm.SMBpm import SMBpm
+from reamber.sm.SMFake import SMFake
+from reamber.sm.SMHit import SMHit
+from reamber.sm.SMHold import SMHold
+from reamber.sm.SMKeySound import SMKeySound
+from reamber.sm.SMLift import SMLift
+from reamber.sm.SMMap import SMMap
+from reamber.sm.SMMapMeta import SMMapMeta
+from reamber.sm.SMMapSet import SMMapSet
+from reamber.sm.SMMapSetMeta import SMMapSetMeta
+from reamber.sm.SMMine import SMMine
+from reamber.sm.SMRoll import SMRoll
+from reamber.sm.SMStop import SMStop
+
+__all__ = ['SMMapSetMeta', 'SMRoll', 'SMHold', 'SMMapSet', 'SMMine', 'SMLift',
+           'SMMapMeta', 'SMKeySound', 'SMFake', 'SMStop', 'SMHit', 'SMMap',
+           'SMBpm']
```

### Comparing `reamber-0.1.7/reamber/sm/lists/notes/__init__.py` & `reamber-0.1.8/reamber/sm/lists/notes/__init__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from reamber.sm.lists.notes.SMFakeList import SMFakeList
-from reamber.sm.lists.notes.SMHitList import SMHitList
-from reamber.sm.lists.notes.SMHoldList import SMHoldList
-from reamber.sm.lists.notes.SMKeySoundList import SMKeySoundList
-from reamber.sm.lists.notes.SMLiftList import SMLiftList
-from reamber.sm.lists.notes.SMMineList import SMMineList
-from reamber.sm.lists.notes.SMNoteList import SMNoteList
-from reamber.sm.lists.notes.SMRollList import SMRollList
-
-__all__ = ['SMRollList', 'SMHoldList', 'SMFakeList', 'SMNoteList',
-           'SMKeySoundList', 'SMHitList', 'SMLiftList', 'SMMineList']
+from reamber.sm.lists.notes.SMFakeList import SMFakeList
+from reamber.sm.lists.notes.SMHitList import SMHitList
+from reamber.sm.lists.notes.SMHoldList import SMHoldList
+from reamber.sm.lists.notes.SMKeySoundList import SMKeySoundList
+from reamber.sm.lists.notes.SMLiftList import SMLiftList
+from reamber.sm.lists.notes.SMMineList import SMMineList
+from reamber.sm.lists.notes.SMNoteList import SMNoteList
+from reamber.sm.lists.notes.SMRollList import SMRollList
+
+__all__ = ['SMRollList', 'SMHoldList', 'SMFakeList', 'SMNoteList',
+           'SMKeySoundList', 'SMHitList', 'SMLiftList', 'SMMineList']
```

