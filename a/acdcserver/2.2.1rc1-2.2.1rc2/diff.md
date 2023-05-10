# Comparing `tmp/acdcserver-2.2.1rc1.tar.gz` & `tmp/acdcserver-2.2.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdcserver-2.2.1rc1.tar", last modified: Tue Apr 25 21:48:20 2023, max compression
+gzip compressed data, was "acdcserver-2.2.1rc2.tar", last modified: Wed May 10 08:20:20 2023, max compression
```

## Comparing `acdcserver-2.2.1rc1.tar` & `acdcserver-2.2.1rc2.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/bin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/bin/HWMon/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23048 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/HWMon/wmcore-SysStat
--rwxr-xr-x   0 runner    (1001) docker     (123)     1918 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/acdcserver-tools
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/bin/adhoc-scripts/
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/ParseSpecCmsswdist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/checkDsetFileCount.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/checkStuckLQE.py
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/createPileupObjects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/drainAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/getWQStatusByWorkflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/mongoInit.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/parseUnifiedCampaigns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/setrequeststatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/summaryWMStatsFailures.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/updateTotalStats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/adhoc-scripts/workflowCompletion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/attempt-to-patch.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3324 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/buildrelease.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/check-ACDC-parentage
--rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/check-phedex-dbs-status
--rwxr-xr-x   0 runner    (1001) docker     (123)     7262 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/check-request-wq-status
--rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/clean-oracle
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/combineMinifyWMStats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/couch-thrash.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/couch_archiver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2025 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/create-iam-token.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/createStoreResults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/dbsbuffer-file-fix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5982 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/deploy-rpm-to-jenkins.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     4803 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/fix-dbs-parentage
--rwxr-xr-x   0 runner    (1001) docker     (123)     1628 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/inject-to-config-cache
--rwxr-xr-x   0 runner    (1001) docker     (123)     2939 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/kill-workflow-in-agent
--rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/kill-workflow-in-global
--rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/make-local-clones.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     3615 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/outputmodules-from-config
--rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/patchComponent.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     6550 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/paused-jobs
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/purgeDeletedCouchDoc.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/reqmgr-put-default-config
--rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/reqmgr-sw-update
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/vaildateCMSSWMergeVersion
--rwxr-xr-x   0 runner    (1001) docker     (123)    19065 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmagent-couchapp-init
--rwxr-xr-x   0 runner    (1001) docker     (123)     3736 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmagent-delete-couchdb-workflow
--rwxr-xr-x   0 runner    (1001) docker     (123)    16408 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmagent-mod-config
--rwxr-xr-x   0 runner    (1001) docker     (123)    15441 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmagent-resource-control
--rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmagent-unregister-wmstats
--rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmagent-upload-config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7198 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmagent-workqueue
--rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmc-dist-patch
--rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmc-dist-unpatch
--rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmc-httpd
--rwxr-xr-x   0 runner    (1001) docker     (123)     4259 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmcore-db-init
--rwxr-xr-x   0 runner    (1001) docker     (123)     2917 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmcore-new-config
--rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmcore-new-flow
--rwxr-xr-x   0 runner    (1001) docker     (123)    10729 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/bin/wmcoreD
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 21:48:19.000000 acdcserver-2.2.1rc1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-25 21:48:19.000000 acdcserver-2.2.1rc1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/setup_build.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/setup_dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.454795 acdcserver-2.2.1rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.450795 acdcserver-2.2.1rc1/src/couchapps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/src/couchapps/ACDC/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/CouchDBLogo.png
--rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/DMWMLogo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/collections.html
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/displaycollection.html
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/style/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/style/main.css
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/_id
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/couchapp.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/src/couchapps/ACDC/filters/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/filters/filterDeletedDocs.js
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/rewrites.json
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/validate_doc_update.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.450795 acdcserver-2.2.1rc1/src/couchapps/ACDC/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.450795 acdcserver-2.2.1rc1/src/couchapps/ACDC/vendor/acdc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/src/couchapps/ACDC/vendor/acdc/_attachments/
--rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/vendor/acdc/_attachments/acdc.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.450795 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/byCollectionName/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/byCollectionName/map.js
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/byCollectionName/reduce.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/byTimestamp/
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/byTimestamp/map.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/coll_fileset_count/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/coll_fileset_count/map.js
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/coll_fileset_count/reduce.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.458795 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/coll_fileset_docs/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/coll_fileset_docs/map.js
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/ACDC/views/coll_fileset_docs/reduce.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/.couchappignore
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/.couchapprc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/_attachments/
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/_attachments/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/_attachments/style/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/_attachments/style/main.css
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/_id
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/couchapp.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/updates/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/updates/newgroup.js
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/updates/newuser.js
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/updates/ownthis.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.450795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/_attachments/
--rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/_attachments/jquery.couchapp.js
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/couchapp.js
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/date.js
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/path.js
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/template.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.450795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/groupuser/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/groupuser/_attachments/
--rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/groupuser/_attachments/groupuser.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.454795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/group_members/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/group_members/map.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/groups/map.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/name_map/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/name_map/map.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/owner_group_user/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/owner_group_user/map.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/users/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/couchapps/GroupUser/views/users/map.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.454795 acdcserver-2.2.1rc1/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/python/WMCore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/python/WMCore/ACDC/
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/ACDC/Collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/ACDC/CollectionTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/ACDC/CouchCollection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/ACDC/CouchFileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/ACDC/CouchService.py
--rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/ACDC/DataCollectionService.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/ACDC/Fileset.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/ACDC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.462795 acdcserver-2.2.1rc1/src/python/WMCore/Algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Algorithms/ParseXMLFile.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Algorithms/Permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/
--rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/File.py
--rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Fileset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/JobGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/JobPackage.py
--rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/LumiList.py
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Mask.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Pickleable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/WMObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/WorkUnit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/src/python/WMCore/Database/
--rw-r--r--   0 runner    (1001) docker     (123)    53857 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/CMSCouch.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/ConfigDBMap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/CouchUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/DBCore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/DBCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/DBExceptionHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/DBFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/DBFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/Dialects.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/ExecuteDAO.py
--rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/MongoDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/MySQLCore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/ResultSet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/Transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Database/ipy_profile_couch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/CouchObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/Decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/Group.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/Interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/User.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30625 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Lexicon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/src/python/WMCore/Services/
--rw-r--r--   0 runner    (1001) docker     (123)    23646 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Services/Requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Services/pycurl_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/WMException.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/src/python/WMCore/Wrappers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/src/python/WMCore/Wrappers/JsonWrapper/
--rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Wrappers/JsonWrapper/JSONThunker.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Wrappers/JsonWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/Wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-25 21:48:16.000000 acdcserver-2.2.1rc1/src/python/WMCore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 21:48:20.466795 acdcserver-2.2.1rc1/src/python/acdcserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-25 21:48:20.000000 acdcserver-2.2.1rc1/src/python/acdcserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-04-25 21:48:20.000000 acdcserver-2.2.1rc1/src/python/acdcserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 21:48:20.000000 acdcserver-2.2.1rc1/src/python/acdcserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-25 21:48:20.000000 acdcserver-2.2.1rc1/src/python/acdcserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-25 21:48:20.000000 acdcserver-2.2.1rc1/src/python/acdcserver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.143239 acdcserver-2.2.1rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 08:20:20.143239 acdcserver-2.2.1rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.131239 acdcserver-2.2.1rc2/bin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.131239 acdcserver-2.2.1rc2/bin/HWMon/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23048 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/HWMon/wmcore-SysStat
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1918 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/acdcserver-tools
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.131239 acdcserver-2.2.1rc2/bin/adhoc-scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/ParseSpecCmsswdist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/checkDsetFileCount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/checkStuckLQE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/createPileupObjects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/drainAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/getWQStatusByWorkflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/mongoInit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/parseUnifiedCampaigns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/setrequeststatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/summaryWMStatsFailures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/updateTotalStats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6294 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/adhoc-scripts/workflowCompletion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1181 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/attempt-to-patch.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3324 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/buildrelease.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/check-ACDC-parentage
+-rwxr-xr-x   0 runner    (1001) docker     (123)      377 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/check-phedex-dbs-status
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7262 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/check-request-wq-status
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3083 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/clean-oracle
+-rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/combineMinifyWMStats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/couch-thrash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/couch_archiver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2025 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/create-iam-token.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/createStoreResults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/dbsbuffer-file-fix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5982 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/deploy-rpm-to-jenkins.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4803 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/fix-dbs-parentage
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1628 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/inject-to-config-cache
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2939 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/kill-workflow-in-agent
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/kill-workflow-in-global
+-rwxr-xr-x   0 runner    (1001) docker     (123)      658 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/make-local-clones.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3615 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/outputmodules-from-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      917 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/patchComponent.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6550 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/paused-jobs
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/purgeDeletedCouchDoc.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/reqmgr-put-default-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      916 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/reqmgr-sw-update
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/vaildateCMSSWMergeVersion
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19065 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmagent-couchapp-init
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3736 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmagent-delete-couchdb-workflow
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16863 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmagent-mod-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15441 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmagent-resource-control
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmagent-unregister-wmstats
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1219 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmagent-upload-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7198 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmagent-workqueue
+-rwxr-xr-x   0 runner    (1001) docker     (123)      646 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmc-dist-patch
+-rwxr-xr-x   0 runner    (1001) docker     (123)      409 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmc-dist-unpatch
+-rwxr-xr-x   0 runner    (1001) docker     (123)       63 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmc-httpd
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4259 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmcore-db-init
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2917 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmcore-new-config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmcore-new-flow
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10729 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/bin/wmcoreD
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 08:20:19.000000 acdcserver-2.2.1rc2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-10 08:20:20.143239 acdcserver-2.2.1rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-10 08:20:19.000000 acdcserver-2.2.1rc2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/setup_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13063 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/setup_dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.123239 acdcserver-2.2.1rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.123239 acdcserver-2.2.1rc2/src/couchapps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.131239 acdcserver-2.2.1rc2/src/couchapps/ACDC/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.131239 acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/CouchDBLogo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    17898 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/DMWMLogo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/collections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/displaycollection.html
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.131239 acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/style/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/style/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/_id
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/couchapp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.131239 acdcserver-2.2.1rc2/src/couchapps/ACDC/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/filters/filterDeletedDocs.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/rewrites.json
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/validate_doc_update.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.123239 acdcserver-2.2.1rc2/src/couchapps/ACDC/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.123239 acdcserver-2.2.1rc2/src/couchapps/ACDC/vendor/acdc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.131239 acdcserver-2.2.1rc2/src/couchapps/ACDC/vendor/acdc/_attachments/
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/vendor/acdc/_attachments/acdc.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.123239 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/byCollectionName/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/byCollectionName/map.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/byCollectionName/reduce.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/byTimestamp/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/byTimestamp/map.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/coll_fileset_count/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/coll_fileset_count/map.js
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/coll_fileset_count/reduce.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/coll_fileset_docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/coll_fileset_docs/map.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/ACDC/views/coll_fileset_docs/reduce.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/.couchappignore
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/.couchapprc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/_attachments/
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/_attachments/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/_attachments/style/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/_attachments/style/main.css
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/_id
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/couchapp.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/updates/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/updates/newgroup.js
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/updates/newuser.js
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/updates/ownthis.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.123239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/_attachments/
+-rw-r--r--   0 runner    (1001) docker     (123)     6984 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/_attachments/jquery.couchapp.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/couchapp.js
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/date.js
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/path.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/template.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.123239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/groupuser/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/groupuser/_attachments/
+-rw-r--r--   0 runner    (1001) docker     (123)     8703 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/groupuser/_attachments/groupuser.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.123239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/group_members/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/group_members/map.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/groups/map.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/name_map/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/name_map/map.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/owner_group_user/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/owner_group_user/map.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/users/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/couchapps/GroupUser/views/users/map.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.127239 acdcserver-2.2.1rc2/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.135239 acdcserver-2.2.1rc2/src/python/WMCore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.139239 acdcserver-2.2.1rc2/src/python/WMCore/ACDC/
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/ACDC/Collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/ACDC/CollectionTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/ACDC/CouchCollection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/ACDC/CouchFileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/ACDC/CouchService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17613 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/ACDC/DataCollectionService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/ACDC/Fileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/ACDC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.139239 acdcserver-2.2.1rc2/src/python/WMCore/Algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Algorithms/ParseXMLFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Algorithms/Permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19948 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.139239 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5211 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Fileset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/JobGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/JobPackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27401 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/LumiList.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Pickleable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/WMObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/WorkUnit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.139239 acdcserver-2.2.1rc2/src/python/WMCore/Database/
+-rw-r--r--   0 runner    (1001) docker     (123)    55027 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/CMSCouch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/ConfigDBMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/CouchUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/DBCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/DBCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/DBExceptionHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/DBFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5578 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/DBFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/Dialects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/ExecuteDAO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10808 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/MongoDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/MySQLCore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/ResultSet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/Transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11958 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Database/ipy_profile_couch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.143239 acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/CouchObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/Decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/Group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/Interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30625 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Lexicon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.143239 acdcserver-2.2.1rc2/src/python/WMCore/Services/
+-rw-r--r--   0 runner    (1001) docker     (123)    23646 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Services/Requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20908 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Services/pycurl_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/WMException.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.143239 acdcserver-2.2.1rc2/src/python/WMCore/Wrappers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.143239 acdcserver-2.2.1rc2/src/python/WMCore/Wrappers/JsonWrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)    12767 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Wrappers/JsonWrapper/JSONThunker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Wrappers/JsonWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/Wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-10 08:20:13.000000 acdcserver-2.2.1rc2/src/python/WMCore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 08:20:20.143239 acdcserver-2.2.1rc2/src/python/acdcserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 08:20:19.000000 acdcserver-2.2.1rc2/src/python/acdcserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6024 2023-05-10 08:20:20.000000 acdcserver-2.2.1rc2/src/python/acdcserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 08:20:19.000000 acdcserver-2.2.1rc2/src/python/acdcserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 08:20:19.000000 acdcserver-2.2.1rc2/src/python/acdcserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 08:20:19.000000 acdcserver-2.2.1rc2/src/python/acdcserver.egg-info/top_level.txt
```

### Comparing `acdcserver-2.2.1rc1/LICENSE` & `acdcserver-2.2.1rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/NOTICE` & `acdcserver-2.2.1rc2/NOTICE`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/README.md` & `acdcserver-2.2.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/HWMon/wmcore-SysStat` & `acdcserver-2.2.1rc2/bin/HWMon/wmcore-SysStat`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/acdcserver-tools` & `acdcserver-2.2.1rc2/bin/acdcserver-tools`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/ParseSpecCmsswdist.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/ParseSpecCmsswdist.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/checkDsetFileCount.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/checkDsetFileCount.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/checkStuckLQE.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/checkStuckLQE.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/createPileupObjects.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/createPileupObjects.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/drainAgent.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/drainAgent.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/getWQStatusByWorkflow.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/getWQStatusByWorkflow.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/mongoInit.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/mongoInit.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/parseUnifiedCampaigns.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/parseUnifiedCampaigns.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/setrequeststatus.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/setrequeststatus.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/summaryWMStatsFailures.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/summaryWMStatsFailures.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/updateTotalStats.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/updateTotalStats.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/adhoc-scripts/workflowCompletion.py` & `acdcserver-2.2.1rc2/bin/adhoc-scripts/workflowCompletion.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/attempt-to-patch.sh` & `acdcserver-2.2.1rc2/bin/attempt-to-patch.sh`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/buildrelease.sh` & `acdcserver-2.2.1rc2/bin/buildrelease.sh`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/check-ACDC-parentage` & `acdcserver-2.2.1rc2/bin/check-ACDC-parentage`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/check-request-wq-status` & `acdcserver-2.2.1rc2/bin/check-request-wq-status`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/clean-oracle` & `acdcserver-2.2.1rc2/bin/clean-oracle`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/combineMinifyWMStats.py` & `acdcserver-2.2.1rc2/bin/combineMinifyWMStats.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/couch-thrash.py` & `acdcserver-2.2.1rc2/bin/couch-thrash.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/couch_archiver.py` & `acdcserver-2.2.1rc2/bin/couch_archiver.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/create-iam-token.sh` & `acdcserver-2.2.1rc2/bin/create-iam-token.sh`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/createStoreResults.py` & `acdcserver-2.2.1rc2/bin/createStoreResults.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/dbsbuffer-file-fix.py` & `acdcserver-2.2.1rc2/bin/dbsbuffer-file-fix.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/deploy-rpm-to-jenkins.sh` & `acdcserver-2.2.1rc2/bin/deploy-rpm-to-jenkins.sh`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/fix-dbs-parentage` & `acdcserver-2.2.1rc2/bin/fix-dbs-parentage`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/inject-to-config-cache` & `acdcserver-2.2.1rc2/bin/inject-to-config-cache`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/kill-workflow-in-agent` & `acdcserver-2.2.1rc2/bin/kill-workflow-in-agent`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/kill-workflow-in-global` & `acdcserver-2.2.1rc2/bin/kill-workflow-in-global`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/make-local-clones.sh` & `acdcserver-2.2.1rc2/bin/make-local-clones.sh`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/outputmodules-from-config` & `acdcserver-2.2.1rc2/bin/outputmodules-from-config`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/patchComponent.sh` & `acdcserver-2.2.1rc2/bin/patchComponent.sh`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/paused-jobs` & `acdcserver-2.2.1rc2/bin/paused-jobs`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/purgeDeletedCouchDoc.py` & `acdcserver-2.2.1rc2/bin/purgeDeletedCouchDoc.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/reqmgr-put-default-config` & `acdcserver-2.2.1rc2/bin/reqmgr-put-default-config`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/reqmgr-sw-update` & `acdcserver-2.2.1rc2/bin/reqmgr-sw-update`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/vaildateCMSSWMergeVersion` & `acdcserver-2.2.1rc2/bin/vaildateCMSSWMergeVersion`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmagent-couchapp-init` & `acdcserver-2.2.1rc2/bin/wmagent-couchapp-init`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmagent-delete-couchdb-workflow` & `acdcserver-2.2.1rc2/bin/wmagent-delete-couchdb-workflow`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmagent-mod-config` & `acdcserver-2.2.1rc2/bin/wmagent-mod-config`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,29 @@
 def importConfigTemplate(filename):
     """
     _importConfigTemplate_
 
     Given filename, load it and grab the configuration object from it
 
     """
