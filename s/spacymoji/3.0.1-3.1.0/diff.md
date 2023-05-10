# Comparing `tmp/spacymoji-3.0.1.tar.gz` & `tmp/spacymoji-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacymoji-3.0.1.tar", last modified: Tue Apr 20 00:52:44 2021, max compression
+gzip compressed data, was "spacymoji-3.1.0.tar", last modified: Wed May 10 14:10:59 2023, max compression
```

## Comparing `spacymoji-3.0.1.tar` & `spacymoji-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-04-20 00:52:44.807777 spacymoji-3.0.1/
--rw-r--r--   0 vsts      (1001) docker     (121)     1102 2021-04-20 00:52:28.000000 spacymoji-3.0.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)       34 2021-04-20 00:52:28.000000 spacymoji-3.0.1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     7546 2021-04-20 00:52:44.807777 spacymoji-3.0.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     5747 2021-04-20 00:52:28.000000 spacymoji-3.0.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (121)     1268 2021-04-20 00:52:44.807777 spacymoji-3.0.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)      153 2021-04-20 00:52:28.000000 spacymoji-3.0.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-04-20 00:52:44.807777 spacymoji-3.0.1/spacymoji/
--rw-r--r--   0 vsts      (1001) docker     (121)     5460 2021-04-20 00:52:28.000000 spacymoji-3.0.1/spacymoji/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-04-20 00:52:44.807777 spacymoji-3.0.1/spacymoji/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-04-20 00:52:28.000000 spacymoji-3.0.1/spacymoji/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3639 2021-04-20 00:52:28.000000 spacymoji-3.0.1/spacymoji/tests/test_emoji.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-04-20 00:52:44.807777 spacymoji-3.0.1/spacymoji.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     7546 2021-04-20 00:52:44.000000 spacymoji-3.0.1/spacymoji.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      356 2021-04-20 00:52:44.000000 spacymoji-3.0.1/spacymoji.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-04-20 00:52:44.000000 spacymoji-3.0.1/spacymoji.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       50 2021-04-20 00:52:44.000000 spacymoji-3.0.1/spacymoji.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       40 2021-04-20 00:52:44.000000 spacymoji-3.0.1/spacymoji.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       10 2021-04-20 00:52:44.000000 spacymoji-3.0.1/spacymoji.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-04-20 00:52:44.000000 spacymoji-3.0.1/spacymoji.egg-info/zip-safe
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-10 14:10:59.743049 spacymoji-3.1.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1102 2023-05-10 14:10:49.000000 spacymoji-3.1.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       34 2023-05-10 14:10:49.000000 spacymoji-3.1.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     6813 2023-05-10 14:10:59.743049 spacymoji-3.1.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     5688 2023-05-10 14:10:49.000000 spacymoji-3.1.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)       81 2023-05-10 14:10:49.000000 spacymoji-3.1.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1382 2023-05-10 14:10:59.743049 spacymoji-3.1.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      153 2023-05-10 14:10:49.000000 spacymoji-3.1.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-10 14:10:59.743049 spacymoji-3.1.0/spacymoji/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5526 2023-05-10 14:10:49.000000 spacymoji-3.1.0/spacymoji/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-10 14:10:59.743049 spacymoji-3.1.0/spacymoji/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-10 14:10:49.000000 spacymoji-3.1.0/spacymoji/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3639 2023-05-10 14:10:49.000000 spacymoji-3.1.0/spacymoji/tests/test_emoji.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-10 14:10:59.743049 spacymoji-3.1.0/spacymoji.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     6813 2023-05-10 14:10:59.000000 spacymoji-3.1.0/spacymoji.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      371 2023-05-10 14:10:59.000000 spacymoji-3.1.0/spacymoji.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-10 14:10:59.000000 spacymoji-3.1.0/spacymoji.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       49 2023-05-10 14:10:59.000000 spacymoji-3.1.0/spacymoji.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       36 2023-05-10 14:10:59.000000 spacymoji-3.1.0/spacymoji.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       10 2023-05-10 14:10:59.000000 spacymoji-3.1.0/spacymoji.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-10 14:10:59.000000 spacymoji-3.1.0/spacymoji.egg-info/zip-safe
```

### Comparing `spacymoji-3.0.1/LICENSE` & `spacymoji-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spacymoji-3.0.1/PKG-INFO` & `spacymoji-3.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,135 @@
 Metadata-Version: 2.1
 Name: spacymoji
