# Comparing `tmp/arc_cli-8.3.0.tar.gz` & `tmp/arc_cli-8.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arc_cli-8.3.0.tar", max compression
+gzip compressed data, was "arc_cli-8.4.0.tar", max compression
```

## Comparing `arc_cli-8.3.0.tar` & `arc_cli-8.4.0.tar`

### file list

```diff
@@ -1,76 +1,77 @@
--rw-r--r--   0        0        0     1053 2023-05-04 03:31:42.938647 arc_cli-8.3.0/README.md
--rw-r--r--   0        0        0      737 2023-05-08 17:17:44.700548 arc_cli-8.3.0/arc/__init__.py
--rw-r--r--   0        0        0     1449 2023-05-04 03:31:42.938647 arc_cli-8.3.0/arc/api.py
--rw-r--r--   0        0        0     6902 2023-05-04 03:31:42.938647 arc_cli-8.3.0/arc/autocompletions.py
--rw-r--r--   0        0        0     2189 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/autoload.py
--rw-r--r--   0        0        0      114 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/color.py
--rw-r--r--   0        0        0     6534 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/config.py
--rw-r--r--   0        0        0      385 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/constants.py
--rw-r--r--   0        0        0      121 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/__init__.py
--rw-r--r--   0        0        0     1379 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/alias.py
--rw-r--r--   0        0        0     1768 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/classful.py
--rw-r--r--   0        0        0    16932 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/define/command.py
--rw-r--r--   0        0        0     3101 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/documentation.py
--rw-r--r--   0        0        0      219 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/__init__.py
--rw-r--r--   0        0        0     8036 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/constructors.py
--rw-r--r--   0        0        0     3499 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/groups.py
--rw-r--r--   0        0        0     8706 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/param.py
--rw-r--r--   0        0        0     8549 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/param_definition.py
--rw-r--r--   0        0        0     3388 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/param_mixin.py
--rw-r--r--   0        0        0     1889 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/define/param/param_tree.py
--rw-r--r--   0        0        0     6314 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/errors.py
--rw-r--r--   0        0        0     1070 2023-05-04 03:31:42.941981 arc_cli-8.3.0/arc/logging.py
--rw-r--r--   0        0        0    16336 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/parser.py
--rw-r--r--   0        0        0      402 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/__init__.py
--rw-r--r--   0        0        0     6168 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/ansi.py
--rw-r--r--   0        0        0     4681 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/box.py
--rw-r--r--   0        0        0     5319 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/console.py
--rw-r--r--   0        0        0      187 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/data.py
--rw-r--r--   0        0        0     2126 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/drawing.py
--rw-r--r--   0        0        0     2748 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/formatters.py
--rw-r--r--   0        0        0     9376 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/help_formatter.py
--rw-r--r--   0        0        0     3024 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/joiner.py
--rw-r--r--   0        0        0       54 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/markdown/__init__.py
--rw-r--r--   0        0        0     6614 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/markdown/markdown_parser.py
--rw-r--r--   0        0        0     3894 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/markdown/nodes.py
--rw-r--r--   0        0        0     1632 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/out.py
--rw-r--r--   0        0        0      987 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/pager.py
--rw-r--r--   0        0        0     9825 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/table.py
--rw-r--r--   0        0        0     5182 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/present/wrap.py
--rw-r--r--   0        0        0      288 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/prompt/__init__.py
--rw-r--r--   0        0        0     3722 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/prompt/helpers.py
--rw-r--r--   0        0        0     5926 2023-05-04 03:31:42.945314 arc_cli-8.3.0/arc/prompt/prompt.py
--rw-r--r--   0        0        0      812 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/prompt/prompts.py
--rw-r--r--   0        0        0     7019 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/prompt/questions.py
--rw-r--r--   0        0        0        0 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/py.typed
--rw-r--r--   0        0        0      304 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/app.py
--rw-r--r--   0        0        0     2678 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/runtime/context.py
--rw-r--r--   0        0        0    12517 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/runtime/exec.py
--rw-r--r--   0        0        0     8933 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/init.py
--rw-r--r--   0        0        0     7409 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/middleware.py
--rw-r--r--   0        0        0     3097 2023-05-08 17:17:15.750745 arc_cli-8.3.0/arc/runtime/plugin.py
--rw-r--r--   0        0        0      382 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/safe.py
--rw-r--r--   0        0        0     1866 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/suggest.py
--rw-r--r--   0        0        0      362 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/types/__init__.py
--rw-r--r--   0        0        0    13898 2023-05-04 03:31:42.948647 arc_cli-8.3.0/arc/types/aliases.py
--rw-r--r--   0        0        0      670 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/convert.py
--rw-r--r--   0        0        0      545 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/default.py
--rw-r--r--   0        0        0     4422 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/file.py
--rw-r--r--   0        0        0       79 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/middleware/__init__.py
--rw-r--r--   0        0        0     1403 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/middleware/observers.py
--rw-r--r--   0        0        0     2630 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/middleware/transformers.py
--rw-r--r--   0        0        0     4042 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/middleware/validators.py
--rw-r--r--   0        0        0     3486 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/network.py
--rw-r--r--   0        0        0      854 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/numbers.py
--rw-r--r--   0        0        0      860 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/path.py
--rw-r--r--   0        0        0     6881 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/semver.py
--rw-r--r--   0        0        0      877 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/state.py
--rw-r--r--   0        0        0     1921 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/strings.py
--rw-r--r--   0        0        0     2155 2023-05-04 03:31:42.951981 arc_cli-8.3.0/arc/types/type_arg.py
--rw-r--r--   0        0        0     2718 2023-05-04 03:31:42.955314 arc_cli-8.3.0/arc/types/type_info.py
--rw-r--r--   0        0        0     3176 2023-05-04 03:31:42.955314 arc_cli-8.3.0/arc/types/users.py
--rw-r--r--   0        0        0     2257 2023-05-04 03:31:42.955314 arc_cli-8.3.0/arc/typing.py
--rw-r--r--   0        0        0     1116 2023-05-08 17:17:45.363876 arc_cli-8.3.0/pyproject.toml
--rw-r--r--   0        0        0     1810 1970-01-01 00:00:00.000000 arc_cli-8.3.0/setup.py
--rw-r--r--   0        0        0     1782 1970-01-01 00:00:00.000000 arc_cli-8.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-10 21:06:03.754164 arc_cli-8.4.0/LICENSE
+-rw-r--r--   0        0        0     1055 2023-05-10 21:03:18.235657 arc_cli-8.4.0/README.md
+-rw-r--r--   0        0        0      737 2023-05-10 21:08:09.333093 arc_cli-8.4.0/arc/__init__.py
+-rw-r--r--   0        0        0     1449 2023-05-08 22:45:01.072694 arc_cli-8.4.0/arc/api.py
+-rw-r--r--   0        0        0     6902 2023-05-08 22:45:01.072694 arc_cli-8.4.0/arc/autocompletions.py
+-rw-r--r--   0        0        0     2189 2023-05-08 22:45:01.072694 arc_cli-8.4.0/arc/autoload.py
+-rw-r--r--   0        0        0      114 2023-05-04 03:31:42.941981 arc_cli-8.4.0/arc/color.py
+-rw-r--r--   0        0        0     6534 2023-05-08 22:45:01.072694 arc_cli-8.4.0/arc/config.py
+-rw-r--r--   0        0        0      385 2023-05-08 22:45:01.072694 arc_cli-8.4.0/arc/constants.py
+-rw-r--r--   0        0        0      121 2023-05-04 03:31:42.941981 arc_cli-8.4.0/arc/define/__init__.py
+-rw-r--r--   0        0        0     1379 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/define/alias.py
+-rw-r--r--   0        0        0     1768 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/define/classful.py
+-rw-r--r--   0        0        0    16932 2023-05-10 02:23:27.369848 arc_cli-8.4.0/arc/define/command.py
+-rw-r--r--   0        0        0     3101 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/define/documentation.py
+-rw-r--r--   0        0        0      219 2023-05-04 03:31:42.941981 arc_cli-8.4.0/arc/define/param/__init__.py
+-rw-r--r--   0        0        0     8036 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/define/param/constructors.py
+-rw-r--r--   0        0        0     3499 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/define/param/groups.py
+-rw-r--r--   0        0        0     8694 2023-05-10 04:09:53.192864 arc_cli-8.4.0/arc/define/param/param.py
+-rw-r--r--   0        0        0     8549 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/define/param/param_definition.py
+-rw-r--r--   0        0        0     3388 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/define/param/param_mixin.py
+-rw-r--r--   0        0        0     1889 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/define/param/param_tree.py
+-rw-r--r--   0        0        0     6314 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/errors.py
+-rw-r--r--   0        0        0     1070 2023-05-10 02:23:27.369848 arc_cli-8.4.0/arc/logging.py
+-rw-r--r--   0        0        0    16336 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/parser.py
+-rw-r--r--   0        0        0      402 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/__init__.py
+-rw-r--r--   0        0        0     6168 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/ansi.py
+-rw-r--r--   0        0        0     4681 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/box.py
+-rw-r--r--   0        0        0     5319 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/console.py
+-rw-r--r--   0        0        0      187 2023-05-04 03:31:42.945314 arc_cli-8.4.0/arc/present/data.py
+-rw-r--r--   0        0        0     2126 2023-05-04 03:31:42.945314 arc_cli-8.4.0/arc/present/drawing.py
+-rw-r--r--   0        0        0     2748 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/formatters.py
+-rw-r--r--   0        0        0     9376 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/help_formatter.py
+-rw-r--r--   0        0        0     3024 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/joiner.py
+-rw-r--r--   0        0        0       54 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/markdown/__init__.py
+-rw-r--r--   0        0        0     6614 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/markdown/markdown_parser.py
+-rw-r--r--   0        0        0     3894 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/markdown/nodes.py
+-rw-r--r--   0        0        0     1632 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/out.py
+-rw-r--r--   0        0        0      987 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/pager.py
+-rw-r--r--   0        0        0     9825 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/table.py
+-rw-r--r--   0        0        0     5182 2023-05-08 22:45:01.076028 arc_cli-8.4.0/arc/present/wrap.py
+-rw-r--r--   0        0        0      288 2023-05-04 03:31:42.945314 arc_cli-8.4.0/arc/prompt/__init__.py
+-rw-r--r--   0        0        0     3731 2023-05-10 04:25:05.907299 arc_cli-8.4.0/arc/prompt/helpers.py
+-rw-r--r--   0        0        0     5926 2023-05-10 04:22:13.775050 arc_cli-8.4.0/arc/prompt/prompt.py
+-rw-r--r--   0        0        0      812 2023-05-08 22:45:01.079361 arc_cli-8.4.0/arc/prompt/prompts.py
+-rw-r--r--   0        0        0     7019 2023-05-08 22:45:01.079361 arc_cli-8.4.0/arc/prompt/questions.py
+-rw-r--r--   0        0        0        0 2023-05-04 03:31:42.948647 arc_cli-8.4.0/arc/py.typed
+-rw-r--r--   0        0        0      304 2023-05-08 22:45:01.079361 arc_cli-8.4.0/arc/runtime/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-10 02:23:27.369848 arc_cli-8.4.0/arc/runtime/app.py
+-rw-r--r--   0        0        0     2786 2023-05-10 20:44:07.009272 arc_cli-8.4.0/arc/runtime/context.py
+-rw-r--r--   0        0        0    12733 2023-05-10 04:09:49.326262 arc_cli-8.4.0/arc/runtime/exec.py
+-rw-r--r--   0        0        0    10026 2023-05-10 20:39:57.711784 arc_cli-8.4.0/arc/runtime/init.py
+-rw-r--r--   0        0        0     7409 2023-05-08 22:45:01.079361 arc_cli-8.4.0/arc/runtime/middleware.py
+-rw-r--r--   0        0        0     3097 2023-05-08 22:45:01.079361 arc_cli-8.4.0/arc/runtime/plugin.py
+-rw-r--r--   0        0        0      382 2023-05-08 22:45:01.079361 arc_cli-8.4.0/arc/safe.py
+-rw-r--r--   0        0        0     1866 2023-05-08 22:45:01.079361 arc_cli-8.4.0/arc/suggest.py
+-rw-r--r--   0        0        0      362 2023-05-10 02:47:29.523000 arc_cli-8.4.0/arc/types/__init__.py
+-rw-r--r--   0        0        0    14196 2023-05-10 02:57:55.763259 arc_cli-8.4.0/arc/types/aliases.py
+-rw-r--r--   0        0        0      670 2023-05-08 22:45:01.082694 arc_cli-8.4.0/arc/types/convert.py
+-rw-r--r--   0        0        0      545 2023-05-08 22:45:01.082694 arc_cli-8.4.0/arc/types/default.py
+-rw-r--r--   0        0        0     4419 2023-05-10 03:51:44.284628 arc_cli-8.4.0/arc/types/file.py
+-rw-r--r--   0        0        0       79 2023-05-04 03:31:42.951981 arc_cli-8.4.0/arc/types/middleware/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-10 03:41:31.066410 arc_cli-8.4.0/arc/types/middleware/observers.py
+-rw-r--r--   0        0        0     2630 2023-05-08 22:45:01.082694 arc_cli-8.4.0/arc/types/middleware/transformers.py
+-rw-r--r--   0        0        0     4236 2023-05-10 02:44:59.447809 arc_cli-8.4.0/arc/types/middleware/validators.py
+-rw-r--r--   0        0        0     3486 2023-05-08 22:45:01.082694 arc_cli-8.4.0/arc/types/network.py
+-rw-r--r--   0        0        0      854 2023-05-04 03:31:42.951981 arc_cli-8.4.0/arc/types/numbers.py
+-rw-r--r--   0        0        0      860 2023-05-08 22:45:01.082694 arc_cli-8.4.0/arc/types/path.py
+-rw-r--r--   0        0        0     6881 2023-05-08 22:45:01.082694 arc_cli-8.4.0/arc/types/semver.py
+-rw-r--r--   0        0        0      877 2023-05-08 22:45:01.082694 arc_cli-8.4.0/arc/types/state.py
+-rw-r--r--   0        0        0     1960 2023-05-10 02:48:47.609034 arc_cli-8.4.0/arc/types/strings.py
+-rw-r--r--   0        0        0     2300 2023-05-10 03:16:28.712436 arc_cli-8.4.0/arc/types/type_arg.py
+-rw-r--r--   0        0        0     2718 2023-05-08 22:45:01.082694 arc_cli-8.4.0/arc/types/type_info.py
+-rw-r--r--   0        0        0     3176 2023-05-08 22:45:01.082694 arc_cli-8.4.0/arc/types/users.py
+-rw-r--r--   0        0        0     2257 2023-05-10 02:23:27.369848 arc_cli-8.4.0/arc/typing.py
+-rw-r--r--   0        0        0     1014 2023-05-10 21:08:09.956421 arc_cli-8.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 arc_cli-8.4.0/setup.py
+-rw-r--r--   0        0        0     1769 1970-01-01 00:00:00.000000 arc_cli-8.4.0/PKG-INFO
```

### Comparing `arc_cli-8.3.0/README.md` & `arc_cli-8.4.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ARC: A Regular CLI
-A tool for building declarative, and highly extendable CLI systems for Python 3.9
+A tool for building declarative, and highly extendable CLI systems for Python 3.10+
 
 # ARC Features
 - Command line arguments based on python type hints
 - Arbitrary command nesting
 - Automatic `--help` documentation
 - Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...