-    modSpecs = importlib.machinery.PathFinder().find_spec(filename)
-    mod = modSpecs.loader.load_module("wmcore_config_input")
-    config = getattr(mod, 'config', None)
+
+    cfgBaseName = os.path.basename(filename).replace(".py", "")
+    cfgDirName = os.path.dirname(filename)
+    if not cfgDirName:
+        modSpecs = importlib.machinery.PathFinder().find_spec(cfgBaseName)
+    else:
+        modSpecs = importlib.machinery.PathFinder().find_spec(cfgBaseName, [cfgDirName])
+    try:
+        modRef = modSpecs.loader.load_module(cfgBaseName)
+    except Exception as ex:
+        msg = "Unable to load Configuration File: %s\n Due to error:\n" % filename
+        msg += str(ex)
+        msg += str(traceback.format_exc())
+        raise RuntimeError(msg)
+    config = getattr(modRef, 'config', None)
     if config is None:
         msg = "No config attribute found in %s" % filename
         raise RuntimeError(msg)
     return config
 
 
 def saveConfiguration(configObject, outputPath):
```

### Comparing `acdcserver-2.2.1rc1/bin/wmagent-resource-control` & `acdcserver-2.2.1rc2/bin/wmagent-resource-control`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmagent-unregister-wmstats` & `acdcserver-2.2.1rc2/bin/wmagent-unregister-wmstats`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmagent-upload-config` & `acdcserver-2.2.1rc2/bin/wmagent-upload-config`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmagent-workqueue` & `acdcserver-2.2.1rc2/bin/wmagent-workqueue`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmc-dist-patch` & `acdcserver-2.2.1rc2/bin/wmc-dist-patch`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmcore-db-init` & `acdcserver-2.2.1rc2/bin/wmcore-db-init`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmcore-new-config` & `acdcserver-2.2.1rc2/bin/wmcore-new-config`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmcore-new-flow` & `acdcserver-2.2.1rc2/bin/wmcore-new-flow`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/bin/wmcoreD` & `acdcserver-2.2.1rc2/bin/wmcoreD`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/setup.py` & `acdcserver-2.2.1rc2/setup.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/setup_build.py` & `acdcserver-2.2.1rc2/setup_build.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/setup_dependencies.py` & `acdcserver-2.2.1rc2/setup_dependencies.py`

 * *Files 4% similar despite different names*