-Version: 3.0.1
-Summary: spaCy pipeline component for adding emoji meta data to Doc, Token and Span objects
+Version: 3.1.0
+Summary: spaCy pipeline component for adding emoji metadata to Doc, Token and Span objects
 Home-page: https://github.com/explosion/spacymoji
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
-Description: # spacymoji: emoji for spaCy
-        
-        [spaCy](https://spacy.io) extension and pipeline component
-        for adding emoji meta data to `Doc` objects. Detects emoji consisting of one
-        or more unicode characters, and can optionally merge multi-char emoji (combined
-        pictures, emoji with skin tone modifiers) into one token. Human-readable emoji
-        descriptions are added as a custom attribute, and an optional lookup table can
-        be provided for your own descriptions. The extension sets the custom `Doc`,
-        `Token` and `Span` attributes `._.is_emoji`, `._.emoji_desc`, `._.has_emoji` and `._.emoji`. You can read more about custom pipeline components and extension attributes [here](https://spacy.io/usage/processing-pipelines).
-        
-        Emoji are matched using spaCy's [`PhraseMatcher`](https://spacy.io/api/phrasematcher), and looked up in the data
-        table provided by the [`emoji` package](https://github.com/carpedm20/emoji).
-        
-        [![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/22/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=22)
-        [![Current Release Version](https://img.shields.io/github/release/explosion/spacymoji.svg?style=flat-square&logo=github)](https://github.com/explosion/spacymoji/releases)
-        [![pypi Version](https://img.shields.io/pypi/v/spacymoji.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacymoji/)
-        
-        # ⏳ Installation
-        
-        `spacymoji` requires `spacy` v3.0.0 or higher. For spaCy v2.x, instally `spacymoji==2.0.0`.
-        
-        ```bash
-        pip install spacymoji
-        ```
-        
-        # ☝️ Usage
-        
-        Import the component and add it anywhere in your pipeline using the string
-        name of the `"emoji"` component factory:
-        
-        ```python
-        import spacy
-        
-        nlp = spacy.load("en_core_web_sm")
-        nlp.add_pipe("emoji", first=True)
-        doc = nlp("This is a test 😻 👍🏿")
-        assert doc._.has_emoji is True
-        assert doc[2:5]._.has_emoji is True
-        assert doc[0]._.is_emoji is False
-        assert doc[4]._.is_emoji is True
-        assert doc[5]._.emoji_desc == "thumbs up dark skin tone"
-        assert len(doc._.emoji) == 2
-        assert doc._.emoji[1] == ("👍🏿", 5, "thumbs up dark skin tone")
-        ```
-        
-        `spacymoji` only cares about the token text, so you can use it on a blank
-        `Language` instance (it should work for all
-        [available languages](https://spacy.io/usage/models#languages)!), or in
-        a pipeline with a loaded pipeline. If your pipeline
-        includes a tagger, parser and entity recognizer, make sure to add the emoji
-        component as `first=True`, so the spans are merged right after tokenization,
-        and _before_ the document is parsed. If your text contains a lot of emoji, this
-        might even give you a nice boost in parser accuracy.
-        
-        ## Available attributes
-        
-        The extension sets attributes on the `Doc`, `Span` and `Token`. You can
-        change the attribute names (and other parameters of the Emoji component) by passing
-        them via the `config` parameter in the `nlp.add_pipe(...)` method. For more details
-        on custom components and attributes, see the
-        [processing pipelines documentation](https://spacy.io/usage/processing-pipelines#custom-components).
-        
-        | Attribute            | Type                       | Description                                                   |
-        | -------------------- | -------------------------- | ------------------------------------------------------------- |
-        | `Token._.is_emoji`   | bool                       | Whether the token is an emoji.                                |
-        | `Token._.emoji_desc` | str                        | A human-readable description of the emoji.                    |
-        | `Doc._.has_emoji`    | bool                       | Whether the document contains emoji.                          |
-        | `Doc._.emoji`        | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the document's emoji. |
-        | `Span._.has_emoji`   | bool                       | Whether the span contains emoji.                              |
-        | `Span._.emoji`       | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the span's emoji.     |
-        
-        ## Settings
-        
-        You can configure the `emoji` factory by setting any of the following parameters in
-        the `config` dictionary:
-        
-        | Setting       | Type                      | Description                                                                                                                            |
-        | ------------- | ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
-        | `attrs`       | Tuple[str, str, str, str] | Attributes to set on the `._` property. Defaults to `('has_emoji', 'is_emoji', 'emoji_desc', 'emoji')`.                                |
-        | `pattern_id`  | str                       | ID of match pattern, defaults to `'EMOJI'`. Can be changed to avoid ID conflicts.                                                      |
-        | `merge_spans` | bool                      | Merge spans containing multi-character emoji, defaults to `True`. Will only merge combined emoji resulting in one icon, not sequences. |
-        | `lookup`      | Dict[str, str]            | Optional lookup table that maps emoji strings to custom descriptions, e.g. translations or other annotations.                          |
-        
-        ```python
-        emoji_config = {"attrs": ("has_e", "is_e", "e_desc", "e"), lookup={"👨‍🎤": "David Bowie"})
-        nlp.add_pipe(emoji, first=True, config=emoji_config)
-        doc = nlp("We can be 👨‍🎤 heroes")
-        assert doc[3]._.is_e
-        assert doc[3]._.e_desc == "David Bowie"
-        ```
-        
-        If you're training a pipeline, you can define the component config in your [`config.cfg`](https://spacy.io/usage/training):
-        
-        ```ini
-        [nlp]
-        pipeline = ["emoji", "ner"]
-        # ...
-        
-        [components.emoji]
-        factory = "emoji"
-        merge_spans = false
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# spacymoji: emoji for spaCy
+
+[spaCy](https://spacy.io) extension and pipeline component for adding emoji meta
+data to `Doc` objects. Detects emoji consisting of one or more unicode
+characters, and can optionally merge multi-char emoji (combined pictures, emoji
+with skin tone modifiers) into one token. Human-readable emoji descriptions are
+added as a custom attribute, and an optional lookup table can be provided for
+your own descriptions. The extension sets the custom `Doc`, `Token` and `Span`
+attributes `._.is_emoji`, `._.emoji_desc`, `._.has_emoji` and `._.emoji`. You
+can read more about custom pipeline components and extension attributes
+[here](https://spacy.io/usage/processing-pipelines).
+
+Emoji are matched using spaCy's
+[`PhraseMatcher`](https://spacy.io/api/phrasematcher), and looked up in the data
+table provided by the [`emoji` package](https://github.com/carpedm20/emoji).
+
+[![tests](https://github.com/explosion/spacymoji/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/spacymoji/actions/workflows/tests.yml)
+[![Current Release Version](https://img.shields.io/github/release/explosion/spacymoji.svg?style=flat-square&logo=github)](https://github.com/explosion/spacymoji/releases)
+[![pypi Version](https://img.shields.io/pypi/v/spacymoji.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacymoji/)
+
+# ⏳ Installation
+
+`spacymoji` requires `spacy` v3.0.0 or higher. For spaCy v2.x, install
+`spacymoji==2.0.0`.
+
+```bash
+pip install spacymoji
+```
+
+# ☝️ Usage
+
+Import the component and add it anywhere in your pipeline using the string name
+of the `"emoji"` component factory:
+
+```python
+import spacy
+
+nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe("emoji", first=True)
+doc = nlp("This is a test 😻 👍🏿")
+assert doc._.has_emoji is True
+assert doc[2:5]._.has_emoji is True
+assert doc[0]._.is_emoji is False
+assert doc[4]._.is_emoji is True
+assert doc[5]._.emoji_desc == "thumbs up dark skin tone"
+assert len(doc._.emoji) == 2
+assert doc._.emoji[1] == ("👍🏿", 5, "thumbs up dark skin tone")
+```
+
+`spacymoji` only cares about the token text, so you can use it on a blank
+`Language` instance (it should work for all
+[available languages](https://spacy.io/usage/models#languages)!), or in a
+pipeline with a loaded pipeline. If your pipeline includes a tagger, parser and
+entity recognizer, make sure to add the emoji component as `first=True`, so the
+spans are merged right after tokenization, and _before_ the document is parsed.
+If your text contains a lot of emoji, this might even give you a nice boost in
+parser accuracy.
+
+## Available attributes
+
+The extension sets attributes on the `Doc`, `Span` and `Token`. You can change
+the attribute names (and other parameters of the Emoji component) by passing
+them via the `config` parameter in the `nlp.add_pipe(...)` method. For more
+details on custom components and attributes, see the
+[processing pipelines documentation](https://spacy.io/usage/processing-pipelines#custom-components).
+
+| Attribute            | Type                       | Description                                                   |
+| -------------------- | -------------------------- | ------------------------------------------------------------- |
+| `Token._.is_emoji`   | bool                       | Whether the token is an emoji.                                |
+| `Token._.emoji_desc` | str                        | A human-readable description of the emoji.                    |
+| `Doc._.has_emoji`    | bool                       | Whether the document contains emoji.                          |
+| `Doc._.emoji`        | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the document's emoji. |
+| `Span._.has_emoji`   | bool                       | Whether the span contains emoji.                              |
+| `Span._.emoji`       | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the span's emoji.     |
+
+## Settings
+
+You can configure the `emoji` factory by setting any of the following parameters
+in the `config` dictionary:
+
+| Setting       | Type                      | Description                                                                                                                            |
+| ------------- | ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
+| `attrs`       | Tuple[str, str, str, str] | Attributes to set on the `._` property. Defaults to `('has_emoji', 'is_emoji', 'emoji_desc', 'emoji')`.                                |
+| `pattern_id`  | str                       | ID of match pattern, defaults to `'EMOJI'`. Can be changed to avoid ID conflicts.                                                      |
+| `merge_spans` | bool                      | Merge spans containing multi-character emoji, defaults to `True`. Will only merge combined emoji resulting in one icon, not sequences. |
+| `lookup`      | Dict[str, str]            | Optional lookup table that maps emoji strings to custom descriptions, e.g. translations or other annotations.                          |
+
+```python
+emoji_config = {"attrs": ("has_e", "is_e", "e_desc", "e"), lookup={"👨‍🎤": "David Bowie"})
+nlp.add_pipe(emoji, first=True, config=emoji_config)
+doc = nlp("We can be 👨‍🎤 heroes")
+assert doc[3]._.is_e
+assert doc[3]._.e_desc == "David Bowie"
+```
+
+If you're training a pipeline, you can define the component config in your
+[`config.cfg`](https://spacy.io/usage/training):
+
+```ini
+[nlp]
+pipeline = ["emoji", "ner"]
+# ...
+
+[components.emoji]
+factory = "emoji"
+merge_spans = false
+```
```

### Comparing `spacymoji-3.0.1/README.md` & `spacymoji-3.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 # spacymoji: emoji for spaCy
 
-[spaCy](https://spacy.io) extension and pipeline component
-for adding emoji meta data to `Doc` objects. Detects emoji consisting of one
-or more unicode characters, and can optionally merge multi-char emoji (combined
-pictures, emoji with skin tone modifiers) into one token. Human-readable emoji
-descriptions are added as a custom attribute, and an optional lookup table can
-be provided for your own descriptions. The extension sets the custom `Doc`,
-`Token` and `Span` attributes `._.is_emoji`, `._.emoji_desc`, `._.has_emoji` and `._.emoji`. You can read more about custom pipeline components and extension attributes [here](https://spacy.io/usage/processing-pipelines).
+[spaCy](https://spacy.io) extension and pipeline component for adding emoji meta
+data to `Doc` objects. Detects emoji consisting of one or more unicode
+characters, and can optionally merge multi-char emoji (combined pictures, emoji
+with skin tone modifiers) into one token. Human-readable emoji descriptions are
+added as a custom attribute, and an optional lookup table can be provided for
+your own descriptions. The extension sets the custom `Doc`, `Token` and `Span`
+attributes `._.is_emoji`, `._.emoji_desc`, `._.has_emoji` and `._.emoji`. You
+can read more about custom pipeline components and extension attributes
+[here](https://spacy.io/usage/processing-pipelines).
 
-Emoji are matched using spaCy's [`PhraseMatcher`](https://spacy.io/api/phrasematcher), and looked up in the data
+Emoji are matched using spaCy's
+[`PhraseMatcher`](https://spacy.io/api/phrasematcher), and looked up in the data
 table provided by the [`emoji` package](https://github.com/carpedm20/emoji).
 
-[![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/22/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=22)
+[![tests](https://github.com/explosion/spacymoji/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/spacymoji/actions/workflows/tests.yml)
 [![Current Release Version](https://img.shields.io/github/release/explosion/spacymoji.svg?style=flat-square&logo=github)](https://github.com/explosion/spacymoji/releases)
 [![pypi Version](https://img.shields.io/pypi/v/spacymoji.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacymoji/)
 
 # ⏳ Installation
 
-`spacymoji` requires `spacy` v3.0.0 or higher. For spaCy v2.x, instally `spacymoji==2.0.0`.
+`spacymoji` requires `spacy` v3.0.0 or higher. For spaCy v2.x, install
+`spacymoji==2.0.0`.
 
 ```bash
 pip install spacymoji
 ```
 
 # ☝️ Usage
 
-Import the component and add it anywhere in your pipeline using the string
-name of the `"emoji"` component factory:
+Import the component and add it anywhere in your pipeline using the string name
+of the `"emoji"` component factory:
 
 ```python
 import spacy
 
 nlp = spacy.load("en_core_web_sm")
 nlp.add_pipe("emoji", first=True)
 doc = nlp("This is a test 😻 👍🏿")
@@ -41,42 +45,42 @@
 assert doc[5]._.emoji_desc == "thumbs up dark skin tone"
 assert len(doc._.emoji) == 2
 assert doc._.emoji[1] == ("👍🏿", 5, "thumbs up dark skin tone")
 ```
 
 `spacymoji` only cares about the token text, so you can use it on a blank
 `Language` instance (it should work for all
-[available languages](https://spacy.io/usage/models#languages)!), or in
-a pipeline with a loaded pipeline. If your pipeline
-includes a tagger, parser and entity recognizer, make sure to add the emoji
-component as `first=True`, so the spans are merged right after tokenization,
-and _before_ the document is parsed. If your text contains a lot of emoji, this
-might even give you a nice boost in parser accuracy.
+[available languages](https://spacy.io/usage/models#languages)!), or in a
+pipeline with a loaded pipeline. If your pipeline includes a tagger, parser and
+entity recognizer, make sure to add the emoji component as `first=True`, so the
+spans are merged right after tokenization, and _before_ the document is parsed.
+If your text contains a lot of emoji, this might even give you a nice boost in
+parser accuracy.
 
 ## Available attributes
 
-The extension sets attributes on the `Doc`, `Span` and `Token`. You can
-change the attribute names (and other parameters of the Emoji component) by passing
-them via the `config` parameter in the `nlp.add_pipe(...)` method. For more details
-on custom components and attributes, see the
+The extension sets attributes on the `Doc`, `Span` and `Token`. You can change
+the attribute names (and other parameters of the Emoji component) by passing
+them via the `config` parameter in the `nlp.add_pipe(...)` method. For more
+details on custom components and attributes, see the
 [processing pipelines documentation](https://spacy.io/usage/processing-pipelines#custom-components).
 
 | Attribute            | Type                       | Description                                                   |
 | -------------------- | -------------------------- | ------------------------------------------------------------- |
 | `Token._.is_emoji`   | bool                       | Whether the token is an emoji.                                |
 | `Token._.emoji_desc` | str                        | A human-readable description of the emoji.                    |
 | `Doc._.has_emoji`    | bool                       | Whether the document contains emoji.                          |
 | `Doc._.emoji`        | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the document's emoji. |
 | `Span._.has_emoji`   | bool                       | Whether the span contains emoji.                              |
 | `Span._.emoji`       | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the span's emoji.     |
 
 ## Settings
 
-You can configure the `emoji` factory by setting any of the following parameters in
-the `config` dictionary:
+You can configure the `emoji` factory by setting any of the following parameters
+in the `config` dictionary:
 
 | Setting       | Type                      | Description                                                                                                                            |
 | ------------- | ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
 | `attrs`       | Tuple[str, str, str, str] | Attributes to set on the `._` property. Defaults to `('has_emoji', 'is_emoji', 'emoji_desc', 'emoji')`.                                |
 | `pattern_id`  | str                       | ID of match pattern, defaults to `'EMOJI'`. Can be changed to avoid ID conflicts.                                                      |
 | `merge_spans` | bool                      | Merge spans containing multi-character emoji, defaults to `True`. Will only merge combined emoji resulting in one icon, not sequences. |
 | `lookup`      | Dict[str, str]            | Optional lookup table that maps emoji strings to custom descriptions, e.g. translations or other annotations.                          |
@@ -85,15 +89,16 @@
 emoji_config = {"attrs": ("has_e", "is_e", "e_desc", "e"), lookup={"👨‍🎤": "David Bowie"})
 nlp.add_pipe(emoji, first=True, config=emoji_config)
 doc = nlp("We can be 👨‍🎤 heroes")
 assert doc[3]._.is_e
 assert doc[3]._.e_desc == "David Bowie"
 ```
 
-If you're training a pipeline, you can define the component config in your [`config.cfg`](https://spacy.io/usage/training):
+If you're training a pipeline, you can define the component config in your
+[`config.cfg`](https://spacy.io/usage/training):
 
 ```ini
 [nlp]
 pipeline = ["emoji", "ner"]
 # ...
 
 [components.emoji]
```

### Comparing `spacymoji-3.0.1/setup.cfg` & `spacymoji-3.1.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
-version = 3.0.1
-description = spaCy pipeline component for adding emoji meta data to Doc, Token and Span objects
+version = 3.1.0
+description = spaCy pipeline component for adding emoji metadata to Doc, Token and Span objects
 url = https://github.com/explosion/spacymoji
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers = 
@@ -16,23 +16,26 @@
 	Operating System :: POSIX :: Linux
 	Operating System :: MacOS :: MacOS X
 	Operating System :: Microsoft :: Windows
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 
 [options]
 zip_safe = true
 include_package_data = true
 python_requires = >=3.6
 install_requires = 
 	spacy>=3.0.0,<4.0.0
-	emoji>=0.4.5,<1.0.0
+	emoji>=2.0,<3.0
 
 [options.entry_points]
 spacy_factories = 
 	emoji = spacymoji:create_emoji
 
 [bdist_wheel]
 universal = true
```

### Comparing `spacymoji-3.0.1/spacymoji/__init__.py` & `spacymoji-3.1.0/spacymoji/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from typing import Dict, Optional, Tuple, List, Union
-from spacy.tokens import Doc, Span, Token
-from spacy.matcher import PhraseMatcher
+from typing import Dict, List, Optional, Tuple, Union
+
+# from emoji import UNICODE_EMOJI
+from emoji import EMOJI_DATA
 from spacy.language import Language
+from spacy.matcher import PhraseMatcher
+from spacy.tokens import Doc, Span, Token
 from spacy.util import filter_spans
-from emoji import UNICODE_EMOJI
-
 
 # Make sure multi-character emoji don't contain whitespace
-EMOJI = {e.replace(" ", ""): t for e, t in UNICODE_EMOJI.items()}
+EMOJI = dict()
+for e, data in EMOJI_DATA.items():
+    EMOJI[e.replace(" ", "")] = data.get("en", "")
 
 DEFAULT_ATTRS = ("has_emoji", "is_emoji", "emoji_desc", "emoji")
 
 DEFAULT_CONFIG = {
     "merge_spans": True,
     "lookup": {},
     "pattern_id": "EMOJI",
```

### Comparing `spacymoji-3.0.1/spacymoji/tests/test_emoji.py` & `spacymoji-3.1.0/spacymoji/tests/test_emoji.py`

 * *Files identical despite different names*

### Comparing `spacymoji-3.0.1/spacymoji.egg-info/PKG-INFO` & `spacymoji-3.1.0/spacymoji.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,127 +1,135 @@
 Metadata-Version: 2.1
 Name: spacymoji
-Version: 3.0.1
-Summary: spaCy pipeline component for adding emoji meta data to Doc, Token and Span objects
+Version: 3.1.0
+Summary: spaCy pipeline component for adding emoji metadata to Doc, Token and Span objects
 Home-page: https://github.com/explosion/spacymoji
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
-Description: # spacymoji: emoji for spaCy
-        
-        [spaCy](https://spacy.io) extension and pipeline component
-        for adding emoji meta data to `Doc` objects. Detects emoji consisting of one
-        or more unicode characters, and can optionally merge multi-char emoji (combined
-        pictures, emoji with skin tone modifiers) into one token. Human-readable emoji
-        descriptions are added as a custom attribute, and an optional lookup table can
-        be provided for your own descriptions. The extension sets the custom `Doc`,
-        `Token` and `Span` attributes `._.is_emoji`, `._.emoji_desc`, `._.has_emoji` and `._.emoji`. You can read more about custom pipeline components and extension attributes [here](https://spacy.io/usage/processing-pipelines).
-        
-        Emoji are matched using spaCy's [`PhraseMatcher`](https://spacy.io/api/phrasematcher), and looked up in the data
-        table provided by the [`emoji` package](https://github.com/carpedm20/emoji).
-        
-        [![Azure Pipelines](https://img.shields.io/azure-devops/build/explosion-ai/public/22/master.svg?logo=azure-pipelines&style=flat-square&label=build)](https://dev.azure.com/explosion-ai/public/_build?definitionId=22)
-        [![Current Release Version](https://img.shields.io/github/release/explosion/spacymoji.svg?style=flat-square&logo=github)](https://github.com/explosion/spacymoji/releases)
-        [![pypi Version](https://img.shields.io/pypi/v/spacymoji.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacymoji/)
-        
-        # ⏳ Installation
-        
-        `spacymoji` requires `spacy` v3.0.0 or higher. For spaCy v2.x, instally `spacymoji==2.0.0`.
-        
-        ```bash
-        pip install spacymoji
-        ```
-        
-        # ☝️ Usage
-        
-        Import the component and add it anywhere in your pipeline using the string
-        name of the `"emoji"` component factory:
-        
-        ```python
-        import spacy
-        
-        nlp = spacy.load("en_core_web_sm")
-        nlp.add_pipe("emoji", first=True)
-        doc = nlp("This is a test 😻 👍🏿")
-        assert doc._.has_emoji is True
-        assert doc[2:5]._.has_emoji is True
-        assert doc[0]._.is_emoji is False
-        assert doc[4]._.is_emoji is True
-        assert doc[5]._.emoji_desc == "thumbs up dark skin tone"
-        assert len(doc._.emoji) == 2
-        assert doc._.emoji[1] == ("👍🏿", 5, "thumbs up dark skin tone")
-        ```
-        
-        `spacymoji` only cares about the token text, so you can use it on a blank
-        `Language` instance (it should work for all
-        [available languages](https://spacy.io/usage/models#languages)!), or in
-        a pipeline with a loaded pipeline. If your pipeline
-        includes a tagger, parser and entity recognizer, make sure to add the emoji
-        component as `first=True`, so the spans are merged right after tokenization,
-        and _before_ the document is parsed. If your text contains a lot of emoji, this
-        might even give you a nice boost in parser accuracy.
-        
-        ## Available attributes
-        
-        The extension sets attributes on the `Doc`, `Span` and `Token`. You can
-        change the attribute names (and other parameters of the Emoji component) by passing
-        them via the `config` parameter in the `nlp.add_pipe(...)` method. For more details
-        on custom components and attributes, see the
-        [processing pipelines documentation](https://spacy.io/usage/processing-pipelines#custom-components).
-        
-        | Attribute            | Type                       | Description                                                   |
-        | -------------------- | -------------------------- | ------------------------------------------------------------- |
-        | `Token._.is_emoji`   | bool                       | Whether the token is an emoji.                                |
-        | `Token._.emoji_desc` | str                        | A human-readable description of the emoji.                    |
-        | `Doc._.has_emoji`    | bool                       | Whether the document contains emoji.                          |
-        | `Doc._.emoji`        | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the document's emoji. |
-        | `Span._.has_emoji`   | bool                       | Whether the span contains emoji.                              |
-        | `Span._.emoji`       | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the span's emoji.     |
-        
-        ## Settings
-        
-        You can configure the `emoji` factory by setting any of the following parameters in
-        the `config` dictionary:
-        
-        | Setting       | Type                      | Description                                                                                                                            |
-        | ------------- | ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
-        | `attrs`       | Tuple[str, str, str, str] | Attributes to set on the `._` property. Defaults to `('has_emoji', 'is_emoji', 'emoji_desc', 'emoji')`.                                |
-        | `pattern_id`  | str                       | ID of match pattern, defaults to `'EMOJI'`. Can be changed to avoid ID conflicts.                                                      |
-        | `merge_spans` | bool                      | Merge spans containing multi-character emoji, defaults to `True`. Will only merge combined emoji resulting in one icon, not sequences. |
-        | `lookup`      | Dict[str, str]            | Optional lookup table that maps emoji strings to custom descriptions, e.g. translations or other annotations.                          |
-        
-        ```python
-        emoji_config = {"attrs": ("has_e", "is_e", "e_desc", "e"), lookup={"👨‍🎤": "David Bowie"})
-        nlp.add_pipe(emoji, first=True, config=emoji_config)
-        doc = nlp("We can be 👨‍🎤 heroes")
-        assert doc[3]._.is_e
-        assert doc[3]._.e_desc == "David Bowie"
-        ```
-        
-        If you're training a pipeline, you can define the component config in your [`config.cfg`](https://spacy.io/usage/training):
-        
-        ```ini
-        [nlp]
-        pipeline = ["emoji", "ner"]
-        # ...
-        
-        [components.emoji]
-        factory = "emoji"
-        merge_spans = false
-        ```
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# spacymoji: emoji for spaCy
+
+[spaCy](https://spacy.io) extension and pipeline component for adding emoji meta
+data to `Doc` objects. Detects emoji consisting of one or more unicode
+characters, and can optionally merge multi-char emoji (combined pictures, emoji
+with skin tone modifiers) into one token. Human-readable emoji descriptions are
+added as a custom attribute, and an optional lookup table can be provided for
+your own descriptions. The extension sets the custom `Doc`, `Token` and `Span`
+attributes `._.is_emoji`, `._.emoji_desc`, `._.has_emoji` and `._.emoji`. You
+can read more about custom pipeline components and extension attributes
+[here](https://spacy.io/usage/processing-pipelines).
+
+Emoji are matched using spaCy's
+[`PhraseMatcher`](https://spacy.io/api/phrasematcher), and looked up in the data
+table provided by the [`emoji` package](https://github.com/carpedm20/emoji).
+
+[![tests](https://github.com/explosion/spacymoji/actions/workflows/tests.yml/badge.svg)](https://github.com/explosion/spacymoji/actions/workflows/tests.yml)
+[![Current Release Version](https://img.shields.io/github/release/explosion/spacymoji.svg?style=flat-square&logo=github)](https://github.com/explosion/spacymoji/releases)
+[![pypi Version](https://img.shields.io/pypi/v/spacymoji.svg?style=flat-square&logo=pypi&logoColor=white)](https://pypi.org/project/spacymoji/)
+
+# ⏳ Installation
+
+`spacymoji` requires `spacy` v3.0.0 or higher. For spaCy v2.x, install
+`spacymoji==2.0.0`.
+
+```bash
+pip install spacymoji
+```
+
+# ☝️ Usage
+
+Import the component and add it anywhere in your pipeline using the string name
+of the `"emoji"` component factory:
+
+```python
+import spacy
+
+nlp = spacy.load("en_core_web_sm")
+nlp.add_pipe("emoji", first=True)
+doc = nlp("This is a test 😻 👍🏿")
+assert doc._.has_emoji is True
+assert doc[2:5]._.has_emoji is True
+assert doc[0]._.is_emoji is False
+assert doc[4]._.is_emoji is True
+assert doc[5]._.emoji_desc == "thumbs up dark skin tone"
+assert len(doc._.emoji) == 2
+assert doc._.emoji[1] == ("👍🏿", 5, "thumbs up dark skin tone")
+```
+
+`spacymoji` only cares about the token text, so you can use it on a blank
+`Language` instance (it should work for all
+[available languages](https://spacy.io/usage/models#languages)!), or in a
+pipeline with a loaded pipeline. If your pipeline includes a tagger, parser and
+entity recognizer, make sure to add the emoji component as `first=True`, so the
+spans are merged right after tokenization, and _before_ the document is parsed.
+If your text contains a lot of emoji, this might even give you a nice boost in
+parser accuracy.
+
+## Available attributes
+
+The extension sets attributes on the `Doc`, `Span` and `Token`. You can change
+the attribute names (and other parameters of the Emoji component) by passing
+them via the `config` parameter in the `nlp.add_pipe(...)` method. For more
+details on custom components and attributes, see the
+[processing pipelines documentation](https://spacy.io/usage/processing-pipelines#custom-components).
+
+| Attribute            | Type                       | Description                                                   |
+| -------------------- | -------------------------- | ------------------------------------------------------------- |
+| `Token._.is_emoji`   | bool                       | Whether the token is an emoji.                                |
+| `Token._.emoji_desc` | str                        | A human-readable description of the emoji.                    |
+| `Doc._.has_emoji`    | bool                       | Whether the document contains emoji.                          |
+| `Doc._.emoji`        | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the document's emoji. |
+| `Span._.has_emoji`   | bool                       | Whether the span contains emoji.                              |
+| `Span._.emoji`       | List[Tuple[str, int, str]] | `(emoji, index, description)` tuples of the span's emoji.     |
+
+## Settings
+
+You can configure the `emoji` factory by setting any of the following parameters
+in the `config` dictionary:
+
+| Setting       | Type                      | Description                                                                                                                            |
+| ------------- | ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
+| `attrs`       | Tuple[str, str, str, str] | Attributes to set on the `._` property. Defaults to `('has_emoji', 'is_emoji', 'emoji_desc', 'emoji')`.                                |
+| `pattern_id`  | str                       | ID of match pattern, defaults to `'EMOJI'`. Can be changed to avoid ID conflicts.                                                      |
+| `merge_spans` | bool                      | Merge spans containing multi-character emoji, defaults to `True`. Will only merge combined emoji resulting in one icon, not sequences. |
+| `lookup`      | Dict[str, str]            | Optional lookup table that maps emoji strings to custom descriptions, e.g. translations or other annotations.                          |
+
+```python
+emoji_config = {"attrs": ("has_e", "is_e", "e_desc", "e"), lookup={"👨‍🎤": "David Bowie"})
+nlp.add_pipe(emoji, first=True, config=emoji_config)
+doc = nlp("We can be 👨‍🎤 heroes")
+assert doc[3]._.is_e
+assert doc[3]._.e_desc == "David Bowie"
+```
+
+If you're training a pipeline, you can define the component config in your
+[`config.cfg`](https://spacy.io/usage/training):
+
+```ini
+[nlp]
+pipeline = ["emoji", "ner"]
+# ...
+
+[components.emoji]
+factory = "emoji"
+merge_spans = false
+```
```

