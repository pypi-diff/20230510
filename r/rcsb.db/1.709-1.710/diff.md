# Comparing `tmp/rcsb.db-1.709.tar.gz` & `tmp/rcsb.db-1.710.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.db-1.709.tar", last modified: Wed Apr 26 21:10:27 2023, max compression
+gzip compressed data, was "rcsb.db-1.710.tar", last modified: Tue May  9 22:05:52 2023, max compression
```

## Comparing `rcsb.db-1.709.tar` & `rcsb.db-1.710.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.259347 rcsb.db-1.709/
--rw-r--r--   0 vsts      (1001) docker     (122)    29680 2023-04-26 20:49:04.000000 rcsb.db-1.709/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-04-26 20:49:04.000000 rcsb.db-1.709/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-04-26 20:49:04.000000 rcsb.db-1.709/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-04-26 21:10:27.259347 rcsb.db-1.709/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    26823 2023-04-26 20:49:04.000000 rcsb.db-1.709/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.235347 rcsb.db-1.709/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.239347 rcsb.db-1.709/rcsb/db/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.239347 rcsb.db-1.709/rcsb/db/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)     9528 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/ETLExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7657 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/RepoHoldingsEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22767 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/RepoLoadExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10064 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/RepoScanExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11316 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/SchemaUpdateExec.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8774 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/SequenceClustersEtlWorker.py
--rw-r--r--   0 vsts      (1001) docker     (122)      155 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cli/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.243347 rcsb.db-1.709/rcsb/db/cockroach/
--rw-r--r--   0 vsts      (1001) docker     (122)     9848 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cockroach/CockroachDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9605 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cockroach/CockroachDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5467 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cockroach/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/cockroach/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.243347 rcsb.db-1.709/rcsb/db/crate/
--rw-r--r--   0 vsts      (1001) docker     (122)     5142 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/crate/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7987 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/crate/CrateDbLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9990 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/crate/CrateDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/crate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.247347 rcsb.db-1.709/rcsb/db/define/
--rw-r--r--   0 vsts      (1001) docker     (122)    33223 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/ContentDefinition.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4169 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/DataTypeApiProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15211 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/DataTypeApplicationInfo.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4188 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/DataTypeInstanceInfo.py
--rw-r--r--   0 vsts      (1001) docker     (122)    34868 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/SchemaDefAccess.py
--rw-r--r--   0 vsts      (1001) docker     (122)    60184 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/SchemaDefBuild.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/define/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.247347 rcsb.db-1.709/rcsb/db/helpers/
--rw-r--r--   0 vsts      (1001) docker     (122)    16974 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/helpers/ContentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    34236 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/helpers/DocumentDefinitionHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/helpers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1611 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/helpers/r.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.251347 rcsb.db-1.709/rcsb/db/mongo/
--rw-r--r--   0 vsts      (1001) docker     (122)     5655 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4938 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15040 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/DocumentLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)    23696 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/MongoDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)    69158 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/PdbxLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mongo/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.251347 rcsb.db-1.709/rcsb/db/mysql/
--rw-r--r--   0 vsts      (1001) docker     (122)     2832 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/Connection.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4258 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/ConnectionBase.py
--rw-r--r--   0 vsts      (1001) docker     (122)    18626 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/MyDbAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12211 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/MyDbUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5169 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/MysqlSchemaImporter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19129 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/SchemaDefLoader.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/mysql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.255347 rcsb.db-1.709/rcsb/db/processors/
--rw-r--r--   0 vsts      (1001) docker     (122)     7467 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/ClusterDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5081 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/DataExchangeStatus.py
--rw-r--r--   0 vsts      (1001) docker     (122)    19485 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/DataTransformFactory.py
--rw-r--r--   0 vsts      (1001) docker     (122)    31322 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/RepoHoldingsDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)    40786 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/SchemaDefDataPrep.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26654 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/SchemaDefReShape.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/processors/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.255347 rcsb.db-1.709/rcsb/db/sql/
--rw-r--r--   0 vsts      (1001) docker     (122)    23627 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/sql/QueryDirectives.py
--rw-r--r--   0 vsts      (1001) docker     (122)    40731 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/sql/SqlGen.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/sql/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.259347 rcsb.db-1.709/rcsb/db/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)     2696 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/CaseNormalizedDict.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12446 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/PdbxSchemaMapReader.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3683 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/ProvenanceProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)    22110 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/SchemaProvider.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1353 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/TextUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2172 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/TimeUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1614 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/makePathList.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1055 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/utils/unescape.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.259347 rcsb.db-1.709/rcsb/db/wf/
--rw-r--r--   0 vsts      (1001) docker     (122)    11438 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/wf/RepoLoadWorkflow.py
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-04-26 20:49:04.000000 rcsb.db-1.709/rcsb/db/wf/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-26 21:10:27.239347 rcsb.db-1.709/rcsb.db.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      209 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-26 20:54:12.000000 rcsb.db-1.709/rcsb.db.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      437 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-04-26 21:10:27.000000 rcsb.db-1.709/rcsb.db.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-04-26 20:49:04.000000 rcsb.db-1.709/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-04-26 21:10:27.259347 rcsb.db-1.709/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2876 2023-04-26 20:49:04.000000 rcsb.db-1.709/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.238813 rcsb.db-1.710/
+-rw-r--r--   0 vsts      (1001) docker     (122)    29779 2023-05-09 21:43:20.000000 rcsb.db-1.710/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-05-09 21:43:20.000000 rcsb.db-1.710/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)      100 2023-05-09 21:43:20.000000 rcsb.db-1.710/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-05-09 22:05:52.238813 rcsb.db-1.710/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    26823 2023-05-09 21:43:20.000000 rcsb.db-1.710/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.226813 rcsb.db-1.710/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.226813 rcsb.db-1.710/rcsb/db/
+-rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9528 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/ETLExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7657 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/RepoHoldingsEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22767 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/RepoLoadExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10064 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/RepoScanExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11316 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/SchemaUpdateExec.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8774 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/SequenceClustersEtlWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      155 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cli/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/cockroach/
+-rw-r--r--   0 vsts      (1001) docker     (122)     9848 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cockroach/CockroachDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9605 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cockroach/CockroachDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5467 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cockroach/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/cockroach/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/crate/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5142 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/crate/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7987 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/crate/CrateDbLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9990 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/crate/CrateDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/crate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/define/
+-rw-r--r--   0 vsts      (1001) docker     (122)    33223 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/ContentDefinition.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4169 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/DataTypeApiProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15211 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/DataTypeApplicationInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4188 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/DataTypeInstanceInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    34868 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/SchemaDefAccess.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    60184 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/SchemaDefBuild.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/define/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.230814 rcsb.db-1.710/rcsb/db/helpers/
+-rw-r--r--   0 vsts      (1001) docker     (122)    16974 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/helpers/ContentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    34236 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/helpers/DocumentDefinitionHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/helpers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1611 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/helpers/r.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.234814 rcsb.db-1.710/rcsb/db/mongo/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5655 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4938 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15040 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/DocumentLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    23696 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/MongoDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    71183 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/PdbxLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mongo/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.234814 rcsb.db-1.710/rcsb/db/mysql/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2832 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/Connection.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4258 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/ConnectionBase.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    18626 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/MyDbAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12211 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/MyDbUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5169 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/MysqlSchemaImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19129 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/SchemaDefLoader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/mysql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.234814 rcsb.db-1.710/rcsb/db/processors/
+-rw-r--r--   0 vsts      (1001) docker     (122)     7467 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/ClusterDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5081 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/DataExchangeStatus.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    19485 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/DataTransformFactory.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    31322 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/RepoHoldingsDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7596 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    40786 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/SchemaDefDataPrep.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26654 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/SchemaDefReShape.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/processors/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.234814 rcsb.db-1.710/rcsb/db/sql/
+-rw-r--r--   0 vsts      (1001) docker     (122)    23627 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/sql/QueryDirectives.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    40731 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/sql/SqlGen.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/sql/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.238813 rcsb.db-1.710/rcsb/db/utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2696 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/CaseNormalizedDict.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12446 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/PdbxSchemaMapReader.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3683 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/ProvenanceProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22110 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/SchemaProvider.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1353 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/TextUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2172 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/TimeUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1614 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/makePathList.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1055 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/utils/unescape.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.238813 rcsb.db-1.710/rcsb/db/wf/
+-rw-r--r--   0 vsts      (1001) docker     (122)    11438 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/wf/RepoLoadWorkflow.py
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-09 21:43:20.000000 rcsb.db-1.710/rcsb/db/wf/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 22:05:52.226813 rcsb.db-1.710/rcsb.db.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    27551 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2298 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      209 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 21:52:46.000000 rcsb.db-1.710/rcsb.db.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)      437 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-05-09 22:05:52.000000 rcsb.db-1.710/rcsb.db.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      513 2023-05-09 21:43:20.000000 rcsb.db-1.710/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-05-09 22:05:52.238813 rcsb.db-1.710/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (122)     2876 2023-05-09 21:43:20.000000 rcsb.db-1.710/setup.py
```

### Comparing `rcsb.db-1.709/HISTORY.txt` & `rcsb.db-1.710/HISTORY.txt`

 * *Files 2% similar despite different names*

```diff
@@ -340,7 +340,8 @@
  23-Dec-2022  V1.703 Configuration changes to support tox 4
  26-Jan-2023  V1.704 Update MA_DICT_LOCATOR path in exdb-config-example.yml and add uchar5 to DataTypeApplicationInfo.py
  30-Jan-2023  V1.705 Update requirements (pin SQLAlchemy)
  14-Feb-2023  V1.706 Updates to PdbxLoader and RepoLoadWorkflow to support resumability of core data loading tasks
  22-Feb-2023  V1.707 Updates to PdbxLoader to use case-sensitivity for brute force document purge
  06-Apr-2023  V1.708 Add support for entity_id_list cifType in DataTypeApplicationInfo
  26-Apr-2023  V1.709 Fix document pre-purge regex during load, and add regexPurge flag to control running that step