```diff
@@ -184,15 +184,23 @@
                      'WMCore.JobStateMachine', 'WMComponent+',
                      'WMCore.ThreadPool',
                      'WMCore.BossAir+', 'WMCore.Credential',
                      'WMCore.JobSplitting+', 'WMCore.ProcessPool',
                      'WMCore.Services+', 'WMCore.WMSpec+',
                      'WMCore.WMBS+', 'WMCore.ResourceControl+'],
         'systems': ['wmc-web', 'wmc-database', 'global-workqueue', 'wmc-runtime'],
-        'statics': ['src/javascript/WMCore/WebTools/Agent',
+        'statics': ['bin+',
+                    'deploy+',
+                    'etc+',
+                    'src/couchapps/SummaryStats+',
+                    'src/couchapps/FWJRDump+',
+                    'src/couchapps/JobDump+',
+                    'src/couchapps/WMStatsAgent+',
+                    'src/couchapps/WorkQueue+',
+                    'src/javascript/WMCore/WebTools/Agent',
                     'src/javascript/WMCore/WebTools/WMBS',
                     'src/javascript/external/graphael',
                     'src/templates/WMCore/WebTools/WMBS'],
     },
     'crabcache': {
         'packages': ['WMCore.Wrappers+', 'WMCore.Services.UserFileCache+'],
         'systems': ['wmc-rest'],
```

