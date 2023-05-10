# Comparing `tmp/changelogging-1.1.0.tar.gz` & `tmp/changelogging-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "changelogging-1.1.0.tar", max compression
+gzip compressed data, was "changelogging-1.2.0.tar", max compression
```

## Comparing `changelogging-1.1.0.tar` & `changelogging-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1092 2023-01-27 19:37:40.012385 changelogging-1.1.0/LICENSE
--rw-r--r--   0        0        0     3098 2023-01-27 19:37:40.012385 changelogging-1.1.0/README.md
--rw-r--r--   0        0        0      517 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/__init__.py
--rw-r--r--   0        0        0      122 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/__main__.py
--rw-r--r--   0        0        0     7908 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/build.py
--rw-r--r--   0        0        0      810 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/changelogging.toml
--rw-r--r--   0        0        0    13464 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/config.py
--rw-r--r--   0        0        0      492 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/constants.py
--rw-r--r--   0        0        0     6037 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/fragments.py
--rw-r--r--   0        0        0      552 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/git.py
--rw-r--r--   0        0        0     2905 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/main.py
--rw-r--r--   0        0        0        0 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/py.typed
--rw-r--r--   0        0        0      614 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/typing.py
--rw-r--r--   0        0        0      915 2023-01-27 19:37:40.012385 changelogging-1.1.0/changelogging/utils.py
--rw-r--r--   0        0        0     3361 2023-01-27 19:37:40.012385 changelogging-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4130 1970-01-01 00:00:00.000000 changelogging-1.1.0/setup.py
--rw-r--r--   0        0        0     4547 1970-01-01 00:00:00.000000 changelogging-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-10 15:46:44.941030 changelogging-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3098 2023-05-10 15:46:44.941030 changelogging-1.2.0/README.md
+-rw-r--r--   0        0        0      517 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/__init__.py
+-rw-r--r--   0        0        0      122 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/__main__.py
+-rw-r--r--   0        0        0     9824 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/build.py
+-rw-r--r--   0        0        0      810 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/changelogging.toml
+-rw-r--r--   0        0        0    13857 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/config.py
+-rw-r--r--   0        0        0      645 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/constants.py
+-rw-r--r--   0        0        0     6040 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/fragments.py
+-rw-r--r--   0        0        0      803 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/git.py
+-rw-r--r--   0        0        0     2966 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/main.py
+-rw-r--r--   0        0        0        0 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/py.typed
+-rw-r--r--   0        0        0      321 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/typing.py
+-rw-r--r--   0        0        0     1443 2023-05-10 15:46:44.941030 changelogging-1.2.0/changelogging/utils.py
+-rw-r--r--   0        0        0     3545 2023-05-10 15:46:44.941030 changelogging-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4610 1970-01-01 00:00:00.000000 changelogging-1.2.0/PKG-INFO
```

### Comparing `changelogging-1.1.0/LICENSE` & `changelogging-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `changelogging-1.1.0/README.md` & `changelogging-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add changelogging
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-changelogging = "^1.1.0"
+changelogging = "^1.2.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.changelogging]
 git = "https://github.com/nekitdev/changelogging.git"
```

### Comparing `changelogging-1.1.0/changelogging/__init__.py` & `changelogging-1.2.0/changelogging/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 
 __description__ = "Building changelogs from fragments."
 __url__ = "https://github.com/nekitdev/changelogging"
 
 __title__ = "changelogging"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 from changelogging.build import Builder
 from changelogging.config import Config
 from changelogging.fragments import Display, Fragment, FragmentType, FragmentTypes, Issue
 
 __all__ = ("Builder", "Config", "Display", "Fragment", "FragmentType", "FragmentTypes", "Issue")
```

### Comparing `changelogging-1.1.0/changelogging/build.py` & `changelogging-1.2.0/changelogging/build.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,50 @@
 from collections import defaultdict as default_dict
 from pathlib import Path
 from textwrap import wrap
 from typing import Dict, Iterable, Iterator, List, Mapping, Tuple, TypeVar
 
 from attrs import define, field
-from pendulum import Date, now
-from typing_extensions import Literal
+from funcs.typing import Binary, Unary
+from funcs.unpacking import unpack_binary
+from iters.iters import iter, wrap_iter
+from pendulum import Date
 
 from changelogging.config import Config
-from changelogging.constants import DOT, DOUBLE_NEW_LINE, EMPTY, HASH, NEW_LINE, SPACE
+from changelogging.constants import (
+    DEFAULT_ENCODING,
+    DEFAULT_ERRORS,
+    DOT,
+    DOUBLE_NEW_LINE,
+    EMPTY,
+    HASH,
+    NEW_LINE,
+    SPACE,
+    WRITE,
+)
 from changelogging.fragments import Fragment, FragmentType, Issue
+from changelogging.utils import left_strip, split_lines, today
 
 __all__ = ("Builder",)
 
 NO_SIGNIFICANT_CHANGES = "No significant changes."
 
