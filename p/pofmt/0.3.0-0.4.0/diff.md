# Comparing `tmp/pofmt-0.3.0.tar.gz` & `tmp/pofmt-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pofmt-0.3.0.tar", last modified: Wed Jun  9 04:10:48 2021, max compression
+gzip compressed data, was "pofmt-0.4.0.tar", last modified: Wed May 10 08:51:54 2023, max compression
```

## Comparing `pofmt-0.3.0.tar` & `pofmt-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-06-09 04:10:42.710776 pofmt-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6757 2021-06-09 04:10:42.710776 pofmt-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2312 2021-06-09 04:10:42.710776 pofmt-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      124 2021-06-09 04:10:42.710776 pofmt-0.3.0/src/pofmt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      121 2021-06-09 04:10:42.710776 pofmt-0.3.0/src/pofmt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8981 2021-06-09 04:10:42.710776 pofmt-0.3.0/src/pofmt/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-06-09 04:10:42.710776 pofmt-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3399 2021-06-09 04:10:42.710776 pofmt-0.3.0/tests/fixtures/golden.po
--rw-r--r--   0 runner    (1001) docker     (121)     3420 2021-06-09 04:10:42.710776 pofmt-0.3.0/tests/fixtures/golden_3x_width.po
--rw-r--r--   0 runner    (1001) docker     (121)     3388 2021-06-09 04:10:42.710776 pofmt-0.3.0/tests/fixtures/golden_no_msgid.po
--rw-r--r--   0 runner    (1001) docker     (121)     3369 2021-06-09 04:10:42.710776 pofmt-0.3.0/tests/fixtures/raw.po
--rw-r--r--   0 runner    (1001) docker     (121)     1887 2021-06-09 04:10:42.710776 pofmt-0.3.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2021-06-09 04:10:42.710776 pofmt-0.3.0/tests/test_formatter.py
--rw-------   0 runner    (1001) docker     (121)     8749 2021-06-09 04:10:48.982874 pofmt-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-10 08:51:47.381013 pofmt-0.4.0/LICENSE
+-rw-r--r--   0        0        0     6757 2023-05-10 08:51:47.381013 pofmt-0.4.0/README.md
+-rw-r--r--   0        0        0     1425 2023-05-10 08:51:54.900967 pofmt-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      124 2023-05-10 08:51:47.381013 pofmt-0.4.0/src/pofmt/__init__.py
+-rw-r--r--   0        0        0      121 2023-05-10 08:51:47.381013 pofmt-0.4.0/src/pofmt/__main__.py
+-rw-r--r--   0        0        0     8958 2023-05-10 08:51:47.381013 pofmt-0.4.0/src/pofmt/core.py
+-rw-r--r--   0        0        0      130 2023-05-10 08:51:47.381013 pofmt-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     3399 2023-05-10 08:51:47.381013 pofmt-0.4.0/tests/fixtures/golden.po
+-rw-r--r--   0        0        0     3420 2023-05-10 08:51:47.381013 pofmt-0.4.0/tests/fixtures/golden_3x_width.po
+-rw-r--r--   0        0        0     3388 2023-05-10 08:51:47.381013 pofmt-0.4.0/tests/fixtures/golden_no_msgid.po
+-rw-r--r--   0        0        0     3369 2023-05-10 08:51:47.381013 pofmt-0.4.0/tests/fixtures/raw.po
+-rw-r--r--   0        0        0     1887 2023-05-10 08:51:47.381013 pofmt-0.4.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1841 2023-05-10 08:51:47.381013 pofmt-0.4.0/tests/test_formatter.py
+-rw-r--r--   0        0        0     7289 1970-01-01 00:00:00.000000 pofmt-0.4.0/PKG-INFO
```

### Comparing `pofmt-0.3.0/LICENSE` & `pofmt-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pofmt-0.3.0/README.md` & `pofmt-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 See [pre-commit](https://pre-commit.com/) for instructions.
 
 A sample `.pre-commit-config.yaml`:
 
 ```yaml
 - repo: https://github.com/frostming/pofmt
-  rev: '0.1.0'
+  rev: '0.4.0'
   hooks:
     - id: pofmt
       additional_dependencies: ['pangu']  # for handling Chinese documents
 ```
 
 ## Usage
```

### Comparing `pofmt-0.3.0/src/pofmt/core.py` & `pofmt-0.4.0/src/pofmt/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,15 @@
 
 try:
     import pangu
 except ModuleNotFoundError:
     pangu = None
 
 MESSAGE_RE = r'"(.*)"[ ]*$'
-_cjk_opening_punct = (
-    r"[\uff08\u3008\u300a\u300c\u300e\ufe43\u3014\uffe5\u3010\u201c\u2018]"
-)
+_cjk_opening_punct = r"[\uff08\u3008\u300a\u300c\u300e\ufe43\u3014\uffe5\u3010\u201c\u2018]"
 _cjk_closing_punct = (
     r"[\uff09\u3009\u300b\u300d\u300f\ufe44\u3015\u2026\u2014\uff5e\ufe4f"
     r"\u3001\u3002\uff0c\uff1f\uff01\uff1a\uff1b\u201d\u2019]"
 )
 
 
 class ParseError(Exception):
@@ -39,15 +37,15 @@
 def is_full_width(text: str) -> bool:
     """See https://stackoverflow.com/a/31666966"""
     return unicodedata.east_asian_width(text) in "WAF"
 
 
 def support_unicode():
     """Check whether operating system supports main symbols or not."""
-    encoding = getattr(sys.stdout, "encoding")
+    encoding = sys.stdout.encoding
     if encoding is None:
         encoding = locale.getpreferredencoding(False)
 
     try:
         encoding = codecs.lookup(encoding).name
     except Exception:
         encoding = "utf-8"
@@ -113,20 +111,18 @@
         with len_with_cjk_width_factor(cjk_width_factor):
             return self._format_text(
                 "msgid", self.msgid, width, reformat=not no_msgid
             ) + self._format_text("msgstr", self.msgstr, width)
 
 
 class Source:
-    def __init__(
-        self, filename: str, lines: t.Optional[t.Sequence[str]] = None
-    ) -> None:
+    def __init__(self, filename: str, lines: t.Optional[t.Sequence[str]] = None) -> None:
         self.filename = filename
         if lines is None:
-            lines = [line for line in Path(filename).read_text("utf-8").splitlines()]
+            lines = list(Path(filename).read_text("utf-8").splitlines())
         self.lines = lines
         self._original = self.lines[:]
         self.lineno = -1
         self._entries: t.List[Entry] = []
 
     def __iter__(self) -> t.Iterator[str]:
         return self
@@ -159,16 +155,18 @@
 
     def _parse_entry(self) -> Entry:
         msgid, msgstr = [], []
         temp = []
         start_line = self.lineno
 
         for line in self:
-            if not line.strip() or line.startswith("#"):
+            if not line.strip():
                 break
+            if line.startswith("#"):
+                continue
             if line.startswith("msgid"):
                 if msgid:
                     self.lineno -= 1
                     break
                 match = re.match(MESSAGE_RE, line[6:])
                 if not match:
                     self.parse_error('Expect `msgid "..."`')
@@ -227,17 +225,15 @@
 
 
 def cli(argv: t.Optional[t.Sequence[str]] = None) -> int:
     parser = argparse.ArgumentParser(description="Format PO files for consistency")
     parser.add_argument(
         "--line-length", type=int, default=76, help="The max length of msgid and msgstr"
     )
-    parser.add_argument(
-        "-c", "--check", action="store_true", help="Check only, don't modify files"
-    )
+    parser.add_argument("-c", "--check", action="store_true", help="Check only, don't modify files")
     parser.add_argument(
         "--cjk-width",
         type=float,
         default=1.8,
         help="The width factor of a CJK character, default: 1.8",
     )
     parser.add_argument("--no-msgid", action="store_true", help="Don't format msgid")
```

### Comparing `pofmt-0.3.0/tests/fixtures/golden.po` & `pofmt-0.4.0/tests/fixtures/golden.po`

 * *Files identical despite different names*

### Comparing `pofmt-0.3.0/tests/fixtures/golden_3x_width.po` & `pofmt-0.4.0/tests/fixtures/golden_3x_width.po`

 * *Files identical despite different names*

### Comparing `pofmt-0.3.0/tests/fixtures/golden_no_msgid.po` & `pofmt-0.4.0/tests/fixtures/golden_no_msgid.po`

 * *Files identical despite different names*

### Comparing `pofmt-0.3.0/tests/fixtures/raw.po` & `pofmt-0.4.0/tests/fixtures/raw.po`

 * *Files identical despite different names*

### Comparing `pofmt-0.3.0/tests/test_cli.py` & `pofmt-0.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pofmt-0.3.0/tests/test_formatter.py` & `pofmt-0.4.0/tests/test_formatter.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,26 @@
     raw = FIXTURES / "raw.po"
     s = Source(raw)
     assert s.fix(76, no_msgid=True)
     content = "\n".join(s.lines) + "\n"
     assert content == golden.read_text(encoding="utf-8")
 
 
+def test_format_fuzzy_translation_with_previous_msgid():
+    lines = [
+        "#: path/to/file.html:136",
+        "#, fuzzy",
+        '#| msgid "Report (HTML)"',
+        'msgid "Report HTML"',
+        'msgstr "Informe (HTML)"',
+    ]
+    s = Source("test_file", lines)
+    assert not s.fix(76)
+
+
 @pytest.mark.parametrize(
     "error_text",
     [
         textwrap.dedent(
             """msgid
     msgstr "hello"
     """
```

### Comparing `pofmt-0.3.0/PKG-INFO` & `pofmt-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,180 +1,177 @@
 Metadata-Version: 2.1
 Name: pofmt
-Version: 0.3.0
+Version: 0.4.0
 Summary: Your missing PO formatter and linter
+Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
-Author-email: Frost Ming <mianghong@gmail.com>
-Requires-Python: >=3.6
 Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: zh
-Project-URL: Homepage, https://github.com/frostming/pofmt
 Project-URL: Repository, https://github.com/frostming/pofmt
+Project-URL: Homepage, https://github.com/frostming/pofmt
+Requires-Python: >=3.7
+Provides-Extra: zh
+Requires-Dist: pangu>=4.0; extra == "zh"
 Description-Content-Type: text/markdown
-Description: # pofmt
-        
-        [![Tests](https://github.com/frostming/pofmt/workflows/Tests/badge.svg)](https://github.com/frostming/pofmt/actions?query=workflow%3Aci)
-        [![pypi version](https://img.shields.io/pypi/v/pofmt.svg)](https://pypi.org/project/pofmt/)
-        [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        Your missing PO formatter and linter
-        
-        ## Features
-        
-        - Wrap msgid and msgstr with a constant max width.
-        - Can act as a [pre-commit](https://pre-commit.com/) hook.
-        - Display lint errors in a human readable format.
-        - Insert white-spaces between Chinese characters and latin letters with [pangu](https://github.com/vinta/pangu.py)
-        - The widths of CJK characters are multiplied by a factor for visual balance.
-        
-        ## Requirements
-        
-        pofmt requires Python >=3.6
-        
-        ## Installation
-        
-        It is recommended to install with `pipx`, if `pipx` haven't been installed yet, refer to the [pipx's docs](https://github.com/pipxproject/pipx)
-        
-        ```bash
-        $ pipx install pofmt
-        ```
-        
-        Alternatively, install with `pip` to the user site:
-        
-        ```bash
-        $ python -m pip install --user pofmt
-        ```
-        
-        If you are formatting PO files with Chinese, it is recommended to install `pofmt[zh]`. This includes
-        a handy function to add spaces between CJK characters and latin letters.
-        
-        ## As a pre-commit hook
-        
-        See [pre-commit](https://pre-commit.com/) for instructions.
-        
-        A sample `.pre-commit-config.yaml`:
-        
-        ```yaml
-        - repo: https://github.com/frostming/pofmt
-          rev: '0.1.0'
-          hooks:
-            - id: pofmt
-              additional_dependencies: ['pangu']  # for handling Chinese documents
-        ```
-        
-        ## Usage
-        
-        ```
-        USAGE: pofmt [-h] [--line-length LINE_LENGTH] [-c] [--cjk-width CJK_WIDTH] [filename ...]
-        
-        Format PO files for consistency
-        
-        positional arguments:
-          filename              Filenames to format, default to all po files under the current directory(recursively)
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          --line-length LINE_LENGTH
-                                The max length of msgid and msgstr
-          -c, --check           Check only, don't modify files
-          --cjk-width CJK_WIDTH
-                                The width factor of a CJK character, default: 1.8
-          --no-msgid            Don't format msgid
-        ```
-        
-        ## Sample output
-        
-        ```diff
-        --- Original
-        +++ Current
-        @@ -21,49 +21,48 @@
-         msgid "Welcome to Flask"
-         msgstr "欢迎来到 Flask 的世界"
-        
-        -msgid "Flask: web development, one "drop" at a time"
-        +msgid "Flask: web development, one \"drop\" at a time"
-         msgstr "Flask： Web 开发，一次一滴"
-        
-         #: ../../index.rst:11
-         msgid ""
-        -"Welcome to Flask's documentation. Get started with :doc:`installation` "
-        -"and then get an overview with the :doc:`quickstart`. There is also a more"
-        -" detailed :doc:`tutorial/index` that shows how to create a small but "
-        +"Welcome to Flask's documentation. Get started with :doc:`installation` and"
-        +" then get an overview with the :doc:`quickstart`. There is also a more "
-        +"detailed :doc:`tutorial/index` that shows how to create a small but "
-         "complete application with Flask. Common patterns are described in the "
-         ":doc:`patterns/index` section. The rest of the docs describe each "
-         "component of Flask in detail, with a full reference in the :doc:`api` "
-         "section."
-         msgstr ""
-        -"欢迎来到Flask的文档。你可以从 :doc:`installation` 入手，然后阅读:doc:`quickstart`来了解基本概念。还有一个包含更多细节的:doc:`tutorial/index`"
-        -"介绍如何用Flask创建一个很小但是完整的程序。一般的开发模式可以在:doc:`patterns/index`章节找到。剩下的文档详细的介绍了Flask的每一个组成部件，"
-        -"其中:doc:`api`章节包括完整的API参考信息。"
-        +"欢迎来到 Flask 的文档。你可以从 :doc:`installation` 入手，然后阅读:doc:`quickstart` "
-        +"来了解基本概念。还有一个包含更多细节的:doc:`tutorial/index` 介绍如何用 Flask "
-        +"创建一个很小但是完整的程序。一般的开发模式可以在:doc:`patterns/index` 章节找到。剩下的文档详细的介绍了 Flask "
-        +"的每一个组成部件，其中:doc:`api` 章节包括完整的 API 参考信息。"
-        
-         #: ../../index.rst:19
-        -msgid "Flask depends on the `Jinja`_ template engine and the `Werkzeug`_ WSGI toolkit. The documentation for these libraries can be found at:"
-        -msgstr ""
-        -"Flask 依赖 `Jinja`_ 模板引擎和 `Werkzeug`_ WSGI 工具集。这些库的文档如下："
-        +msgid ""
-        +"Flask depends on the `Jinja`_ template engine and the `Werkzeug`_ WSGI "
-        +"toolkit. The documentation for these libraries can be found at:"
-        +msgstr "Flask 依赖 `Jinja`_ 模板引擎和 `Werkzeug`_ WSGI 工具集。这些库的文档如下："
-        
-         #: ../../index.rst:22
-         msgid "`Jinja documentation <https://jinja.palletsprojects.com/>`_"
-        -msgstr "`Jinja文档<https://jinja.palletsprojects.com/>`_"
-        +msgstr "`Jinja 文档 <https://jinja.palletsprojects.com/>`_"
-        
-         #: ../../index.rst:23
-         msgid "`Werkzeug documentation <https://werkzeug.palletsprojects.com/>`_"
-        -msgstr "`Werkzeug文档<https://werkzeug.palletsprojects.com/>`_"
-        +msgstr "`Werkzeug 文档 <https://werkzeug.palletsprojects.com/>`_"
-        
-         #: ../../index.rst:30
-         msgid "User's Guide"
-        -msgstr ""
-        -"用户指南"
-        +msgstr "用户指南"
-        
-         #: ../../index.rst:32
-         msgid ""
-         "This part of the documentation, which is mostly prose, begins with some "
-         "background information about Flask, then focuses on step-by-step "
-         "instructions for web development with Flask."
-        -msgstr ""
-        -"这部分的文档大部分是独立章节，以一些关于 Flask 的背景信息开始，然后重点介绍如何"
-        -"使用 Flask 一步步进行 Web 开发。"
-        +msgstr "这部分的文档大部分是独立章节，以一些关于 Flask 的背景信息开始，然后重点介绍如何使用 Flask 一步步进行 Web 开发。"
-        
-         #: ../../index.rst:66
-         msgid "API Reference"
-        @@ -73,13 +72,13 @@
-         msgid ""
-         "If you are looking for information on a specific function, class or "
-         "method, this part of the documentation is for you."
-        -msgstr ""
-        -"如果你想找关于某个特定函数、类或方法的信息，那么这部分文档就是为你准备的。"
-        +msgstr "如果你想找关于某个特定函数、类或方法的信息，那么这部分文档就是为你准备的。"
-        
-         #: ../../index.rst:78
-         msgid "Additional Notes"
-         msgstr "附加笔记"
-        
-         #: ../../index.rst:80
-        -msgid "Design notes, legal information and changelog are here for the interested."
-        +msgid ""
-        +"Design notes, legal information and changelog are here for the interested."
-         msgstr "如果你感兴趣的话，这里有一些设计笔记、法律信息和变更日志（changelog）。"
-        ```
 
+# pofmt
+
+[![Tests](https://github.com/frostming/pofmt/workflows/Tests/badge.svg)](https://github.com/frostming/pofmt/actions?query=workflow%3Aci)
+[![pypi version](https://img.shields.io/pypi/v/pofmt.svg)](https://pypi.org/project/pofmt/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Your missing PO formatter and linter
+
+## Features
+
+- Wrap msgid and msgstr with a constant max width.
+- Can act as a [pre-commit](https://pre-commit.com/) hook.
+- Display lint errors in a human readable format.
+- Insert white-spaces between Chinese characters and latin letters with [pangu](https://github.com/vinta/pangu.py)
+- The widths of CJK characters are multiplied by a factor for visual balance.
+
+## Requirements
+
+pofmt requires Python >=3.6
+
+## Installation
+
+It is recommended to install with `pipx`, if `pipx` haven't been installed yet, refer to the [pipx's docs](https://github.com/pipxproject/pipx)
+
+```bash
+$ pipx install pofmt
+```
+
+Alternatively, install with `pip` to the user site:
+
+```bash
+$ python -m pip install --user pofmt
+```
+
+If you are formatting PO files with Chinese, it is recommended to install `pofmt[zh]`. This includes
+a handy function to add spaces between CJK characters and latin letters.
+
+## As a pre-commit hook
+
+See [pre-commit](https://pre-commit.com/) for instructions.
+
+A sample `.pre-commit-config.yaml`:
+
+```yaml
+- repo: https://github.com/frostming/pofmt
+  rev: '0.4.0'
+  hooks:
+    - id: pofmt
+      additional_dependencies: ['pangu']  # for handling Chinese documents
+```
+
+## Usage
+
+```
+USAGE: pofmt [-h] [--line-length LINE_LENGTH] [-c] [--cjk-width CJK_WIDTH] [filename ...]
+
+Format PO files for consistency
+
+positional arguments:
+  filename              Filenames to format, default to all po files under the current directory(recursively)
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --line-length LINE_LENGTH
+                        The max length of msgid and msgstr
+  -c, --check           Check only, don't modify files
+  --cjk-width CJK_WIDTH
+                        The width factor of a CJK character, default: 1.8
+  --no-msgid            Don't format msgid
+```
+
+## Sample output
+
+```diff
+--- Original
++++ Current
+@@ -21,49 +21,48 @@
+ msgid "Welcome to Flask"
+ msgstr "欢迎来到 Flask 的世界"
+
+-msgid "Flask: web development, one "drop" at a time"
++msgid "Flask: web development, one \"drop\" at a time"
+ msgstr "Flask： Web 开发，一次一滴"
+
+ #: ../../index.rst:11
+ msgid ""
+-"Welcome to Flask's documentation. Get started with :doc:`installation` "
+-"and then get an overview with the :doc:`quickstart`. There is also a more"
+-" detailed :doc:`tutorial/index` that shows how to create a small but "
++"Welcome to Flask's documentation. Get started with :doc:`installation` and"
++" then get an overview with the :doc:`quickstart`. There is also a more "
++"detailed :doc:`tutorial/index` that shows how to create a small but "
+ "complete application with Flask. Common patterns are described in the "
+ ":doc:`patterns/index` section. The rest of the docs describe each "
+ "component of Flask in detail, with a full reference in the :doc:`api` "
+ "section."
+ msgstr ""
+-"欢迎来到Flask的文档。你可以从 :doc:`installation` 入手，然后阅读:doc:`quickstart`来了解基本概念。还有一个包含更多细节的:doc:`tutorial/index`"
+-"介绍如何用Flask创建一个很小但是完整的程序。一般的开发模式可以在:doc:`patterns/index`章节找到。剩下的文档详细的介绍了Flask的每一个组成部件，"
+-"其中:doc:`api`章节包括完整的API参考信息。"
++"欢迎来到 Flask 的文档。你可以从 :doc:`installation` 入手，然后阅读:doc:`quickstart` "
++"来了解基本概念。还有一个包含更多细节的:doc:`tutorial/index` 介绍如何用 Flask "
++"创建一个很小但是完整的程序。一般的开发模式可以在:doc:`patterns/index` 章节找到。剩下的文档详细的介绍了 Flask "
++"的每一个组成部件，其中:doc:`api` 章节包括完整的 API 参考信息。"
+
+ #: ../../index.rst:19
+-msgid "Flask depends on the `Jinja`_ template engine and the `Werkzeug`_ WSGI toolkit. The documentation for these libraries can be found at:"
+-msgstr ""
+-"Flask 依赖 `Jinja`_ 模板引擎和 `Werkzeug`_ WSGI 工具集。这些库的文档如下："
++msgid ""
++"Flask depends on the `Jinja`_ template engine and the `Werkzeug`_ WSGI "
++"toolkit. The documentation for these libraries can be found at:"
++msgstr "Flask 依赖 `Jinja`_ 模板引擎和 `Werkzeug`_ WSGI 工具集。这些库的文档如下："
+
+ #: ../../index.rst:22
+ msgid "`Jinja documentation <https://jinja.palletsprojects.com/>`_"
+-msgstr "`Jinja文档<https://jinja.palletsprojects.com/>`_"
++msgstr "`Jinja 文档 <https://jinja.palletsprojects.com/>`_"
+
+ #: ../../index.rst:23
+ msgid "`Werkzeug documentation <https://werkzeug.palletsprojects.com/>`_"
+-msgstr "`Werkzeug文档<https://werkzeug.palletsprojects.com/>`_"
++msgstr "`Werkzeug 文档 <https://werkzeug.palletsprojects.com/>`_"
+
+ #: ../../index.rst:30
+ msgid "User's Guide"
+-msgstr ""
+-"用户指南"
++msgstr "用户指南"
+
+ #: ../../index.rst:32
+ msgid ""
+ "This part of the documentation, which is mostly prose, begins with some "
+ "background information about Flask, then focuses on step-by-step "
+ "instructions for web development with Flask."
+-msgstr ""
+-"这部分的文档大部分是独立章节，以一些关于 Flask 的背景信息开始，然后重点介绍如何"
+-"使用 Flask 一步步进行 Web 开发。"
++msgstr "这部分的文档大部分是独立章节，以一些关于 Flask 的背景信息开始，然后重点介绍如何使用 Flask 一步步进行 Web 开发。"
+
+ #: ../../index.rst:66
+ msgid "API Reference"
+@@ -73,13 +72,13 @@
+ msgid ""
+ "If you are looking for information on a specific function, class or "
+ "method, this part of the documentation is for you."
+-msgstr ""
+-"如果你想找关于某个特定函数、类或方法的信息，那么这部分文档就是为你准备的。"
++msgstr "如果你想找关于某个特定函数、类或方法的信息，那么这部分文档就是为你准备的。"
+
+ #: ../../index.rst:78
+ msgid "Additional Notes"
+ msgstr "附加笔记"
+
+ #: ../../index.rst:80
+-msgid "Design notes, legal information and changelog are here for the interested."
++msgid ""
++"Design notes, legal information and changelog are here for the interested."
+ msgstr "如果你感兴趣的话，这里有一些设计笔记、法律信息和变更日志（changelog）。"
+```
```