### Comparing `acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/CouchDBLogo.png` & `acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/CouchDBLogo.png`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/DMWMLogo.png` & `acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/DMWMLogo.png`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/collections.html` & `acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/collections.html`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/displaycollection.html` & `acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/displaycollection.html`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/ACDC/_attachments/index.html` & `acdcserver-2.2.1rc2/src/couchapps/ACDC/_attachments/index.html`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/ACDC/rewrites.json` & `acdcserver-2.2.1rc2/src/couchapps/ACDC/rewrites.json`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/ACDC/vendor/acdc/_attachments/acdc.js` & `acdcserver-2.2.1rc2/src/couchapps/ACDC/vendor/acdc/_attachments/acdc.js`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/GroupUser/_attachments/index.html` & `acdcserver-2.2.1rc2/src/couchapps/GroupUser/_attachments/index.html`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/_attachments/jquery.couchapp.js` & `acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/_attachments/jquery.couchapp.js`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/date.js` & `acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/date.js`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/path.js` & `acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/path.js`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/couchapp/template.js` & `acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/couchapp/template.js`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/couchapps/GroupUser/vendor/groupuser/_attachments/groupuser.js` & `acdcserver-2.2.1rc2/src/couchapps/GroupUser/vendor/groupuser/_attachments/groupuser.js`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/ACDC/Collection.py` & `acdcserver-2.2.1rc2/src/python/WMCore/ACDC/Collection.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/ACDC/CouchCollection.py` & `acdcserver-2.2.1rc2/src/python/WMCore/ACDC/CouchCollection.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/ACDC/CouchFileset.py` & `acdcserver-2.2.1rc2/src/python/WMCore/ACDC/CouchFileset.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/ACDC/CouchService.py` & `acdcserver-2.2.1rc2/src/python/WMCore/ACDC/CouchService.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/ACDC/DataCollectionService.py` & `acdcserver-2.2.1rc2/src/python/WMCore/ACDC/DataCollectionService.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/ACDC/Fileset.py` & `acdcserver-2.2.1rc2/src/python/WMCore/ACDC/Fileset.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Algorithms/ParseXMLFile.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Algorithms/ParseXMLFile.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Algorithms/Permissions.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Algorithms/Permissions.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Configuration.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Configuration.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/File.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/File.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Fileset.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Fileset.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Job.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Job.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/JobGroup.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/JobGroup.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/JobPackage.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/JobPackage.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/LumiList.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/LumiList.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Mask.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Mask.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Run.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Run.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Subscription.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Subscription.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/WMObject.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/WMObject.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/WorkUnit.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/WorkUnit.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/DataStructs/Workflow.py` & `acdcserver-2.2.1rc2/src/python/WMCore/DataStructs/Workflow.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/CMSCouch.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/CMSCouch.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,19 @@
 from future import standard_library
 standard_library.install_aliases()
 from future.utils import viewitems
 import urllib.request, urllib.parse, urllib.error
 
 import base64
 import hashlib