-concat_new_line = NEW_LINE.join
-concat_double_new_line = DOUBLE_NEW_LINE.join
-
-WRITE: Literal["w"] = "w"
-
-
-def today() -> Date:
-    return now().date()  # type: ignore
-
-
 FT = TypeVar("FT", bound=FragmentType)
 IT = TypeVar("IT", bound=Issue)
 
 Fragments = Iterable[Fragment[FT, IT]]
 Sections = Mapping[FT, Fragments[FT, IT]]
 
 
+def get_path(item: Tuple[Path, FragmentType]) -> Path:  # pragma: no cover  # `main` only
+    path, _ = item
+
+    return path
+
+
 @define()
 class Builder:
     """Represents changelog builders."""
 
     config: Config = field()
     """The config of the builder."""
 
@@ -106,15 +115,15 @@
 
         Arguments:
             fragments: The fragments to build.
 
         Returns:
             The fragments built.
         """
-        return concat_new_line(map(self.build_fragment, fragments))
+        return iter(fragments).map(self.build_fragment).join(NEW_LINE)
 
     def collect_sections(self, fragments: Fragments[FT, IT]) -> Sections[FT, IT]:
         """Collects `fragments` into sections.
 
         Arguments:
             fragments: The fragments to collect.
 
@@ -127,14 +136,15 @@
             sections[fragment.type].append(fragment)
 
         for fragments in sections.values():
             fragments.sort()
 
         return sections
 
+    @wrap_iter
     def build_generate(self, sections: Sections[FragmentType, Issue]) -> Iterator[str]:
         """Builds `sections`, returning an iterator.
 
         Arguments:
             sections: The sections to build.
 
         Returns:
@@ -154,87 +164,133 @@
 
                 yield self.build_section_title(type)
                 yield self.build_fragments(fragments)
 
         if empty:  # pragma: no cover  # not tested
             yield NO_SIGNIFICANT_CHANGES
 
-    def collect_fragments(self) -> Fragments[FragmentType, Issue]:
+    def fetch_fragment(
+        self,
+        path: Path,
+        type: FragmentType,
+        encoding: str = DEFAULT_ENCODING,
+        errors: str = DEFAULT_ERRORS,
+    ) -> Fragment[FragmentType, Issue]:
+        """Fetches a fragment of `type` from `path`.
+
+        Arguments:
+            path: The path to fetch the fragment from.
+            type: The type of the fragment to fetch.
+            encoding: The encoding to use.
+            errors: The error handling strategy to use.
+
+        Returns:
+            The fetched fragment.
+        """
+        issue = self.get_issue(path)
+        content = path.read_text(encoding, errors)
+
+        return Fragment(type, content, issue)
+
+    def fetching_fragment(
+        self, encoding: str = DEFAULT_ENCODING, errors: str = DEFAULT_ERRORS
+    ) -> Binary[Path, FragmentType, Fragment[FragmentType, Issue]]:
+        def fetch_fragment(path: Path, type: FragmentType) -> Fragment[FragmentType, Issue]:
+            return self.fetch_fragment(path, type, encoding, errors)
+
+        return fetch_fragment
+
+    @wrap_iter
+    def collect_fragments(
+        self, encoding: str = DEFAULT_ENCODING, errors: str = DEFAULT_ERRORS
+    ) -> Fragments[FragmentType, Issue]:
         """Collects fragments from the changes directory specified in the config.
 