```

### Comparing `arc_cli-8.3.0/arc/__init__.py` & `arc_cli-8.4.0/arc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "8.3.0"
+__version__ = "8.4.0"
 
 from arc import types, prompt, present, errors
 from arc.config import (
     ColorConfig,
     Config,
     LinksConfig,
     SuggestionConfig,
```

### Comparing `arc_cli-8.3.0/arc/api.py` & `arc_cli-8.4.0/arc/api.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/autocompletions.py` & `arc_cli-8.4.0/arc/autocompletions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/autoload.py` & `arc_cli-8.4.0/arc/autoload.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/config.py` & `arc_cli-8.4.0/arc/config.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/define/alias.py` & `arc_cli-8.4.0/arc/define/alias.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/define/classful.py` & `arc_cli-8.4.0/arc/define/classful.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/define/command.py` & `arc_cli-8.4.0/arc/define/command.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/define/documentation.py` & `arc_cli-8.4.0/arc/define/documentation.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/define/param/constructors.py` & `arc_cli-8.4.0/arc/define/param/constructors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/define/param/groups.py` & `arc_cli-8.4.0/arc/define/param/groups.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/define/param/param.py` & `arc_cli-8.4.0/arc/define/param/param.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argparse
 import enum
 import typing as t
 from functools import cached_property
 
 import arc.typing as at
-from arc import api, constants, errors, safe
+from arc import api, safe
 from arc.autocompletions import CompletionInfo, get_completions
 from arc.color import colorize, fg
 from arc.constants import MISSING, Constant
 from arc.types.convert import convert_type
 from arc.types.type_info import TypeInfo
 
 T = t.TypeVar("T")
@@ -20,16 +20,16 @@
     STORE = "store"
     STORE_TRUE = "store_true"
     STORE_FALSE = "store_false"
     APPEND = "append"
     COUNT = "count"
 
 
-class ValueOrigin(enum.Enum):
-    CLI = "cli"
+class ValueOrigin:
+    COMMAND_LINE = "command_line"
     ENV = "env"
     PROMPT = "prompt"
     DEFAULT = "default"
     INJECTED = "injected"
     GETTER = "getter"
```

### Comparing `arc_cli-8.3.0/arc/define/param/param_definition.py` & `arc_cli-8.4.0/arc/define/param/param_definition.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/define/param/param_mixin.py` & `arc_cli-8.4.0/arc/define/param/param_mixin.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/define/param/param_tree.py` & `arc_cli-8.4.0/arc/define/param/param_tree.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/errors.py` & `arc_cli-8.4.0/arc/errors.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/logging.py` & `arc_cli-8.4.0/arc/logging.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/parser.py` & `arc_cli-8.4.0/arc/parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/ansi.py` & `arc_cli-8.4.0/arc/present/ansi.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/box.py` & `arc_cli-8.4.0/arc/present/box.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/console.py` & `arc_cli-8.4.0/arc/present/console.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/drawing.py` & `arc_cli-8.4.0/arc/present/drawing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/formatters.py` & `arc_cli-8.4.0/arc/present/formatters.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/help_formatter.py` & `arc_cli-8.4.0/arc/present/help_formatter.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/joiner.py` & `arc_cli-8.4.0/arc/present/joiner.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/markdown/markdown_parser.py` & `arc_cli-8.4.0/arc/present/markdown/markdown_parser.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/markdown/nodes.py` & `arc_cli-8.4.0/arc/present/markdown/nodes.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/out.py` & `arc_cli-8.4.0/arc/present/out.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/pager.py` & `arc_cli-8.4.0/arc/present/pager.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/table.py` & `arc_cli-8.4.0/arc/present/table.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/present/wrap.py` & `arc_cli-8.4.0/arc/present/wrap.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/prompt/helpers.py` & `arc_cli-8.4.0/arc/prompt/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,17 +70,18 @@
 
     @staticmethod
     def prevline(val: int = 1) -> None:
         sys.stdout.write(f"\x1b[{val}F")
 
     @staticmethod
     def getpos() -> tuple[int, int]:
-        sys.stdout.write(f"\x1b[6n")
-        sys.stdout.flush()
         with RawTerminal() as term:
+            sys.stdout.write(f"\x1b[6n")
+            sys.stdout.flush()
+
             seq = term.getch()
             while seq[-1] != "R":
                 seq += term.getch()
 
         match = re.match(r"\x1b\[(\d+);(\d+)R", seq)
         if not match:
             raise RuntimeError("Could not match position string returned")
```

### Comparing `arc_cli-8.3.0/arc/prompt/prompt.py` & `arc_cli-8.4.0/arc/prompt/prompt.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/prompt/prompts.py` & `arc_cli-8.4.0/arc/prompt/prompts.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/prompt/questions.py` & `arc_cli-8.4.0/arc/prompt/questions.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/runtime/app.py` & `arc_cli-8.4.0/arc/runtime/app.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/runtime/context.py` & `arc_cli-8.4.0/arc/runtime/context.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import arc.typing as at
 
 if t.TYPE_CHECKING:
     from logging import Logger
 
     from arc.config import Config
     from arc.define.command import Command
-    from arc.define.param.param import ValueOrigin
     from arc.prompt.prompt import Prompt
     from arc.runtime import App
 
 
 T = t.TypeVar("T")
 
 
@@ -71,27 +70,30 @@
         def sub(val: int):
             print(sub)
         ```
 
         """
         return self.app.execute(command, **kwargs)
 
+    def set_origin(self, param_name: str, origin: str) -> None:
+        """Sets the origin of a parameter"""
+        origins = self.setdefault("arc.args.origins", {})
+        origins[param_name] = origin
+
     @t.overload
-    def get_origin(self, param_name: str) -> ValueOrigin | None:
+    def get_origin(self, param_name: str) -> str | None:
         ...
 
     @t.overload
-    def get_origin(self, param_name: str, default: T) -> ValueOrigin | T:
+    def get_origin(self, param_name: str, default: T) -> str | T:
         ...
 
-    def get_origin(
-        self, param_name: str, default: T | None = None
-    ) -> ValueOrigin | T | None:
+    def get_origin(self, param_name: str, default: T | None = None) -> str | T | None:
         """Gets the origin of a paramter"""
-        origins: dict[str, ValueOrigin] | None = self.get("arc.args.origins")
+        origins: dict[str, str] | None = self.get("arc.args.origins")
 
         if not origins:
             return default
 
         return origins.get(param_name, default)
 
     @classmethod
```

### Comparing `arc_cli-8.3.0/arc/runtime/exec.py` & `arc_cli-8.4.0/arc/runtime/exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,22 +53,22 @@
     `arc.args.origins` - Dictionary that stores where each parameter value comes from. See `Context.get_origin()`
     """
 
     def __call__(self, ctx: Context) -> t.Any:
         command: Command = ctx["arc.command"]
         param_instance = command.param_def.create_instance()
         ctx["arc.args.tree"] = param_instance
-        ctx["arc.args.origins"] = {}
+        ctx.setdefault("arc.args.origins", {})
 
 
 class ParamProcessor(MiddlewareBase):
     ctx: Context
     param_tree: ParamTree[type[dict[str, t.Any]]]
     config: Config
-    origins: dict[str, ValueOrigin]
+    origins: dict[str, str]
 
     __IGNORE = object()
 
     def __call__(self, ctx: Context) -> t.Any:
         self.ctx = ctx
         self.param_tree: ParamTree[type[dict[str, t.Any]]] = ctx["arc.args.tree"]
         self.config = ctx["arc.config"]
@@ -99,15 +99,15 @@
 
     def process_not_missing(self, param: Param[t.Any], value: t.Any) -> t.Any:
         return self.__IGNORE
 
     def skip(self, param: Param[t.Any], value: t.Any) -> bool:
         return param.is_injected or not param.expose
 
-    def set_origin(self, param: Param[t.Any], origin: ValueOrigin) -> None:
+    def set_origin(self, param: Param[t.Any], origin: str) -> None:
         self.origins[param.argument_name] = origin
 
 
 class ApplyParseResultMiddleware(ParamProcessor):
     """Update the parameter values with the values found from parsing the input
 
     # Context Dependencies
@@ -124,15 +124,15 @@
 
     def __call__(self, ctx: Context) -> t.Any:
         self.res = ctx["arc.parse.result"]
         return super().__call__(ctx)
 
     def process_missing(self, param: Param[t.Any]) -> t.Any:
         value: t.Any = self.res.pop(param.argument_name, constants.MISSING)
-        self.set_origin(param, ValueOrigin.CLI)
+        self.set_origin(param, ValueOrigin.COMMAND_LINE)
 
         # This is dependent on the fact that the current parser
         # adds a None to the result when you input a keyword, but
         # with no value
         if param.is_required and value is None:
             raise errors.MissingOptionValueError(param)
 
@@ -222,24 +222,29 @@
     - `arc.args.origins`
 
     # Context Additions
     None
     """
 
     def process_not_missing(self, param: Param[t.Any], value: t.Any) -> t.Any:
-        if value in (None, constants.MISSING, True, False,) and param.type.origin in (
+        if value in (None, constants.MISSING, True, False) and param.type.origin in (
             bool,
             t.Any,
         ):
             return value
 
         try:
             return param.convert(value)
         except errors.ConversionError as e:
-            raise errors.InvalidParamValueError(str(e), param, e.details) from e
+            details = e.details
+
+            if self.ctx.get_origin(param.argument_name) == ValueOrigin.ENV:
+                details = f"Invalid value in enviroment variable: {self.config.env_prefix}{param.envvar}"
+
+            raise errors.InvalidParamValueError(str(e), param, details) from e
 
 
 class DefaultValueMiddleware(ParamProcessor):
     """Retrieves parameter values from the defaults for each parameter
 
     # Context Dependencies
     - `arc.args.tree`
```

### Comparing `arc_cli-8.3.0/arc/runtime/init.py` & `arc_cli-8.4.0/arc/runtime/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,14 +42,25 @@
             end = datetime.now()
             ctx["arc.debug.end"] = end
             diff = end - start
             ctx.logger.debug(f"Execution took: {diff.total_seconds():.4f}s")
 
 
 class LoadPluginsMiddleware(MiddlewareBase):
+    """Utility Middleware that loads plugins defined in the
+    configuration into the application and calls their hooks
+
+    # Context Dependencies
+    - `arc.config` - Configuration object
+    - `arc.app` - Application object
+
+    # Context Additions
+    None
+    """
+
     def __call__(self, ctx: Context) -> t.Any:
         ctx.logger.debug("Loading plugins...")
         app = ctx.app
         app.plugins.paths(*ctx.config.plugins.paths)
         app.plugins.groups(*ctx.config.plugins.groups)
         app.plugins.entrypoints(*ctx.config.plugins.entrypoints)
 
@@ -190,22 +201,46 @@
             ctx.logger.debug("Using provided iterable as input: %s", args)
 
         args = list(args)
         ctx["arc.input"] = args
 
 
 class CommandFinderMiddleware(MiddlewareBase):
+    """Middleware that finds the command to execute based on the input.
+    Finds the command by walking the tree of commands from the root and
+    comparing them with each next word in the input
+
+    # Context Dependencies
+    - `arc.input`: The input to find the command from
+
+    # Context Additions
+    - `arc.command`: The command to execute
+    - `arc.input`: The input to pass to the command.
+    Will be what's left of the input after removing the command path
+    """
+
     def __call__(self, ctx: Context) -> t.Any:
         args: list[str] = ctx["arc.input"]
         command, command_args = ctx.root.find_command(args)
         ctx["arc.command"] = command
         ctx["arc.input"] = command_args
 
 
 class ArgParseMiddleware(MiddlewareBase):
+    """Middleware that parses the input using the `argparse` library
+
+    # Context Dependencies
+    - `arc.command`: The command to parse the input for
+    - `arc.input`: The input to parse
+
+    # Context Additions
+    - `arc.parse.result`: The result of the parsing
+    - `arc.parse.extra`: Any extra arguments that were not parsed
+    """
+
     def __call__(self, ctx: Context) -> t.Any:
         args: list[str] = ctx["arc.input"]
 
         result, extra = self.parse_args(ctx.command, args)
         ctx["arc.parse.result"] = result
         ctx["arc.parse.extra"] = extra
 
@@ -253,15 +288,15 @@
     def command():
         arc.print("hello there")
 
     # To add your own init middlewares, you need to
     # create the App object explicitly
     app = arc.App(command)
 
-    @app.use(before=arc.InitMiddleware.Parse)
+    @app.use(before=arc.InitMiddleware.Parser)
     def before_parse(ctx: arc.Context):
         # Will run before the middleware that performs the parsing operation
         ...
 
     app()
     ```
```

### Comparing `arc_cli-8.3.0/arc/runtime/middleware.py` & `arc_cli-8.4.0/arc/runtime/middleware.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/runtime/plugin.py` & `arc_cli-8.4.0/arc/runtime/plugin.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/suggest.py` & `arc_cli-8.4.0/arc/suggest.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/aliases.py` & `arc_cli-8.4.0/arc/types/aliases.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import collections
 import enum
 import ipaddress
 import pathlib
 import re
 import types
 import typing as t
+import uuid
 
 import _io  # type: ignore
 
 from arc import api, autocompletions, errors, safe
 from arc.autocompletions import Completion, CompletionInfo, CompletionType
 from arc.color import colorize, fg
 from arc.present.joiner import Join
@@ -425,7 +426,16 @@
             ) from e
 
     @classmethod
     def flags(cls, info: TypeInfo[t.Any]) -> int:
         if len(info.annotations) == 0:
             return 0
         return info.annotations[0]