+  8-May-2023  V1.710 Fix error handling in PdbxLoader to cause failure when documents fail to load
```

### Comparing `rcsb.db-1.709/LICENSE` & `rcsb.db-1.710/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/PKG-INFO` & `rcsb.db-1.710/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.709
+Version: 1.710
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.db-1.709/README.md` & `rcsb.db-1.710/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/cli/ETLExec.py` & `rcsb.db-1.710/rcsb/db/cli/ETLExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/cli/RepoHoldingsEtlWorker.py` & `rcsb.db-1.710/rcsb/db/cli/RepoHoldingsEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/cli/RepoLoadExec.py` & `rcsb.db-1.710/rcsb/db/cli/RepoLoadExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/cli/RepoScanExec.py` & `rcsb.db-1.710/rcsb/db/cli/RepoScanExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/cli/SchemaUpdateExec.py` & `rcsb.db-1.710/rcsb/db/cli/SchemaUpdateExec.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/cli/SequenceClustersEtlWorker.py` & `rcsb.db-1.710/rcsb/db/cli/SequenceClustersEtlWorker.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/cockroach/CockroachDbLoader.py` & `rcsb.db-1.710/rcsb/db/cockroach/CockroachDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/cockroach/CockroachDbUtil.py` & `rcsb.db-1.710/rcsb/db/cockroach/CockroachDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/cockroach/Connection.py` & `rcsb.db-1.710/rcsb/db/cockroach/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/crate/Connection.py` & `rcsb.db-1.710/rcsb/db/crate/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/crate/CrateDbLoader.py` & `rcsb.db-1.710/rcsb/db/crate/CrateDbLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/crate/CrateDbUtil.py` & `rcsb.db-1.710/rcsb/db/crate/CrateDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/define/ContentDefinition.py` & `rcsb.db-1.710/rcsb/db/define/ContentDefinition.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/define/DataTypeApiProvider.py` & `rcsb.db-1.710/rcsb/db/define/DataTypeApiProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/define/DataTypeApplicationInfo.py` & `rcsb.db-1.710/rcsb/db/define/DataTypeApplicationInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/define/DataTypeInstanceInfo.py` & `rcsb.db-1.710/rcsb/db/define/DataTypeInstanceInfo.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/define/SchemaDefAccess.py` & `rcsb.db-1.710/rcsb/db/define/SchemaDefAccess.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/define/SchemaDefBuild.py` & `rcsb.db-1.710/rcsb/db/define/SchemaDefBuild.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/helpers/ContentDefinitionHelper.py` & `rcsb.db-1.710/rcsb/db/helpers/ContentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/helpers/DocumentDefinitionHelper.py` & `rcsb.db-1.710/rcsb/db/helpers/DocumentDefinitionHelper.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/helpers/r.py` & `rcsb.db-1.710/rcsb/db/helpers/r.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mongo/Connection.py` & `rcsb.db-1.710/rcsb/db/mongo/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mongo/ConnectionBase.py` & `rcsb.db-1.710/rcsb/db/mongo/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mongo/DocumentLoader.py` & `rcsb.db-1.710/rcsb/db/mongo/DocumentLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mongo/MongoDbUtil.py` & `rcsb.db-1.710/rcsb/db/mongo/MongoDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mongo/PdbxLoader.py` & `rcsb.db-1.710/rcsb/db/mongo/PdbxLoader.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 #     18-May-2020 jdw  Add brute force document purging for loadType=replace
 #     10-Jan-2022 dwp  Add support for loading id code lists for mongo PdbxLoader() (preliminary)
 #     29-Apr-2022 dwp  Add support for handling and making use of internal computed-model identifiers
 #     29-Jun-2022 dwp  Remove uneeded custom-support for computed-model identifiers (will now use the internally-modified entry.id)
 #      2-Feb-2023 dwp  Add removeAndRecreateDbCollections method for wiping a database without involving any data loading
 #     22-Feb-2023 dwp  Use case-sensitivity for brute force document purge
 #     26-Apr-2023 dwp  Fix regex document purge, and add regexPurge flag to control running that step (with default set to skip it)