+        Arguments:
+            encoding: The encoding to use.
+            errors: The error handling strategy to use.
+
         Returns:
             The iterator over the fragments found.
         """
-        for path, type in self.collect_paths_types():
-            issue = self.get_issue(path)
-            content = path.read_text()
-
-            yield Fragment(type, content, issue)
+        return (
+            self.collect_paths_types()
+            .map(unpack_binary(self.fetching_fragment(encoding, errors)))
+            .unwrap()
+        )
 
+    @wrap_iter
     def collect_paths_types(self) -> Iterator[Tuple[Path, FragmentType]]:
         config = self.config
         directory = config.directory
         types = config.types
 
+        # TODO: perhaps rewrite this using iterators?
+
         for path in directory.iterdir():
             if path.is_file():
                 for suffix in path.suffixes:
                     if types.has_suffix(suffix):
                         yield (path, types.get_suffix(suffix))
 
-    def collect_paths(self) -> Iterator[Path]:  # pragma: no cover  # only used in `main`
+    @wrap_iter
+    def collect_paths(self) -> Iterator[Path]:
         """Collect paths to fragments.
 
         Returns:
             The iterator over paths found.
         """
-        for path, _ in self.collect_paths_types():
-            yield path
+        return self.collect_paths_types().map(get_path).unwrap()  # pragma: no cover  # `main` only
 
     @classmethod
     def get_issue(cls, path: Path) -> Issue:
         return Issue(int(cls.name_no_suffixes(path)))
 
     def build(self) -> str:
         """Builds the changelog.
 
         Returns:
             The build result.
         """
-        return concat_double_new_line(
-            self.build_generate(self.collect_sections(self.collect_fragments()))
+        return self.build_generate(self.collect_sections(self.collect_fragments().unwrap())).join(
+            DOUBLE_NEW_LINE
         )
 
-    def write(self) -> None:
-        """Builds the changelog and writes it to the output file."""
+    def write(self, encoding: str = DEFAULT_ENCODING, errors: str = DEFAULT_ERRORS) -> None:
+        """Builds the changelog and writes it to the output file.
+
+        Arguments:
+            encoding: The encoding to use.
+            errors: The error handling strategy to use.
+        """
         config = self.config
 
         output = config.output
         start_string = config.start_string
 
         content = self.build()
 
-        current = output.read_text() if output.exists() else EMPTY
+        current = output.read_text(encoding, errors) if output.exists() else EMPTY
 
         before, start, after = current.partition(start_string)
 
-        with output.open(WRITE) as file:
+        with output.open(WRITE, encoding=encoding, errors=errors) as file:
             if not start:  # pragma: no cover  # not tested
                 file.write(content + NEW_LINE)
 
                 if current.strip():
-                    file.write(NEW_LINE + current.lstrip())
+                    file.write(NEW_LINE + left_strip(current))
 
             else:
                 file.write(before)
                 file.write(start)
                 file.write(DOUBLE_NEW_LINE + content + NEW_LINE)
 
                 if after.strip():
-                    file.write(NEW_LINE + after.lstrip())
+                    file.write(NEW_LINE + left_strip(after))
 
     @staticmethod
     def heading(level: int) -> str:
         return HASH * level + SPACE
 
     @staticmethod
     def indents(bullet: str) -> Tuple[str, str]:
@@ -243,35 +299,39 @@
 
     @staticmethod
     def name_no_suffixes(path: Path) -> str:
         name, _, _ = path.name.partition(DOT)
         return name
 
     @classmethod
+    @wrap_iter
     def generate_indent_lines(cls, string: str, bullet: str) -> Iterator[str]:
         if not string:  # pragma: no cover  # not tested
             return
 
         initial, subsequent = cls.indents(bullet)
 
-        head, *tail = string.splitlines()
+        head, *tail = split_lines(string)
 
         yield (initial + head if head.strip() else head)
 
         for item in tail:
             yield (subsequent + item if item.strip() else item)
 
     @classmethod
     def indent_lines(cls, string: str, bullet: str) -> str:
-        return concat_new_line(cls.generate_indent_lines(string, bullet))
+        return cls.generate_indent_lines(string, bullet).join(NEW_LINE)
+
+    @staticmethod
+    def wrapping_line(size: int) -> Unary[str, str]:
+        def wrap_line(line: str) -> str:
+            return iter(wrap(line, size, break_long_words=False)).join(NEW_LINE)
+
+        return wrap_line
 
     @classmethod
     def indent_wrap_lines(cls, string: str, bullet: str, size: int) -> str:
-        size -= max(map(len, cls.indents(bullet)))
+        size -= iter(cls.indents(bullet)).map(len).max().unwrap()
 
         return cls.indent_lines(
-            concat_new_line(
-                concat_new_line(wrap(line, size, break_long_words=False))
-                for line in string.splitlines()
-            ),
-            bullet,
+            iter(split_lines(string)).map(cls.wrapping_line(size)).join(NEW_LINE), bullet
         )
```

### Comparing `changelogging-1.1.0/changelogging/changelogging.toml` & `changelogging-1.2.0/changelogging/changelogging.toml`

 * *Files identical despite different names*

### Comparing `changelogging-1.1.0/changelogging/config.py` & `changelogging-1.2.0/changelogging/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from pathlib import Path
-from typing import Any, Dict, Iterable, Optional, Type, TypeVar, cast, overload
+from typing import Any, Iterable, Optional, Type, TypeVar, cast, overload
 
 import toml
 from attrs import define
-from iters import iter
+from funcs.typing import Unary
+from iters.iters import iter
 from iters.utils import empty
-from versions import Version, parse_version
-from wraps import Option, wrap_optional
+from versions.functions import parse_version
+from versions.version import Version
+from wraps.option import Option, Some
+from wraps.wraps import wrap_optional
 from yarl import URL
 
 from changelogging.constants import (
     DEFAULT_ENCODING,
     DEFAULT_ERRORS,
     DEFAULT_IGNORE_REQUIRED,
     EMPTY,
     ROOT,
 )
 from changelogging.fragments import AnyFragmentTypes, Display, FragmentType
-from changelogging.typing import IntoPath, Unary
+from changelogging.typing import IntoPath, StringDict
+from changelogging.utils import contains_only_item
 
 __all__ = ("Config", "ConfigData", "AnyConfigData")
 
 CHANGELOGGING = "changelogging.toml"
 PYPROJECT = "pyproject.toml"
 
 SEARCH = (CHANGELOGGING, PYPROJECT)
@@ -30,14 +34,16 @@
 
 CONFIG_NOT_FOUND = "can not find config in {}"
 EXPECTED_FILE_OR_DIRECTORY = "expected either a file or a directory"
 
 EXPECTED = "expected `{}`"
 expected = EXPECTED.format
 
+EXPECTED_ONE_CHARACTER_BULLET = "expected one character bullet"
+
 EXPECTED_CHANGELOGGING = expected("changelogging")
 EXPECTED_CHANGELOGGING_NAME = expected("changelogging.name")
 EXPECTED_CHANGELOGGING_VERSION = expected("changelogging.version")
 EXPECTED_CHANGELOGGING_URL = expected("changelogging.url")
 EXPECTED_CHANGELOGGING_DIRECTORY = expected("changelogging.directory")
 EXPECTED_CHANGELOGGING_OUTPUT = expected("changelogging.output")
 EXPECTED_CHANGELOGGING_TITLE_LEVEL = expected("changelogging.title_level")
@@ -64,15 +70,15 @@
 
 T = TypeVar("T")
 
 
 CD = TypeVar("CD", bound="AnyConfigData")
 
 
-class ConfigData(Dict[str, T]):
+class ConfigData(StringDict[T]):
     """Dictionaries that support attribute access."""
 
     def __getattr__(self, name: str) -> Option[T]:
         return wrap_optional(self.get(name))
 
     def copy(self: CD) -> CD:
         return type(self)(self)
@@ -97,14 +103,18 @@
 def mapping_to_type(mapping: ConfigData[str], fragment_type: Type[Any] = FragmentType) -> Any:
     return fragment_type(
         mapping.name.expect(EXPECTED_CHANGELOGGING_TYPES_TYPE_NAME),
         mapping.title.expect(EXPECTED_CHANGELOGGING_TYPES_TYPE_TITLE),
     )
 
 
+def validate_bullet(bullet: str) -> str:
+    return Some(bullet).filter(contains_only_item).expect(EXPECTED_ONE_CHARACTER_BULLET)
+
+
 C = TypeVar("C", bound="Config")
 
 
 @define()
 class Config:
     name: str
     """The name of the project."""
@@ -245,15 +255,15 @@
             # map to `URL` and `Path` to simplify interaction
             url=config.url.map(URL).expect(EXPECTED_CHANGELOGGING_URL),
             directory=config.directory.map_or(default_config.directory, source_path(source)),
             output=config.output.map_or(default_config.output, source_path(source)),
             # merely return defaults if needed
             title_level=config.title_level.unwrap_or(default_config.title_level),
             section_level=config.section_level.unwrap_or(default_config.section_level),
-            bullet=config.bullet.unwrap_or(default_config.bullet),
+            bullet=validate_bullet(config.bullet.unwrap_or(default_config.bullet)),
             wrap=config.wrap.unwrap_or(default_config.wrap),
             wrap_size=config.wrap_size.unwrap_or(default_config.wrap_size),
             start_string=config.start_string.unwrap_or(default_config.start_string),
             title_format=config.title_format.unwrap_or(default_config.title_format),
             issue_format=config.issue_format.unwrap_or(default_config.issue_format),
             fragment_format=config.fragment_format.unwrap_or(default_config.fragment_format),
             # map to `Display` type
@@ -363,15 +373,15 @@
             url=url,
             directory=config.directory.map(source_path(source)).expect(
                 EXPECTED_CHANGELOGGING_DIRECTORY
             ),
             output=config.output.map(source_path(source)).expect(EXPECTED_CHANGELOGGING_OUTPUT),
             title_level=config.title_level.expect(EXPECTED_CHANGELOGGING_TITLE_LEVEL),
             section_level=config.section_level.expect(EXPECTED_CHANGELOGGING_SECTION_LEVEL),
-            bullet=config.bullet.expect(EXPECTED_CHANGELOGGING_BULLET),
+            bullet=validate_bullet(config.bullet.expect(EXPECTED_CHANGELOGGING_BULLET)),
             wrap=config.wrap.expect(EXPECTED_CHANGELOGGING_WRAP),
             wrap_size=config.wrap_size.expect(EXPECTED_CHANGELOGGING_WRAP_SIZE),
             start_string=config.start_string.expect(EXPECTED_CHANGELOGGING_START_STRING),
             title_format=config.title_format.expect(EXPECTED_CHANGELOGGING_TITLE_FORMAT),
             issue_format=config.issue_format.expect(EXPECTED_CHANGELOGGING_ISSUE_FORMAT),
             fragment_format=config.fragment_format.expect(EXPECTED_CHANGELOGGING_FRAGMENT_FORMAT),
             display=config.display.map(Display.from_iterable).expect(
```

### Comparing `changelogging-1.1.0/changelogging/fragments.py` & `changelogging-1.2.0/changelogging/fragments.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Any, Generic, Iterable, Iterator, Type, TypeVar
 
 from attrs import field, frozen
+from funcs.typing import DynamicTuple
+from iters.mappings import merge
 
-from changelogging.typing import DynamicTuple, StringDict
-from changelogging.utils import mapping_merge
+from changelogging.typing import StringDict
 
 __all__ = ("Display", "Fragment", "FragmentType", "FragmentTypes", "AnyFragmentTypes", "Issue")
 
 SUFFIX = ".{}"
 suffix = SUFFIX.format
 
 
@@ -71,15 +72,15 @@
 
         Arguments:
             other: The types to merge with `self`.
 
         Returns:
             The merged [`FragmentTypes`][changelogging.fragments.FragmentTypes] instance.
         """
