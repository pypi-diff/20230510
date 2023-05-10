# Comparing `tmp/uidom-0.2a0.tar.gz` & `tmp/uidom-0.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uidom-0.2a0.tar", max compression
+gzip compressed data, was "uidom-0.2a1.tar", max compression
```

## Comparing `uidom-0.2a0.tar` & `uidom-0.2a1.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.2a0/LICENSE
--rw-r--r--   0        0        0     5686 2023-05-01 05:55:18.794343 uidom-0.2a0/README.md
--rw-r--r--   0        0        0     1271 2023-05-09 21:00:02.884891 uidom-0.2a0/pyproject.toml
--rw-r--r--   0        0        0      218 2023-05-09 20:59:28.648696 uidom-0.2a0/uidom/__init__.py
--rw-r--r--   0        0        0     1067 2023-05-09 19:55:16.645883 uidom-0.2a0/uidom/cli/__init__.py
--rw-r--r--   0        0        0    12108 2023-05-05 19:23:34.126884 uidom-0.2a0/uidom/cli/_cli.py
--rw-r--r--   0        0        0     6636 2023-05-09 20:55:47.274480 uidom-0.2a0/uidom/cli/cli.py
--rw-r--r--   0        0        0      517 2023-05-09 11:52:14.395273 uidom-0.2a0/uidom/dom/__init__.py
--rw-r--r--   0        0        0     4944 2023-05-09 14:03:20.721191 uidom-0.2a0/uidom/dom/htmldocument.py
--rw-r--r--   0        0        0     5924 2023-05-09 16:54:51.261005 uidom-0.2a0/uidom/dom/htmlelement.py
--rw-r--r--   0        0        0    42978 2023-03-25 19:14:55.486184 uidom-0.2a0/uidom/dom/icons.py
--rw-r--r--   0        0        0     1363 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/dom/jinja.py
--rwxr-xr-x   0        0        0      304 2022-07-09 13:34:38.382685 uidom-0.2a0/uidom/dom/src/__init__.py
--rw-r--r--   0        0        0    14370 2023-05-09 20:03:33.062191 uidom-0.2a0/uidom/dom/src/component.py
--rw-r--r--   0        0        0     2188 2023-04-30 13:08:13.941319 uidom-0.2a0/uidom/dom/src/csstags.py
--rw-r--r--   0        0        0     3926 2023-04-28 22:16:02.820670 uidom-0.2a0/uidom/dom/src/dom1core.py
--rw-r--r--   0        0        0    16849 2023-05-09 16:40:11.620271 uidom-0.2a0/uidom/dom/src/dom_tag.py
--rw-r--r--   0        0        0    31872 2023-05-08 10:55:40.270991 uidom-0.2a0/uidom/dom/src/ext.py
--rw-r--r--   0        0        0     7837 2023-05-09 12:02:36.374388 uidom-0.2a0/uidom/dom/src/html_string.py
--rw-r--r--   0        0        0    29966 2023-05-06 16:54:04.821779 uidom-0.2a0/uidom/dom/src/htmltags.py
--rw-r--r--   0        0        0     5048 2023-04-28 12:53:57.974327 uidom-0.2a0/uidom/dom/src/jinjatags.py
--rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.2a0/uidom/dom/src/main.py
--rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.2a0/uidom/dom/src/parse_html.py
--rw-r--r--   0        0        0     2836 2023-05-05 16:26:47.195943 uidom-0.2a0/uidom/dom/src/pythontags.py
--rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.2a0/uidom/dom/src/sphinxtags.py
--rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.2a0/uidom/dom/src/svgtags.py
--rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.2a0/uidom/dom/src/utils/__init__.py
--rw-r--r--   0        0        0     4330 2023-05-09 05:24:01.353063 uidom-0.2a0/uidom/dom/src/utils/dom_util.py
--rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.2a0/uidom/dom/src/utils/sheets.py
--rw-r--r--   0        0        0     6623 2023-04-28 14:41:04.189760 uidom-0.2a0/uidom/dom/src/ws_rpc.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.2a0/uidom/dom/src/xmltags.py
--rw-r--r--   0        0        0    16753 2023-04-26 07:43:57.647609 uidom-0.2a0/uidom/dom/ui.py
--rw-r--r--   0        0        0     3921 2023-03-17 15:40:20.920740 uidom-0.2a0/uidom/dom/uniqueid.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.2a0/uidom/edge_db/__init__.py
--rw-r--r--   0        0        0     9912 2023-03-26 09:48:59.256451 uidom-0.2a0/uidom/edge_db/ql.py
--rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.2a0/uidom/elements/__init__.py
--rw-r--r--   0        0        0     4950 2023-04-27 19:01:56.240091 uidom-0.2a0/uidom/elements/booleans.py
--rw-r--r--   0        0        0     4067 2023-03-14 11:52:41.667372 uidom-0.2a0/uidom/elements/buttons.py
--rw-r--r--   0        0        0    12944 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/elements/chars.py
--rw-r--r--   0        0        0      741 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/elements/dates.py
--rw-r--r--   0        0        0     1903 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/elements/enums.py
--rw-r--r--   0        0        0     5512 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/elements/floats.py
--rw-r--r--   0        0        0     8833 2023-04-22 19:36:12.299643 uidom-0.2a0/uidom/elements/integers.py
--rw-r--r--   0        0        0      908 2023-03-14 11:52:41.623355 uidom-0.2a0/uidom/examples/links.py
--rw-r--r--   0        0        0     2685 2023-04-08 22:55:33.640049 uidom-0.2a0/uidom/examples/toggle.py
--rw-r--r--   0        0        0      157 2023-03-27 08:33:16.449491 uidom-0.2a0/uidom/reloader/__init__.py
--rw-r--r--   0        0        0     3945 2023-04-29 11:35:21.410489 uidom-0.2a0/uidom/reloader/_app.py
--rw-r--r--   0        0        0      158 2023-03-26 20:17:15.474214 uidom-0.2a0/uidom/reloader/_models.py
--rw-r--r--   0        0        0     1320 2022-11-13 21:32:18.000000 uidom-0.2a0/uidom/reloader/_notify.py
--rw-r--r--   0        0        0       83 2023-05-02 15:38:28.533313 uidom-0.2a0/uidom/reloader/_types.py
--rw-r--r--   0        0        0     2031 2023-03-26 05:34:24.365178 uidom-0.2a0/uidom/reloader/_watch.py
--rw-r--r--   0        0        0     1626 2023-03-26 14:13:50.090675 uidom-0.2a0/uidom/reloader/script/reloader.js
--rw-r--r--   0        0        0      118 2023-04-08 11:27:56.180219 uidom-0.2a0/uidom/response/__init__.py
--rw-r--r--   0        0        0     3264 2023-03-17 13:35:31.999152 uidom-0.2a0/uidom/response/starlette.py
--rw-r--r--   0        0        0      118 2023-04-08 11:28:05.452370 uidom-0.2a0/uidom/routing/__init__.py
--rw-r--r--   0        0        0     6890 2023-04-08 11:28:44.765011 uidom-0.2a0/uidom/routing/fastapi.py
--rw-r--r--   0        0        0      768 2023-04-12 16:05:27.697495 uidom-0.2a0/uidom/scripts/__init__.py
--rw-r--r--   0        0        0     4560 2023-04-22 05:04:01.008470 uidom-0.2a0/uidom/scripts/cdn.py
--rw-r--r--   0        0        0    11947 2023-04-11 21:23:32.778552 uidom-0.2a0/uidom/scripts/xcomponent.js
--rw-r--r--   0        0        0      197 2023-05-04 14:36:51.260441 uidom-0.2a0/uidom/settings/__init__.py
--rw-r--r--   0        0        0     8105 2023-05-05 19:27:38.753086 uidom-0.2a0/uidom/settings/commands.py
--rw-r--r--   0        0        0     8691 2023-05-05 06:53:34.240389 uidom-0.2a0/uidom/settings/document.py
--rw-r--r--   0        0        0     4201 2023-05-03 20:51:42.982950 uidom-0.2a0/uidom/settings/paths.py
--rw-r--r--   0        0        0      219 2023-03-16 11:20:30.258980 uidom-0.2a0/uidom/slots/__init__.py
--rw-r--r--   0        0        0     1968 2023-05-01 05:14:03.631193 uidom-0.2a0/uidom/slots/custom_element_slot.py
--rw-r--r--   0        0        0     1594 2023-03-16 11:17:14.416579 uidom-0.2a0/uidom/slots/web_component_slot.py
--rw-r--r--   0        0        0      118 2023-05-04 22:15:22.715253 uidom-0.2a0/uidom/utils/__init__.py
--rwxr-xr-x   0        0        0     5295 2023-05-05 08:54:45.688998 uidom-0.2a0/uidom/utils/functional.py
--rw-r--r--   0        0        0     1320 2023-05-05 05:50:42.208687 uidom-0.2a0/uidom/utils/logger.py
--rw-r--r--   0        0        0     6458 2023-05-05 15:56:41.572034 uidom-0.2a0/uidom/utils/parameters.py
--rw-r--r--   0        0        0      337 2023-05-03 18:21:26.051460 uidom-0.2a0/uidom/web_io/__init__.py
--rw-r--r--   0        0        0    12444 2023-05-03 15:26:45.936106 uidom-0.2a0/uidom/web_io/_adapter.py
--rw-r--r--   0        0        0     7291 2023-05-03 18:18:45.850893 uidom-0.2a0/uidom/web_io/_events.py
--rw-r--r--   0        0        0     1467 2023-04-22 19:48:06.786062 uidom-0.2a0/uidom/web_io/_protocol.py
--rw-r--r--   0        0        0      353 2023-04-22 11:35:31.981365 uidom-0.2a0/uidom/web_io/_types.py
--rw-r--r--   0        0        0     6849 1970-01-01 00:00:00.000000 uidom-0.2a0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.2a1/LICENSE
+-rw-r--r--   0        0        0     5686 2023-05-01 05:55:18.794343 uidom-0.2a1/README.md
+-rw-r--r--   0        0        0     1271 2023-05-10 12:10:59.233347 uidom-0.2a1/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-10 12:00:14.418589 uidom-0.2a1/uidom/__init__.py
+-rw-r--r--   0        0        0     1067 2023-05-09 19:55:16.645883 uidom-0.2a1/uidom/cli/__init__.py
+-rw-r--r--   0        0        0    12108 2023-05-05 19:23:34.126884 uidom-0.2a1/uidom/cli/_cli.py
+-rw-r--r--   0        0        0     6773 2023-05-10 12:10:44.741105 uidom-0.2a1/uidom/cli/cli.py
+-rw-r--r--   0        0        0      517 2023-05-09 11:52:14.395273 uidom-0.2a1/uidom/dom/__init__.py
+-rw-r--r--   0        0        0     4944 2023-05-09 14:03:20.721191 uidom-0.2a1/uidom/dom/htmldocument.py
+-rw-r--r--   0        0        0     5924 2023-05-09 16:54:51.261005 uidom-0.2a1/uidom/dom/htmlelement.py
+-rw-r--r--   0        0        0    42978 2023-03-25 19:14:55.486184 uidom-0.2a1/uidom/dom/icons.py
+-rw-r--r--   0        0        0     1363 2023-03-14 11:52:41.187178 uidom-0.2a1/uidom/dom/jinja.py
+-rwxr-xr-x   0        0        0      304 2022-07-09 13:34:38.382685 uidom-0.2a1/uidom/dom/src/__init__.py
+-rw-r--r--   0        0        0    14512 2023-05-10 11:50:34.948921 uidom-0.2a1/uidom/dom/src/component.py
+-rw-r--r--   0        0        0     2188 2023-04-30 13:08:13.941319 uidom-0.2a1/uidom/dom/src/csstags.py
+-rw-r--r--   0        0        0     3926 2023-04-28 22:16:02.820670 uidom-0.2a1/uidom/dom/src/dom1core.py
+-rw-r--r--   0        0        0    16849 2023-05-09 16:40:11.620271 uidom-0.2a1/uidom/dom/src/dom_tag.py
+-rw-r--r--   0        0        0    31872 2023-05-08 10:55:40.270991 uidom-0.2a1/uidom/dom/src/ext.py
+-rw-r--r--   0        0        0     7837 2023-05-09 12:02:36.374388 uidom-0.2a1/uidom/dom/src/html_string.py
+-rw-r--r--   0        0        0    29966 2023-05-06 16:54:04.821779 uidom-0.2a1/uidom/dom/src/htmltags.py
+-rw-r--r--   0        0        0     5048 2023-04-28 12:53:57.974327 uidom-0.2a1/uidom/dom/src/jinjatags.py
+-rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.2a1/uidom/dom/src/main.py
+-rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.2a1/uidom/dom/src/parse_html.py
+-rw-r--r--   0        0        0     2836 2023-05-05 16:26:47.195943 uidom-0.2a1/uidom/dom/src/pythontags.py
+-rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.2a1/uidom/dom/src/sphinxtags.py
+-rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.2a1/uidom/dom/src/svgtags.py
+-rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.2a1/uidom/dom/src/utils/__init__.py
+-rw-r--r--   0        0        0     4330 2023-05-09 05:24:01.353063 uidom-0.2a1/uidom/dom/src/utils/dom_util.py
+-rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.2a1/uidom/dom/src/utils/sheets.py
+-rw-r--r--   0        0        0     6623 2023-04-28 14:41:04.189760 uidom-0.2a1/uidom/dom/src/ws_rpc.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.2a1/uidom/dom/src/xmltags.py
+-rw-r--r--   0        0        0    16753 2023-04-26 07:43:57.647609 uidom-0.2a1/uidom/dom/ui.py
+-rw-r--r--   0        0        0     3921 2023-03-17 15:40:20.920740 uidom-0.2a1/uidom/dom/uniqueid.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.2a1/uidom/edge_db/__init__.py
+-rw-r--r--   0        0        0     9912 2023-03-26 09:48:59.256451 uidom-0.2a1/uidom/edge_db/ql.py
+-rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.2a1/uidom/elements/__init__.py
+-rw-r--r--   0        0        0     4950 2023-04-27 19:01:56.240091 uidom-0.2a1/uidom/elements/booleans.py
+-rw-r--r--   0        0        0     4067 2023-03-14 11:52:41.667372 uidom-0.2a1/uidom/elements/buttons.py
+-rw-r--r--   0        0        0    12944 2023-03-14 11:52:41.187178 uidom-0.2a1/uidom/elements/chars.py
+-rw-r--r--   0        0        0      741 2023-03-14 11:52:41.187178 uidom-0.2a1/uidom/elements/dates.py
+-rw-r--r--   0        0        0     1903 2023-03-14 11:52:41.187178 uidom-0.2a1/uidom/elements/enums.py
+-rw-r--r--   0        0        0     5512 2023-03-14 11:52:41.187178 uidom-0.2a1/uidom/elements/floats.py
+-rw-r--r--   0        0        0     8833 2023-04-22 19:36:12.299643 uidom-0.2a1/uidom/elements/integers.py
+-rw-r--r--   0        0        0      908 2023-03-14 11:52:41.623355 uidom-0.2a1/uidom/examples/links.py
+-rw-r--r--   0        0        0     2685 2023-04-08 22:55:33.640049 uidom-0.2a1/uidom/examples/toggle.py
+-rw-r--r--   0        0        0      157 2023-03-27 08:33:16.449491 uidom-0.2a1/uidom/reloader/__init__.py
+-rw-r--r--   0        0        0     3945 2023-04-29 11:35:21.410489 uidom-0.2a1/uidom/reloader/_app.py
+-rw-r--r--   0        0        0      158 2023-03-26 20:17:15.474214 uidom-0.2a1/uidom/reloader/_models.py
+-rw-r--r--   0        0        0     1320 2022-11-13 21:32:18.000000 uidom-0.2a1/uidom/reloader/_notify.py
+-rw-r--r--   0        0        0       83 2023-05-02 15:38:28.533313 uidom-0.2a1/uidom/reloader/_types.py
+-rw-r--r--   0        0        0     2031 2023-03-26 05:34:24.365178 uidom-0.2a1/uidom/reloader/_watch.py
+-rw-r--r--   0        0        0     1626 2023-03-26 14:13:50.090675 uidom-0.2a1/uidom/reloader/script/reloader.js
+-rw-r--r--   0        0        0      118 2023-04-08 11:27:56.180219 uidom-0.2a1/uidom/response/__init__.py
+-rw-r--r--   0        0        0     3264 2023-03-17 13:35:31.999152 uidom-0.2a1/uidom/response/starlette.py
+-rw-r--r--   0        0        0      118 2023-04-08 11:28:05.452370 uidom-0.2a1/uidom/routing/__init__.py
+-rw-r--r--   0        0        0     6329 2023-05-10 11:27:41.741983 uidom-0.2a1/uidom/routing/fastapi.py
+-rw-r--r--   0        0        0      768 2023-04-12 16:05:27.697495 uidom-0.2a1/uidom/scripts/__init__.py
+-rw-r--r--   0        0        0     4560 2023-04-22 05:04:01.008470 uidom-0.2a1/uidom/scripts/cdn.py
+-rw-r--r--   0        0        0    11947 2023-04-11 21:23:32.778552 uidom-0.2a1/uidom/scripts/xcomponent.js
+-rw-r--r--   0        0        0      197 2023-05-04 14:36:51.260441 uidom-0.2a1/uidom/settings/__init__.py
+-rw-r--r--   0        0        0     8105 2023-05-05 19:27:38.753086 uidom-0.2a1/uidom/settings/commands.py
+-rw-r--r--   0        0        0     8691 2023-05-05 06:53:34.240389 uidom-0.2a1/uidom/settings/document.py
+-rw-r--r--   0        0        0     4201 2023-05-03 20:51:42.982950 uidom-0.2a1/uidom/settings/paths.py
+-rw-r--r--   0        0        0      219 2023-03-16 11:20:30.258980 uidom-0.2a1/uidom/slots/__init__.py
+-rw-r--r--   0        0        0     1968 2023-05-01 05:14:03.631193 uidom-0.2a1/uidom/slots/custom_element_slot.py
+-rw-r--r--   0        0        0     1594 2023-03-16 11:17:14.416579 uidom-0.2a1/uidom/slots/web_component_slot.py
+-rw-r--r--   0        0        0      118 2023-05-04 22:15:22.715253 uidom-0.2a1/uidom/utils/__init__.py
+-rwxr-xr-x   0        0        0     5295 2023-05-05 08:54:45.688998 uidom-0.2a1/uidom/utils/functional.py
+-rw-r--r--   0        0        0     1320 2023-05-05 05:50:42.208687 uidom-0.2a1/uidom/utils/logger.py
+-rw-r--r--   0        0        0     6458 2023-05-05 15:56:41.572034 uidom-0.2a1/uidom/utils/parameters.py
+-rw-r--r--   0        0        0      337 2023-05-03 18:21:26.051460 uidom-0.2a1/uidom/web_io/__init__.py
+-rw-r--r--   0        0        0    12444 2023-05-03 15:26:45.936106 uidom-0.2a1/uidom/web_io/_adapter.py
+-rw-r--r--   0        0        0     7291 2023-05-03 18:18:45.850893 uidom-0.2a1/uidom/web_io/_events.py
+-rw-r--r--   0        0        0     1467 2023-04-22 19:48:06.786062 uidom-0.2a1/uidom/web_io/_protocol.py
+-rw-r--r--   0        0        0      353 2023-04-22 11:35:31.981365 uidom-0.2a1/uidom/web_io/_types.py
+-rw-r--r--   0        0        0     6849 1970-01-01 00:00:00.000000 uidom-0.2a1/PKG-INFO
```

### Comparing `uidom-0.2a0/LICENSE` & `uidom-0.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/README.md` & `uidom-0.2a1/README.md`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/pyproject.toml` & `uidom-0.2a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uidom"
-version = "0.2a0"
+version = "0.2a1"
 description = "HTML library"
 authors = ["bitplorer <bitplorer@outlook.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `uidom-0.2a0/uidom/cli/__init__.py` & `uidom-0.2a1/uidom/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/cli/_cli.py` & `uidom-0.2a1/uidom/cli/_cli.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/cli/cli.py` & `uidom-0.2a1/uidom/cli/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,36 +49,42 @@
     await send({"type": "http.response.body", "body": str(Index("Hello, world!")).encode()})
     """
 )
 
 
 SERVER_TEMP = _Template(
     """
