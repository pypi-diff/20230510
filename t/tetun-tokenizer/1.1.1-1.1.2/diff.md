# Comparing `tmp/tetun_tokenizer-1.1.1.tar.gz` & `tmp/tetun_tokenizer-1.1.2.tar.gz`

## Comparing `tetun_tokenizer-1.1.1.tar` & `tetun_tokenizer-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/.DS_Store
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/Pipfile
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/Pipfile.lock
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/_token
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/tetuntokenizer/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/tetuntokenizer/tetun_patterns.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/tetuntokenizer/tokenizer.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/LICENSE
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/README.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/.DS_Store
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/Pipfile
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/Pipfile.lock
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/_token
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/tetuntokenizer/__init__.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/tetuntokenizer/tetun_patterns.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/tetuntokenizer/tokenizer.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/LICENSE
+-rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/README.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/PKG-INFO
```

### Comparing `tetun_tokenizer-1.1.1/.DS_Store` & `tetun_tokenizer-1.1.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.1/Pipfile.lock` & `tetun_tokenizer-1.1.2/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.1/tetuntokenizer/tetun_patterns.py` & `tetun_tokenizer-1.1.2/tetuntokenizer/tetun_patterns.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 
 
 """ This file contains all the regular expressions for the Tetun tokenizer. """
 
-# E.g.: Ataúru, ne'ebé, ida-ne'ebé, Ofisiál, etc.
-TETUN_TEXT_PATTERN = r"[A-Za-zÂÁáãéêÉÊíÍóÓúÚñç]+(?:[-’'][A-Za-zÂÁáãéêÉÊíÍóÓúÚñç]+)*"
+# E.g.: Ataúru, ne'ebé, ida-ne'ebé, Ofisiál, Ângela, Conceição, Kompañia, etc.
+TETUN_TEXT_PATTERN = r"[A-Za-zÂÁÃâáãÉÊéêÍíÓóÚúÑñÇç]+(?:[-’'][A-Za-zÂÁÃâáãÉÊéêÍíÓóÚúÑñÇç]+)*"
 
 # E.g.: 20.000.000.000,45 or 20,000,000,000.45.
 # E.g.; char ',' or '.' followed digits will be ignored.
 DIGITS_PATTERN = r"\d+(?:[,.]\d+)*"
 
 # These punctuations and symbols will be tokenized as a token in the Tetun standard tokenizer.
 PUNCTUATIONS_SYMBOLS = '!,./:;?"“”()[\\]^_`{|}#&§©°$€£μ@*+÷%<=>«»~'
```

### Comparing `tetun_tokenizer-1.1.1/tetuntokenizer/tokenizer.py` & `tetun_tokenizer-1.1.2/tetuntokenizer/tokenizer.py`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.1/LICENSE` & `tetun_tokenizer-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.1/README.md` & `tetun_tokenizer-1.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ### Tetun Tokenizer
 
-Tetun tokenizer is a Python package for tokenizing an input text into tokens. There are several tokenization techniques we built alongside this package as follows:
+Tetun tokenizer is a Python package for tokenizing an input text into tokens. There are several tokenization techniques we built along with this package as follows:
 1. `TetunStandardTokenizer()`: tokenize the input text by `word`, `punctuations`, and `special characters`.
 2. `TetunWhiteSpaceTokenizer()`: tokenize the input text by `whitespace` delimiter.
 3. `TetunSentenceTokenizer()`: tokenize the input text by `.?!` delimiters.
 4. `TetunBlankLineTokenizer()`: tokenize the input text by `blank lines` delimiter.
 5. `TetunSimpleTokenizer()`: tokenize the input text by extracting `only string and number` and ignore punctuations and special characters.
 6. `TetunWordTokenizer()`: tokenize the input text by extracting `only string` and ignore numbers, punctuations, and special characters.
```

### Comparing `tetun_tokenizer-1.1.1/PKG-INFO` & `tetun_tokenizer-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: tetun_tokenizer
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tetun tokenizer
 Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ### Tetun Tokenizer
 
-Tetun tokenizer is a Python package for tokenizing an input text into tokens. There are several tokenization techniques we built alongside this package as follows:
+Tetun tokenizer is a Python package for tokenizing an input text into tokens. There are several tokenization techniques we built along with this package as follows:
 1. `TetunStandardTokenizer()`: tokenize the input text by `word`, `punctuations`, and `special characters`.
 2. `TetunWhiteSpaceTokenizer()`: tokenize the input text by `whitespace` delimiter.
 3. `TetunSentenceTokenizer()`: tokenize the input text by `.?!` delimiters.
 4. `TetunBlankLineTokenizer()`: tokenize the input text by `blank lines` delimiter.
 5. `TetunSimpleTokenizer()`: tokenize the input text by extracting `only string and number` and ignore punctuations and special characters.
 6. `TetunWordTokenizer()`: tokenize the input text by extracting `only string` and ignore numbers, punctuations, and special characters.
```