-        merged = mapping_merge(self.name_to_type, other.name_to_type)
+        merged = merge(self.name_to_type, other.name_to_type)
 
         return self.from_iterable(merged.values())
 
     @property
     def name_to_type(self) -> FragmentTypeDict[FT]:
         """The `name -> type` mapping."""
         return {type.name: type for type in self.types}
```

### Comparing `changelogging-1.1.0/changelogging/git.py` & `changelogging-1.2.0/changelogging/git.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 from pathlib import Path
 from subprocess import call
 from typing import Iterable, Sequence
 
-from changelogging.typing import DynamicTuple
+from funcs.typing import DynamicTuple
+
+from changelogging.constants import DEFAULT_QUIET
+from changelogging.utils import unary_tuple
 
 __all__ = ("remove_command", "remove_paths")
 
 GIT = "git"
 REMOVE = "rm"
-QUIET = "--quiet"
-FORCE = "--force"
+QUIET = "-q"
+FORCE = "-f"
+
+
+def resolve_path(path: Path) -> str:
+    return path.resolve().as_posix()
+
 
+def remove_command(iterable: Iterable[Path], quiet: bool = DEFAULT_QUIET) -> Sequence[str]:
+    command: DynamicTuple[str] = (GIT, REMOVE, FORCE)
 