+
+
+class UUIDAlias(Alias, of=uuid.UUID):
+    @classmethod
+    def convert(cls, value: str, info: TypeInfo[t.Any]) -> uuid.UUID:
+        try:
+            return uuid.UUID(value)
+        except ValueError as e:
+            raise errors.ConversionError(value, "Not a valid UUID", e) from e
```

### Comparing `arc_cli-8.3.0/arc/types/convert.py` & `arc_cli-8.4.0/arc/types/convert.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/default.py` & `arc_cli-8.4.0/arc/types/default.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/file.py` & `arc_cli-8.4.0/arc/types/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+from __future__ import annotations
 import abc
 import sys
-import types
 import typing as t
-from dataclasses import dataclass
+from arc.define.param.param import ValueOrigin
 
 from arc.types.convert import convert_type
 from arc.types.default import Default, unwrap
 from arc.types.type_arg import TypeArg
 from arc.types.type_info import TypeInfo
 
+if t.TYPE_CHECKING:
+    from arc import Context
+
 __all__ = ["File", "Stdin"]
 
 
 OpenNewline = t.Literal[None, "", "\n", "\r", "\r\n"]
 OpenErrors = t.Literal[
     None,
     "strict",
@@ -111,39 +114,34 @@
     """Equivalent to `open(filename, "ab")`"""
     BinaryAppendRead = t.Annotated[t.BinaryIO, Args("ab+")]
     """Equivalent to `open(filename, "ab+")`"""
 
 
 T = t.TypeVar("T")
 
-StreamOrigin = t.Literal["cli", "stream"]
-
 
 class Stream(t.Generic[T]):
-    def __init__(self, value: T, origin: StreamOrigin) -> None:
+    def __init__(self, value: T) -> None:
         self.value: T = value
-        self.origin = origin
 
     @classmethod
     def __convert__(cls, value: str, info: TypeInfo[t.Any]) -> "Stream[T]":
         arg: Stream.Args = TypeArg.ensure(
             t.cast(t.Optional[Stream.Args], info.type_arg), cls.__name__
         )
 
-        origin: StreamOrigin = "cli"
-
         if value == unwrap(arg.char):
             value = arg.stream.read()
-            origin = "stream"
 
         sub = info.sub_types[0]
-        return cls(convert_type(sub.resolved_type, value, sub), origin)
+        return cls(convert_type(sub.resolved_type, value, sub))
 
     class Args(TypeArg):
         __slots__ = ("stream", "char")
 
         def __init__(self, stream: t.IO[str] = sys.stdin, char: str = Default("-")):
             self.stream = stream
             self.char = char
 
 
 Stdin = t.Annotated[Stream[T], Stream.Args(sys.stdin)]
+"""Read input from command line, or from stdin if `-` is passed as the argument"""
```

### Comparing `arc_cli-8.3.0/arc/types/middleware/observers.py` & `arc_cli-8.4.0/arc/types/middleware/observers.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,10 +54,10 @@
                 "param": param.param_name,
                 "cli": param.cli_name,
             }
 
             origin = ctx.get_origin(param.argument_name, ValueOrigin.DEFAULT)
             name = names.get(self.name_kind, param.argument_name)
 