+#      8-May-2023 dwp  Fix error handling in PdbxLoader to cause failure when documents fail to load
 #
 ##
 """
 Worker methods for loading primary data content following mapping conventions in external schema definitions.
 
 """
 
@@ -716,16 +717,21 @@
                 #       like how it's done for other pieces of code (e.g., see rcsb.utils.insilico3d.ModelReorganizer).
                 # pdbxLoaderWorker = PdbxLoaderWorker(self.__cfgOb, self.__rpP, self.__dmh, self.__resourceName)
                 #
                 mpu = MultiProcUtil(verbose=True)
                 mpu.setWorkingDir(self.__cachePath)
                 mpu.setOptions(optionsD=optD)
                 mpu.set(workerObj=self, workerMethod="loadWorker")
-                ok, failListT, _, _ = mpu.runMulti(dataList=subList, numProc=numProc, numResults=1, chunkSize=chunkSize)
+                ok, failListT, resultList, _ = mpu.runMulti(dataList=subList, numProc=numProc, numResults=1, chunkSize=chunkSize)
                 logger.info("Completed outer subtask %d of %d (status=%r) length %d failures (%d) %r", ii + 1, len(subLists), ok, len(subList), len(failListT), failListT)
+                # Note: 'resultList' is the 'retList' returned from loadWorker method below, BUT NESTED WITHIN AN ADDITIONAL LIST!
+                #       (i.e., resultList = [retList])
+                if len(resultList) > 0:
+                    logger.debug("resultList[0] length (%d), first item: %r", len(resultList[0]), resultList[0][0])
+                #
                 failList.extend(failListT)
             failList = list(set(failList))
             if failList:
                 logger.info("Full failed path list %r", failList)
             #
             failedPathList = self.__rpP.getLocatorPaths(failList, locatorIndex=0)
             if failedFilePath and failedPathList:
@@ -769,14 +775,26 @@
     def loadWorker(self, dataList, procName, optionsD, workingDir):
         """Multi-proc worker method for MongoDb loading -
 
         successList, resultList, diagList=workerFunc(runList=nextList,procName, optionsD, workingDir)
 
         locatorObjList -> containerList -> docList  ->|LOAD|<-  .... return success locatorObjList
 
+        Args:
+            dataList (list): list of items to work on
+            procName (str): worker process name
+            optionsD (dict): dictionary of additional options that worker can access
+            workingDir (str): path to working directory
+
+        Returns:
+            successList (list): list of input data items that were successfully processed (items must be in same format as input
+                                dataList in order for MultiProc to properly generate failList returned by mpu.runMulti(...))
+            retList (list): list of all processed items, both successes and failures (items can be in any format you wish, e.g., (cId, locatorObj, ok));
+                            Note that this gets assigned to the variable, 'resultList', returned by mpu.runMulti(...) call above
+            diagList (list): list of unique diagnostics (usually left empty)
         """
         try:
             startTime = self.__begin(message=procName)
             # Recover common options
             styleType = optionsD["styleType"]
             filterType = optionsD["filterType"]
             readBackCheck = optionsD["readBackCheck"]
@@ -798,14 +816,18 @@
             # -------------------------------------------
             # -- Create map of  cIdD{ container identifier} =  locatorObj
             #
             collectionName = None
             cIdD = {}
             cNameL = []
             containerList = []