-def remove_command(iterable: Iterable[Path]) -> Sequence[str]:
-    command: DynamicTuple[str] = (GIT, REMOVE, QUIET, FORCE)
+    if quiet:
+        command += unary_tuple(QUIET)
 
-    command += tuple(path.resolve().as_posix() for path in iterable)
+    command += tuple(map(resolve_path, iterable))
 
     return command
 
 
-def remove_paths(iterable: Iterable[Path]) -> None:
-    call(remove_command(iterable))
+def remove_paths(iterable: Iterable[Path], quiet: bool = DEFAULT_QUIET) -> None:
+    call(remove_command(iterable, quiet=quiet))
```

### Comparing `changelogging-1.1.0/changelogging/main.py` & `changelogging-1.2.0/changelogging/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,73 +1,70 @@
 from pathlib import Path
 from typing import Optional
 
 import click
-from iters import iter
-from pendulum import Date, parse
-from wraps import Option, wrap_optional
+from iters.iters import iter
+from pendulum import Date
+from wraps.option import Option
+from wraps.wraps import wrap_optional
 
 from changelogging import __version__ as version
 from changelogging.build import Builder
 from changelogging.config import Config
-from changelogging.constants import DEFAULT_NAME, HASH, NEW_LINE
+from changelogging.constants import DEFAULT_NAME, DEFAULT_QUIET, HASH, NEW_LINE
 from changelogging.git import remove_paths
-from changelogging.utils import today
+from changelogging.utils import parse_date, right_strip, split_lines, starts_with, today
 
 __all__ = ("changelogging", "build", "create")
 
 
 def get_config(string: Option[str]) -> Config:
     return Config.from_path(string.map_or_else(Path, Path))
 
 
 def get_date(string: Option[str]) -> Date:
     return string.map_or_else(today, parse_date)
 
 
-def parse_date(string: str) -> Date:
-    return parse(string).date()  # type: ignore
-
-
-split_lines = str.splitlines
-right_strip = str.rstrip
-
-
 @click.group(name=DEFAULT_NAME)
-@click.help_option("-h", "--help")
-@click.version_option(version, "-V", "--version")
+@click.help_option("--help", "-h")
+@click.version_option(version, "--version", "-V")
 def changelogging() -> None:
     pass
 
 
 CONFIG_PATH = "config_path"
 DATE_STRING = "date_string"
 
+REMOVING = "removing `{}`"
+removing = REMOVING.format
+
 
 @changelogging.command()