-            ctx.logger.log(self.level, f"{name} = {value} ({origin.value})")
+            ctx.logger.log(self.level, f"{name} = {value} ({origin})")
 
         return value
```

### Comparing `arc_cli-8.3.0/arc/types/middleware/transformers.py` & `arc_cli-8.4.0/arc/types/middleware/transformers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/middleware/validators.py` & `arc_cli-8.4.0/arc/types/middleware/validators.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,31 @@
 class Matches:
     """Validator to match a regular expression.
 
     ## Type Constraints
     - Matches against `str(value)`, so the type must have a sensible string representation
     """
 
-    def __init__(self, pattern: str | re.Pattern[str], flags: int = 0):
+    def __init__(
+        self,
+        pattern: str | re.Pattern[str],
+        flags: int = 0,
+        message: str = "does not match expected format: {pattern}",
+    ):
         self.pattern = pattern
         self.flags = flags
+        self.message = message
 
     def __call__(self, value: t.Any) -> t.Any:
         if not re.match(self.pattern, str(value), self.flags):
             raise errors.ValidationError(
-                f"does not match expected format: {self.pattern}"
+                self.message.format(
+                    pattern=self.pattern,
+                    value=value,
+                )
             )
 
         return value
 
 
 class SupportsLen(t.Protocol):
     def __len__(self) -> int:
```

### Comparing `arc_cli-8.3.0/arc/types/network.py` & `arc_cli-8.4.0/arc/types/network.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/numbers.py` & `arc_cli-8.4.0/arc/types/numbers.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/path.py` & `arc_cli-8.4.0/arc/types/path.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/semver.py` & `arc_cli-8.4.0/arc/types/semver.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/state.py` & `arc_cli-8.4.0/arc/types/state.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/type_arg.py` & `arc_cli-8.4.0/arc/types/type_arg.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 from arc import errors
 from arc.types.default import isdefault, unwrap
 
 T = t.TypeVar("T")
 
 
 class TypeArg:
+    """A type argument that can be used to annotate a type.
+    This is used to provide additional information neccessary to convert a type."""
+
     __slots__: tuple[str, ...]
 
     def __repr__(self) -> str:
         values = ", ".join(
             [f"{member}={repr(getattr(self, member))}" for member in self.__slots__]
         )
         return f"{type(self).__name__}({values})"
```

### Comparing `arc_cli-8.3.0/arc/types/type_info.py` & `arc_cli-8.4.0/arc/types/type_info.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/types/users.py` & `arc_cli-8.4.0/arc/types/users.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/arc/typing.py` & `arc_cli-8.4.0/arc/typing.py`

 * *Files identical despite different names*

### Comparing `arc_cli-8.3.0/pyproject.toml` & `arc_cli-8.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 [tool.poetry]
 name = "arc-cli"