+            successList = []
+            retList = []
+            diagList = []
+
             for locatorObj in dataList:
                 # JDW
                 cL = self.__rpP.getContainerList([locatorObj])
                 if cL:
                     cNameL.append(cL[0].getName().upper().strip())
                     cId = cL[0].getName() if useNameFlag else cL[0].getProp("uid")
                     cIdD[cId] = locatorObj
@@ -927,56 +949,59 @@
                     cardinalIdFailS.add(dId[0])
                     failContainerIdS.add(cId)
                     locObj = cIdD[cId]
                     failPathList.extend(self.__rpP.getLocatorPaths([locObj], locatorIndex=0))
                 failPathList = list(set(failPathList))
                 #
                 if failPathList:
-                    logger.debug("%s %s/%s worker load failures %r", procName, databaseName, collectionName, [os.path.basename(pth) for pth in failPathList if pth is not None])
+                    logger.error("%s %s/%s worker load failures %r", procName, databaseName, collectionName, [os.path.basename(pth) for pth in failPathList if pth is not None])
                 if rejectPathList:
                     logger.debug("%s %s/%s worker load rejected %r", procName, databaseName, collectionName, [os.path.basename(pth) for pth in rejectPathList])
             #
             # -------------------------
             #  failContainerIdS = set()
             #  rejectContainerIdS = set()
             #
             #  cIdD[cId] = locatorObj
             # ----
-            retList = [locatorObj for cId, locatorObj in cIdD.items() if cId not in failContainerIdS]
-            logger.debug("%s %s load worker returns  successes %d rejects %d failures %d", procName, databaseName, len(retList), len(rejectContainerIdS), len(failContainerIdS))
+            successList = [locatorObj for cId, locatorObj in cIdD.items() if cId not in failContainerIdS]
+            logger.debug("%s %s load worker returns  successes %d rejects %d failures %d", procName, databaseName, len(successList), len(rejectContainerIdS), len(failContainerIdS))
+            #
+            retList = [(cId, locatorObj, True) for cId, locatorObj in cIdD.items() if cId not in failContainerIdS]
+            retList += [(cId, locatorObj, False) for cId, locatorObj in cIdD.items() if cId in failContainerIdS]
             #
             if cardinalIdFailS:
                 # remove all collection objects related to a load failure
                 for collectionName in collectionNameList:
                     logger.info("Purging all objects from %s for failed ids: %r", collectionName, cardinalIdFailS)
                     ok = self.__purgeDocuments(databaseName, collectionName, list(cardinalIdFailS))
             #
             ok = len(failContainerIdS) == 0
             self.__end(startTime, procName + " with status " + str(ok))
-            return retList, [], []
+
+            return successList, retList, diagList
 
         except Exception as e:
             # logger.error("Failing for dataList %r" % dataList)
             logger.exception("Failing with %s", str(e))
 
         return [], [], []
 
     # -------------- -------------- -------------- -------------- -------------- -------------- --------------
     #                                        ---  Supporting code follows ---
     #
     def __validateAndFix(self, databaseName, collectionName, dList, docIdL, schemaLevel="full"):
         """[summary]
-
         Args:
-            databaseName ([type]): [description]
-            collectionName ([type]): [description]
-            dList ([type]): [description]
-            docIdL ([type]): [description]
-            schemaLevel (str, optional): [description]. Defaults to "full".
-
+            databaseName (str): Target database name
+            collectionName (str): Target collection name
+            dList (list): document list
+            docIdL (list): list of key document attributes required to uniquely identify a document in a given collection
+                           (from SchemaDefAccess.getDocumentKeyAttributeNames())
+            schemaLevel (str, optional): Completeness of json/bson metadata schema bound to each collection (e.g. 'min', 'full' or None); Defaults to "full"
         Returns:
             (list):  updated document list (remediated for validation issues)
         """
         #
         rList = []
         logger.info("Validating and fixing objects in databaseName %s collectionName %s numObject %d docIdL %r", databaseName, collectionName, len(dList), docIdL)
         cD = self.__schP.getJsonSchema(databaseName, collectionName, encodingType="JSON", level=schemaLevel)
@@ -989,14 +1014,15 @@
         filterArtifactErrors = True
         valInfo = Draft4Validator(cD, format_checker=FormatChecker())
         for ii, dD in enumerate(dList):
             cN = self.__getKeyValues(dD, docIdL)
             logger.info("Checking %r with schema %s collection %s document (%d)", cN, databaseName, collectionName, ii + 1)
             updL = []
             try:
+                failFlag = False
                 for error in sorted(valInfo.iter_errors(dD), key=str):
                     #
                     # Filter and cleanup artifacts -
                     #
                     if filterArtifactErrors and "properties are not allowed ('_id' was unexpected)" in error.message:
                         dD.pop("_id")
                         continue
@@ -1012,17 +1038,18 @@
                         if subObjName in dD:
                             logger.info("Found subobject %r", subObjName)
                             logger.info("subObject %r", dD[subObjName])
                             dD.pop(subObjName)
                             updL.append(cN)
                     #
             except Exception as e:
+                failFlag = True
                 logger.exception("Validation updating processing error %s", str(e))
             #
-            if updL:
+            if not failFlag:
                 rList.append(dD)
         #
         logger.info("Corrected document count (%d) %r", len(updL), updL)
         return rList
 
     #
     def __validateDocuments(self, databaseName, collectionName, dList, docIdL, schemaLevel="full"):
```

### Comparing `rcsb.db-1.709/rcsb/db/mysql/Connection.py` & `rcsb.db-1.710/rcsb/db/mysql/Connection.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mysql/ConnectionBase.py` & `rcsb.db-1.710/rcsb/db/mysql/ConnectionBase.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mysql/MyDbAdapter.py` & `rcsb.db-1.710/rcsb/db/mysql/MyDbAdapter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mysql/MyDbUtil.py` & `rcsb.db-1.710/rcsb/db/mysql/MyDbUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mysql/MysqlSchemaImporter.py` & `rcsb.db-1.710/rcsb/db/mysql/MysqlSchemaImporter.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/mysql/SchemaDefLoader.py` & `rcsb.db-1.710/rcsb/db/mysql/SchemaDefLoader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/processors/ClusterDataPrep.py` & `rcsb.db-1.710/rcsb/db/processors/ClusterDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/processors/DataExchangeStatus.py` & `rcsb.db-1.710/rcsb/db/processors/DataExchangeStatus.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/processors/DataTransformFactory.py` & `rcsb.db-1.710/rcsb/db/processors/DataTransformFactory.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/processors/RepoHoldingsDataPrep.py` & `rcsb.db-1.710/rcsb/db/processors/RepoHoldingsDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py` & `rcsb.db-1.710/rcsb/db/processors/RepoHoldingsRemoteDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/processors/SchemaDefDataPrep.py` & `rcsb.db-1.710/rcsb/db/processors/SchemaDefDataPrep.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/processors/SchemaDefReShape.py` & `rcsb.db-1.710/rcsb/db/processors/SchemaDefReShape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/sql/QueryDirectives.py` & `rcsb.db-1.710/rcsb/db/sql/QueryDirectives.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/sql/SqlGen.py` & `rcsb.db-1.710/rcsb/db/sql/SqlGen.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/utils/CaseNormalizedDict.py` & `rcsb.db-1.710/rcsb/db/utils/CaseNormalizedDict.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/utils/PdbxSchemaMapReader.py` & `rcsb.db-1.710/rcsb/db/utils/PdbxSchemaMapReader.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/utils/ProvenanceProvider.py` & `rcsb.db-1.710/rcsb/db/utils/ProvenanceProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/utils/SchemaProvider.py` & `rcsb.db-1.710/rcsb/db/utils/SchemaProvider.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/utils/TextUtil.py` & `rcsb.db-1.710/rcsb/db/utils/TextUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/utils/TimeUtil.py` & `rcsb.db-1.710/rcsb/db/utils/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/utils/makePathList.py` & `rcsb.db-1.710/rcsb/db/utils/makePathList.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/utils/unescape.py` & `rcsb.db-1.710/rcsb/db/utils/unescape.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb/db/wf/RepoLoadWorkflow.py` & `rcsb.db-1.710/rcsb/db/wf/RepoLoadWorkflow.py`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/rcsb.db.egg-info/PKG-INFO` & `rcsb.db-1.710/rcsb.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rcsb.db
-Version: 1.709
+Version: 1.710
 Summary: RCSB Python Database Access and Loading Utility Classes
 Home-page: https://github.com/rcsb/py-rcsb_db
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rcsb.db-1.709/rcsb.db.egg-info/SOURCES.txt` & `rcsb.db-1.710/rcsb.db.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/requirements.txt` & `rcsb.db-1.710/requirements.txt`

 * *Files identical despite different names*

### Comparing `rcsb.db-1.709/setup.py` & `rcsb.db-1.710/setup.py`

 * *Files identical despite different names*