-
-import uvicorn
-
+HAS_UVICORN = True
+ 
+try:
+    import uvicorn
+except ImportError:
+    pass
+    HAS_UVICORN = True
+    
 if __name__ == "__main__":
-    uvicorn.run(
-        "$variable::app_name.api:home",
-        host="127.0.0.1",
-        port=8081,
-        reload=True,
-        # ssl_keyfile='../$variable::app_name/key.pem',
-        # ssl_certfile='../$variable::app_name/cert.pem'
-    )
+    if HAS_UVICORN:
+        uvicorn.run(
+            "$variable::app_name.api:home",
+            host="127.0.0.1",
+            port=8081,
+            reload=True,
+            # ssl_keyfile='../$variable::app_name/key.pem',
+            # ssl_certfile='../$variable::app_name/cert.pem'
+        )
     """
 )
 
 
 DOCUMENT_TEMP = _Template(
     """
-from $variable::app_name import settings
-from $variable::app_name.tailwindcss import tailwind
 from uidom import UiDOM
 from uidom.dom import link, raw
+from $variable::app_name import settings
+from $variable::app_name.tailwindcss import tailwind
 
 __all__ = ["document"]
 
 
 document = UiDOM(
     webassets=settings.webassets,
     head=[
```

### Comparing `uidom-0.2a0/uidom/dom/__init__.py` & `uidom-0.2a1/uidom/dom/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/htmldocument.py` & `uidom-0.2a1/uidom/dom/htmldocument.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/htmlelement.py` & `uidom-0.2a1/uidom/dom/htmlelement.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/icons.py` & `uidom-0.2a1/uidom/dom/icons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/jinja.py` & `uidom-0.2a1/uidom/dom/jinja.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/component.py` & `uidom-0.2a1/uidom/dom/src/component.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     parent: Union[html_tags.dom_tag, None] = field(init=False, default=None)
     document: Union[html_tags.dom_tag, None] = field(init=False, default=None)
     files_directory: Union[str, Path, None] = field(init=False, default=None)
     escape_string: bool = field(init=False, default=True)
     string_is_markdown: bool = field(init=False, default=False)
 
     def __init__(self, *args, **kwargs):
+        global markdown
+        markdown = kwargs.pop("markdown", None) or markdown
+        markdown = getattr(markdown, "convert", markdown)
         # first we get the child from the render method and sanitize it.
         child = self.render(*args, **kwargs)
 
         if isinstance(child, str):
             if self.string_is_markdown:
                 child = (
                     markdown(child) if self.escape_string else unescape(markdown(child))
```

### Comparing `uidom-0.2a0/uidom/dom/src/csstags.py` & `uidom-0.2a1/uidom/dom/src/csstags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/dom1core.py` & `uidom-0.2a1/uidom/dom/src/dom1core.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/dom_tag.py` & `uidom-0.2a1/uidom/dom/src/dom_tag.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/ext.py` & `uidom-0.2a1/uidom/dom/src/ext.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/html_string.py` & `uidom-0.2a1/uidom/dom/src/html_string.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/htmltags.py` & `uidom-0.2a1/uidom/dom/src/htmltags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/jinjatags.py` & `uidom-0.2a1/uidom/dom/src/jinjatags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/parse_html.py` & `uidom-0.2a1/uidom/dom/src/parse_html.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/pythontags.py` & `uidom-0.2a1/uidom/dom/src/pythontags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/sphinxtags.py` & `uidom-0.2a1/uidom/dom/src/sphinxtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/svgtags.py` & `uidom-0.2a1/uidom/dom/src/svgtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/utils/dom_util.py` & `uidom-0.2a1/uidom/dom/src/utils/dom_util.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/utils/sheets.py` & `uidom-0.2a1/uidom/dom/src/utils/sheets.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/src/ws_rpc.py` & `uidom-0.2a1/uidom/dom/src/ws_rpc.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/ui.py` & `uidom-0.2a1/uidom/dom/ui.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/dom/uniqueid.py` & `uidom-0.2a1/uidom/dom/uniqueid.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/edge_db/ql.py` & `uidom-0.2a1/uidom/edge_db/ql.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/elements/booleans.py` & `uidom-0.2a1/uidom/elements/booleans.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/elements/buttons.py` & `uidom-0.2a1/uidom/elements/buttons.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/elements/chars.py` & `uidom-0.2a1/uidom/elements/chars.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/elements/dates.py` & `uidom-0.2a1/uidom/elements/dates.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/elements/enums.py` & `uidom-0.2a1/uidom/elements/enums.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/elements/floats.py` & `uidom-0.2a1/uidom/elements/floats.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/elements/integers.py` & `uidom-0.2a1/uidom/elements/integers.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/examples/links.py` & `uidom-0.2a1/uidom/examples/links.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/examples/toggle.py` & `uidom-0.2a1/uidom/examples/toggle.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/reloader/_app.py` & `uidom-0.2a1/uidom/reloader/_app.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/reloader/_notify.py` & `uidom-0.2a1/uidom/reloader/_notify.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/reloader/_watch.py` & `uidom-0.2a1/uidom/reloader/_watch.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/reloader/script/reloader.js` & `uidom-0.2a1/uidom/reloader/script/reloader.js`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/response/starlette.py` & `uidom-0.2a1/uidom/response/starlette.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/routing/fastapi.py` & `uidom-0.2a1/uidom/routing/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,150 +1,148 @@
 # Copyright (c) 2023 UiDOM
 #
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 __all__ = ["HTMLRoute", "StreamingRoute"]
 
-try:
-    from enum import Enum
-    from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Type, Union
-
-    from fastapi import params, routing
-    from fastapi.datastructures import Default, DefaultPlaceholder
-    from fastapi.encoders import DictIntStrAny, SetIntStr
-    from fastapi.utils import generate_unique_id
-    from starlette.responses import JSONResponse, Response
-    from starlette.routing import BaseRoute
-
-    from uidom.response.starlette import async_html_response, html_response
-
-    class HTMLRoute(routing.APIRoute):
-        def __init__(
-            self,
-            path: str,
-            endpoint: Callable[..., Any],
-            *,
-            response_model: Optional[Type[Any]] = None,
-            status_code: Optional[int] = None,
-            tags: Optional[List[Union[str, Enum]]] = None,
-            dependencies: Optional[Sequence[params.Depends]] = None,
-            summary: Optional[str] = None,
-            description: Optional[str] = None,
-            response_description: str = "Successful Response",
-            responses: Optional[Dict[Union[int, str], Dict[str, Any]]] = None,
-            deprecated: Optional[bool] = None,
-            name: Optional[str] = None,
-            methods: Optional[Union[Set[str], List[str]]] = None,
-            operation_id: Optional[str] = None,
-            response_model_include: Optional[Union[SetIntStr, DictIntStrAny]] = None,
-            response_model_exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None,
-            response_model_by_alias: bool = True,
-            response_model_exclude_unset: bool = False,
-            response_model_exclude_defaults: bool = False,
-            response_model_exclude_none: bool = False,
-            include_in_schema: bool = True,
-            response_class: Union[Type[Response], DefaultPlaceholder] = Default(
-                JSONResponse
-            ),
-            dependency_overrides_provider: Optional[Any] = None,
-            callbacks: Optional[List[BaseRoute]] = None,
-            openapi_extra: Optional[Dict[str, Any]] = None,
-            generate_unique_id_function: Union[
-                Callable[["routing.APIRoute"], str], DefaultPlaceholder
-            ] = Default(generate_unique_id)
-        ) -> None:
-            super().__init__(
-                path=path,
-                endpoint=html_response(endpoint),
-                response_model=response_model,
-                status_code=status_code,
-                tags=tags,
-                dependencies=dependencies,
-                summary=summary,
-                description=description,
-                response_description=response_description,
-                responses=responses,
-                deprecated=deprecated,
-                name=name,
-                methods=methods,
-                operation_id=operation_id,
-                response_model_include=response_model_include,
-                response_model_exclude=response_model_exclude,
-                response_model_by_alias=response_model_by_alias,
-                response_model_exclude_unset=response_model_exclude_unset,
-                response_model_exclude_defaults=response_model_exclude_defaults,
-                response_model_exclude_none=response_model_exclude_none,
-                include_in_schema=include_in_schema,
-                response_class=response_class,
-                dependency_overrides_provider=dependency_overrides_provider,
-                callbacks=callbacks,
-                openapi_extra=openapi_extra,
-                generate_unique_id_function=generate_unique_id_function,
-            )
-
-    class StreamingRoute(routing.APIRoute):
-        def __init__(
-            self,
-            path: str,
-            endpoint: Callable[..., Any],
-            *,
-            response_model: Optional[Type[Any]] = None,
-            status_code: Optional[int] = None,
-            tags: Optional[List[Union[str, Enum]]] = None,
-            dependencies: Optional[Sequence[params.Depends]] = None,
-            summary: Optional[str] = None,
-            description: Optional[str] = None,
-            response_description: str = "Successful Response",
-            responses: Optional[Dict[Union[int, str], Dict[str, Any]]] = None,
-            deprecated: Optional[bool] = None,
-            name: Optional[str] = None,
-            methods: Optional[Union[Set[str], List[str]]] = None,
-            operation_id: Optional[str] = None,
-            response_model_include: Optional[Union[SetIntStr, DictIntStrAny]] = None,
-            response_model_exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None,
-            response_model_by_alias: bool = True,
-            response_model_exclude_unset: bool = False,
-            response_model_exclude_defaults: bool = False,
-            response_model_exclude_none: bool = False,
-            include_in_schema: bool = True,
-            response_class: Union[Type[Response], DefaultPlaceholder] = Default(
-                JSONResponse
-            ),
-            dependency_overrides_provider: Optional[Any] = None,
-            callbacks: Optional[List[BaseRoute]] = None,
-            openapi_extra: Optional[Dict[str, Any]] = None,
-            generate_unique_id_function: Union[
-                Callable[["routing.APIRoute"], str], DefaultPlaceholder
-            ] = Default(generate_unique_id)
-        ) -> None:
-            super().__init__(
-                path=path,
-                endpoint=async_html_response(endpoint),
-                response_model=response_model,
-                status_code=status_code,
-                tags=tags,
-                dependencies=dependencies,
-                summary=summary,
-                description=description,
-                response_description=response_description,
-                responses=responses,
-                deprecated=deprecated,
-                name=name,
-                methods=methods,
-                operation_id=operation_id,
-                response_model_include=response_model_include,
-                response_model_exclude=response_model_exclude,
-                response_model_by_alias=response_model_by_alias,
-                response_model_exclude_unset=response_model_exclude_unset,
-                response_model_exclude_defaults=response_model_exclude_defaults,
-                response_model_exclude_none=response_model_exclude_none,
-                include_in_schema=include_in_schema,
-                response_class=response_class,
-                dependency_overrides_provider=dependency_overrides_provider,
-                callbacks=callbacks,
-                openapi_extra=openapi_extra,
-                generate_unique_id_function=generate_unique_id_function,
-            )
+from enum import Enum
+from typing import Any, Callable, Dict, List, Optional, Sequence, Set, Type, Union
 
-except:
-    pass
+from fastapi import params, routing
+from fastapi.datastructures import Default, DefaultPlaceholder
+from fastapi.encoders import DictIntStrAny, SetIntStr
+from fastapi.utils import generate_unique_id
+from starlette.responses import JSONResponse, Response
+from starlette.routing import BaseRoute
+
+from uidom.response.starlette import async_html_response, html_response
+
+
+class HTMLRoute(routing.APIRoute):
+    def __init__(
+        self,
+        path: str,
+        endpoint: Callable[..., Any],
+        *,
+        response_model: Optional[Type[Any]] = None,
+        status_code: Optional[int] = None,
+        tags: Optional[List[Union[str, Enum]]] = None,
+        dependencies: Optional[Sequence[params.Depends]] = None,
+        summary: Optional[str] = None,
+        description: Optional[str] = None,
+        response_description: str = "Successful Response",
+        responses: Optional[Dict[Union[int, str], Dict[str, Any]]] = None,
+        deprecated: Optional[bool] = None,
+        name: Optional[str] = None,
+        methods: Optional[Union[Set[str], List[str]]] = None,
+        operation_id: Optional[str] = None,
+        response_model_include: Optional[Union[SetIntStr, DictIntStrAny]] = None,
+        response_model_exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None,
+        response_model_by_alias: bool = True,
+        response_model_exclude_unset: bool = False,
+        response_model_exclude_defaults: bool = False,
+        response_model_exclude_none: bool = False,
+        include_in_schema: bool = True,
+        response_class: Union[Type[Response], DefaultPlaceholder] = Default(
+            JSONResponse
+        ),
+        dependency_overrides_provider: Optional[Any] = None,
+        callbacks: Optional[List[BaseRoute]] = None,
+        openapi_extra: Optional[Dict[str, Any]] = None,
+        generate_unique_id_function: Union[
+            Callable[["routing.APIRoute"], str], DefaultPlaceholder
+        ] = Default(generate_unique_id)
+    ) -> None:
+        super().__init__(
+            path=path,
+            endpoint=html_response(endpoint),
+            response_model=response_model,
+            status_code=status_code,
+            tags=tags,
+            dependencies=dependencies,
+            summary=summary,
+            description=description,
+            response_description=response_description,
+            responses=responses,
+            deprecated=deprecated,
+            name=name,
+            methods=methods,
+            operation_id=operation_id,
+            response_model_include=response_model_include,
+            response_model_exclude=response_model_exclude,
+            response_model_by_alias=response_model_by_alias,
+            response_model_exclude_unset=response_model_exclude_unset,
+            response_model_exclude_defaults=response_model_exclude_defaults,
+            response_model_exclude_none=response_model_exclude_none,
+            include_in_schema=include_in_schema,
+            response_class=response_class,
+            dependency_overrides_provider=dependency_overrides_provider,
+            callbacks=callbacks,
+            openapi_extra=openapi_extra,
+            generate_unique_id_function=generate_unique_id_function,
+        )
+
+
+class StreamingRoute(routing.APIRoute):
+    def __init__(
+        self,
+        path: str,
+        endpoint: Callable[..., Any],
+        *,
+        response_model: Optional[Type[Any]] = None,
+        status_code: Optional[int] = None,
+        tags: Optional[List[Union[str, Enum]]] = None,
+        dependencies: Optional[Sequence[params.Depends]] = None,
+        summary: Optional[str] = None,
+        description: Optional[str] = None,
+        response_description: str = "Successful Response",
+        responses: Optional[Dict[Union[int, str], Dict[str, Any]]] = None,
+        deprecated: Optional[bool] = None,
+        name: Optional[str] = None,
+        methods: Optional[Union[Set[str], List[str]]] = None,
+        operation_id: Optional[str] = None,
+        response_model_include: Optional[Union[SetIntStr, DictIntStrAny]] = None,
+        response_model_exclude: Optional[Union[SetIntStr, DictIntStrAny]] = None,
+        response_model_by_alias: bool = True,
+        response_model_exclude_unset: bool = False,
+        response_model_exclude_defaults: bool = False,
+        response_model_exclude_none: bool = False,
+        include_in_schema: bool = True,
+        response_class: Union[Type[Response], DefaultPlaceholder] = Default(
+            JSONResponse
+        ),
+        dependency_overrides_provider: Optional[Any] = None,
+        callbacks: Optional[List[BaseRoute]] = None,
+        openapi_extra: Optional[Dict[str, Any]] = None,
+        generate_unique_id_function: Union[
+            Callable[["routing.APIRoute"], str], DefaultPlaceholder
+        ] = Default(generate_unique_id)
+    ) -> None:
+        super().__init__(
+            path=path,
+            endpoint=async_html_response(endpoint),
+            response_model=response_model,
+            status_code=status_code,
+            tags=tags,
+            dependencies=dependencies,
+            summary=summary,
+            description=description,
+            response_description=response_description,
+            responses=responses,
+            deprecated=deprecated,
+            name=name,
+            methods=methods,
+            operation_id=operation_id,
+            response_model_include=response_model_include,
+            response_model_exclude=response_model_exclude,
+            response_model_by_alias=response_model_by_alias,
+            response_model_exclude_unset=response_model_exclude_unset,
+            response_model_exclude_defaults=response_model_exclude_defaults,
+            response_model_exclude_none=response_model_exclude_none,
+            include_in_schema=include_in_schema,
+            response_class=response_class,
+            dependency_overrides_provider=dependency_overrides_provider,
+            callbacks=callbacks,
+            openapi_extra=openapi_extra,
+            generate_unique_id_function=generate_unique_id_function,
+        )
```

### Comparing `uidom-0.2a0/uidom/scripts/__init__.py` & `uidom-0.2a1/uidom/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/scripts/cdn.py` & `uidom-0.2a1/uidom/scripts/cdn.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/scripts/xcomponent.js` & `uidom-0.2a1/uidom/scripts/xcomponent.js`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/settings/commands.py` & `uidom-0.2a1/uidom/settings/commands.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/settings/document.py` & `uidom-0.2a1/uidom/settings/document.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/settings/paths.py` & `uidom-0.2a1/uidom/settings/paths.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/slots/custom_element_slot.py` & `uidom-0.2a1/uidom/slots/custom_element_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/slots/web_component_slot.py` & `uidom-0.2a1/uidom/slots/web_component_slot.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/utils/functional.py` & `uidom-0.2a1/uidom/utils/functional.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/utils/logger.py` & `uidom-0.2a1/uidom/utils/logger.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/utils/parameters.py` & `uidom-0.2a1/uidom/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/web_io/_adapter.py` & `uidom-0.2a1/uidom/web_io/_adapter.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/web_io/_events.py` & `uidom-0.2a1/uidom/web_io/_events.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/uidom/web_io/_protocol.py` & `uidom-0.2a1/uidom/web_io/_protocol.py`

 * *Files identical despite different names*

### Comparing `uidom-0.2a0/PKG-INFO` & `uidom-0.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uidom
-Version: 0.2a0
+Version: 0.2a1
 Summary: HTML library
 License: MIT
 Author: bitplorer
 Author-email: bitplorer@outlook.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