-version = "8.3.0"
-description = "A Regular CLI"
-authors = ["Sean Collings <seanrcollings@gmail.com>"]
+version = "8.4.0"
+description = "Package for creating CLI's with ease."
+authors = ["Sean Collings <me@seancollings.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/seanrcollings/arc"
-documentation = "https://arc.seanrcollings.com"
-keywords = ["CLI", "extendable", "easy", "arc"]
+documentation = "https://arc.seancollings.dev"
 classifiers= [
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
     "Typing :: Typed"
 ]
@@ -31,13 +30,10 @@
 types-PyYAML = "^6.0.1"
 mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 Jinja2 = "3.0.3"
 mkdocs-awesome-pages-plugin = "^2.8.0"
 hypothesis = "^6.68.2"
 pygithub = "^1.58.1"
 
-# [tool.poetry.plugins."arc.plugins"]
-# "test_plugin" = "plugin:plugin"
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `arc_cli-8.3.0/setup.py` & `arc_cli-8.4.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,19 +13,19 @@
  'arc.types.middleware']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'arc-cli',
-    'version': '8.3.0',
-    'description': 'A Regular CLI',
-    'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.9\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# Links\n- [Docs](https://arc.seancollings.dev)\n- [Playground](https://playground.arc.seancollings.dev)\n- [PyPi](https://pypi.org/project/arc-cli/)\n\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
+    'version': '8.4.0',
+    'description': "Package for creating CLI's with ease.",
+    'long_description': '# ARC: A Regular CLI\nA tool for building declarative, and highly extendable CLI systems for Python 3.10+\n\n# ARC Features\n- Command line arguments based on python type hints\n- Arbitrary command nesting\n- Automatic `--help` documentation\n- Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...\n\n# Links\n- [Docs](https://arc.seancollings.dev)\n- [Playground](https://playground.arc.seancollings.dev)\n- [PyPi](https://pypi.org/project/arc-cli/)\n\n\n# Quick Start\n\n```py\nimport arc\n\n@arc.command\ndef hello(name: str):\n    """My first arc program!"""\n    arc.print(f"Hello {name}!")\n\nhello()\n```\n\n```\n$ python hello.py Sean\nHello, Sean!\n```\n\n```\n$ python hello.py --help\nUSAGE\n    hello.py [-h] [--] name\n\nDESCRIPTION\n    My first arc program!\n\nARGUMENTS\n    name\n\nOPTIONS\n    --help (-h)  Displays this help message\n```\n\n# Installation\n\n```\n$ pip install arc-cli\n```\n\nClone for development\n```\n$ git clone https://github.com/seanrcollings/arc\n$ poetry install\n```\n\n# Tests\nTests are written with `pytest`\n```\n$ pytest\n```\n',
     'author': 'Sean Collings',
-    'author_email': 'seanrcollings@gmail.com',
+    'author_email': 'me@seancollings.dev',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/seanrcollings/arc',
     'packages': packages,
     'package_data': package_data,
     'python_requires': '>=3.10,<4.0',
 }
```

### Comparing `arc_cli-8.3.0/PKG-INFO` & `arc_cli-8.4.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: arc-cli
-Version: 8.3.0
-Summary: A Regular CLI
+Version: 8.4.0
+Summary: Package for creating CLI's with ease.
 Home-page: https://github.com/seanrcollings/arc
 License: MIT
-Keywords: CLI,extendable,easy,arc
 Author: Sean Collings
-Author-email: seanrcollings@gmail.com
+Author-email: me@seancollings.dev
 Requires-Python: >=3.10,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Typing :: Typed
-Project-URL: Documentation, https://arc.seanrcollings.com
+Project-URL: Documentation, https://arc.seancollings.dev
 Description-Content-Type: text/markdown
 
 # ARC: A Regular CLI
-A tool for building declarative, and highly extendable CLI systems for Python 3.9
+A tool for building declarative, and highly extendable CLI systems for Python 3.10+
 
 # ARC Features
 - Command line arguments based on python type hints
 - Arbitrary command nesting
 - Automatic `--help` documentation
 - Fully Extensible with custom middlewares,  types, validators, parameter configurations, etc...
```