-@click.help_option("-h", "--help")
-@click.option("-c", "--config", CONFIG_PATH, default=None)
-@click.option("-d", "--date", DATE_STRING, default=None)
-@click.option("-D", "--draft", is_flag=True, default=False)
-@click.option("-r/-n", "--remove/--no-remove", default=False)
+@click.help_option("--help", "-h")
+@click.option("--config", "-c", CONFIG_PATH, default=None)
+@click.option("--date", "-d", DATE_STRING, default=None)
+@click.option("--quiet", "-q", is_flag=True, default=DEFAULT_QUIET)
+@click.option("--draft", "-D", is_flag=True, default=False)
+@click.option("--remove/--no-remove", "-r/-n", default=False)
 def build(
-    config_path: Optional[str], date_string: Optional[str], draft: bool, remove: bool
+    config_path: Optional[str], date_string: Optional[str], quiet: bool, draft: bool, remove: bool
 ) -> None:
     date = get_date(wrap_optional(date_string))
 
     config = get_config(wrap_optional(config_path))
 
     builder = Builder(config, date)
 
     if draft:
         click.echo(builder.build())
 
     else:
         if remove:
-            remove_paths(builder.collect_paths())
+            remove_paths(builder.collect_paths(), quiet=quiet)
 
         builder.write()
 
 
 ABORTED = "Creation aborted."
 CREATED = "Created the `{}` fragment."
 PLACEHOLDER = "Add the content here."