+import json
 import logging
 import re
 import time
+import sys
 from datetime import datetime
 from http.client import HTTPException
 
 from Utils.IteratorTools import grouper, nestedDictUpdate
 from WMCore.Lexicon import sanitizeURL
 from WMCore.Services.Requests import JSONRequests
 
@@ -142,37 +144,39 @@
     def checkForCouchError(self, status, reason, data=None, result=None):
         """
         _checkForCouchError_
 
         Check the HTTP status and raise an appropriate exception.
         """
         if status == 400:
-            raise CouchBadRequestError(reason, data, result)
+            raise CouchBadRequestError(reason, data, result, status)
         elif status == 401:
-            raise CouchUnauthorisedError(reason, data, result)
+            raise CouchUnauthorisedError(reason, data, result, status)
         elif status == 403:
-            raise CouchForbidden(reason, data, result)
+            raise CouchForbidden(reason, data, result, status)
         elif status == 404:
-            raise CouchNotFoundError(reason, data, result)
+            raise CouchNotFoundError(reason, data, result, status)
         elif status == 405:
-            raise CouchNotAllowedError(reason, data, result)
+            raise CouchNotAllowedError(reason, data, result, status)
         elif status == 406:
-            raise CouchNotAcceptableError(reason, data, result)
+            raise CouchNotAcceptableError(reason, data, result, status)
         elif status == 409:
-            raise CouchConflictError(reason, data, result)
+            raise CouchConflictError(reason, data, result, status)
         elif status == 410:
-            raise CouchFeatureGone(reason, data, result)
+            raise CouchFeatureGone(reason, data, result, status)
         elif status == 412:
-            raise CouchPreconditionFailedError(reason, data, result)
+            raise CouchPreconditionFailedError(reason, data, result, status)
+        elif status == 413:
+            raise CouchRequestTooLargeError(reason, data, result, status)
         elif status == 416:
-            raise CouchRequestedRangeNotSatisfiableError(reason, data, result)
+            raise CouchRequestedRangeNotSatisfiableError(reason, data, result, status)
         elif status == 417:
-            raise CouchExpectationFailedError(reason, data, result)
+            raise CouchExpectationFailedError(reason, data, result, status)
         elif status == 500:
-            raise CouchInternalServerError(reason, data, result)
+            raise CouchInternalServerError(reason, data, result, status)
         elif status in [502, 503, 504]:
             # There are HTTP errors that CouchDB doesn't raise but can appear
             # in our environment, e.g. behind a proxy. Reraise the HTTPException
             raise CouchError(reason, data, result, status)
         else:
             # We have a new error status, log it
             raise CouchError(reason, data, result, status)
@@ -218,29 +222,36 @@
             data[label] = int(time.time())
         else:
             for doc in data:
                 if label not in doc:
                     doc[label] = int(time.time())
         return data
 
