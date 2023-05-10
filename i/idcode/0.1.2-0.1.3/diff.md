# Comparing `tmp/idcode-0.1.2.tar.gz` & `tmp/idcode-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idcode-0.1.2.tar", max compression
+gzip compressed data, was "idcode-0.1.3.tar", max compression
```

## Comparing `idcode-0.1.2.tar` & `idcode-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2023-05-03 14:58:29.726031 idcode-0.1.2/idcode/__init__.py
--rw-r--r--   0        0        0     1603 2023-05-03 15:18:46.916433 idcode-0.1.2/idcode/cli.py
--rw-r--r--   0        0        0     2123 2023-05-03 15:18:50.169379 idcode-0.1.2/idcode/core_values.py
--rw-r--r--   0        0        0    11104 2023-05-03 15:18:53.014665 idcode-0.1.2/idcode/custom_encoding.py
--rw-r--r--   0        0        0     5713 2023-05-03 15:17:18.838725 idcode-0.1.2/idcode/interactive_decoder.py
--rw-r--r--   0        0        0      339 2023-05-02 10:49:07.137334 idcode-0.1.2/idcode/preprocessing.py
--rw-r--r--   0        0        0     1083 2023-05-01 19:53:11.733482 idcode-0.1.2/LICENSE
--rw-r--r--   0        0        0      506 2023-05-03 15:21:39.235003 idcode-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1538 2023-05-03 15:21:30.738476 idcode-0.1.2/README.md
--rw-r--r--   0        0        0     2193 1970-01-01 00:00:00.000000 idcode-0.1.2/setup.py
--rw-r--r--   0        0        0     2004 1970-01-01 00:00:00.000000 idcode-0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1083 2023-05-01 19:53:11.733482 idcode-0.1.3/LICENSE
+-rwxr-xr-x   0        0        0     1554 2023-05-10 12:13:27.926198 idcode-0.1.3/README.md
+-rwxr-xr-x   0        0        0        0 2023-05-03 14:58:29.726031 idcode-0.1.3/idcode/__init__.py
+-rwxr-xr-x   0        0        0     1603 2023-05-03 15:18:46.916433 idcode-0.1.3/idcode/cli.py
+-rwxr-xr-x   0        0        0     2123 2023-05-03 15:18:50.169379 idcode-0.1.3/idcode/core_values.py
+-rwxr-xr-x   0        0        0    11443 2023-05-10 12:12:58.897782 idcode-0.1.3/idcode/custom_encoding.py
+-rwxr-xr-x   0        0        0     5713 2023-05-03 15:17:18.838725 idcode-0.1.3/idcode/interactive_decoder.py
+-rwxr-xr-x   0        0        0      339 2023-05-02 10:49:07.137334 idcode-0.1.3/idcode/preprocessing.py
+-rwxr-xr-x   0        0        0      506 2023-05-10 12:14:46.494620 idcode-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2209 1970-01-01 00:00:00.000000 idcode-0.1.3/setup.py
+-rw-r--r--   0        0        0     2019 1970-01-01 00:00:00.000000 idcode-0.1.3/PKG-INFO
```

### Comparing `idcode-0.1.2/idcode/cli.py` & `idcode-0.1.3/idcode/cli.py`

 * *Files identical despite different names*

### Comparing `idcode-0.1.2/idcode/core_values.py` & `idcode-0.1.3/idcode/core_values.py`

 * *Files identical despite different names*

### Comparing `idcode-0.1.2/idcode/custom_encoding.py` & `idcode-0.1.3/idcode/custom_encoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -359,13 +359,23 @@
     ALPHABET = '富强民主文明和谐自由平等公正法治爱国敬业诚信友善'
 
     @staticmethod
     def decode(encoded_text):
         return values_decode(encoded_text)
 
 
+class AsciiEncoding(Encoding):
+    pattern = r'^((0|[1-9]|[1-9]\d|1[0-1]\d|12[0-7])[-:,;\s]?)+$'
+
+    @staticmethod
+    def decode(encoded_text):
+        encoded_text = re.sub(r'[-:,;]', '', encoded_text)
+        decoded_text = ''.join([chr(int(c)) for c in encoded_text.split()])
+        return decoded_text
+
 all_encodings = [
     Base94Encoding, Base92Encoding, Base91Encoding, Base85Encoding, Ascii85Encoding,
     AdobeAscii85Encoding, Z85Encoding, Base64Encoding, Base62Encoding, Base58Encoding,
     Base45Encoding, Base36Encoding, Base32Encoding, HexEncoding, Base8Encoding,
-    BinaryEncoding, URLEncoding,  HTMLEncoding, QuotedPrintableEncoding, CoreValuesEncoding
+    BinaryEncoding, URLEncoding,  HTMLEncoding, QuotedPrintableEncoding, CoreValuesEncoding,
+    AsciiEncoding
 ]