@@ -77,40 +74,39 @@
 # Close the file without saving to abort.
 """
 
 NAME = "name"
 
 
 def is_comment(line: str) -> bool:
-    return line.startswith(HASH)
+    return starts_with(line, HASH)
 
 
 def is_content(line: str) -> bool:
     return not is_comment(line)
 
 
-concat_new_line = NEW_LINE.join
-
-
 @changelogging.command()
-@click.help_option("-h", "--help")
-@click.option("-c", "--config", CONFIG_PATH, default=None)
-@click.option("-e/-n", "--edit/--no-edit", default=True)
+@click.help_option("--help", "-h")
+@click.option("--config", "-c", CONFIG_PATH, default=None)
+@click.option("--edit/--no-edit", "-e/-n", default=True)
 @click.argument(NAME)
 def create(config_path: Optional[str], edit: bool, name: str) -> None:
     config = get_config(wrap_optional(config_path))
 
     if edit:
         string = click.edit(EDIT)
 
         if string is None:
             click.echo(ABORTED)
+
             return
 
-        string = iter(split_lines(string)).filter(is_content).map(right_strip).collect(concat_new_line)
+        string = iter(split_lines(string)).filter(is_content).map(right_strip).join(NEW_LINE)
+
     else:
         string = PLACEHOLDER
 
     path = config.directory / name
 
     path.write_text(right_strip(string) + NEW_LINE)
```

### Comparing `changelogging-1.1.0/pyproject.toml` & `changelogging-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "changelogging"
-version = "1.1.0"
+version = "1.2.0"
 description = "Building changelogs from fragments."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/changelogging"
@@ -31,67 +31,76 @@
 
 [tool.poetry.scripts]
 changelogging = "changelogging.main:changelogging"
 
 [tool.poetry.dependencies]
 python = ">= 3.7"
 
-attrs = ">= 22.2.0"
+attrs = ">= 23.1.0"
 click = ">= 8.1.3"
 toml = ">= 0.10.2"
-yarl = ">= 1.8.2"
+yarl = ">= 1.9.2"
 
-typing-extensions = ">= 4.3.0"
+typing-extensions = ">= 4.5.0"
 
 pendulum = ">= 2.1.2"
 
-entrypoint = ">= 1.3.0"
-versions = ">= 1.3.0"
-wraps = ">= 0.3.0"
+entrypoint = ">= 1.4.0"
+versions = ">= 1.4.0"
+funcs = ">= 0.5.1"
+wraps = ">= 0.4.0"
+iters = ">= 0.12.0"
 
 [tool.poetry.group.format]
 optional = true
 
 [tool.poetry.group.format.dependencies]
-black = "22.12.0"
+black = "23.3.0"
+flake8-pyproject = "1.2.3"
 
 [tool.poetry.group.format.dependencies.isort]
-version = "5.11.4"
+version = "5.12.0"
+python = ">= 3.8"
+
+[tool.poetry.group.format.dependencies.flake8]
+version = "6.0.0"
+python = ">= 3.8.1"
 
 [tool.poetry.group.check]
 optional = true
 
 [tool.poetry.group.check.dependencies]
-mypy = "0.991"
+mypy = "1.2.0"
 
-types-toml = "0.10.8.1"
+types-toml = "0.10.8.6"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "7.1.3"
-pytest-cov = "3.0.0"
-
-hypothesis = "6.65.2"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-mkdocs = "1.3.1"
-mkdocs-material = "8.5.3"
+mkdocs = "1.4.3"
+mkdocs-material = "9.1.11"
 
 [tool.poetry.group.docs.dependencies.mkdocstrings]
-version = "0.19.0"
+version = "0.21.2"
 extras = ["python"]
 
 [tool.black]
 line_length = 100
 
+[tool.flake8]
+max_line_length = 100
+
 [tool.isort]
 line_length = 100
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = "--cov changelogging"
 testpaths = ["tests"]
@@ -140,15 +149,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "changelogging"
-version = "1.1.0"
+version = "1.2.0"
 url = "https://github.com/nekitdev/changelogging"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
@@ -157,9 +166,9 @@
 bullet = "-"
 wrap = true
 wrap_size = 100
 
 display = ["security", "feature", "change", "fix", "deprecation", "removal", "internal"]
 
 [build-system]
-requires = ["poetry-core >= 1.4.0"]
+requires = ["poetry-core >= 1.5.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `changelogging-1.1.0/setup.py` & `changelogging-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,148 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: changelogging
+Version: 1.2.0
+Summary: Building changelogs from fragments.
+Home-page: https://github.com/nekitdev/changelogging
+License: MIT
+Keywords: python,changelog,changes
+Author: nekitdev
+Requires-Python: >=3.7
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Classifier: Typing :: Typed
+Requires-Dist: attrs (>=23.1.0)
+Requires-Dist: click (>=8.1.3)
+Requires-Dist: entrypoint (>=1.4.0)
+Requires-Dist: funcs (>=0.5.1)
+Requires-Dist: iters (>=0.12.0)
+Requires-Dist: pendulum (>=2.1.2)
+Requires-Dist: toml (>=0.10.2)
+Requires-Dist: typing-extensions (>=4.5.0)
+Requires-Dist: versions (>=1.4.0)
+Requires-Dist: wraps (>=0.4.0)
+Requires-Dist: yarl (>=1.9.2)
+Project-URL: Documentation, https://nekitdev.github.io/changelogging
+Project-URL: Discord, https://nekit.dev/discord
+Project-URL: Funding, https://patreon.com/nekitdev
+Project-URL: Issues, https://github.com/nekitdev/changelogging/issues
+Project-URL: Repository, https://github.com/nekitdev/changelogging
+Description-Content-Type: text/markdown
 
-packages = \
-['changelogging']
+# `changelogging`
 
-package_data = \
-{'': ['*']}
+[![License][License Badge]][License]
+[![Version][Version Badge]][Package]
+[![Downloads][Downloads Badge]][Package]
+[![Discord][Discord Badge]][Discord]
 
-install_requires = \
-['attrs>=22.2.0',
- 'click>=8.1.3',
- 'entrypoint>=1.3.0',
- 'pendulum>=2.1.2',
- 'toml>=0.10.2',
- 'typing-extensions>=4.3.0',
- 'versions>=1.3.0',
- 'wraps>=0.3.0',
- 'yarl>=1.8.2']
-
-entry_points = \
-{'console_scripts': ['changelogging = changelogging.main:changelogging']}
-
-setup_kwargs = {
-    'name': 'changelogging',
-    'version': '1.1.0',
-    'description': 'Building changelogs from fragments.',
-    'long_description': '# `changelogging`\n\n[![License][License Badge]][License]\n[![Version][Version Badge]][Package]\n[![Downloads][Downloads Badge]][Package]\n[![Discord][Discord Badge]][Discord]\n\n[![Documentation][Documentation Badge]][Documentation]\n[![Check][Check Badge]][Actions]\n[![Test][Test Badge]][Actions]\n[![Coverage][Coverage Badge]][Coverage]\n\n> *Building changelogs from fragments.*\n\n## Installing\n\n**Python 3.7 or above is required.**\n\n### pip\n\nInstalling the library with `pip` is quite simple:\n\n```console\n$ pip install changelogging\n```\n\nAlternatively, the library can be installed from source:\n\n```console\n$ git clone https://github.com/nekitdev/changelogging.git\n$ cd changelogging\n$ python -m pip install .\n```\n\n### poetry\n\nYou can add `changelogging` as a dependency with the following command:\n\n```console\n$ poetry add changelogging\n```\n\nOr by directly specifying it in the configuration like so:\n\n```toml\n[tool.poetry.dependencies]\nchangelogging = "^1.1.0"\n```\n\nAlternatively, you can add it directly from the source:\n\n```toml\n[tool.poetry.dependencies.changelogging]\ngit = "https://github.com/nekitdev/changelogging.git"\n```\n\n## Documentation\n\nYou can find the documentation [here][Documentation].\n\n## Support\n\nIf you need support with the library, you can send an [email][Email]\nor refer to the official [Discord server][Discord].\n\n## Changelog\n\nYou can find the changelog [here][Changelog].\n\n## Security Policy\n\nYou can find the Security Policy of `changelogging` [here][Security].\n\n## Contributing\n\nIf you are interested in contributing to `changelogging`, make sure to take a look at the\n[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].\n\n## License\n\n`changelogging` is licensed under the MIT License terms. See [License][License] for details.\n\n[Email]: mailto:support@nekit.dev\n\n[Discord]: https://nekit.dev/discord\n\n[Actions]: https://github.com/nekitdev/changelogging/actions\n\n[Changelog]: https://github.com/nekitdev/changelogging/blob/main/CHANGELOG.md\n[Code of Conduct]: https://github.com/nekitdev/changelogging/blob/main/CODE_OF_CONDUCT.md\n[Contributing Guide]: https://github.com/nekitdev/changelogging/blob/main/CONTRIBUTING.md\n[Security]: https://github.com/nekitdev/changelogging/blob/main/SECURITY.md\n\n[License]: https://github.com/nekitdev/changelogging/blob/main/LICENSE\n\n[Package]: https://pypi.org/project/changelogging\n[Coverage]: https://codecov.io/gh/nekitdev/changelogging\n[Documentation]: https://nekitdev.github.io/changelogging\n\n[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2\n[License Badge]: https://img.shields.io/pypi/l/changelogging\n[Version Badge]: https://img.shields.io/pypi/v/changelogging\n[Downloads Badge]: https://img.shields.io/pypi/dm/changelogging\n\n[Documentation Badge]: https://github.com/nekitdev/changelogging/workflows/docs/badge.svg\n[Check Badge]: https://github.com/nekitdev/changelogging/workflows/check/badge.svg\n[Test Badge]: https://github.com/nekitdev/changelogging/workflows/test/badge.svg\n[Coverage Badge]: https://codecov.io/gh/nekitdev/changelogging/branch/main/graph/badge.svg\n',
-    'author': 'nekitdev',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/nekitdev/changelogging',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7',
-}
+[![Documentation][Documentation Badge]][Documentation]
+[![Check][Check Badge]][Actions]
+[![Test][Test Badge]][Actions]
+[![Coverage][Coverage Badge]][Coverage]
 
+> *Building changelogs from fragments.*
+
+## Installing
+
+**Python 3.7 or above is required.**
+
+### pip
+
+Installing the library with `pip` is quite simple:
+
+```console
+$ pip install changelogging
+```
+
+Alternatively, the library can be installed from source:
+
+```console
+$ git clone https://github.com/nekitdev/changelogging.git
+$ cd changelogging
+$ python -m pip install .
+```
+
+### poetry
+
+You can add `changelogging` as a dependency with the following command:
+
+```console
+$ poetry add changelogging
+```
+
+Or by directly specifying it in the configuration like so:
+
+```toml
+[tool.poetry.dependencies]
+changelogging = "^1.2.0"
+```
+
+Alternatively, you can add it directly from the source:
+
+```toml
+[tool.poetry.dependencies.changelogging]
+git = "https://github.com/nekitdev/changelogging.git"
+```
+
+## Documentation
+
+You can find the documentation [here][Documentation].
+
+## Support
+
+If you need support with the library, you can send an [email][Email]
+or refer to the official [Discord server][Discord].
+
+## Changelog
+
+You can find the changelog [here][Changelog].
+
+## Security Policy
+
+You can find the Security Policy of `changelogging` [here][Security].
+
+## Contributing
+
+If you are interested in contributing to `changelogging`, make sure to take a look at the
+[Contributing Guide][Contributing Guide], as well as the [Code of Conduct][Code of Conduct].
+
+## License
+
+`changelogging` is licensed under the MIT License terms. See [License][License] for details.
+
+[Email]: mailto:support@nekit.dev
+
+[Discord]: https://nekit.dev/discord
+
+[Actions]: https://github.com/nekitdev/changelogging/actions
+
+[Changelog]: https://github.com/nekitdev/changelogging/blob/main/CHANGELOG.md
+[Code of Conduct]: https://github.com/nekitdev/changelogging/blob/main/CODE_OF_CONDUCT.md
+[Contributing Guide]: https://github.com/nekitdev/changelogging/blob/main/CONTRIBUTING.md
+[Security]: https://github.com/nekitdev/changelogging/blob/main/SECURITY.md
+
+[License]: https://github.com/nekitdev/changelogging/blob/main/LICENSE
+
+[Package]: https://pypi.org/project/changelogging
+[Coverage]: https://codecov.io/gh/nekitdev/changelogging
+[Documentation]: https://nekitdev.github.io/changelogging
+
+[Discord Badge]: https://img.shields.io/badge/chat-discord-5865f2
+[License Badge]: https://img.shields.io/pypi/l/changelogging
+[Version Badge]: https://img.shields.io/pypi/v/changelogging
+[Downloads Badge]: https://img.shields.io/pypi/dm/changelogging
+
+[Documentation Badge]: https://github.com/nekitdev/changelogging/workflows/docs/badge.svg
+[Check Badge]: https://github.com/nekitdev/changelogging/workflows/check/badge.svg
+[Test Badge]: https://github.com/nekitdev/changelogging/workflows/test/badge.svg
+[Coverage Badge]: https://codecov.io/gh/nekitdev/changelogging/branch/main/graph/badge.svg
 
-setup(**setup_kwargs)
```