+    def getQueueSize(self):
+        """
+        Return the current size of the queue, i.e., how
+        many documents are already queued up
+        """
+        return len(self._queue)
+
     def queue(self, doc, timestamp=False, viewlist=None, callback=None):
         """
         Queue up a doc for bulk insert. If timestamp = True add a timestamp
         field if one doesn't exist. Use this over commit(timestamp=True) if you
         want to timestamp when a document was added to the queue instead of when
         it was committed
         If a callback is specified then pass it to the commit function if a
         commit is triggered
         """
         viewlist = viewlist or []
         if timestamp:
             self.timestamp(doc, timestamp)
         # TODO: Thread this off so that it's non blocking...
-        if len(self._queue) >= self._queue_size:
-            print('queue larger than %s records, committing' % self._queue_size)
+        if self.getQueueSize() >= self._queue_size:
+            logging.warning('queue larger than %s records, committing', self._queue_size)
             self.commit(viewlist=viewlist, callback=callback)
         self._queue.append(doc)
 
     def queueDelete(self, doc):
         """
         Queue up a document for deletion
         """
@@ -1113,90 +1124,102 @@
         self.reason = reason
         self.data = data
         self.result = result
         self.type = "CouchError"
         self.status = status
 
     def __str__(self):
-        "Stringify the error"
-        if self.status != None:
-            errorMsg = "NEW ERROR STATUS! UPDATE CMSCOUCH.PY!: %s\n" % self.status
-        else:
-            errorMsg = ""
-        return errorMsg + "%s - reason: %s, data: %s result: %s" % (self.type,
-                                                                    self.reason,
-                                                                    repr(self.data),
-                                                                    self.result)
+        """Stringify the error"""
+        errorMsg = ""
+        if self.type == "CouchError":
+            errorMsg += "A NEW COUCHDB ERROR TYPE/STATUS HAS BEEN FOUND! "
+            errorMsg += "UPDATE CMSCOUCH.PY IMPLEMENTATION WITH A NEW COUCH ERROR/STATUS! "
+            errorMsg += f"Status: {self.status}\n"
+        errorMsg += f"Error type: {self.type}, Status code: {self.status}, "
+        errorMsg += f"Reason: {self.reason}, Data: {repr(self.data)}"
+        return errorMsg
 
 
 class CouchBadRequestError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchBadRequestError"
 
 
 class CouchUnauthorisedError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchUnauthorisedError"
 
 
 class CouchNotFoundError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchNotFoundError"
 
 
 class CouchNotAllowedError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchNotAllowedError"
 
 class CouchNotAcceptableError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchNotAcceptableError"
 
 class CouchConflictError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchConflictError"
 
 
 class CouchFeatureGone(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchFeatureGone"
 
 
 class CouchPreconditionFailedError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchPreconditionFailedError"
 
+
+class CouchRequestTooLargeError(CouchError):
+    def __init__(self, reason, data, result, status):
+        # calculate the size of this JSON serialized object
+        docSize = sys.getsizeof(json.dumps(data))
+        errorMsg = f"Document has {docSize} bytes and it's too large to be accepted by CouchDB. "
+        errorMsg += f"Check the CouchDB configuration to see the current value "
+        errorMsg += f"under 'couchdb.max_document_size' (default is 8M bytes)."
+        CouchError.__init__(self, reason, errorMsg, result, status)
+        self.type = "CouchRequestTooLargeError"
+
+
 class CouchExpectationFailedError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchExpectationFailedError"
 
 class CouchRequestedRangeNotSatisfiableError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchRequestedRangeNotSatisfiableError"
 
 
 class CouchInternalServerError(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchInternalServerError"
 
 
 class CouchForbidden(CouchError):
-    def __init__(self, reason, data, result):
-        CouchError.__init__(self, reason, data, result)
+    def __init__(self, reason, data, result, status):
+        CouchError.__init__(self, reason, data, result, status)
         self.type = "CouchForbidden"
 
 
 class CouchMonitor(object):
     def __init__(self, couchURL):
         if isinstance(couchURL, CouchServer):
             self.couchServer = couchURL
```

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/ConfigDBMap.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/ConfigDBMap.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/CouchUtils.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/CouchUtils.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/DBCore.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/DBCore.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/DBCreator.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/DBCreator.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/DBExceptionHandler.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/DBExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/DBFactory.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/DBFactory.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/DBFormatter.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/DBFormatter.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/ExecuteDAO.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/ExecuteDAO.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/MongoDB.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/MongoDB.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/MySQLCore.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/MySQLCore.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/ResultSet.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/ResultSet.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/Transaction.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/Transaction.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Database/ipy_profile_couch.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Database/ipy_profile_couch.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/CouchObject.py` & `acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/CouchObject.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/Decorators.py` & `acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/Decorators.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/Group.py` & `acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/Group.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/Interface.py` & `acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/Interface.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/GroupUser/User.py` & `acdcserver-2.2.1rc2/src/python/WMCore/GroupUser/User.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Lexicon.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Lexicon.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Services/Requests.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Services/Requests.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Services/pycurl_manager.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Services/pycurl_manager.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/WMException.py` & `acdcserver-2.2.1rc2/src/python/WMCore/WMException.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/WMCore/Wrappers/JsonWrapper/JSONThunker.py` & `acdcserver-2.2.1rc2/src/python/WMCore/Wrappers/JsonWrapper/JSONThunker.py`

 * *Files identical despite different names*

### Comparing `acdcserver-2.2.1rc1/src/python/acdcserver.egg-info/SOURCES.txt` & `acdcserver-2.2.1rc2/src/python/acdcserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

