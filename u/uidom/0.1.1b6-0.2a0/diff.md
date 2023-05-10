# Comparing `tmp/uidom-0.1.1b6.tar.gz` & `tmp/uidom-0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uidom-0.1.1b6.tar", max compression
+gzip compressed data, was "uidom-0.2a0.tar", max compression
```

## Comparing `uidom-0.1.1b6.tar` & `uidom-0.2a0.tar`

### file list

```diff
@@ -1,110 +1,76 @@
--rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.1.1b6/LICENSE
--rw-r--r--   0        0        0      596 2022-11-20 07:09:31.765793 uidom-0.1.1b6/pyproject.toml
--rw-r--r--   0        0        0      196 2022-11-20 07:09:37.762032 uidom-0.1.1b6/uidom/__init__.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:19.547307 uidom-0.1.1b6/uidom/asgi_plugs/__init__.py
--rw-r--r--   0        0        0     1046 2022-07-09 13:34:04.747809 uidom-0.1.1b6/uidom/asgi_plugs/asgi_header.py
--rw-r--r--   0        0        0      145 2022-07-09 13:34:06.015765 uidom-0.1.1b6/uidom/components/__init__.py
--rw-r--r--   0        0        0     1717 2022-07-10 00:50:55.565557 uidom-0.1.1b6/uidom/components/accordian.py
--rw-r--r--   0        0        0      183 2022-07-09 13:34:03.567849 uidom-0.1.1b6/uidom/components/alpinejs/__init__.py
--rw-r--r--   0        0        0     2119 2022-07-10 00:46:01.772286 uidom-0.1.1b6/uidom/components/alpinejs/slot_element.py
--rw-r--r--   0        0        0     1605 2022-07-31 05:33:22.833084 uidom-0.1.1b6/uidom/components/alpinejs/web_component_slot.py
--rw-r--r--   0        0        0      120 2022-07-09 13:34:06.443751 uidom-0.1.1b6/uidom/components/atoms/__init__.py
--rw-r--r--   0        0        0     2771 2022-07-10 00:50:55.565557 uidom-0.1.1b6/uidom/components/atoms/toggle.py
--rw-r--r--   0        0        0      347 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/components/atoms/xlinks.py
--rw-r--r--   0        0        0      834 2022-07-09 14:45:47.892447 uidom-0.1.1b6/uidom/dom/__init__.py
--rw-r--r--   0        0        0      989 2022-07-10 00:50:55.565557 uidom-0.1.1b6/uidom/dom/css.py
--rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.1.1b6/uidom/dom/elements/__init__.py
--rw-r--r--   0        0        0     5647 2022-07-26 08:48:47.482856 uidom-0.1.1b6/uidom/dom/elements/booleans.py
--rw-r--r--   0        0        0     4106 2022-07-26 09:00:52.116685 uidom-0.1.1b6/uidom/dom/elements/buttons.py
--rw-r--r--   0        0        0    12983 2022-07-26 09:25:59.575230 uidom-0.1.1b6/uidom/dom/elements/chars.py
--rw-r--r--   0        0        0      749 2022-07-26 09:27:12.630375 uidom-0.1.1b6/uidom/dom/elements/dates.py
--rw-r--r--   0        0        0     1918 2022-07-10 00:35:42.672677 uidom-0.1.1b6/uidom/dom/elements/enums.py
--rw-r--r--   0        0        0     5531 2022-07-26 09:30:49.527774 uidom-0.1.1b6/uidom/dom/elements/floats.py
--rw-r--r--   0        0        0    10664 2022-07-31 05:52:46.311778 uidom-0.1.1b6/uidom/dom/elements/integers.py
--rw-r--r--   0        0        0     6670 2022-11-20 07:03:34.788986 uidom-0.1.1b6/uidom/dom/html_to_dom.py
--rw-r--r--   0        0        0     4423 2022-07-10 00:50:55.561557 uidom-0.1.1b6/uidom/dom/htmldocument.py
--rw-r--r--   0        0        0     6703 2022-11-19 11:57:35.392234 uidom-0.1.1b6/uidom/dom/htmlelement.py
--rw-r--r--   0        0        0      120 2022-07-09 13:34:32.522876 uidom-0.1.1b6/uidom/dom/iconify/__init__.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:15.283450 uidom-0.1.1b6/uidom/dom/iconify/account/__init__.py
--rw-r--r--   0        0        0      120 2022-07-09 13:34:38.666675 uidom-0.1.1b6/uidom/dom/iconify/brands/__init__.py
--rw-r--r--   0        0        0    45104 2022-07-10 00:50:55.561557 uidom-0.1.1b6/uidom/dom/icons.py
--rw-r--r--   0        0        0     1367 2022-07-10 03:35:51.277060 uidom-0.1.1b6/uidom/dom/jinja.py
--rw-r--r--   0        0        0      916 2022-07-10 00:50:55.561557 uidom-0.1.1b6/uidom/dom/links.py
--rwxr-xr-x   0        0        0      304 2022-07-09 13:34:38.382685 uidom-0.1.1b6/uidom/dom/src/__init__.py
--rw-r--r--   0        0        0     3943 2022-07-27 04:02:22.189854 uidom-0.1.1b6/uidom/dom/src/component.py
--rw-r--r--   0        0        0     2016 2022-07-10 00:50:55.561557 uidom-0.1.1b6/uidom/dom/src/csstags.py
--rw-r--r--   0        0        0     2110 2022-07-09 13:34:16.715402 uidom-0.1.1b6/uidom/dom/src/dom1core.py
--rw-r--r--   0        0        0    15571 2022-07-27 03:58:00.751070 uidom-0.1.1b6/uidom/dom/src/dom_tag.py
--rw-r--r--   0        0        0    22115 2022-08-11 13:44:50.596917 uidom-0.1.1b6/uidom/dom/src/ext.py
--rw-r--r--   0        0        0    31116 2022-07-10 00:50:55.561557 uidom-0.1.1b6/uidom/dom/src/htmltags.py
--rw-r--r--   0        0        0     5641 2022-09-18 09:16:24.056395 uidom-0.1.1b6/uidom/dom/src/jinjatags.py
--rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.1.1b6/uidom/dom/src/main.py
--rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.1.1b6/uidom/dom/src/parse_html.py
--rw-r--r--   0        0        0     2054 2022-07-10 00:50:55.437557 uidom-0.1.1b6/uidom/dom/src/pythontags.py
--rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.1.1b6/uidom/dom/src/sphinxtags.py
--rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.1.1b6/uidom/dom/src/svgtags.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:42.506551 uidom-0.1.1b6/uidom/dom/src/tests/__init__.py
--rw-r--r--   0        0        0     1144 2022-07-10 03:48:07.030255 uidom-0.1.1b6/uidom/dom/src/tests/jinja_tags_tests.py
--rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.1.1b6/uidom/dom/src/utils/__init__.py
--rw-r--r--   0        0        0     4326 2022-07-10 00:50:55.437557 uidom-0.1.1b6/uidom/dom/src/utils/dom_util.py
--rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.1.1b6/uidom/dom/src/utils/sheets.py
--rw-r--r--   0        0        0      324 2022-07-10 00:50:55.437557 uidom-0.1.1b6/uidom/dom/src/vuetags.py
--rw-r--r--   0        0        0     1329 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/src/vuetifytags.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.1.1b6/uidom/dom/src/xmltags.py
--rw-r--r--   0        0        0      260 2022-07-09 13:34:27.367046 uidom-0.1.1b6/uidom/dom/tailwindcss/__init__.py
--rw-r--r--   0        0        0      121 2022-07-09 13:33:53.612195 uidom-0.1.1b6/uidom/dom/tailwindcss/background/__init__.py
--rw-r--r--   0        0        0     3442 2022-07-09 13:34:11.675572 uidom-0.1.1b6/uidom/dom/tailwindcss/css.py
--rw-r--r--   0        0        0      251 2022-07-09 13:34:39.282656 uidom-0.1.1b6/uidom/dom/tailwindcss/flexbox/__init__.py
--rw-r--r--   0        0        0      732 2022-07-10 00:50:55.437557 uidom-0.1.1b6/uidom/dom/tailwindcss/flexbox/direction.py
--rw-r--r--   0        0        0      769 2022-07-10 00:50:55.437557 uidom-0.1.1b6/uidom/dom/tailwindcss/flexbox/flexes.py
--rw-r--r--   0        0        0      414 2022-07-10 00:50:55.333557 uidom-0.1.1b6/uidom/dom/tailwindcss/flexbox/grow.py
--rw-r--r--   0        0        0      304 2022-07-10 00:50:55.333557 uidom-0.1.1b6/uidom/dom/tailwindcss/flexbox/order.py
--rw-r--r--   0        0        0      422 2022-07-10 00:50:55.333557 uidom-0.1.1b6/uidom/dom/tailwindcss/flexbox/shrink.py
--rw-r--r--   0        0        0      549 2022-07-10 00:50:55.333557 uidom-0.1.1b6/uidom/dom/tailwindcss/flexbox/wrap.py
--rw-r--r--   0        0        0      142 2022-07-09 13:34:33.394847 uidom-0.1.1b6/uidom/dom/tailwindcss/gridbox/__init__.py
--rw-r--r--   0        0        0     2528 2022-07-10 00:50:55.329557 uidom-0.1.1b6/uidom/dom/tailwindcss/gridbox/grids.py
--rw-r--r--   0        0        0      495 2022-07-09 13:34:02.119899 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/__init__.py
--rw-r--r--   0        0        0      660 2022-07-10 00:50:55.329557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/clear.py
--rw-r--r--   0        0        0     1020 2022-07-10 00:50:55.201557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/container.py
--rw-r--r--   0        0        0      439 2022-07-10 00:50:55.201557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/decoration.py
--rw-r--r--   0        0        0     2559 2022-07-10 00:50:55.201557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/display.py
--rw-r--r--   0        0        0      538 2022-07-10 00:50:55.201557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/floats.py
--rw-r--r--   0        0        0      412 2022-07-10 00:50:55.197557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/isolation.py
--rw-r--r--   0        0        0      816 2022-07-10 00:50:55.197557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/objectfit.py
--rw-r--r--   0        0        0     1344 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/objectposition.py
--rw-r--r--   0        0        0     1793 2022-07-10 00:50:55.197557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/overflow.py
--rw-r--r--   0        0        0     1400 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/overscroll.py
--rw-r--r--   0        0        0      758 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/position.py
--rw-r--r--   0        0        0      415 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/sizing.py
--rw-r--r--   0        0        0      938 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/toprightbottomleft.py
--rw-r--r--   0        0        0      407 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/visibility.py
--rw-r--r--   0        0        0      946 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/tailwindcss/layout/zindex.py
--rw-r--r--   0        0        0     3731 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/tailwindcss/placements.py
--rw-r--r--   0        0        0      659 2022-07-10 00:50:55.437557 uidom-0.1.1b6/uidom/dom/tailwindcss/responsive.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:29.182986 uidom-0.1.1b6/uidom/dom/tailwindcss/sizing/__init__.py
--rw-r--r--   0        0        0      240 2022-07-09 13:34:37.114726 uidom-0.1.1b6/uidom/dom/tailwindcss/spacing/__init__.py
--rw-r--r--   0        0        0      240 2022-07-09 13:34:48.770350 uidom-0.1.1b6/uidom/dom/tailwindcss/typography/__init__.py
--rw-r--r--   0        0        0    16159 2022-07-10 00:50:55.565557 uidom-0.1.1b6/uidom/dom/ui.py
--rw-r--r--   0        0        0      146 2022-07-09 13:34:21.415244 uidom-0.1.1b6/uidom/dom/utils/__init__.py
--rwxr-xr-x   0        0        0     5268 2022-07-09 13:34:15.543441 uidom-0.1.1b6/uidom/dom/utils/functional.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:10.483613 uidom-0.1.1b6/uidom/dom/vue.py
--rw-r--r--   0        0        0     1674 2022-07-10 00:50:55.561557 uidom-0.1.1b6/uidom/dom/vueloader.py
--rw-r--r--   0        0        0      287 2022-07-10 00:50:55.565557 uidom-0.1.1b6/uidom/dom/vuetify.py
--rw-r--r--   0        0        0      166 2022-07-09 13:33:54.548162 uidom-0.1.1b6/uidom/dom/widgets/__init__.py
--rw-r--r--   0        0        0     1675 2022-07-10 00:47:18.800900 uidom-0.1.1b6/uidom/dom/widgets/dropdown.py
--rw-r--r--   0        0        0     5281 2022-07-10 00:50:56.525557 uidom-0.1.1b6/uidom/dom/widgets/forms.py
--rw-r--r--   0        0        0    14094 2022-08-11 13:27:49.138492 uidom-0.1.1b6/uidom/dom/xcomponent_js.py
--rw-r--r--   0        0        0     2689 2022-07-10 00:50:31.613549 uidom-0.1.1b6/uidom/dom/xshadowcomponent.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.1.1b6/uidom/edge_db/__init__.py
--rw-r--r--   0        0        0     9225 2022-08-11 14:09:54.677171 uidom-0.1.1b6/uidom/edge_db/ql.py
--rw-r--r--   0        0        0      184 2022-07-12 14:25:09.679603 uidom-0.1.1b6/uidom/response/__init__.py
--rw-r--r--   0        0        0     1161 2022-07-26 03:41:20.821181 uidom-0.1.1b6/uidom/response/starlette_response.py
--rw-r--r--   0        0        0      198 2022-07-09 13:33:40.112673 uidom-0.1.1b6/uidom/settings/__init__.py
--rw-r--r--   0        0        0     7529 2022-07-09 13:34:46.054437 uidom-0.1.1b6/uidom/settings/commands.py
--rw-r--r--   0        0        0     9643 2022-07-10 00:50:55.565557 uidom-0.1.1b6/uidom/settings/document.py
--rw-r--r--   0        0        0      581 2022-07-10 00:50:55.565557 uidom-0.1.1b6/uidom/settings/initialiser.py
--rw-r--r--   0        0        0     4197 2022-07-09 13:33:47.056425 uidom-0.1.1b6/uidom/settings/paths.py
--rw-r--r--   0        0        0      121 2022-07-09 13:34:24.323147 uidom-0.1.1b6/uidom/web_io/__init__.py
--rw-r--r--   0        0        0     2647 2022-07-09 13:34:21.503241 uidom-0.1.1b6/uidom/web_io/base.py
--rw-r--r--   0        0        0     1406 2022-11-20 07:10:12.594268 uidom-0.1.1b6/setup.py
--rw-r--r--   0        0        0      511 2022-11-20 07:10:12.594672 uidom-0.1.1b6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-07-10 01:25:07.454978 uidom-0.2a0/LICENSE
+-rw-r--r--   0        0        0     5686 2023-05-01 05:55:18.794343 uidom-0.2a0/README.md
+-rw-r--r--   0        0        0     1271 2023-05-09 21:00:02.884891 uidom-0.2a0/pyproject.toml
+-rw-r--r--   0        0        0      218 2023-05-09 20:59:28.648696 uidom-0.2a0/uidom/__init__.py
+-rw-r--r--   0        0        0     1067 2023-05-09 19:55:16.645883 uidom-0.2a0/uidom/cli/__init__.py
+-rw-r--r--   0        0        0    12108 2023-05-05 19:23:34.126884 uidom-0.2a0/uidom/cli/_cli.py
+-rw-r--r--   0        0        0     6636 2023-05-09 20:55:47.274480 uidom-0.2a0/uidom/cli/cli.py
+-rw-r--r--   0        0        0      517 2023-05-09 11:52:14.395273 uidom-0.2a0/uidom/dom/__init__.py
+-rw-r--r--   0        0        0     4944 2023-05-09 14:03:20.721191 uidom-0.2a0/uidom/dom/htmldocument.py
+-rw-r--r--   0        0        0     5924 2023-05-09 16:54:51.261005 uidom-0.2a0/uidom/dom/htmlelement.py
+-rw-r--r--   0        0        0    42978 2023-03-25 19:14:55.486184 uidom-0.2a0/uidom/dom/icons.py
+-rw-r--r--   0        0        0     1363 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/dom/jinja.py
+-rwxr-xr-x   0        0        0      304 2022-07-09 13:34:38.382685 uidom-0.2a0/uidom/dom/src/__init__.py
+-rw-r--r--   0        0        0    14370 2023-05-09 20:03:33.062191 uidom-0.2a0/uidom/dom/src/component.py
+-rw-r--r--   0        0        0     2188 2023-04-30 13:08:13.941319 uidom-0.2a0/uidom/dom/src/csstags.py
+-rw-r--r--   0        0        0     3926 2023-04-28 22:16:02.820670 uidom-0.2a0/uidom/dom/src/dom1core.py
+-rw-r--r--   0        0        0    16849 2023-05-09 16:40:11.620271 uidom-0.2a0/uidom/dom/src/dom_tag.py
+-rw-r--r--   0        0        0    31872 2023-05-08 10:55:40.270991 uidom-0.2a0/uidom/dom/src/ext.py
+-rw-r--r--   0        0        0     7837 2023-05-09 12:02:36.374388 uidom-0.2a0/uidom/dom/src/html_string.py
+-rw-r--r--   0        0        0    29966 2023-05-06 16:54:04.821779 uidom-0.2a0/uidom/dom/src/htmltags.py
+-rw-r--r--   0        0        0     5048 2023-04-28 12:53:57.974327 uidom-0.2a0/uidom/dom/src/jinjatags.py
+-rw-r--r--   0        0        0      164 2022-07-10 00:50:55.437557 uidom-0.2a0/uidom/dom/src/main.py
+-rw-r--r--   0        0        0    13731 2022-07-09 23:35:41.025062 uidom-0.2a0/uidom/dom/src/parse_html.py
+-rw-r--r--   0        0        0     2836 2023-05-05 16:26:47.195943 uidom-0.2a0/uidom/dom/src/pythontags.py
+-rw-r--r--   0        0        0     1729 2022-07-10 00:50:55.437557 uidom-0.2a0/uidom/dom/src/sphinxtags.py
+-rw-r--r--   0        0        0     8929 2022-07-10 00:50:55.437557 uidom-0.2a0/uidom/dom/src/svgtags.py
+-rw-r--r--   0        0        0      145 2022-07-09 13:34:17.763367 uidom-0.2a0/uidom/dom/src/utils/__init__.py
+-rw-r--r--   0        0        0     4330 2023-05-09 05:24:01.353063 uidom-0.2a0/uidom/dom/src/utils/dom_util.py
+-rw-r--r--   0        0        0     5091 2022-07-09 13:34:16.191419 uidom-0.2a0/uidom/dom/src/utils/sheets.py
+-rw-r--r--   0        0        0     6623 2023-04-28 14:41:04.189760 uidom-0.2a0/uidom/dom/src/ws_rpc.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:30.126955 uidom-0.2a0/uidom/dom/src/xmltags.py
+-rw-r--r--   0        0        0    16753 2023-04-26 07:43:57.647609 uidom-0.2a0/uidom/dom/ui.py
+-rw-r--r--   0        0        0     3921 2023-03-17 15:40:20.920740 uidom-0.2a0/uidom/dom/uniqueid.py
+-rw-r--r--   0        0        0      121 2022-07-09 13:34:42.034566 uidom-0.2a0/uidom/edge_db/__init__.py
+-rw-r--r--   0        0        0     9912 2023-03-26 09:48:59.256451 uidom-0.2a0/uidom/edge_db/ql.py
+-rw-r--r--   0        0        0      277 2022-07-09 13:33:39.112708 uidom-0.2a0/uidom/elements/__init__.py
+-rw-r--r--   0        0        0     4950 2023-04-27 19:01:56.240091 uidom-0.2a0/uidom/elements/booleans.py
+-rw-r--r--   0        0        0     4067 2023-03-14 11:52:41.667372 uidom-0.2a0/uidom/elements/buttons.py
+-rw-r--r--   0        0        0    12944 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/elements/chars.py
+-rw-r--r--   0        0        0      741 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/elements/dates.py
+-rw-r--r--   0        0        0     1903 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/elements/enums.py
+-rw-r--r--   0        0        0     5512 2023-03-14 11:52:41.187178 uidom-0.2a0/uidom/elements/floats.py
+-rw-r--r--   0        0        0     8833 2023-04-22 19:36:12.299643 uidom-0.2a0/uidom/elements/integers.py
+-rw-r--r--   0        0        0      908 2023-03-14 11:52:41.623355 uidom-0.2a0/uidom/examples/links.py
+-rw-r--r--   0        0        0     2685 2023-04-08 22:55:33.640049 uidom-0.2a0/uidom/examples/toggle.py
+-rw-r--r--   0        0        0      157 2023-03-27 08:33:16.449491 uidom-0.2a0/uidom/reloader/__init__.py
+-rw-r--r--   0        0        0     3945 2023-04-29 11:35:21.410489 uidom-0.2a0/uidom/reloader/_app.py
+-rw-r--r--   0        0        0      158 2023-03-26 20:17:15.474214 uidom-0.2a0/uidom/reloader/_models.py
+-rw-r--r--   0        0        0     1320 2022-11-13 21:32:18.000000 uidom-0.2a0/uidom/reloader/_notify.py
+-rw-r--r--   0        0        0       83 2023-05-02 15:38:28.533313 uidom-0.2a0/uidom/reloader/_types.py
+-rw-r--r--   0        0        0     2031 2023-03-26 05:34:24.365178 uidom-0.2a0/uidom/reloader/_watch.py
+-rw-r--r--   0        0        0     1626 2023-03-26 14:13:50.090675 uidom-0.2a0/uidom/reloader/script/reloader.js
+-rw-r--r--   0        0        0      118 2023-04-08 11:27:56.180219 uidom-0.2a0/uidom/response/__init__.py
+-rw-r--r--   0        0        0     3264 2023-03-17 13:35:31.999152 uidom-0.2a0/uidom/response/starlette.py
+-rw-r--r--   0        0        0      118 2023-04-08 11:28:05.452370 uidom-0.2a0/uidom/routing/__init__.py
+-rw-r--r--   0        0        0     6890 2023-04-08 11:28:44.765011 uidom-0.2a0/uidom/routing/fastapi.py
+-rw-r--r--   0        0        0      768 2023-04-12 16:05:27.697495 uidom-0.2a0/uidom/scripts/__init__.py
+-rw-r--r--   0        0        0     4560 2023-04-22 05:04:01.008470 uidom-0.2a0/uidom/scripts/cdn.py
+-rw-r--r--   0        0        0    11947 2023-04-11 21:23:32.778552 uidom-0.2a0/uidom/scripts/xcomponent.js
+-rw-r--r--   0        0        0      197 2023-05-04 14:36:51.260441 uidom-0.2a0/uidom/settings/__init__.py
+-rw-r--r--   0        0        0     8105 2023-05-05 19:27:38.753086 uidom-0.2a0/uidom/settings/commands.py
+-rw-r--r--   0        0        0     8691 2023-05-05 06:53:34.240389 uidom-0.2a0/uidom/settings/document.py
+-rw-r--r--   0        0        0     4201 2023-05-03 20:51:42.982950 uidom-0.2a0/uidom/settings/paths.py
+-rw-r--r--   0        0        0      219 2023-03-16 11:20:30.258980 uidom-0.2a0/uidom/slots/__init__.py
+-rw-r--r--   0        0        0     1968 2023-05-01 05:14:03.631193 uidom-0.2a0/uidom/slots/custom_element_slot.py
+-rw-r--r--   0        0        0     1594 2023-03-16 11:17:14.416579 uidom-0.2a0/uidom/slots/web_component_slot.py
+-rw-r--r--   0        0        0      118 2023-05-04 22:15:22.715253 uidom-0.2a0/uidom/utils/__init__.py
+-rwxr-xr-x   0        0        0     5295 2023-05-05 08:54:45.688998 uidom-0.2a0/uidom/utils/functional.py
+-rw-r--r--   0        0        0     1320 2023-05-05 05:50:42.208687 uidom-0.2a0/uidom/utils/logger.py
+-rw-r--r--   0        0        0     6458 2023-05-05 15:56:41.572034 uidom-0.2a0/uidom/utils/parameters.py
+-rw-r--r--   0        0        0      337 2023-05-03 18:21:26.051460 uidom-0.2a0/uidom/web_io/__init__.py
+-rw-r--r--   0        0        0    12444 2023-05-03 15:26:45.936106 uidom-0.2a0/uidom/web_io/_adapter.py
+-rw-r--r--   0        0        0     7291 2023-05-03 18:18:45.850893 uidom-0.2a0/uidom/web_io/_events.py
+-rw-r--r--   0        0        0     1467 2023-04-22 19:48:06.786062 uidom-0.2a0/uidom/web_io/_protocol.py
+-rw-r--r--   0        0        0      353 2023-04-22 11:35:31.981365 uidom-0.2a0/uidom/web_io/_types.py
+-rw-r--r--   0        0        0     6849 1970-01-01 00:00:00.000000 uidom-0.2a0/PKG-INFO
```

### Comparing `uidom-0.1.1b6/LICENSE` & `uidom-0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `uidom-0.1.1b6/uidom/components/alpinejs/web_component_slot.py` & `uidom-0.2a0/uidom/slots/web_component_slot.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 import typing
 from dataclasses import dataclass
 
-from uidom.components.alpinejs.slot_element import x_slot
 from uidom.dom.htmlelement import *
 from uidom.dom.src.htmltags import *
+from uidom.slots.custom_element_slot import x_slot
 
 __all__ = [
     "WebComponentSlot"
 ]
 
 
 @dataclass
@@ -27,15 +27,15 @@
         super(WebComponentSlot, self).__post_init__(
             slot_names=self.slot_names,
             classes=self.classes,
             css=self.css,
             slot_class=self.slot_class
         )
 
-    def __render__(
+    def render(
             self,
             tag_name,
             slot_names,
             classes,
             css,
             slot_class
     ):
```

### Comparing `uidom-0.1.1b6/uidom/components/atoms/toggle.py` & `uidom-0.2a0/uidom/examples/toggle.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,67 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
+from dataclasses import dataclass
 
 from uidom.dom import *
 
-__all__ = [
-    "TogglePlain",
-    "ToggleOutset",
-    "ToggleInset"
-]
+__all__ = ["TogglePlain", "ToggleOutset", "ToggleInset"]
 
 
+@dataclass
 class TogglePlain(AlpineComponent):
     # from https://alpineapple.dev/toggle/
-    x_data = {"toggle": "false"}
 
-    def __render__(self, tag_name):
+    def render(self, tag_name):
         # "{{'toggle': 'false'}}" <--- how single-quotes ['false', 'toggle'] etc are used
         # to correctly parse f-string
-        return HTMLStringToDom(f'''
+        return f"""
         <div x-data="{{'toggle': 'false'}}" 
             @click="toggle = !toggle" 
             x_component="{tag_name}"
-            class="relative cursor-pointer h-6 w-12 rounded-full transition-all duration-300 
-                   ease-in-out bg-cyan-400 bg-slate-400" :class=" toggle ? 'bg-cyan-400' : 'bg-slate-400' ">
-            <span class="absolute h-6 w-6 rounded-full bg-white transition-all duration-300 ease-in-out" :class=" toggle ? 'translate-x-7' : '' "></span>
+            class="relative w-12 h-6 transition-all duration-300 ease-in-out rounded-full cursor-pointer bg-slate-400" :class=" toggle ? 'bg-cyan-400' : 'bg-slate-400' ">
+            <span class="absolute w-6 h-6 transition-all duration-300 ease-in-out bg-white rounded-full" :class=" toggle ? 'translate-x-7' : '' "></span>
         </div>
-        ''').parse()
+        """
 
 
+@dataclass
 class ToggleInset(XComponent):
-
-    def __render__(self, tag_name):
-        return HTMLStringToDom(f'''
+    def render(self, tag_name):
+        return f"""
         <template x-component="{tag_name}" >
             <label for="Toggle1" x-data="$el.parentElement.data()" class="inline-flex items-center space-x-4 cursor-pointer dark:text-gray-100">
                 <span>Left</span>
                 <span class="relative">
                     <input id="Toggle1" type="checkbox" class="hidden peer">
                     <div class="w-10 h-6 rounded-full shadow-inner dark:bg-gray-400 peer-checked:dark:bg-violet-400"></div>
                     <div class="absolute inset-y-0 left-0 w-4 h-4 m-1 rounded-full shadow peer-checked:right-0 peer-checked:left-auto dark:bg-gray-800"></div>
                 </span>
                 <span>Right</span>
             </label>
         </template>
-        ''').parse()
+        """
 
 
+@dataclass
 class ToggleOutset(XComponent):
-
-    def __render__(self, tag_name):
-        return HTMLStringToDom(f'''
+    def render(self, tag_name):
+        return f"""
         <template x-component={tag_name}>
             <label for="Toggle1" class="inline-flex items-center space-x-4 cursor-pointer dark:text-gray-100">
                 <span>Left</span>
                 <span class="relative">
                     <input id="Toggle1" type="checkbox" class="hidden peer">
                     <div class="w-10 h-6 rounded-full shadow-inner dark:bg-gray-400 peer-checked:dark:bg-violet-400"></div>
                     <div class="absolute inset-y-0 left-0 w-4 h-4 m-1 rounded-full shadow peer-checked:right-0 peer-checked:left-auto dark:bg-gray-800"></div>
                 </span>
                 <span>Right</span>
             </label>
         </template>
-        ''').parse()
+        """
 
 
-if __name__ == '__main__':
-    print(TogglePlain('xyz'))
+if __name__ == "__main__":
+    print(ToggleOutset("xyz")["x-component"])
```

### Comparing `uidom-0.1.1b6/uidom/dom/elements/booleans.py` & `uidom-0.2a0/uidom/elements/booleans.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,80 +1,77 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 import typing as T
 from dataclasses import dataclass
 
-from uidom.dom.elements.buttons import SubmitButton
-from uidom.dom.htmlelement import HTMLElement
 from valio import StringValidator, Validator
 
+from uidom.dom.htmlelement import HTMLElement
+from uidom.elements.buttons import SubmitButton
+
 __all__ = [
     # boolean html
     "BooleanLabel",
     "BooleanLegend",
     "BooleanInput",
     "CheckboxInput",
     "RadioInput",
-    "BooleanField"
+    "BooleanField",
 ]
 
 
 @dataclass(eq=False)
 class BooleanLabel(HTMLElement):
     label: str = StringValidator(logger=False, debug=True)
 
     def __post_init__(self, *args, **kwargs):
         super(BooleanLabel, self).__init__(self.label, *args, **kwargs)
 
-    def __render__(self, label: str, *args, **kwargs):  # noqa
+    def render(self, label: str, *args, **kwargs):  # noqa
         return self.html_tags.label(label, *args, **kwargs)
 
 
 class BooleanLabelValidator(Validator):
     annotation = T.Union[BooleanLabel, None]
 
 
 @dataclass(eq=False)
 class BooleanLegend(HTMLElement):
     label: str = StringValidator(logger=False, debug=True)
 
     def __post_init__(self, *args, **kwargs):
         super(BooleanLegend, self).__init__(self.label, *args, **kwargs)
 
-    def __render__(self, label: str, *args, **kwargs):
+    def render(self, label: str, *args, **kwargs):
         return self.html_tags.legend(label, *args, **kwargs)
 
 
 @dataclass(eq=False)
 class BooleanInput(HTMLElement):
     name: str = StringValidator(logger=False, debug=True)
-    type: str = StringValidator(in_choice=["checkbox", "radio"], logger=False, debug=True, default="checkbox")
-    checked: T.Union[str, bool] = Validator(in_choice=["unchecked", "checked", "null", True, False],
-                                                 logger=False, debug=True, default="checked")
+    type: str = StringValidator(
+        in_choice=["checkbox", "radio"], logger=False, debug=True, default="checkbox"
+    )
+    checked: T.Union[str, bool] = Validator(
+        in_choice=["unchecked", "checked", "null", True, False],
+        logger=False,
+        debug=True,
+        default="checked",
+    )
 
     def __post_init__(self, *args, **kwargs):
-        super(BooleanInput, self).__init__(*args,
-                                           name=self.name,
-                                           type=self.type,
-                                           checked=self.checked,
-                                           **kwargs)
-
-    def __render__(
-            self,
-            *args,
-            name,
-            type,
-            checked,
-            **kwargs
-    ):
+        super(BooleanInput, self).__init__(
+            *args, name=self.name, type=self.type, checked=self.checked, **kwargs
+        )
 
+    def render(self, *args, name, type, checked, **kwargs):
         return self.html_tags.input_(
             *args,
             name=name,
             type=type,
             checked=checked if checked != "null" else False,
             **kwargs,
         )
@@ -83,60 +80,52 @@
 class BooleanInputValidator(Validator):
     annotation = T.Union[BooleanInput, None]
 
 
 @dataclass(eq=False)
 class CheckboxInput(BooleanInput):
     name: str = StringValidator(logger=False, debug=True)
-    checked: T.Union[str, bool] = Validator(in_choice=["unchecked", "checked", "null", True, False],
-                                            logger=False, debug=True)
+    checked: T.Union[str, bool] = Validator(
+        in_choice=["unchecked", "checked", "null", True, False],
+        logger=False,
+        debug=True,
+    )
 
     def __post_init__(self, *args, **kwargs):
-        super(BooleanInput, self).__init__(*args,
-                                           name=self.name,
-                                           checked=self.checked,
-                                           **kwargs)
-
-    def __render__(
-            self,
-            *args,
-            name,
-            checked,
-            **kwargs
-    ):
+        super(BooleanInput, self).__init__(
+            *args, name=self.name, checked=self.checked, **kwargs
+        )
 
-        return super().__render__(
+    def render(self, *args, name, checked, **kwargs):
+        return super().render(
             *args,
             name=name,
             type="checkbox",
             checked=checked,
             **kwargs,
         )
 
 
 @dataclass(eq=False)
 class RadioInput(BooleanInput):
     name: str = StringValidator(logger=False, debug=True)
-    checked: T.Union[str, bool] = Validator(in_choice=["unchecked", "checked", "null", True, False],
-                                            logger=False, debug=True, default="checked")
+    checked: T.Union[str, bool] = Validator(
+        in_choice=["unchecked", "checked", "null", True, False],
+        logger=False,
+        debug=True,
+        default="checked",
+    )
 
     def __post_init__(self, *args, **kwargs):
-        super(BooleanInput, self).__init__(*args,
-                                           name=self.name,
-                                           checked=self.checked,
-                                           **kwargs)
+        super(BooleanInput, self).__init__(
+            *args, name=self.name, checked=self.checked, **kwargs
+        )
 
-    def __render__(
-            self,
-            *args,
-            name,
-            checked,
-            **kwargs
-    ):
-        return super().__render__(
+    def render(self, *args, name, checked, **kwargs):
+        return super().render(
             *args,
             name=name,
             type="radio",
             checked=checked,
             **kwargs,
         )
 
@@ -147,38 +136,45 @@
     input = BooleanInputValidator(logger=False, debug=True)
     label: str
     name: str
     type: str
     checked: T.Union[str, bool]
 
     def __post_init__(self, *args, **kwargs):
-        super(BooleanField, self).__init__(*args,
-                                           label=self.label,
-                                           name=self.name,
-                                           type=self.type,
-                                           checked=self.checked,
-                                           **kwargs
-                                           )
+        super(BooleanField, self).__init__(
+            *args,
+            label=self.label,
+            name=self.name,
+            type=self.type,
+            checked=self.checked,
+            **kwargs,
+        )
 
-    def __render__(self, *args, label, name, type, checked, **kwargs):
+    @property
+    def input_id(self):
+        return self.input["id"]
+
+    @input_id.setter
+    def input_id(self, id):
+        self.labeled["for"] = self.input["id"] = id
+
+    def render(self, *args, label, name, type, checked, **kwargs):
         self.labeled = BooleanLabel(label)
         self.input = BooleanInput(
-                  name=name,
-                  type=type,
-                  checked=checked,
-              )
+            name=name,
+            type=type,
+            checked=checked,
+        )
         return self.html_tags.div(*args, self.labeled, self.input, **kwargs)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from uidom.dom import form
+
     field = BooleanField(
-        label="Terms and Conditions",
-        checked="null",
-        name="select",
-        type="radio")
+        label="Terms and Conditions", checked="null", name="select", type="radio"
+    )
     button = SubmitButton(label="Agree", value="agree")
-    field.labeled["for"] = field.input["id"] = "select"
+    field.input_id = "select"
     button["for"] = field["id"] = "xyz"
     print(form(field, button, method="POST"))
     print(RadioInput(checked="unchecked", name="deliver"))
-
```

### Comparing `uidom-0.1.1b6/uidom/dom/elements/buttons.py` & `uidom-0.2a0/uidom/elements/buttons.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 import typing as T
 from dataclasses import dataclass
 
+from valio import StringValidator, Validator
+
 from uidom.dom.htmlelement import HTMLElement
 from uidom.dom.src.htmltags import html_tag
-from valio import StringValidator, Validator
 
 __all__ = [
     "Button",
     "SubmitButton",
     "ResetButton",
     "ButtonInput",
     "SubmitButtonInput",
@@ -36,100 +37,100 @@
             *args,
             label=self.label,
             type=self.type,
             value=self.value,
             icon=self.icon if self.icon is not None else False,
             **kwargs)
 
-    def __render__(self, *args, label, type, value, icon=None, **kwargs):
+    def render(self, *args, label, type, value, icon=None, **kwargs):
         return self.html_tags.button(icon or '', label, *args, type=type, value=value, **kwargs)
 
 
 @dataclass(eq=False)
 class _ButtonInput(HTMLElement):
     type: str = StringValidator(in_choice=["submit", "reset", "button", "file", "image"], logger=False, debug=True)
     value: str = StringValidator(logger=False, debug=True)
 
     def __post_init__(self, *args, **kwargs):
         super(_ButtonInput, self).__init__(*args, type=self.type, value=self.value, **kwargs)
 
-    def __render__(self, *args, type, value, **kwargs):
+    def render(self, *args, type, value, **kwargs):
         return self.html_tags.input_(*args, type=type, value=value, **kwargs)
 
 
 @dataclass(eq=False)
 class Button(HTMLElement):
     label: str
     value: str
 
     def __post_init__(self, *args, **kwargs):
         super(Button, self).__init__(*args, label=self.label, value=self.value, **kwargs)
 
-    def __render__(self, *args, label, value, **kwargs):
+    def render(self, *args, label, value, **kwargs):
         return _Button(label=label, type="button", value=value)
 
 
 @dataclass(eq=False)
 class SubmitButton(HTMLElement):
     label: str
     value: str
     icon: T.Union[html_tag, None] = None
 
     def __post_init__(self, *args, **kwargs):
         super(SubmitButton, self).__init__(*args, label=self.label, value=self.value, icon=self.icon, **kwargs)
 
-    def __render__(self, *args, value, label, icon, **kwargs):
+    def render(self, *args, value, label, icon, **kwargs):
         return _Button(type="submit", value=value, label=label, icon=icon)
 
 
 @dataclass(eq=False)
 class ResetButton(HTMLElement):
     label: str
     value: str
     icon: T.Union[html_tag, None] = None
 
     def __post_init__(self, *args, **kwargs):
         super(ResetButton, self).__init__(*args, label=self.label, value=self.value, icon=self.icon, **kwargs)
 
-    def __render__(self, *args, label, value, icon, **kwargs):
+    def render(self, *args, label, value, icon, **kwargs):
         return _Button(*args, type="reset", label=label, value=value, icon=icon, **kwargs)
 
 @dataclass(eq=False)
 class ButtonInput(HTMLElement):
     value: str
     
-    def __render__(self, *args, value, **kwargs):
+    def render(self, *args, value, **kwargs):
         return _ButtonInput(type="button", value=value)
 
 @dataclass(eq=False)
 class SubmitButtonInput(HTMLElement):
     value: str 
     
-    def __render__(self, *args, value, **kwargs):
+    def render(self, *args, value, **kwargs):
         return _ButtonInput(type="submit", value=value)
 
 @dataclass(eq=False)
 class ResetButtonInput(HTMLElement):
     value: str
     
-    def __render__(self, *args, value, **kwargs):
+    def render(self, *args, value, **kwargs):
         return _ButtonInput(type="reset", value=value)
 
 @dataclass(eq=False)
 class FileButtonInput(HTMLElement):
     value: str 
     
-    def __render__(self, *args, value, **kwargs):
+    def render(self, *args, value, **kwargs):
         return _ButtonInput(type="file", value=value)
 
 @dataclass(eq=False)
 class ImageButtonInput(HTMLElement):
     value: str 
     
-    def __render__(self, *args, value, **kwargs):
+    def render(self, *args, value, **kwargs):
         return _ButtonInput(type="image", value=value)
 
 
 if __name__ == '__main__':
     print(SubmitButton(label="submit", value="upload"))
     print(ResetButton(label="reset", value="reset"))
     # print(FileButtonInput(value="a"))
```

### Comparing `uidom-0.1.1b6/uidom/dom/elements/chars.py` & `uidom-0.2a0/uidom/elements/chars.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 import typing as T
 from dataclasses import dataclass, field
 
-from uidom.dom.htmlelement import HTMLElement
 from valio import StringValidator, Validator
 
+from uidom.dom.htmlelement import HTMLElement
+
 __all__ = [
     # char html
     "CharLabel",
     "CharLegend",
     "CharInput",
     "TextInput",
     "PasswordInput",
@@ -27,30 +28,30 @@
 @dataclass(eq=False)
 class CharLabel(HTMLElement):
     label: str = StringValidator(logger=False, debug=True)
 
     def __post_init__(self, *args, **kwargs):
         super(CharLabel, self).__init__(label=self.label, *args, **kwargs)
 
-    def __render__(self, label: str, *args, **kwargs):  # noqa
+    def render(self, label: str, *args, **kwargs):  # noqa
         return self.html_tags.label(label, *args, **kwargs)
 
 
 class CharLabelValidator(Validator):
     annotation = T.Union[CharLabel, None]
 
 
 @dataclass(eq=False)
 class CharLegend(HTMLElement):
     label: str = StringValidator(logger=False, debug=True)
 
     def __post_init__(self, *args, **kwargs):
         super(CharLegend, self).__init__(label=self.label, *args, **kwargs)
 
-    def __render__(self, label, *args, **kwargs):
+    def render(self, label, *args, **kwargs):
         return self.html_tags.legend(label, *args, **kwargs)
 
 
 min_length_field = StringValidator(logger=False, debug=True, name="min_length")
 max_length_field = StringValidator(logger=False, debug=True, name="max_length")
 spell_check_field = StringValidator(in_choice=["true", "false"], 
                                     logger=False, debug=True, name="spell_check", 
@@ -94,15 +95,15 @@
                                         spell_check=self.spell_check,
                                         type=self.type,
                                         min_length=self.min_length,
                                         max_length=self.max_length,
                                         pattern=self.pattern,
                                         **kwargs)
 
-    def __render__(
+    def render(
             self,
             *args,
             name: str = None,
             placeholder: str = "",
             spell_check: str,
             type: str,
             min_length: str,
@@ -144,15 +145,15 @@
                                         placeholder=self.placeholder,
                                         spell_check=self.spell_check,
                                         min_length=self.min_length,
                                         max_length=self.max_length,
                                         pattern=self.pattern,
                                         **kwargs)
 
-    def __render__(
+    def render(
             self,
             *args,
             name: str = None,
             placeholder: str = "",
             spell_check: str = "true",
             min_length: str,
             max_length: str = "null",
@@ -185,15 +186,15 @@
                                             placeholder=self.placeholder,
                                             spell_check=self.spell_check,
                                             min_length=self.min_length,
                                             max_length=self.max_length,
                                             pattern=self.pattern,
                                             **kwargs)
 
-    def __render__(
+    def render(
             self,
             *args,
             name,
             placeholder,
             spell_check,
             min_length,
             max_length,
@@ -228,15 +229,15 @@
                                           placeholder=self.placeholder,
                                           spell_check=self.spell_check,
                                           min_length=self.min_length,
                                           max_length=self.max_length,
                                           pattern=self.pattern,
                                           **kwargs)
 
-    def __render__(
+    def render(
             self,
             *args,
             name: str = None,
             placeholder: str = "",
             spell_check: str = "true",
             min_length: str = "null",
             max_length: str = "null",
@@ -271,15 +272,15 @@
                                          placeholder=self.placeholder,
                                          spell_check=self.spell_check,
                                          min_length=self.min_length,
                                          max_length=self.max_length,
                                          pattern=self.pattern,
                                          **kwargs)
 
-    def __render__(
+    def render(
             self,
             *args,
             name: str = None,
             placeholder: str = "",
             spell_check: str = "true",
             min_length: str = "null",
             max_length: str = "null",
@@ -314,15 +315,15 @@
                                           placeholder=self.placeholder,
                                           spell_check=self.spell_check,
                                           min_length=self.min_length,
                                           max_length=self.max_length,
                                           pattern=self.pattern,
                                           **kwargs)
 
-    def __render__(
+    def render(
             self,
             *args,
             name: str = None,
             placeholder: str = "",
             spell_check: str = "true",
             min_length: str = "null",
             max_length: str = "null",
@@ -357,27 +358,27 @@
                                         label=self.label,
                                         name=self.name,
                                         placeholder=self.placeholder,
                                         type=self.type,
                                         **kwargs
                                         )
 
-    def __render__(self, *args, label, name, placeholder, type, **kwargs):
+    def render(self, *args, label, name, placeholder, type, **kwargs):
         self.labeled = CharLabel(label)
         self.input = CharInput(
                   name=name,
                   placeholder=placeholder,
                   type=type
               )
         return self.html_tags.div(*args, self.labeled, self.input, **kwargs)
 
 
 class CharFieldSet(HTMLElement):
 
-    def __render__(self, legend: CharLegend, *fields: HTMLElement, **kwargs):
+    def render(self, legend: CharLegend, *fields: HTMLElement, **kwargs):
         return self.html_tags.fieldset(legend, *fields, **kwargs)
 
 
 if __name__ == '__main__':
     print(CharField(label="Cut", name="cut", placeholder="Diamond Cut", type="text"))
     print(HiddenInput(name="password", placeholder="Enter Password", min_length="4"))
     print(CharInput(name="text", placeholder="Enter Password", min_length="13", spell_check="false"))
```

### Comparing `uidom-0.1.1b6/uidom/dom/elements/dates.py` & `uidom-0.2a0/uidom/elements/dates.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,21 +14,21 @@
 
 @dataclass(eq=False)
 class DateLabel(HTMLElement):
     
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
     
-    def __render__(self, *args, **kwargs):
+    def render(self, *args, **kwargs):
         return self.html_tags.label(*args, **kwargs)    
 
 
 @dataclass(eq=False)
 class DateInput(HTMLElement):
     
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def __render__(self, *args, **kwargs):
+    def render(self, *args, **kwargs):
         return self.html_tags.input_(*args, type="date", **kwargs)
```

### Comparing `uidom-0.1.1b6/uidom/dom/elements/enums.py` & `uidom-0.2a0/uidom/elements/enums.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,57 +3,58 @@
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 import typing as T
 from enum import Enum, IntEnum
 
-from uidom.dom.htmlelement import HTMLElement
-from uidom.dom.src.htmltags import option, select
 from valio import (EnumValidator, IntegerEnumValidator, StringEnumValidator,
                    StringValidator)
 
+from uidom.dom.htmlelement import HTMLElement
+from uidom.dom.src.htmltags import option, select
+
 __all__ = [
     "EnumLabel",
     "EnumInput",
     "IntegerEnumInput",
     "CharEnumInput"
 ]
 
 
 class EnumLabel(HTMLElement):
     label = StringValidator(logger=False, debug=True)
 
-    def __render__(self, label, *args, **kwargs):
+    def render(self, label, *args, **kwargs):
         self.label = label
         return self.html_tags.label(self.label, *args, **kwargs)
 
 
 class EnumInput(HTMLElement):
     options: Enum = EnumValidator(logger=False, debug=True)
 
-    def __render__(self, *args, options, **kwargs):
+    def render(self, *args, options, **kwargs):
         self.options = options
         return select(option(opt.value, value=str(opt.value).capitalize())
                       if len(opt.value) == 1 else option(opt.value[0], value=str(opt.value[1]))
                       for opt in options)
 
 
 class IntegerEnumInput(HTMLElement):
     options: IntEnum = IntegerEnumValidator(logger=False, debug=True)
 
-    def __render__(self, *args, options, **kwargs):
+    def render(self, *args, options, **kwargs):
         self.options = options
         return select(option(opt.value, value=str(opt.value).capitalize())
                       if len(opt.value) == 1 else option(opt.value[0], value=str(opt.value[1]))
                       for opt in options)
 
 
 class CharEnumInput(HTMLElement):
     options: T.Union[str, Enum, None] = StringEnumValidator(logger=False, debug=True)
 
-    def __render__(self, *args, options, **kwargs):
+    def render(self, *args, options, **kwargs):
         self.options = options
         return select(option(opt.value, value=str(opt.value).capitalize())
                       if len(opt.value) == 1 else option(opt.value[0], value=str(opt.value[1]))
                       for opt in options)
```

### Comparing `uidom-0.1.1b6/uidom/dom/elements/floats.py` & `uidom-0.2a0/uidom/elements/floats.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,17 +3,18 @@
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 import typing as T
 from dataclasses import dataclass, field
 
-from uidom.dom.htmlelement import HTMLElement
 from valio import StringValidator
 
+from uidom.dom.htmlelement import HTMLElement
+
 __all__ = [
     # integer html
     "FloatLabel",
     "FloatLegend",
     "FloatInput",
     "FloatNumberInput",
     "FloatRangeInput",
@@ -23,26 +24,26 @@
 @dataclass(eq=False)
 class FloatLabel(HTMLElement):
     label: str = StringValidator(logger=False, debug=True)
 
     def __post_init__(self, *args, **kwargs):
         super(FloatLabel, self).__init__(self.label, *args, **kwargs)
 
-    def __render__(self, label, *args, **kwargs):
+    def render(self, label, *args, **kwargs):
         return self.html_tags.label(label, *args, **kwargs)
 
 
 @dataclass(eq=False)
 class FloatLegend(HTMLElement):
     label: str = StringValidator(logger=False, debug=True)
 
     def __post_init__(self, *args, **kwargs):
         super(FloatLegend, self)._init__(self.label, *args, **kwargs)
 
-    def __render__(self, label, *args, **kwargs):
+    def render(self, label, *args, **kwargs):
         return self.html_tags.legend(label, *args, **kwargs)
 
 
 min_field = StringValidator(logger=False, debug=True)
 max_field = StringValidator(logger=False, debug=True)
 
 
@@ -73,15 +74,15 @@
                                          type=self.type,
                                          min=self.min,
                                          max=self.max,
                                          pattern=self.pattern,
                                          **kwargs
                                          )
 
-    def __render__(
+    def render(
             self,
             *args,
             name,
             placeholder="",
             type,
             min,
             max,
@@ -115,15 +116,15 @@
                                                placeholder=self.placeholder,
                                                min=self.min,
                                                max=self.max,
                                                pattern=self.pattern,
                                                **kwargs
                                                )
 
-    def __render__(
+    def render(
             self,
             *args,
             name,
             placeholder="",
             min,
             max,
             pattern,
@@ -153,15 +154,15 @@
                                               placeholder=self.placeholder,
                                               min=self.min,
                                               max=self.max,
                                               pattern=self.pattern,
                                               **kwargs
                                               )
 
-    def __render__(
+    def render(
             self,
             *args,
             name,
             placeholder="",
             min,
             max,
             pattern,
```

### Comparing `uidom-0.1.1b6/uidom/dom/elements/integers.py` & `uidom-0.2a0/uidom/elements/integers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,103 +1,96 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 import typing as T
 from dataclasses import dataclass, field
 
-from uidom.dom.htmlelement import HTMLElement
 from valio import StringValidator, Validator
 
+from uidom.dom.htmlelement import HTMLElement
+
 __all__ = [
     # integer html
     "IntegerLabel",
     "IntegerLegend",
     "IntegerInput",
     "IntegerNumberInput",
     "IntegerRangeInput",
     "TelephoneInput",
     "IntegerField",
 ]
 
+
 @Validator.register
 @dataclass(eq=False)
 class IntegerLabel(HTMLElement):
     label: str = StringValidator(logger=False, debug=True)
 
     def __post_init__(self, *args, **kwargs):
         super(IntegerLabel, self).__init__(*args, label=self.label, **kwargs)
 
-    def __render__(self, label, *args, **kwargs):
+    def render(self, label, *args, **kwargs):
         return self.html_tags.label(label, *args, **kwargs)
 
 
-
 class IntegerLabelValidator(Validator):
     annotation = T.Union[IntegerLabel, None]
 
 
 @dataclass(eq=False)
 class IntegerLegend(HTMLElement):
     label: str = StringValidator(logger=False, debug=True)
 
     def __post_init__(self, *args, **kwargs):
         super(IntegerLegend, self).__init__(label=self.label, *args, *kwargs)
 
-    def __render__(self, label, *args, **kwargs):
+    def render(self, label, *args, **kwargs):
         return self.html_tags.legend(label, *args, **kwargs)
 
+
 min_field = StringValidator(logger=False, debug=True, name="min")
 max_field = StringValidator(logger=False, debug=True, name="max")
 
+
 @dataclass(eq=False)
 class IntegerInput(HTMLElement):
-
     @max_field.add_validator
     @min_field.add_validator
     def cast2int(self, value):
         if value not in ["null", None]:
             try:
                 int(value)
             except TypeError as e:
                 raise ValueError(f"{value} is not an integer value") from e
 
     name: str = StringValidator(logger=False, debug=True)
     placeholder: str = StringValidator(logger=False, debug=True)
-    type: str = StringValidator(in_choice=["number", "range", "tel"],
-                                logger=False, debug=True, default="number")
+    type: str = StringValidator(
+        in_choice=["number", "range", "tel"], logger=False, debug=True, default="number"
+    )
     min: str = min_field
     max: str = max_field
     pattern: str = StringValidator(logger=False, debug=True, default=None)
 
     def __post_init__(self, *args, **kwargs):
-        super(IntegerInput, self).__init__(*args,
-                                           name=self.name,
-                                           placeholder=self.placeholder,
-                                           type=self.type,
-                                           min=self.min,
-                                           max=self.max,
-                                           pattern=self.pattern,
-                                           **kwargs
-                                           )
-
-    def __render__(
-            self,
+        super(IntegerInput, self).__init__(
             *args,
-            name,
-            placeholder="",
-            type,
-            min,
-            max,
-            pattern,
-            **kwargs
-    ):
+            name=self.name,
+            placeholder=self.placeholder,
+            type=self.type,
+            min=self.min,
+            max=self.max,
+            pattern=self.pattern,
+            **kwargs,
+        )
 
+    def render(self, *args, name, placeholder="", type, min, max, pattern, **kwargs):
         return self.html_tags.input_(
             *args,
             name=name,
             placeholder=placeholder,
             type=type,
             min=min if min not in ["null", None] else False,
             max=max if max not in ["null", None] else False,
@@ -111,41 +104,32 @@
 
 class IntegerInputValidator(Validator):
     annotation = T.Union[IntegerInput, None]
 
 
 @dataclass(eq=False)
 class IntegerNumberInput(HTMLElement):
-
     name: str
     placeholder: str
     min: T.Union[str, None] = field(default=None)
     max: T.Union[str, None] = field(default=None)
     pattern: T.Union[str, None] = field(default=None)
 
     def __post_init__(self, *args, **kwargs):
-        super(IntegerNumberInput, self).__init__(*args,
-                                                 name=self.name,
-                                                 placeholder=self.placeholder,
-                                                 min=self.min,
-                                                 max=self.max,
-                                                 pattern=self.pattern,
-                                                 **kwargs
-                                                 )
-
-    def __render__(
-            self,
+        super(IntegerNumberInput, self).__init__(
             *args,
-            name,
-            placeholder="",
-            min,
-            max,
-            pattern="null",
-            **kwargs
-    ):
+            name=self.name,
+            placeholder=self.placeholder,
+            min=self.min,
+            max=self.max,
+            pattern=self.pattern,
+            **kwargs,
+        )
+
+    def render(self, *args, name, placeholder="", min, max, pattern="null", **kwargs):
         return IntegerInput(
             name=name,
             placeholder=placeholder,
             type="number",
             min=min,
             max=max,
             pattern=pattern,
@@ -157,87 +141,78 @@
 
 class IntegerNumberInputValidator(Validator):
     annotation = T.Union[IntegerNumberInput, None]
 
 
 @dataclass(eq=False)
 class IntegerRangeInput(HTMLElement):
-
     name: str
     placeholder: str
     min: T.Union[str, None] = field(default=None)
     max: T.Union[str, None] = field(default=None)
     pattern: T.Union[str, None] = field(default=None)
 
     def __post_init__(self, *args, **kwargs):
-        super(IntegerRangeInput, self).__init__(*args,
-                                                name=self.name,
-                                                placeholder=self.placeholder,
-                                                min=self.min,
-                                                max=self.max,
-                                                pattern=self.pattern,
-                                                **kwargs
-                                                )
-
-    def __render__(
-            self,
+        super(IntegerRangeInput, self).__init__(
             *args,
-            name,
-            placeholder="",
-            min="null",
-            max="null",
-            pattern="null",
-            **kwargs
+            name=self.name,
+            placeholder=self.placeholder,
+            min=self.min,
+            max=self.max,
+            pattern=self.pattern,
+            **kwargs,
+        )
+
+    def render(
+        self,
+        *args,
+        name,
+        placeholder="",
+        min="null",
+        max="null",
+        pattern="null",
+        **kwargs,
     ):
         return IntegerInput(
             type="range",
             name=name,
             placeholder=placeholder,
             min=min,
             max=max,
-            pattern=pattern
+            pattern=pattern,
         )
 
 
 Validator.register(IntegerRangeInput)  # noqa
 
 
 class IntegerRangeInputValidator(Validator):
     annotation = T.Union[IntegerRangeInput, None]
 
 
 @dataclass(eq=False)
 class TelephoneInput(HTMLElement):
-
     name: str
     placeholder: str
     min: T.Union[str, None] = field(default=None)
     max: T.Union[str, None] = field(default=None)
     pattern: T.Union[str, None] = field(default=None)
 
     def __post_init__(self, *args, **kwargs):
-        super(TelephoneInput, self).__init__(*args,
-                                             name=self.name,
-                                             placeholder=self.placeholder,
-                                             min=self.min,
-                                             max=self.max,
-                                             pattern=self.pattern,
-                                             **kwargs
-                                             )
-
-    def __render__(
-            self,
+        super(TelephoneInput, self).__init__(
             *args,
-            name,
-            placeholder="",
-            min,
-            max,
-            pattern,
-            **kwargs
-    ):
+            name=self.name,
+            placeholder=self.placeholder,
+            min=self.min,
+            max=self.max,
+            pattern=self.pattern,
+            **kwargs,
+        )
+
+    def render(self, *args, name, placeholder="", min, max, pattern, **kwargs):
         return IntegerInput(
             type="tel",
             name=name,
             placeholder=placeholder,
             min=min,
             max=max,
             pattern=pattern,
@@ -251,23 +226,24 @@
 
     label: str
     name: str
     placeholder: str
     type: str
 
     def __post_init__(self, *args, **kwargs):
-        super(IntegerField, self).__init__(*args,
-                                           label=self.label,
-                                           name=self.name,
-                                           placeholder=self.placeholder,
-                                           type=self.type,
-                                           **kwargs
-                                           )
+        super(IntegerField, self).__init__(
+            *args,
+            label=self.label,
+            name=self.name,
+            placeholder=self.placeholder,
+            type=self.type,
+            **kwargs,
+        )
 
-    def __render__(self, *args, label, name, placeholder, type, **kwargs):
+    def render(self, *args, label, name, placeholder, type, **kwargs):
         self.labeled = IntegerLabel(label=label)
         self.input = IntegerInput(name=name, placeholder=placeholder, type=type)
         return self.html_tags.div(*args, self.labeled, self.input, **kwargs)
 
 
 @dataclass(eq=False)
 class IntegerNumberField(HTMLElement):
@@ -275,22 +251,23 @@
     input = IntegerNumberInputValidator(logger=False, debug=True)
 
     label: str
     name: str
     placeholder: str
 
     def __post_init__(self, *args, **kwargs):
-        super(IntegerNumberField, self).__init__(*args,
-                                                 label=self.label,
-                                                 name=self.name,
-                                                 placeholder=self.placeholder,
-                                                 **kwargs
-                                                 )
+        super(IntegerNumberField, self).__init__(
+            *args,
+            label=self.label,
+            name=self.name,
+            placeholder=self.placeholder,
+            **kwargs,
+        )
 
-    def __render__(self, *args, label, name, placeholder, **kwargs):
+    def render(self, *args, label, name, placeholder, **kwargs):
         self.labeled = IntegerLabel(label=label)
         self.input = IntegerNumberInput(name=name, placeholder=placeholder)
         return self.html_tags.div(*args, self.labeled, self.input, **kwargs)
 
 
 @dataclass(eq=False)
 class IntegerRangeField(HTMLElement):
@@ -298,30 +275,35 @@
     input = IntegerRangeInputValidator(logger=False, debug=True)
 
     label: str
     name: str
     placeholder: str
 
     def __post_init__(self, *args, **kwargs):
-        super(IntegerRangeField, self).__init__(*args,
-                                                label=self.label,
-                                                name=self.name,
-                                                placeholder=self.placeholder,
-                                                **kwargs
-                                                )
+        super(IntegerRangeField, self).__init__(
+            *args,
+            label=self.label,
+            name=self.name,
+            placeholder=self.placeholder,
+            **kwargs,
+        )
 
-    def __render__(self, *args, label, name, placeholder, **kwargs):
+    def render(self, *args, label, name, placeholder, **kwargs):
         self.labeled = IntegerLabel(label=label)
         self.input = IntegerRangeInput(name=name, placeholder=placeholder)
         return self.html_tags.div(*args, self.labeled, self.input, **kwargs)
 
 
-if __name__ == '__main__':
-    from uidom.dom import SubmitButton, form
-    quantity = IntegerNumberField(label="Quantity", name="quantity", placeholder="quantity")
+if __name__ == "__main__":
+    from uidom.dom import form
+    from uidom.elements import SubmitButton
+
+    quantity = IntegerNumberField(
+        label="Quantity", name="quantity", placeholder="quantity"
+    )
     quantity.input["id"] = quantity.labeled["for"] = "quantity-id"
     price = IntegerNumberField(label="Price", name="price", placeholder="price")
     price.input["id"] = price.labeled["for"] = "price-id"
     button = SubmitButton("Submit", value="submit")
     forms = form(IntegerLegend("Product"), price, quantity, button)
     print(forms)
     print(IntegerNumberInput(name="price", placeholder="Price", min="2"))
```

### Comparing `uidom-0.1.1b6/uidom/dom/html_to_dom.py` & `uidom-0.2a0/uidom/dom/src/html_string.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,151 +1,176 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 import builtins
 import os
 import sys
 import types
 import typing as T
 from copy import deepcopy
 from dataclasses import dataclass, field
 
-from uidom.dom.htmlelement import HTMLElement
 from uidom.dom.src import ext, htmltags, jinjatags, svgtags
-from uidom.dom.src.htmltags import ConcatTag, html_tag
+from uidom.dom.src.htmltags import html_tag
 from uidom.dom.src.parse_html import Element, tokenize_html
 from uidom.dom.src.utils import dom_text
 
-__all__ = [
-    "HTMLStringToDom",
-    "HTMLStringToElement"
-]
+__all__ = ["HTMLStringToDom", "string_to_element"]
 
 
 def create_dynamic_element(tag_name: str) -> T.Type[ext.Tags]:
     class _Element(ext.Tags):
         tagname = tag_name
 
-    cls_name = ''.join(map(lambda x: x.capitalize(), tag_name.split("-")))
+    cls_name = "".join(map(lambda x: x.capitalize(), tag_name.split("-")))
     _Element.__qualname__ = cls_name
     _Element.__name__ = cls_name
-    module_name: str = os.path.splitext(os.path.basename(sys.modules["__main__"].__file__))[0] # type: ignore
+    module_name: str = os.path.splitext(os.path.basename(sys.modules["__main__"].__file__))[0]  # type: ignore
     _Element.__module__ = module_name
-    element: T.Type[ext.Tags]  = deepcopy(_Element)
+    element: T.Type[ext.Tags] = deepcopy(_Element)
     del _Element
     setattr(sys.modules["__main__"], cls_name, element)
     return element
 
 
 @dataclass
 class HTMLStringToDom(object):
+    # TODO convert DOM object instance to Code Object for AST conversion to python code.
+    # from https://stackoverflow.com/questions/68577587/how-to-find-the-ast-assignment-node-related-to-the-instance-creation
+    # this.ast_object can be easily used to create python code for any html object
+    # https://stackoverflow.com/a/68584740 for parsing a python object into an ast_object
+    # https://stackoverflow.com/a/63212256 for unparsing a python ast_object
+
     html_string_or_token: T.Union[str, Element, list[Element], ext.Tags]
     modules: list[types.ModuleType] = field(default_factory=list)
+    escape: bool = field(default=True)
 
     def __post_init__(self):
-        self.tokens: T.Union[Element, list[Element], ext.Tags] = tokenize_html(
-            self.html_string_or_token if not isinstance(self.html_string_or_token, html_tag)
-            else str(self.html_string_or_token)
-        ).children if isinstance(self.html_string_or_token, (str, html_tag)) else self.html_string_or_token
-        
-        # for htmlt, svg and jinja tags lookup 
+        self.tokens: T.Union[Element, list[Element], ext.Tags] = (
+            tokenize_html(
+                self.html_string_or_token
+                if not isinstance(self.html_string_or_token, html_tag)
+                else str(self.html_string_or_token)
+            ).children
+            if isinstance(self.html_string_or_token, (str, html_tag))
+            else self.html_string_or_token
+        )
+
+        # for html, svg and jinja tags lookup
         if htmltags not in self.modules:
             self.modules.append(htmltags)
-            
+
         if svgtags not in self.modules:
             self.modules.append(svgtags)
-            
+
         if jinjatags not in self.modules:
             self.modules.append(jinjatags)
-        
+
     def parse(self, tag: T.Optional[ext.Tags] = None) -> T.Union[str, ext.Tags, None]:
         for token in self.tokens:
             if not token.name:
                 # myst_parser gives out Data['abc'] kind of Token with {"name":'', 'data': 'abc', ...} attributes
                 # we are parsing plain strings, <script> body or jinja token strings here
 
                 if hasattr(token, "data"):
                     # handle leading and trailing newline with spaces in myst parser Data Token ex: "  \n Hello\n  "
                     if data := token.data.strip("\n").strip(" ").strip("\n"):
-                        with (tag or ConcatTag()) as tag:
+                        with tag or ext.PlaceholderTag() as tag:
                             # handling
                             if tag.__class__.__name__ == "script":
                                 dom_text(data, escape=False)
                             else:
                                 if token.__class__.__name__ != "Comment":
                                     if data.startswith("{") and data.endswith("}"):
                                         # these are jinja tags
                                         dom_text(data, escape=False)
                                     else:
                                         # normal text is here
-                                        dom_text(data, escape=True)
+                                        dom_text(data, escape=self.escape)
                                 else:
                                     # this is a comment section
                                     htmltags.comment(data)
 
             else:
                 element = None
                 tag_name = token.name
                 if tag_name in builtins.__dict__:
                     # work around for builtins like 'input' tag
-                    tag_name = ''.join([token.name, "_"])
-                    
+                    tag_name = "".join([token.name, "_"])
+
                 for module in self.modules:
                     try:
                         element = getattr(module, tag_name)
+                        if element is not None:
+                            break
                     except (AttributeError,):
                         pass
                 if element is None:
                     element = create_dynamic_element(tag_name=tag_name)
-                
-                tag = tag if tag is not None else ConcatTag()
-                
-                with tag:
-                    with element(**token.attrs) as child_tag:
-                        HTMLStringToDom(token.children, modules=self.modules).parse(tag=child_tag)
+
+                # tag = tag if tag is not None else ConcatTag()
+
+                if tag is not None:
+                    with tag:
+                        with element(**token.attrs) as child_tag:
+                            HTMLStringToDom(
+                                token.children, modules=self.modules, escape=self.escape
+                            ).parse(tag=child_tag)
+                else:
+                    with element(**token.attrs) as tag:
+                        HTMLStringToDom(
+                            token.children, modules=self.modules, escape=self.escape
+                        ).parse(tag=tag)
         return tag
 
     def __repr__(self):
         return str(self.parse())
 
 
-@dataclass
-class HTMLStringToElement(HTMLElement):
-    # TODO convert DOM object instance to Code Object for AST conversion to python code.
-    # from https://stackoverflow.com/questions/68577587/how-to-find-the-ast-assignment-node-related-to-the-instance-creation
-    # this.ast_object can be easily used to create python code for any html object
-    # https://stackoverflow.com/a/68584740 for parsing a python object into an ast_object
-    # https://stackoverflow.com/a/63212256 for unparsing a python ast_object
-
-
-    def __init__(self, *args, **kwargs):
-        super(HTMLStringToElement, self).__init__(*args, **kwargs)
-
-    def __render__(self, raw_string) -> T.Union[str, ext.Tags, None]: # noqa
-        return HTMLStringToDom(raw_string).parse()
+# don't decorate string_to_element with functools.lru_cache because if string_to_element is used in isolation
+# like:
+# with div() as parent_div:
+#   child_element = string_to_element("some html string")
+#
+# with lru_cache decorated on string_to_element the evaluation of child_element at run time will not happen twice
+# and thus parent_div will never add child_element in subsequest runs thus better way to cache string_to_element
+# evaluation is to cache the method where it is used.
+def string_to_element(raw_string, escape=True) -> T.List[ext.Tags]:  # noqa
+    tokens = tokenize_html(raw_string).children
+    elements = []
+    for token in tokens:
+        element = HTMLStringToDom([token], escape=escape).parse()
+        if element:
+            assert isinstance(
+                element, ext.Tags
+            ), f"{element=} is not instance of {ext.Tags}"
+            elements.append(element)
+    return elements
+    # element = HTMLStringToDom(raw_string, escape=escape).parse()
+    # assert isinstance(element, ext.Tags), f"{element=} is not instance of {ext.Tags}"
+    # return element
 
 
 # if __name__ == '__main__':
-    # from uidom.dom import ConcatTag, For, Var, div, li, raw, script, ul
+# from uidom.dom import ConcatTag, For, Var, div, li, raw, script, ul
 
-    # print(HTMLStringToElement("<li><ul><i><!--Hello World--></i></ul><a href='www.google.com'></a></li>"))
+# print(HTMLStringToElement("<li><ul><i><!--Hello World--></i></ul><a href='www.google.com'></a></li>"))
 #     class XName(ext.Tags):
 #         tagname = "x-name"
 
 
-    # print(HTMLStringToDom(div("hello", div("Jai SHree Ram"), script(raw("function () => {}")), className="sdaf")).parse())
-    # print(div("hello", div("Jai SHree Ram"), script(raw("function () => {}")), className="sdaf"))
-    # print(StringToDom(str(div("hello", div("Jai SHree Ram"), script(raw("function () => {}")), className="sdaf", x_data=None))))
-    # x = HTMLToPy(str(XName("hello", Var("haha"), ul(For("name in names", li(Var("name")))),
-    #                        div("Jai SHree Ram aa", className="safn"), script(raw("function () => {}")),
-    #                         script(src="https://unpkg.com/filepond/dist/filepond.js"),
-    #                         className="sdaf", x_data={}, x_transition_enter="")))
-    # print(x)
-    # print(XName("hello >", Var("haha >"), ul(For("name in names", li(Var("name")))),
-    #             div("Jai SHree Ram   a ", className="safn"), script(raw("function () => {}")),
-    #                         script(src="https://unpkg.com/filepond/dist/filepond.js"),
-    #                         className="sdaf", x_data={}, x_transition_enter=""))
-    # print(HTMLStringToDom(str(ul(For("name in names", li(Var("name")))))))
-    
+# print(HTMLStringToDom(div("hello", div("Jai SHree Ram"), script(raw("function () => {}")), className="sdaf")).parse())
+# print(div("hello", div("Jai SHree Ram"), script(raw("function () => {}")), className="sdaf"))
+# print(StringToDom(str(div("hello", div("Jai SHree Ram"), script(raw("function () => {}")), className="sdaf", x_data=None))))
+# x = HTMLToPy(str(XName("hello", Var("haha"), ul(For("name in names", li(Var("name")))),
+#                        div("Jai SHree Ram aa", className="safn"), script(raw("function () => {}")),
+#                         script(src="https://unpkg.com/filepond/dist/filepond.js"),
+#                         className="sdaf", x_data={}, x_transition_enter="")))
+# print(x)
+# print(XName("hello >", Var("haha >"), ul(For("name in names", li(Var("name")))),
+#             div("Jai SHree Ram   a ", className="safn"), script(raw("function () => {}")),
+#                         script(src="https://unpkg.com/filepond/dist/filepond.js"),
+#                         className="sdaf", x_data={}, x_transition_enter=""))
+# print(HTMLStringToDom(str(ul(For("name in names", li(Var("name")))))))
```

### Comparing `uidom-0.1.1b6/uidom/dom/htmldocument.py` & `uidom-0.2a0/uidom/dom/htmldocument.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,113 +1,130 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
+from dataclasses import dataclass, field
+
 from uidom.dom import htmlelement as htm
+from uidom.dom.src import dom_tag
 from uidom.dom.src.main import extension
 
-__all__ = [
-    "HtmlDocument"
-]
+__all__ = ["HtmlDocument"]
 
 
 class Meta(htm.HTMLElement):
-
-    def __render__(self, **kwargs):
+    def render(self, **kwargs):
         return self.html_tags.meta(**kwargs)
 
 
 class Head(htm.HTMLElement):
-
-    def __render__(self, *args, **kwargs):
+    def render(self, *args, **kwargs):
         return self.html_tags.head(*args, **kwargs)
 
 
 class Body(htm.HTMLElement):
-
-    def __render__(self, *args, **kwargs):
+    def render(self, *args, **kwargs):
         return self.html_tags.body(*args, **kwargs)
 
 
+@dataclass(eq=False)
 class HtmlDocument(htm.HTMLElement):
     csrf_field = "X-CSRF-TOKEN"
-    ensure_csrf_token_in_meta = True
+    ensure_csrf_token_in_meta: bool = field(default=True, init=False)
 
     def __init__(self, *args, **kwargs):
         self.document = self
         super(HtmlDocument, self).__init__(*args, **kwargs)
         self._entry = self.body
+        self._old_entry = None
 
-    def __script__(self, element):
-        ...
+    def __enter__(self):
+        super().__enter__()
+        self._old_entry = self._entry
+        self._entry = self._entry_with_context
+        return self
+
+    def __exit__(self, type, value, traceback):
+        super().__exit__(type, value, traceback)
+        self._entry = self._old_entry
 
-    def __checks__(self, element: extension.Tags) -> extension.Tags:
+    def __checks__(self, element):
         if self.ensure_csrf_token_in_meta:
             token_element = element.get(name=self.csrf_field)
             if not token_element:
-                raise AttributeError(f"{self.__class__.__qualname__} {self.csrf_field} must be set")
+                raise AttributeError(
+                    f"{self.__class__.__qualname__} {self.csrf_field} must be set"
+                )
             if len(token_element) > 1:
-                raise AssertionError(f"{self.__class__.__qualname__} {self.csrf_field} set at multiple places")
+                raise AssertionError(
+                    f"{self.__class__.__qualname__} {self.csrf_field} set at multiple places"
+                )
         return element
 
-    def __render__(self, *args, head=None, body=None, common_head=None, common_body=None, **kwargs):
-        common_head = [common_head] if not isinstance(common_head, list) else common_head
-        common_body = [common_body] if not isinstance(common_body, list) else common_body
+    def render(
+        self, *args, head=None, body=None, common_head=None, common_body=None, **kwargs
+    ):
+        common_head = (
+            [common_head] if not isinstance(common_head, list) else common_head
+        )
+        common_body = (
+            [common_body] if not isinstance(common_body, list) else common_body
+        )
         head = [head] if not isinstance(head, list) else head
         body = [body] if not isinstance(body, list) else body
 
         # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
         # ^Head Section
         # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
         self.head = Head()
 
         if any(head):
             for _head_file in head:
-                if isinstance(_head_file, extension.Tags):
+                if isinstance(_head_file, dom_tag):
                     self.head.add(_head_file)
                 elif isinstance(_head_file, str):
                     self.head.add(self.html_tags.link(href=_head_file))
                 elif isinstance(_head_file, dict):
                     self.head.add(self.html_tags.link(**_head_file))
 
         if any(common_head):
-            _ = [self.head.add(_hd) for _hd in common_head if isinstance(_hd, extension.Tags)]
+            _ = [self.head.add(_hd) for _hd in common_head if isinstance(_hd, dom_tag)]
         # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
         # $Head Section
         # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
 
         # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
         # ^Body Section
         # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
-        self.body = Body(*args, **kwargs)
+        self._entry_with_context = extension.PlaceholderTag()
+        self.body = Body(self._entry_with_context, *args, **kwargs)
 
         if any(body):
             for _body_file in body:
-                if isinstance(_body_file, extension.Tags):
+                if isinstance(_body_file, dom_tag):
                     self.body.add(_body_file)
                 elif isinstance(_body_file, str):
                     self.body.add(self.html_tags.script(src=_body_file))
                 elif isinstance(_body_file, dict):
                     self.body.add(self.html_tags.script(**_body_file))
 
         if any(common_body):
-            _ = [self.body.add(_bd) for _bd in common_body if isinstance(_bd, extension.Tags)]
+            _ = [self.body.add(_bd) for _bd in common_body if isinstance(_bd, dom_tag)]
         # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
         # $Body Section
         # ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++ #
         if not self.head.get("meta", name="viewport"):
             viewport_meta = Meta(
                 name="viewport",
-                content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no, minimal-ui"
+                content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no, minimal-ui",
             )
             self.head.add(viewport_meta)
 
         if not self.head.get("meta", charset="utf-8"):
             charset = Meta(charset="utf-8")
             self.head.add(charset)
 
         self.html = self.html_tags.html(self.head, self.body)
         doc = self.html_tags.DocType("html")
-        return self.html_tags.ConcatTag(doc, self.html)
-
+        return doc & self.html
```

### Comparing `uidom-0.1.1b6/uidom/dom/htmlelement.py` & `uidom-0.2a0/uidom/dom/htmlelement.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,197 +1,206 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
-from dataclasses import dataclass, field, make_dataclass
-from typing import Union
+from dataclasses import dataclass
 
 from uidom.dom.src import DoubleTags, component
+from uidom.dom.src.jinjatags import render
 
 __all__ = [
     "HTMLElement",
     "AMPElement",
     "XComponent",
     "CustomElement",
     "WebComponent",
     "AlpineElement",
     "AlpineComponent",
+    "JinjaElement",
+    "MarkdownElement",
 ]
 
 
 @dataclass
 class HtmlBaseMiddleware(object):
     """
     HTMLBaseMiddleware to intercept and modify dom elements.
     """
 
 
 @dataclass(eq=False)
 class HTMLElement(component.Component):
-    file_extension = ".html"
-
     def __init__(self, *args, **kwargs):
         super(HTMLElement, self).__init__(*args, **kwargs)
 
-    def __render__(self, *args, **kwargs):
-        return self.html_tags.ConcatTag(*args, **kwargs)
-
-    def __script__(self, *args, **kwargs):
-        ...
+    def __post_init__(self, *args, **kwargs):
+        super(HTMLElement, self).__post_init__(*args, **kwargs)
 
-    def __repr__(self):
-        return str(self)
+    def __and__(self, other):
+        return super().__and__(other)
 
 
 @dataclass(eq=False)
-class AMPElement(HTMLElement):
+class AMPElement(component.Component):
     tag_name: str
 
     def __post_init__(self, *args, **kwargs):
         super(AMPElement, self).__init__(*args, tag_name=self.tag_name, **kwargs)
 
         class Element(DoubleTags):
             tagname = f"amp-{self.tag_name}"  # noqa
 
-        element = Element
-
-        self.Element = element
+        self.Element = Element
         self.Element.is_inline = self.is_inline
         self.Element.is_single = self.is_single
         self.Element.is_pretty = self.is_pretty
 
     def __call__(self, *args, **kwargs):
         return self.Element(*args, **kwargs)
 
+    def __and__(self, other):
+        return super().__and__(other)
 
-# here init=False is necessary to avoid double initialization
-@dataclass(init=False, eq=False)
-class XComponent(HTMLElement):
-    fields = None
+
+@dataclass(eq=False)
+class XComponent(component.Component):
     tag_name: str
 
     def __post_init__(self, *args, **kwargs):
         super(XComponent, self).__init__(*args, tag_name=self.tag_name, **kwargs)
-        if self.fields is not None:
-            element = make_dataclass(cls_name=''.join(map(lambda x: x.capitalize(), self.tag_name.split('-'))),
-                                     fields=[*self.fields,
-                                             ("tagname", str, field(init=False, default=f"x-{self.tag_name}")),
-                                             ("attributes", dict, field(init=False, default_factory=lambda: dict())),
-                                             ("children", list, field(init=False, default_factory=lambda: list())),
-                                             ("document", list, field(init=False, default_factory=lambda: None)),
-                                             ],
-                                     bases=(DoubleTags,), )
-        else:
-            class Element(DoubleTags):
-                tagname = f"x-{self.tag_name}"  # noqa
 
-            element = Element
+        class Element(DoubleTags):
+            tagname = f"x-{self.tag_name}"  # noqa
 
-        self.Element = element
+        self.Element = Element
         self.Element.is_inline = self.is_inline
         self.Element.is_single = self.is_single
         self.Element.is_pretty = self.is_pretty
-        # self.__call__ = element.__init__
 
     def __checks__(self, element):
-        HTMLElement.__checks__(self, element)
+        component.Component.__checks__(self, element)
         return self.__x_component_checks(element)
 
     def __x_component_checks(self, element):
-        if not element.attributes.get("x-component"):
-            if not element.get(x_component=self.tag_name):
-                raise AttributeError(f"{element.__class__.__qualname__}: must have 'x_component' attribute")
-        return super(HTMLElement, self).__checks__(element)
+        x_component_attr = None
+        try:
+            # check if "x-component" attribute is present in element, if it throws error raise
+            # AttributeError
+            x_component_attr = element["x-component"]
+        except AttributeError:
+            pass
+
+        if not x_component_attr:
+            raise AttributeError(
+                f"{self.__class__.__name__}.{element.__class__.__qualname__}: must have 'x-component' attribute"
+            )
+        return element
 
     def __call__(self, *args, **kwargs):
         return self.Element(*args, **kwargs)
 
+    def __and__(self, other):
+        return super().__and__(other)
+
 
 @dataclass(eq=False)
 class CustomElement(XComponent):
     # using x-component attribute to upgrade to the element in html to light-element
 
     def __checks__(self, element):
         XComponent.__checks__(self, element)
         return self.__custom_element_checks(element)
 
     def __custom_element_checks(self, element):  # noqa
-        if (element.attributes.get("shadowroot") or element.get(shadowroot="shadowroot") or element.get(
-                shadowroot="true")):
-            raise AttributeError(f"{element.__class__.__qualname__}: must not have 'shadowroot' attribute")
+        shadow_root_attr = None
+        try:
+            shadow_root_attr = element["shadowroot"]
+        except AttributeError:
+            pass
+
+        if shadow_root_attr:
+            raise AttributeError(
+                f"{self.__class__.__name__}.{element.__class__.__qualname__}: must not have 'shadowroot' attribute"
+            )
         return element
 
-    def __render__(self, tag_name):
-        return self.html_tags.template(self.html_tags.div(x_component=tag_name))
+    def render(self, tag_name):
+        # smallest example of custom elements
+        with self.html_tags.template(x_component=tag_name) as cus_elem:
+            self.html_tags.div()
+        return cus_elem
 
 
 @dataclass(eq=False)
 class WebComponent(XComponent):
-    # using x-component attribute to upgrade to the element in html to shadow-element
+    # using "shadowroot" attribute to upgrade to the element in html to shadow-element
 
     def __checks__(self, element):
         XComponent.__checks__(self, element)
         return self.__web_component_checks(element)
 
     def __web_component_checks(self, element):  # noqa
-        if not (element.attributes.get("shadowroot") or element.get(shadowroot="shadowroot") or element.get(
-                shadowroot="true")):
-            raise AttributeError(f"{element.__class__.__qualname__}: must have 'shadowroot' attribute set")
+        shadow_root_attr = element.get(shadowroot=None)
+
+        if not shadow_root_attr:
+            raise AttributeError(
+                f"{self.__class__.__name__}.{element.__class__.__qualname__}: must have 'shadowroot' attribute"
+            )
         return element
 
-    def __render__(self, tag_name):
+    def render(self, tag_name):
         # smallest example of a web component
-        return self.html_tags.template(self.html_tags.div(x_component=tag_name, shadowroot="true"))
+        with self.html_tags.template(
+            x_component=tag_name, shadowroot="true"
+        ) as web_comp:
+            self.html_tags.slot()
+        return web_comp
 
 
 @dataclass(eq=False)
-class AlpineElement(HTMLElement):
-    x_data: Union[str, dict, bool, None] = False
-
+class AlpineElement(component.Component):
     def __checks__(self, element):
-        HTMLElement.__checks__(self, element)
         return self.__alpine_js_checks(element)
 
     def __alpine_js_checks(self, element):
-        if not self.x_data:
-            x_data = element.attributes.get("x-data") or element.get(x_data=self.x_data)
-            if not x_data or x_data == "False":
-                raise AttributeError(f"{element.__class__.__qualname__}: must have 'x-data' attribute")
+        # we look for x_data=None because we exactly don't know if its value is present,
+        # so we get x_data for any value by making x_data=None.
+        x_data_attr = element.get(x_data=None)
+
+        if not x_data_attr:
+            raise AttributeError(
+                f"{self.__class__.__name__}.{element.__class__.__qualname__}: must have 'x-data' attribute"
+            )
         return element
 
-    def __render__(self, *args, **kwargs):
+    def render(self, *args, **kwargs):
         ...
 
+    def __and__(self, other):
+        return super().__and__(other)
+
 
 @dataclass(eq=False)
 class AlpineComponent(AlpineElement, XComponent):
-
     def __checks__(self, element):
         XComponent.__checks__(self, element)
         return AlpineElement.__checks__(self, element)
 
 
-# if __name__ == '__main__':
-    # image = CustomElement(tag_name="img")
-    # print(image)
-    # x = image(image(image("hello")), src="http://....", alt="some image", className="h-32 w-32")
-    # print(x)
-    # # print(signature(image))
-    # def story(*args, **kwargs):
-    #     return AMPElement(tag_name="story-page")(
-    #         AMPElement(tag_name="story-grid-layer")(
-    #             AMPElement(tag_name="video")(*args, **kwargs),
-    #     template="fill"),
-    #     id="cover"
-    # )
-
-    # print(
-    #     story(
-    #         layout="fill", 
-    #         src="background.mp4", 
-    #         poster="https://images.unsplash.com/photo-1605100804763-247f67b3557e?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=870&q=80", 
-    #         muted=None, 
-    #         autoplay=None
-    #         )
-    #       )
+class JinjaElement(component.Component):
+    escape_string = False
+
+    def render(self, elem_or_str_or_path):
+        return elem_or_str_or_path
+
+    def __call__(self, **options):
+        return render(self, **options)
+
+
+class MarkdownElement(component.Component):
+    escape_string = False
+    string_is_markdown = True
+
+    def render(self, md_str_or_path):
+        return md_str_or_path
```

### Comparing `uidom-0.1.1b6/uidom/dom/icons.py` & `uidom-0.2a0/uidom/dom/icons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,66 +1,70 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
-from uidom.dom.htmlelement import HTMLElement
+from uidom.dom.src import Component
 from uidom.dom.src.utils import raw
 
 
-class Icons(HTMLElement):
-
-    def __render__(
-            self,
-            *args,
-            version="1.1",
-            id="Layer_1",
-            x="0px",
-            y="0px",
-            viewBox="0 0 512 512",
-            style="enable-background:new 0 0 512 512;",
-            xmlns="http://www.w3.org/2000/svg",
-            xmlns_xlink="http://www.w3.org/1999/xlink",
-            xml_space="preserve",
-            **kwargs
+class Icons(Component):
+    def render(
+        self,
+        *args,
+        version="1.1",
+        id="Layer_1",
+        x="0px",
+        y="0px",
+        viewBox="0 0 512 512",
+        style="enable-background:new 0 0 512 512;",
+        xmlns="http://www.w3.org/2000/svg",
+        xmlns_xlink="http://www.w3.org/1999/xlink",
+        xml_space="preserve",
+        **kwargs
     ):
-        return self.svg_tags.svg(version=version,
-                   id=id,
-                   xmlns=xmlns,
-                   xmlns_xlink=xmlns_xlink,
-                   x=x,
-                   y=y,
-                   viewBox=viewBox,
-                   style=style,
-                   xml_space=xml_space,
-                   **kwargs)
+        return self.svg_tags.svg(
+            version=version,
+            id=id,
+            xmlns=xmlns,
+            xmlns_xlink=xmlns_xlink,
+            x=x,
+            y=y,
+            viewBox=viewBox,
+            style=style,
+            xml_space=xml_space,
+            **kwargs
+        )
 
 
 # logos taken from https://www.svgrepo.com/collection/jewelry-2/
 diamond_icon = Icons()
 diamond_icon.add(
-    diamond_icon.svg_tags.path(d="M424.729,192.453l-53.025-81.188c-4.475-6.842-12.006-10.927-20.142-10.927h-112.28c-4.329,0-7.837,3.509-7.837,7.837\
+    diamond_icon.svg_tags.path(
+        d="M424.729,192.453l-53.025-81.188c-4.475-6.842-12.006-10.927-20.142-10.927h-112.28c-4.329,0-7.837,3.509-7.837,7.837\
 			c0,4.329,3.508,7.837,7.837,7.837h2.146l-37.541,57.471l-37.541-57.471h40.544c4.329,0,7.837-3.508,7.837-7.837\
 			c0-4.328-3.508-7.837-7.837-7.837h-46.448c-8.144,0-15.673,4.087-20.144,10.931l-53.026,81.182\
 			c-5.842,8.94-5.224,20.495,1.535,28.755L237.39,402.786c4.595,5.618,11.379,8.841,18.612,8.841c7.23,0,14.012-3.221,18.609-8.839\
 			l84.218-102.918c2.741-3.35,2.247-8.288-1.102-11.029c-3.35-2.74-8.286-2.248-11.029,1.102l-75.269,91.983l54.819-167.212h82.011\
 			l-39.975,48.851c-2.741,3.35-2.247,8.288,1.102,11.029c1.458,1.192,3.213,1.771,4.959,1.771c2.268,0,4.52-0.98,6.07-2.873\
 			l42.784-52.286C429.954,212.948,430.569,201.394,424.729,192.453z M345.654,116.012l-37.542,57.47l-37.54-57.47H345.654z\
 			 M151.772,122.363l42.754,65.451l-7.334,11.226h-85.504L151.772,122.363z M256.024,378.598l-31.543-96.813\
 			c-1.341-4.116-5.769-6.367-9.878-5.024c-4.116,1.341-6.364,5.764-5.024,9.878l31.079,95.39L103.746,214.714h82.399l13.904,42.674\
 			c1.077,3.309,4.148,5.411,7.449,5.411c0.805,0,1.624-0.124,2.429-0.388c4.116-1.341,6.365-5.764,5.024-9.878l-12.322-37.818\
 			h39.423c4.329,0,7.837-3.508,7.837-7.837c0-4.329-3.508-7.837-7.837-7.837h-36.138L256,122.363l50.087,76.678h-26.549\
 			c-4.329,0-7.837,3.508-7.837,7.837c0,4.329,3.508,7.837,7.837,7.837h30.212L256.024,378.598z M324.809,199.041l-7.335-11.228\
-			l42.756-65.453l50.082,76.682H324.809z")
+			l42.756-65.453l50.082,76.682H324.809z"
+    )
 )
 
 color_stone_icon = Icons()
-color_stone_icon.add(color_stone_icon.svg_tags.path(
-    d="M463.669,207.941l-26.24-40.374c-2.922-4.49-7.83-7.183-13.152-7.229v-59.851c0-7.203-5.859-13.061-13.061-13.061H302.759\
+color_stone_icon.add(
+    color_stone_icon.svg_tags.path(
+        d="M463.669,207.941l-26.24-40.374c-2.922-4.49-7.83-7.183-13.152-7.229v-59.851c0-7.203-5.859-13.061-13.061-13.061H302.759\
 	   V75.898c0-7.202-5.859-13.061-13.061-13.061H196.13c-7.203,0-13.061,5.859-13.061,13.061v11.528H74.614\
 			c-7.202,0-13.061,5.859-13.061,13.061v95.91l-19.62,19.62c-3.429,3.427-4.872,8.317-3.861,13.081l5.661,26.686\
 			c-4.588,2.028-7.801,6.616-7.801,11.946v180.672c0,7.202,5.859,13.061,13.061,13.061h7.271v12.667\
 			c0,7.202,5.859,13.061,13.061,13.061h36.114c7.202,0,13.061-5.859,13.061-13.061v-12.667h248.831v12.667\
 			c0,7.202,5.859,13.061,13.061,13.061h36.112c7.202,0,13.061-5.859,13.061-13.061v-12.667h7.271\
 			c7.203,0,13.061-5.859,13.061-13.061V267.731c0-6.203-4.35-11.399-10.157-12.725l22.92-28.148\
 			C467.085,221.422,467.49,213.82,463.669,207.941z M413.943,176.008l-11.301,17.384l-11.299-17.384H413.943z M326.316,225.089\
@@ -93,28 +97,34 @@
 			H81.304l4.448-4.448L94.468,254.67z M90.156,189.96l8.87-8.87l2.389,11.259L90.156,189.96z M113.85,175.439l20.226,4.291\
 			l-15.936,15.936L113.85,175.439z M69.681,210.436l2.389,11.258l-11.259-2.389L69.681,210.436z M75.387,238.42l-15.935,15.936\
 			l-4.291-20.225L75.387,238.42z M102.827,471.52h-0.001H71.938v-10.055h30.889V471.52z M413.891,471.52h-30.887v-10.055h30.887\
 			V471.52z M434.224,445.791H51.605V270.343h139.623v14.954H79.444c-7.202,0-13.061,5.859-13.061,13.061v119.415\
 			c0,7.202,5.859,13.061,13.061,13.061h326.942c7.202,0,13.061-5.859,13.061-13.061V298.358c0-7.203-5.859-13.061-13.061-13.061\
 			H294.6v-14.954h139.624V445.791z M419.803,254.67h-54.325l-9.59-29.58h41.941l-4.354,13.429c-1.334,4.117,0.922,8.537,5.037,9.871\
 			c0.802,0.26,1.619,0.385,2.419,0.385c3.305,0,6.378-2.108,7.453-5.422l5.921-18.263h29.582L419.803,254.67z M413.059,209.415\
-			l-1.068-1.644l16.438-25.292l17.505,26.935H413.059z"))
+			l-1.068-1.644l16.438-25.292l17.505,26.935H413.059z"
+    )
+)
 
 
-color_stone_icon2 = Icons(version="1.1",
-                          id="Layer_1",
-                          xmlns="http://www.w3.org/2000/svg",
-                          xmlns_xlink="http://www.w3.org/1999/xlink",
-                          x="0px",
-                          y="0px",
-	                      viewBox="0 0 512.013 512.013",
-                          style="enable-background:new 0 0 512.013 512.013;",
-                          xml_space="preserve")
+color_stone_icon2 = Icons(
+    version="1.1",
+    id="Layer_1",
+    xmlns="http://www.w3.org/2000/svg",
+    xmlns_xlink="http://www.w3.org/1999/xlink",
+    x="0px",
+    y="0px",
+    viewBox="0 0 512.013 512.013",
+    style="enable-background:new 0 0 512.013 512.013;",
+    xml_space="preserve",
+)
 
-color_stone_icon2.add(color_stone_icon2.svg_tags.path(d="M376.308,507.071c0.495-0.414,0.982-0.845,1.45-1.313l106.667-106.667c0.468-0.468,0.899-0.955,1.314-1.45\
+color_stone_icon2.add(
+    color_stone_icon2.svg_tags.path(
+        d="M376.308,507.071c0.495-0.414,0.982-0.845,1.45-1.313l106.667-106.667c0.468-0.468,0.899-0.955,1.314-1.45\
 				c0.062-0.075,0.125-0.15,0.186-0.226c3.219-3.955,4.746-8.675,4.746-13.352c0-0.019,0.003-0.038,0.003-0.057v-256\
 				c0-0.019-0.003-0.038-0.003-0.057c0-4.677-1.527-9.396-4.746-13.352c-0.061-0.076-0.124-0.151-0.186-0.226\
 				c-0.414-0.495-0.845-0.982-1.314-1.45L377.758,6.255c-0.468-0.468-0.955-0.899-1.45-1.313c-0.076-0.063-0.151-0.125-0.227-0.187\
 				c-3.955-3.219-8.673-4.745-13.35-4.745c-0.02,0-0.039-0.003-0.059-0.003H149.34c-0.02,0-0.039,0.003-0.059,0.003\
 				c-4.676,0-9.395,1.527-13.35,4.745c-0.076,0.062-0.151,0.124-0.227,0.187c-0.495,0.414-0.982,0.845-1.45,1.313L27.588,112.922\
 				c-0.468,0.468-0.899,0.955-1.313,1.45c-0.063,0.076-0.125,0.151-0.187,0.227c-3.219,3.955-4.745,8.673-4.745,13.35\
 				c0,0.02-0.003,0.039-0.003,0.059v256c0,0.02,0.003,0.039,0.003,0.059c0,4.676,1.527,9.395,4.745,13.35\
@@ -122,22 +132,24 @@
 				c0.076,0.063,0.151,0.125,0.227,0.187c3.955,3.219,8.674,4.746,13.351,4.745c0.019,0,0.038,0.003,0.057,0.003h213.333\
 				c0.019,0,0.038-0.003,0.057-0.003c4.677,0,9.396-1.526,13.351-4.745C376.158,507.197,376.233,507.134,376.308,507.071z\
 				 M111.091,89.758l30.456-30.456l25.427,63.567l-22.773,22.773l-63.567-25.427L111.091,89.758z M200.852,362.682l-30.178-30.178\
 				V179.518l30.17-30.17H311.17l30.17,30.17v152.985l-30.179,30.178H200.852z M384.006,185.117l64-25.6v192.98l-64-25.6V185.117z\
 				 M305.56,106.682h-99.106L180.85,42.673h150.313L305.56,106.682z M128.006,185.117v141.78l-64,25.6v-192.98L128.006,185.117z\
 				 M206.446,405.348h99.12l25.597,63.991H180.85L206.446,405.348z M370.465,452.711l-25.424-63.561l22.776-22.776l63.561,25.424\
 				l-30.456,30.456L370.465,452.711z M431.378,120.215l-63.567,25.427l-22.773-22.773l25.427-63.567L431.378,120.215z\
-				 M80.635,391.798l63.561-25.424l22.776,22.776l-25.424,63.561L80.635,391.798z")
-                )
+				 M80.635,391.798l63.561-25.424l22.776,22.776l-25.424,63.561L80.635,391.798z"
+    )
+)
 
 
 jewellery_icon = Icons()
 jewellery_icon.add(
     jewellery_icon.svg_tags.path(
-        d="M491.779,150.646C491.756,150.591,491.756,150.591,491.779,150.646L491.779,150.646z"),
+        d="M491.779,150.646C491.756,150.591,491.756,150.591,491.779,150.646L491.779,150.646z"
+    ),
     jewellery_icon.svg_tags.path(
         d="M493.024,153.494c0.297,0.68,0.421,0.963-0.002-0.005c-0.82-1.877-1.167-2.67-1.243-2.844\
 				c0.126,0.289,0.839,1.92,1.241,2.839c-3.459-7.91-8.947-11.056-14.758-14.387C405.45,97.372,359.151,53.593,354.41,21.988\
 				C352.529,9.452,341.392,0,328.502,0h-58.92c-4.329,0-7.837,3.509-7.837,7.837c0,4.328,3.508,7.837,7.837,7.837h58.92\
 				c5.195,0,9.669,3.715,10.408,8.64c3.444,22.958,22.398,49.013,54.858,76.218c-4.032,7.235-8.307,14.364-12.815,21.378\
 				c-3.573-1.384-7.45-2.151-11.505-2.151c-17.616,0-31.948,14.332-31.948,31.948c0,7.229,2.417,13.902,6.48,19.262\
 				c-3.81,4.344-7.72,8.619-11.721,12.824c-4.752-2.808-10.288-4.427-16.197-4.427c-17.616,0-31.949,14.332-31.949,31.948\
@@ -174,126 +186,168 @@
 				c0.64,0.16,1.28,0.237,1.911,0.237c3.509,0,6.703-2.375,7.594-5.933c9.525-37.994,14.538-78.069,14.901-119.112\
 				C495.178,160.284,494.465,156.792,493.024,153.494z M143.099,167.979c-8.974,0-16.274-7.301-16.274-16.274\
 				s7.301-16.274,16.274-16.274s16.274,7.301,16.274,16.274S152.073,167.979,143.099,167.979z M281.72,282.099\
 				c0,14.031-11.415,25.445-25.446,25.445c-14.031,0-25.446-11.414-25.446-25.445c0-14.031,11.416-25.445,25.446-25.445\
 				C270.304,256.654,281.72,268.069,281.72,282.099z M316.064,227.587c-8.975,0-16.275-7.301-16.275-16.274\
 				s7.301-16.274,16.275-16.274c8.974,0,16.273,7.301,16.273,16.274C332.338,220.286,325.037,227.587,316.064,227.587z\
 				 M369.448,167.979c-8.974,0-16.274-7.301-16.274-16.274s7.301-16.274,16.274-16.274c8.974,0,16.274,7.301,16.274,16.274\
-				C385.723,160.678,378.422,167.979,369.448,167.979z"),
-    jewellery_icon.svg_tags.path(d="M256.274,362.432c-22.673,0-41.12,18.446-41.12,41.12c0,22.673,18.446,41.119,41.12,41.119\
+				C385.723,160.678,378.422,167.979,369.448,167.979z"
+    ),
+    jewellery_icon.svg_tags.path(
+        d="M256.274,362.432c-22.673,0-41.12,18.446-41.12,41.12c0,22.673,18.446,41.119,41.12,41.119\
 			c22.674,0,41.12-18.446,41.12-41.119C297.393,380.879,278.948,362.432,256.274,362.432z M256.274,428.997\
 			c-14.031,0-25.446-11.414-25.446-25.445s11.416-25.446,25.446-25.446c14.031,0,25.446,11.414,25.446,25.446\
-			C281.72,417.583,270.304,428.997,256.274,428.997z")
+			C281.72,417.583,270.304,428.997,256.274,428.997z"
+    ),
 )
 
 gemstone_icon_alt = Icons()
-gemstone_icon_alt.add(gemstone_icon_alt.svg_tags.path(
-    d="M220.278,305.633c4.328,0,7.837-3.509,7.837-7.837V233.49c0-5.767-2.46-11.316-6.752-15.226l-87.531-79.654\
+gemstone_icon_alt.add(
+    gemstone_icon_alt.svg_tags.path(
+        d="M220.278,305.633c4.328,0,7.837-3.509,7.837-7.837V233.49c0-5.767-2.46-11.316-6.752-15.226l-87.531-79.654\
 			c-3.856-3.512-8.863-5.445-14.101-5.445c-5.238,0-10.246,1.934-14.102,5.444l-87.533,79.657\
 			c-4.288,3.904-6.748,9.453-6.748,15.225v176.902c0,5.714,2.417,11.223,6.628,15.114l87.533,80.938\
 			c3.875,3.582,8.927,5.555,14.222,5.555c5.298,0,10.349-1.974,14.22-5.556l87.531-80.936c4.215-3.894,6.633-9.404,6.633-15.117\
 			v-83.339c0-4.328-3.509-7.837-7.837-7.837s-7.837,3.509-7.837,7.837v72.6l-36.383-11.655v-131.95l36.383-11.782v53.53\
 			C212.441,302.124,215.95,305.633,220.278,305.633z M111.893,154.097v48.658l-42.567,38.736L29.892,228.72L111.893,154.097z\
 			 M27.02,244.266l36.38,11.782v131.95l-36.38,11.654V244.266z M111.893,491.003L29.9,415.188l39.374-12.613l42.619,39.407V491.003z\
 			 M209.557,415.187L127.567,491v-49.018l42.616-39.407L209.557,415.187z M170.132,241.492l-11.261-10.248\
 			c-3.199-2.912-8.156-2.679-11.071,0.521c-2.913,3.201-2.679,8.158,0.521,11.071l12.062,10.977V390.29l-40.653,37.592\
 			L79.074,390.29V253.813l40.656-36.998l8.746,7.958c3.201,2.912,8.157,2.679,11.071-0.521c2.913-3.202,2.679-8.158-0.521-11.071\
-			l-11.457-10.427v-48.655l81.999,74.62L170.132,241.492z"))
+			l-11.457-10.427v-48.655l81.999,74.62L170.132,241.492z"
+    )
+)
 
 
-metal_icon = Icons(id="Capa_1", viewBox="0 0 311.783 311.783", style="enable-background:new 0 0 311.783 311.783;")
-metal_icon.add(metal_icon.svg_tags.path(d="M198.523,123.575h-85.262c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.768-40.632\
+metal_icon = Icons(
+    id="Capa_1",
+    viewBox="0 0 311.783 311.783",
+    style="enable-background:new 0 0 311.783 311.783;",
+)
+metal_icon.add(
+    metal_icon.svg_tags.path(
+        d="M198.523,123.575h-85.262c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.768-40.632\
 			c0.991-3.42,4.123-5.774,7.685-5.774h61.726c3.561,0,6.693,2.354,7.684,5.774l11.768,40.632c0.699,2.416,0.222,5.021-1.289,7.032\
-			C203.407,122.392,201.038,123.575,198.523,123.575z M123.906,107.575h63.971l-7.134-24.632h-49.702L123.906,107.575z"),
-               metal_icon.svg_tags.path(d="M145.891,184.208H60.63c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.769-40.632\
+			C203.407,122.392,201.038,123.575,198.523,123.575z M123.906,107.575h63.971l-7.134-24.632h-49.702L123.906,107.575z"
+    ),
+    metal_icon.svg_tags.path(
+        d="M145.891,184.208H60.63c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.769-40.632\
 			c0.991-3.421,4.123-5.774,7.685-5.774h61.726c3.561,0,6.693,2.354,7.685,5.775l11.767,40.632c0.699,2.416,0.222,5.021-1.289,7.031\
-			C150.774,183.025,148.406,184.208,145.891,184.208z M71.275,168.208h63.97l-7.133-24.632H78.41L71.275,168.208z"),
-               metal_icon.svg_tags.path(d="M251.153,184.208h-85.261c-2.516,0-4.884-1.183-6.396-3.194c-1.511-2.011-1.988-4.615-1.289-7.031l11.767-40.632\
+			C150.774,183.025,148.406,184.208,145.891,184.208z M71.275,168.208h63.97l-7.133-24.632H78.41L71.275,168.208z"
+    ),
+    metal_icon.svg_tags.path(
+        d="M251.153,184.208h-85.261c-2.516,0-4.884-1.183-6.396-3.194c-1.511-2.011-1.988-4.615-1.289-7.031l11.767-40.632\
 			c0.991-3.421,4.123-5.775,7.685-5.775h61.726c3.561,0,6.693,2.354,7.684,5.774l11.769,40.632c0.699,2.416,0.222,5.02-1.289,7.032\
-			C256.038,183.025,253.669,184.208,251.153,184.208z M176.538,168.208h63.97l-7.135-24.632h-49.702L176.538,168.208z"),
-               metal_icon.svg_tags.path(d="M93.261,244.84H8c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.769-40.632\
+			C256.038,183.025,253.669,184.208,251.153,184.208z M176.538,168.208h63.97l-7.135-24.632h-49.702L176.538,168.208z"
+    ),
+    metal_icon.svg_tags.path(
+        d="M93.261,244.84H8c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.769-40.632\
 			c0.991-3.42,4.123-5.774,7.685-5.774h61.725c3.561,0,6.693,2.354,7.684,5.774l11.768,40.632c0.699,2.416,0.222,5.021-1.289,7.032\
-			C98.146,243.657,95.776,244.84,93.261,244.84z M18.646,228.84h63.97l-7.134-24.632H25.78L18.646,228.84z"),
-               metal_icon.svg_tags.path(d="M198.523,244.84h-85.262c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.767-40.632\
+			C98.146,243.657,95.776,244.84,93.261,244.84z M18.646,228.84h63.97l-7.134-24.632H25.78L18.646,228.84z"
+    ),
+    metal_icon.svg_tags.path(
+        d="M198.523,244.84h-85.262c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.767-40.632\
 			c0.991-3.42,4.123-5.774,7.685-5.774h61.726c3.561,0,6.693,2.354,7.685,5.774l11.768,40.632c0.699,2.416,0.222,5.02-1.289,7.032\
-			C203.407,243.657,201.038,244.84,198.523,244.84z M123.906,228.84h63.971l-7.135-24.632H131.04L123.906,228.84z"),
-               metal_icon.svg_tags.path(d="M303.783,244.84h-85.261c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.768-40.632\
+			C203.407,243.657,201.038,244.84,198.523,244.84z M123.906,228.84h63.971l-7.135-24.632H131.04L123.906,228.84z"
+    ),
+    metal_icon.svg_tags.path(
+        d="M303.783,244.84h-85.261c-2.516,0-4.885-1.183-6.396-3.194c-1.511-2.011-1.988-4.616-1.289-7.032l11.768-40.632\
 			c0.991-3.42,4.123-5.774,7.685-5.774h61.725c3.562,0,6.693,2.354,7.685,5.774l11.769,40.632c0.699,2.416,0.222,5.02-1.289,7.032\
-			C308.668,243.657,306.299,244.84,303.783,244.84z M229.168,228.84h63.97l-7.135-24.632h-49.701L229.168,228.84z")
-               )
+			C308.668,243.657,306.299,244.84,303.783,244.84z M229.168,228.84h63.97l-7.135-24.632h-49.701L229.168,228.84z"
+    ),
+)
 
 
-dots_horizontal = Icons(fill="none",
-                        xmlns="http://www.w3.org/2000/svg",
-                        viewBox="0 0 24 24",
-                        stroke="currentColor")
+dots_horizontal = Icons(
+    fill="none",
+    xmlns="http://www.w3.org/2000/svg",
+    viewBox="0 0 24 24",
+    stroke="currentColor",
+)
 dots_horizontal.add(
     dots_horizontal.svg_tags.path(
         stroke_linecap="round",
         stroke_linejoin="round",
         stroke_width="2",
         d="M12 5v.01M12 12v.01M12 19v.01M12 6a1 1 0 110-2 1 1 0 010 2zm0 7a1 1 0 110-2 1 1 0 010 "
-          "2zm0 7a1 1 0 110-2 1 1 0 010 2z"
-    ))
+        "2zm0 7a1 1 0 110-2 1 1 0 010 2z",
+    )
+)
 
 dots_horizontal["class"] = "h-6 w-6"
 
-bell_icon = Icons(version="1.1",
-                  id="Capa_1",
-                  xmlns="http://www.w3.org/2000/svg",
-                  xmlns_xlink="http://www.w3.org/1999/xlink",
-                  x="0px",
-                  y="0px",
-                  viewBox="0 0 297 297",
-                  style="enable-background:new 0 0 297 297;",
-                  xml_space="preserve")
-bell_icon.add(bell_icon.svg_tags.path(d="M249.357,192.818v-62.863c0-42.553-26.344-79.049-63.535-93.957C185.061,16.021,168.616,0,148.5,0\
+bell_icon = Icons(
+    version="1.1",
+    id="Capa_1",
+    xmlns="http://www.w3.org/2000/svg",
+    xmlns_xlink="http://www.w3.org/1999/xlink",
+    x="0px",
+    y="0px",
+    viewBox="0 0 297 297",
+    style="enable-background:new 0 0 297 297;",
+    xml_space="preserve",
+)
+bell_icon.add(
+    bell_icon.svg_tags.path(
+        d="M249.357,192.818v-62.863c0-42.553-26.344-79.049-63.535-93.957C185.061,16.021,168.616,0,148.5,0\
 		s-36.563,16.021-37.323,35.998c-37.191,14.908-63.534,51.404-63.534,93.957v62.863C37.399,194.28,29.5,203.123,29.5,213.778v14.34\
 		c0,11.676,9.483,21.175,21.14,21.175h61.928c-0.939,3.308-1.427,6.759-1.427,10.264c0,20.646,16.76,37.443,37.359,37.443\
 		s37.358-16.797,37.358-37.443c0-3.506-0.487-6.956-1.426-10.264h61.928c11.656,0,21.14-9.499,21.14-21.175v-14.34\
 		C267.5,203.123,259.601,194.28,249.357,192.818z M148.5,276.712c-9.413,0-17.071-7.695-17.071-17.155\
 		c0-2.891,0.721-5.699,2.07-8.191h30.002c1.35,2.492,2.069,5.301,2.069,8.191C165.57,269.017,157.912,276.712,148.5,276.712z\
 		 M148.5,20.289c6.75,0,12.58,3.969,15.349,9.696c-5.005-0.77-10.132-1.169-15.349-1.169c-5.218,0-10.344,0.399-15.351,1.169\
 		C135.918,24.258,141.749,20.289,148.5,20.289z M247.211,228.118c0,0.464-0.405,0.886-0.851,0.886H50.64\
 		c-0.445,0-0.85-0.422-0.85-0.886v-14.34c0-0.463,0.405-0.884,0.85-0.884h7.146c5.603,0,10.145-4.542,10.145-10.145v-72.795\
 		c0-44.581,36.144-80.85,80.569-80.85s80.569,36.269,80.569,80.85v72.795c0,5.602,4.542,10.145,10.145,10.145h7.146\
-		c0.445,0,0.851,0.421,0.851,0.884V228.118z"),
-              bell_icon.svg_tags.path(d="M184.787,101.611c-5.602,0-10.145,4.542-10.145,10.145v72.797c0,5.603,4.542,10.145,10.145,10.145\
-		c5.602,0,10.144-4.542,10.144-10.145v-72.797C194.931,106.153,190.389,101.611,184.787,101.611z")
-              )
-
-mail_icon = Icons(version="1.1",
-                  id="Capa_1",
-                  xmlns="http://www.w3.org/2000/svg",
-                  xmlns_xlink="http://www.w3.org/1999/xlink",
-                  x="0px",
-                  y="0px",
-              	  viewBox="0 0 474 474",
-                  style="enable-background:new 0 0 474 474;",
-                  xml_space="preserve")
-mail_icon.add(mail_icon.svg_tags.path(d="M437.5,59.3h-401C16.4,59.3,0,75.7,0,95.8v282.4c0,20.1,16.4,36.5,36.5,36.5h401c20.1,0,36.5-16.4,36.5-36.5V95.8\
+		c0.445,0,0.851,0.421,0.851,0.884V228.118z"
+    ),
+    bell_icon.svg_tags.path(
+        d="M184.787,101.611c-5.602,0-10.145,4.542-10.145,10.145v72.797c0,5.603,4.542,10.145,10.145,10.145\
+		c5.602,0,10.144-4.542,10.144-10.145v-72.797C194.931,106.153,190.389,101.611,184.787,101.611z"
+    ),
+)
+
+mail_icon = Icons(
+    version="1.1",
+    id="Capa_1",
+    xmlns="http://www.w3.org/2000/svg",
+    xmlns_xlink="http://www.w3.org/1999/xlink",
+    x="0px",
+    y="0px",
+    viewBox="0 0 474 474",
+    style="enable-background:new 0 0 474 474;",
+    xml_space="preserve",
+)
+mail_icon.add(
+    mail_icon.svg_tags.path(
+        d="M437.5,59.3h-401C16.4,59.3,0,75.7,0,95.8v282.4c0,20.1,16.4,36.5,36.5,36.5h401c20.1,0,36.5-16.4,36.5-36.5V95.8\
 		C474,75.7,457.6,59.3,437.5,59.3z M432.2,86.3L239.5,251.1L46.8,86.3H432.2z M447,378.2c0,5.2-4.3,9.5-9.5,9.5h-401\
 		c-5.2,0-9.5-4.3-9.5-9.5V104.9l203.7,174.2c0.1,0.1,0.3,0.2,0.4,0.3c0.1,0.1,0.3,0.2,0.4,0.3c0.3,0.2,0.5,0.4,0.8,0.5\
 		c0.1,0.1,0.2,0.1,0.3,0.2c0.4,0.2,0.8,0.4,1.2,0.6c0.1,0,0.2,0.1,0.3,0.1c0.3,0.1,0.6,0.3,1,0.4c0.1,0,0.3,0.1,0.4,0.1\
 		c0.3,0.1,0.6,0.2,0.9,0.2c0.1,0,0.3,0.1,0.4,0.1c0.3,0.1,0.7,0.1,1,0.2c0.1,0,0.2,0,0.3,0c0.4,0,0.9,0.1,1.3,0.1l0,0l0,0\
 		c0.4,0,0.9,0,1.3-0.1c0.1,0,0.2,0,0.3,0c0.3,0,0.7-0.1,1-0.2c0.1,0,0.3-0.1,0.4-0.1c0.3-0.1,0.6-0.2,0.9-0.2c0.1,0,0.3-0.1,0.4-0.1\
 		c0.3-0.1,0.6-0.2,1-0.4c0.1,0,0.2-0.1,0.3-0.1c0.4-0.2,0.8-0.4,1.2-0.6c0.1-0.1,0.2-0.1,0.3-0.2c0.3-0.2,0.5-0.3,0.8-0.5\
-		c0.1-0.1,0.3-0.2,0.4-0.3c0.1-0.1,0.3-0.2,0.4-0.3L447,109.2V378.2z")
-              )
+		c0.1-0.1,0.3-0.2,0.4-0.3c0.1-0.1,0.3-0.2,0.4-0.3L447,109.2V378.2z"
+    )
+)
 
-profile_icon = Icons(version="1.1",
-                     id="Layer_1",
-                     xmlns="http://www.w3.org/2000/svg",
-                     xmlns_xlink="http://www.w3.org/1999/xlink",
-                     x="0px",
-                     y="0px",
-                     viewBox="0 0 326.343 326.343",
-                     style="enable-background:new 0 0 326.343 326.343;",
-                     xml_space="preserve")
-profile_icon.add(profile_icon.svg_tags.path(d="M271.535,274.603c-0.892-16.852-33.704-30.088-50.568-35.796c-0.34-3.304-0.904-6.876-3.096-9.2\
+profile_icon = Icons(
+    version="1.1",
+    id="Layer_1",
+    xmlns="http://www.w3.org/2000/svg",
+    xmlns_xlink="http://www.w3.org/1999/xlink",
+    x="0px",
+    y="0px",
+    viewBox="0 0 326.343 326.343",
+    style="enable-background:new 0 0 326.343 326.343;",
+    xml_space="preserve",
+)
+profile_icon.add(
+    profile_icon.svg_tags.path(
+        d="M271.535,274.603c-0.892-16.852-33.704-30.088-50.568-35.796c-0.34-3.304-0.904-6.876-3.096-9.2\
 				c-2.34-2.512-6.116-3.404-9.564-3.928c-2.396-5.044-7.608-7.616-13.16-6.32c-0.66-3.208-1.596-11.172-2.096-11.7\
 				c17.416-11.932,33.872-33.28,41.08-59.964c5.088,3.032,10.84,4.276,16.22,0.168c6.592-5.032,6.776-15.432,4.448-22.7\
 				c-1.644-5.156-5.452-10.172-10.592-12.028c11.372-34.664-0.38-69.328-6.7-75.2c-6.044-5.604-13.98-5.124-20.364-3.5\
 				c0-0.004,0.004-0.004,0.004-0.012c1.564-2.836,3.12-5.676,3.784-7.08c0.6-1.268,0.284-2.788-0.78-3.7\
 				c-4.692-4.072-11.88-3.032-18.16-0.796c1.34-2.256,2.192-3.004,2.724-3.144c0.944-0.196,1.748-0.812,2.176-1.6\
 				c0.428-0.86,0.436-1.876,0.024-2.744c-8.64-18.12-30.612-15.572-42.42-14.208c-18.456,2.14-36.268,10.828-50.428,24.5\
 				c-2.14-1.132-4.572-1.62-7.152-1.412c-4.428,0.348-8.92,2.772-12.028,6.488c-4.868,5.824-6.8,13.676-8.164,21.2\
@@ -345,216 +399,278 @@
 				c-0.58,1.2-1.184,2.444-1.54,3.844c-0.396,1.564-0.34,2.964,0.16,4.16c1.068,2.556,3.516,3.308,5.488,3.9\
 				c1.076,0.328,2.092,0.644,2.684,1.152c0.808,0.696,1.124,2.02,1.492,3.556c0.436,1.812,0.928,3.864,2.448,5.4\
 				c0.432,0.464,1.02,0.696,1.612,0.696c0.544,0,1.084-0.196,1.512-0.6c0.892-0.836,0.936-2.232,0.1-3.1\
 				c-0.72-0.76-1.036-2.084-1.372-3.484c-0.476-1.996-1.02-4.252-2.912-5.884c-1.292-1.108-2.872-1.592-4.268-2.\
 				c-1.516-0.468-2.456-0.792-2.704-1.392c-0.068-0.168-0.156-0.568,0.048-1.372c0.244-0.96,0.724-1.948,1.232-2.9\
 				c0.904-1.864,1.932-3.984,1.776-6.456c-0.168-2.76-1.88-5.476-4.692-7.44c-1.974-1.387-4.02-2.496-5.99-2.8\
 				c15.008-1.644,31.65-5.517,40.358-18.854c1.528,0.452,5.852,1.996,6.464,2.032c20.536,6.888,46.456,19.224,47.044,30.\
-				c0.828,15.728,1.984,37.044,2.424,45.14H163.896z"),
-			profile_icon.svg_tags.path(d="M109.32,37.083c-8.804,1.036-11.664,13.252-12.08,20.568c-0.16,2.848,4.256,2.84,4.42,0.004\
-				c0.164-2.916,0.684-5.724,1.704-8.472c0.924-2.484,2.828-7.308,5.956-7.68C112.112,41.175,112.144,36.751,109.32,37.083z"),
-			profile_icon.svg_tags.path(d="M237.456,95.423c0.252-3.768,0.564-7.556,0.612-11.336c0.036-2.844-4.388-2.848-4.424,0\
-				c-0.048,3.776-0.356,7.568-0.612,11.336C232.844,98.263,237.268,98.251,237.456,95.423z"),
-			profile_icon.svg_tags.path(d="M180.86,69.347c1.924,0.768,3.872,1.432,5.868,1.988c2.744,0.764,3.916-3.5,1.176-4.264\
-				c-1.996-0.556-3.944-1.22-5.868-1.988C179.396,64.031,178.248,68.303,180.86,69.347z"),
-			profile_icon.svg_tags.path(d="M172.088,64.995c2.44,1.476,4.664-2.348,2.232-3.816c-7.204-4.356-13.66-9.708-20.06-15.144\
-				c-2.156-1.832-5.296,1.28-3.124,3.124C157.82,54.835,164.568,60.443,172.088,64.995z")
-		)
-
-
-password_icon = Icons(xmlns="http://www.w3.org/2000/svg", viewBox="0 0 20 20", fill="currentColor")
-password_icon.add(password_icon.svg_tags.path(fill_rule="evenodd",
-                                         d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2"
-                                         " 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 "
-                                         "0 012-2zm8-2v2H7V7a3 3 0 016 0z",
-                                         clip_rule="evenodd"))
-
-close_icon = Icons(xmlns="http://www.w3.org/2000/svg",
-                   height="24",
-                   viewBox="0 0 24 24",
-                   width="24",
-                   fill="currentColor")
-close_icon.add(close_icon.svg_tags.path(d="M0 0h24v24H0z", fill="none"),
-               close_icon.svg_tags.path(d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 "
-                                     "19 12 13.41 17.59 19 19 17.59 13.41 12z"))
+				c0.828,15.728,1.984,37.044,2.424,45.14H163.896z"
+    ),
+    profile_icon.svg_tags.path(
+        d="M109.32,37.083c-8.804,1.036-11.664,13.252-12.08,20.568c-0.16,2.848,4.256,2.84,4.42,0.004\
+				c0.164-2.916,0.684-5.724,1.704-8.472c0.924-2.484,2.828-7.308,5.956-7.68C112.112,41.175,112.144,36.751,109.32,37.083z"
+    ),
+    profile_icon.svg_tags.path(
+        d="M237.456,95.423c0.252-3.768,0.564-7.556,0.612-11.336c0.036-2.844-4.388-2.848-4.424,0\
+				c-0.048,3.776-0.356,7.568-0.612,11.336C232.844,98.263,237.268,98.251,237.456,95.423z"
+    ),
+    profile_icon.svg_tags.path(
+        d="M180.86,69.347c1.924,0.768,3.872,1.432,5.868,1.988c2.744,0.764,3.916-3.5,1.176-4.264\
+				c-1.996-0.556-3.944-1.22-5.868-1.988C179.396,64.031,178.248,68.303,180.86,69.347z"
+    ),
+    profile_icon.svg_tags.path(
+        d="M172.088,64.995c2.44,1.476,4.664-2.348,2.232-3.816c-7.204-4.356-13.66-9.708-20.06-15.144\
+				c-2.156-1.832-5.296,1.28-3.124,3.124C157.82,54.835,164.568,60.443,172.088,64.995z"
+    ),
+)
+
+
+password_icon = Icons(
+    xmlns="http://www.w3.org/2000/svg", viewBox="0 0 20 20", fill="currentColor"
+)
+password_icon.add(
+    password_icon.svg_tags.path(
+        fill_rule="evenodd",
+        d="M5 9V7a5 5 0 0110 0v2a2 2 0 012 2v5a2 2"
+        " 0 01-2 2H5a2 2 0 01-2-2v-5a2 2 "
+        "0 012-2zm8-2v2H7V7a3 3 0 016 0z",
+        clip_rule="evenodd",
+    )
+)
+
+close_icon = Icons(
+    xmlns="http://www.w3.org/2000/svg",
+    height="24",
+    viewBox="0 0 24 24",
+    width="24",
+    fill="currentColor",
+)
+close_icon.add(
+    close_icon.svg_tags.path(d="M0 0h24v24H0z", fill="none"),
+    close_icon.svg_tags.path(
+        d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 "
+        "19 12 13.41 17.59 19 19 17.59 13.41 12z"
+    ),
+)
 
-tooltip_icon = Icons(focusable="false", xmlns="http://www.w3.org/2000/svg", viewBox="0 0 16 16")
+tooltip_icon = Icons(
+    focusable="false", xmlns="http://www.w3.org/2000/svg", viewBox="0 0 16 16"
+)
 tooltip_icon.add(
     tooltip_icon.svg_tags.path(d="M0 0h16v16h-16z", fill="none"),
-    tooltip_icon.svg_tags.path(d="M8 1a7 7 0 1 0 7 7 7 7 0 0 0-7-7zm1 10a1 1 0 0 1-2 0v-3a1 1 0 0 1 2 "
-                            "0zm-.293-5.293a1 1 0 1 1 .293-.707 1 1 0 0 1-.293.707z",
-                          fill="#767676"))
-
-
-drag_and_drop_icon = Icons(focusable="false", xmlns="http://www.w3.org/2000/svg", viewBox="0 0 16 16",
-                           enable_background="new 0 0 16 16")
-drag_and_drop_icon.add(drag_and_drop_icon.svg_tags.g(
-    drag_and_drop_icon.svg_tags.path(d="M2.25 "
-    "0h-1.25c-.263 0-.521.107-.707.293-.186.186-.293.444-.293.707v1.25c0 "
-    ".552.448 1 1 1s1-.448 1-1v-.25h.25c.552 0 1-.448 1-1s-.448-1-1-1zM1 "
-    "8.75c.552 0 1-.448 1-1v-1.5c0-.552-.448-1-1-1s-1 .448-1 1v1.5c0 "
-    ".552.448 1 1 1zM2.25 12h-.25v-.25c0-.552-.448-1-1-1s-1 .448-1 "
-    "1v1.25c0 .263.107.521.293.707s.444.293.707.293h1.25c.552 0 1-.448 "
-    "1-1s-.448-1-1-1zM11.75 2h.25v.25c0 .552.448 1 1 1s1-.448 "
-    "1-1v-1.25c0-.263-.107-.521-.293-.707-.186-.186-.444-.293-.707-.293h-1.25c-.552 0-1 "
-    ".448-1 1s.448 1 1 1zM6.25 2h1.5c.552 0 1-.448 "
-    "1-1s-.448-1-1-1h-1.5c-.552 0-1 .448-1 1s.448 1 1 1zM14.5 "
-    "7h-.5v-.75c0-.552-.448-1-1-1s-1 .448-1 1v.75h-3.5c-.828 "
-    "0-1.5.671-1.5 1.5v3.5h-.75c-.552 0-1 .448-1 1s.448 1 1 "
-    "1h.75v.5c0 .828.672 1.5 1.5 1.5h6c.828 0 1.5-.672 1.5-1.5v-6c0-.829-.672-1.5-1.5-1.5z"),
-    fill="#00809D"), drag_and_drop_icon.svg_tags.path(fill="none", d="M0 0h16v16h-16z"))
-
-
-eyes_icon = Icons(xmlns="http://www.w3.org/2000/svg",
-                  xmlns_xlink="http://www.w3.org/1999/xlink",
-                  aria_hidden="true",
-                  focusable="false",
-                  width="1em",
-                  height="1em",
-                  style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);",
-                  preserveAspectRatio="xMidYMid meet",
-                  viewBox="0 0 16 16",
-                  fill="currentColor",
-                  stroke="currentColor")
-eyes_icon.add(eyes_icon.svg_tags.g(eyes_icon.svg_tags.path(d="M16 8s-3-5.5-8-5.5S0 8 0 8s3 5.5 8 5.5S16 8 16 8zM1.173 8a13.133 "
-                                                 "13.133 0 0 1 1.66-2.043C4.12 4.668 5.88 3.5 8 3.5c2.12 0 3.879 1.168 "
-                                                 "5.168 2.457A13.133 13.133 0 0 1 14.828"
-                                                 " 8c-.058.087-.122.183-.195.288c-.335.48-.83 1.12-1.465 1.755C11.879 "
-                                                 "11.332 10.119 12.5 8 12.5c-2.12 0-3.879-1.168-5.168-2.457A13.134 "
-                                                 "13.134 0 0 1 1.172 8z"),
-                              eyes_icon.svg_tags.path(d="M8 5.5a2.5 2.5 0 1 0 0 5a2.5 2.5 0 0 0 0-5zM4.5 8a3.5 3.5 0 1 1 7"
-                                                   " 0a3.5 3.5 0 0 1-7 0z"),
-                              ))
-
-eyes_splash_icon = Icons(xmlns="http://www.w3.org/2000/svg",
-                         xmlns_xlink="http://www.w3.org/1999/xlink",
-                         aria_hidden="true",
-                         focusable="false",
-                         width="1em",
-                         height="1em",
-                         style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); "
-                               "transform: rotate(360deg);" ,
-                         preserveAspectRatio="xMidYMid meet",
-                         viewBox="0 0 16 16",
-                         fill="currentColor",
-                         stroke="currentColor")
-eyes_splash_icon.add(eyes_splash_icon.svg_tags.g(
-    eyes_splash_icon.svg_tags.path(d="M13.359 11.238C15.06 9.72 16 8 16 8s-3-5.5-8-5.5a7.028 7.028 0 0 "
-                                "0-2.79.588l.77.771A5.944 5.944 0 0 1 8 3.5c2.12 0 3.879 1.168 5.168 "
-                                "2.457A13.134 13.134 0 0 1 14.828 8c-.058.087-.122.183-.195.288c-.335.48-.83 "
-                                "1.12-1.465 1.755c-.165.165-.337.328-.517.486l.708.709z"),
-    eyes_splash_icon.svg_tags.path(d="M11.297 9.176a3.5 3.5 0 0 0-4.474-4.474l.823.823a2.5 2.5 0 0 1 2.829 "
-                                "2.829l.822.822zm-2.943 1.299l.822.822a3.5 3.5 0 0 1-4.474-4.474l.823.823a2.5 "
-                                "2.5 0 0 0 2.829 2.829z"),
-    eyes_splash_icon.svg_tags.path(d="M3.35 5.47c-.18.16-.353.322-.518.487A13.134 13.134 0 0 0 1.172 "
-                                "8l.195.288c.335.48.83 1.12 1.465 1.755C4.121 11.332 5.881 12.5 8 12.5c.716 0 "
-                                "1.39-.133 2.02-.36l.77.772A7.029 7.029 0 0 1 8 13.5C3 13.5 0 8 0 8s.939-1.721 "
-                                "2.641-3.238l.708.709zm10.296 8.884l-12-12l.708-.708l12 12l-.708.708z"),
-    ))
-
-new_icon = Icons(xmlns="http://www.w3.org/2000/svg",
-                 xmlns_xlink="http://www.w3.org/1999/xlink",
-                 aria_hidden="true",
-                 focusable="false",
-                 width="1em",
-                 height="1em",
-                 style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);",
-                 preserveAspectRatio="xMidYMid meet",
-                 viewBox="0 0 100 100")
-new_icon.add(new_icon.svg_tags.path(d="M88.558 "
-                                 "49.96c0-.885-.435-1.663-1.097-2.151l.014-.024l-9.324-5.383l5.367-9.296l-.018-.011a2.666 "
-                                 "2.666 0 0 0-.127-2.408a2.667 2.667 "
-                                 "0 0 0-2.025-1.314v-.026H70.58V18.61h-.022a2.667 2.667 0 0 0-1.314-2.022a2.662 2.662 "
-                                 "0 0 0-2.412-.125l-.013-.023l-9.481 5.474l-5.25-9.094l-.019.011a2.668 2.668 "
-                                 "0 0 0-2.149-1.094c-.885 0-1.664.435-2.151 1.097l-.024-.014l-5.337 9.244l-9.19-5.306l-.011.019a2.666 "
-                                 "2.666 0 0 0-2.408.127a2.666 2.666 0 0 0-1.315 2.025h-.027v10.674H18.845v.021a2.667 2.667 "
-                                 "0 0 0-2.022 1.314a2.667 2.667 0 0 0-.126 2.41l-.023.014l5.246 9.087l-9.394 5.424l.011.019a2.668 "
-                                 "2.668 0 0 0-1.094 2.149c0 .885.435 1.664 1.097 2.151l-.014.024l9.324 5.383l-5.367 "
-                                 "9.296l.018.01a2.666 2.666 0 0 0 .127 2.408a2.667 2.667 0 "
-                                 "0 0 2.025 1.314v.027H29.42V81.39h.022c.092.816.549 1.58 1.314 2.022a2.665 2.665 0 "
-                                 "0 0 2.412.125l.013.023l9.481-5.474l5.25 9.094l.019-.011a2.668 2.668 0 "
-                                 "0 0 2.149 1.094c.885 0 1.664-.435 2.151-1.096l.023.013l5.337-9.244l9.191 "
-                                 "5.306l.011-.019a2.666 2.666 0 0 0 2.408-.127a2.666 2.666 0 "
-                                 "0 0 1.315-2.025h.027V70.398h10.613v-.021a2.667 2.667 0 0 0 2.022-1.314a2.67 2.67 0 "
-                                 "0 0 .126-2.411l.023-.013l-5.246-9.087l9.394-5.424l-.011-.019a2.666 2.666 0 "
-                                 "0 0 1.094-2.149zM43.715 61.355l-9.846-4.35l4.345 7.525l-2.456 "
-                                 "1.418l-6.662-11.537l2.525-1.459l9.53 4.162l-4.185-7.248l2.457-1.418l6.66 "
-                                 "11.537l-2.368 1.37zm4.652-2.686l-6.661-11.538l8.165-4.713l1.248 2.162l-5.709 "
-                                 "3.295l1.398 2.422l5.587-3.225l1.248 2.16l-5.587 3.227l1.518 2.629l5.709-3.295l1.248 "
-                                 "2.162l-8.164 4.714zm18.906-10.915L60.675 41l2.567 9.08l-2.611 "
-                                 "1.508l-9.965-9.629l2.75-1.588l6.838 7.168l-2.617-9.605l1.92-1.108l6.993 "
-                                 "7.079l-2.79-9.506l2.75-1.588l3.375 13.436l-2.612 1.507z", fill="#626262"))
-
-
-class MaterialDesignIcons(HTMLElement):
-
-    def __render__(self, *args, **kwargs):
-        return self.html_tags.i(*args, **kwargs)
-
-
-MDI = MaterialDesignIcons(cls="small material-icons")
-
-search_icon = MaterialDesignIcons("search", cls="small material-icons")
-manage_icon = MaterialDesignIcons("edit", cls="small material-icons")
-save_icon = MaterialDesignIcons("class", cls="small material-icons")
-delete_icon = MaterialDesignIcons("delete", cls="small material-icons")
-upload_icon = MaterialDesignIcons("file_upload", cls="small material-icons")
-track_icon = MaterialDesignIcons("track_changes", cls="small material-icons")
-bread_crumb_icon = MaterialDesignIcons("chevron_right", cls="small material-icons")
-bread_crumb_left_icon = MaterialDesignIcons("chevron_left", cls="small material-icons")
-close_md_icon = MaterialDesignIcons("chevron_left", cls="small material-icons")
-
-
-class Iconify(HTMLElement):
-    def __render__(self, *args, **kwargs):
-        return self.html_tags.span(*args, **kwargs)
-
-
-rupees_icon = Iconify(cls="iconify", data_icon="healthicons:rupee", data_inline="false")
-detail_icon = Iconify(cls="iconify", data_icon="bx:bx-detail", data_inline="false")
-more_icon = Iconify(cls="iconify", data_icon="gg:details-more", data_inline="false")
-discount_icon = Iconify(cls="iconify", data_icon="bx:bxs-discount", data_inline="false")
-counter_icon = Iconify(cls="iconify", data_icon="mdi:counter", data_inline="false")
-heart_icon = Iconify(cls="iconify", data_icon="bi:suit-heart")
-heart_filled_icon = Iconify(cls="iconify", data_icon="bi:suit-heart-fill")
-up_icon = Iconify(cls="iconify", data_icon="akar-icons:chevron-up")
-down_icon = Iconify(cls="iconify", data_icon="akar-icons:chevron-down")
-password2_icon = Iconify(cls="iconify", data_icon="carbon:password")
-mail2_icon = Iconify(cls="iconify", data_icon="fluent:mail-20-regular")
-changes_icon = Iconify(cls="iconify", data_icon="ant-design:line-chart-outlined")
-follow_icon = Iconify(cls="iconify", data_icon="ri:user-follow-line")
-unfollow_icon = Iconify(cls="iconify", data_icon="ri:user-unfollow-line")
-user_following_icon = Iconify(cls="iconify", data_icon="simple-line-icons:user-following")
-user_follow_icon = Iconify(cls="iconify", data_icon="simple-line-icons:user-follow")
-plus_icon = Iconify(cls="iconify", data_icon="bi:plus-circle")
-tick_icon = Iconify(cls="iconify", data_icon="teenyicons:tick-circle-outline")
-verified_icon = Iconify(cls="iconify", data_icon="ic:round-verified")
-coin_icon = Iconify(cls="iconify", data_icon="system-uicons:coins")
-coin_icon2 = raw('''
+    tooltip_icon.svg_tags.path(
+        d="M8 1a7 7 0 1 0 7 7 7 7 0 0 0-7-7zm1 10a1 1 0 0 1-2 0v-3a1 1 0 0 1 2 "
+        "0zm-.293-5.293a1 1 0 1 1 .293-.707 1 1 0 0 1-.293.707z",
+        fill="#767676",
+    ),
+)
+
+
+drag_and_drop_icon = Icons(
+    focusable="false",
+    xmlns="http://www.w3.org/2000/svg",
+    viewBox="0 0 16 16",
+    enable_background="new 0 0 16 16",
+)
+drag_and_drop_icon.add(
+    drag_and_drop_icon.svg_tags.g(
+        drag_and_drop_icon.svg_tags.path(
+            d="M2.25 "
+            "0h-1.25c-.263 0-.521.107-.707.293-.186.186-.293.444-.293.707v1.25c0 "
+            ".552.448 1 1 1s1-.448 1-1v-.25h.25c.552 0 1-.448 1-1s-.448-1-1-1zM1 "
+            "8.75c.552 0 1-.448 1-1v-1.5c0-.552-.448-1-1-1s-1 .448-1 1v1.5c0 "
+            ".552.448 1 1 1zM2.25 12h-.25v-.25c0-.552-.448-1-1-1s-1 .448-1 "
+            "1v1.25c0 .263.107.521.293.707s.444.293.707.293h1.25c.552 0 1-.448 "
+            "1-1s-.448-1-1-1zM11.75 2h.25v.25c0 .552.448 1 1 1s1-.448 "
+            "1-1v-1.25c0-.263-.107-.521-.293-.707-.186-.186-.444-.293-.707-.293h-1.25c-.552 0-1 "
+            ".448-1 1s.448 1 1 1zM6.25 2h1.5c.552 0 1-.448 "
+            "1-1s-.448-1-1-1h-1.5c-.552 0-1 .448-1 1s.448 1 1 1zM14.5 "
+            "7h-.5v-.75c0-.552-.448-1-1-1s-1 .448-1 1v.75h-3.5c-.828 "
+            "0-1.5.671-1.5 1.5v3.5h-.75c-.552 0-1 .448-1 1s.448 1 1 "
+            "1h.75v.5c0 .828.672 1.5 1.5 1.5h6c.828 0 1.5-.672 1.5-1.5v-6c0-.829-.672-1.5-1.5-1.5z"
+        ),
+        fill="#00809D",
+    ),
+    drag_and_drop_icon.svg_tags.path(fill="none", d="M0 0h16v16h-16z"),
+)
+
+
+eyes_icon = Icons(
+    xmlns="http://www.w3.org/2000/svg",
+    xmlns_xlink="http://www.w3.org/1999/xlink",
+    aria_hidden="true",
+    focusable="false",
+    width="1em",
+    height="1em",
+    style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);",
+    preserveAspectRatio="xMidYMid meet",
+    viewBox="0 0 16 16",
+    fill="currentColor",
+    stroke="currentColor",
+)
+eyes_icon.add(
+    eyes_icon.svg_tags.g(
+        eyes_icon.svg_tags.path(
+            d="M16 8s-3-5.5-8-5.5S0 8 0 8s3 5.5 8 5.5S16 8 16 8zM1.173 8a13.133 "
+            "13.133 0 0 1 1.66-2.043C4.12 4.668 5.88 3.5 8 3.5c2.12 0 3.879 1.168 "
+            "5.168 2.457A13.133 13.133 0 0 1 14.828"
+            " 8c-.058.087-.122.183-.195.288c-.335.48-.83 1.12-1.465 1.755C11.879 "
+            "11.332 10.119 12.5 8 12.5c-2.12 0-3.879-1.168-5.168-2.457A13.134 "
+            "13.134 0 0 1 1.172 8z"
+        ),
+        eyes_icon.svg_tags.path(
+            d="M8 5.5a2.5 2.5 0 1 0 0 5a2.5 2.5 0 0 0 0-5zM4.5 8a3.5 3.5 0 1 1 7"
+            " 0a3.5 3.5 0 0 1-7 0z"
+        ),
+    )
+)
+
+eyes_splash_icon = Icons(
+    xmlns="http://www.w3.org/2000/svg",
+    xmlns_xlink="http://www.w3.org/1999/xlink",
+    aria_hidden="true",
+    focusable="false",
+    width="1em",
+    height="1em",
+    style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); "
+    "transform: rotate(360deg);",
+    preserveAspectRatio="xMidYMid meet",
+    viewBox="0 0 16 16",
+    fill="currentColor",
+    stroke="currentColor",
+)
+eyes_splash_icon.add(
+    eyes_splash_icon.svg_tags.g(
+        eyes_splash_icon.svg_tags.path(
+            d="M13.359 11.238C15.06 9.72 16 8 16 8s-3-5.5-8-5.5a7.028 7.028 0 0 "
+            "0-2.79.588l.77.771A5.944 5.944 0 0 1 8 3.5c2.12 0 3.879 1.168 5.168 "
+            "2.457A13.134 13.134 0 0 1 14.828 8c-.058.087-.122.183-.195.288c-.335.48-.83 "
+            "1.12-1.465 1.755c-.165.165-.337.328-.517.486l.708.709z"
+        ),
+        eyes_splash_icon.svg_tags.path(
+            d="M11.297 9.176a3.5 3.5 0 0 0-4.474-4.474l.823.823a2.5 2.5 0 0 1 2.829 "
+            "2.829l.822.822zm-2.943 1.299l.822.822a3.5 3.5 0 0 1-4.474-4.474l.823.823a2.5 "
+            "2.5 0 0 0 2.829 2.829z"
+        ),
+        eyes_splash_icon.svg_tags.path(
+            d="M3.35 5.47c-.18.16-.353.322-.518.487A13.134 13.134 0 0 0 1.172 "
+            "8l.195.288c.335.48.83 1.12 1.465 1.755C4.121 11.332 5.881 12.5 8 12.5c.716 0 "
+            "1.39-.133 2.02-.36l.77.772A7.029 7.029 0 0 1 8 13.5C3 13.5 0 8 0 8s.939-1.721 "
+            "2.641-3.238l.708.709zm10.296 8.884l-12-12l.708-.708l12 12l-.708.708z"
+        ),
+    )
+)
+
+new_icon = Icons(
+    xmlns="http://www.w3.org/2000/svg",
+    xmlns_xlink="http://www.w3.org/1999/xlink",
+    aria_hidden="true",
+    focusable="false",
+    width="1em",
+    height="1em",
+    style="-ms-transform: rotate(360deg); -webkit-transform: rotate(360deg); transform: rotate(360deg);",
+    preserveAspectRatio="xMidYMid meet",
+    viewBox="0 0 100 100",
+)
+new_icon.add(
+    new_icon.svg_tags.path(
+        d="M88.558 "
+        "49.96c0-.885-.435-1.663-1.097-2.151l.014-.024l-9.324-5.383l5.367-9.296l-.018-.011a2.666 "
+        "2.666 0 0 0-.127-2.408a2.667 2.667 "
+        "0 0 0-2.025-1.314v-.026H70.58V18.61h-.022a2.667 2.667 0 0 0-1.314-2.022a2.662 2.662 "
+        "0 0 0-2.412-.125l-.013-.023l-9.481 5.474l-5.25-9.094l-.019.011a2.668 2.668 "
+        "0 0 0-2.149-1.094c-.885 0-1.664.435-2.151 1.097l-.024-.014l-5.337 9.244l-9.19-5.306l-.011.019a2.666 "
+        "2.666 0 0 0-2.408.127a2.666 2.666 0 0 0-1.315 2.025h-.027v10.674H18.845v.021a2.667 2.667 "
+        "0 0 0-2.022 1.314a2.667 2.667 0 0 0-.126 2.41l-.023.014l5.246 9.087l-9.394 5.424l.011.019a2.668 "
+        "2.668 0 0 0-1.094 2.149c0 .885.435 1.664 1.097 2.151l-.014.024l9.324 5.383l-5.367 "
+        "9.296l.018.01a2.666 2.666 0 0 0 .127 2.408a2.667 2.667 0 "
+        "0 0 2.025 1.314v.027H29.42V81.39h.022c.092.816.549 1.58 1.314 2.022a2.665 2.665 0 "
+        "0 0 2.412.125l.013.023l9.481-5.474l5.25 9.094l.019-.011a2.668 2.668 0 "
+        "0 0 2.149 1.094c.885 0 1.664-.435 2.151-1.096l.023.013l5.337-9.244l9.191 "
+        "5.306l.011-.019a2.666 2.666 0 0 0 2.408-.127a2.666 2.666 0 "
+        "0 0 1.315-2.025h.027V70.398h10.613v-.021a2.667 2.667 0 0 0 2.022-1.314a2.67 2.67 0 "
+        "0 0 .126-2.411l.023-.013l-5.246-9.087l9.394-5.424l-.011-.019a2.666 2.666 0 "
+        "0 0 1.094-2.149zM43.715 61.355l-9.846-4.35l4.345 7.525l-2.456 "
+        "1.418l-6.662-11.537l2.525-1.459l9.53 4.162l-4.185-7.248l2.457-1.418l6.66 "
+        "11.537l-2.368 1.37zm4.652-2.686l-6.661-11.538l8.165-4.713l1.248 2.162l-5.709 "
+        "3.295l1.398 2.422l5.587-3.225l1.248 2.16l-5.587 3.227l1.518 2.629l5.709-3.295l1.248 "
+        "2.162l-8.164 4.714zm18.906-10.915L60.675 41l2.567 9.08l-2.611 "
+        "1.508l-9.965-9.629l2.75-1.588l6.838 7.168l-2.617-9.605l1.92-1.108l6.993 "
+        "7.079l-2.79-9.506l2.75-1.588l3.375 13.436l-2.612 1.507z",
+        fill="#626262",
+    )
+)
+
+
+i = Component.html_tags.i
+
+search_icon = i("search", className="small material-icons")
+manage_icon = i("edit", className="small material-icons")
+save_icon = i("class", className="small material-icons")
+delete_icon = i("delete", className="small material-icons")
+upload_icon = i("file_upload", className="small material-icons")
+track_icon = i("track_changes", className="small material-icons")
+bread_crumb_icon = i("chevron_right", className="small material-icons")
+bread_crumb_left_icon = i("chevron_left", className="small material-icons")
+close_md_icon = i("chevron_left", className="small material-icons")
+
+span = Component.html_tags.span
+
+rupees_icon = span(
+    className="iconify", data_icon="healthicons:rupee", data_inline="false"
+)
+detail_icon = span(className="iconify", data_icon="bx:bx-detail", data_inline="false")
+more_icon = span(className="iconify", data_icon="gg:details-more", data_inline="false")
+discount_icon = span(
+    className="iconify", data_icon="bx:bxs-discount", data_inline="false"
+)
+counter_icon = span(className="iconify", data_icon="mdi:counter", data_inline="false")
+heart_icon = span(className="iconify", data_icon="bi:suit-heart")
+heart_filled_icon = span(className="iconify", data_icon="bi:suit-heart-fill")
+up_icon = span(className="iconify", data_icon="akar-icons:chevron-up")
+down_icon = span(className="iconify", data_icon="akar-icons:chevron-down")
+password2_icon = span(className="iconify", data_icon="carbon:password")
+mail2_icon = span(className="iconify", data_icon="fluent:mail-20-regular")
+changes_icon = span(className="iconify", data_icon="ant-design:line-chart-outlined")
+follow_icon = span(className="iconify", data_icon="ri:user-follow-line")
+unfollow_icon = span(className="iconify", data_icon="ri:user-unfollow-line")
+user_following_icon = span(
+    className="iconify", data_icon="simple-line-icons:user-following"
+)
+user_follow_icon = span(className="iconify", data_icon="simple-line-icons:user-follow")
+plus_icon = span(className="iconify", data_icon="bi:plus-circle")
+tick_icon = span(className="iconify", data_icon="teenyicons:tick-circle-outline")
+verified_icon = span(className="iconify", data_icon="ic:round-verified")
+coin_icon = span(className="iconify", data_icon="system-uicons:coins")
+coin_icon2 = raw(
+    """
 <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-coin" viewBox="0 0 16 16">
   <path d="M5.5 9.511c.076.954.83 1.697 2.182 1.785V12h.6v-.709c1.4-.098 2.218-.846 2.218-1.932 
   0-.987-.626-1.496-1.745-1.76l-.473-.112V5.57c.6.068.982.396 1.074.85h1.052c-.076-.919-.864-1.638-2.126-1.716V4h-.6v.719c-1.195.117-2.01.836-2.01 
   1.853 0 .9.606 1.472 1.613 1.707l.397.098v2.034c-.615-.093-1.022-.43-1.114-.9H5.5zm2.177-2.166c-.59-.137-.91-.416-.91-.836 0-.47.345-.822.915-.925v1.76h-.005zm.692 
   1.193c.717.166 1.048.435 1.048.91 0 .542-.412.914-1.135.982V8.518l.087.02z"/>
   <path d="M8 15A7 7 0 1 1 8 1a7 7 0 0 1 0 14zm0 1A8 8 0 1 0 8 0a8 8 0 0 0 0 16z"/>
   <path d="M8 13.5a5.5 5.5 0 1 1 0-11 5.5 5.5 0 0 1 0 11zm0 .5A6 6 0 1 0 8 2a6 6 0 0 0 0 12z"/>
-</svg>''')
-menu_open_icon = Iconify(className="iconify", data_icon="heroicons-outline:menu")
-menu_open2_icon = Iconify(className="iconify", data_icon="line-md:menu")
-hero_list_icon = Iconify(className="iconify", data_icon="heroicons-solid:view-list")
-hero_x_icon = Iconify(className="iconify", data_icon="heroicons-solid:x")
-hero_add_to_cart_icon = Iconify(className="iconify", data_icon="bi:cart-plus-fill")
-hero_added_to_cart_icon = Iconify(className="iconify", data_icon="bi:cart-check-fill")
-hero_remove_from_cart_icon = Iconify(className="iconify", data_icon="bi:cart-dash-fill")
-hero_removed_from_cart_icon = Iconify(className="iconify", data_icon="bi:cart-x-fill")
-loading_icon = Iconify(className="iconify", data_icon="ant-design:loading-3-quarters-outlined")
-linkedin_icon = Iconify(className="iconify", data_icon="carbon:logo-linkedin")
-pinterest_icon = Iconify(className="iconify", data_icon="carbon:logo-pinterest")
-facebook_icon = Iconify(className="iconify", data_icon="carbon:logo-facebook")
-twitter_icon = Iconify(className="iconify", data_icon="carbon:logo-twitter")
-youtube_icon = Iconify(className="iconify", data_icon="carbon:logo-youtube")
-instagram_icon = Iconify(className="iconify", data_icon="carbon:logo-instagram")
-skype_icon = Iconify(className="iconify", data_icon="carbon:logo-skype")
-github_icon = Iconify(className="iconify", data_icon="carbon:logo-github")
-snapchat_icon = Iconify(className="iconify", data_icon="carbon:logo-snapchat")
-gmail_icon = Iconify(className="iconify", data_icon="mdi:gmail")
-google_icon = Iconify(className="iconify", data_icon="mdi:google")
+</svg>"""
+)
+menu_open_icon = span(className="iconify", data_icon="heroicons-outline:menu")
+menu_open2_icon = span(className="iconify", data_icon="line-md:menu")
+hero_list_icon = span(className="iconify", data_icon="heroicons-solid:view-list")
+hero_x_icon = span(className="iconify", data_icon="heroicons-solid:x")
+hero_add_to_cart_icon = span(className="iconify", data_icon="bi:cart-plus-fill")
+hero_added_to_cart_icon = span(className="iconify", data_icon="bi:cart-check-fill")
+hero_remove_from_cart_icon = span(className="iconify", data_icon="bi:cart-dash-fill")
+hero_removed_from_cart_icon = span(className="iconify", data_icon="bi:cart-x-fill")
+loading_icon = span(
+    className="iconify", data_icon="ant-design:loading-3-quarters-outlined"
+)
+linkedin_icon = span(className="iconify", data_icon="carbon:logo-linkedin")
+pinterest_icon = span(className="iconify", data_icon="carbon:logo-pinterest")
+facebook_icon = span(className="iconify", data_icon="carbon:logo-facebook")
+twitter_icon = span(className="iconify", data_icon="carbon:logo-twitter")
+youtube_icon = span(className="iconify", data_icon="carbon:logo-youtube")
+instagram_icon = span(className="iconify", data_icon="carbon:logo-instagram")
+skype_icon = span(className="iconify", data_icon="carbon:logo-skype")
+github_icon = span(className="iconify", data_icon="carbon:logo-github")
+snapchat_icon = span(className="iconify", data_icon="carbon:logo-snapchat")
+gmail_icon = span(className="iconify", data_icon="mdi:gmail")
+google_icon = span(className="iconify", data_icon="mdi:google")
```

### Comparing `uidom-0.1.1b6/uidom/dom/jinja.py` & `uidom-0.2a0/uidom/dom/jinja.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "JinjaComponent"
 ]
 
 
 class JinjaComponent(component.Component):
     file_extension = ".html"
 
-    def __render__(self, *args, **kwargs):
+    def render(self, *args, **kwargs):
         pass
 
     def __block__(self, block_name, *args):
         return self.jinja_tags.Block(block_name, *args)
 
     def __if__(self, if_condition, *if_args):
         return self.jinja_tags.If(if_condition, *if_args)
```

### Comparing `uidom-0.1.1b6/uidom/dom/links.py` & `uidom-0.2a0/uidom/examples/links.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,22 +11,22 @@
     "Link",
     "HtmxLink"
 ]
 
 
 class Link(HTMLElement):
 
-    def __render__(self, *args, item_link, item_name=None, **kwargs):
+    def render(self, *args, item_link, item_name=None, **kwargs):
         self.div = div() if item_name is None else div(item_name)
         return a(*args, self.div, href=item_link,  **kwargs)
 
 
 class HtmxLink(HTMLElement):
 
-    def __render__(self, *args, item_link, target_id, item_name=None, push_url=True, **kwargs):
+    def render(self, *args, item_link, target_id, item_name=None, push_url=True, **kwargs):
         self.text = div() if item_name is None else div(item_name)
         link = div(*args, self.text, hx_get=item_link, hx_trigger="click", hx_target=target_id,
                    className="cursor-pointer",
                    **kwargs)
         if push_url:
             link["hx-push-url"] = "true"
         return link
```

### Comparing `uidom-0.1.1b6/uidom/dom/src/csstags.py` & `uidom-0.2a0/uidom/dom/src/csstags.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 from uidom.dom.src.main import extension
 
-__all__ = [
-    "CSSClass",
-    "CSSId",
-    "CSS",
-    "CSSProperty"
-]
+__all__ = ["CSSClass", "CSSId", "CSS", "CSSProperty"]
 
 
 class CSS(extension.StyleTags):
     pass
 
 
 class CSSClass(extension.StyleTags):
@@ -25,63 +20,61 @@
 
 class CSSId(extension.StyleTags):
     is_id = True
     is_inline = True
 
 
 class CSSProperty(extension.StyleTags):
-
     def __set_name__(self, owner, name):
+        self.is_inline = getattr(owner, "is_inline", False)
         self._id = f"{owner.__name__}.{name}".replace(".", "-").replace("_", "-")
         self._class = name.replace("_", "-")
-        self._apply = f"{owner.__name__}::part({name})".replace("_", "-")
+        self._apply_part = f"{owner.__name__}::part({name})".replace("_", "-")
+        self._apply = f"{owner.__name__}".replace("_", "-")
 
         class Class(CSSClass):
             tagname = self._class
+            is_inline = self.is_inline
 
         class Id(CSSId):
             tagname = self._id.lower()
+            is_inline = self.is_inline
 
         class CSS(extension.StyleTags):
             tagname = name.replace("_", "-")
+            is_inline = self.is_inline
 
         class Apply(extension.StyleTags):
             tagname = self._apply.lower()
             is_apply = True
-            left_delimiter = "{@"
+            is_inline = self.is_inline
 
-        self.css_class = Class
-        self.css_id = Id
+        self.cls = Class
+        self.id = Id
         self.css = CSS
-        self.css_apply = Apply
+        self.apply = Apply
+
 
+if __name__ == "__main__":
 
-if __name__ == '__main__':
-    # from myst_parser import parse_html
+    class div(extension.Tags):
+        pass
 
-    class Order(object):
+    class Order(extension.Tags):
+        render_tag = False
         product_name = CSSProperty()
         product_category = CSSProperty()
         product_id = CSSProperty()
 
-
-    order = Order()
-    products = order.product_name.css_id(background_color='red', width="12%")
-    category = order.product_category.css_class(color="#23cfff")
-    csss = order.product_id.css_apply(apply="bg-rose-500")
-    id = order.product_id.css_id()
-
-
-    # ast = parse_html.tokenize_html(html(style(products, category)).render())
-    # print(list(ast.walk()))
-
-    class product(CSSClass):
-        pass
-
-
-    cs = products
-    # cs.attributes.update(padding="10px")
-    cs["boxsize"] = "border-box"
-    cs["background-color"] = "red"
-    print(cs)
+    order = Order(div("hello"))
+    prod_name = Order.product_name.id(background_color="red", width="12%")
+    category = Order.product_category.cls(color="#23cfff")
+    prod_id = Order.product_id.apply(apply="bg-rose-500 text-rose-400")
+    print(order)
+    # products.attributes.update(padding="10px")
+    prod_name["boxsize"] = "border-box"
+    prod_name["background-color"] = "red"
+    # print(prod_name)
+    # print(order.product_name.css(textdecoration="none"))
     print(category)
-    print(csss.render(pretty=False))
+    prod_id.add(prod_name)
+    print(prod_id)
```

### Comparing `uidom-0.1.1b6/uidom/dom/src/dom_tag.py` & `uidom-0.2a0/uidom/dom/src/dom_tag.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,55 +1,37 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
-__license__ = """
-This file is part of Dominate.
-
-Dominate is free software: you can redistribute it and/or modify
-it under the terms of the GNU Lesser General Public License as
-published by the Free Software Foundation, either version 3 of
-the License, or (at your option) any later version.
-
-Dominate is distributed in the hope that it will be useful, but
-WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU Lesser General Public License for more details.
-
-You should have received a copy of the GNU Lesser General
-Public License along with Dominate.  If not, see
-<http://www.gnu.org/licenses/>.
-"""
+import copy
 
 # pylint: disable=bad-indentation, bad-whitespace, missing-docstring
-
-import copy
 import numbers
 import threading
 import typing
 from collections import defaultdict, namedtuple
 from functools import wraps
 
 try:
     # Python 3
     from collections.abc import Callable
 except ImportError:
     # Python 2.7
-    from collections import Callable
+    from collections import Callable  # type: ignore
 
 try:
-    basestring = basestring
+    basestring = basestring  # type: ignore
 except NameError:  # py3
     basestring = str
     unicode = str
 
 try:
-    import greenlet
+    import greenlet  # type: ignore
 except ImportError:
     greenlet = None
 
 
 def _get_thread_context():
     context = [threading.current_thread()]
     if greenlet:
@@ -59,14 +41,15 @@
 
 class dom_tag(object):
     is_single = False  # Tag does not require matching end tag (ex. <hr/>)
     is_pretty = True  # Text inside the tag should be left as-is (ex. <pre>)
     # otherwise, text will be escaped() and whitespace may be
     # modified
     is_inline = False
+    escape_string = True
 
     def __new__(_cls, *args, **kwargs):
         """
         Check if bare tag is being used as a decorator
         (called with a single function arg).
         decorate the function and return
         """
@@ -101,55 +84,57 @@
         self.children = []
         self.parent = None
         self.document = None
 
         # Does not insert newlines on all children if True (recursive attribute)
         self.is_inline = kwargs.pop("__inline", self.is_inline)
         self.is_pretty = kwargs.pop("__pretty", self.is_pretty)
+        self.escape_string = kwargs.pop("__escape_string", self.escape_string)
 
         # Add child elements
         if args:
-            self.add(*args)
+            self.add(args)
 
         for attr, value in kwargs.items():
             self.set_attribute(*type(self).clean_pair(attr, value))
 
-        self._ctx = None
+        # this is where the this class instance is added to the parent context via _add_to_context
+        self._ctx: typing.Optional[dom_tag.frame] = None
         self._add_to_ctx()
 
     # context manager
     frame = namedtuple("frame", ["tag", "items", "used"])
     # stack of frames
     _with_contexts: typing.DefaultDict = defaultdict(list)
 
     def _add_to_ctx(self):
+        # here we are assuming that when the self is initialized it is
+        # under only single level of context and that the thread_context to which its
+        # child is added is same as that of self. But its not true in case we define
+        # render() methods in dom_tag subclasses in with multiple levels of context
+        # are present where a child can be added to subcontext
         stack = dom_tag._with_contexts.get(_get_thread_context())
         if stack:
             self._ctx = stack[-1]
             stack[-1].items.append(self)
 
     def __enter__(self):
         stack = dom_tag._with_contexts[_get_thread_context()]
         stack.append(dom_tag.frame(self, [], set()))
         return self
 
     def __exit__(self, type, value, traceback):
         thread_id = _get_thread_context()
         stack = dom_tag._with_contexts[thread_id]
         frame = stack.pop()
+
         for item in frame.items:
-            if not hasattr(item, "__render__"):
-                # deal with all the Tags but not Components
-                if item in frame.used:
-                    continue
-            else:
-                # deal with all the components here, as all components have ._entry attributes
-                # we can now check the membership of it
-                if item._entry in frame.used:
-                    continue
+            if item in frame.used:
+                continue
+            # if not hasattr(item, "_entry"):
             self.add(item)
         if not stack:
             del dom_tag._with_contexts[thread_id]
 
     def __call__(self, func):
         """
         tag instance is being used as a decorator.
@@ -197,50 +182,53 @@
         """
         Creates a reference to the parent document to allow for partial-tree
         validation.
         """
         # assume that a document is correct in the subtree
         if self.document != doc:
             self.document = doc
-            for i in self.children:
-                if not isinstance(i, dom_tag):
-                    return
-                i.setdocument(doc)
+            # we changed "for child in self.children" to "for child in self"
+            # because we want to implement custom __iter__ method that returns
+            # children that can refere any entry point in dom_tag subclasses
+            for child in self:
+                if not isinstance(child, dom_tag):
+                    continue
+                child.setdocument(doc)
 
     def add(self, *args):
         """
         Add new child tags.
         """
         for obj in args:
             if isinstance(obj, numbers.Number):
                 # Convert to string so we fall into next if block
                 obj = str(obj)
 
             if isinstance(obj, basestring):
-                obj = escape(obj)
+                # we are going to add the support for escaping only those strings whoes parents
+                # have explicit variable "escape_string" set to True
+                if hasattr(self, "escape_string"):
+                    if self.escape_string:
+                        obj = escape(obj)
+                else:
+                    obj = escape(obj)
                 self.children.append(obj)
 
             elif isinstance(obj, dom_tag):
                 stack = dom_tag._with_contexts.get(_get_thread_context())
                 if stack:
-                    if hasattr(obj, 'render_tag'):
-                        if obj.render_tag:
-                            stack[-1].used.add(obj)
-                        else:
-                            stack[-1].used.add(obj.children[0])
-                    else:
-                        stack[-1].used.add(obj)
-                        
+                    stack[-1].used.add(obj)
+
                 self.children.append(obj)
                 obj.parent = self
                 obj.setdocument(self.document)
 
             elif isinstance(obj, dict):
                 for attr, value in obj.items():
-                    self.set_attribute(*dom_tag.clean_pair(attr, value))
+                    self.set_attribute(*self.clean_pair(attr, value))
 
             elif hasattr(obj, "__iter__"):
                 for subobj in obj:
                     self.add(subobj)
 
             else:  # wtf is it?
                 raise ValueError(self.__class__, "%r not a tag or string." % obj)
@@ -267,31 +255,47 @@
         Recursively searches children for tags of a certain
         type with matching attributes.
         """
         # Stupid workaround since we can not use dom_tag in the method declaration
         if tag is None:
             tag = dom_tag
 
-        attrs = [
-            (self.clean_attribute(attr), value) for attr, value in kwargs.items()
-        ]
+        attrs = [(self.clean_attribute(attr), value) for attr, value in kwargs.items()]
 
         results = []
-        for child in self.children:
-            if (isinstance(tag, basestring) and type(child).__name__ == tag) or (
-                not isinstance(tag, basestring) and isinstance(child, tag)
-            ):
-
-                if all(
-                    child.attributes.get(attribute) == value
-                    for attribute, value in attrs
+        # the reason for changing from "for child in self.children" to "for child in self" below
+        # is that self already has __iter__ method and it iter over self.children, also when we
+        # subclass dom_tag its subclasses can implement different __iter__ method so we don't have
+        # to care for each implementations.
+
+        for child in self:
+            if isinstance(tag, (basestring, type)):
+                # tags here can be of any type (including basestring type), while
+                # child can be only string or dom_tag.
+                #
+                if (isinstance(tag, basestring) and type(child).__name__ == tag) or (
+                    not isinstance(tag, basestring) and isinstance(child, tag)
                 ):
-                    # If the child is of correct type and has all attributes and values
-                    # in kwargs add as a result
+                    if all(
+                        child.attributes.get(attribute) == value
+                        if value is not None
+                        else child.attributes.get(attribute)
+                        # this is to handle cases where we want to check mere
+                        # presence of attributes like x-data or x-component so
+                        # we use element.get(x_data=None) as a work around as
+                        # we aren't sure whats the actual value.
+                        for attribute, value in attrs
+                    ):
+                        # If the child is of correct type and has all attributes and values
+                        # in kwargs add as a result
+                        results.append(child)
+            elif isinstance(tag, dom_tag):
+                if child is tag:
                     results.append(child)
+
             if isinstance(child, dom_tag):
                 # If the child is a dom_tag extend the search down through its children
                 results.extend(child.get(tag, **kwargs))
         return results
 
     def __getitem__(self, key):
         """
@@ -348,33 +352,39 @@
     def __iadd__(self, obj):
         """
         Reflexive binary addition simply adds tag as a child.
         """
         self.add(obj)
         return self
 
-    # String and unicode representations are the same as render()
+    # String and unicode representations are the same as __render__()
     def __unicode__(self):
-        return self.render()
+        return self.__render__()
 
     __str__ = __unicode__
 
-    def render(self, indent="  ", pretty=True, xhtml=False):
-        data = self._render([], 0, indent, pretty, xhtml)
-        return u"".join(data)
+    def __render__(self, indent="  ", pretty=True, xhtml=False):
+        html_tokens = self._render([], 0, indent, pretty, xhtml)
+        return "".join(html_tokens)
+
+    async def __async_render__(self, indent="  ", pretty=True, xhtml=False):
+        for html_token in self._render([], 0, indent, pretty, xhtml):
+            yield html_token
 
     def _render(self, sb, indent_level, indent_str, pretty, xhtml):
         pretty = pretty and self.is_pretty
 
         name = getattr(self, "tagname", type(self).__name__)
 
         # Workaround for python keywords and standard classes/methods
         # (del, object, input)
         if name[-1] == "_":
             name = name[:-1]
+        if name[0] == "_":
+            name = name[1:]
 
         # open tag
         sb.append("<")
         sb.append(name)
 
         for attribute, value in sorted(self.attributes.items()):
             if value is not False:  # False values must be omitted completely
@@ -396,15 +406,15 @@
             sb.append(name)
             sb.append(">")
 
         return sb
 
     def _render_children(self, sb, indent_level, indent_str, pretty, xhtml):
         inline = True
-        for child in self.children:
+        for child in self:
             if isinstance(child, dom_tag):
                 if pretty and not child.is_inline:
                     inline = False
                     sb.append("\n")
                     sb.append(indent_str * indent_level)
                 child._render(sb, indent_level, indent_str, pretty, xhtml)
             else:
@@ -423,16 +433,16 @@
         children_len = len(self.children)
         children = "%s child" % children_len
         if children_len != 1:
             children += "ren"
 
         return "<%s at %x: %s, %s>" % (name, id(self), attributes, children)
 
-    @staticmethod
-    def clean_attribute(attribute):
+    @classmethod
+    def clean_attribute(cls, attribute):
         """
         Normalize attribute names for shorthand and work arounds for limitations
         in Python's syntax
         """
 
         # Shorthand
         attribute = {
```

### Comparing `uidom-0.1.1b6/uidom/dom/src/htmltags.py` & `uidom-0.2a0/uidom/dom/src/htmltags.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,132 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 from uidom.dom.src.dom_tag import dom_tag
 from uidom.dom.src.main import extension
 
 try:
     basestring = basestring
 except NameError:  # py3
     basestring = str
     unicode = str
 
-underscored_classes = set(['del', 'input', 'map', 'object'])
+underscored_classes = set(["del", "input", "map", "object"])
 
 # Tag attributes
-_ATTR_GLOBAL = set([
-    'accesskey', 'class', 'class', 'contenteditable', 'contextmenu', 'dir',
-    'draggable', 'id', 'item', 'hidden', 'lang', 'itemprop', 'spellcheck',
-    'style', 'subject', 'tabindex', 'title'
-])
-_ATTR_EVENTS = set([
-    'onabort', 'onblur', 'oncanplay', 'oncanplaythrough', 'onchange', 'onclick',
-    'oncontextmenu', 'ondblclick', 'ondrag', 'ondragend', 'ondragenter',
-    'ondragleave', 'ondragover', 'ondragstart', 'ondrop', 'ondurationchange',
-    'onemptied', 'onended', 'onerror', 'onfocus', 'onformchange', 'onforminput',
-    'oninput', 'oninvalid', 'onkeydown', 'onkeypress', 'onkeyup', 'onload',
-    'onloadeddata', 'onloadedmetadata', 'onloadstart', 'onmousedown',
-    'onmousemove', 'onmouseout', 'onmouseover', 'onmouseup', 'onmousewheel',
-    'onpause', 'onplay', 'onplaying', 'onprogress', 'onratechange',
-    'onreadystatechange', 'onscroll', 'onseeked', 'onseeking', 'onselect',
-    'onshow', 'onstalled', 'onsubmit', 'onsuspend', 'ontimeupdate',
-    'onvolumechange', 'onwaiting'
-])
-
-ERR_ATTRIBUTE = 'attributes'
-ERR_CONTEXT = 'context'
-ERR_CONTENT = 'content'
+_ATTR_GLOBAL = set(
+    [
+        "accesskey",
+        "class",
+        "class",
+        "contenteditable",
+        "contextmenu",
+        "dir",
+        "draggable",
+        "id",
+        "item",
+        "hidden",
+        "lang",
+        "itemprop",
+        "spellcheck",
+        "style",
+        "subject",
+        "tabindex",
+        "title",
+    ]
+)
+_ATTR_EVENTS = set(
+    [
+        "onabort",
+        "onblur",
+        "oncanplay",
+        "oncanplaythrough",
+        "onchange",
+        "onclick",
+        "oncontextmenu",
+        "ondblclick",
+        "ondrag",
+        "ondragend",
+        "ondragenter",
+        "ondragleave",
+        "ondragover",
+        "ondragstart",
+        "ondrop",
+        "ondurationchange",
+        "onemptied",
+        "onended",
+        "onerror",
+        "onfocus",
+        "onformchange",
+        "onforminput",
+        "oninput",
+        "oninvalid",
+        "onkeydown",
+        "onkeypress",
+        "onkeyup",
+        "onload",
+        "onloadeddata",
+        "onloadedmetadata",
+        "onloadstart",
+        "onmousedown",
+        "onmousemove",
+        "onmouseout",
+        "onmouseover",
+        "onmouseup",
+        "onmousewheel",
+        "onpause",
+        "onplay",
+        "onplaying",
+        "onprogress",
+        "onratechange",
+        "onreadystatechange",
+        "onscroll",
+        "onseeked",
+        "onseeking",
+        "onselect",
+        "onshow",
+        "onstalled",
+        "onsubmit",
+        "onsuspend",
+        "ontimeupdate",
+        "onvolumechange",
+        "onwaiting",
+    ]
+)
+
+ERR_ATTRIBUTE = "attributes"
+ERR_CONTEXT = "context"
+ERR_CONTENT = "content"
 
 
-class HtmlSingleTemplates(extension.SingleTemplates):
+class DocType(extension.SingleTemplates):
+    left_delimiter = "<!"
+    right_delimiter = ">"
     self_dedent = False
     child_dedent = True
     enable_left_delimiter_space = False
     enable_right_delimiter_space = False
 
-
-class HtmlDoubleTemplates(extension.DoubleTemplates):
-    # self_dedent = True
-    # child_dedent = True
-    enable_left_delimiter_space = True
-    enable_right_delimiter_space = True
-
-
-class HtmlSingleTags(extension.SingleTags):
-    pass
-
-
-class HtmlDoubleTags(extension.DoubleTags):
-    pass
-
-
-class DocType(HtmlSingleTemplates):
-    left_delimiter = "<!"
-    right_delimiter = ">"
-
     def __init__(self, template_text="html", *dom_elements):
         """
         :param template_text:
         :param dom_elements: [optional] template
         """
 
         super(DocType, self).__init__("DOCTYPE", template_text, *dom_elements)
 
 
 class html_tag(extension.Tags):
     def __init__(self, *args, **kwargs):
-        '''
+        """
         Creates a new html tag instance.
-        '''
+        """
         super(html_tag, self).__init__(*args, **kwargs)
 
     # def validate(self):
     #   '''
     #   Validate the tag. This will check the attributes, context, and contents and
     #   emit tuples in the form of: element, message.
     #   '''
@@ -125,18 +168,20 @@
 
 ################################################################################
 ############################### Html Tag Classes ###############################
 ################################################################################
 
 # Root element
 
+
 class html(html_tag):
-    '''
+    """
     The html element represents the root of an HTML document.
-    '''
+    """
+
     pass
     # def validate_attributes(self):
     #   errors = []
     #   for invalid in self._check_attributes(_ATTR_GLOBAL, 'manifest'):
     #     errors.append( (self, ERR_ATTRIBUTE, 'Invalid attribute: "%s"' % invalid) )
     #   return errors
 
@@ -149,1045 +194,1111 @@
     #   if len(self) != 2 or not isinstance(self[0], head) or not isinstance(self[1], body):
     #     return [(self, ERR_CONTENT, 'Children must be <head> and then <body>.')]
     #   return []
 
 
 # Document metadata
 class head(html_tag):
-    '''
+    """
     The head element represents a collection of metadata for the document.
-    '''
+    """
+
     pass
 
 
 class title(html_tag):
-    '''
+    """
     The title element represents the document's title or name. Authors should use
     titles that identify their documents even when they are used out of context,
     for example in a user's history or bookmarks, or in search results. The
     document's title is often different from its first heading, since the first
     heading does not have to stand alone when taken out of context.
-    '''
+    """
 
     def _get_text(self):
-        return u''.join(self.get(basestring))
+        return "".join(self.get(basestring))
 
     def _set_text(self, text):
         self.clear()
         self.add(text)
 
     text = property(_get_text, _set_text)
 
 
 class base(html_tag):
-    '''
+    """
     The base element allows authors to specify the document base URL for the
     purposes of resolving relative URLs, and the name of the default browsing
     context for the purposes of following hyperlinks. The element does not
     represent any content beyond this information.
-    '''
+    """
+
     is_single = True
 
 
 class link(html_tag):
-    '''
+    """
     The link element allows authors to link their document to other resources.
-    '''
+    """
+
     is_single = True
 
 
 class meta(html_tag):
-    '''
+    """
     The meta element represents various kinds of metadata that cannot be
     expressed using the title, base, link, style, and script elements.
-    '''
+    """
+
     is_single = True
 
 
 class style(html_tag):
-    '''
+    """
     The style element allows authors to embed style information in their
     documents. The style element is one of several inputs to the styling
     processing model. The element does not represent content for the user.
-    '''
+    """
+
     is_pretty = False
 
 
 # Scripting
 class script(html_tag):
-    '''
+    """
     The script element allows authors to include dynamic script and data blocks
     in their documents. The element does not represent content for the user.
-    '''
+    """
+
     is_pretty = True
 
 
 class noscript(html_tag):
-    '''
+    """
     The noscript element represents nothing if scripting is enabled, and
     represents its children if scripting is disabled. It is used to present
     different markup to user agents that support scripting and those that don't
     support scripting, by affecting how the document is parsed.
-    '''
+    """
+
     pass
 
 
 # Sections
 class body(html_tag):
-    '''
+    """
     The body element represents the main content of the document.
-    '''
+    """
+
     pass
 
 
 class main(html_tag):
-    '''
+    """
     The main content area of a document includes content that is unique to that
     document and excludes content that is repeated across a set of documents such
     as site navigation links, copyright information, site logos and banners and
     search forms (unless the document or application's main function is that of a
     search form).
-    '''
+    """
 
 
 class section(html_tag):
-    '''
+    """
     The section element represents a generic section of a document or
     application. A section, in this context, is a thematic grouping of content,
     typically with a heading.
-    '''
+    """
+
     pass
 
 
 class nav(html_tag):
-    '''
+    """
     The nav element represents a section of a page that links to other pages or
     to parts within the page: a section with navigation links.
-    '''
+    """
+
     pass
 
 
 class article(html_tag):
-    '''
+    """
     The article element represents a self-contained composition in a document,
     page, application, or site and that is, in principle, independently
     distributable or reusable, e.g. in syndication. This could be a forum post, a
     magazine or newspaper article, a blog entry, a user-submitted comment, an
     interactive widget or gadget, or any other independent item of content.
-    '''
+    """
+
     pass
 
 
 class aside(html_tag):
-    '''
+    """
     The aside element represents a section of a page that consists of content
     that is tangentially related to the content around the aside element, and
     which could be considered separate from that content. Such sections are
     often represented as sidebars in printed typography.
-    '''
+    """
+
     pass
 
 
 class h1(html_tag):
-    '''
+    """
     Represents the highest ranking heading.
-    '''
+    """
+
     pass
 
 
 class h2(html_tag):
-    '''
+    """
     Represents the second-highest ranking heading.
-    '''
+    """
+
     pass
 
 
 class h3(html_tag):
-    '''
+    """
     Represents the third-highest ranking heading.
-    '''
+    """
+
     pass
 
 
 class h4(html_tag):
-    '''
+    """
     Represents the fourth-highest ranking heading.
-    '''
+    """
+
     pass
 
 
 class h5(html_tag):
-    '''
+    """
     Represents the fifth-highest ranking heading.
-    '''
+    """
+
     pass
 
 
 class h6(html_tag):
-    '''
+    """
     Represents the sixth-highest ranking heading.
-    '''
+    """
+
     pass
 
 
 class hgroup(html_tag):
-    '''
+    """
     The hgroup element represents the heading of a section. The element is used
     to group a set of h1-h6 elements when the heading has multiple levels, such
     as subheadings, alternative titles, or taglines.
-    '''
+    """
+
     pass
 
 
 class header(html_tag):
-    '''
+    """
     The header element represents a group of introductory or navigational aids.
-    '''
+    """
+
     pass
 
 
 class footer(html_tag):
-    '''
+    """
     The footer element represents a footer for its nearest ancestor sectioning
     content or sectioning root element. A footer typically contains information
     about its section such as who wrote it, links to related documents,
     copyright data, and the like.
-    '''
+    """
+
     pass
 
 
 class address(html_tag):
-    '''
+    """
     The address element represents the contact information for its nearest
     article or body element ancestor. If that is the body element, then the
     contact information applies to the document as a whole.
-    '''
+    """
+
     pass
 
 
 # Grouping content
 class p(html_tag):
-    '''
+    """
     The p element represents a paragraph.
-    '''
+    """
+
     pass
 
 
 class hr(html_tag):
-    '''
+    """
     The hr element represents a paragraph-level thematic break, e.g. a scene
     change in a story, or a transition to another topic within a section of a
     reference book.
-    '''
+    """
+
     is_single = True
 
 
 class pre(html_tag):
-    '''
+    """
     The pre element represents a block of preformatted text, in which structure
     is represented by typographic conventions rather than by elements.
-    '''
+    """
+
     is_pretty = False
 
 
 class blockquote(html_tag):
-    '''
+    """
     The blockquote element represents a section that is quoted from another
     source.
-    '''
+    """
+
     pass
 
 
 class ol(html_tag):
-    '''
+    """
     The ol element represents a list of items, where the items have been
     intentionally ordered, such that changing the order would change the
     meaning of the document.
-    '''
+    """
+
     pass
 
 
 class ul(html_tag):
-    '''
+    """
     The ul element represents a list of items, where the order of the items is
     not important - that is, where changing the order would not materially change
     the meaning of the document.
-    '''
+    """
+
     pass
 
 
 class li(html_tag):
-    '''
+    """
     The li element represents a list item. If its parent element is an ol, ul, or
     menu element, then the element is an item of the parent element's list, as
     defined for those elements. Otherwise, the list item has no defined
     list-related relationship to any other li element.
-    '''
+    """
+
     pass
 
 
 class dl(html_tag):
-    '''
+    """
     The dl element represents an association list consisting of zero or more
     name-value groups (a description list). Each group must consist of one or
     more names (dt elements) followed by one or more values (dd elements).
     Within a single dl element, there should not be more than one dt element for
     each name.
-    '''
+    """
+
     pass
 
 
 class dt(html_tag):
-    '''
+    """
     The dt element represents the term, or name, part of a term-description group
     in a description list (dl element).
-    '''
+    """
+
     pass
 
 
 class dd(html_tag):
-    '''
+    """
     The dd element represents the description, definition, or value, part of a
     term-description group in a description list (dl element).
-    '''
+    """
+
     pass
 
 
 class figure(html_tag):
-    '''
+    """
     The figure element represents some flow content, optionally with a caption,
     that is self-contained and is typically referenced as a single unit from the
     main flow of the document.
-    '''
+    """
+
     pass
 
 
 class figcaption(html_tag):
-    '''
+    """
     The figcaption element represents a caption or legend for the rest of the
     contents of the figcaption element's parent figure element, if any.
-    '''
+    """
+
     pass
 
 
 class div(html_tag):
-    '''
+    """
     The div element has no special meaning at all. It represents its children. It
     can be used with the class, lang, and title attributes to mark up semantics
     common to a group of consecutive elements.
-    '''
+    """
+
     pass
 
 
 # Text semantics
 class a(html_tag):
-    '''
+    """
     If the a element has an href attribute, then it represents a hyperlink (a
     hypertext anchor).
 
     If the a element has no href attribute, then the element represents a
     placeholder for where a link might otherwise have been placed, if it had been
     relevant.
-    '''
+    """
+
     pass
 
 
 class em(html_tag):
-    '''
+    """
     The em element represents stress emphasis of its contents.
-    '''
+    """
+
     pass
 
 
 class strong(html_tag):
-    '''
+    """
     The strong element represents strong importance for its contents.
-    '''
+    """
+
     pass
 
 
 class small(html_tag):
-    '''
+    """
     The small element represents side comments such as small print.
-    '''
+    """
+
     pass
 
 
 class s(html_tag):
-    '''
+    """
     The s element represents contents that are no longer accurate or no longer
     relevant.
-    '''
+    """
+
     pass
 
 
 class cite(html_tag):
-    '''
+    """
     The cite element represents the title of a work (e.g. a book, a paper, an
     essay, a poem, a score, a song, a script, a film, a TV show, a game, a
     sculpture, a painting, a theatre production, a play, an opera, a musical, an
     exhibition, a legal case report, etc). This can be a work that is being
     quoted or referenced in detail (i.e. a citation), or it can just be a work
     that is mentioned in passing.
-    '''
+    """
+
     pass
 
 
 class q(html_tag):
-    '''
+    """
     The q element represents some phrasing content quoted from another source.
-    '''
+    """
+
     pass
 
 
 class dfn(html_tag):
-    '''
+    """
     The dfn element represents the defining instance of a term. The paragraph,
     description list group, or section that is the nearest ancestor of the dfn
     element must also contain the definition(s) for the term given by the dfn
     element.
-    '''
+    """
+
     pass
 
 
 class abbr(html_tag):
-    '''
+    """
     The abbr element represents an abbreviation or acronym, optionally with its
     expansion. The title attribute may be used to provide an expansion of the
     abbreviation. The attribute, if specified, must contain an expansion of the
     abbreviation, and nothing else.
-    '''
+    """
+
     pass
 
 
 class time_(html_tag):
-    '''
+    """
     The time element represents either a time on a 24 hour clock, or a precise
     date in the proleptic Gregorian calendar, optionally with a time and a
     time-zone offset.
-    '''
+    """
+
     pass
 
 
 _time = time_
 
 
 class code(html_tag):
-    '''
+    """
     The code element represents a fragment of computer code. This could be an XML
     element name, a filename, a computer program, or any other string that a
     computer would recognize.
-    '''
+    """
+
     pass
 
 
 class var(html_tag):
-    '''
+    """
     The var element represents a variable. This could be an actual variable in a
     mathematical expression or programming context, an identifier representing a
     constant, a function parameter, or just be a term used as a placeholder in
     prose.
-    '''
+    """
+
     pass
 
 
 class samp(html_tag):
-    '''
+    """
     The samp element represents (sample) output from a program or computing
     system.
-    '''
+    """
+
     pass
 
 
 class kbd(html_tag):
-    '''
+    """
     The kbd element represents user input (typically keyboard input, although it
     may also be used to represent other input, such as voice commands).
-    '''
+    """
+
     pass
 
 
 class sub(html_tag):
-    '''
+    """
     The sub element represents a subscript.
-    '''
+    """
+
     pass
 
 
 class sup(html_tag):
-    '''
+    """
     The sup element represents a superscript.
-    '''
+    """
+
     pass
 
 
 class i(html_tag):
-    '''
+    """
     The i element represents a span of text in an alternate voice or mood, or
     otherwise offset from the normal prose in a manner indicating a different
     quality of text, such as a taxonomic designation, a technical term, an
     idiomatic phrase from another language, a thought, or a ship name in Western
     texts.
-    '''
+    """
+
     pass
 
 
 class b(html_tag):
-    '''
+    """
     The b element represents a span of text to which attention is being drawn for
     utilitarian purposes without conveying any extra importance and with no
     implication of an alternate voice or mood, such as key words in a document
     abstract, product names in a review, actionable words in interactive
     text-driven software, or an article lede.
-    '''
+    """
+
     pass
 
 
 class u(html_tag):
-    '''
+    """
     The u element represents a span of text with an unarticulated, though
     explicitly rendered, non-textual annotation, such as labeling the text as
     being a proper name in Chinese text (a Chinese proper name mark), or
     labeling the text as being misspelt.
-    '''
+    """
+
     pass
 
 
 class mark(html_tag):
-    '''
+    """
     The mark element represents a run of text in one document marked or
     highlighted for reference purposes, due to its relevance in another context.
     When used in a quotation or other block of text referred to from the prose,
     it indicates a highlight that was not originally present but which has been
     added to bring the reader's attention to a part of the text that might not
     have been considered important by the original author when the block was
     originally written, but which is now under previously unexpected scrutiny.
     When used in the main prose of a document, it indicates a part of the
     document that has been highlighted due to its likely relevance to the user's
     current activity.
-    '''
+    """
+
     pass
 
 
 class ruby(html_tag):
-    '''
+    """
     The ruby element allows one or more spans of phrasing content to be marked
     with ruby annotations. Ruby annotations are short runs of text presented
     alongside base text, primarily used in East Asian typography as a guide for
     pronunciation or to include other annotations. In Japanese, this form of
     typography is also known as furigana.
-    '''
+    """
+
     pass
 
 
 class rt(html_tag):
-    '''
+    """
     The rt element marks the ruby text component of a ruby annotation.
-    '''
+    """
+
     pass
 
 
 class rp(html_tag):
-    '''
+    """
     The rp element can be used to provide parentheses around a ruby text
     component of a ruby annotation, to be shown by user agents that don't support
     ruby annotations.
-    '''
+    """
+
     pass
 
 
 class bdi(html_tag):
-    '''
+    """
     The bdi element represents a span of text that is to be isolated from its
     surroundings for the purposes of bidirectional text formatting.
-    '''
+    """
+
     pass
 
 
 class bdo(html_tag):
-    '''
+    """
     The bdo element represents explicit text directionality formatting control
     for its children. It allows authors to override the Unicode bidirectional
     algorithm by explicitly specifying a direction override.
-    '''
+    """
+
     pass
 
 
 class span(html_tag):
-    '''
+    """
     The span element doesn't mean anything on its own, but can be useful when
     used together with the global attributes, e.g. class, lang, or dir. It
     represents its children.
-    '''
+    """
+
     pass
 
 
 class br(html_tag):
-    '''
+    """
     The br element represents a line break.
-    '''
+    """
+
     is_single = True
     is_inline = True
 
 
 class wbr(html_tag):
-    '''
+    """
     The wbr element represents a line break opportunity.
-    '''
+    """
+
     is_single = True
     is_inline = True
 
 
 # Edits
 class ins(html_tag):
-    '''
+    """
     The ins element represents an addition to the document.
-    '''
+    """
+
     pass
 
 
 class del_(html_tag):
-    '''
+    """
     The del element represents a removal from the document.
-    '''
+    """
+
     pass
 
 
 _del = del_
 
 
 # Embedded content
 class img(html_tag):
-    '''
+    """
     An img element represents an image.
-    '''
+    """
+
     is_single = True
+    child_dedent = True
 
 
 class iframe(html_tag):
-    '''
+    """
     The iframe element represents a nested browsing context.
-    '''
+    """
+
     pass
 
 
 class embed(html_tag):
-    '''
+    """
     The embed element represents an integration point for an external (typically
     non-HTML) application or interactive content.
-    '''
+    """
+
     is_single = True
 
 
 class object_(html_tag):
-    '''
+    """
     The object element can represent an external resource, which, depending on
     the type of the resource, will either be treated as an image, as a nested
     browsing context, or as an external resource to be processed by a plugin.
-    '''
+    """
+
     pass
 
 
 _object = object_
 
 
 class param(html_tag):
-    '''
+    """
     The param element defines parameters for plugins invoked by object elements.
     It does not represent anything on its own.
-    '''
+    """
+
     is_single = True
 
 
 class video(html_tag):
-    '''
+    """
     A video element is used for playing videos or movies, and audio files with
     captions.
-    '''
+    """
+
     pass
 
 
 class audio(html_tag):
-    '''
+    """
     An audio element represents a sound or audio stream.
-    '''
+    """
+
     pass
 
 
 class source(html_tag):
-    '''
+    """
     The source element allows authors to specify multiple alternative media
     resources for media elements. It does not represent anything on its own.
-    '''
+    """
+
     is_single = True
 
 
 class track(html_tag):
-    '''
+    """
     The track element allows authors to specify explicit external timed text
     tracks for media elements. It does not represent anything on its own.
-    '''
+    """
+
     is_single = True
 
 
 class canvas(html_tag):
-    '''
+    """
     The canvas element provides scripts with a resolution-dependent bitmap
     canvas, which can be used for rendering graphs, game graphics, or other
     visual images on the fly.
-    '''
+    """
+
     pass
 
 
 class map_(html_tag):
-    '''
+    """
     The map element, in conjunction with any area element descendants, defines an
     image map. The element represents its children.
-    '''
+    """
+
     pass
 
 
 _map = map_
 
 
 class area(html_tag):
-    '''
+    """
     The area element represents either a hyperlink with some text and a
     corresponding area on an image map, or a dead area on an image map.
-    '''
+    """
+
     is_single = True
 
 
 # Tabular data
 class table(html_tag):
-    '''
+    """
     The table element represents data with more than one dimension, in the form
     of a table.
-    '''
+    """
+
     pass
 
 
 class caption(html_tag):
-    '''
+    """
     The caption element represents the title of the table that is its parent, if
     it has a parent and that is a table element.
-    '''
+    """
+
     pass
 
 
 class colgroup(html_tag):
-    '''
+    """
     The colgroup element represents a group of one or more columns in the table
     that is its parent, if it has a parent and that is a table element.
-    '''
+    """
+
     pass
 
 
 class col(html_tag):
-    '''
+    """
     If a col element has a parent and that is a colgroup element that itself has
     a parent that is a table element, then the col element represents one or more
     columns in the column group represented by that colgroup.
-    '''
+    """
+
     is_single = True
 
 
 class tbody(html_tag):
-    '''
+    """
     The tbody element represents a block of rows that consist of a body of data
     for the parent table element, if the tbody element has a parent and it is a
     table.
-    '''
+    """
+
     pass
 
 
 class thead(html_tag):
-    '''
+    """
     The thead element represents the block of rows that consist of the column
     labels (headers) for the parent table element, if the thead element has a
     parent and it is a table.
-    '''
+    """
+
     pass
 
 
 class tfoot(html_tag):
-    '''
+    """
     The tfoot element represents the block of rows that consist of the column
     summaries (footers) for the parent table element, if the tfoot element has a
     parent and it is a table.
-    '''
+    """
+
     pass
 
 
 class tr(html_tag):
-    '''
+    """
     The tr element represents a row of cells in a table.
-    '''
+    """
+
     pass
 
 
 class td(html_tag):
-    '''
+    """
     The td element represents a data cell in a table.
-    '''
+    """
+
     pass
 
 
 class th(html_tag):
-    '''
+    """
     The th element represents a header cell in a table.
-    '''
+    """
+
     pass
 
 
 # Forms
 class form(html_tag):
-    '''
+    """
     The form element represents a collection of form-associated elements, some of
     which can represent editable values that can be submitted to a server for
     processing.
-    '''
+    """
+
     pass
 
 
 class fieldset(html_tag):
-    '''
+    """
     The fieldset element represents a set of form controls optionally grouped
     under a common name.
-    '''
+    """
+
     pass
 
 
 class legend(html_tag):
-    '''
+    """
     The legend element represents a caption for the rest of the contents of the
     legend element's parent fieldset element, if any.
-    '''
+    """
+
     pass
 
 
 class label(html_tag):
-    '''
+    """
     The label represents a caption in a user interface. The caption can be
     associated with a specific form control, known as the label element's labeled
     control, either using for attribute, or by putting the form control inside
     the label element itself.
-    '''
+    """
+
     pass
 
 
 class input_(html_tag):
-    '''
+    """
     The input element represents a typed data field, usually with a form control
     to allow the user to edit the data.
-    '''
+    """
+
     is_single = True
 
 
 _input = input_
 
 
 class button(html_tag):
-    '''
+    """
     The button element represents a button. If the element is not disabled, then
     the user agent should allow the user to activate the button.
-    '''
+    """
+
     pass
 
 
 class select(html_tag):
-    '''
+    """
     The select element represents a control for selecting amongst a set of
     options.
-    '''
+    """
+
     pass
 
 
 class datalist(html_tag):
-    '''
+    """
     The datalist element represents a set of option elements that represent
     predefined options for other controls. The contents of the element represents
     fallback content for legacy user agents, intermixed with option elements that
     represent the predefined options. In the rendering, the datalist element
     represents nothing and it, along with its children, should be hidden.
-    '''
+    """
+
     pass
 
 
 class optgroup(html_tag):
-    '''
+    """
     The optgroup element represents a group of option elements with a common
     label.
-    '''
+    """
+
     pass
 
 
 class option(html_tag):
-    '''
+    """
     The option element represents an option in a select element or as part of a
     list of suggestions in a datalist element.
-    '''
+    """
+
     pass
 
 
 class textarea(html_tag):
-    '''
+    """
     The textarea element represents a multiline plain text edit control for the
     element's raw value. The contents of the control represent the control's
     default value.
-    '''
+    """
+
     pass
 
 
 class keygen(html_tag):
-    '''
+    """
     The keygen element represents a key pair generator control. When the
     control's form is submitted, the private key is stored in the local keystore,
     and the public key is packaged and sent to the server.
-    '''
+    """
+
     is_single = True
 
 
 class output(html_tag):
-    '''
+    """
     The output element represents the result of a calculation.
-    '''
+    """
+
     pass
 
 
 class progress(html_tag):
-    '''
+    """
     The progress element represents the completion progress of a task. The
     progress is either indeterminate, indicating that progress is being made but
     that it is not clear how much more work remains to be done before the task is
     complete (e.g. because the task is waiting for a remote host to respond), or
     the progress is a number in the range zero to a maximum, giving the fraction
     of work that has so far been completed.
-    '''
+    """
+
     pass
 
 
 class meter(html_tag):
-    '''
+    """
     The meter element represents a scalar measurement within a known range, or a
     fractional value; for example disk usage, the relevance of a query result, or
     the fraction of a voting population to have selected a particular candidate.
-    '''
+    """
+
     pass
 
 
 # Interactive elements
 class details(html_tag):
-    '''
+    """
     The details element represents a disclosure widget from which the user can
     obtain additional information or controls.
-    '''
+    """
+
     pass
 
 
 class summary(html_tag):
-    '''
+    """
     The summary element represents a summary, caption, or legend for the rest of
     the contents of the summary element's parent details element, if any.
-    '''
+    """
+
     pass
 
 
 class command(html_tag):
-    '''
+    """
     The command element represents a command that the user can invoke.
-    '''
+    """
+
     is_single = True
 
 
 class menu(html_tag):
-    '''
+    """
     The menu element represents a list of commands.
-    '''
+    """
+
     pass
 
 
 class font(html_tag):
-    '''
+    """
     The font element represents the font in a html .
-    '''
+    """
+
     pass
 
 
-# Additional markup
-class comment(html_tag):
-    is_inline = True
-    '''
-    Normal, one-line comment:
-      >>> print comment("Hello, comments!")
-      <!--Hello, comments!-->
-
-    For IE's "if" statement comments:
-      >>> print comment(p("Upgrade your browser."), condition='lt IE6')
-      <!--[if lt IE6]><p>Upgrade your browser.</p><![endif]-->
-
-    Downlevel conditional comments:
-      >>> print comment(p("You are using a ", em("downlevel"), " browser."),
-              condition='false', downlevel='revealed')
-      <![if false]><p>You are using a <em>downlevel</em> browser.</p><![endif]>
-
-    For more on conditional comments see:
-      http://msdn.microsoft.com/en-us/library/ms537512(VS.85).aspx
-    '''
-
-    ATTRIBUTE_CONDITION = 'condition'
-
-    # Valid values are 'hidden', 'downlevel' or 'revealed'
-    ATTRIBUTE_DOWNLEVEL = 'downlevel'
-
-    def _render(self, sb, indent_level=1, indent_str='  ', pretty=True, xhtml=False):
-        has_condition = comment.ATTRIBUTE_CONDITION in self.attributes
-        is_revealed = comment.ATTRIBUTE_DOWNLEVEL in self.attributes and \
-                      self.attributes[comment.ATTRIBUTE_DOWNLEVEL] == 'revealed'
-
-        sb.append('<!')
-        if not is_revealed:
-            sb.append('--')
-        if has_condition:
-            sb.append('[if %s]>' % self.attributes[comment.ATTRIBUTE_CONDITION])
-
-        pretty = self._render_children(sb, indent_level+1, indent_str, pretty, xhtml)
-
-        # if len(self.children) > 1:
-        if any(isinstance(child, dom_tag) for child in self):
-            sb.append('\n')
-            sb.append(indent_str * indent_level)
-
-        if has_condition:
-            sb.append('<![endif]')
-        if not is_revealed:
-            if pretty:
-                sb, _ = self._new_line_and_inline_handler(sb, indent_level, indent_str, pretty, self.is_inline)
-            sb.append('--')
-        sb.append('>')
+class comment(extension.SingleTemplates):
+    left_delimiter = "<!--"
+    right_delimiter = "-->"
+    enable_left_delimiter_space = True
+    enable_right_delimiter_space = True
 
-        return sb
+    """
+    <-- comments -->
+    """
+
+    def __init__(self, comments):
+        super().__init__("", comments)
 
 
 class template(html_tag):
     "The template element represents a template."
     pass
 
 
 class slot(html_tag):
     "The slot element represents a slot."
     pass
 
 
-class ConcatTag(extension.DoubleTags):
-    # this is an empty tag with spits out children concatenated with new-line
-    '''
-    Supporting Concatenation of Tags as siblings with newline at end
-    '''
-    render_tag = False
-    new_line_at_child_end = True
-
+if __name__ == "__main__":
+    from uidom.dom.src.utils.dom_util import dom_text
 
-if __name__ == '__main__':
-    from uidom.dom.src.utils.dom_util import text
+    print(comment("sjskdj"))
     print(div(div(div(div(script("aa")), __inline=True))))
-    print(ConcatTag(text('h')))
+    print(extension.PlaceholderTag(dom_text("a"), dom_text("b"), dom_text("  c data")))
+    print(extension.PlaceholderTag("h", "h", "h"))
+    print(div(div(img(img(), img(self_dedent=True), div()), img(), div(div()))))
+    print(div(div(div(img(div(div(img())))))))
+    print(div(div(self_dedent=True), child_dedent=False))
+    print(div(div(self_dedent=False), child_dedent=False))
+    print((div() & p() & div()))
```

### Comparing `uidom-0.1.1b6/uidom/dom/src/jinjatags.py` & `uidom-0.2a0/uidom/dom/src/jinjatags.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 from jinja2.environment import Template
+
+from uidom.dom.src.dom_tag import dom_tag
 from uidom.dom.src.main import extension
 
 __all__ = [
     "If",
     "Elif",
     "Else",
     "For",
@@ -17,55 +19,64 @@
     "Cycle",
     "Comment",
     "Extends",
     "Load",
     "CSRFToken",
     "Block",
     "Var",
-    "render"
+    "render",
+    "JinjaSingleTags",
+    "JinjaDoubleTags",
+    "JinjaBaseTag",
 ]
 
 
-class JinjaConfig(object):
+class JinjaBaseTag(object):
+    pass
+
+
+class JinjaDoubleTags(JinjaBaseTag, extension.DoubleTemplates):
     self_dedent = False
     child_dedent = False
     enable_left_delimiter_space = True
     enable_right_delimiter_space = True
 
+    def __call__(self, **options):
+        return render(self, **options)
 
-class JinjaDoubleTags(JinjaConfig, extension.DoubleTemplates):
-    pass
 
+class JinjaSingleTags(JinjaBaseTag, extension.SingleTemplates):
+    self_dedent = False
+    child_dedent = True
+    enable_left_delimiter_space = True
+    enable_right_delimiter_space = True
 
-class JinjaSingleTags(JinjaConfig, extension.SingleTemplates):
-    pass
+    def __call__(self, **options):
+        return render(self, **options)
 
 
 class Block(JinjaDoubleTags):
-
     def __init__(self, template_text, *dom_elements):
         """
         :param template_text:
         :param dom_elements: [optional] template
         """
         super(Block, self).__init__("block", template_text, *dom_elements)
 
 
 class For(JinjaDoubleTags):
-
     def __init__(self, template_text, *dom_elements):
         """
         :param template_text:
         :param dom_elements: [optional] template
         """
         super(For, self).__init__("for", template_text, *dom_elements)
 
 
 class If(JinjaDoubleTags):
-
     def __init__(self, template_text, *dom_elements):
         """
         :param template_text:
         :param dom_elements: [optional] template
         """
         super(If, self).__init__("if", template_text, *dom_elements)
 
@@ -77,21 +88,24 @@
     def __init__(self, template_text, *dom_elements):
         """
         :param template_text:
         :param dom_elements: [optional] template
         """
 
         super(Elif, self).__init__(
-            "elif", template_text, *dom_elements,
+            "elif",
+            template_text,
+            *dom_elements,
         )
 
 
 class Else(JinjaSingleTags):
     self_dedent = True
     child_dedent = False
+    enable_right_delimiter_space = False
 
     def __init__(self, *dom_elements):
         """
         :param template_text:
         :param dom_elements: [optional] template
         """
 
@@ -105,15 +119,14 @@
         :param dom_elements: [optional] template
         """
 
         super(AutoEscape, self).__init__("autoescape", template_text, *dom_elements)
 
 
 class Include(JinjaSingleTags):
-
     def __init__(self, template_text, *dom_elements):
         """
         :param template_text:
         :param dom_elements: [optional] template
         """
 
         super(Include, self).__init__("include", template_text, *dom_elements)
@@ -179,53 +192,18 @@
         :param dom_elements: [optional] template
         """
 
         super(Var, self).__init__("", template_text, *dom_elements)
 
 
 def render(template, **options):
-    return Template(
-        template.render() if isinstance(template, extension.Tags) else template,
-        lstrip_blocks=True,
-        trim_blocks=True,
-        enable_async=True).render(**options)
-
-
-if __name__ == '__main__':
-    from collections import namedtuple as nt
-
-    from uidom.dom.src.htmltags import a, html, li, nav, p, section, ul
-
-    print(Block("base",
-                html(For("name in names",
-                         If("name", Block("load", Load("space")),
-                            Elif("njnsf", p("ksf")),
-                            Else(section(p("ok", Var("name"))))
-                            )
-                         )
-                     ))
-          )
-
-    menu = Block(
-        "nav",
-        nav(
-            ul(
-                For(
-                    "item in menu_items",
-                    li(a(Var("item.name"), href=Var("item.link"))),
-                )
-            )
-        ),
-    )
-    menu_url = nt("menu_url", "name link")
-    print(render(
-        menu,
-        menu_items=[
-            menu_url("Home", "home.html"),
-            menu_url("About", "about.html"),
-            menu_url("Contact Us", "contact_us.html")
-        ]
-    )
+    return raw(
+        Template(
+            template.__render__() if isinstance(template, dom_tag) else template,
+            lstrip_blocks=True,
+            trim_blocks=True,
+            enable_async=True,
+        ).render(**options)
     )
 
-    print(ul(For("name in names", li(Var("name")))))
-    print(ul(li(x_text="name"), x_for="name in names", x_data={}))
+
+from uidom.dom.src.utils import raw
```

### Comparing `uidom-0.1.1b6/uidom/dom/src/parse_html.py` & `uidom-0.2a0/uidom/dom/src/parse_html.py`

 * *Files identical despite different names*

### Comparing `uidom-0.1.1b6/uidom/dom/src/pythontags.py` & `uidom-0.2a0/uidom/dom/src/pythontags.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 from uidom.dom.src import extension
 
 
 class Python(extension.SingleTemplates):
     enable_right_delimiter_space = False
     enable_left_delimiter_space = True
     enable_space_in_between = False
 
-    def render(self, indent="    ", pretty=True, xhtml=False):
+    def __render__(self, indent="    ", pretty=True, xhtml=False):
         data = self._render([], 0, indent, pretty, xhtml)
         return "".join(data)
 
 
 class Class(Python):
     self_dedent = True
     child_dedent = False
@@ -46,29 +46,64 @@
 
 
 class Def(Python):
     left_delimiter = "def"
     right_delimiter = ":"
 
     def __init__(self, func_name, *dom_elements, args=""):
-        super(Def, self).__init__(f"{func_name}", f"({', '.join(['self', *args.split(' ')]) if any(args) else 'self'})",
-                                  *dom_elements)
+        super(Def, self).__init__(
+            f"{func_name}",
+            f"({', '.join(['self', *args.split(' ')]) if any(args) else 'self'})",
+            *dom_elements,
+        )
         if func_name == "__init__" and any(args):
             [self.add(SelfAttr(arg)) for arg in args.split(" ")]
 
 
 class SelfAttr(Python):
     left_delimiter = ""
     right_delimiter = ""
     enable_left_delimiter_space = False
 
     def __init__(self, atr_name, *dom_elements):
-        super(SelfAttr, self).__init__(f"self.{atr_name}", '', *dom_elements)
+        super(SelfAttr, self).__init__(f"self.{atr_name}", "", *dom_elements)
+
+
+class With(Python):
+    self_dedent = True
+    child_dedent = False
+    left_delimiter = "with"
+    right_delimiter = ":"
+
+    def __init__(self, element_name, *children, **kwargs):
+        items = []
+        for k, v in kwargs.items():
+            k = self.clean_attribute(k)
+            k.replace("-", "_")
+            if k == "class":
+                k = "className"
+            items.append("%s='%s'" % (k, v))
+        super(With, self).__init__(element_name, f"({', '.join(items)})", *children)
 
 
 if __name__ == "__main__":
-    import ast
-    person = Class("Person",
-                   # Def("__init__", args="name address"),
-                   Def('__render__', args="*args **kwargs"),
-                   bases="models.Model logging.Logger")
+    person = Class(
+        "Person",
+        # Def("__init__", args="name address"),
+        Def("render", args="*args **kwargs"),
+        bases="models.Model logging.Logger",
+    )
     print(person)
+
+    elem = With(
+        "html",
+        With("div", "pass", className="bg-rose-400"),
+        className="World",
+        hx_get="/index",
+    )
+    print("\n")
+    _html = Class(
+        "Html",
+        Def("render", elem, args="*args **kwargs"),
+        bases="HTMLElement",
+    )
+    print(_html)
```

### Comparing `uidom-0.1.1b6/uidom/dom/src/sphinxtags.py` & `uidom-0.2a0/uidom/dom/src/sphinxtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.1.1b6/uidom/dom/src/svgtags.py` & `uidom-0.2a0/uidom/dom/src/svgtags.py`

 * *Files identical despite different names*

### Comparing `uidom-0.1.1b6/uidom/dom/src/utils/dom_util.py` & `uidom-0.2a0/uidom/dom/src/utils/dom_util.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
-'''
+"""
 Utility classes for creating dynamic html documents
-'''
+"""
 
-__license__ = '''
+__license__ = """
 This file is part of Dominate.
 
 Dominate is free software: you can redistribute it and/or modify
 it under the terms of the GNU Lesser General Public License as
 published by the Free Software Foundation, either version 3 of
 the License, or (at your option) any later version.
 
@@ -20,160 +20,162 @@
 WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU Lesser General Public License for more details.
 
 You should have received a copy of the GNU Lesser General
 Public License along with Dominate.  If not, see
 <http://www.gnu.org/licenses/>.
-'''
+"""
 
 import re
 
 from uidom.dom.src.dom_tag import dom_tag
 
 try:
     basestring = basestring
 except NameError:
     basestring = str
     unichr = chr
 
 
 def include(f):
-    '''
+    """
     includes the contents of a file on disk.
     takes a filename
-    '''
-    fl = open(f, 'r')
+    """
+    fl = open(f, "r")
     data = fl.read()
     fl.close()
     return raw(data)
 
 
 def system(cmd, data=None):
-    '''
+    """
     pipes the output of a program
-    '''
+    """
     import subprocess
+
     s = subprocess.Popen(cmd, shell=True, stdout=subprocess.PIPE, stdin=subprocess.PIPE)
     out, err = s.communicate(data)
-    return out.decode('utf8')
+    return out.decode("utf8")
 
 
 def escape(data, quote=True):  # stolen from std lib cgi
-    '''
+    """
     Escapes special characters into their html entities
     Replace special characters "&", "<" and ">" to HTML-safe sequences.
     If the optional flag quote is true, the quotation mark character (")
     is also translated.
 
     This is used to escape content that appears in the body of an HTML document
-    '''
+    """
     data = data.replace("&", "&amp;")  # Must be done first!
     data = data.replace("<", "&lt;")
     data = data.replace(">", "&gt;")
     if quote:
         data = data.replace('"', "&quot;")
     return data
 
 
 _unescape = {
-    'quot': 34,
-    'amp': 38,
-    'lt': 60,
-    'gt': 62,
-    'nbsp': 32,
+    "quot": 34,
+    "amp": 38,
+    "lt": 60,
+    "gt": 62,
+    "nbsp": 32,
     # more here
     # http://www.w3.org/TR/html4/sgml/entities.html
-    'yuml': 255,
+    "yuml": 255,
 }
 str_escape = escape
 
 
 def unescape(data):
-    '''
+    """
     unescapes html entities. the opposite of escape.
-    '''
-    cc = re.compile(r'&(?:(?:#(\d+))|([^;]+));')
+    """
+    cc = re.compile(r"&(?:(?:#(\d+))|([^;]+));")
 
     result = []
     m = cc.search(data)
     while m:
-        result.append(data[0:m.start()])
+        result.append(data[0 : m.start()])
         d = m.group(1)
         if d:
             d = int(d)
             result.append(unichr(d))
         else:
-            d = _unescape.get(m.group(2), ord('?'))
+            d = _unescape.get(m.group(2), ord("?"))
             result.append(unichr(d))
 
-        data = data[m.end():]
+        data = data[m.end() :]
         m = cc.search(data)
 
     result.append(data)
-    return ''.join(result)
+    return "".join(result)
 
 
 _reserved = ";/?:@&=+$, "
-_replace_map = dict((c, '%%%2X' % ord(c)) for c in _reserved)
+_replace_map = dict((c, "%%%2X" % ord(c)) for c in _reserved)
 
 
 def url_escape(data):
-    return ''.join(_replace_map.get(c, c) for c in data)
+    return "".join(_replace_map.get(c, c) for c in data)
 
 
 def url_unescape(data):
-    return re.sub('%([0-9a-fA-F]{2})',
-                  lambda m: unichr(int(m.group(1), 16)), data)
+    return re.sub("%([0-9a-fA-F]{2})", lambda m: unichr(int(m.group(1), 16)), data)
 
 
 class lazy(dom_tag):
-    '''
+    """
     delays function execution until rendered
-    '''
+    """
 
     def __new__(_cls, *args, **kwargs):
-        '''
+        """
         Need to reset this special method or else
         dom_tag will think it's being used as a dectorator.
 
         This means lazy() can't be used as a dectorator, but
         thinking about when you might want that just confuses me.
-        '''
+        """
         return object.__new__(_cls)
 
     def __init__(self, func, *args, **kwargs):
         super(lazy, self).__init__()
         self.func = func
         self.args = args
         self.kwargs = kwargs
 
     def _render(self, sb, *a, **kw):
         r = self.func(*self.args, **self.kwargs)
         sb.append(str(r))
+        return sb
 
 
 # TODO rename this to raw?
 class dom_text(dom_tag):
-    '''
+    """
     Just a string. useful for inside context managers
-    '''
+    """
+
     is_pretty = False
     is_inline = False
 
     def __init__(self, _text, escape=True):
-        super(dom_text, self).__init__()
         if escape:
             self.text = str_escape(_text)
         else:
             self.text = _text
+        super(dom_text, self).__init__()
 
     def _render(self, sb, *a, **kw):
         sb.append(self.text)
         return sb
 
 
 def raw(s):
-    '''
+    """
     Inserts a raw string into the DOM. Unsafe.
-    '''
+    """
     return dom_text(s, escape=False)
```

### Comparing `uidom-0.1.1b6/uidom/dom/src/utils/sheets.py` & `uidom-0.2a0/uidom/dom/src/utils/sheets.py`

 * *Files identical despite different names*

### Comparing `uidom-0.1.1b6/uidom/dom/ui.py` & `uidom-0.2a0/uidom/dom/ui.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
 import asyncio
 import typing
 import uuid
@@ -11,15 +11,16 @@
 from datetime import datetime, time
 from enum import Enum, IntEnum
 from pathlib import Path
 from uuid import UUID
 
 import valio
 from tortoise import Model, Tortoise
-from uidom import dom
+
+from uidom import dom, elements
 
 valio.Validator.register(Model)
 
 
 class ModelValidator(valio.Validator):
     annotation = typing.Union[Model, None]
 
@@ -69,18 +70,15 @@
         return await self.get(field=field, value=value)
 
 
 async def init():
     # Here we create a SQLite DB using file "db.sqlite3"
     #  also specify the app name of "models"
     #  which contain models from "app.models"
-    await Tortoise.init(
-        db_url='sqlite://db.sqlite3',
-        modules={'models': ['__main__']}
-    )
+    await Tortoise.init(db_url="sqlite://db.sqlite3", modules={"models": ["__main__"]})
     # Generate the schema
     await Tortoise.generate_schemas()
 
 
 async def query(q):
     await init()
     value = await asyncio.gather(q)
@@ -92,199 +90,236 @@
     labels = None
     inputs = None
     fields = None
     buttons = None
     form = None
 
     INPUT = {
-        str: dom.CharInput,
-        int: dom.IntegerField,
-        float: dom.FloatInput,
-        bytes: dom.FileButtonInput,
-        bool: dom.CheckboxInput,
-        time: dom.DateInput,
-        Path: dom.FileButtonInput,
-        UUID: dom.CharInput,
-        Enum: dom.EnumInput,
-        IntEnum: dom.IntegerEnumInput
+        str: elements.CharInput,
+        int: elements.IntegerField,
+        float: elements.FloatInput,
+        bytes: elements.FileButtonInput,
+        bool: elements.CheckboxInput,
+        time: elements.DateInput,
+        Path: elements.FileButtonInput,
+        UUID: elements.CharInput,
+        Enum: elements.EnumInput,
+        IntEnum: elements.IntegerEnumInput,
     }
 
     LABEL = {
-        str: dom.CharLabel,
-        int: dom.IntegerLabel,
-        float: dom.FloatLabel,
-        bytes: dom.CharLabel,
-        bool: dom.BooleanLabel,
-        datetime.time: dom.DateLabel,
-        Path: dom.CharLabel,
-        UUID: dom.CharLabel,
-        Enum: dom.EnumLabel,
-        IntEnum: dom.EnumLabel
+        str: elements.CharLabel,
+        int: elements.IntegerLabel,
+        float: elements.FloatLabel,
+        bytes: elements.CharLabel,
+        bool: elements.BooleanLabel,
+        datetime.time: elements.DateLabel,
+        Path: elements.CharLabel,
+        UUID: elements.CharLabel,
+        Enum: elements.EnumLabel,
+        IntEnum: elements.EnumLabel,
     }
 
     CSS = {
         str: {
             "labels": "font-sm font-mono text-md px-2 uppercase",
             "inputs": "px-2 focus:outline-none focus:ring-2 focus:ring-gray-300 rounded-lg "
-                      "placeholder-gray-400 bg-gray-100",
-            "fields": "flex flex-row justify-between space-x-4 m-1 p-2 " 
-                      "rounded-lg shadow-md border-2 border-gray-300 w-full"
+            "placeholder-gray-400 bg-gray-100",
+            "fields": "flex flex-row justify-between space-x-4 m-1 p-2 "
+            "rounded-lg shadow-md border-2 border-gray-300 w-full",
         },
-
         bool: {
             "labels": "font-sm font-mono text-md px-2 uppercase",
             "inputs": "px-2 focus:outline-none focus:ring-2 focus:ring-gray-300 rounded-lg bg-gray-100",
             "fields": "flex flex-row justify-between space-x-2 m-1 p-2 "
-                      "rounded-lg shadow-md border-2 border-gray-300 w-full"
+            "rounded-lg shadow-md border-2 border-gray-300 w-full",
         },
-
-        "buttons": {"save": "flex flex-row bg-green-500 hover:bg-green-400 whitespace-nowrap "
-                            "text-white m-2 p-2 rounded-lg justify-evenly space-x-2",
-                    "delete": "flex flex-row border border-red-500 hover:border-red-400 whitespace-nowrap "
-                              "text-red-500 m-2 p-2 rounded-lg justify-evenly space-x-2",
-                    "edit": "flex flex-row bg-blue-500 hover:bg-blue-400 whitespace-nowrap "
-                            "m-2 text-white p-2 rounded-lg justify-evenly space-x-2",
-                    "buttons": "flex flex-row p-2 m-2 justify-between"}
-
-        }
+        "buttons": {
+            "save": "flex flex-row bg-green-500 hover:bg-green-400 whitespace-nowrap "
+            "text-white m-2 p-2 rounded-lg justify-evenly space-x-2",
+            "delete": "flex flex-row border border-red-500 hover:border-red-400 whitespace-nowrap "
+            "text-red-500 m-2 p-2 rounded-lg justify-evenly space-x-2",
+            "edit": "flex flex-row bg-blue-500 hover:bg-blue-400 whitespace-nowrap "
+            "m-2 text-white p-2 rounded-lg justify-evenly space-x-2",
+            "buttons": "flex flex-row p-2 m-2 justify-between",
+        },
+    }
 
     def __new__(mcs, name, bases, namespaces):
         inputs = dict()
         labels = dict()
         fields = dict()
         _annotations = dict()
         buttons = dict()
         btn_css = mcs.CSS.get("buttons", None)
-        meta = namespaces.get('Meta', None)
-        model = getattr(meta, 'model', None)
+        meta = namespaces.get("Meta", None)
+        model = getattr(meta, "model", None)
 
         for base in bases:
             for ns, ann in base.__dict__.get("__annotations__", {}).items():
                 if ns in getattr(base, "Meta", mcs.Meta).exclude:
                     continue
                 _annotations[ns] = ann
                 if not issubclass(ann, UIBase):
                     inputs[ns] = mcs.INPUT[ann]
                     labels[ns] = mcs.LABEL[ann]
                 else:
                     data = queries(model.all().select_related(ns))
                     labels[ns] = dom.span(f"Choose {ns}")
-                    inputs[ns] = dom.select(dom.option(opt, value=str(opt)) for opt in data)
-                    edit_btn = dom.SubmitButton(label=f"Edit {ann.__qualname__}",
-                                                     value=f"edit_{ann.__qualname__.lower()}")
-                    edit_btn["class"] = btn_css.get("edit", '') if btn_css is not None else ''
+                    inputs[ns] = dom.select(
+                        dom.option(opt, value=str(opt)) for opt in data
+                    )
+                    edit_btn = dom.SubmitButton(
+                        label=f"Edit {ann.__qualname__}",
+                        value=f"edit_{ann.__qualname__.lower()}",
+                    )
+                    edit_btn["class"] = (
+                        btn_css.get("edit", "") if btn_css is not None else ""
+                    )
                     fields[ns] = dom.div(labels[ns], inputs[ns], edit_btn)
 
         for ns, ann in namespaces.get("__annotations__", {}).items():
             if ns in getattr(namespaces, "Meta", mcs.Meta).exclude:
                 continue
             _annotations[ns] = ann
             if not issubclass(ann, UIBase):
                 inputs[ns] = mcs.INPUT[ann]
                 labels[ns] = mcs.LABEL[ann]
             else:
                 data = asyncio.run(query(model.all().select_related(ns)))
                 labels[ns] = dom.span(f"Choose {ns}")
-                inputs[ns] = dom.select(dom.option(id=opt.id, value=str(opt)) for opt in data)
-                edit_btn = dom.SubmitButton(label=f"Edit {ann.__qualname__}", icon=dom.manage_icon,
-                                                 value=f"edit_{ann.__qualname__.lower()}")
-                edit_btn["class"] = btn_css.get("edit", '') if btn_css is not None else ''
+                inputs[ns] = dom.select(
+                    dom.option(id=opt.id, value=str(opt)) for opt in data
+                )
+                edit_btn = dom.SubmitButton(
+                    label=f"Edit {ann.__qualname__}",
+                    icon=dom.manage_icon,
+                    value=f"edit_{ann.__qualname__.lower()}",
+                )
+                edit_btn["class"] = (
+                    btn_css.get("edit", "") if btn_css is not None else ""
+                )
                 fields[ns] = dom.div(labels[ns], inputs[ns], edit_btn)
 
         for atr in inputs:
             if not isinstance(inputs[atr], dict):
                 if callable(inputs[atr]):
                     atr_name = atr.replace("_", "-")
                     if "_" in atr:
-                        atr_label = " ".join(map(lambda x: x.capitalize(), atr.replace('_', ' ').split()))
+                        atr_label = " ".join(
+                            map(lambda x: x.capitalize(), atr.replace("_", " ").split())
+                        )
                     else:
                         atr_label = atr.capitalize()
                     css = mcs.CSS.get(_annotations[atr], None)
-                    inputs[atr] = inputs[atr](name=atr_name, placeholder=f"Enter {atr_label}",
-                                              cls=css.get("inputs", '') if css is not None else '')
-                    labels[atr] = labels[atr](label=atr_label,
-                                              cls=css.get("labels", '') if css is not None else '')
+                    inputs[atr] = inputs[atr](
+                        name=atr_name,
+                        placeholder=f"Enter {atr_label}",
+                        cls=css.get("inputs", "") if css is not None else "",
+                    )
+                    labels[atr] = labels[atr](
+                        label=atr_label,
+                        cls=css.get("labels", "") if css is not None else "",
+                    )
                     labels[atr]["for"] = inputs[atr]["id"] = atr_name
-                    fields[atr] = dom.div(labels[atr], inputs[atr],
-                                               cls=css.get("fields", '') if css is not None else '')
-
-        buttons["save"] = dom.SubmitButton(label=f"Save {name}", icon=dom.save_icon,
-                                                value=f'save_{name.lower()}')
-        buttons["save"]["class"] = btn_css.get("save", '') if btn_css is not None else ''
-        buttons["delete"] = dom.SubmitButton(label=f"Delete {name}", icon=dom.delete_icon,
-                                                  value=f'delete_{name.lower()}')
-        buttons["delete"]["class"] = btn_css.get("delete", '') if btn_css is not None else ''
-        buttons["buttons"] = dom.div(buttons["delete"], buttons["save"],
-                                          cls=btn_css.get("buttons", '') if btn_css is not None else '')
+                    fields[atr] = dom.div(
+                        labels[atr],
+                        inputs[atr],
+                        cls=css.get("fields", "") if css is not None else "",
+                    )
+
+        buttons["save"] = dom.SubmitButton(
+            label=f"Save {name}", icon=dom.save_icon, value=f"save_{name.lower()}"
+        )
+        buttons["save"]["class"] = (
+            btn_css.get("save", "") if btn_css is not None else ""
+        )
+        buttons["delete"] = dom.SubmitButton(
+            label=f"Delete {name}", icon=dom.delete_icon, value=f"delete_{name.lower()}"
+        )
+        buttons["delete"]["class"] = (
+            btn_css.get("delete", "") if btn_css is not None else ""
+        )
+        buttons["buttons"] = dom.div(
+            buttons["delete"],
+            buttons["save"],
+            cls=btn_css.get("buttons", "") if btn_css is not None else "",
+        )
 
         form = dom.Form(*fields.values(), buttons["buttons"])
         cls = type.__new__(mcs, name, bases, namespaces)
         setattr(cls, "labels", labels)
         setattr(cls, "inputs", inputs)
         setattr(cls, "fields", fields)
         setattr(cls, "buttons", buttons)
         setattr(cls, "form", form)
         return cls
 
     class Meta:
-        exclude:list = []
+        exclude: list = []
 
 
 @dataclass
 class UIBase(metaclass=UiMeta):
     pass
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import typing
     from dataclasses import dataclass
 
     import valio
     from tortoise import Model, fields
+
     from uidom.backend.database.db import queries
 
     class IDMixin(object):
         id = fields.UUIDField(pk=True)
 
     class TimeStampMixin(object):
         created_at = fields.DatetimeField(auto_now_add=True)
         updated_at = fields.DatetimeField(auto_now=True)
 
-
     class CountryModel(Model, IDMixin, TimeStampMixin):
         country = fields.CharField(max_length=50)
 
         def __str__(self):
             return f"Country: {str(self.country)}"
 
         class Meta:
             table = "country"
 
     class StateModel(Model, IDMixin, TimeStampMixin):
-        country = fields.ForeignKeyField(model_name="models.CountryModel", related_name="states")
+        country = fields.ForeignKeyField(
+            model_name="models.CountryModel", related_name="states"
+        )
         state = fields.CharField(max_length=50)
 
         def __str__(self):
             return f"State: {str(self.state)}, {str(self.country)}"
 
         class Meta:
             table = "state"
 
     class CityModel(Model, IDMixin, TimeStampMixin):
-        state = fields.ForeignKeyField(model_name="models.StateModel", related_name="cities")
+        state = fields.ForeignKeyField(
+            model_name="models.StateModel", related_name="cities"
+        )
         city = fields.CharField(max_length=50)
 
         def __str__(self):
             return f"City: {self.city}, {str(self.state)}"
 
         class Meta:
             table = "city"
 
     class LocationModel(Model, IDMixin, TimeStampMixin):
-        city = fields.ForeignKeyField(model_name="models.CityModel", related_name="locations")
+        city = fields.ForeignKeyField(
+            model_name="models.CityModel", related_name="locations"
+        )
         street_name = fields.CharField(max_length=50)
 
         class Meta:
             table = "location"
 
     class UserModel(Model, IDMixin, TimeStampMixin):
         first_name = fields.CharField(max_length=50, blank=True, null=True)
@@ -319,18 +354,26 @@
             table = "product_type"
 
     class AccountModel(Model, IDMixin, TimeStampMixin):
         email = fields.CharField(max_length=50)
         password = fields.CharField(max_length=80)
         is_active = fields.BooleanField(default=False)
         is_verified = fields.BooleanField(default=False)
-        user = fields.ForeignKeyField(model_name="models.UserModel", related_name="accounts")
-        product_type = fields.ForeignKeyField(model_name="models.ProductTypeModel", related_name="accounts")
-        account_type = fields.ForeignKeyField(model_name="models.AccountTypeModel", related_name="accounts")
-        location = fields.ForeignKeyField(model_name="models.LocationModel", related_name="accounts")
+        user = fields.ForeignKeyField(
+            model_name="models.UserModel", related_name="accounts"
+        )
+        product_type = fields.ForeignKeyField(
+            model_name="models.ProductTypeModel", related_name="accounts"
+        )
+        account_type = fields.ForeignKeyField(
+            model_name="models.AccountTypeModel", related_name="accounts"
+        )
+        location = fields.ForeignKeyField(
+            model_name="models.LocationModel", related_name="accounts"
+        )
 
         class Meta:
             table = "account"
 
     class Tokens(Model, IDMixin, TimeStampMixin):
         account = fields.ForeignKeyField(model_name="models.Account")
 
@@ -358,23 +401,20 @@
         country: str = country_field.validator
 
         class Meta:
             model = CountryModel
 
     valio.Validator.register(Country)  # noqa
 
-
     class CountryValidator(valio.Validator):
         annotation = typing.Union[Country, None]
 
-
     class CountryField(valio.Field):
         validator = CountryValidator
 
-
     @dataclass
     class State(UIBase, ID, TimeStamp):
         country_field = CountryField(logger=False, debug=True)
         state_field = valio.StringField(logger=False, max_length=50)
 
         country: typing.Union[Country, CountryValidator] = country_field.validator
         state: str = state_field.validator
@@ -405,15 +445,15 @@
     class CityValidator(valio.Validator):
         annotation = typing.Union[City, None]
 
     class CityField(valio.Field):
         validator = CityValidator
 
     @dataclass
-    class Location(UIBase, ID,  TimeStamp):
+    class Location(UIBase, ID, TimeStamp):
         city_field = CityField(logger=False)
         street_field = valio.StringField(logger=False)
 
         city: City = city_field.validator
         street_name = street_field.validator
 
         class Meta:
@@ -440,16 +480,20 @@
 
     @dataclass
     class Account(UIBase, TimeStamp):
         email: str = valio.EmailIDValidator(logger=False, debug=True)
         is_active: bool = valio.BooleanValidator(logger=False, debug=True)
         is_verified: bool = valio.BooleanValidator(logger=False, debug=True)
         user: User = UserValidator(logger=False, debug=True)
-        account_type: typing.Union[str, Enum, None] = valio.StringEnumField(in_choices=AccountTypeEnum, debug=True)
-        product_type: typing.Union[str, Enum, None] = valio.StringEnumField(in_choices=ProductTypeEnum, debug=True)
+        account_type: typing.Union[str, Enum, None] = valio.StringEnumField(
+            in_choices=AccountTypeEnum, debug=True
+        )
+        product_type: typing.Union[str, Enum, None] = valio.StringEnumField(
+            in_choices=ProductTypeEnum, debug=True
+        )
         locations: Location = LocationValidator(logger=False, debug=True)
 
         class Meta:
             model = AccountModel
 
     print(Country.form)
```

### Comparing `uidom-0.1.1b6/uidom/dom/utils/functional.py` & `uidom-0.2a0/uidom/utils/functional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
-import collections
+import types
 import typing
 
 __all__ = ["map_recursive", "apply_to_list", "apply_to_dict", "apply_to_tuple"]
 
 iter_types = typing.Iterable, typing.Iterator, typing.Mapping
 
 
-def f(value, key=None): return value if key is None else key, value
+def f(value, key=None):
+    return value if key is None else key, value
 
 
 def apply_to_list(elem_func, iterable, obj_func=None):
     obj_func = obj_func or f
     return list(
         apply_to_frozenset(elem_func, item, obj_func)
         if isinstance(item, frozenset)
@@ -112,26 +113,28 @@
         return apply_to_list(elem_func, iterable, obj_func)
     if isinstance(iterable, tuple):
         return apply_to_tuple(elem_func, iterable, obj_func)
     if isinstance(iterable, set):
         return apply_to_set(elem_func, iterable, obj_func)
     if isinstance(iterable, frozenset):
         return apply_to_frozenset(elem_func, iterable, obj_func)
-    if isinstance(iterable, collections.Generator):
+    if isinstance(iterable, types.GeneratorType):
         return (map_recursive(elem_func, item, obj_func) for item in iterable)
+    return elem_func(iterable)
 
 
 def map_r(func, iterables):
     return (map_recursive(func, iterable) for iterable in iterables)
 
 
 def zip_recursive(iterables):
     # TODO make this function
     pass
 
+
 #
 # def _test_dict_map():
 #     return map_recursive(
 #         lambda x: x if isinstance(x, int) else None,
 #         {"prices": [1, [2, [3.0], (9.0, 5)]]},
 #     )
 #
```

### Comparing `uidom-0.1.1b6/uidom/dom/xcomponent_js.py` & `uidom-0.2a0/uidom/scripts/xcomponent.js`

 * *Files 13% similar despite different names*

```diff
@@ -1,881 +1,747 @@
-00000000: 2320 436f 7079 7269 6768 7420 2863 2920  # Copyright (c) 
-00000010: 3230 3232 2075 6964 6f6d 0a23 200a 2320  2022 uidom.# .# 
-00000020: 5468 6973 2073 6f66 7477 6172 6520 6973  This software is
-00000030: 2072 656c 6561 7365 6420 756e 6465 7220   released under 
-00000040: 7468 6520 4d49 5420 4c69 6365 6e73 652e  the MIT License.
-00000050: 0a23 2068 7474 7073 3a2f 2f6f 7065 6e73  .# https://opens
-00000060: 6f75 7263 652e 6f72 672f 6c69 6365 6e73  ource.org/licens
-00000070: 6573 2f4d 4954 0a0a 0a66 726f 6d20 7569  es/MIT...from ui
-00000080: 646f 6d2e 646f 6d2e 6874 6d6c 656c 656d  dom.dom.htmlelem
-00000090: 656e 7420 696d 706f 7274 2048 544d 4c45  ent import HTMLE
-000000a0: 6c65 6d65 6e74 0a66 726f 6d20 7569 646f  lement.from uido
-000000b0: 6d2e 646f 6d2e 7372 632e 6874 6d6c 7461  m.dom.src.htmlta
-000000c0: 6773 2069 6d70 6f72 7420 7363 7269 7074  gs import script
-000000d0: 0a66 726f 6d20 7569 646f 6d2e 646f 6d2e  .from uidom.dom.
-000000e0: 7372 632e 7574 696c 732e 646f 6d5f 7574  src.utils.dom_ut
-000000f0: 696c 2069 6d70 6f72 7420 7261 770a 0a23  il import raw..#
-00000100: 2054 6865 2070 7572 6520 636c 6965 6e74   The pure client
-00000110: 2d73 6964 6520 636f 6465 2074 616b 656e  -side code taken
-00000120: 2066 726f 6d20 6874 7470 733a 2f2f 7374   from https://st
-00000130: 6163 6b6f 7665 7266 6c6f 772e 636f 6d2f  ackoverflow.com/
-00000140: 612f 3637 3237 3635 3835 0a23 2061 6e64  a/67276585.# and
-00000150: 2068 7474 7073 3a2f 2f73 7461 636b 6f76   https://stackov
-00000160: 6572 666c 6f77 2e63 6f6d 2f61 2f34 3837  erflow.com/a/487
-00000170: 3737 3438 310a 0a5f 5f61 6c6c 5f5f 203d  77481..__all__ =
-00000180: 205b 2258 436f 6d70 6f6e 656e 744a 5322   ["XComponentJS"
-00000190: 5d0a 0a0a 636c 6173 7320 5843 6f6d 706f  ]...class XCompo
-000001a0: 6e65 6e74 4a53 2848 544d 4c45 6c65 6d65  nentJS(HTMLEleme
-000001b0: 6e74 293a 0a20 2020 2022 2222 0a20 2020  nt):.    """.   
-000001c0: 2041 6461 7074 6f72 2063 6f6e 6365 7074   Adaptor concept
-000001d0: 2074 616b 656e 2066 726f 6d3a 0a20 2020   taken from:.   
-000001e0: 2020 2020 2068 7474 7073 3a2f 2f67 6974       https://git
-000001f0: 6875 622e 636f 6d2f 6d61 7465 7269 616c  hub.com/material
-00000200: 2d63 6f6d 706f 6e65 6e74 732f 6d61 7465  -components/mate
-00000210: 7269 616c 2d63 6f6d 706f 6e65 6e74 732d  rial-components-
-00000220: 7765 622f 7472 6565 2f39 3733 3664 6463  web/tree/9736ddc
-00000230: 6539 6331 3266 3534 3835 6537 3436 3938  e9c12f5485e74698
-00000240: 3432 3235 3931 3935 3638 3534 3165 3838  4225919568541e88
-00000250: 642f 7061 636b 6167 6573 2f6d 6463 2d62  d/packages/mdc-b
-00000260: 6173 650a 2020 2020 2222 220a 0a20 2020  ase.    """..   
-00000270: 2064 6566 205f 5f72 656e 6465 725f 5f28   def __render__(
-00000280: 7365 6c66 2c20 2a61 7267 732c 202a 2a6b  self, *args, **k
-00000290: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-000002a0: 6a73 203d 2022 2222 0a20 2020 2020 2020  js = """.       
-000002b0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-000002c0: 2020 6675 6e63 7469 6f6e 2067 7569 6447    function guidG
-000002d0: 656e 6572 6174 6f72 2829 207b 0a20 2020  enerator() {.   
-000002e0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000002f0: 7374 2053 3420 3d20 6675 6e63 7469 6f6e  st S4 = function
-00000300: 2028 297b 0a20 2020 2020 2020 2020 2020   (){.           
-00000310: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000320: 2828 2831 202b 204d 6174 682e 7261 6e64  (((1 + Math.rand
-00000330: 6f6d 2829 2920 2a20 3078 3130 3030 3029  om()) * 0x10000)
-00000340: 207c 2030 292e 746f 5374 7269 6e67 2831   | 0).toString(1
-00000350: 3629 2e73 7562 7374 7269 6e67 2831 293b  6).substring(1);
-00000360: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000370: 207d 3b0a 2020 2020 2020 2020 2020 2020   };.            
-00000380: 2020 2020 7265 7475 726e 2053 3428 2920      return S4() 
-00000390: 2b20 5334 2829 202b 2027 2d27 202b 2053  + S4() + '-' + S
-000003a0: 3428 2920 2b20 272d 2720 2b20 5334 2829  4() + '-' + S4()
-000003b0: 202b 2027 2d27 202b 2053 3428 2920 2b20   + '-' + S4() + 
-000003c0: 272d 2720 2b20 5334 2829 202b 2053 3428  '-' + S4() + S4(
-000003d0: 2920 2b20 5334 2829 3b0a 2020 2020 2020  ) + S4();.      
-000003e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-000003f0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-00000400: 7374 2074 6f43 616d 656c 203d 2028 7329  st toCamel = (s)
-00000410: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-00000420: 2020 2020 2020 7265 7475 726e 2073 2e72        return s.r
-00000430: 6570 6c61 6365 282f 285b 2d5f 5d5b 612d  eplace(/([-_][a-
-00000440: 7a5d 292f 6967 2c20 2824 3129 203d 3e20  z])/ig, ($1) => 
-00000450: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000460: 2020 2020 2020 7265 7475 726e 2024 312e        return $1.
-00000470: 746f 5570 7065 7243 6173 6528 290a 2020  toUpperCase().  
-00000480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000490: 2020 2020 2020 2e72 6570 6c61 6365 2827        .replace('
-000004a0: 2d27 2c20 2727 290a 2020 2020 2020 2020  -', '').        
-000004b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000004c0: 2e72 6570 6c61 6365 2827 5f27 2c20 2727  .replace('_', ''
-000004d0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-000004e0: 2020 207d 293b 0a20 2020 2020 2020 2020     });.         
-000004f0: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-00000500: 2020 636f 6e73 7420 6973 4a53 4f4e 203d    const isJSON =
-00000510: 2028 7374 7229 203d 3e20 7b0a 2020 2020   (str) => {.    
-00000520: 2020 2020 2020 2020 2020 2020 7472 7920              try 
-00000530: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00000540: 2020 2020 2020 7265 7475 726e 2028 4a53        return (JS
-00000550: 4f4e 2e70 6172 7365 2873 7472 2920 2626  ON.parse(str) &&
-00000560: 2021 2173 7472 293b 0a20 2020 2020 2020   !!str);.       
-00000570: 2020 2020 2020 2020 207d 2063 6174 6368           } catch
-00000580: 2028 6529 207b 0a20 2020 2020 2020 2020   (e) {.         
-00000590: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000005a0: 6e20 6661 6c73 653b 0a20 2020 2020 2020  n false;.       
-000005b0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
-000005c0: 2020 2020 2020 207d 0a0a 2020 2020 2020         }..      
-000005d0: 2020 2020 2020 636f 6e73 7420 6f62 7365        const obse
-000005e0: 7276 6541 7474 7243 6861 6e67 6520 3d20  rveAttrChange = 
-000005f0: 2865 6c2c 2061 7474 7269 6275 7465 4368  (el, attributeCh
-00000600: 616e 6765 6443 616c 6c62 6163 6b29 203d  angedCallback) =
-00000610: 3e20 7b0a 2020 2020 2020 2020 2020 2020  > {.            
-00000620: 2020 2020 7661 7220 6f62 7365 7276 6572      var observer
-00000630: 203d 206e 6577 204d 7574 6174 696f 6e4f   = new MutationO
-00000640: 6273 6572 7665 7228 6d75 7461 7469 6f6e  bserver(mutation
-00000650: 7320 3d3e 207b 0a20 2020 2020 2020 2020  s => {.         
-00000660: 2020 2020 2020 2020 2020 206d 7574 6174             mutat
-00000670: 696f 6e73 2e66 6f72 4561 6368 2828 6d75  ions.forEach((mu
-00000680: 7461 7469 6f6e 2920 3d3e 207b 0a20 2020  tation) => {.   
-00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006a0: 2020 2020 2069 6620 286d 7574 6174 696f       if (mutatio
-000006b0: 6e2e 7479 7065 203d 3d3d 2027 6174 7472  n.type === 'attr
-000006c0: 6962 7574 6573 2729 207b 0a20 2020 2020  ibutes') {.     
-000006d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006e0: 2020 2020 2020 206c 6574 206f 6c64 5661         let oldVa
-000006f0: 6c20 3d20 6d75 7461 7469 6f6e 2e6f 6c64  l = mutation.old
-00000700: 5661 6c75 653b 0a20 2020 2020 2020 2020  Value;.         
-00000710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000720: 2020 206c 6574 206e 6577 5661 6c20 3d20     let newVal = 
-00000730: 6d75 7461 7469 6f6e 2e74 6172 6765 742e  mutation.target.
-00000740: 6765 7441 7474 7269 6275 7465 286d 7574  getAttribute(mut
-00000750: 6174 696f 6e2e 6174 7472 6962 7574 654e  ation.attributeN
-00000760: 616d 6529 3b0a 2020 2020 2020 2020 2020  ame);.          
-00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000780: 2020 6174 7472 6962 7574 6543 6861 6e67    attributeChang
-00000790: 6564 4361 6c6c 6261 636b 286d 7574 6174  edCallback(mutat
-000007a0: 696f 6e2e 6174 7472 6962 7574 654e 616d  ion.attributeNam
-000007b0: 652c 206f 6c64 5661 6c2c 206e 6577 5661  e, oldVal, newVa
-000007c0: 6c29 3b0a 2020 2020 2020 2020 2020 2020  l);.            
-000007d0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-000007e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000007f0: 2020 7d29 3b0a 2020 2020 2020 2020 2020    });.          
-00000800: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
-00000810: 2020 2020 2020 2020 2020 6f62 7365 7276            observ
-00000820: 6572 2e6f 6273 6572 7665 2865 6c2c 207b  er.observe(el, {
-00000830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000840: 2020 2020 2061 7474 7269 6275 7465 733a       attributes:
-00000850: 2074 7275 652c 0a20 2020 2020 2020 2020   true,.         
-00000860: 2020 2020 2020 2020 2020 2061 7474 7269             attri
-00000870: 6275 7465 4f6c 6456 616c 7565 3a20 7472  buteOldValue: tr
-00000880: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
-00000890: 2020 2020 2020 2020 6174 7472 6962 7574          attribut
-000008a0: 6546 696c 7465 723a 205b 2769 6427 2c20  eFilter: ['id', 
-000008b0: 2763 6c61 7373 272c 2027 7374 796c 6527  'class', 'style'
-000008c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-000008d0: 2020 7d29 3b0a 2020 2020 2020 2020 2020    });.          
-000008e0: 2020 2020 2020 7265 7475 726e 206f 6273        return obs
-000008f0: 6572 7665 723b 0a20 2020 2020 2020 2020  erver;.         
-00000900: 2020 207d 0a0a 2020 2020 2020 2020 2020     }..          
-00000910: 2020 2828 2920 3d3e 207b 0a20 2020 2020    (() => {.     
-00000920: 2020 2020 2020 2020 2020 206c 6574 2073             let s
-00000930: 6f63 6b65 7420 3d20 7b7d 3b0a 2020 2020  ocket = {};.    
-00000940: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
-00000950: 6d65 7373 6167 6548 616e 646c 6572 203d  messageHandler =
-00000960: 207b 7d3b 0a20 2020 2020 2020 2020 2020   {};.           
-00000970: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00000980: 2020 2020 2020 636f 6e73 7420 7365 7455        const setU
-00000990: 704f 7247 6574 5765 6253 6f63 6b65 7420  pOrGetWebSocket 
-000009a0: 3d20 2865 6c65 6d65 6e74 4944 2c20 6d65  = (elementID, me
-000009b0: 7373 6167 6548 616e 646c 6572 2c20 656e  ssageHandler, en
-000009c0: 6450 6f69 6e74 203d 2027 7773 2729 203d  dPoint = 'ws') =
-000009d0: 3e20 7b0a 2020 2020 2020 2020 2020 2020  > {.            
-000009e0: 2020 2020 2020 2020 6966 2028 2173 6f63          if (!soc
-000009f0: 6b65 745b 6024 7b65 6e64 506f 696e 747d  ket[`${endPoint}
-00000a00: 605d 2920 7b0a 2020 2020 2020 2020 2020  `]) {.          
-00000a10: 2020 2020 2020 2020 2020 2020 2020 6c65                le
-00000a20: 7420 7572 6c20 3d20 6e65 7720 5552 4c28  t url = new URL(
-00000a30: 646f 6375 6d65 6e74 2e6c 6f63 6174 696f  document.locatio
-00000a40: 6e29 3b0a 2020 2020 2020 2020 2020 2020  n);.            
-00000a50: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
-00000a60: 7420 7773 5572 6c20 3d20 6024 7b75 726c  t wsUrl = `${url
-00000a70: 2e70 726f 746f 636f 6c2e 7265 706c 6163  .protocol.replac
-00000a80: 6528 2768 7474 7027 2c20 2777 7327 297d  e('http', 'ws')}
-00000a90: 2f2f 247b 7572 6c2e 686f 7374 6e61 6d65  //${url.hostname
-00000aa0: 7d3a 247b 7572 6c2e 706f 7274 7d2f 247b  }:${url.port}/${
-00000ab0: 656e 6450 6f69 6e74 7d60 3b0a 2020 2020  endPoint}`;.    
-00000ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ad0: 2020 2020 736f 636b 6574 5b60 247b 656e      socket[`${en
-00000ae0: 6450 6f69 6e74 7d60 5d20 3d20 6e65 7720  dPoint}`] = new 
-00000af0: 5765 6253 6f63 6b65 7428 7773 5572 6c29  WebSocket(wsUrl)
-00000b00: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00000b10: 2020 2020 2020 2020 2020 736f 636b 6574            socket
-00000b20: 5b60 247b 656e 6450 6f69 6e74 7d60 5d2e  [`${endPoint}`].
-00000b30: 6f6e 6f70 656e 203d 2028 6576 656e 7429  onopen = (event)
-00000b40: 203d 3e20 7b0a 2020 2020 2020 2020 2020   => {.          
-00000b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b60: 2020 636f 6e73 6f6c 652e 6c6f 6728 6063    console.log(`c
-00000b70: 6f6e 6e65 6374 6564 2074 6f20 247b 7773  onnected to ${ws
-00000b80: 5572 6c7d 6029 3b0a 2020 2020 2020 2020  Url}`);.        
-00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ba0: 2020 2020 736f 636b 6574 5b60 247b 656e      socket[`${en
-00000bb0: 6450 6f69 6e74 7d60 5d2e 7365 6e64 2860  dPoint}`].send(`
-00000bc0: 636f 6e6e 6563 7469 6f6e 2074 6f20 636c  connection to cl
-00000bd0: 6965 6e74 2075 7365 7220 247b 656c 656d  ient user ${elem
-00000be0: 656e 7449 447d 3a24 7b4a 534f 4e2e 7374  entID}:${JSON.st
-00000bf0: 7269 6e67 6966 7928 6576 656e 7429 7d60  ringify(event)}`
-00000c00: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00000c20: 6f6e 736f 6c65 2e6c 6f67 2865 7665 6e74  onsole.log(event
-00000c30: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-00000c40: 2020 2020 2020 2020 2020 207d 3b0a 2020             };.  
-00000c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c60: 2020 2020 2020 736f 636b 6574 5b60 247b        socket[`${
-00000c70: 656e 6450 6f69 6e74 7d60 5d2e 6f6e 636c  endPoint}`].oncl
-00000c80: 6f73 6520 3d20 2865 7665 6e74 2920 3d3e  ose = (event) =>
-00000c90: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00000cb0: 6f6e 736f 6c65 2e6c 6f67 2860 636f 6e6e  onsole.log(`conn
-00000cc0: 6563 7469 6f6e 2063 6c6f 7365 6420 746f  ection closed to
-00000cd0: 2024 7b65 6c65 6d65 6e74 4944 7d3a 247b   ${elementID}:${
-00000ce0: 7773 5572 6c7d 6029 3b0a 2020 2020 2020  wsUrl}`);.      
-00000cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d00: 2020 2020 2020 736f 636b 6574 5b60 247b        socket[`${
-00000d10: 656e 6450 6f69 6e74 7d60 5d20 3d20 6e75  endPoint}`] = nu
-00000d20: 6c6c 3b0a 2020 2020 2020 2020 2020 2020  ll;.            
-00000d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d40: 7365 7454 696d 656f 7574 280a 2020 2020  setTimeout(.    
-00000d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000d60: 2020 2020 2020 2020 2020 2020 2829 203d              () =
-00000d70: 3e20 7b73 6f63 6b65 745b 6024 7b65 6e64  > {socket[`${end
-00000d80: 506f 696e 747d 605d 203d 2073 6574 5570  Point}`] = setUp
-00000d90: 4f72 4765 7457 6562 536f 636b 6574 2865  OrGetWebSocket(e
-00000da0: 6c65 6d65 6e74 4944 2c20 6d65 7373 6167  lementID, messag
-00000db0: 6548 616e 646c 6572 2c20 656e 6450 6f69  eHandler, endPoi
-00000dc0: 6e74 297d 0a20 2020 2020 2020 2020 2020  nt)}.           
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000de0: 2020 2020 202c 2033 3030 293b 0a20 2020       , 300);.   
-00000df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e00: 2020 2020 2020 2020 2063 6c65 6172 5469           clearTi
-00000e10: 6d65 6f75 7428 293b 0a20 2020 2020 2020  meout();.       
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 207d 3b0a 2020 2020 2020 2020 2020 2020   };.            
-00000e40: 2020 2020 2020 2020 2020 2020 736f 636b              sock
-00000e50: 6574 5b60 247b 656e 6450 6f69 6e74 7d60  et[`${endPoint}`
-00000e60: 5d2e 6f6e 6572 726f 7220 3d20 2865 7665  ].onerror = (eve
-00000e70: 6e74 2920 3d3e 207b 0a20 2020 2020 2020  nt) => {.       
-00000e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e90: 2020 2020 2063 6f6e 736f 6c65 2e6c 6f67       console.log
-00000ea0: 2860 636f 6e6e 6563 7469 6f6e 2063 6c6f  (`connection clo
-00000eb0: 7365 6420 746f 2024 7b65 6c65 6d65 6e74  sed to ${element
-00000ec0: 4944 7d3a 247b 7773 5572 6c7d 2064 7565  ID}:${wsUrl} due
-00000ed0: 2074 6f20 6572 726f 7260 293b 0a20 2020   to error`);.   
-00000ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ef0: 2020 2020 207d 3b0a 2020 2020 2020 2020       };.        
-00000f00: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00000f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000f20: 2020 736f 636b 6574 5b60 247b 656e 6450    socket[`${endP
-00000f30: 6f69 6e74 7d60 5d2e 6f6e 6d65 7373 6167  oint}`].onmessag
-00000f40: 6520 3d20 286d 6573 7361 6765 2920 3d3e  e = (message) =>
-00000f50: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-00000f60: 2020 2020 2020 2020 2020 206c 6574 2064             let d
-00000f70: 6174 6120 3d20 6d65 7373 6167 652e 6461  ata = message.da
-00000f80: 7461 3b0a 2020 2020 2020 2020 2020 2020  ta;.            
-00000f90: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00000fa0: 6973 4a53 4f4e 2864 6174 6129 2920 7b0a  isJSON(data)) {.
-00000fb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000fc0: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00000fd0: 203d 204a 534f 4e2e 7061 7273 6528 6461   = JSON.parse(da
-00000fe0: 7461 293b 0a20 2020 2020 2020 2020 2020  ta);.           
-00000ff0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 2020 2020 2020 206d 6573 7361 6765 4861         messageHa
-00001020: 6e64 6c65 725b 6024 7b65 6c65 6d65 6e74  ndler[`${element
-00001030: 4944 7d60 5d28 6461 7461 293b 0a20 2020  ID}`](data);.   
-00001040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001050: 207d 3b0a 2020 2020 2020 2020 2020 2020   };.            
-00001060: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00001070: 6f63 6b65 745b 6024 7b65 6e64 506f 696e  ocket[`${endPoin
-00001080: 747d 605d 3b0a 2020 2020 2020 2020 2020  t}`];.          
-00001090: 2020 2020 2020 7d3b 0a20 2020 2020 2020        };.       
-000010a0: 2020 2020 2020 2020 2064 6f63 756d 656e           documen
-000010b0: 742e 7365 7455 704f 7247 6574 5765 6253  t.setUpOrGetWebS
-000010c0: 6f63 6b65 7420 3d20 7365 7455 704f 7247  ocket = setUpOrG
-000010d0: 6574 5765 6253 6f63 6b65 743b 0a20 2020  etWebSocket;.   
-000010e0: 2020 2020 2020 2020 2020 2020 2064 6f63               doc
-000010f0: 756d 656e 742e 6d65 7373 6167 6548 616e  ument.messageHan
-00001100: 646c 6572 203d 206d 6573 7361 6765 4861  dler = messageHa
-00001110: 6e64 6c65 723b 0a20 2020 2020 2020 2020  ndler;.         
-00001120: 2020 207d 2928 293b 0a0a 2020 2020 2020     })();..      
-00001130: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00001140: 2020 2064 6f63 756d 656e 742e 7175 6572     document.quer
-00001150: 7953 656c 6563 746f 7241 6c6c 2827 5b78  ySelectorAll('[x
-00001160: 2d63 6f6d 706f 6e65 6e74 5d27 292e 666f  -component]').fo
-00001170: 7245 6163 6828 636f 6d70 6f6e 656e 7420  rEach(component 
-00001180: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
-00001190: 2020 2020 2063 6f6e 7374 2063 6f6d 706f       const compo
-000011a0: 6e65 6e74 4e61 6d65 203d 2060 782d 247b  nentName = `x-${
-000011b0: 636f 6d70 6f6e 656e 742e 6765 7441 7474  component.getAtt
-000011c0: 7269 6275 7465 2827 782d 636f 6d70 6f6e  ribute('x-compon
-000011d0: 656e 7427 297d 603b 0a0a 2020 2020 2020  ent')}`;..      
-000011e0: 2020 2020 2020 2020 2020 636c 6173 7320            class 
-000011f0: 5843 6f6d 706f 6e65 6e74 2065 7874 656e  XComponent exten
-00001200: 6473 2048 544d 4c45 6c65 6d65 6e74 207b  ds HTMLElement {
-00001210: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001220: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00001230: 2020 2020 2020 2020 2020 636f 6e73 7472            constr
-00001240: 7563 746f 7228 2920 7b0a 2020 2020 2020  uctor() {.      
-00001250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001260: 2020 7375 7065 7228 293b 0a20 2020 2020    super();.     
-00001270: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00001280: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00001290: 2020 2020 2020 636f 6e6e 6563 7465 6443        connectedC
-000012a0: 616c 6c62 6163 6b28 2920 7b0a 2020 2020  allback() {.    
-000012b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012c0: 2020 2020 7661 7220 6973 5368 6164 6f77      var isShadow
-000012d0: 526f 6f74 203d 2063 6f6d 706f 6e65 6e74  Root = component
-000012e0: 2e67 6574 4174 7472 6962 7574 6528 2773  .getAttribute('s
-000012f0: 6861 646f 7772 6f6f 7427 293b 0a20 2020  hadowroot');.   
-00001300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001310: 2020 2020 2069 6620 2821 2169 7353 6861       if (!!isSha
-00001320: 646f 7752 6f6f 7429 7b0a 2020 2020 2020  dowRoot){.      
-00001330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001340: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001360: 2020 206c 6574 2073 6861 646f 7720 3d20     let shadow = 
-00001370: 7468 6973 2e61 7474 6163 6853 6861 646f  this.attachShado
-00001380: 7728 7b6d 6f64 653a 2027 6f70 656e 277d  w({mode: 'open'}
-00001390: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-000013a0: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-000013b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013c0: 2020 2020 2020 2020 2020 2020 6c65 7420              let 
-000013d0: 7465 6d70 6c61 7465 3b0a 2020 2020 2020  template;.      
-000013e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000013f0: 2020 2020 2020 6966 2028 636f 6d70 6f6e        if (compon
-00001400: 656e 742e 7461 674e 616d 6520 3d3d 3d20  ent.tagName === 
-00001410: 2754 454d 504c 4154 4527 297b 0a20 2020  'TEMPLATE'){.   
-00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001430: 2020 2020 2020 2020 2020 2020 2074 656d               tem
-00001440: 706c 6174 6520 3d20 636f 6d70 6f6e 656e  plate = componen
-00001450: 743b 0a20 2020 2020 2020 2020 2020 2020  t;.             
-00001460: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00001470: 2065 6c73 6520 7b0a 2020 2020 2020 2020   else {.        
-00001480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001490: 2020 2020 2020 2020 7465 6d70 6c61 7465          template
-000014a0: 203d 2063 6f6d 706f 6e65 6e74 2e67 6574   = component.get
-000014b0: 456c 656d 656e 7473 4279 5461 674e 616d  ElementsByTagNam
-000014c0: 6528 2774 656d 706c 6174 6527 295b 305d  e('template')[0]
-000014d0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-000014e0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-000014f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001500: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001510: 2874 656d 706c 6174 653f 2e63 6f6e 7465  (template?.conte
-00001520: 6e74 2e63 6869 6c64 456c 656d 656e 7443  nt.childElementC
-00001530: 6f75 6e74 2920 7b0a 2020 2020 2020 2020  ount) {.        
-00001540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001550: 2020 2020 2020 2020 7368 6164 6f77 2e61          shadow.a
-00001560: 7070 656e 6443 6869 6c64 2874 656d 706c  ppendChild(templ
-00001570: 6174 652e 636f 6e74 656e 742e 636c 6f6e  ate.content.clon
-00001580: 654e 6f64 6528 7472 7565 2929 3b0a 2020  eNode(true));.  
-00001590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015a0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015c0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-000015d0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000015e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000015f0: 2020 206c 6574 2073 6c6f 7420 3d20 646f     let slot = do
-00001600: 6375 6d65 6e74 2e63 7265 6174 6545 6c65  cument.createEle
-00001610: 6d65 6e74 2827 736c 6f74 2729 3b0a 2020  ment('slot');.  
-00001620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001630: 2020 2020 2020 2020 2020 2020 2020 7368                sh
-00001640: 6164 6f77 2e61 7070 656e 6443 6869 6c64  adow.appendChild
-00001650: 2873 6c6f 7429 3b0a 2020 2020 2020 2020  (slot);.        
-00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001670: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00001680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001690: 2020 2020 2020 7468 6973 2e73 6861 646f        this.shado
-000016a0: 7720 3d20 7368 6164 6f77 3b0a 2020 2020  w = shadow;.    
-000016b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016c0: 2020 2020 2020 2020 7468 6973 2e63 6865          this.che
-000016d0: 636b 4964 2829 3b0a 2020 2020 2020 2020  ckId();.        
-000016e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000016f0: 2020 2020 646f 6375 6d65 6e74 2e61 6464      document.add
-00001700: 4576 656e 744c 6973 7465 6e65 7228 2761  EventListener('a
-00001710: 6c70 696e 653a 696e 6974 6961 6c69 7a65  lpine:initialize
-00001720: 6427 2c20 2829 203d 3e20 7b0a 2020 2020  d', () => {.    
-00001730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001740: 2020 2020 2020 2020 2020 2020 416c 7069              Alpi
-00001750: 6e65 2e69 6e69 7454 7265 6528 7468 6973  ne.initTree(this
-00001760: 2e73 6861 646f 7729 3b0a 2020 2020 2020  .shadow);.      
-00001770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001780: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-000017b0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017d0: 2020 2020 2069 6620 2821 7468 6973 2e69       if (!this.i
-000017e0: 6429 7b0a 2020 2020 2020 2020 2020 2020  d){.            
-000017f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001800: 7468 6973 2e61 7070 656e 6428 636f 6d70  this.append(comp
-00001810: 6f6e 656e 742e 636f 6e74 656e 742e 636c  onent.content.cl
-00001820: 6f6e 654e 6f64 6528 7472 7565 2929 3b0a  oneNode(true));.
-00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001840: 2020 2020 2020 2020 2020 2020 7468 6973              this
-00001850: 2e63 6865 636b 4964 2829 3b0a 2020 2020  .checkId();.    
-00001860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001870: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00001880: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00001890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018a0: 2020 2020 2020 2074 6869 732e 6164 6445         this.addE
-000018b0: 7665 6e74 4c69 7374 656e 6572 2827 616c  ventListener('al
-000018c0: 7069 6e65 3a69 6e69 7427 2c20 2829 203d  pine:init', () =
-000018d0: 3e20 7b0a 2020 2020 2020 2020 2020 2020  > {.            
-000018e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000018f0: 416c 7069 6e65 2e64 6174 6128 2270 6172  Alpine.data("par
-00001900: 656e 7445 6c65 6d65 6e74 4461 7461 222c  entElementData",
-00001910: 2028 2920 3d3e 2028 7b0a 2020 2020 2020   () => ({.      
-00001920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001930: 2020 2020 2020 2020 2020 2e2e 2e74 6869            ...thi
-00001940: 732e 6461 7461 2829 0a20 2020 2020 2020  s.data().       
-00001950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001960: 2020 2020 207d 2929 0a20 2020 2020 2020       })).       
-00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001980: 207d 293b 0a20 2020 2020 2020 2020 2020   });.           
-00001990: 2020 2020 2020 2020 2020 2020 200a 2020               .  
-000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019b0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000019d0: 2020 2020 2074 6869 732e 6461 7461 4361       this.dataCa
-000019e0: 6c6c 6261 636b 203d 2074 6869 732e 6461  llback = this.da
-000019f0: 7461 4361 6c6c 6261 636b 2e62 696e 6428  taCallback.bind(
-00001a00: 7468 6973 293b 2020 2020 2020 2020 2020  this);          
-00001a10: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00001a20: 2020 2020 2020 2020 2020 2020 202f 2f20               // 
-00001a30: 3c6d 792d 6469 7620 6163 7469 7665 3d22  <my-div active="
-00001a40: 7472 7565 222c 2064 6174 612d 7461 7267  true", data-targ
-00001a50: 6574 3d22 2361 6363 6f72 6469 616e 223e  et="#accordian">
-00001a60: 3c2f 6d79 2d64 6976 3e0a 2020 2020 2020  </my-div>.      
-00001a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a80: 2020 2f2f 2065 7861 6d70 6c65 3a20 666f    // example: fo
-00001a90: 7220 7365 7474 696e 6720 7570 2020 6e61  r setting up  na
-00001aa0: 6d65 3d22 636f 6f6c 2d64 7564 6522 2076  me="cool-dude" v
-00001ab0: 616c 7565 2061 7320 7468 6973 2e6e 616d  alue as this.nam
-00001ac0: 6520 7661 6c75 650a 2020 2020 2020 2020  e value.        
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 6c65 7420 5f64 6174 6153 7461 7465 203d  let _dataState =
-00001af0: 2074 6869 732e 6461 7461 2829 3b0a 0a20   this.data();.. 
-00001b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b10: 2020 2020 2020 202f 2f20 666f 7220 7365         // for se
-00001b20: 7474 696e 6720 7570 2064 6174 612d 7461  tting up data-ta
-00001b30: 7267 6574 2076 616c 7565 0a20 2020 2020  rget value.     
-00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b50: 2020 206c 6574 205f 6461 7461 5461 7267     let _dataTarg
-00001b60: 6574 203d 2074 6869 733f 2e64 6174 6173  et = this?.datas
-00001b70: 6574 2e74 6172 6765 7420 7c7c 207b 7d3b  et.target || {};
-00001b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001b90: 2020 2020 2020 2020 2069 6620 2869 734a           if (isJ
-00001ba0: 534f 4e28 5f64 6174 6154 6172 6765 7429  SON(_dataTarget)
-00001bb0: 297b 0a20 2020 2020 2020 2020 2020 2020  ){.             
-00001bc0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-00001bd0: 6461 7461 5461 7267 6574 203d 204a 534f  dataTarget = JSO
-00001be0: 4e2e 7061 7273 6528 5f64 6174 6154 6172  N.parse(_dataTar
-00001bf0: 6765 7429 3b0a 2020 2020 2020 2020 2020  get);.          
-00001c00: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
+00000000: 2f2f 2043 6f70 7972 6967 6874 2028 6329  // Copyright (c)
+00000010: 2032 3032 3320 5569 444f 4d0a 2f2f 200a   2023 UiDOM.// .
+00000020: 2f2f 2054 6869 7320 736f 6674 7761 7265  // This software
+00000030: 2069 7320 7265 6c65 6173 6564 2075 6e64   is released und
+00000040: 6572 2074 6865 204d 4954 204c 6963 656e  er the MIT Licen
+00000050: 7365 2e0a 2f2f 2068 7474 7073 3a2f 2f6f  se..// https://o
+00000060: 7065 6e73 6f75 7263 652e 6f72 672f 6c69  pensource.org/li
+00000070: 6365 6e73 6573 2f4d 4954 0a0a 0a66 756e  censes/MIT...fun
+00000080: 6374 696f 6e20 6775 6964 4765 6e65 7261  ction guidGenera
+00000090: 746f 7228 2920 7b0a 2020 2020 636f 6e73  tor() {.    cons
+000000a0: 7420 5334 203d 2066 756e 6374 696f 6e20  t S4 = function 
+000000b0: 2829 7b0a 2020 2020 2020 2020 7265 7475  (){.        retu
+000000c0: 726e 2028 2828 3120 2b20 4d61 7468 2e72  rn (((1 + Math.r
+000000d0: 616e 646f 6d28 2929 202a 2030 7831 3030  andom()) * 0x100
+000000e0: 3030 2920 7c20 3029 2e74 6f53 7472 696e  00) | 0).toStrin
+000000f0: 6728 3136 292e 7375 6273 7472 696e 6728  g(16).substring(
+00000100: 3129 3b0a 2020 2020 7d3b 0a20 2020 2072  1);.    };.    r
+00000110: 6574 7572 6e20 5334 2829 202b 2053 3428  eturn S4() + S4(
+00000120: 2920 2b20 272d 2720 2b20 5334 2829 202b  ) + '-' + S4() +
+00000130: 2027 2d27 202b 2053 3428 2920 2b20 272d   '-' + S4() + '-
+00000140: 2720 2b20 5334 2829 202b 2027 2d27 202b  ' + S4() + '-' +
+00000150: 2053 3428 2920 2b20 5334 2829 202b 2053   S4() + S4() + S
+00000160: 3428 293b 0a7d 0a0a 636f 6e73 7420 746f  4();.}..const to
+00000170: 4361 6d65 6c20 3d20 2873 2920 3d3e 207b  Camel = (s) => {
+00000180: 0a20 2020 2072 6574 7572 6e20 732e 7265  .    return s.re
+00000190: 706c 6163 6528 2f28 5b2d 5f5d 5b61 2d7a  place(/([-_][a-z
+000001a0: 5d29 2f69 672c 2028 2431 2920 3d3e 207b  ])/ig, ($1) => {
+000001b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000001c0: 2431 2e74 6f55 7070 6572 4361 7365 2829  $1.toUpperCase()
+000001d0: 0a20 2020 2020 2020 2020 2020 202e 7265  .            .re
+000001e0: 706c 6163 6528 272d 272c 2027 2729 0a20  place('-', ''). 
+000001f0: 2020 2020 2020 2020 2020 202e 7265 706c             .repl
+00000200: 6163 6528 275f 272c 2027 2729 3b0a 2020  ace('_', '');.  
+00000210: 2020 7d29 3b0a 7d0a 0a63 6f6e 7374 2069    });.}..const i
+00000220: 734a 534f 4e20 3d20 2873 7472 2920 3d3e  sJSON = (str) =>
+00000230: 207b 0a20 2020 2074 7279 207b 0a20 2020   {.    try {.   
+00000240: 2020 2020 2072 6574 7572 6e20 284a 534f       return (JSO
+00000250: 4e2e 7061 7273 6528 7374 7229 2026 2620  N.parse(str) && 
+00000260: 2121 7374 7229 3b0a 2020 2020 7d20 6361  !!str);.    } ca
+00000270: 7463 6820 2865 2920 7b0a 2020 2020 2020  tch (e) {.      
+00000280: 2020 7265 7475 726e 2066 616c 7365 3b0a    return false;.
+00000290: 2020 2020 7d0a 7d0a 0a63 6f6e 7374 206f      }.}..const o
+000002a0: 6273 6572 7665 4174 7472 4368 616e 6765  bserveAttrChange
+000002b0: 203d 2028 656c 2c20 6174 7472 6962 7574   = (el, attribut
+000002c0: 6543 6861 6e67 6564 4361 6c6c 6261 636b  eChangedCallback
+000002d0: 2920 3d3e 207b 0a20 2020 2076 6172 206f  ) => {.    var o
+000002e0: 6273 6572 7665 7220 3d20 6e65 7720 4d75  bserver = new Mu
+000002f0: 7461 7469 6f6e 4f62 7365 7276 6572 286d  tationObserver(m
+00000300: 7574 6174 696f 6e73 203d 3e20 7b0a 2020  utations => {.  
+00000310: 2020 2020 2020 6d75 7461 7469 6f6e 732e        mutations.
+00000320: 666f 7245 6163 6828 286d 7574 6174 696f  forEach((mutatio
+00000330: 6e29 203d 3e20 7b0a 2020 2020 2020 2020  n) => {.        
+00000340: 2020 2020 6966 2028 6d75 7461 7469 6f6e      if (mutation
+00000350: 2e74 7970 6520 3d3d 3d20 2761 7474 7269  .type === 'attri
+00000360: 6275 7465 7327 2920 7b0a 2020 2020 2020  butes') {.      
+00000370: 2020 2020 2020 2020 2020 6c65 7420 6f6c            let ol
+00000380: 6456 616c 203d 206d 7574 6174 696f 6e2e  dVal = mutation.
+00000390: 6f6c 6456 616c 7565 3b0a 2020 2020 2020  oldValue;.      
+000003a0: 2020 2020 2020 2020 2020 6c65 7420 6e65            let ne
+000003b0: 7756 616c 203d 206d 7574 6174 696f 6e2e  wVal = mutation.
+000003c0: 7461 7267 6574 2e67 6574 4174 7472 6962  target.getAttrib
+000003d0: 7574 6528 6d75 7461 7469 6f6e 2e61 7474  ute(mutation.att
+000003e0: 7269 6275 7465 4e61 6d65 293b 0a20 2020  ributeName);.   
+000003f0: 2020 2020 2020 2020 2020 2020 2061 7474               att
+00000400: 7269 6275 7465 4368 616e 6765 6443 616c  ributeChangedCal
+00000410: 6c62 6163 6b28 6d75 7461 7469 6f6e 2e61  lback(mutation.a
+00000420: 7474 7269 6275 7465 4e61 6d65 2c20 6f6c  ttributeName, ol
+00000430: 6456 616c 2c20 6e65 7756 616c 293b 0a20  dVal, newVal);. 
+00000440: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00000450: 2020 2020 207d 293b 0a20 2020 207d 293b       });.    });
+00000460: 0a20 2020 206f 6273 6572 7665 722e 6f62  .    observer.ob
+00000470: 7365 7276 6528 656c 2c20 7b0a 2020 2020  serve(el, {.    
+00000480: 2020 2020 6174 7472 6962 7574 6573 3a20      attributes: 
+00000490: 7472 7565 2c0a 2020 2020 2020 2020 6174  true,.        at
+000004a0: 7472 6962 7574 654f 6c64 5661 6c75 653a  tributeOldValue:
+000004b0: 2074 7275 652c 0a20 2020 2020 2020 2061   true,.        a
+000004c0: 7474 7269 6275 7465 4669 6c74 6572 3a20  ttributeFilter: 
+000004d0: 5b27 6964 272c 2027 636c 6173 7327 2c20  ['id', 'class', 
+000004e0: 2773 7479 6c65 275d 0a20 2020 207d 293b  'style'].    });
+000004f0: 0a20 2020 2072 6574 7572 6e20 6f62 7365  .    return obse
+00000500: 7276 6572 3b0a 7d0a 0a28 2829 203d 3e20  rver;.}..(() => 
+00000510: 7b0a 2020 2020 6c65 7420 736f 636b 6574  {.    let socket
+00000520: 203d 207b 7d3b 0a20 2020 206c 6574 206d   = {};.    let m
+00000530: 6573 7361 6765 4861 6e64 6c65 7220 3d20  essageHandler = 
+00000540: 7b7d 3b0a 2020 2020 6c65 7420 636f 6e6e  {};.    let conn
+00000550: 6563 7469 6f6e 5f72 6573 6f6c 7665 7273  ection_resolvers
+00000560: 203d 207b 7d3b 0a20 2020 206c 6574 2077   = {};.    let w
+00000570: 6169 7446 6f72 436f 6e6e 6563 7469 6f6e  aitForConnection
+00000580: 203d 207b 7d0a 2020 2020 2f2f 2063 6f6e   = {}.    // con
+00000590: 6e65 6374 696f 6e5f 7265 736f 6c76 6572  nection_resolver
+000005a0: 7320 6973 2074 616b 656e 2066 726f 6d20  s is taken from 
+000005b0: 6874 7470 733a 2f2f 7374 6163 6b6f 7665  https://stackove
+000005c0: 7266 6c6f 772e 636f 6d2f 612f 3638 3535  rflow.com/a/6855
+000005d0: 3935 3539 0a20 2020 200a 2020 2020 636f  9559.    .    co
+000005e0: 6e73 7420 7365 7455 704f 7247 6574 5765  nst setUpOrGetWe
+000005f0: 6253 6f63 6b65 7420 3d20 2865 6c65 6d65  bSocket = (eleme
+00000600: 6e74 4944 2c20 6d65 7373 6167 6548 616e  ntID, messageHan
+00000610: 646c 6572 2c20 656e 6450 6f69 6e74 203d  dler, endPoint =
+00000620: 2027 2f77 7327 2920 3d3e 207b 0a20 2020   '/ws') => {.   
+00000630: 2020 2020 2069 6620 2821 736f 636b 6574       if (!socket
+00000640: 5b60 247b 656e 6450 6f69 6e74 7d60 5d29  [`${endPoint}`])
+00000650: 207b 0a20 2020 2020 2020 2020 2020 206c   {.            l
+00000660: 6574 2075 726c 203d 206e 6577 2055 524c  et url = new URL
+00000670: 2864 6f63 756d 656e 742e 6c6f 6361 7469  (document.locati
+00000680: 6f6e 293b 0a20 2020 2020 2020 2020 2020  on);.           
+00000690: 2063 6f6e 7374 2077 7355 726c 203d 2060   const wsUrl = `
+000006a0: 247b 7572 6c2e 7072 6f74 6f63 6f6c 2e72  ${url.protocol.r
+000006b0: 6570 6c61 6365 2827 6874 7470 272c 2027  eplace('http', '
+000006c0: 7773 2729 7d2f 2f24 7b75 726c 2e68 6f73  ws')}//${url.hos
+000006d0: 746e 616d 657d 3a24 7b75 726c 2e70 6f72  tname}:${url.por
+000006e0: 747d 247b 656e 6450 6f69 6e74 7d60 3b0a  t}${endPoint}`;.
+000006f0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00000700: 6f6c 652e 6c6f 6728 6063 7265 6174 696e  ole.log(`creatin
+00000710: 6720 6e65 7720 5765 6253 6f63 6b65 7420  g new WebSocket 
+00000720: 496e 7374 616e 6365 2074 6f20 247b 7773  Instance to ${ws
+00000730: 5572 6c7d 6029 3b0a 2020 2020 2020 2020  Url}`);.        
+00000740: 2020 2020 736f 636b 6574 5b60 247b 656e      socket[`${en
+00000750: 6450 6f69 6e74 7d60 5d20 3d20 6e65 7720  dPoint}`] = new 
+00000760: 5765 6253 6f63 6b65 7428 7773 5572 6c29  WebSocket(wsUrl)
+00000770: 3b0a 2020 2020 2020 2020 2020 2020 6966  ;.            if
+00000780: 2028 2163 6f6e 6e65 6374 696f 6e5f 7265   (!connection_re
+00000790: 736f 6c76 6572 735b 6024 7b65 6e64 506f  solvers[`${endPo
+000007a0: 696e 747d 605d 297b 0a20 2020 2020 2020  int}`]){.       
+000007b0: 2020 2020 2020 2020 2063 6f6e 6e65 6374           connect
+000007c0: 696f 6e5f 7265 736f 6c76 6572 735b 6024  ion_resolvers[`$
+000007d0: 7b65 6e64 506f 696e 747d 605d 203d 205b  {endPoint}`] = [
+000007e0: 5d3b 0a20 2020 2020 2020 2020 2020 207d  ];.            }
+000007f0: 0a20 2020 2020 2020 2020 2020 200a 2020  .            .  
+00000800: 2020 2020 2020 2020 2020 6966 2028 2177            if (!w
+00000810: 6169 7446 6f72 436f 6e6e 6563 7469 6f6e  aitForConnection
+00000820: 5b60 247b 656e 6450 6f69 6e74 7d60 5d29  [`${endPoint}`])
+00000830: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00000840: 2020 7761 6974 466f 7243 6f6e 6e65 6374    waitForConnect
+00000850: 696f 6e5b 6024 7b65 6e64 506f 696e 747d  ion[`${endPoint}
+00000860: 605d 203d 2028 2920 3d3e 207b 0a20 2020  `] = () => {.   
+00000870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000880: 2072 6574 7572 6e20 6e65 7720 5072 6f6d   return new Prom
+00000890: 6973 6528 2872 6573 6f6c 7665 2c20 7265  ise((resolve, re
+000008a0: 6a65 6374 2920 3d3e 207b 0a20 2020 2020  ject) => {.     
+000008b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000008c0: 2020 2063 6f6e 6e65 6374 696f 6e5f 7265     connection_re
+000008d0: 736f 6c76 6572 735b 6024 7b65 6e64 506f  solvers[`${endPo
+000008e0: 696e 747d 605d 2e70 7573 6828 7b72 6573  int}`].push({res
+000008f0: 6f6c 7665 2c20 7265 6a65 6374 7d29 3b0a  olve, reject});.
+00000900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000910: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
+00000920: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00000930: 2020 2020 2020 7d0a 0a20 2020 2020 2020        }..       
+00000940: 2020 2020 2073 6f63 6b65 745b 6024 7b65       socket[`${e
+00000950: 6e64 506f 696e 747d 605d 2e61 6464 4576  ndPoint}`].addEv
+00000960: 656e 744c 6973 7465 6e65 7228 276f 7065  entListener('ope
+00000970: 6e27 2c20 2829 203d 3e20 7b0a 2020 2020  n', () => {.    
+00000980: 2020 2020 2020 2020 2020 2020 636f 6e6e              conn
+00000990: 6563 7469 6f6e 5f72 6573 6f6c 7665 7273  ection_resolvers
+000009a0: 5b60 247b 656e 6450 6f69 6e74 7d60 5d2e  [`${endPoint}`].
+000009b0: 666f 7245 6163 6828 7220 3d3e 2072 2e72  forEach(r => r.r
+000009c0: 6573 6f6c 7665 2829 290a 2020 2020 2020  esolve()).      
+000009d0: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
+000009e0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+000009f0: 2020 2073 6f63 6b65 745b 6024 7b65 6e64     socket[`${end
+00000a00: 506f 696e 747d 605d 2e6f 6e6f 7065 6e20  Point}`].onopen 
+00000a10: 3d20 2865 7665 6e74 2920 3d3e 207b 0a20  = (event) => {. 
+00000a20: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00000a30: 6f6e 736f 6c65 2e6c 6f67 2860 636f 6e6e  onsole.log(`conn
+00000a40: 6563 7465 6420 746f 2024 7b77 7355 726c  ected to ${wsUrl
+00000a50: 7d60 293b 0a20 2020 2020 2020 2020 2020  }`);.           
+00000a60: 2020 2020 2073 6f63 6b65 745b 6024 7b65       socket[`${e
+00000a70: 6e64 506f 696e 747d 605d 2e73 656e 6428  ndPoint}`].send(
+00000a80: 6063 6f6e 6e65 6374 696f 6e20 6f70 656e  `connection open
+00000a90: 2074 6f20 636c 6965 6e74 2065 6c65 6d65   to client eleme
+00000aa0: 6e74 2024 7b65 6c65 6d65 6e74 4944 7d3a  nt ${elementID}:
+00000ab0: 247b 4a53 4f4e 2e73 7472 696e 6769 6679  ${JSON.stringify
+00000ac0: 2865 7665 6e74 297d 6029 3b0a 2020 2020  (event)}`);.    
+00000ad0: 2020 2020 2020 2020 7d3b 0a20 2020 2020          };.     
+00000ae0: 2020 2020 2020 2073 6f63 6b65 745b 6024         socket[`$
+00000af0: 7b65 6e64 506f 696e 747d 605d 2e6f 6e63  {endPoint}`].onc
+00000b00: 6c6f 7365 203d 2028 6576 656e 7429 203d  lose = (event) =
+00000b10: 3e20 7b0a 2020 2020 2020 2020 2020 2020  > {.            
+00000b20: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
+00000b30: 6063 6f6e 6e65 6374 696f 6e20 636c 6f73  `connection clos
+00000b40: 6564 2074 6f20 247b 656c 656d 656e 7449  ed to ${elementI
+00000b50: 447d 3a20 247b 7773 5572 6c7d 6029 3b0a  D}: ${wsUrl}`);.
+00000b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b70: 736f 636b 6574 5b60 247b 656e 6450 6f69  socket[`${endPoi
+00000b80: 6e74 7d60 5d20 3d20 6e75 6c6c 3b0a 2020  nt}`] = null;.  
+00000b90: 2020 2020 2020 2020 2020 2020 2020 7469                ti
+00000ba0: 6d65 4f75 7420 3d20 7365 7454 696d 656f  meOut = setTimeo
+00000bb0: 7574 280a 2020 2020 2020 2020 2020 2020  ut(.            
+00000bc0: 2020 2020 2020 2020 2829 203d 3e20 7b73          () => {s
+00000bd0: 6f63 6b65 745b 6024 7b65 6e64 506f 696e  ocket[`${endPoin
+00000be0: 747d 605d 203d 2073 6574 5570 4f72 4765  t}`] = setUpOrGe
+00000bf0: 7457 6562 536f 636b 6574 2865 6c65 6d65  tWebSocket(eleme
+00000c00: 6e74 4944 2c20 6d65 7373 6167 6548 616e  ntID, messageHan
+00000c10: 646c 6572 2c20 656e 6450 6f69 6e74 297d  dler, endPoint)}
+00000c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000c30: 2020 2020 202c 2033 3030 293b 0a20 2020       , 300);.   
+00000c40: 2020 2020 2020 2020 2020 2020 2063 6c65               cle
+00000c50: 6172 5469 6d65 6f75 7428 7469 6d65 4f75  arTimeout(timeOu
+00000c60: 7429 3b0a 2020 2020 2020 2020 2020 2020  t);.            
+00000c70: 7d3b 0a20 2020 2020 2020 2020 2020 2073  };.            s
+00000c80: 6f63 6b65 745b 6024 7b65 6e64 506f 696e  ocket[`${endPoin
+00000c90: 747d 605d 2e6f 6e65 7272 6f72 203d 2028  t}`].onerror = (
+00000ca0: 6576 656e 7429 203d 3e20 7b0a 2020 2020  event) => {.    
+00000cb0: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00000cc0: 6f6c 652e 6c6f 6728 6063 6f6e 6e65 6374  ole.log(`connect
+00000cd0: 696f 6e20 636c 6f73 6564 2074 6f20 247b  ion closed to ${
+00000ce0: 656c 656d 656e 7449 447d 3a24 7b77 7355  elementID}:${wsU
+00000cf0: 726c 7d20 6475 6520 746f 2065 7272 6f72  rl} due to error
+00000d00: 207b 6576 656e 747d 6029 3b0a 2020 2020   {event}`);.    
+00000d10: 2020 2020 2020 2020 7d3b 0a20 2020 2020          };.     
+00000d20: 2020 207d 0a20 2020 2020 2020 2073 6f63     }.        soc
+00000d30: 6b65 745b 6024 7b65 6e64 506f 696e 747d  ket[`${endPoint}
+00000d40: 605d 2e6f 6e6d 6573 7361 6765 203d 2028  `].onmessage = (
+00000d50: 6d65 7373 6167 6529 203d 3e20 7b0a 2020  message) => {.  
+00000d60: 2020 2020 2020 2020 2020 6c65 7420 6461            let da
+00000d70: 7461 203d 206d 6573 7361 6765 2e64 6174  ta = message.dat
+00000d80: 613b 0a20 2020 2020 2020 2020 2020 2069  a;.            i
+00000d90: 6620 2869 734a 534f 4e28 6d65 7373 6167  f (isJSON(messag
+00000da0: 6529 2920 7b0a 2020 2020 2020 2020 2020  e)) {.          
+00000db0: 2020 2020 2020 6461 7461 203d 204a 534f        data = JSO
+00000dc0: 4e2e 7061 7273 6528 6461 7461 293b 0a20  N.parse(data);. 
+00000dd0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00000de0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00000df0: 4861 6e64 6c65 725b 6024 7b65 6c65 6d65  Handler[`${eleme
+00000e00: 6e74 4944 7d60 5d28 6461 7461 293b 0a20  ntID}`](data);. 
+00000e10: 2020 2020 2020 207d 3b0a 2020 2020 2020         };.      
+00000e20: 2020 7265 7475 726e 2073 6f63 6b65 745b    return socket[
+00000e30: 6024 7b65 6e64 506f 696e 747d 605d 3b0a  `${endPoint}`];.
+00000e40: 2020 2020 7d3b 0a20 2020 2064 6f63 756d      };.    docum
+00000e50: 656e 742e 7365 7455 704f 7247 6574 5765  ent.setUpOrGetWe
+00000e60: 6253 6f63 6b65 7420 3d20 7365 7455 704f  bSocket = setUpO
+00000e70: 7247 6574 5765 6253 6f63 6b65 743b 0a20  rGetWebSocket;. 
+00000e80: 2020 2064 6f63 756d 656e 742e 6d65 7373     document.mess
+00000e90: 6167 6548 616e 646c 6572 203d 206d 6573  ageHandler = mes
+00000ea0: 7361 6765 4861 6e64 6c65 723b 0a20 2020  sageHandler;.   
+00000eb0: 2064 6f63 756d 656e 742e 7761 6974 466f   document.waitFo
+00000ec0: 7243 6f6e 6e65 6374 696f 6e20 3d20 7761  rConnection = wa
+00000ed0: 6974 466f 7243 6f6e 6e65 6374 696f 6e3b  itForConnection;
+00000ee0: 0a7d 2928 293b 0a0a 0a2f 2f20 7461 6b65  .})();...// take
+00000ef0: 6e20 6672 6f6d 2068 7474 7073 3a2f 2f73  n from https://s
+00000f00: 7461 636b 6f76 6572 666c 6f77 2e63 6f6d  tackoverflow.com
+00000f10: 2f61 2f37 3339 3536 3135 350a 2f2f 2061  /a/73956155.// a
+00000f20: 6e64 2068 7474 7073 3a2f 2f67 6974 6875  nd https://githu
+00000f30: 622e 636f 6d2f 616c 7069 6e65 6a73 2f61  b.com/alpinejs/a
+00000f40: 6c70 696e 652f 626c 6f62 2f30 6133 3630  lpine/blob/0a360
+00000f50: 6662 6165 3731 3266 6436 6266 3938 6233  fbae712fd6bf98b3
+00000f60: 3832 3134 3063 6464 3761 6633 6463 3639  82140cdd7af3dc69
+00000f70: 3634 342f 7061 636b 6167 6573 2f75 692f  644/packages/ui/
+00000f80: 7372 632f 6d65 6e75 2e6a 730a 2f2f 2064  src/menu.js.// d
+00000f90: 6f63 756d 656e 742e 6164 6445 7665 6e74  ocument.addEvent
+00000fa0: 4c69 7374 656e 6572 2822 616c 7069 6e65  Listener("alpine
+00000fb0: 3a69 6e69 7422 2c20 2829 203d 3e20 7b0a  :init", () => {.
+00000fc0: 2f2f 2020 2020 2077 696e 646f 772e 416c  //     window.Al
+00000fd0: 7069 6e65 2e64 6972 6563 7469 7665 2827  pine.directive('
+00000fe0: 7569 646f 6d27 2c20 2865 6c2c 2064 6972  uidom', (el, dir
+00000ff0: 6563 7469 7665 2920 3d3e 207b 0a2f 2f20  ective) => {.// 
+00001000: 2020 2020 2020 2020 7769 6e64 6f77 2e41          window.A
+00001010: 6c70 696e 652e 6269 6e64 2865 6c2c 207b  lpine.bind(el, {
+00001020: 0a2f 2f20 2020 2020 2020 2020 2778 2d64  .//         'x-d
+00001030: 6174 6127 2829 207b 0a2f 2f20 2020 2020  ata'() {.//     
+00001040: 2020 2020 2020 2020 7265 7475 726e 2065          return e
+00001050: 6c2e 7061 7265 6e74 456c 656d 656e 742e  l.parentElement.
+00001060: 6461 7461 2829 3b0a 2f2f 2020 2020 2020  data();.//      
+00001070: 2020 207d 0a2f 2f20 2020 2020 2020 2020     }.//         
+00001080: 7d29 0a2f 2f20 2020 2020 7d29 200a 2f2f  }).//     }) .//
+00001090: 207d 293b 0a0a 0a64 6f63 756d 656e 742e   });...document.
+000010a0: 7175 6572 7953 656c 6563 746f 7241 6c6c  querySelectorAll
+000010b0: 2827 5b78 2d63 6f6d 706f 6e65 6e74 5d27  ('[x-component]'
+000010c0: 292e 666f 7245 6163 6828 636f 6d70 6f6e  ).forEach(compon
+000010d0: 656e 7420 3d3e 207b 0a20 2020 2063 6f6e  ent => {.    con
+000010e0: 7374 2063 6f6d 706f 6e65 6e74 4e61 6d65  st componentName
+000010f0: 203d 2060 782d 247b 636f 6d70 6f6e 656e   = `x-${componen
+00001100: 742e 6765 7441 7474 7269 6275 7465 2827  t.getAttribute('
+00001110: 782d 636f 6d70 6f6e 656e 7427 297d 603b  x-component')}`;
+00001120: 0a0a 2020 2020 636c 6173 7320 5843 6f6d  ..    class XCom
+00001130: 706f 6e65 6e74 2065 7874 656e 6473 2048  ponent extends H
+00001140: 544d 4c45 6c65 6d65 6e74 207b 0a20 2020  TMLElement {.   
+00001150: 2020 2020 200a 2020 2020 2020 2020 636f       .        co
+00001160: 6e73 7472 7563 746f 7228 2920 7b0a 2020  nstructor() {.  
+00001170: 2020 2020 2020 2020 2020 7375 7065 7228            super(
+00001180: 293b 0a20 2020 2020 2020 207d 0a0a 2020  );.        }..  
+00001190: 2020 2020 2020 6173 796e 6320 636f 6e6e        async conn
+000011a0: 6563 7465 6443 616c 6c62 6163 6b28 2920  ectedCallback() 
+000011b0: 7b0a 2020 2020 2020 2020 2020 2020 7661  {.            va
+000011c0: 7220 6973 5368 6164 6f77 526f 6f74 203d  r isShadowRoot =
+000011d0: 2063 6f6d 706f 6e65 6e74 2e67 6574 4174   component.getAt
+000011e0: 7472 6962 7574 6528 2773 6861 646f 7772  tribute('shadowr
+000011f0: 6f6f 7427 293b 0a20 2020 2020 2020 2020  oot');.         
+00001200: 2020 206c 6574 2074 656d 706c 6174 653b     let template;
+00001210: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00001220: 2863 6f6d 706f 6e65 6e74 2e74 6167 4e61  (component.tagNa
+00001230: 6d65 203d 3d3d 2027 5445 4d50 4c41 5445  me === 'TEMPLATE
+00001240: 2729 7b0a 2020 2020 2020 2020 2020 2020  '){.            
+00001250: 2020 2020 7465 6d70 6c61 7465 203d 2063      template = c
+00001260: 6f6d 706f 6e65 6e74 3b0a 2020 2020 2020  omponent;.      
+00001270: 2020 2020 2020 7d20 656c 7365 207b 0a20        } else {. 
+00001280: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001290: 656d 706c 6174 6520 3d20 636f 6d70 6f6e  emplate = compon
+000012a0: 656e 742e 6765 7445 6c65 6d65 6e74 7342  ent.getElementsB
+000012b0: 7954 6167 4e61 6d65 2827 7465 6d70 6c61  yTagName('templa
+000012c0: 7465 2729 5b30 5d3b 0a20 2020 2020 2020  te')[0];.       
+000012d0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+000012e0: 2020 2069 6620 2821 2169 7353 6861 646f     if (!!isShado
+000012f0: 7752 6f6f 7429 7b0a 2020 2020 2020 2020  wRoot){.        
+00001300: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001310: 2020 2020 2020 2020 206c 6574 2073 6861           let sha
+00001320: 646f 7720 3d20 7468 6973 2e61 7474 6163  dow = this.attac
+00001330: 6853 6861 646f 7728 7b6d 6f64 653a 2027  hShadow({mode: '
+00001340: 6f70 656e 277d 293b 0a0a 2020 2020 2020  open'});..      
+00001350: 2020 2020 2020 2020 2020 6966 2028 7465            if (te
+00001360: 6d70 6c61 7465 3f2e 636f 6e74 656e 742e  mplate?.content.
+00001370: 6368 696c 6445 6c65 6d65 6e74 436f 756e  childElementCoun
+00001380: 7429 207b 0a20 2020 2020 2020 2020 2020  t) {.           
+00001390: 2020 2020 2020 2020 2073 6861 646f 772e           shadow.
+000013a0: 6170 7065 6e64 4368 696c 6428 7465 6d70  appendChild(temp
+000013b0: 6c61 7465 2e63 6f6e 7465 6e74 2e63 6c6f  late.content.clo
+000013c0: 6e65 4e6f 6465 2874 7275 6529 293b 0a20  neNode(true));. 
+000013d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000013e0: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
+000013f0: 2020 2020 2065 6c73 6520 7b0a 2020 2020       else {.    
+00001400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001410: 6c65 7420 736c 6f74 203d 2064 6f63 756d  let slot = docum
+00001420: 656e 742e 6372 6561 7465 456c 656d 656e  ent.createElemen
+00001430: 7428 2773 6c6f 7427 293b 0a20 2020 2020  t('slot');.     
+00001440: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00001450: 6861 646f 772e 6170 7065 6e64 4368 696c  hadow.appendChil
+00001460: 6428 736c 6f74 293b 0a20 2020 2020 2020  d(slot);.       
+00001470: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
+00001480: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00001490: 6869 732e 7368 6164 6f77 203d 2073 6861  his.shadow = sha
+000014a0: 646f 773b 0a20 2020 2020 2020 2020 2020  dow;.           
+000014b0: 2020 2020 2074 6869 732e 6368 6563 6b4f       this.checkO
+000014c0: 7243 7265 6174 6549 6428 293b 0a20 2020  rCreateId();.   
+000014d0: 2020 2020 2020 2020 2020 2020 2064 6f63               doc
+000014e0: 756d 656e 742e 6164 6445 7665 6e74 4c69  ument.addEventLi
+000014f0: 7374 656e 6572 2827 616c 7069 6e65 3a69  stener('alpine:i
+00001500: 6e69 7469 616c 697a 6564 272c 2028 2920  nitialized', () 
+00001510: 3d3e 207b 0a20 2020 2020 2020 2020 2020  => {.           
+00001520: 2020 2020 2020 2020 2041 6c70 696e 652e           Alpine.
+00001530: 696e 6974 5472 6565 2874 6869 732e 7368  initTree(this.sh
+00001540: 6164 6f77 293b 0a20 2020 2020 2020 2020  adow);.         
+00001550: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
+00001560: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001570: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00001580: 2020 656c 7365 207b 0a20 2020 2020 2020    else {.       
+00001590: 2020 2020 2020 2020 2074 6869 732e 6170           this.ap
+000015a0: 7065 6e64 2863 6f6d 706f 6e65 6e74 2e63  pend(component.c
+000015b0: 6f6e 7465 6e74 2e63 6c6f 6e65 4e6f 6465  ontent.cloneNode
+000015c0: 2874 7275 6529 293b 0a20 2020 2020 2020  (true));.       
+000015d0: 2020 2020 2020 2020 2074 6869 732e 6368           this.ch
+000015e0: 6563 6b4f 7243 7265 6174 6549 6428 293b  eckOrCreateId();
+000015f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001600: 2064 6f63 756d 656e 742e 6164 6445 7665   document.addEve
+00001610: 6e74 4c69 7374 656e 6572 2827 616c 7069  ntListener('alpi
+00001620: 6e65 3a69 6e69 7469 616c 697a 6564 272c  ne:initialized',
+00001630: 2028 2920 3d3e 207b 0a20 2020 2020 2020   () => {.       
+00001640: 2020 2020 2020 2020 2020 2020 2041 6c70               Alp
+00001650: 696e 652e 696e 6974 5472 6565 2874 6869  ine.initTree(thi
+00001660: 7329 3b0a 2020 2020 2020 2020 2020 2020  s);.            
+00001670: 2020 2020 7d29 3b0a 2020 2020 2020 2020      });.        
+00001680: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00001690: 2020 2020 2020 2020 2020 200a 2020 2020             .    
+000016a0: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
+000016b0: 2020 2020 2020 2020 2020 2074 6869 732e             this.
+000016c0: 6461 7461 4361 6c6c 6261 636b 203d 2074  dataCallback = t
+000016d0: 6869 732e 6461 7461 4361 6c6c 6261 636b  his.dataCallback
+000016e0: 2e62 696e 6428 7468 6973 293b 2020 2020  .bind(this);    
+000016f0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
+00001700: 2020 2020 2020 202f 2f20 3c6d 792d 6469         // <my-di
+00001710: 7620 6163 7469 7665 3d22 7472 7565 222c  v active="true",
+00001720: 2064 6174 612d 7461 7267 6574 3d22 2361   data-target="#a
+00001730: 6363 6f72 6469 616e 223e 3c2f 6d79 2d64  ccordian"></my-d
+00001740: 6976 3e0a 2020 2020 2020 2020 2020 2020  iv>.            
+00001750: 2f2f 2065 7861 6d70 6c65 3a20 666f 7220  // example: for 
+00001760: 7365 7474 696e 6720 7570 2020 6e61 6d65  setting up  name
+00001770: 3d22 636f 6f6c 2d64 7564 6522 2076 616c  ="cool-dude" val
+00001780: 7565 2061 7320 7468 6973 2e6e 616d 6520  ue as this.name 
+00001790: 7661 6c75 650a 2020 2020 2020 2020 2020  value.          
+000017a0: 2020 7468 6973 2e5f 6461 7461 5374 6174    this._dataStat
+000017b0: 6520 3d20 7468 6973 2e73 7461 7465 4461  e = this.stateDa
+000017c0: 7461 2829 3b0a 2020 2020 2020 2020 2020  ta();.          
+000017d0: 2020 0a20 2020 2020 2020 2020 2020 202f    .            /
+000017e0: 2f20 666f 7220 7365 7474 696e 6720 7570  / for setting up
+000017f0: 2064 6174 612d 7461 7267 6574 2076 616c   data-target val
+00001800: 7565 0a20 2020 2020 2020 2020 2020 206c  ue.            l
+00001810: 6574 205f 6461 7461 5461 7267 6574 203d  et _dataTarget =
+00001820: 2074 6869 733f 2e64 6174 6173 6574 2e74   this?.dataset.t
+00001830: 6172 6765 7420 7c7c 206e 6577 204d 6170  arget || new Map
+00001840: 2829 3b0a 2020 2020 2020 2020 2020 2020  ();.            
+00001850: 6966 2028 6973 4a53 4f4e 285f 6461 7461  if (isJSON(_data
+00001860: 5461 7267 6574 2929 7b0a 2020 2020 2020  Target)){.      
+00001870: 2020 2020 2020 2020 2020 5f64 6174 6154            _dataT
+00001880: 6172 6765 7420 3d20 4a53 4f4e 2e70 6172  arget = JSON.par
+00001890: 7365 285f 6461 7461 5461 7267 6574 293b  se(_dataTarget);
+000018a0: 0a20 2020 2020 2020 2020 2020 207d 0a20  .            }. 
+000018b0: 2020 2020 2020 2020 2020 202f 2f20 666f             // fo
+000018c0: 7220 7365 7474 696e 6720 7570 2064 6174  r setting up dat
+000018d0: 612d 6163 7469 6f6e 2076 616c 7565 0a20  a-action value. 
+000018e0: 2020 2020 2020 2020 2020 206c 6574 205f             let _
+000018f0: 6461 7461 4163 7469 6f6e 203d 2074 6869  dataAction = thi
+00001900: 733f 2e64 6174 6173 6574 2e61 6374 696f  s?.dataset.actio
+00001910: 6e20 7c7c 206e 6577 204d 6170 2829 3b0a  n || new Map();.
+00001920: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00001930: 2020 2020 2020 2020 2069 6620 2821 2174           if (!!t
+00001940: 6869 732e 5f64 6174 6153 7461 7465 2920  his._dataState) 
+00001950: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001960: 2020 7468 6973 2e5f 6461 7461 5374 6174    this._dataStat
+00001970: 652e 666f 7245 6163 6828 2876 616c 7565  e.forEach((value
+00001980: 2c20 6174 7472 2920 3d3e 207b 0a20 2020  , attr) => {.   
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 2069 6620 2874 6869 732e 6861 734f 776e   if (this.hasOwn
+000019b0: 5072 6f70 6572 7479 2861 7474 7229 297b  Property(attr)){
+000019c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000019d0: 2020 2020 2020 2020 2074 6872 6f77 206e           throw n
+000019e0: 6577 2045 7272 6f72 2860 6174 7472 6962  ew Error(`attrib
+000019f0: 7574 6520 247b 6174 7472 7d20 6361 6e27  ute ${attr} can'
+00001a00: 7420 6265 2061 7373 6967 6e65 6420 6173  t be assigned as
+00001a10: 2069 7473 2062 7569 6c74 696e 2048 746d   its builtin Htm
+00001a20: 6c45 6c65 6d65 6e74 2070 726f 7065 7274  lElement propert
+00001a30: 7960 293b 0a20 2020 2020 2020 2020 2020  y`);.           
+00001a40: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00001a50: 2020 2020 2020 2020 2020 2020 2020 204f                 O
+00001a60: 626a 6563 742e 6465 6669 6e65 5072 6f70  bject.defineProp
+00001a70: 6572 7479 2874 6869 732c 2060 5f64 6174  erty(this, `_dat
+00001a80: 615f 247b 6174 7472 7d60 2c20 7b0a 2020  a_${attr}`, {.  
+00001a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001aa0: 2020 2020 2020 6765 7428 2920 7b0a 2020        get() {.  
+00001ab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ac0: 2020 2020 2020 2020 2020 6966 2028 7468            if (th
+00001ad0: 6973 2e68 6173 4174 7472 6962 7574 6528  is.hasAttribute(
+00001ae0: 6024 7b61 7474 727d 6029 2920 7b0a 2020  `${attr}`)) {.  
+00001af0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b00: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00001b10: 7475 726e 2074 6869 732e 6765 7441 7474  turn this.getAtt
+00001b20: 7269 6275 7465 2860 247b 6174 7472 7d60  ribute(`${attr}`
+00001b30: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
+00001b40: 2020 2020 2020 2020 2020 2020 2020 207d                 }
+00001b50: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00001b60: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00001b70: 7475 726e 3b0a 2020 2020 2020 2020 2020  turn;.          
+00001b80: 2020 2020 2020 2020 2020 2020 2020 7d2c                },
+00001b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001ba0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00001bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001bc0: 2020 7365 7428 7661 6c75 6529 207b 0a20    set(value) {. 
+00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001be0: 2020 2020 2020 2020 2020 2069 6620 2869             if (i
+00001bf0: 734a 534f 4e28 7661 6c75 6529 2920 7b0a  sJSON(value)) {.
+00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c20: 2020 2020 2020 2020 2f2f 2066 6f72 2073          // for s
-00001c30: 6574 7469 6e67 2075 7020 6461 7461 2d61  etting up data-a
-00001c40: 6374 696f 6e20 7661 6c75 650a 2020 2020  ction value.    
-00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c60: 2020 2020 6c65 7420 5f64 6174 6141 6374      let _dataAct
-00001c70: 696f 6e20 3d20 7468 6973 3f2e 6461 7461  ion = this?.data
-00001c80: 7365 742e 6163 7469 6f6e 207c 7c20 7b7d  set.action || {}
-00001c90: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00001ca0: 2020 2020 2020 2020 2020 2f2f 636f 6e73            //cons
-00001cb0: 6f6c 652e 6c6f 6728 2244 4154 415f 5354  ole.log("DATA_ST
-00001cc0: 4154 453a 2022 2c20 5f64 6174 6153 7461  ATE: ", _dataSta
-00001cd0: 7465 293b 0a20 2020 2020 2020 2020 2020  te);.           
-00001ce0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00001cf0: 2821 215f 6461 7461 5374 6174 6529 207b  (!!_dataState) {
-00001d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001d10: 2020 2020 2020 2020 2020 2020 204f 626a               Obj
-00001d20: 6563 742e 6b65 7973 285f 6461 7461 5374  ect.keys(_dataSt
-00001d30: 6174 6529 2e66 6f72 4561 6368 2861 7474  ate).forEach(att
-00001d40: 7220 3d3e 207b 0a20 2020 2020 2020 2020  r => {.         
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d60: 2020 2020 2020 2069 6620 2874 6869 732e         if (this.
-00001d70: 6861 734f 776e 5072 6f70 6572 7479 2861  hasOwnProperty(a
-00001d80: 7474 7229 297b 0a20 2020 2020 2020 2020  ttr)){.         
-00001d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001da0: 2020 2020 2020 2020 2020 2074 6872 6f77             throw
-00001db0: 206e 6577 2045 7272 6f72 2860 6174 7472   new Error(`attr
-00001dc0: 6962 7574 6520 247b 6174 7472 7d20 6361  ibute ${attr} ca
-00001dd0: 6e27 7420 6265 2061 7373 6967 6e65 6420  n't be assigned 
-00001de0: 6173 2069 7473 2062 7569 6c74 696e 2048  as its builtin H
-00001df0: 746d 6c45 6c65 6d65 6e74 2070 726f 7065  tmlElement prope
-00001e00: 7274 7960 293b 0a20 2020 2020 2020 2020  rty`);.         
-00001e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e20: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e40: 2020 2020 2020 2020 204f 626a 6563 742e           Object.
-00001e50: 6465 6669 6e65 5072 6f70 6572 7479 2874  defineProperty(t
-00001e60: 6869 732c 2060 5f64 6174 615f 247b 6174  his, `_data_${at
-00001e70: 7472 7d60 2c20 7b0a 2020 2020 2020 2020  tr}`, {.        
-00001e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e90: 2020 2020 2020 2020 2020 2020 6765 7428              get(
-00001ea0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ec0: 2020 2020 2020 2020 2020 2020 6966 2028              if (
-00001ed0: 7468 6973 2e68 6173 4174 7472 6962 7574  this.hasAttribut
-00001ee0: 6528 605f 5f24 7b61 7474 727d 6029 2920  e(`__${attr}`)) 
-00001ef0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00001f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f10: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00001f20: 7475 726e 2074 6869 732e 6765 7441 7474  turn this.getAtt
-00001f30: 7269 6275 7465 2860 5f5f 247b 6174 7472  ribute(`__${attr
-00001f40: 7d60 293b 0a20 2020 2020 2020 2020 2020  }`);.           
-00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f60: 2020 2020 2020 2020 2020 2020 207d 2065               } e
-00001f70: 6c73 6520 7b0a 2020 2020 2020 2020 2020  lse {.          
-00001f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fa0: 2020 6c65 7420 7661 6c20 3d20 5f64 6174    let val = _dat
-00001fb0: 6153 7461 7465 5b61 7474 725d 3b0a 2020  aState[attr];.  
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fe0: 2020 2020 2020 2020 2020 6966 2028 6973            if (is
-00001ff0: 4a53 4f4e 2876 616c 2929 207b 0a20 2020  JSON(val)) {.   
-00002000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002020: 2020 2020 2020 2020 2020 2020 2074 6869               thi
-00002030: 732e 7365 7441 7474 7269 6275 7465 2860  s.setAttribute(`
-00002040: 5f5f 247b 6174 7472 7d60 2c20 4a53 4f4e  __${attr}`, JSON
-00002050: 2e70 6172 7365 2876 616c 2929 3b0a 2020  .parse(val));.  
-00002060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002080: 2020 2020 2020 2020 2020 7d20 656c 7365            } else
-00002090: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
-000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020c0: 2020 2074 6869 732e 7365 7441 7474 7269     this.setAttri
-000020d0: 6275 7465 2860 5f5f 247b 6174 7472 7d60  bute(`__${attr}`
-000020e0: 2c20 7661 6c29 3b0a 2020 2020 2020 2020  , val);.        
-000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002110: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002140: 2020 7265 7475 726e 2074 6869 732e 6765    return this.ge
-00002150: 7441 7474 7269 6275 7465 2860 5f5f 247b  tAttribute(`__${
-00002160: 6174 7472 7d60 293b 0a20 2020 2020 2020  attr}`);.       
-00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002190: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021b0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
-000021c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000021d0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-000021e0: 7428 7661 6c75 6529 207b 0a20 2020 2020  t(value) {.     
-000021f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002210: 2020 2069 6620 2869 734a 534f 4e28 7661     if (isJSON(va
-00002220: 6c75 6529 2920 7b0a 2020 2020 2020 2020  lue)) {.        
-00002230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002250: 2020 2020 7468 6973 2e73 6574 4174 7472      this.setAttr
-00002260: 6962 7574 6528 605f 5f24 7b61 7474 727d  ibute(`__${attr}
-00002270: 602c 204a 534f 4e2e 7061 7273 6528 7661  `, JSON.parse(va
-00002280: 6c75 6529 293b 0a20 2020 2020 2020 2020  lue));.         
-00002290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022a0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000022b0: 2065 6c73 6520 7b0a 2020 2020 2020 2020   else {.        
-000022c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000022e0: 2020 2020 7468 6973 2e73 6574 4174 7472      this.setAttr
-000022f0: 6962 7574 6528 605f 5f24 7b61 7474 727d  ibute(`__${attr}
-00002300: 602c 2076 616c 7565 293b 0a20 2020 2020  `, value);.     
-00002310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002330: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00002340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002350: 2020 2020 2020 2020 2020 2020 206c 6574               let
-00002360: 206f 6c64 5661 6c75 6520 3d20 7468 6973   oldValue = this
-00002370: 2e64 6174 6173 6574 2e73 7461 7465 5b61  .dataset.state[a
-00002380: 7474 725d 3b0a 2020 2020 2020 2020 2020  ttr];.          
-00002390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000023b0: 2028 6f6c 6456 616c 7565 2021 3d3d 2076   (oldValue !== v
-000023c0: 616c 7565 2920 7b0a 2020 2020 2020 2020  alue) {.        
-000023d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023f0: 2020 2020 7468 6973 2e64 6174 6173 6574      this.dataset
-00002400: 2e73 7461 7465 5b61 7474 725d 203d 2076  .state[attr] = v
-00002410: 616c 7565 3b0a 2020 2020 2020 2020 2020  alue;.          
-00002420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002430: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002460: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002480: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
-00002490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024a0: 2020 2020 2020 7d29 3b0a 2020 2020 2020        });.      
-000024b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000024c0: 2020 7d0a 0a20 2020 2020 2020 2020 2020    }..           
-000024d0: 2020 2020 2020 2020 2020 2020 202f 2f20               // 
-000024e0: 636f 6e6e 6563 7469 6e67 2074 6f20 7765  connecting to we
-000024f0: 6273 6f63 6b65 7473 0a20 2020 2020 2020  bsockets.       
-00002500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002510: 2069 6620 285f 6461 7461 5374 6174 653f   if (_dataState?
-00002520: 2e77 7329 7b0a 2020 2020 2020 2020 2020  .ws){.          
-00002530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002540: 2020 6c65 7420 6d65 7373 6167 6548 616e    let messageHan
-00002550: 646c 6572 203d 2064 6f63 756d 656e 742e  dler = document.
-00002560: 6d65 7373 6167 6548 616e 646c 6572 3b0a  messageHandler;.
-00002570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002580: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00002590: 6167 6548 616e 646c 6572 5b60 247b 7468  ageHandler[`${th
-000025a0: 6973 2e69 647d 605d 203d 2028 2920 3d3e  is.id}`] = () =>
-000025b0: 207b 7d3b 0a20 2020 2020 2020 2020 2020   {};.           
-000025c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025d0: 2074 6869 732e 7773 203d 2064 6f63 756d   this.ws = docum
-000025e0: 656e 742e 7365 7455 704f 7247 6574 5765  ent.setUpOrGetWe
-000025f0: 6253 6f63 6b65 7428 7468 6973 2e69 642c  bSocket(this.id,
-00002600: 206d 6573 7361 6765 4861 6e64 6c65 722c   messageHandler,
-00002610: 205f 6461 7461 5374 6174 653f 2e77 7320   _dataState?.ws 
-00002620: 7c7c 2027 7773 2729 3b0a 2020 2020 2020  || 'ws');.      
-00002630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002640: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00002650: 2020 2020 2020 2020 2020 2020 6966 2020              if  
-00002660: 2821 2174 6869 733f 2e77 733f 2e72 6561  (!!this?.ws?.rea
-00002670: 6479 5374 6174 6529 7b0a 2020 2020 2020  dyState){.      
-00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002690: 2020 2020 2020 7468 6973 2e77 732e 7365        this.ws.se
-000026a0: 6e64 284a 534f 4e2e 7374 7269 6e67 6966  nd(JSON.stringif
-000026b0: 7928 7b69 643a 2074 6869 732e 6964 7d29  y({id: this.id})
-000026c0: 293b 0a20 2020 2020 2020 2020 2020 2020  );.             
-000026d0: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
-000026e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000026f0: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-00002700: 2020 2020 2020 2020 2020 2020 2020 0a20                . 
-00002710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002720: 2020 2020 2020 2074 6869 732e 6f62 7365         this.obse
-00002730: 7276 6572 203d 206f 6273 6572 7665 4174  rver = observeAt
-00002740: 7472 4368 616e 6765 2874 6869 732c 2028  trChange(this, (
-00002750: 6174 7472 2c20 6f6c 6456 616c 2c20 6e65  attr, oldVal, ne
-00002760: 7756 616c 2920 3d3e 207b 0a20 2020 2020  wVal) => {.     
-00002770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002780: 2020 2020 2020 202f 2f20 736c 6963 6520         // slice 
-00002790: 3a61 7474 7220 746f 2072 656d 6f76 6520  :attr to remove 
-000027a0: 6c65 6164 696e 6720 275f 2720 2875 6e64  leading '_' (und
-000027b0: 6572 7363 6f72 6529 2074 6f20 6368 6563  erscore) to chec
-000027c0: 6b20 696e 205f 6461 7461 5374 6174 650a  k in _dataState.
-000027d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027e0: 2020 2020 2020 2020 2020 2020 2f2f 636f              //co
-000027f0: 6e73 6f6c 652e 6c6f 6728 6174 7472 2c20  nsole.log(attr, 
-00002800: 5f64 6174 6153 7461 7465 2e69 6e63 6c75  _dataState.inclu
-00002810: 6465 7328 6174 7472 2e72 6570 6c61 6365  des(attr.replace
-00002820: 2827 5f5f 272c 2027 2729 2929 3b0a 2020  ('__', '')));.  
-00002830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002840: 2020 2020 2020 2020 2020 6966 2028 5f64            if (_d
-00002850: 6174 6153 7461 7465 3f2e 696e 636c 7564  ataState?.includ
-00002860: 6573 2861 7474 722e 7265 706c 6163 6528  es(attr.replace(
-00002870: 275f 5f27 2c20 2727 2929 2920 7b0a 2020  '__', ''))) {.  
-00002880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002890: 2020 2020 2020 2020 2020 2020 2020 7468                th
-000028a0: 6973 2e61 7474 7269 6275 7465 4368 616e  is.attributeChan
-000028b0: 6765 6443 616c 6c62 6163 6b28 6174 7472  gedCallback(attr
-000028c0: 2e72 6570 6c61 6365 2827 5f5f 272c 2027  .replace('__', '
-000028d0: 2729 2c20 6f6c 6456 616c 2c20 6e65 7756  '), oldVal, newV
-000028e0: 616c 293b 0a20 2020 2020 2020 2020 2020  al);.           
-000028f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002900: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00002910: 2020 2020 2020 2020 2020 207d 293b 0a20             });. 
-00002920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002930: 2020 207d 0a20 2020 2020 2020 2020 2020     }.           
-00002940: 2020 2020 2020 2020 200a 2020 2020 2020           .      
-00002950: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00002960: 6563 6b49 6428 2920 7b0a 2020 2020 2020  eckId() {.      
-00002970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002980: 2020 6966 2028 2174 6869 732e 6964 2920    if (!this.id) 
-00002990: 7468 6973 2e69 6420 3d20 6078 2d24 7b63  this.id = `x-${c
-000029a0: 6f6d 706f 6e65 6e74 2e67 6574 4174 7472  omponent.getAttr
-000029b0: 6962 7574 6528 2778 2d63 6f6d 706f 6e65  ibute('x-compone
-000029c0: 6e74 2729 7d60 202b 2027 2d27 202b 2067  nt')}` + '-' + g
-000029d0: 7569 6447 656e 6572 6174 6f72 2829 3b0a  uidGenerator();.
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00002a00: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00002a10: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00002a20: 6174 6143 616c 6c62 6163 6b28 6d65 7373  ataCallback(mess
-00002a30: 6167 6529 7b0a 2020 2020 2020 2020 2020  age){.          
-00002a40: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002a50: 2028 6973 4a53 4f4e 286d 6573 7361 6765   (isJSON(message
-00002a60: 2929 7b0a 2020 2020 2020 2020 2020 2020  )){.            
-00002a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a80: 6d65 7373 6167 6520 3d20 4a53 4f4e 2e70  message = JSON.p
-00002a90: 6172 7365 286d 6573 7361 6765 293b 0a20  arse(message);. 
-00002aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ab0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
-00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ad0: 2069 6620 2874 7970 656f 6620 6d65 7373   if (typeof mess
-00002ae0: 6167 6520 3d3d 3d20 225b 6f62 6a65 6374  age === "[object
-00002af0: 2053 7472 696e 675d 2229 7b0a 2020 2020   String]"){.    
-00002b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b10: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
-00002b20: 6c6f 6728 2253 4552 5645 525f 4d45 5353  log("SERVER_MESS
-00002b30: 4147 4522 2c20 6d65 7373 6167 6529 3b0a  AGE", message);.
-00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b50: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00002b60: 726e 3b0a 2020 2020 2020 2020 2020 2020  rn;.            
-00002b70: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00002b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b90: 2020 2020 2020 6966 2028 7468 6973 2e69        if (this.i
-00002ba0: 6420 3d3d 3d20 6d65 7373 6167 652e 6964  d === message.id
-00002bb0: 297b 0a20 2020 2020 2020 2020 2020 2020  ){.             
-00002bc0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00002bd0: 6869 732e 6174 7472 6962 7574 6543 6861  his.attributeCha
-00002be0: 6e67 6564 4361 6c6c 6261 636b 286d 6573  ngedCallback(mes
-00002bf0: 7361 6765 2e61 7474 722c 206d 6573 7361  sage.attr, messa
-00002c00: 6765 2e6f 6c64 5661 6c2c 206d 6573 7361  ge.oldVal, messa
-00002c10: 6765 2e6e 6577 5661 6c29 3b0a 2020 2020  ge.newVal);.    
-00002c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c30: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
-00002c40: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00002c50: 6973 2e77 732e 7365 6e64 280a 2020 2020  is.ws.send(.    
-00002c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002c70: 2020 2020 2020 2020 4a53 4f4e 2e73 7472          JSON.str
-00002c80: 696e 6769 6679 280a 2020 2020 2020 2020  ingify(.        
-00002c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ca0: 2020 2020 2020 2020 7b69 643a 206d 6573          {id: mes
-00002cb0: 7361 6765 2e69 6420 2c20 0a20 2020 2020  sage.id , .     
-00002cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002cd0: 2020 2020 2020 2020 2020 2020 6174 7472              attr
-00002ce0: 3a6d 6573 7361 6765 2e61 7474 722c 0a20  :message.attr,. 
-00002cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d10: 6f6c 6456 616c 3a20 6d65 7373 6167 652e  oldVal: message.
-00002d20: 6f6c 6456 616c 2c20 0a20 2020 2020 2020  oldVal, .       
-00002d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d40: 2020 2020 2020 2020 2020 6e65 7756 616c            newVal
-00002d50: 3a20 6d65 7373 6167 652e 6e65 7756 616c  : message.newVal
-00002d60: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-00002d70: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00002d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002d90: 2020 2020 2020 2020 293b 0a20 2020 2020          );.     
-00002da0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-00002db0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002dc0: 2020 2020 2020 6174 7472 6962 7574 6543        attributeC
-00002dd0: 6861 6e67 6564 4361 6c6c 6261 636b 2861  hangedCallback(a
-00002de0: 7474 724e 616d 652c 206f 2c20 6e29 207b  ttrName, o, n) {
-00002df0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002e00: 2020 2020 2020 2020 2063 6f6e 736f 6c65           console
-00002e10: 2e6c 6f67 2861 7474 724e 616d 652c 206f  .log(attrName, o
-00002e20: 2c20 6e29 3b0a 2020 2020 2020 2020 2020  , n);.          
-00002e30: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00002e40: 2028 6e20 213d 3d20 6f29 7b0a 2020 2020   (n !== o){.    
-00002e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e60: 2020 2020 2020 2020 7468 6973 5b61 7474          this[att
-00002e70: 724e 616d 655d 203d 206e 3b20 2020 0a20  rName] = n;   . 
-00002e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002e90: 2020 2020 2020 2020 2020 202f 2f74 6869             //thi
-00002ea0: 732e 6461 7461 4361 6c6c 6261 636b 2861  s.dataCallback(a
-00002eb0: 7474 724e 616d 652c 206f 2c20 6e29 3b0a  ttrName, o, n);.
-00002ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002ed0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-00002ee0: 2020 2020 2020 2020 2020 2020 2020 7d0a                }.
-00002ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002f00: 2020 2020 2064 6973 636f 6e6e 6563 7465       disconnecte
-00002f10: 6443 616c 6c62 6163 6b28 2920 7b0a 2020  dCallback() {.  
-00002f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002f30: 2020 2020 2020 2f2f 7375 7065 722e 6469        //super.di
-00002f40: 7363 6f6e 6e65 6374 6564 4361 6c6c 6261  sconnectedCallba
-00002f50: 636b 2829 3b0a 2020 2020 2020 2020 2020  ck();.          
-00002f60: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00002f70: 6973 2e6f 6273 6572 7665 722e 6469 7363  is.observer.disc
-00002f80: 6f6e 6e65 6374 2829 3b0a 2020 2020 2020  onnect();.      
-00002f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fa0: 2020 7468 6973 2e6f 6273 6572 7665 7220    this.observer 
-00002fb0: 3d20 6e75 6c6c 3b0a 2020 2020 2020 2020  = null;.        
-00002fc0: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
-00002fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002fe0: 2020 2061 7379 6e63 2067 6574 4669 6c65     async getFile
-00002ff0: 2875 726c 2920 7b0a 2020 2020 2020 2020  (url) {.        
-00003000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003010: 636f 6e73 7420 7265 7320 3d20 6177 6169  const res = awai
-00003020: 7420 6665 7463 6828 7572 6c29 3b0a 2020  t fetch(url);.  
-00003030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003040: 2020 2020 2020 6966 2028 2172 6573 2e6f        if (!res.o
-00003050: 6b29 207b 0a20 2020 2020 2020 2020 2020  k) {.           
-00003060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003070: 2074 6872 6f77 204f 626a 6563 742e 6173   throw Object.as
-00003080: 7369 676e 286e 6577 2045 7272 6f72 2872  sign(new Error(r
-00003090: 6573 2e73 7461 7475 7354 6578 7420 2b20  es.statusText + 
-000030a0: 2720 2720 2b20 7572 6c29 2c20 7b0a 2020  ' ' + url), {.  
-000030b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000030d0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-000030e0: 2020 2020 2020 2020 2020 2020 2020 7d29                })
-000030f0: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
-00003100: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
-00003110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003120: 2020 2020 7265 7475 726e 207b 0a20 2020      return {.   
-00003130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003140: 2020 2020 2020 2020 2067 6574 436f 6e74           getCont
-00003150: 656e 7444 6174 613a 2061 7342 696e 6172  entData: asBinar
-00003160: 7920 3d3e 2061 7342 696e 6172 7920 3f20  y => asBinary ? 
-00003170: 7265 732e 6172 7261 7942 7566 6665 7228  res.arrayBuffer(
-00003180: 2920 3a20 7265 732e 7465 7874 2829 2c0a  ) : res.text(),.
-00003190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000031a0: 2020 2020 2020 2020 7d3b 0a20 2020 2020          };.     
-000031b0: 2020 2020 2020 2020 2020 2020 2020 207d                 }
-000031c0: 0a0a 0a20 2020 2020 2020 2020 2020 2020  ...             
-000031d0: 2020 2020 2020 2064 6973 7061 7463 6828         dispatch(
-000031e0: 6e61 6d65 2c20 6461 7461 2c20 6f70 7469  name, data, opti
-000031f0: 6f6e 7320 3d20 7b0a 2020 2020 2020 2020  ons = {.        
-00003200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003210: 6275 6262 6c65 3a20 7472 7565 2c0a 2020  bubble: true,.  
-00003220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003230: 2020 2020 2020 6361 6e63 656c 6162 6c65        cancelable
-00003240: 3a20 6661 6c73 652c 0a20 2020 2020 2020  : false,.       
-00003250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003260: 2063 6f6d 706f 7365 643a 2066 616c 7365   composed: false
-00003270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003280: 2020 2020 207d 2920 7b0a 2020 2020 2020       }) {.      
-00003290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032a0: 2020 636f 6e73 7420 6576 656e 7420 3d20    const event = 
-000032b0: 6e65 7720 4375 7374 6f6d 4576 656e 7428  new CustomEvent(
-000032c0: 6e61 6d65 2c20 7b0a 2020 2020 2020 2020  name, {.        
-000032d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000032e0: 2020 2020 6275 6262 6c65 733a 206f 7074      bubbles: opt
-000032f0: 696f 6e73 2e62 7562 626c 652c 0a20 2020  ions.bubble,.   
-00003300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003310: 2020 2020 2020 2020 2063 616e 6365 6c61           cancela
-00003320: 626c 653a 206f 7074 696f 6e73 2e63 616e  ble: options.can
-00003330: 6365 6c61 626c 652c 0a20 2020 2020 2020  celable,.       
-00003340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003350: 2020 2020 2063 6f6d 706f 7365 643a 206f       composed: o
-00003360: 7074 696f 6e73 2e63 6f6d 706f 7365 642c  ptions.composed,
-00003370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003380: 2020 2020 2020 2020 2020 2020 2064 6574               det
-00003390: 6169 6c3a 2064 6174 610a 2020 2020 2020  ail: data.      
-000033a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000033b0: 2020 7d29 3b0a 2020 2020 2020 2020 2020    });.          
-000033c0: 2020 2020 2020 2020 2020 2020 2020 7468                th
-000033d0: 6973 2e64 6973 7061 7463 6845 7665 6e74  is.dispatchEvent
-000033e0: 2865 7665 6e74 293b 0a20 2020 2020 2020  (event);.       
-000033f0: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00003400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003410: 2020 200a 0a20 2020 2020 2020 2020 2020     ..           
-00003420: 2020 2020 2020 2020 2064 6174 6128 2920           data() 
-00003430: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-00003440: 2020 2020 2020 2020 2020 636f 6e73 7420            const 
-00003450: 6174 7472 6962 7574 6573 203d 2074 6869  attributes = thi
-00003460: 732e 6765 7441 7474 7269 6275 7465 4e61  s.getAttributeNa
-00003470: 6d65 7328 293b 0a20 2020 2020 2020 2020  mes();.         
-00003480: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003490: 6f6e 7374 2064 6174 6120 3d20 7b7d 3b0a  onst data = {};.
-000034a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000034b0: 2020 2020 2020 2020 2061 7474 7269 6275           attribu
-000034c0: 7465 732e 666f 7245 6163 6828 6174 7472  tes.forEach(attr
-000034d0: 6962 7574 6520 3d3e 207b 0a0a 2020 2020  ibute => {..    
-000034e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000034f0: 2020 2020 2020 2020 6966 2028 2169 734a          if (!isJ
-00003500: 534f 4e28 7468 6973 2e67 6574 4174 7472  SON(this.getAttr
-00003510: 6962 7574 6528 6174 7472 6962 7574 6529  ibute(attribute)
-00003520: 2929 207b 0a20 2020 2020 2020 2020 2020  )) {.           
-00003530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003540: 2020 2020 2064 6174 615b 6174 7472 6962       data[attrib
-00003550: 7574 655d 203d 2074 6869 732e 6765 7441  ute] = this.getA
-00003560: 7474 7269 6275 7465 2861 7474 7269 6275  ttribute(attribu
-00003570: 7465 293b 0a20 2020 2020 2020 2020 2020  te);.           
-00003580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003590: 207d 2065 6c73 6520 7b0a 2020 2020 2020   } else {.      
-000035a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000035b0: 2020 2020 2020 2020 2020 6461 7461 5b61            data[a
-000035c0: 7474 7269 6275 7465 5d20 3d20 4a53 4f4e  ttribute] = JSON
-000035d0: 2e70 6172 7365 2874 6869 732e 6765 7441  .parse(this.getA
-000035e0: 7474 7269 6275 7465 2861 7474 7269 6275  ttribute(attribu
-000035f0: 7465 2929 3b0a 2020 2020 2020 2020 2020  te));.          
-00003600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003610: 2020 7d0a 2020 2020 2020 2020 2020 2020    }.            
-00003620: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
-00003630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003640: 2020 2020 2020 2020 7265 7475 726e 2064          return d
-00003650: 6174 613b 0a20 2020 2020 2020 2020 2020  ata;.           
-00003660: 2020 2020 2020 2020 207d 0a0a 2020 2020           }..    
-00003670: 2020 2020 2020 2020 2020 2020 7d0a 0a20              }.. 
-00003680: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00003690: 7573 746f 6d45 6c65 6d65 6e74 732e 6465  ustomElements.de
-000036a0: 6669 6e65 2863 6f6d 706f 6e65 6e74 4e61  fine(componentNa
-000036b0: 6d65 2c20 5843 6f6d 706f 6e65 6e74 293b  me, XComponent);
-000036c0: 0a20 2020 2020 2020 2020 2020 207d 293b  .            });
-000036d0: 200a 2020 2020 2020 2020 2020 2020 0a20   .            . 
-000036e0: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
-000036f0: 2020 2020 2020 2072 6574 7572 6e20 7363         return sc
-00003700: 7269 7074 2872 6177 286a 7329 290a       ript(raw(js)).
+00001c20: 7468 6973 2e73 6574 4174 7472 6962 7574  this.setAttribut
+00001c30: 6528 6024 7b61 7474 727d 602c 204a 534f  e(`${attr}`, JSO
+00001c40: 4e2e 7061 7273 6528 7661 6c75 6529 293b  N.parse(value));
+00001c50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c60: 2020 2020 2020 2020 2020 2020 207d 2065               } e
+00001c70: 6c73 6520 7b0a 2020 2020 2020 2020 2020  lse {.          
+00001c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001c90: 2020 2020 2020 7468 6973 2e73 6574 4174        this.setAt
+00001ca0: 7472 6962 7574 6528 6024 7b61 7474 727d  tribute(`${attr}
+00001cb0: 602c 2076 616c 7565 293b 0a20 2020 2020  `, value);.     
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cd0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cf0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
+00001d00: 2020 2020 2020 207d 293b 0a20 2020 2020         });.     
+00001d10: 2020 2020 2020 2020 2020 207d 293b 0a20             });. 
+00001d20: 2020 2020 2020 2020 2020 207d 0a0a 2020             }..  
+00001d30: 2020 2020 2020 2020 2020 2f2f 2063 6f6e            // con
+00001d40: 6e65 6374 696e 6720 746f 2077 6562 736f  necting to webso
+00001d50: 636b 6574 730a 2020 2020 2020 2020 2020  ckets.          
+00001d60: 2020 6966 2028 7468 6973 2e5f 6461 7461    if (this._data
+00001d70: 5374 6174 652e 6765 7428 2777 7327 2929  State.get('ws'))
+00001d80: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00001d90: 2020 6c65 7420 6d65 7373 6167 6548 616e    let messageHan
+00001da0: 646c 6572 203d 2064 6f63 756d 656e 742e  dler = document.
+00001db0: 6d65 7373 6167 6548 616e 646c 6572 3b0a  messageHandler;.
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001dd0: 6d65 7373 6167 6548 616e 646c 6572 5b60  messageHandler[`
+00001de0: 247b 7468 6973 2e69 647d 605d 203d 2074  ${this.id}`] = t
+00001df0: 6869 732e 6461 7461 4361 6c6c 6261 636b  his.dataCallback
+00001e00: 3b0a 2020 2020 2020 2020 2020 2020 2020  ;.              
+00001e10: 2020 7468 6973 2e77 7320 3d20 646f 6375    this.ws = docu
+00001e20: 6d65 6e74 2e73 6574 5570 4f72 4765 7457  ment.setUpOrGetW
+00001e30: 6562 536f 636b 6574 2874 6869 732e 6964  ebSocket(this.id
+00001e40: 2c20 6d65 7373 6167 6548 616e 646c 6572  , messageHandler
+00001e50: 2c20 7468 6973 2e5f 6461 7461 5374 6174  , this._dataStat
+00001e60: 652e 6765 7428 2777 7327 2929 3b0a 2020  e.get('ws'));.  
+00001e70: 2020 2020 2020 2020 2020 2020 2020 7468                th
+00001e80: 6973 2e77 6169 7446 6f72 436f 6e6e 6563  is.waitForConnec
+00001e90: 7469 6f6e 203d 2064 6f63 756d 656e 742e  tion = document.
+00001ea0: 7761 6974 466f 7243 6f6e 6e65 6374 696f  waitForConnectio
+00001eb0: 6e5b 6024 7b74 6869 732e 5f64 6174 6153  n[`${this._dataS
+00001ec0: 7461 7465 2e67 6574 2827 7773 2729 7d60  tate.get('ws')}`
+00001ed0: 5d0a 2020 2020 2020 2020 2020 2020 7d0a  ].            }.
+00001ee0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
+00001ef0: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+00001f00: 2020 2020 2020 7468 6973 2e6f 6273 6572        this.obser
+00001f10: 7665 7220 3d20 6f62 7365 7276 6541 7474  ver = observeAtt
+00001f20: 7243 6861 6e67 6528 7468 6973 2c20 2861  rChange(this, (a
+00001f30: 7474 722c 206f 6c64 5661 6c2c 206e 6577  ttr, oldVal, new
+00001f40: 5661 6c29 203d 3e20 7b0a 2020 2020 2020  Val) => {.      
+00001f50: 2020 2020 2020 2020 2020 2f2f 2073 6c69            // sli
+00001f60: 6365 203a 6174 7472 2074 6f20 7265 6d6f  ce :attr to remo
+00001f70: 7665 206c 6561 6469 6e67 2027 5f27 2028  ve leading '_' (
+00001f80: 756e 6465 7273 636f 7265 2920 746f 2063  underscore) to c
+00001f90: 6865 636b 2069 6e20 7468 6973 2e5f 6461  heck in this._da
+00001fa0: 7461 5374 6174 650a 2020 2020 2020 2020  taState.        
+00001fb0: 2020 2020 2020 2020 636f 6e73 6f6c 652e          console.
+00001fc0: 6c6f 6728 2766 726f 6d20 6f62 7365 7276  log('from observ
+00001fd0: 6572 272c 6174 7472 2c20 6f6c 6456 616c  er',attr, oldVal
+00001fe0: 2c20 6e65 7756 616c 293b 0a20 2020 2020  , newVal);.     
+00001ff0: 2020 2020 2020 2020 2020 202f 2f63 6f6e             //con
+00002000: 736f 6c65 2e6c 6f67 2861 7474 722c 2074  sole.log(attr, t
+00002010: 6869 732e 5f64 6174 6153 7461 7465 2e67  his._dataState.g
+00002020: 6574 2861 7474 722e 7265 706c 6163 6528  et(attr.replace(
+00002030: 275f 6461 7461 5f27 2c20 2727 2929 293b  '_data_', '')));
+00002040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002050: 2069 6620 2874 6869 732e 5f64 6174 6153   if (this._dataS
+00002060: 7461 7465 2e67 6574 2861 7474 722e 7265  tate.get(attr.re
+00002070: 706c 6163 6528 275f 6461 7461 5f27 2c20  place('_data_', 
+00002080: 2727 2929 2920 7b0a 2020 2020 2020 2020  ''))) {.        
+00002090: 2020 2020 2020 2020 2020 2020 7468 6973              this
+000020a0: 2e61 7474 7269 6275 7465 4368 616e 6765  .attributeChange
+000020b0: 6443 616c 6c62 6163 6b28 6174 7472 2e72  dCallback(attr.r
+000020c0: 6570 6c61 6365 2827 5f64 6174 615f 272c  eplace('_data_',
+000020d0: 2027 2729 2c20 6f6c 6456 616c 2c20 6e65   ''), oldVal, ne
+000020e0: 7756 616c 293b 0a20 2020 2020 2020 2020  wVal);.         
+000020f0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00002100: 2020 2020 207d 293b 0a20 2020 2020 2020       });.       
+00002110: 2020 2020 200a 2020 2020 2020 2020 2020       .          
+00002120: 2020 2f2f 7365 7454 696d 656f 7574 2828    //setTimeout((
+00002130: 2920 3d3e 207b 7468 6973 2e77 732e 7365  ) => {this.ws.se
+00002140: 6e64 284a 534f 4e2e 7374 7269 6e67 6966  nd(JSON.stringif
+00002150: 7928 7468 6973 2e64 6174 6128 2929 293b  y(this.data()));
+00002160: 7d2c 2033 3030 293b 0a20 2020 2020 2020  }, 300);.       
+00002170: 2020 2020 2069 6620 2874 6869 732e 6765       if (this.ge
+00002180: 7441 7474 7269 6275 7465 2827 7773 5f73  tAttribute('ws_s
+00002190: 656e 6427 2929 7b0a 2020 2020 2020 2020  end')){.        
+000021a0: 2020 2020 2020 2020 7468 6973 2e73 656e          this.sen
+000021b0: 6428 4a53 4f4e 2e73 7472 696e 6769 6679  d(JSON.stringify
+000021c0: 2874 6869 732e 5f64 6174 6153 7461 7465  (this._dataState
+000021d0: 2e67 6574 2827 7773 5f73 656e 6427 2929  .get('ws_send'))
+000021e0: 293b 0a20 2020 2020 2020 2020 2020 207d  );.            }
+000021f0: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00002200: 2020 200a 2020 2020 2020 2020 0a20 2020     .        .   
+00002210: 2020 2020 2063 6865 636b 4f72 4372 6561       checkOrCrea
+00002220: 7465 4964 2829 207b 0a20 2020 2020 2020  teId() {.       
+00002230: 2020 2020 2069 6620 2821 7468 6973 2e69       if (!this.i
+00002240: 6429 2074 6869 732e 6964 203d 2060 782d  d) this.id = `x-
+00002250: 247b 636f 6d70 6f6e 656e 742e 6765 7441  ${component.getA
+00002260: 7474 7269 6275 7465 2827 782d 636f 6d70  ttribute('x-comp
+00002270: 6f6e 656e 7427 297d 6020 2b20 272d 2720  onent')}` + '-' 
+00002280: 2b20 6775 6964 4765 6e65 7261 746f 7228  + guidGenerator(
+00002290: 293b 0a20 2020 2020 2020 207d 0a20 2020  );.        }.   
+000022a0: 2020 2020 200a 2020 2020 2020 2020 0a20       .        . 
+000022b0: 2020 2020 2020 2064 6174 6143 616c 6c62         dataCallb
+000022c0: 6163 6b28 6d65 7373 6167 6529 7b0a 2020  ack(message){.  
+000022d0: 2020 2020 2020 2020 2020 6966 2028 6973            if (is
+000022e0: 4a53 4f4e 286d 6573 7361 6765 2929 7b0a  JSON(message)){.
+000022f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002300: 6d65 7373 6167 6520 3d20 4a53 4f4e 2e70  message = JSON.p
+00002310: 6172 7365 286d 6573 7361 6765 293b 0a20  arse(message);. 
+00002320: 2020 2020 2020 2020 2020 207d 0a20 2020             }.   
+00002330: 2020 2020 2020 2020 2069 6620 2874 7970           if (typ
+00002340: 656f 6620 6d65 7373 6167 6520 3d3d 3d20  eof message === 
+00002350: 225b 6f62 6a65 6374 2053 7472 696e 675d  "[object String]
+00002360: 2229 7b0a 2020 2020 2020 2020 2020 2020  "){.            
+00002370: 2020 2020 636f 6e73 6f6c 652e 6c6f 6728      console.log(
+00002380: 2253 4552 5645 525f 4d45 5353 4147 4522  "SERVER_MESSAGE"
+00002390: 2c20 6d65 7373 6167 6529 3b0a 2020 2020  , message);.    
+000023a0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000023b0: 726e 3b0a 2020 2020 2020 2020 2020 2020  rn;.            
+000023c0: 7d0a 2020 2020 2020 2020 2020 2020 6966  }.            if
+000023d0: 2028 7468 6973 2e69 6420 3d3d 3d20 6d65   (this.id === me
+000023e0: 7373 6167 652e 6964 297b 0a20 2020 2020  ssage.id){.     
+000023f0: 2020 2020 2020 2020 2020 2074 6869 732e             this.
+00002400: 6174 7472 6962 7574 6543 6861 6e67 6564  attributeChanged
+00002410: 4361 6c6c 6261 636b 286d 6573 7361 6765  Callback(message
+00002420: 2e61 7474 722c 206d 6573 7361 6765 2e6f  .attr, message.o
+00002430: 6c64 5661 6c2c 206d 6573 7361 6765 2e6e  ldVal, message.n
+00002440: 6577 5661 6c29 3b0a 2020 2020 2020 2020  ewVal);.        
+00002450: 2020 2020 7d0a 2020 2020 2020 2020 2020      }.          
+00002460: 2020 7468 6973 2e73 656e 6428 4a53 4f4e    this.send(JSON
+00002470: 2e73 7472 696e 6769 6679 286d 6573 7361  .stringify(messa
+00002480: 6765 2929 3b0a 2020 2020 2020 2020 7d0a  ge));.        }.
+00002490: 0a20 2020 2020 2020 2061 7474 7269 6275  .        attribu
+000024a0: 7465 4368 616e 6765 6443 616c 6c62 6163  teChangedCallbac
+000024b0: 6b28 6174 7472 4e61 6d65 2c20 6f2c 206e  k(attrName, o, n
+000024c0: 2920 7b0a 2020 2020 2020 2020 2020 2020  ) {.            
+000024d0: 636f 6e73 6f6c 652e 6c6f 6728 2766 726f  console.log('fro
+000024e0: 6d20 6174 7472 6962 7574 6543 6861 6e67  m attributeChang
+000024f0: 6564 4361 6c6c 6261 636b 272c 2061 7474  edCallback', att
+00002500: 724e 616d 652c 206f 2c20 6e29 3b0a 2020  rName, o, n);.  
+00002510: 2020 2020 2020 2020 2020 6966 2028 6e20            if (n 
+00002520: 213d 3d20 6f29 7b0a 2020 2020 2020 2020  !== o){.        
+00002530: 2020 2020 2020 2020 7468 6973 5b61 7474          this[att
+00002540: 724e 616d 655d 203d 206e 3b0a 2020 2020  rName] = n;.    
+00002550: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002560: 2020 7d0a 0a20 2020 2020 2020 2064 6973    }..        dis
+00002570: 636f 6e6e 6563 7465 6443 616c 6c62 6163  connectedCallbac
+00002580: 6b28 2920 7b0a 2020 2020 2020 2020 2020  k() {.          
+00002590: 2020 2f2f 7375 7065 722e 6469 7363 6f6e    //super.discon
+000025a0: 6e65 6374 6564 4361 6c6c 6261 636b 2829  nectedCallback()
+000025b0: 3b0a 2020 2020 2020 2020 2020 2020 7468  ;.            th
+000025c0: 6973 2e6f 6273 6572 7665 722e 6469 7363  is.observer.disc
+000025d0: 6f6e 6e65 6374 2829 3b0a 2020 2020 2020  onnect();.      
+000025e0: 2020 2020 2020 7468 6973 2e6f 6273 6572        this.obser
+000025f0: 7665 7220 3d20 6e75 6c6c 3b0a 2020 2020  ver = null;.    
+00002600: 2020 2020 2020 2020 7468 6973 2e77 732e          this.ws.
+00002610: 636c 6f73 6528 293b 0a20 2020 2020 2020  close();.       
+00002620: 2020 2020 2074 6869 732e 7773 203d 206e       this.ws = n
+00002630: 756c 6c3b 0a20 2020 2020 2020 207d 0a20  ull;.        }. 
+00002640: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00002650: 7365 6e64 2864 6174 612c 2072 6574 7269  send(data, retri
+00002660: 6573 203d 2034 2920 7b0a 2020 2020 2020  es = 4) {.      
+00002670: 2020 2020 2020 7472 7920 7b0a 2020 2020        try {.    
+00002680: 2020 2020 2020 2020 2020 2020 7468 6973              this
+00002690: 2e77 732e 7365 6e64 2864 6174 6129 3b0a  .ws.send(data);.
+000026a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026b0: 7265 7475 726e 2064 6174 613b 0a20 2020  return data;.   
+000026c0: 2020 2020 2020 2020 207d 200a 2020 2020           } .    
+000026d0: 2020 2020 2020 2020 6361 7463 6820 2865          catch (e
+000026e0: 7272 6f72 2920 7b0a 2020 2020 2020 2020  rror) {.        
+000026f0: 2020 2020 2020 2020 6966 2028 7265 7472          if (retr
+00002700: 6965 7320 3e20 3020 2626 2065 7272 6f72  ies > 0 && error
+00002710: 2e6e 616d 6520 3d3d 3d20 2249 6e76 616c  .name === "Inval
+00002720: 6964 5374 6174 6545 7272 6f72 2229 207b  idStateError") {
+00002730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002740: 2020 2020 2074 6869 732e 7761 6974 466f       this.waitFo
+00002750: 7243 6f6e 6e65 6374 696f 6e28 290a 2020  rConnection().  
+00002760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002770: 2020 2020 2020 2e74 6865 6e28 2829 3d3e        .then(()=>
+00002780: 2074 6869 732e 7365 6e64 2864 6174 612c   this.send(data,
+00002790: 2072 6574 7269 6573 202d 2031 2929 3b0a   retries - 1));.
+000027a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027b0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+000027c0: 2020 656c 7365 207b 0a20 2020 2020 2020    else {.       
+000027d0: 2020 2020 2020 2020 2020 2020 2074 6872               thr
+000027e0: 6f77 2065 7272 6f72 3b0a 2020 2020 2020  ow error;.      
+000027f0: 2020 2020 2020 2020 2020 7d0a 2020 2020            }.    
+00002800: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00002810: 2020 7d0a 0a20 2020 2020 2020 2061 7379    }..        asy
+00002820: 6e63 2067 6574 4669 6c65 2875 726c 2920  nc getFile(url) 
+00002830: 7b0a 2020 2020 2020 2020 2020 2020 636f  {.            co
+00002840: 6e73 7420 7265 7320 3d20 6177 6169 7420  nst res = await 
+00002850: 6665 7463 6828 7572 6c29 3b0a 2020 2020  fetch(url);.    
+00002860: 2020 2020 2020 2020 6966 2028 2172 6573          if (!res
+00002870: 2e6f 6b29 207b 0a20 2020 2020 2020 2020  .ok) {.         
+00002880: 2020 2020 2020 2074 6872 6f77 204f 626a         throw Obj
+00002890: 6563 742e 6173 7369 676e 286e 6577 2045  ect.assign(new E
+000028a0: 7272 6f72 2872 6573 2e73 7461 7475 7354  rror(res.statusT
+000028b0: 6578 7420 2b20 2720 2720 2b20 7572 6c29  ext + ' ' + url)
+000028c0: 2c20 7b0a 2020 2020 2020 2020 2020 2020  , {.            
+000028d0: 2020 2020 2020 2020 7265 730a 2020 2020          res.    
+000028e0: 2020 2020 2020 2020 2020 2020 7d29 3b0a              });.
+000028f0: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
+00002900: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00002910: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00002920: 2020 2067 6574 436f 6e74 656e 7444 6174     getContentDat
+00002930: 613a 2061 7342 696e 6172 7920 3d3e 2061  a: asBinary => a
+00002940: 7342 696e 6172 7920 3f20 7265 732e 6172  sBinary ? res.ar
+00002950: 7261 7942 7566 6665 7228 2920 3a20 7265  rayBuffer() : re
+00002960: 732e 7465 7874 2829 2c0a 2020 2020 2020  s.text(),.      
+00002970: 2020 2020 2020 7d3b 0a20 2020 2020 2020        };.       
+00002980: 207d 0a0a 0a20 2020 2020 2020 2064 6973   }...        dis
+00002990: 7061 7463 6828 6e61 6d65 2c20 6461 7461  patch(name, data
+000029a0: 2c20 6f70 7469 6f6e 7320 3d20 7b0a 2020  , options = {.  
+000029b0: 2020 2020 2020 2020 2020 6275 6262 6c65            bubble
+000029c0: 3a20 7472 7565 2c0a 2020 2020 2020 2020  : true,.        
+000029d0: 2020 2020 6361 6e63 656c 6162 6c65 3a20      cancelable: 
+000029e0: 6661 6c73 652c 0a20 2020 2020 2020 2020  false,.         
+000029f0: 2020 2063 6f6d 706f 7365 643a 2066 616c     composed: fal
+00002a00: 7365 0a20 2020 2020 2020 207d 2920 7b0a  se.        }) {.
+00002a10: 2020 2020 2020 2020 2020 2020 636f 6e73              cons
+00002a20: 7420 6576 656e 7420 3d20 6e65 7720 4375  t event = new Cu
+00002a30: 7374 6f6d 4576 656e 7428 6e61 6d65 2c20  stomEvent(name, 
+00002a40: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002a50: 2020 6275 6262 6c65 733a 206f 7074 696f    bubbles: optio
+00002a60: 6e73 2e62 7562 626c 652c 0a20 2020 2020  ns.bubble,.     
+00002a70: 2020 2020 2020 2020 2020 2063 616e 6365             cance
+00002a80: 6c61 626c 653a 206f 7074 696f 6e73 2e63  lable: options.c
+00002a90: 616e 6365 6c61 626c 652c 0a20 2020 2020  ancelable,.     
+00002aa0: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
+00002ab0: 7365 643a 206f 7074 696f 6e73 2e63 6f6d  sed: options.com
+00002ac0: 706f 7365 642c 0a20 2020 2020 2020 2020  posed,.         
+00002ad0: 2020 2020 2020 2064 6574 6169 6c3a 2064         detail: d
+00002ae0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+00002af0: 7d29 3b0a 2020 2020 2020 2020 2020 2020  });.            
+00002b00: 7468 6973 2e64 6973 7061 7463 6845 7665  this.dispatchEve
+00002b10: 6e74 2865 7665 6e74 293b 0a20 2020 2020  nt(event);.     
+00002b20: 2020 207d 0a0a 0a20 2020 2020 2020 2064     }...        d
+00002b30: 6174 6128 2920 7b0a 2020 2020 2020 2020  ata() {.        
+00002b40: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00002b50: 206c 6574 2066 696c 7465 7241 7474 7220   let filterAttr 
+00002b60: 3d20 5b22 4022 2c20 2278 2d22 2c20 2269  = ["@", "x-", "i
+00002b70: 6422 2c20 2263 6c61 7373 222c 2022 3a22  d", "class", ":"
+00002b80: 5d0a 2020 2020 2020 2020 2020 2020 6c65  ].            le
+00002b90: 7420 7468 6973 4574 7269 6573 203d 204f  t thisEtries = O
+00002ba0: 626a 6563 742e 656e 7472 6965 7328 0a20  bject.entries(. 
+00002bb0: 2020 2020 2020 2020 2020 2020 2020 204f                 O
+00002bc0: 626a 6563 742e 6672 6f6d 456e 7472 6965  bject.fromEntrie
+00002bd0: 7328 7468 6973 2e73 7461 7465 4461 7461  s(this.stateData
+00002be0: 2829 290a 2020 2020 2020 2020 2020 2020  ()).            
+00002bf0: 2020 2020 292e 6669 6c74 6572 2828 5b61      ).filter(([a
+00002c00: 7474 722c 2076 616c 7565 5d29 203d 3e20  ttr, value]) => 
+00002c10: 2166 696c 7465 7241 7474 722e 736f 6d65  !filterAttr.some
+00002c20: 2828 6c65 7474 6572 2920 3d3e 2061 7474  ((letter) => att
+00002c30: 722e 7374 6172 7473 5769 7468 286c 6574  r.startsWith(let
+00002c40: 7465 7229 2929 3b0a 2020 2020 2020 2020  ter)));.        
+00002c50: 2020 2020 7265 7475 726e 204f 626a 6563      return Objec
+00002c60: 742e 6672 6f6d 456e 7472 6965 7328 7468  t.fromEntries(th
+00002c70: 6973 4574 7269 6573 293b 2020 2020 2020  isEtries);      
+00002c80: 2020 2020 2020 0a20 2020 2020 2020 207d        .        }
+00002c90: 0a0a 2020 2020 2020 2020 7374 6174 6544  ..        stateD
+00002ca0: 6174 6128 2920 7b0a 2020 2020 2020 2020  ata() {.        
+00002cb0: 2020 2020 636f 6e73 7420 6174 7472 6962      const attrib
+00002cc0: 7574 6573 203d 2074 6869 732e 6765 7441  utes = this.getA
+00002cd0: 7474 7269 6275 7465 4e61 6d65 7328 293b  ttributeNames();
+00002ce0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00002cf0: 7374 2064 6174 6120 3d20 6e65 7720 4d61  st data = new Ma
+00002d00: 7028 293b 0a0a 2020 2020 2020 2020 2020  p();..          
+00002d10: 2020 6174 7472 6962 7574 6573 2e66 6f72    attributes.for
+00002d20: 4561 6368 2861 7474 7269 6275 7465 203d  Each(attribute =
+00002d30: 3e20 7b0a 0a20 2020 2020 2020 2020 2020  > {..           
+00002d40: 2020 2020 2069 6620 2821 6973 4a53 4f4e       if (!isJSON
+00002d50: 2874 6869 732e 6765 7441 7474 7269 6275  (this.getAttribu
+00002d60: 7465 2861 7474 7269 6275 7465 2929 2920  te(attribute))) 
+00002d70: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002d80: 2020 2020 2020 6461 7461 2e73 6574 2861        data.set(a
+00002d90: 7474 7269 6275 7465 2c20 7468 6973 2e67  ttribute, this.g
+00002da0: 6574 4174 7472 6962 7574 6528 6174 7472  etAttribute(attr
+00002db0: 6962 7574 6529 293b 0a20 2020 2020 2020  ibute));.       
+00002dc0: 2020 2020 2020 2020 207d 2065 6c73 6520           } else 
+00002dd0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00002de0: 2020 2020 2020 6461 7461 2e73 6574 2861        data.set(a
+00002df0: 7474 7269 6275 7465 2c20 4a53 4f4e 2e70  ttribute, JSON.p
+00002e00: 6172 7365 2874 6869 732e 6765 7441 7474  arse(this.getAtt
+00002e10: 7269 6275 7465 2861 7474 7269 6275 7465  ribute(attribute
+00002e20: 2929 293b 0a20 2020 2020 2020 2020 2020  )));.           
+00002e30: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00002e40: 2020 207d 293b 0a20 2020 2020 2020 2020     });.         
+00002e50: 2020 2072 6574 7572 6e20 6461 7461 3b0a     return data;.
+00002e60: 2020 2020 2020 2020 7d0a 0a20 2020 207d          }..    }
+00002e70: 0a0a 2020 2020 6375 7374 6f6d 456c 656d  ..    customElem
+00002e80: 656e 7473 2e64 6566 696e 6528 636f 6d70  ents.define(comp
+00002e90: 6f6e 656e 744e 616d 652c 2058 436f 6d70  onentName, XComp
+00002ea0: 6f6e 656e 7429 3b0a 7d29 3b              onent);.});
```

### Comparing `uidom-0.1.1b6/uidom/edge_db/ql.py` & `uidom-0.2a0/uidom/edge_db/ql.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,60 +1,75 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 from dataclasses import dataclass, is_dataclass
-#TODO: WIP
+
+# TODO: WIP
 from datetime import datetime
 from typing import get_args
 
-from valio import (BOOL, CHOICE, DATE_TIME_DELTA, DEBUG, DEFAULT, DOC, INT,
-                   NAME, PATTERN, STR, VALUE, TypeValidator, Validator,
-                   email_pattern)
+from valio import (
+    BOOL,
+    CHOICE,
+    DATE_TIME_DELTA,
+    DEBUG,
+    DEFAULT,
+    DOC,
+    INT,
+    NAME,
+    PATTERN,
+    STR,
+    VALUE,
+    TypeValidator,
+    Validator,
+    email_pattern,
+)
 
 
 class EdgeQLValidator(Validator):
     exclusive: BOOL = TypeValidator(logger=False, debug=True)
-    
-    def __init__(self, 
-                 default: DEFAULT = None, 
-                 name: NAME = None, 
-                 doc: DOC = None, 
-                 required: BOOL = None, 
-                 pattern: PATTERN = None, 
-                 reassign: BOOL = None, 
-                 multiple_of: VALUE = None, 
-                 min_value: VALUE = None, 
-                 value: VALUE = None, 
-                 max_value: VALUE = None, 
-                 gt: VALUE = None, 
-                 eq: VALUE = None, 
-                 lt: VALUE = None, 
-                 min_length: INT = None, 
-                 length: INT = None, 
-                 max_length: INT = None, 
-                 expire_after: DATE_TIME_DELTA = None, 
-                 expire_on: DATE_TIME_DELTA = None, 
-                 expire_before: DATE_TIME_DELTA = None, 
-                 in_choice: CHOICE = None, 
-                 not_in_choice: CHOICE = None, 
-                 has_attributes: list[STR] = None, 
-                 task_interval: INT = None, 
-                 cache_task: BOOL = True, 
-                 debug: DEBUG = None, 
-                 cache_validation: BOOL = None, 
-                 enable_async: BOOL = None, 
-                 allow_validation: BOOL = True, 
-                 exclusive: BOOL = None, 
-                 **kwargs
-                 ):
-        
+
+    def __init__(
+        self,
+        default: DEFAULT = None,
+        name: NAME = None,
+        doc: DOC = None,
+        required: BOOL = None,
+        pattern: PATTERN = None,
+        reassign: BOOL = None,
+        multiple_of: VALUE = None,
+        min_value: VALUE = None,
+        value: VALUE = None,
+        max_value: VALUE = None,
+        gt: VALUE = None,
+        eq: VALUE = None,
+        lt: VALUE = None,
+        min_length: INT = None,
+        length: INT = None,
+        max_length: INT = None,
+        expire_after: DATE_TIME_DELTA = None,
+        expire_on: DATE_TIME_DELTA = None,
+        expire_before: DATE_TIME_DELTA = None,
+        in_choice: CHOICE = None,
+        not_in_choice: CHOICE = None,
+        has_attributes: list[STR] = None,
+        task_interval: INT = None,
+        cache_task: BOOL = True,
+        debug: DEBUG = None,
+        cache_validation: BOOL = None,
+        enable_async: BOOL = None,
+        allow_validation: BOOL = True,
+        exclusive: BOOL = None,
+        **kwargs,
+    ):
+
         self.exclusive = exclusive
-        
+
         super().__init__(
             default=default,
             name=name,
             doc=doc,
             required=required,
             pattern=pattern,
             reassign=reassign,
@@ -76,171 +91,261 @@
             has_attributes=has_attributes,
             task_interval=task_interval,
             cache_task=cache_task,
             debug=debug,
             cache_validation=cache_validation,
             enable_async=enable_async,
             allow_validation=allow_validation,
-            **kwargs)
-    
+            **kwargs,
+        )
+
     def __set_name__(self, owner, name):
         super(EdgeQLValidator, self).__set_name__(owner=owner, name=name)
         if getattr(owner, "create", None) is None:
-            setattr(owner, "create", '')
-            
-        abstract = None 
+            setattr(owner, "create", "")
+
+        abstract = None
         exclusive = None
-        required = None 
-        reassign = None 
+        required = None
+        reassign = None
         min_value = None
-        max_value = None 
-        min_length = None 
-        max_length = None 
+        max_value = None
+        min_length = None
+        max_length = None
         pattern = None
         in_choice = None
         default = None
         constraint = None
         try:
-            Meta = getattr(owner, 'Meta', None)
-            abstract = getattr(Meta, 'abstract', None)
+            Meta = getattr(owner, "Meta", None)
+            abstract = getattr(Meta, "abstract", None)
         except:
-            pass 
-        
+            pass
+
         try:
             exclusive = self.exclusive
         except KeyError as ke:
             pass
 
         try:
             required = self.required
-        except KeyError as ke: 
-            pass 
-        
-        try: 
+        except KeyError as ke:
+            pass
+
+        try:
             reassign = self.reassign
-        except KeyError as ke: 
-            pass 
-        
-        try: 
+        except KeyError as ke:
+            pass
+
+        try:
             min_value = self.min_value
-        except KeyError as ke: 
-            pass 
-        
-        try: 
+        except KeyError as ke:
+            pass
+
+        try:
             max_value = self.max_value
-        except KeyError as ke: 
-            pass 
-        
-        try: 
+        except KeyError as ke:
+            pass
+
+        try:
             min_length = self.min_length
-        except KeyError as ke: 
+        except KeyError as ke:
             pass
-        
-        try: 
+
+        try:
             max_length = self.max_length
-        except KeyError as ke: 
+        except KeyError as ke:
             pass
-        
-        try: 
+
+        try:
             pattern = self.pattern
-        except KeyError as ke: 
+        except KeyError as ke:
             pass
-        
+
         try:
             in_choice = self.in_choice
         except KeyError as ke:
-            pass 
-        
+            pass
+
         try:
             default = self.default
         except KeyError as ke:
             pass
-        
-        if any([exclusive, reassign is not None and not reassign, min_length, max_length, min_value, max_value, pattern, in_choice, default]):
-            constraint = True 
-        
+
+        if any(
+            [
+                exclusive,
+                reassign is not None and not reassign,
+                min_length,
+                max_length,
+                min_value,
+                max_value,
+                pattern,
+                in_choice,
+                default,
+            ]
+        ):
+            constraint = True
+
         args = get_args(owner.__annotations__[name])
         if any(args):
             if any(get_args(args[0])):
                 annotation_name = get_args(args[0])[0].__name__
             else:
-                 annotation_name = args[0].__name__
-        else:            
-            annotation_name = self.annotation.__name__ if not isinstance(self.annotation, str) else self.annotation
-             
-        owner.create += f"{'abstract ' if abstract is not None and abstract else ''}type {owner.__name__}" + " {" if owner.create == '' else ''
+                annotation_name = args[0].__name__
+        else:
+            annotation_name = (
+                self.annotation.__name__
+                if not isinstance(self.annotation, str)
+                else self.annotation
+            )
+
+        owner.create += (
+            f"{'abstract ' if abstract is not None and abstract else ''}type {owner.__name__}"
+            + " {"
+            if owner.create == ""
+            else ""
+        )
 
         if owner.create.endswith("\n\t};\n}") or owner.create.endswith("\n}"):
             owner.create = owner.create[:-2]
-        
-        
+
         if not is_dataclass(owner.__annotations__[name] if not any(args) else args[0]):
             if required:
-                owner.create += f"\n\trequired property {name} -> {annotation_name};" if not any(args) else f"\n\trequired multi property {name} -> array<<{annotation_name}>>;"
+                owner.create += (
+                    f"\n\trequired property {name} -> {annotation_name};"
+                    if not any(args)
+                    else f"\n\trequired multi property {name} -> array<<{annotation_name}>>;"
+                )
             else:
-                owner.create += f"\n\tproperty {name} -> {annotation_name};" if not any(args) else f"\n\tmulti property {name} -> array<<{annotation_name}>>;"
+                owner.create += (
+                    f"\n\tproperty {name} -> {annotation_name};"
+                    if not any(args)
+                    else f"\n\tmulti property {name} -> array<<{annotation_name}>>;"
+                )
         else:
             if required:
-                owner.create += f"\n\trequired link {name} -> {annotation_name};" if not any(args) else f"\n\trequired multi link {name} -> {annotation_name};"
+                owner.create += (
+                    f"\n\trequired link {name} -> {annotation_name};"
+                    if not any(args)
+                    else f"\n\trequired multi link {name} -> {annotation_name};"
+                )
             else:
-                owner.create += f"\n\tlink {name} -> {annotation_name};" if not any(args) else f"\n\tmulti link {name} -> {annotation_name};"
+                owner.create += (
+                    f"\n\tlink {name} -> {annotation_name};"
+                    if not any(args)
+                    else f"\n\tmulti link {name} -> {annotation_name};"
+                )
 
         if constraint:
-            if owner.create.endswith(';'):
+            if owner.create.endswith(";"):
                 owner.create = owner.create[:-1]
             owner.create += "\n\t{"
 
-        owner.create += '''\n\t\tconstraint exclusive;''' if exclusive is not None and exclusive else ''
-        owner.create += '''\n\t\treadonly := true;''' if not reassign and reassign is not None else ''
-        owner.create += f'''\n\t\tconstraint min_value({min_value});''' if min_value and min_value is not None else ''
-        owner.create += f'''\n\t\tconstraint max_value({max_value});''' if max_value and max_value is not None else ''
-        owner.create += f'''\n\t\tconstraint min_len_value({min_length});''' if min_length and min_length is not None else ''
-        owner.create += f'''\n\t\tconstraint max_len_value({max_length});''' if max_length and max_length is not None else ''
-        owner.create += f'''\n\t\tconstraint regexp({pattern});''' if pattern and pattern is not None else ''
-        owner.create += f'''\n\t\tconstraint one_of({in_choice});''' if in_choice and in_choice is not None else ''
+        owner.create += (
+            """\n\t\tconstraint exclusive;"""
+            if exclusive is not None and exclusive
+            else ""
+        )
+        owner.create += (
+            """\n\t\treadonly := true;"""
+            if not reassign and reassign is not None
+            else ""
+        )
+        owner.create += (
+            f"""\n\t\tconstraint min_value({min_value});"""
+            if min_value and min_value is not None
+            else ""
+        )
+        owner.create += (
+            f"""\n\t\tconstraint max_value({max_value});"""
+            if max_value and max_value is not None
+            else ""
+        )
+        owner.create += (
+            f"""\n\t\tconstraint min_len_value({min_length});"""
+            if min_length and min_length is not None
+            else ""
+        )
+        owner.create += (
+            f"""\n\t\tconstraint max_len_value({max_length});"""
+            if max_length and max_length is not None
+            else ""
+        )
+        owner.create += (
+            f"""\n\t\tconstraint regexp({pattern});"""
+            if pattern and pattern is not None
+            else ""
+        )
+        owner.create += (
+            f"""\n\t\tconstraint one_of({in_choice});"""
+            if in_choice and in_choice is not None
+            else ""
+        )
         if not self.annotation is datetime:
-            owner.create += f'''\n\t\tdefault := {self.default if not callable(self.default) else self.default.__qualname__};''' if default is not None else ''
+            owner.create += (
+                f"""\n\t\tdefault := {self.default if not callable(self.default) else self.default.__qualname__};"""
+                if default is not None
+                else ""
+            )
         else:
             if self.default in [datetime.now, datetime.utcnow]:
-                owner.create += f'''\n\t\tdefault := datetime_current()'''
-                
+                owner.create += f"""\n\t\tdefault := datetime_current()"""
+
         if constraint:
             owner.create += "\n\t}"
-            
+
         owner.create += "\n}"
 
-    
+
 @dataclass
 class User(object):
-    create = ''
-    created_at: datetime = EdgeQLValidator(logger=False, debug=True, required=True, default=datetime.utcnow)
-    updated_at: datetime = EdgeQLValidator(logger=False, debug=True, reassign=True, default=datetime.utcnow)
+    create = ""
+    created_at: datetime = EdgeQLValidator(
+        logger=False, debug=True, required=True, default=datetime.utcnow
+    )
+    updated_at: datetime = EdgeQLValidator(
+        logger=False, debug=True, reassign=True, default=datetime.utcnow
+    )
     name: str = EdgeQLValidator(
-        logger=False, 
-        required=True, 
-        reassign=False, 
-        debug=True, 
+        logger=False,
+        required=True,
+        reassign=False,
+        debug=True,
         min_length=4,
-        default='Guest',
+        default="Guest",
         exclusive=True,
-        )
-    email_ids: list[str] | None = EdgeQLValidator(logger=False, debug=True, pattern=email_pattern)
+    )
+    email_ids: list[str] | None = EdgeQLValidator(
+        logger=False, debug=True, pattern=email_pattern
+    )
 
     class Meta:
         abstract: bool = True
 
+
 @dataclass
 class SocialMedia(object):
-    media_host: str = EdgeQLValidator(logger=False, debug=True, pattern=r"^https?://www.|www.\w{2,}.(net|com|edu|app|io|tech|store|biz|in|us|co.in)")
+    media_host: str = EdgeQLValidator(
+        logger=False,
+        debug=True,
+        pattern=r"^https?://www.|www.\w{2,}.(net|com|edu|app|io|tech|store|biz|in|us|co.in)",
+    )
     media_handle: str = EdgeQLValidator(logger=False, debug=True)
 
 
 @dataclass
 class Account(object):
-    users: list[User] = EdgeQLValidator(logger=False, debug=True, required=True, default=User(name="Guest"))
+    users: list[User] = EdgeQLValidator(
+        logger=False, debug=True, required=True, default=User(name="Guest")
+    )
     media: list[SocialMedia] = EdgeQLValidator(logger=False, debug=True)
-    
-    
-# if __name__ == '__main__':
-    # print(Account(users=[User(name="User-1"), User(name="User-2")], 
-    #               media=[SocialMedia(media_host="www.youtube.com", media_handle="unique1")]))
-    # print(User.create)
+
+
+# if __name__ == "__main__":
+#     print(
+#         Account(
+#             users=[User(name="User-1"), User(name="User-2")],
+#             media=[SocialMedia(media_host="www.youtube.com", media_handle="unique1")],
+#         )
+#     )
+#     print(User.create)
```

### Comparing `uidom-0.1.1b6/uidom/settings/commands.py` & `uidom-0.2a0/uidom/settings/commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,85 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
+import asyncio
+import logging
 import platform
 import subprocess
 import sys
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 
 import valio
+
 from uidom.settings import WebAssets
 
-__all__ = [
-    "Command",
-    "TailwindCommand"
-]
+__all__ = ["Command", "TailwindCommand"]
+
+
+logger = logging.getLogger(__name__)
+
 
 def is_windows():
-    if platform.system() == 'Windows':
+    if platform.system() == "Windows":
         return True
-    if platform.system().startswith('MINGW64_NT-'):
+    if platform.system().startswith("MINGW64_NT-"):
         return True
     return False
 
 
 IS_WINDOWS = is_windows()
 
+
 @dataclass
 class Command(object):
     # command = valito.StringField(logger=False, debug=True)
 
     def run_command(self, *cmd, **kw) -> tuple[int, list[str]]:
         # self.command.logger.info(f'# {" ".join(cmd)}')
 
-        if kw.get('shell'):
+        if kw.get("shell"):
             while isinstance(cmd, list) or isinstance(cmd, tuple):
                 cmd = cmd[0]
             # self.command.logger.debug(f'shell: {cmd}')
-        with subprocess.Popen(cmd,
-                              stdout=subprocess.PIPE,
-                              stderr=subprocess.PIPE,
-                              **kw) as p:
+        with subprocess.Popen(
+            cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, **kw
+        ) as p:
             if not p.stdout:
                 raise Exception("fail to popen")
             while p.poll() is None:
                 lines = []
-                for line_bytes in iter(p.stdout.readline, b''):
+                for line_bytes in iter(p.stdout.readline, b""):
                     line_bytes = line_bytes.rstrip()
                     try:
-                        line = line_bytes.decode(encoding)
+                        line = line_bytes.decode(kw.get("encoding"))
                     except (Exception,):
-                        encoding = 'utf-8'
+                        encoding = "utf-8"
                         line = line_bytes.decode(encoding)
                     # self.command.logger.debug(line.rstrip())
                     lines.append(line)
                 returncode = p.wait()
         if returncode != 0:
             raise subprocess.CalledProcessError(returncode, cmd)
         return p.returncode, lines
 
 
-GROUPS = Union[str, list[str], None]
+# GROUPS = Union[str, list[str], None]
 
 
-class GroupValidator(valio.Validator):
-    annotation = GROUPS
+# class GroupValidator(valio.Validator):
+#     annotation = GROUPS
 
 
-class GroupField(valio.Field):
-    validator = GroupValidator
+# class GroupField(valio.Field):
+#     validator = GroupValidator
 
 
 # @dataclass
 # class Group(Command):
 #     groups = GroupField(logger=False, debug=True)
 #
 #     @groups.add_post_validator
@@ -111,111 +115,132 @@
 
 
 @dataclass
 class TailwindCommand(Command):
     tailwindcss = TailwindValidator(debug=True, logger=False, default="tailwindcss")
     file_path: Union[str, Path]
     webassets: WebAssets
-    input_file: Union[str, Path]
-    output_file: Union[str, Path]
+    input_css: Optional[Union[str, Path]] = field(default="tailwind.css")
+    output_css: Optional[Union[str, Path]] = field(default="styles.css")
     minify: bool = False
 
     def __post_init__(self):
-        self.root_dir = self.webassets.directory.ROOT_DIR
-        self.project_dir = Path(self.file_path).parent
-        self.input_file = self.root_dir / self.input_file
-        self.output_file = self.webassets.static.css / self.output_file
-        sys.exit(self.init_tailwind_project())
+        self._root_dir = self.webassets.dir
+        self._project_dir = Path(self.file_path).parent
+        self._input_file = self._root_dir / self.input_css
+        self._output_file = self.webassets.static.css / self.output_css
+        self.init_tailwind_project()
 
     def init_tailwind_project(self):
         if self.is_tailwindcss_available():
-            tailwind_config_js = (self.root_dir / 'tailwind.config.js')
+            tailwind_config_js = self._root_dir / "tailwind.config.js"
             if not tailwind_config_js.exists():
-                print("initialising Tailwindcss Config")
-                self.init_tailwind_config(init_dir=self.root_dir)
+                logger.info("initialising Tailwindcss Config")
+                self.init_tailwind_config(init_dir=self._root_dir)
                 if tailwind_config_js.exists():
                     with tailwind_config_js.open("w", encoding="utf-8") as tw:
-                        tw.write(f'''
-    module.exports = {{
-        mode: "jit",
-        content: {{
-            files:[
-            "../../{self.project_dir.relative_to(self.root_dir.parent.parent)}/*.{{html,py}}",
-            "../../{self.project_dir.relative_to(self.root_dir.parent.parent)}/**/*.{{html,py}}",
-            "../../{self.project_dir.relative_to(self.root_dir.parent.parent)}/**/**/*.{{html,py}}",
-            ]
-          }},
-        plugins: [
-            require('@tailwindcss/aspect-ratio'),
-            require('@tailwindcss/forms'),
-            require('@tailwindcss/line-clamp'),
-            require('@tailwindcss/typography'),
-            require('tailwindcss/colors'),
-        ],
-        theme: {{
-            extend: {{}}
-        }}
-        
-        }}''')
-            if not self.input_file.exists() and tailwind_config_js.exists():
-                with self.input_file.open("w", encoding="utf-8") as f:
-                    f.write('''@tailwind base;\n@tailwind components;\n@tailwind utilities;''')
-
-    def run_command(self, *cmd, **kw) -> tuple[int, list[str]]:
-        # self.command.logger.info(f'# {" ".join(cmd)}')
-
-        if kw.get('shell'):
-            while isinstance(cmd, list) or isinstance(cmd, tuple):
-                cmd = cmd[0]
-            # self.command.logger.debug(f'shell: {cmd}')
-        with subprocess.Popen(cmd,
-                              stdout=subprocess.PIPE,
-                              stderr=subprocess.PIPE,
-                              **kw) as p:
-            if not p.stdout:
-                raise Exception("fail to popen")
-            while p.poll() is None:
-                lines = []
-                for line_bytes in iter(p.stdout.readline, b''):
-                    line_bytes = line_bytes.rstrip()
-                    try:
-                        line = line_bytes.decode(encoding)
-                    except (Exception,):
-                        encoding = 'utf-8'
-                        line = line_bytes.decode(encoding)
-                    # self.command.logger.debug(line.rstrip())
-                    lines.append(line)
-                returncode = p.wait()
-        if returncode != 0:
-            raise subprocess.CalledProcessError(returncode, cmd)
-        return p.returncode, lines
+                        tw.write(
+                            f"""module.exports = {{
+    mode: "jit",
+    darkMode: "class",
+    content: {{
+        files:[
+        "../../{self._project_dir.relative_to(self._root_dir.parent.parent)}/*.{{html,py}}",
+        "../../{self._project_dir.relative_to(self._root_dir.parent.parent)}/**/*.{{html,py}}",
+        "../../{self._project_dir.relative_to(self._root_dir.parent.parent)}/**/**/*.{{html,py}}",
+        ]
+        }},
+    plugins: [
+        require('@tailwindcss/aspect-ratio'),
+        require('@tailwindcss/forms'),
+        require('@tailwindcss/line-clamp'),
+        require('@tailwindcss/typography'),
+        require('tailwindcss/colors'),
+    ],
+    theme: {{
+        extend: {{}}
+    }}
+    
+    }}"""
+                        )
+            if not self._input_file.exists() and tailwind_config_js.exists():
+                with self._input_file.open("w", encoding="utf-8") as f:
+                    f.write(
+                        """@tailwind base;\n@tailwind components;\n@tailwind utilities;"""
+                    )
 
     def is_tailwindcss_available(self):
-        output = subprocess.run([self.tailwindcss], cwd=self.root_dir.as_posix().encode() if not IS_WINDOWS else str(self.root_dir).encode())
-        print("tailwindcss command :> ", output)
+        output = subprocess.run(
+            ["which" if not IS_WINDOWS else "where", self.tailwindcss],
+            cwd=self._root_dir.as_posix().encode()
+            if not IS_WINDOWS
+            else str(self._root_dir).encode(),
+            stdout=subprocess.DEVNULL,
+            stderr=subprocess.PIPE,
+        )
+        # logger.info("tailwindcss command :> ", output)
         return output
 
     def init_tailwind_config(self, init_dir: Path):
-        print("trying to init tailwindcss config")
-        output = subprocess.run([self.tailwindcss, "init"], cwd=init_dir.as_posix().encode() if not IS_WINDOWS else str(self.root_dir).encode())
-        print("intialisation > ", bool(output))
-
-    def start(self):
-        print("cwd", self.root_dir)
-        print("input_file > ", self.input_file)
-        print("output_file > ", self.output_file)
+        logger.info("trying to init tailwindcss config")
+        output = subprocess.run(
+            [self.tailwindcss, "init"],
+            cwd=init_dir.as_posix().encode()
+            if not IS_WINDOWS
+            else str(self._root_dir).encode(),
+        )
+        logger.info(f"intialisation: { bool(output)}")
+
+    def run(self):
+        logger.info(f"cwd: { self._root_dir}")
+        logger.info(f"input_file: { self._input_file}")
+        logger.info(f"output_file: { self._output_file}")
         try:
-            output = subprocess.run([
-                self.tailwindcss,
-                '-i', self.input_file.relative_to(self.root_dir),
-                "-o", self.output_file.relative_to(self.root_dir),
-                f"--{(self.minify and 'minify') or 'watch'}",
+            output = subprocess.run(
+                [
+                    self.tailwindcss,
+                    "-i",
+                    self._input_file.relative_to(self._root_dir),
+                    "-o",
+                    self._output_file.relative_to(self._root_dir),
+                    f"--{(self.minify and 'minify') or 'watch'}",
                 ],
-                cwd=self.root_dir
+                cwd=self._root_dir,
             )
             return output
         except (Exception,) as e:
-            print(e)
+            logger.error(e)
+
+    async def async_run(self):
+        logger.info(f"cwd: { self._root_dir}")
+        logger.info(f"input_file: { self._input_file}")
+        logger.info(f"output_file: { self._output_file}")
+
+        try:
+            if not hasattr(self, "_tailwind_process"):
+                tailwind_process = asyncio.create_subprocess_shell(
+                    " ".join(
+                        [
+                            self.tailwindcss,
+                            "-i",
+                            str(self._input_file.relative_to(self._root_dir)),
+                            "-o",
+                            str(self._output_file.relative_to(self._root_dir)),
+                            f"--{(self.minify and 'minify') or 'watch'}",
+                        ]
+                    ),
+                    cwd=self._root_dir,
+                    stdout=subprocess.PIPE,  # if you want the output in the terminal comment this line
+                    stderr=subprocess.PIPE,
+                )
+                self._tailwind_process = tailwind_process
+            process = await self._tailwind_process
+            stdout, stderr = await process.communicate()
+            logger.info(f"Output: { stdout}")
+            logger.info(f"Error: { stderr}")
+        except (Exception,) as e:
+            logger.error(e)
+
 
 #
 # if __name__ == "__main__":
 #     print(Group(["asdf", "kubctrl"]).exists())
```

### Comparing `uidom-0.1.1b6/uidom/settings/paths.py` & `uidom-0.2a0/uidom/settings/paths.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # Copyright (c) 2022 uidom
-# 
+#
 # This software is released under the MIT License.
 # https://opensource.org/licenses/MIT
 
 
-
 import os
 from collections.abc import Iterable
 from typing import List, Union
 
-__all__ = [
-    "make_paths"
-]
+__all__ = ["make_paths", "MakePath"]
 
 
 def path_exists(path):
     if not os.path.isabs(path):
         path = os.path.abspath(path)
     path_exist = os.path.exists(path)
     return path_exist
```