```

### Comparing `idcode-0.1.2/idcode/interactive_decoder.py` & `idcode-0.1.3/idcode/interactive_decoder.py`

 * *Files identical despite different names*

### Comparing `idcode-0.1.2/LICENSE` & `idcode-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `idcode-0.1.2/README.md` & `idcode-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 ## 支持的编码格式
 
 idcode 支持多种编码格式，包括：
 
 - Base85/Base64/Base32
 - Base94/Base92/Base91/Ascii85/AdobeAscii85/Z85/Base58/Base45/Base36/Base8
 - Binary 编码
+- ASCII 编码
 - Hex 编码
 - URL 编码
 - HTML 实体编码
 - Quoted-printable 编码
 - 核心价值观编码
 
 ## 安装
```

### Comparing `idcode-0.1.2/setup.py` & `idcode-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['idcode = idcode.cli:main']}
 
 setup_kwargs = {
     'name': 'idcode',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': '交互式检测并解码编码文本。',
-    'long_description': '# idcode\n\nidcode 是一个使用 Python 编写的命令行工具，用于交互式检测并解码编码文本。它支持命令行输入和文件输入，可以自动检测编码类型和尝试解码，并提供了一个交互式界面来逐步解码编码文本。\n\n## 支持的编码格式\n\nidcode 支持多种编码格式，包括：\n\n- Base85/Base64/Base32\n- Base94/Base92/Base91/Ascii85/AdobeAscii85/Z85/Base58/Base45/Base36/Base8\n- Binary 编码\n- Hex 编码\n- URL 编码\n- HTML 实体编码\n- Quoted-printable 编码\n- 核心价值观编码\n\n## 安装\n\n从 PyPi 安装：\n\n```sh\npip install idcode\n```\n\n## 用法\n\nidcode 支持交互式输入、命令行输入和文件输入来获取编码文本。\n\n### 交互式输入\n\n当不给出任何命令行参数时，程序会在运行后提示你给出目标文本：\n\n```sh\nidcode\n```\n\n### 命令行输入\n\n要使用命令行输入方式来解码编码文本，你可以运行以下命令：\n\n```sh\nidcode -t "编码文本"\n```\n\n其中，`-t` 参数用于指定要解码的文本。\n\n### 文件输入\n\n要使用文件输入方式来解码编码文本，你可以运行以下命令：\n\n```sh\nidcode -f "文件路径"\n```\n\n其中，`-f` 参数用于指定包含编码文本的文件路径。\n\n## 贡献\n\n如果你发现了 bug，或者有改进建议，请随时创建 issue 或者 pull request。我们欢迎任何形式的贡献。\n\n## 许可证\n\nidcode 使用 MIT 许可证。请参阅 LICENSE 文件了解更多详情。',
+    'long_description': '# idcode\n\nidcode 是一个使用 Python 编写的命令行工具，用于交互式检测并解码编码文本。它支持命令行输入和文件输入，可以自动检测编码类型和尝试解码，并提供了一个交互式界面来逐步解码编码文本。\n\n## 支持的编码格式\n\nidcode 支持多种编码格式，包括：\n\n- Base85/Base64/Base32\n- Base94/Base92/Base91/Ascii85/AdobeAscii85/Z85/Base58/Base45/Base36/Base8\n- Binary 编码\n- ASCII 编码\n- Hex 编码\n- URL 编码\n- HTML 实体编码\n- Quoted-printable 编码\n- 核心价值观编码\n\n## 安装\n\n从 PyPi 安装：\n\n```sh\npip install idcode\n```\n\n## 用法\n\nidcode 支持交互式输入、命令行输入和文件输入来获取编码文本。\n\n### 交互式输入\n\n当不给出任何命令行参数时，程序会在运行后提示你给出目标文本：\n\n```sh\nidcode\n```\n\n### 命令行输入\n\n要使用命令行输入方式来解码编码文本，你可以运行以下命令：\n\n```sh\nidcode -t "编码文本"\n```\n\n其中，`-t` 参数用于指定要解码的文本。\n\n### 文件输入\n\n要使用文件输入方式来解码编码文本，你可以运行以下命令：\n\n```sh\nidcode -f "文件路径"\n```\n\n其中，`-f` 参数用于指定包含编码文本的文件路径。\n\n## 贡献\n\n如果你发现了 bug，或者有改进建议，请随时创建 issue 或者 pull request。我们欢迎任何形式的贡献。\n\n## 许可证\n\nidcode 使用 MIT 许可证。请参阅 LICENSE 文件了解更多详情。',
     'author': 'p0ise',
     'author_email': 'changelf@163.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/p0ise/idcode',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `idcode-0.1.2/PKG-INFO` & `idcode-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idcode
-Version: 0.1.2
+Version: 0.1.3
 Summary: 交互式检测并解码编码文本。
 Home-page: https://github.com/p0ise/idcode
 License: MIT
 Author: p0ise
 Author-email: changelf@163.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -21,14 +21,15 @@
 ## 支持的编码格式
 
 idcode 支持多种编码格式，包括：
 
 - Base85/Base64/Base32
 - Base94/Base92/Base91/Ascii85/AdobeAscii85/Z85/Base58/Base45/Base36/Base8
 - Binary 编码
+- ASCII 编码
 - Hex 编码
 - URL 编码
 - HTML 实体编码
 - Quoted-printable 编码
 - 核心价值观编码
 
 ## 安装
```

