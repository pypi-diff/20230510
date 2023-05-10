# Comparing `tmp/git-changelog-1.0.0.tar.gz` & `tmp/git_changelog-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-changelog-1.0.0.tar", last modified: Sat Feb  4 19:36:46 2023, max compression
+gzip compressed data, was "git_changelog-1.0.1.tar", last modified: Wed May 10 15:56:33 2023, max compression
```

## Comparing `git-changelog-1.0.0.tar` & `git_changelog-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0 pawamoy   (1000) users      (985)      754 2023-02-03 19:06:33.851332 git-changelog-1.0.0/LICENSE
--rw-r--r--   0 pawamoy   (1000) users      (985)     7863 2023-02-04 15:13:02.831902 git-changelog-1.0.0/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)     3327 2023-02-03 19:06:33.851332 git-changelog-1.0.0/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) users      (985)      271 2023-02-03 19:06:33.851332 git-changelog-1.0.0/src/git_changelog/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      388 2023-02-03 19:06:33.851332 git-changelog-1.0.0/src/git_changelog/__main__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    14787 2023-02-04 15:04:45.847501 git-changelog-1.0.0/src/git_changelog/build.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    12699 2023-02-04 15:18:37.815429 git-changelog-1.0.0/src/git_changelog/cli.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    13510 2023-02-04 13:48:51.359388 git-changelog-1.0.0/src/git_changelog/commit.py
--rw-r--r--   0 pawamoy   (1000) users      (985)    11228 2023-01-29 23:15:36.980770 git-changelog-1.0.0/src/git_changelog/providers.py
--rw-r--r--   0 pawamoy   (1000) users      (985)        0 2023-02-03 19:06:33.554669 git-changelog-1.0.0/src/git_changelog/py.typed
--rw-r--r--   0 pawamoy   (1000) users      (985)     1122 2023-02-03 19:05:40.815432 git-changelog-1.0.0/src/git_changelog/templates/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     1588 2023-02-04 13:50:13.931438 git-changelog-1.0.0/src/git_changelog/templates/angular.md.jinja
--rw-r--r--   0 pawamoy   (1000) users      (985)     2213 2023-02-04 13:49:16.982323 git-changelog-1.0.0/src/git_changelog/templates/keepachangelog.md.jinja
--rw-r--r--   0 pawamoy   (1000) users      (985)       37 2021-11-14 15:27:29.516885 git-changelog-1.0.0/tests/.pytest_cache/.gitignore
--rw-r--r--   0 pawamoy   (1000) users      (985)      194 2021-11-14 15:27:29.516885 git-changelog-1.0.0/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0 pawamoy   (1000) users      (985)      295 2021-11-14 15:27:29.516885 git-changelog-1.0.0/tests/.pytest_cache/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)        2 2021-11-14 15:32:24.789513 git-changelog-1.0.0/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0 pawamoy   (1000) users      (985)        2 2021-11-14 15:32:24.789513 git-changelog-1.0.0/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0 pawamoy   (1000) users      (985)       10 2021-11-14 15:32:24.236192 git-changelog-1.0.0/tests/.pytest_cache/v/randomly_seed
--rw-r--r--   0 pawamoy   (1000) users      (985)      166 2023-02-03 19:06:33.544669 git-changelog-1.0.0/tests/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       47 2023-02-03 19:06:33.541336 git-changelog-1.0.0/tests/conftest.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2149 2023-02-04 15:05:50.089572 git-changelog-1.0.0/tests/test_angular_style.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2096 2023-02-04 15:06:04.165963 git-changelog-1.0.0/tests/test_basic_style.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      980 2023-02-04 15:19:43.215128 git-changelog-1.0.0/tests/test_cli.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      979 2023-01-29 23:15:37.004104 git-changelog-1.0.0/tests/test_commit.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     5127 2023-02-04 15:06:19.022339 git-changelog-1.0.0/tests/test_conventional_commit_style.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     4153 2023-02-04 15:06:29.782128 git-changelog-1.0.0/tests/test_end_to_end.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     1191 2023-02-03 19:05:40.818765 git-changelog-1.0.0/tests/test_providers.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2207 2023-02-03 19:05:40.818765 git-changelog-1.0.0/tests/test_version.py
--rw-------   0 pawamoy   (1000) users      (985)     9410 2023-02-04 19:36:46.788724 git-changelog-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-05-10 15:37:31.957872 git_changelog-1.0.1/LICENSE
+-rw-r--r--   0        0        0     7863 2023-05-10 15:37:31.957872 git_changelog-1.0.1/README.md
+-rw-r--r--   0        0        0     2697 2023-05-10 15:56:33.713125 git_changelog-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      254 2023-05-10 15:37:31.957872 git_changelog-1.0.1/src/git_changelog/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-10 15:37:31.957872 git_changelog-1.0.1/src/git_changelog/__main__.py
+-rw-r--r--   0        0        0    14779 2023-05-10 15:20:51.179724 git_changelog-1.0.1/src/git_changelog/build.py
+-rw-r--r--   0        0        0    13174 2023-05-10 15:51:30.408729 git_changelog-1.0.1/src/git_changelog/cli.py
+-rw-r--r--   0        0        0    13748 2023-05-10 15:20:51.179724 git_changelog-1.0.1/src/git_changelog/commit.py
+-rw-r--r--   0        0        0    11212 2023-05-10 15:20:51.179724 git_changelog-1.0.1/src/git_changelog/providers.py
+-rw-r--r--   0        0        0        0 2023-05-10 15:37:29.431312 git_changelog-1.0.1/src/git_changelog/py.typed
+-rw-r--r--   0        0        0     1122 2023-02-03 19:05:40.815432 git_changelog-1.0.1/src/git_changelog/templates/__init__.py
+-rw-r--r--   0        0        0     1588 2023-02-04 13:50:13.931438 git_changelog-1.0.1/src/git_changelog/templates/angular.md.jinja
+-rw-r--r--   0        0        0     2213 2023-02-04 13:49:16.982323 git_changelog-1.0.1/src/git_changelog/templates/keepachangelog.md.jinja
+-rw-r--r--   0        0        0       37 2021-11-14 15:27:29.516885 git_changelog-1.0.1/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      194 2021-11-14 15:27:29.516885 git_changelog-1.0.1/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      295 2021-11-14 15:27:29.516885 git_changelog-1.0.1/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2021-11-14 15:32:24.789513 git_changelog-1.0.1/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2021-11-14 15:32:24.789513 git_changelog-1.0.1/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       10 2021-11-14 15:32:24.236192 git_changelog-1.0.1/tests/.pytest_cache/v/randomly_seed
+-rw-r--r--   0        0        0      166 2023-05-10 15:37:29.424645 git_changelog-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-10 15:37:29.421312 git_changelog-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0     2361 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_angular_style.py
+-rw-r--r--   0        0        0     2308 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_basic_style.py
+-rw-r--r--   0        0        0     1172 2023-05-10 15:37:31.957872 git_changelog-1.0.1/tests/test_cli.py
+-rw-r--r--   0        0        0     1079 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_commit.py
+-rw-r--r--   0        0        0     5483 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_conventional_commit_style.py
+-rw-r--r--   0        0        0     6039 2023-05-10 15:52:36.028834 git_changelog-1.0.1/tests/test_end_to_end.py
+-rw-r--r--   0        0        0     1207 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_providers.py
+-rw-r--r--   0        0        0     2297 2023-05-10 15:20:51.179724 git_changelog-1.0.1/tests/test_version.py
+-rw-r--r--   0        0        0     9526 1970-01-01 00:00:00.000000 git_changelog-1.0.1/PKG-INFO
```

### Comparing `git-changelog-1.0.0/LICENSE` & `git_changelog-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-changelog-1.0.0/README.md` & `git_changelog-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `git-changelog-1.0.0/pyproject.toml` & `git_changelog-1.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 name = "git-changelog"
 description = "Automatic Changelog generator using Jinja2 templates."
 authors = [
     { name = "Timothée Mazzucotelli", email = "pawamoy@pm.me" },
 ]
-license = "ISC"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
     "git",
     "changelog",
     "changelog-generator",
     "commit-style",
@@ -39,98 +38,78 @@
     "Typing :: Typed",
 ]
 dependencies = [
     "Jinja2>=2.10,<4",
     "semver~=2.13",
     "importlib-metadata; python_version < '3.8'",
 ]
-version = "1.0.0"
+version = "1.0.1"
+
+[project.license]
+text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/git-changelog"
 Documentation = "https://pawamoy.github.io/git-changelog"
 Changelog = "https://pawamoy.github.io/git-changelog/changelog"
 Repository = "https://github.com/pawamoy/git-changelog"
 Issues = "https://github.com/pawamoy/git-changelog/issues"
 Discussions = "https://github.com/pawamoy/git-changelog/discussions"
 Gitter = "https://gitter.im/git-changelog/community"
 Funding = "https://github.com/sponsors/pawamoy"
 
 [project.scripts]
 git-changelog = "git_changelog.cli:main"
 
-[project.optional-dependencies]
+[tool.pdm]
+plugins = [
+    "pdm-multirun",
+]
 
 [tool.pdm.version]
 source = "scm"
 
 [tool.pdm.build]
 package-dir = "src"
 editable-backend = "editables"
 
 [tool.pdm.dev-dependencies]
 duty = [
-    "duty>=0.7",
+    "duty>=0.10",
 ]
 docs = [
+    "black>=23.1",
+    "markdown-callouts>=0.2",
+    "markdown-exec>=0.5",
     "mkdocs>=1.3",
     "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
+    "mkdocs-git-committers-plugin-2>=1.1",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
-    "mkdocs-section-index>=0.3",
+    "mkdocs-minify-plugin>=0.6.4",
     "mkdocstrings[python]>=0.18",
-    "markdown-callouts>=0.2",
-    "markdown-exec>=0.5",
     "toml>=0.10",
 ]
-format = [
-    "autoflake>=1.4",
-    "black>=21.10b0",
-    "isort>=5.10",
+maintain = [
+    "black>=23.1",
+    "blacken-docs>=1.13",
 ]
 quality = [
-    "importlib-metadata<5; python_version < '3.8'",
-    "flake8>=4; python_version >= '3.8'",
-    "darglint>=1.8",
-    "flake8-bandit>=2.1",
-    "flake8-black>=0.2",
-    "flake8-bugbear>=21.9",
-    "flake8-builtins>=1.5",
-    "flake8-comprehensions>=3.7",
-    "flake8-docstrings>=1.6",
-    "flake8-pytest-style>=1.5",
-    "flake8-string-format>=0.3",
-    "flake8-tidy-imports>=4.5",
-    "flake8-variables-names>=0.0",
-    "pep8-naming>=0.12",
-    "wps-light>=0.15",
+    "ruff>=0.0.246",
 ]
 tests = [
     "pytest>=6.2",
     "pytest-cov>=3.0",
     "pytest-randomly>=3.10",
     "pytest-xdist>=2.4",
 ]
 typing = [
     "mypy>=0.910",
     "types-markdown>=3.3",
+    "types-pyyaml>=6.0",
     "types-toml>=0.10",
     "types-setuptools>=65.5.0.2",
 ]
 security = [
     "safety>=2",
 ]
-
-[tool.black]
-line-length = 120
-exclude = "tests/fixtures"
-
-[tool.isort]
-line_length = 120
-not_skip = "__init__.py"
-multi_line_output = 3
-force_single_line = false
-balanced_wrapping = true
-default_section = "THIRDPARTY"
-known_first_party = "git_changelog"
-include_trailing_comma = true
```

### Comparing `git-changelog-1.0.0/src/git_changelog/build.py` & `git_changelog-1.0.1/src/git_changelog/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 
 from __future__ import annotations
 
 import datetime
 import os
 import sys
 from contextlib import suppress
-from pathlib import Path
-from subprocess import check_output  # noqa: S404 (we trust the commands we run)
-from typing import Type, Union
+from subprocess import check_output  # (we trust the commands we run)
+from typing import TYPE_CHECKING, Type, Union
 
 from semver import VersionInfo
 
 from git_changelog.commit import (
     AngularConvention,
     AtomConvention,
     BasicConvention,
     Commit,
     CommitConvention,
     ConventionalCommitConvention,
 )
 from git_changelog.providers import GitHub, GitLab, ProviderRefParser
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 ConventionType = Union[str, CommitConvention, Type[CommitConvention]]
 
 
-def bump(version: str, part: str = "patch") -> str:  # noqa: WPS231
-    """
-    Bump a version.
+def bump(version: str, part: str = "patch") -> str:
+    """Bump a version.
 
     Arguments:
         version: The version to bump.
         part: The part of the version to bump (major, minor, or patch).
 
     Returns:
         The bumped version.
@@ -51,16 +52,15 @@
     return prefix + str(semver_version)
 
 
 class Section:
     """A list of commits grouped by section_type."""
 
     def __init__(self, section_type: str = "", commits: list[Commit] | None = None):
-        """
-        Initialization method.
+        """Initialization method.
 
         Arguments:
             section_type: The section section_type.
             commits: The list of commits.
         """
         self.type: str = section_type
         self.commits: list[Commit] = commits or []
@@ -74,16 +74,15 @@
         tag: str = "",
         date: datetime.date | None = None,
         sections: list[Section] | None = None,
         commits: list[Commit] | None = None,
         url: str = "",
         compare_url: str = "",
     ):
-        """
-        Initialization method.
+        """Initialization method.
 
         Arguments:
             tag: The version tag.
             date: The version date.
             sections: The version sections.
             commits: The version commits.
             url: The version URL.
@@ -139,44 +138,44 @@
 
 
 class Changelog:
     """The main changelog class."""
 
     MARKER: str = "--GIT-CHANGELOG MARKER--"
     FORMAT: str = (
-        r"%H%n"  # commit commit_hash  # noqa: WPS323
+        r"%H%n"  # commit commit_hash
         r"%an%n"  # author name
         r"%ae%n"  # author email
         r"%ad%n"  # author date
         r"%cn%n"  # committer name
         r"%ce%n"  # committer email
         r"%cd%n"  # committer date
         r"%D%n"  # tag
         r"%s%n"  # subject
         r"%b%n" + MARKER  # body
     )
-    CONVENTION: dict[str, Type[CommitConvention]] = {
+    CONVENTION: dict[str, type[CommitConvention]] = {
         "basic": BasicConvention,
         "angular": AngularConvention,
         "atom": AtomConvention,
         "conventional": ConventionalCommitConvention,
     }
 
-    def __init__(  # noqa: WPS231
+    def __init__(
         self,
         repository: str | Path,
+        *,
         provider: ProviderRefParser | None = None,
         convention: ConventionType | None = None,
         parse_provider_refs: bool = False,
         parse_trailers: bool = False,
         sections: list[str] | None = None,
         bump_latest: bool = False,
     ):
-        """
-        Initialization method.
+        """Initialization method.
 
         Arguments:
             repository: The repository (directory) for which to build the changelog.
             provider: The provider to use (github.com, gitlab.com, etc.).
             convention: The commit convention to use (angular, atom, etc.).
             parse_provider_refs: Whether to parse provider-specific references in the commit messages.
             parse_trailers: Whether to parse Git trailers in the commit messages.
@@ -201,30 +200,29 @@
         self.provider = provider
 
         # set convention
         if isinstance(convention, str):
             try:
                 convention = self.CONVENTION[convention]()
             except KeyError:
-                print(
+                print(  # noqa: T201
                     f"git-changelog: no such convention available: {convention}, using default convention",
                     file=sys.stderr,
                 )
                 convention = BasicConvention()
         elif convention is None:
             convention = BasicConvention()
         elif not isinstance(convention, CommitConvention) and issubclass(convention, CommitConvention):
             convention = convention()
         self.convention: CommitConvention = convention
 
         # set sections
-        if sections:
-            sections = [self.convention.TYPES[section] for section in sections]
-        else:
-            sections = self.convention.DEFAULT_RENDER
+        sections = (
+            [self.convention.TYPES[section] for section in sections] if sections else self.convention.DEFAULT_RENDER
+        )
         self.sections = sections
 
         # get git log and parse it into list of commits
         self.raw_log: str = self.get_log()
         self.commits: list[Commit] = self.parse_commits()
 
         # apply dates to commits and group them by version
@@ -247,15 +245,15 @@
             *args: Arguments passed to the git command.
 
         Returns:
             The git command output.
         """
         return check_output(["git", *args], cwd=self.repository).decode("utf8")  # noqa: S603,S607
 
-    def get_remote_url(self) -> str:  # noqa: WPS615
+    def get_remote_url(self) -> str:
         """Get the git remote URL for the repository.
 
         Returns:
             The origin remote URL.
         """
         remote = "remote." + os.environ.get("GIT_CHANGELOG_REMOTE", "origin") + ".url"
         git_url = self.run_git("config", "--get", remote).rstrip("\n")
@@ -306,41 +304,42 @@
                 parse_trailers=self.parse_trailers,
             )
 
             pos += nbl_index + 1
 
             # expand commit object with provider parsing
             if self.provider:
-                commit.update_with_provider(self.provider, self.parse_provider_refs)
+                commit.update_with_provider(self.provider, parse_refs=self.parse_provider_refs)
 
             # set the commit url based on remote_url (could be wrong)
             elif self.remote_url:
                 commit.url = self.remote_url + "/commit/" + commit.hash
 
             # expand commit object with convention parsing
             if self.convention:
                 commit.update_with_convention(self.convention)
 
             commits.append(commit)
 
         return commits
 
     def _apply_versions_to_commits(self) -> dict[str, datetime.date]:
-        versions_dates = {"": datetime.date.today()}
+        versions_dates = {"": datetime.date.today()}  # noqa: DTZ011
         version = None
         for commit in self.commits:
             if commit.version:
                 version = commit.version
                 versions_dates[version] = commit.committer_date.date()
             elif version:
                 commit.version = version
         return versions_dates
 
-    def _group_commits_by_version(  # noqa: WPS231
-        self, dates: dict[str, datetime.date]
+    def _group_commits_by_version(
+        self,
+        dates: dict[str, datetime.date],
     ) -> tuple[list[Version], dict[str, Version]]:
         versions_list = []
         versions_dict = {}
         versions_types_dict: dict[str, dict[str, Section]] = {}
         next_version = None
         for commit in self.commits:
             if commit.version not in versions_dict:
@@ -349,57 +348,60 @@
                 if self.provider:
                     version.url = self.provider.get_tag_url(tag=commit.version)
                 if next_version:
                     version.next_version = next_version
                     next_version.previous_version = version
                     if self.provider:
                         next_version.compare_url = self.provider.get_compare_url(
-                            base=version.tag, target=next_version.tag or "HEAD"
+                            base=version.tag,
+                            target=next_version.tag or "HEAD",
                         )
                 next_version = version
                 versions_list.append(version)
                 versions_types_dict[commit.version] = {}
             versions_dict[commit.version].commits.append(commit)
             if "type" in commit.convention and commit.convention["type"] not in versions_types_dict[commit.version]:
                 section = Section(section_type=commit.convention["type"])
                 versions_types_dict[commit.version][commit.convention["type"]] = section
                 versions_dict[commit.version].sections_list.append(section)
                 versions_dict[commit.version].sections_dict = versions_types_dict[commit.version]
             versions_types_dict[commit.version][commit.convention["type"]].commits.append(commit)
         if next_version is not None and self.provider:
             next_version.compare_url = self.provider.get_compare_url(
-                base=versions_list[-1].commits[-1].hash, target=next_version.tag or "HEAD"
+                base=versions_list[-1].commits[-1].hash,
+                target=next_version.tag or "HEAD",
             )
         return versions_list, versions_dict
 
-    def _bump_latest(self) -> None:  # noqa: WPS231
+    def _bump_latest(self) -> None:
         # guess the next version number based on last version and recent commits
         last_version = self.versions_list[0]
         if not last_version.tag and last_version.previous_version:
             last_tag = last_version.previous_version.tag
-            major = minor = False  # noqa: WPS429
+            major = minor = False
             for commit in last_version.commits:
                 if commit.convention["is_major"]:
                     major = True
                     break
-                elif commit.convention["is_minor"]:
+                if commit.convention["is_minor"]:
                     minor = True
             # never fail on non-semver versions
             with suppress(ValueError):
                 if major:
                     planned_tag = bump(last_tag, "major")
                 elif minor:
                     planned_tag = bump(last_tag, "minor")
                 else:
                     planned_tag = bump(last_tag, "patch")
                 last_version.planned_tag = planned_tag
                 if self.provider:
                     last_version.url = self.provider.get_tag_url(tag=planned_tag)
                     last_version.compare_url = self.provider.get_compare_url(
-                        base=last_version.previous_version.tag, target=last_version.planned_tag
+                        base=last_version.previous_version.tag,
+                        target=last_version.planned_tag,
                     )
 
     def _fix_single_version(self) -> None:
         last_version = self.versions_list[0]
         if len(self.versions_list) == 1 and last_version.planned_tag is None:
             planned_tag = "0.1.0"
             last_version.tag = planned_tag
```

### Comparing `git-changelog-1.0.0/src/git_changelog/cli.py` & `git_changelog-1.0.1/src/git_changelog/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,49 @@
+"""Module that contains the command line application."""
+
 # Why does this file exist, and why not put this in `__main__`?
 #
 # You might be tempted to import things from `__main__` later,
 # but that will cause problems: the code will get executed twice:
 #
 # - When you run `python -m git_changelog` python will execute
 #   `__main__.py` as a script. That means there won't be any
 #   `git_changelog.__main__` in `sys.modules`.
 # - When you import `__main__` it will get executed again (as a module) because
 #   there's no `git_changelog.__main__` in `sys.modules`.
 
-"""Module that contains the command line application."""
-
 from __future__ import annotations
 
 import argparse
 import re
 import sys
 from typing import Pattern, TextIO
 
 from jinja2.exceptions import TemplateNotFound
 
 from git_changelog import templates
 from git_changelog.build import Changelog, Version
-from git_changelog.commit import AngularConvention, BasicConvention, CommitConvention, ConventionalCommitConvention
+from git_changelog.commit import (
+    AngularConvention,
+    BasicConvention,
+    CommitConvention,
+    ConventionalCommitConvention,
+)
 
 if sys.version_info < (3, 8):
     import importlib_metadata as metadata
 else:
-    from importlib import metadata  # noqa: WPS440
+    from importlib import metadata
 
-DEFAULT_VERSION_REGEX = r"^## \[v?(?P<version>[^\]]+)"
+DEFAULT_VERSION_REGEX = r"^## \[(?P<version>v?[^\]]+)"
 DEFAULT_MARKER_LINE = "<!-- insertion marker -->"
 CONVENTIONS = ("angular", "atom", "conventional", "basic")
 
 
-class Templates(tuple):  # noqa: WPS600 (subclassing tuple)
+class Templates(tuple):  # (subclassing tuple)
     """Helper to pick a template on the command line."""
 
     def __contains__(self, item: object) -> bool:
         if isinstance(item, str):
             return item.startswith("path:") or super().__contains__(item)
         return False
 
@@ -82,35 +87,43 @@
             Each version contains a set of commits, and will be an entry
             in your changelog. Commits in each version will be grouped
             by sections, depending on the commit convention you follow.
 
             {BasicConvention._format_sections_help()}
             {AngularConvention._format_sections_help()}
             {ConventionalCommitConvention._format_sections_help()}
-            """,  # noqa: WPS437
+            """,
         ),
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
 
     parser.add_argument(
-        "repository", metavar="REPOSITORY", nargs="?", default=".", help="The repository path, relative or absolute."
+        "repository",
+        metavar="REPOSITORY",
+        nargs="?",
+        default=".",
+        help="The repository path, relative or absolute.",
     )
 
     parser.add_argument(
         "-b",
         "--bump-latest",
         action="store_true",
         dest="bump_latest",
         default=False,
         help="Guess the new latest version by bumping the previous one based on the set of unreleased commits. "
         "For example, if a commit contains breaking changes, bump the major number (or the minor number for 0.x versions). "
         "Else if there are new features, bump the minor number. Else just bump the patch number.",
     )
     parser.add_argument(
-        "-h", "--help", action="help", default=argparse.SUPPRESS, help="Show this help message and exit."
+        "-h",
+        "--help",
+        action="help",
+        default=argparse.SUPPRESS,
+        help="Show this help message and exit.",
     )
     parser.add_argument(
         "-i",
         "--in-place",
         action="store_true",
         dest="in_place",
         default=False,
@@ -199,29 +212,29 @@
         dest="parse_trailers",
         help="Parse Git trailers in the commit message. See https://git-scm.com/docs/git-interpret-trailers.",
     )
     parser.add_argument(
         "-v",
         "--version",
         action="version",
-        version="%(prog)s " + get_version(),  # noqa: WPS323 (%)
+        version="%(prog)s " + get_version(),  # (%)
         help="Show the current version of the program and exit.",
     )
     return parser
 
 
 def _latest(lines: list[str], regex: Pattern) -> str | None:
     for line in lines:
         match = regex.search(line)
         if match:
             return match.groupdict()["version"]
     return None
 
 
-def _unreleased(versions: list[Version], last_release: str):
+def _unreleased(versions: list[Version], last_release: str) -> list[Version]:
     for index, version in enumerate(versions):
         if version.tag == last_release:
             return versions[:index]
     return versions
 
 
 def main(args: list[str] | None = None) -> int:
@@ -255,26 +268,26 @@
     except ValueError as error:
         print(f"git-changelog: {error}", file=sys.stderr)
         return 1
 
     return 0
 
 
-def build_and_render(  # noqa: WPS231
+def build_and_render(
     repository: str,
     template: str,
     convention: str | CommitConvention,
-    parse_refs: bool = False,
-    parse_trailers: bool = False,
+    parse_refs: bool = False,  # noqa: FBT001,FBT002
+    parse_trailers: bool = False,  # noqa: FBT001,FBT002
     sections: list[str] | None = None,
-    in_place: bool = False,
+    in_place: bool = False,  # noqa: FBT001,FBT002
     output: str | TextIO | None = None,
     version_regex: str = DEFAULT_VERSION_REGEX,
     marker_line: str = DEFAULT_MARKER_LINE,
-    bump_latest: bool = False,
+    bump_latest: bool = False,  # noqa: FBT001,FBT002
 ) -> tuple[Changelog, str]:
     """Build a changelog and render it.
 
     This function returns the changelog instance and the rendered contents,
     but also updates the specified output file (side-effect) or writes to stdout.
 
     Parameters:
@@ -297,16 +310,16 @@
         The built changelog and the rendered contents.
     """
     # get template
     if template.startswith("path:"):
         path = template.replace("path:", "", 1)
         try:
             jinja_template = templates.get_custom_template(path)
-        except TemplateNotFound:
-            raise ValueError(f"No such file: {path}")
+        except TemplateNotFound as error:
+            raise ValueError(f"No such file: {path}") from error
     else:
         jinja_template = templates.get_template(template)
 
     if output is None:
         output = sys.stdout
 
     # handle misconfiguration early
@@ -322,43 +335,52 @@
         sections=sections,
         bump_latest=bump_latest,
     )
 
     # render new entries in-place
     if in_place:
         # read current changelog lines
-        with open(output, "r") as changelog_file:  # type: ignore[arg-type]
+        with open(output) as changelog_file:  # type: ignore[arg-type]
             lines = changelog_file.read().splitlines()
 
         # prepare version regex and marker line
         if template in {"angular", "keepachangelog"}:
             version_regex = DEFAULT_VERSION_REGEX
             marker_line = DEFAULT_MARKER_LINE
 
         # only keep new entries (missing from changelog)
         last_released = _latest(lines, re.compile(version_regex))
         if last_released:
-            changelog.versions_list = _unreleased(changelog.versions_list, last_released)
+            # check if the latest version is already in the changelog
+            if (
+                last_released == changelog.versions_list[0].tag
+                or last_released == changelog.versions_list[0].planned_tag
+            ):
+                raise ValueError(f"Version {last_released} already in changelog")
+            changelog.versions_list = _unreleased(
+                changelog.versions_list,
+                last_released,
+            )
 
         # render new entries
         rendered = jinja_template.render(changelog=changelog, in_place=True).rstrip("\n") + "\n"
 
         # find marker line(s) in current changelog
         marker = lines.index(marker_line)
         try:
             marker2 = lines[marker + 1 :].index(marker_line)
         except ValueError:
             # apply new entries at marker line
             lines[marker] = rendered
         else:
             # apply new entries between marker lines
-            lines[marker : marker + marker2 + 2] = [rendered]  # noqa: WPS362
+            lines[marker : marker + marker2 + 2] = [rendered]
 
         # write back updated changelog lines
-        with open(output, "w") as changelog_file:  # type: ignore[arg-type]  # noqa: WPS440
+        with open(output, "w") as changelog_file:  # type: ignore[arg-type]
             changelog_file.write("\n".join(lines).rstrip("\n") + "\n")
 
     # overwrite output file
     else:
         rendered = jinja_template.render(changelog=changelog)
 
         # write result in specified output
```

### Comparing `git-changelog-1.0.0/src/git_changelog/commit.py` & `git_changelog-1.0.1/src/git_changelog/commit.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,47 +3,48 @@
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from contextlib import suppress
 from datetime import datetime
-from typing import Any, Pattern
+from typing import TYPE_CHECKING, Any, Pattern
 
-from git_changelog.providers import ProviderRefParser, Ref
+if TYPE_CHECKING:
+    from git_changelog.providers import ProviderRefParser, Ref
 
 
-def _clean_body(lines: list[str]):
+def _clean_body(lines: list[str]) -> list[str]:
     while lines and not lines[0].strip():
         lines.pop(0)
     while lines and not lines[-1].strip():
         lines.pop()
     return lines
 
 
 class Commit:
     """A class to represent a commit."""
 
-    def __init__(  # noqa: WPS231
+    def __init__(
         self,
         commit_hash: str,
         author_name: str = "",
         author_email: str = "",
         author_date: str | datetime = "",
         committer_name: str = "",
         committer_email: str = "",
         committer_date: str | datetime = "",
         refs: str = "",
         subject: str = "",
         body: list[str] | None = None,
         url: str = "",
+        *,
         parse_trailers: bool = False,
     ):
-        """
-        Initialization method.
+        """Initialization method.
 
         Arguments:
             commit_hash: The commit hash.
             author_name: The author name.
             author_email: The author email.
             author_date: The authoring date (datetime or UTC timestamp).
             committer_name: The committer name.
@@ -52,36 +53,36 @@
             refs: The commit refs.
             subject: The commit message subject.
             body: The commit message body.
             url: The commit URL.
             parse_trailers: Whether to parse Git trailers.
         """
         if not author_date:
-            author_date = datetime.now()
+            author_date = datetime.now()  # noqa: DTZ005
         elif isinstance(author_date, str):
-            author_date = datetime.utcfromtimestamp(float(author_date))
+            author_date = datetime.utcfromtimestamp(float(author_date))  # noqa: DTZ004
         if not committer_date:
-            committer_date = datetime.now()
+            committer_date = datetime.now()  # noqa: DTZ005
         elif isinstance(committer_date, str):
-            committer_date = datetime.utcfromtimestamp(float(committer_date))
+            committer_date = datetime.utcfromtimestamp(float(committer_date))  # noqa: DTZ004
 
         self.hash: str = commit_hash
         self.author_name: str = author_name
         self.author_email: str = author_email
         self.author_date: datetime = author_date
         self.committer_name: str = committer_name
         self.committer_email: str = committer_email
         self.committer_date: datetime = committer_date
         self.subject: str = subject
         self.body: list[str] = _clean_body(body) if body else []
         self.url: str = url
 
         tag = ""
         for ref in refs.split(","):
-            ref = ref.strip()
+            ref = ref.strip()  # noqa: PLW2901
             if ref.startswith("tag: "):
                 tag = ref.replace("tag: ", "")
                 break
         self.tag: str = tag
         self.version: str = tag
 
         self.text_refs: dict[str, list[Ref]] = {}
@@ -90,25 +91,27 @@
         self.trailers: dict[str, str] = {}
         self.body_without_trailers = self.body
 
         if parse_trailers:
             self._parse_trailers()
 
     def update_with_convention(self, convention: CommitConvention) -> None:
-        """
-        Apply the convention-parsed data to this commit.
+        """Apply the convention-parsed data to this commit.
 
         Arguments:
             convention: The convention to use.
         """
         self.convention.update(convention.parse_commit(self))
 
-    def update_with_provider(self, provider: ProviderRefParser, parse_refs: bool = True) -> None:  # noqa: WPS231
-        """
-        Apply the provider-parsed data to this commit.
+    def update_with_provider(
+        self,
+        provider: ProviderRefParser,
+        parse_refs: bool = True,  # noqa: FBT001,FBT002
+    ) -> None:
+        """Apply the provider-parsed data to this commit.
 
         Arguments:
             provider: The provider to use.
             parse_refs: Whether to parse references for this provider.
         """
         # set the commit url based on provider
         # FIXME: hardcoded 'commits'
@@ -116,16 +119,19 @@
             self.url = provider.build_ref_url("commits", {"ref": self.hash})
         else:
             # use default "commit" url (could be wrong)
             self.url = f"{provider.url}/{provider.namespace}/{provider.project}/commit/{self.hash}"
 
         # build commit text references from its subject and body
         if parse_refs:
-            for ref_type in provider.REF.keys():
-                self.text_refs[ref_type] = provider.get_refs(ref_type, "\n".join([self.subject] + self.body))
+            for ref_type in provider.REF:
+                self.text_refs[ref_type] = provider.get_refs(
+                    ref_type,
+                    "\n".join([self.subject, *self.body]),
+                )
 
             if "issues" in self.text_refs:
                 self.text_refs["issues_not_in_subject"] = []
                 for issue in self.text_refs["issues"]:
                     if issue.ref not in self.subject:
                         self.text_refs["issues_not_in_subject"].append(issue)
 
@@ -154,27 +160,26 @@
     TYPES: dict[str, str]
     TYPE_REGEX: Pattern
     BREAK_REGEX: Pattern
     DEFAULT_RENDER: list[str]
 
     @abstractmethod
     def parse_commit(self, commit: Commit) -> dict[str, str | bool]:
-        """
-        Parse the commit to extract information.
+        """Parse the commit to extract information.
 
         Arguments:
             commit: The commit to parse.
 
         Returns:
             A dictionary containing the parsed data.
-        """  # noqa: DAR202,DAR401
+        """
         raise NotImplementedError
 
     @classmethod
-    def _format_sections_help(cls):
+    def _format_sections_help(cls) -> str:
         reversed_map = defaultdict(list)
         for section_type, section_title in cls.TYPES.items():
             reversed_map[section_title].append(section_type)
         default_sections = cls.DEFAULT_RENDER
         default = "- " + "\n- ".join(f"{', '.join(reversed_map[title])}: {title}" for title in default_sections)
         additional = "- " + "\n- ".join(
             f"{', '.join(types)}: {title}" for title, types in reversed_map.items() if title not in default_sections
@@ -202,26 +207,39 @@
         "fix": "Fixed",
         "change": "Changed",
         "remove": "Removed",
         "merge": "Merged",
         "doc": "Documented",
     }
 
-    TYPE_REGEX: Pattern = re.compile(r"^(?P<type>(%s))" % "|".join(TYPES.keys()), re.I)  # noqa: WPS323
-    BREAK_REGEX: Pattern = re.compile(r"^break(s|ing changes?)?[ :].+$", re.I | re.MULTILINE)
-    DEFAULT_RENDER: list[str] = [TYPES["add"], TYPES["fix"], TYPES["change"], TYPES["remove"]]
+    TYPE_REGEX: Pattern = re.compile(r"^(?P<type>(%s))" % "|".join(TYPES.keys()), re.I)
+    BREAK_REGEX: Pattern = re.compile(
+        r"^break(s|ing changes?)?[ :].+$",
+        re.I | re.MULTILINE,
+    )
+    DEFAULT_RENDER: list[str] = [
+        TYPES["add"],
+        TYPES["fix"],
+        TYPES["change"],
+        TYPES["remove"],
+    ]
 
-    def parse_commit(self, commit: Commit) -> dict[str, str | bool]:  # noqa: D102 (use parent docstring)
+    def parse_commit(self, commit: Commit) -> dict[str, str | bool]:  # noqa: D102
         commit_type = self.parse_type(commit.subject)
-        message = "\n".join([commit.subject] + commit.body)
+        message = "\n".join([commit.subject, *commit.body])
         is_major = self.is_major(message)
         is_minor = not is_major and self.is_minor(commit_type)
         is_patch = not any((is_major, is_minor))
 
-        return {"type": commit_type, "is_major": is_major, "is_minor": is_minor, "is_patch": is_patch}
+        return {
+            "type": commit_type,
+            "is_major": is_major,
+            "is_minor": is_minor,
+            "is_patch": is_patch,
+        }
 
     def parse_type(self, commit_subject: str) -> str:
         """Parse the type of the commit given its subject.
 
         Arguments:
             commit_subject: The commit message subject.
 
@@ -273,22 +291,31 @@
         "refactor": "Code Refactoring",
         "revert": "Reverts",
         "style": "Style",
         "test": "Tests",
         "tests": "Tests",
     }
     SUBJECT_REGEX: Pattern = re.compile(
-        r"^(?P<type>(%s))(?:\((?P<scope>.+)\))?: (?P<subject>.+)$" % ("|".join(TYPES.keys()))  # noqa: WPS323 (%)
+        r"^(?P<type>(%s))(?:\((?P<scope>.+)\))?: (?P<subject>.+)$" % ("|".join(TYPES.keys())),  # (%)
+    )
+    BREAK_REGEX: Pattern = re.compile(
+        r"^break(s|ing changes?)?[ :].+$",
+        re.I | re.MULTILINE,
     )
-    BREAK_REGEX: Pattern = re.compile(r"^break(s|ing changes?)?[ :].+$", re.I | re.MULTILINE)
-    DEFAULT_RENDER: list[str] = [TYPES["feat"], TYPES["fix"], TYPES["revert"], TYPES["refactor"], TYPES["perf"]]
+    DEFAULT_RENDER: list[str] = [
+        TYPES["feat"],
+        TYPES["fix"],
+        TYPES["revert"],
+        TYPES["refactor"],
+        TYPES["perf"],
+    ]
 
-    def parse_commit(self, commit: Commit) -> dict[str, str | bool]:  # noqa: D102 (use parent docstring)
+    def parse_commit(self, commit: Commit) -> dict[str, str | bool]:  # noqa: D102
         subject = self.parse_subject(commit.subject)
-        message = "\n".join([commit.subject] + commit.body)
+        message = "\n".join([commit.subject, *commit.body])
         is_major = self.is_major(message)
         is_minor = not is_major and self.is_minor(subject["type"])
         is_patch = not any((is_major, is_minor))
 
         return {
             "type": subject["type"],
             "scope": subject["scope"],
@@ -339,21 +366,20 @@
 
 class ConventionalCommitConvention(AngularConvention):
     """Conventional commit message convention."""
 
     TYPES: dict[str, str] = AngularConvention.TYPES
     DEFAULT_RENDER: list[str] = AngularConvention.DEFAULT_RENDER
     SUBJECT_REGEX: Pattern = re.compile(
-        r"^(?P<type>(%s))(?:\((?P<scope>.+)\))?(?P<breaking>!)?: (?P<subject>.+)$"  # noqa: WPS323 (%)
-        % ("|".join(TYPES.keys()))
+        r"^(?P<type>(%s))(?:\((?P<scope>.+)\))?(?P<breaking>!)?: (?P<subject>.+)$" % ("|".join(TYPES.keys())),  # (%)
     )
 
-    def parse_commit(self, commit: Commit) -> dict[str, str | bool]:  # noqa: D102 (use parent docstring)
+    def parse_commit(self, commit: Commit) -> dict[str, str | bool]:  # noqa: D102
         subject = self.parse_subject(commit.subject)
-        message = "\n".join([commit.subject] + commit.body)
+        message = "\n".join([commit.subject, *commit.body])
         is_major = self.is_major(message) or subject.get("breaking") == "!"
         is_minor = not is_major and self.is_minor(subject["type"])
         is_patch = not any((is_major, is_minor))
 
         return {
             "type": subject["type"],
             "scope": subject["scope"],
```

### Comparing `git-changelog-1.0.0/src/git_changelog/providers.py` & `git_changelog-1.0.1/src/git_changelog/providers.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,15 @@
     MENTION = r"@(?P<ref>\w[-\w]*)"
 
 
 class Ref:
     """A class to represent a reference and its URL."""
 
     def __init__(self, ref: str, url: str) -> None:
-        """
-        Initialization method.
+        """Initialization method.
 
         Arguments:
             ref: The reference text.
             url: The reference URL.
         """
         self.ref: str = ref
         self.url: str = url
@@ -39,16 +38,15 @@
         return self.ref + ": " + self.url
 
 
 class RefDef:
     """A class to store a reference regular expression and URL building string."""
 
     def __init__(self, regex: Pattern, url_string: str):
-        """
-        Initialization method.
+        """Initialization method.
 
         Arguments:
             regex: The regular expression to match the reference.
             url_string: The URL string to format using matched groups.
         """
         self.regex = regex
         self.url_string = url_string
@@ -59,83 +57,78 @@
 
     url: str
     namespace: str
     project: str
     REF: dict[str, RefDef] = {}
 
     def get_refs(self, ref_type: str, text: str) -> list[Ref]:
-        """
-        Find all references in the given text.
+        """Find all references in the given text.
 
         Arguments:
             ref_type: The reference type.
             text: The text in which to search references.
 
         Returns:
             A list of references (instances of [Ref][git_changelog.providers.Ref]).
         """
         return [
             Ref(ref=match.group().strip(), url=self.build_ref_url(ref_type, match.groupdict()))
             for match in self.parse_refs(ref_type, text)
         ]
 
     def parse_refs(self, ref_type: str, text: str) -> list[Match]:
-        """
-        Parse references in the given text.
+        """Parse references in the given text.
 
         Arguments:
             ref_type: The reference type.
             text: The text to parse.
 
         Returns:
             A list of regular expressions matches.
         """
         if ref_type not in self.REF:
-            refs = [key for key in self.REF.keys() if key.startswith(ref_type)]
+            refs = [key for key in self.REF if key.startswith(ref_type)]
             return [match for ref in refs for match in self.REF[ref].regex.finditer(text)]
         return list(self.REF[ref_type].regex.finditer(text))
 
     def build_ref_url(self, ref_type: str, match_dict: dict[str, str]) -> str:
-        """
-        Build the URL for a reference type and a dictionary of matched groups.
+        """Build the URL for a reference type and a dictionary of matched groups.
 
         Arguments:
             ref_type: The reference type.
             match_dict: The matched groups.
 
         Returns:
             The built URL.
         """
         return self.REF[ref_type].url_string.format(**match_dict)
 
     @abstractmethod
     def get_tag_url(self, tag: str) -> str:
-        """
-        Get the URL for a git tag.
+        """Get the URL for a git tag.
 
         Arguments:
             tag: The git tag.
 
         Returns:
             The tag URL.
-        """  # noqa: DAR202,DAR401
+        """
         raise NotImplementedError
 
     @abstractmethod
     def get_compare_url(self, base: str, target: str) -> str:
-        """
-        Get the URL for a tag comparison.
+        """Get the URL for a tag comparison.
 
         Arguments:
             base: The base tag.
             target: The target tag.
 
         Returns:
             The comparison URL.
-        """  # noqa: DAR202,DAR401
+        """
         raise NotImplementedError
 
 
 class GitHub(ProviderRefParser):
     """A parser for the GitHub references."""
 
     url: str = "https://github.com"
@@ -150,55 +143,57 @@
             regex=re.compile(RefRe.BB + RefRe.NP + "?" + RefRe.ID.format(symbol="#"), re.I),
             url_string="{base_url}/{namespace}/{project}/issues/{ref}",
         ),
         "commits": RefDef(
             regex=re.compile(
                 RefRe.BB
                 + r"(?:{np}@)?{commit}{ba}".format(
-                    np=RefRe.NP, commit=RefRe.COMMIT.format(min=commit_min_length, max=commit_max_length), ba=RefRe.BA
+                    np=RefRe.NP,
+                    commit=RefRe.COMMIT.format(min=commit_min_length, max=commit_max_length),
+                    ba=RefRe.BA,
                 ),
                 re.I,
             ),
             url_string="{base_url}/{namespace}/{project}/commit/{ref}",
         ),
         "commits_ranges": RefDef(
             regex=re.compile(
                 RefRe.BB
                 + r"(?:{np}@)?{commit_range}".format(
-                    np=RefRe.NP, commit_range=RefRe.COMMIT_RANGE.format(min=commit_min_length, max=commit_max_length)
+                    np=RefRe.NP,
+                    commit_range=RefRe.COMMIT_RANGE.format(min=commit_min_length, max=commit_max_length),
                 ),
                 re.I,
             ),
             url_string="{base_url}/{namespace}/{project}/compare/{ref}",
         ),
         "mentions": RefDef(regex=re.compile(RefRe.BB + RefRe.MENTION, re.I), url_string="{base_url}/{ref}"),
     }
 
     def __init__(self, namespace: str, project: str, url: str = url):
-        """
-        Initialization method.
+        """Initialization method.
 
         Arguments:
             namespace: The GitHub namespace.
             project: The GitHub project.
             url: The GitHub URL.
         """
         self.namespace: str = namespace
         self.project: str = project
-        self.url: str = url  # noqa: WPS601 (shadowing but uses class' as default)
+        self.url: str = url  # (shadowing but uses class' as default)
 
     def build_ref_url(self, ref_type: str, match_dict: dict[str, str]) -> str:  # noqa: D102 (use parent docstring)
         match_dict["base_url"] = self.url
         if not match_dict.get("namespace"):
             match_dict["namespace"] = self.namespace
         if not match_dict.get("project"):
             match_dict["project"] = self.project
         return super().build_ref_url(ref_type, match_dict)
 
-    def get_tag_url(self, tag: str = "") -> str:  # noqa: D102,WPS615
+    def get_tag_url(self, tag: str = "") -> str:  # noqa: D102
         return self.tag_url.format(base_url=self.url, namespace=self.namespace, project=self.project, ref=tag)
 
     def get_compare_url(self, base: str, target: str) -> str:  # noqa: D102 (use parent docstring)
         return self.build_ref_url("commits_ranges", {"ref": f"{base}...{target}"})
 
 
 class GitLab(ProviderRefParser):
@@ -226,25 +221,27 @@
         ),
         "labels_ids": RefDef(
             regex=re.compile(RefRe.BB + RefRe.NP + "?" + RefRe.ID.format(symbol=r"~"), re.I),
             url_string="{base_url}/{namespace}/{project}/issues?label_name[]={ref}",  # no label_id param?
         ),
         "labels_one_word": RefDef(
             regex=re.compile(  # also matches label IDs
-                RefRe.BB + RefRe.NP + "?" + RefRe.ONE_WORD.format(symbol=r"~"), re.I
+                RefRe.BB + RefRe.NP + "?" + RefRe.ONE_WORD.format(symbol=r"~"),
+                re.I,
             ),
             url_string="{base_url}/{namespace}/{project}/issues?label_name[]={ref}",
         ),
         "labels_multi_word": RefDef(
             regex=re.compile(RefRe.BB + RefRe.NP + "?" + RefRe.MULTI_WORD.format(symbol=r"~"), re.I),
             url_string="{base_url}/{namespace}/{project}/issues?label_name[]={ref}",
         ),
         "milestones_ids": RefDef(
             regex=re.compile(  # also matches milestones IDs
-                RefRe.BB + RefRe.NP + "?" + RefRe.ID.format(symbol=r"%"), re.I
+                RefRe.BB + RefRe.NP + "?" + RefRe.ID.format(symbol=r"%"),
+                re.I,
             ),
             url_string="{base_url}/{namespace}/{project}/milestones/{ref}",
         ),
         "milestones_one_word": RefDef(
             regex=re.compile(RefRe.BB + RefRe.NP + "?" + RefRe.ONE_WORD.format(symbol=r"%"), re.I),
             url_string="{base_url}/{namespace}/{project}/milestones",  # cannot guess ID
         ),
@@ -252,54 +249,56 @@
             regex=re.compile(RefRe.BB + RefRe.NP + "?" + RefRe.MULTI_WORD.format(symbol=r"%"), re.I),
             url_string="{base_url}/{namespace}/{project}/milestones",  # cannot guess ID
         ),
         "commits": RefDef(
             regex=re.compile(
                 RefRe.BB
                 + r"(?:{np}@)?{commit}{ba}".format(
-                    np=RefRe.NP, commit=RefRe.COMMIT.format(min=commit_min_length, max=commit_max_length), ba=RefRe.BA
+                    np=RefRe.NP,
+                    commit=RefRe.COMMIT.format(min=commit_min_length, max=commit_max_length),
+                    ba=RefRe.BA,
                 ),
                 re.I,
             ),
             url_string="{base_url}/{namespace}/{project}/commit/{ref}",
         ),
         "commits_ranges": RefDef(
             regex=re.compile(
                 RefRe.BB
                 + r"(?:{np}@)?{commit_range}".format(
-                    np=RefRe.NP, commit_range=RefRe.COMMIT_RANGE.format(min=commit_min_length, max=commit_max_length)
+                    np=RefRe.NP,
+                    commit_range=RefRe.COMMIT_RANGE.format(min=commit_min_length, max=commit_max_length),
                 ),
                 re.I,
             ),
             url_string="{base_url}/{namespace}/{project}/compare/{ref}",
         ),
         "mentions": RefDef(regex=re.compile(RefRe.BB + RefRe.MENTION, re.I), url_string="{base_url}/{ref}"),
     }
 
     def __init__(self, namespace: str, project: str, url: str = url):
-        """
-        Initialization method.
+        """Initialization method.
 
         Arguments:
             namespace: The GitLab namespace.
             project: The GitLab project.
             url: The GitLab URL.
         """
         self.namespace: str = namespace
         self.project: str = project
-        self.url: str = url  # noqa: WPS601 (shadowing but uses class' as default)
+        self.url: str = url  # (shadowing but uses class' as default)
 
     def build_ref_url(self, ref_type: str, match_dict: dict[str, str]) -> str:  # noqa: D102 (use parent docstring)
         match_dict["base_url"] = self.url
         if not match_dict.get("namespace"):
             match_dict["namespace"] = self.namespace
         if not match_dict.get("project"):
             match_dict["project"] = self.project
         if ref_type.startswith("label"):
             match_dict["ref"] = match_dict["ref"].replace('"', "").replace(" ", "+")
         return super().build_ref_url(ref_type, match_dict)
 
-    def get_tag_url(self, tag: str = "") -> str:  # noqa: D102,WPS615
+    def get_tag_url(self, tag: str = "") -> str:  # noqa: D102
         return self.tag_url.format(base_url=self.url, namespace=self.namespace, project=self.project, ref=tag)
 
     def get_compare_url(self, base: str, target: str) -> str:  # noqa: D102 (use parent docstring)
         return self.build_ref_url("commits_ranges", {"ref": f"{base}...{target}"})
```

### Comparing `git-changelog-1.0.0/src/git_changelog/templates/__init__.py` & `git_changelog-1.0.1/src/git_changelog/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `git-changelog-1.0.0/src/git_changelog/templates/angular.md.jinja` & `git_changelog-1.0.1/src/git_changelog/templates/angular.md.jinja`

 * *Files identical despite different names*

### Comparing `git-changelog-1.0.0/src/git_changelog/templates/keepachangelog.md.jinja` & `git_changelog-1.0.1/src/git_changelog/templates/keepachangelog.md.jinja`

 * *Files identical despite different names*

### Comparing `git-changelog-1.0.0/tests/test_angular_style.py` & `git_changelog-1.0.1/tests/test_basic_style.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,73 @@
-"""Tests for the Angular conventionntion."""
+"""Tests for the basic commit convention."""
 
-from git_changelog.commit import AngularConvention, Commit
+from __future__ import annotations
 
+from git_changelog.commit import BasicConvention, Commit
 
-def test_angular_convention_breaking_change():
+
+def test_basic_convention_breaking_change() -> None:
     """Breaking change (singular) is correctly identified."""
-    subject = "feat: this is a new breaking feature"
+    subject = "Added a new breaking feature"
     body = ["BREAKING CHANGE: there is a breaking feature in this code"]
     commit = Commit(
-        commit_hash="aaaaaaa", subject=subject, body=body, author_date="1574340645", committer_date="1574340645"
+        commit_hash="aaaaaaa",
+        subject=subject,
+        body=body,
+        author_date="1574340645",
+        committer_date="1574340645",
     )
-    convention = AngularConvention()
+    convention = BasicConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_angular_convention_breaking_changes():
+def test_basic_convention_breaking_changes() -> None:
     """Breaking changes (plural) are correctly identified."""
-    subject = "feat: this is a new breaking feature"
+    subject = "Added a new breaking feature"
     body = ["BREAKING CHANGES: there is a breaking feature in this code"]
     commit = Commit(
-        commit_hash="aaaaaaa", subject=subject, body=body, author_date="1574340645", committer_date="1574340645"
+        commit_hash="aaaaaaa",
+        subject=subject,
+        body=body,
+        author_date="1574340645",
+        committer_date="1574340645",
     )
-    convention = AngularConvention()
+    convention = BasicConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_angular_convention_feat():
+def test_basic_convention_feat() -> None:
     """Feature commit is correctly identified."""
-    subject = "feat: this is a new feature"
-    commit = Commit(commit_hash="aaaaaaa", subject=subject, author_date="1574340645", committer_date="1574340645")
-    convention = AngularConvention()
+    subject = "Added a new feature"
+    commit = Commit(
+        commit_hash="aaaaaaa",
+        subject=subject,
+        author_date="1574340645",
+        committer_date="1574340645",
+    )
+    convention = BasicConvention()
     commit_dict = convention.parse_commit(commit)
     assert not commit_dict["is_major"]
     assert commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_angular_convention_fix():
+def test_basic_convention_fix() -> None:
     """Bug fix commit is correctly identified."""
-    subject = "fix: this is a bug fix"
-    commit = Commit(commit_hash="aaaaaaa", subject=subject, author_date="1574340645", committer_date="1574340645")
-    convention = AngularConvention()
+    subject = "Fixed a bug"
+    commit = Commit(
+        commit_hash="aaaaaaa",
+        subject=subject,
+        author_date="1574340645",
+        committer_date="1574340645",
+    )
+    convention = BasicConvention()
     commit_dict = convention.parse_commit(commit)
     assert not commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert commit_dict["is_patch"]
```

### Comparing `git-changelog-1.0.0/tests/test_basic_style.py` & `git_changelog-1.0.1/tests/test_angular_style.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,73 @@
-"""Tests for the basic commit convention."""
+"""Tests for the Angular conventionntion."""
 
-from git_changelog.commit import BasicConvention, Commit
+from __future__ import annotations
 
+from git_changelog.commit import AngularConvention, Commit
 
-def test_basic_convention_breaking_change():
+
+def test_angular_convention_breaking_change() -> None:
     """Breaking change (singular) is correctly identified."""
-    subject = "Added a new breaking feature"
+    subject = "feat: this is a new breaking feature"
     body = ["BREAKING CHANGE: there is a breaking feature in this code"]
     commit = Commit(
-        commit_hash="aaaaaaa", subject=subject, body=body, author_date="1574340645", committer_date="1574340645"
+        commit_hash="aaaaaaa",
+        subject=subject,
+        body=body,
+        author_date="1574340645",
+        committer_date="1574340645",
     )
-    convention = BasicConvention()
+    convention = AngularConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_basic_convention_breaking_changes():
+def test_angular_convention_breaking_changes() -> None:
     """Breaking changes (plural) are correctly identified."""
-    subject = "Added a new breaking feature"
+    subject = "feat: this is a new breaking feature"
     body = ["BREAKING CHANGES: there is a breaking feature in this code"]
     commit = Commit(
-        commit_hash="aaaaaaa", subject=subject, body=body, author_date="1574340645", committer_date="1574340645"
+        commit_hash="aaaaaaa",
+        subject=subject,
+        body=body,
+        author_date="1574340645",
+        committer_date="1574340645",
     )
-    convention = BasicConvention()
+    convention = AngularConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_basic_convention_feat():
+def test_angular_convention_feat() -> None:
     """Feature commit is correctly identified."""
-    subject = "Added a new feature"
-    commit = Commit(commit_hash="aaaaaaa", subject=subject, author_date="1574340645", committer_date="1574340645")
-    convention = BasicConvention()
+    subject = "feat: this is a new feature"
+    commit = Commit(
+        commit_hash="aaaaaaa",
+        subject=subject,
+        author_date="1574340645",
+        committer_date="1574340645",
+    )
+    convention = AngularConvention()
     commit_dict = convention.parse_commit(commit)
     assert not commit_dict["is_major"]
     assert commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_basic_convention_fix():
+def test_angular_convention_fix() -> None:
     """Bug fix commit is correctly identified."""
-    subject = "Fixed a bug"
-    commit = Commit(commit_hash="aaaaaaa", subject=subject, author_date="1574340645", committer_date="1574340645")
-    convention = BasicConvention()
+    subject = "fix: this is a bug fix"
+    commit = Commit(
+        commit_hash="aaaaaaa",
+        subject=subject,
+        author_date="1574340645",
+        committer_date="1574340645",
+    )
+    convention = AngularConvention()
     commit_dict = convention.parse_commit(commit)
     assert not commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert commit_dict["is_patch"]
```

### Comparing `git-changelog-1.0.0/tests/test_conventional_commit_style.py` & `git_changelog-1.0.1/tests/test_conventional_commit_style.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,119 +1,157 @@
 """Tests for the conventional commit convention."""
 
+from __future__ import annotations
+
 from git_changelog.commit import Commit, ConventionalCommitConvention
 
 
-def test_conventional_convention_breaking_change():
+def test_conventional_convention_breaking_change() -> None:
     """Breaking change (singular) is correctly identified."""
     subject = "feat: this is a new breaking feature"
     body = ["BREAKING CHANGE: there is a breaking feature in this code"]
     commit = Commit(
-        commit_hash="aaaaaaa", subject=subject, body=body, author_date="1574340645", committer_date="1574340645"
+        commit_hash="aaaaaaa",
+        subject=subject,
+        body=body,
+        author_date="1574340645",
+        committer_date="1574340645",
     )
     convention = ConventionalCommitConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["type"] == "Features"
     assert commit_dict["scope"] is None
     assert commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_conventional_convention_breaking_changes():
+def test_conventional_convention_breaking_changes() -> None:
     """Breaking changes (plural) are correctly identified."""
     subject = "feat: this is a new breaking feature"
     body = ["BREAKING CHANGES: there is a breaking feature in this code"]
     commit = Commit(
-        commit_hash="aaaaaaa", subject=subject, body=body, author_date="1574340645", committer_date="1574340645"
+        commit_hash="aaaaaaa",
+        subject=subject,
+        body=body,
+        author_date="1574340645",
+        committer_date="1574340645",
     )
     convention = ConventionalCommitConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["type"] == "Features"
     assert commit_dict["scope"] is None
     assert commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_conventional_convention_subject_breaking_change():  # noqa: WPS118
+def test_conventional_convention_subject_breaking_change() -> None:
     """Breaking change in the subject (!) are correctly identified."""
     subject = "feat!: this is a new breaking feature"
     body = ["There is a breaking feature in this code"]
     commit = Commit(
-        commit_hash="aaaaaaa", subject=subject, body=body, author_date="1574340645", committer_date="1574340645"
+        commit_hash="aaaaaaa",
+        subject=subject,
+        body=body,
+        author_date="1574340645",
+        committer_date="1574340645",
     )
     convention = ConventionalCommitConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["type"] == "Features"
     assert commit_dict["scope"] is None
     assert commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_conventional_convention_subject_breaking_change_with_scope():  # noqa: WPS118
+def test_conventional_convention_subject_breaking_change_with_scope() -> None:
     """Breaking change in the subject (!) with scope are correctly identified."""
     subject = "feat(scope)!: this is a new breaking feature"
     body = ["There is a breaking feature in this code"]
     commit = Commit(
-        commit_hash="aaaaaaa", subject=subject, body=body, author_date="1574340645", committer_date="1574340645"
+        commit_hash="aaaaaaa",
+        subject=subject,
+        body=body,
+        author_date="1574340645",
+        committer_date="1574340645",
     )
     convention = ConventionalCommitConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["type"] == "Features"
     assert commit_dict["scope"] == "scope"
     assert commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_conventional_convention_feat():
+def test_conventional_convention_feat() -> None:
     """Feature commit is correctly identified."""
     subject = "feat: this is a new feature"
-    commit = Commit(commit_hash="aaaaaaa", subject=subject, author_date="1574340645", committer_date="1574340645")
+    commit = Commit(
+        commit_hash="aaaaaaa",
+        subject=subject,
+        author_date="1574340645",
+        committer_date="1574340645",
+    )
     convention = ConventionalCommitConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["type"] == "Features"
     assert commit_dict["scope"] is None
     assert not commit_dict["is_major"]
     assert commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_conventional_convention_feat_with_scope():
+def test_conventional_convention_feat_with_scope() -> None:
     """Feature commit is correctly identified."""
     subject = "feat(scope): this is a new feature"
-    commit = Commit(commit_hash="aaaaaaa", subject=subject, author_date="1574340645", committer_date="1574340645")
+    commit = Commit(
+        commit_hash="aaaaaaa",
+        subject=subject,
+        author_date="1574340645",
+        committer_date="1574340645",
+    )
     convention = ConventionalCommitConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["type"] == "Features"
     assert commit_dict["scope"] == "scope"
     assert not commit_dict["is_major"]
     assert commit_dict["is_minor"]
     assert not commit_dict["is_patch"]
 
 
-def test_conventional_convention_fix():
+def test_conventional_convention_fix() -> None:
     """Bug fix commit is correctly identified."""
     subject = "fix: this is a bug fix"
-    commit = Commit(commit_hash="aaaaaaa", subject=subject, author_date="1574340645", committer_date="1574340645")
+    commit = Commit(
+        commit_hash="aaaaaaa",
+        subject=subject,
+        author_date="1574340645",
+        committer_date="1574340645",
+    )
     convention = ConventionalCommitConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["type"] == "Bug Fixes"
     assert commit_dict["scope"] is None
     assert not commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert commit_dict["is_patch"]
 
 
-def test_conventional_convention_fix_with_scope():
+def test_conventional_convention_fix_with_scope() -> None:
     """Bug fix commit is correctly identified."""
     subject = "fix(scope): this is a bug fix"
-    commit = Commit(commit_hash="aaaaaaa", subject=subject, author_date="1574340645", committer_date="1574340645")
+    commit = Commit(
+        commit_hash="aaaaaaa",
+        subject=subject,
+        author_date="1574340645",
+        committer_date="1574340645",
+    )
     convention = ConventionalCommitConvention()
     commit_dict = convention.parse_commit(commit)
     assert commit_dict["type"] == "Bug Fixes"
     assert commit_dict["scope"] == "scope"
     assert not commit_dict["is_major"]
     assert not commit_dict["is_minor"]
     assert commit_dict["is_patch"]
```

### Comparing `git-changelog-1.0.0/tests/test_end_to_end.py` & `git_changelog-1.0.1/tests/test_end_to_end.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,106 +1,123 @@
 """End-to-end tests."""
 
+from __future__ import annotations
+
 import random
 import re
 import shutil
-import subprocess  # noqa: S404
+import subprocess
 from functools import partial
-from pathlib import Path
-from typing import Iterator
+from typing import TYPE_CHECKING, Iterator
 
 import pytest
 
 from git_changelog import Changelog
 from git_changelog.build import bump
 from git_changelog.cli import build_and_render
 from git_changelog.commit import AngularConvention
 from git_changelog.templates import get_template
 
+if TYPE_CHECKING:
+    from pathlib import Path
+
 VERSIONS = ("0.1.0", "0.2.0", "0.2.1", "1.0.0", "1.1.0", "")
+VERSIONS_V = ("v0.1.0", "v0.2.0", "v0.2.1", "v1.0.0", "v1.1.0", "")
 KEEP_A_CHANGELOG = get_template("keepachangelog")
 
 
-def _git(*args) -> str:
-    return subprocess.check_output([shutil.which("git") or "git", *args], text=True)  # noqa: S603
+def _git(*args: str) -> str:
+    return subprocess.check_output(
+        [shutil.which("git") or "git", *args],  # noqa: S603
+        text=True,
+    )
 
 
-def _commit(repo, filename, section):
+def _commit(repo: Path, filename: str, section: str) -> None:
     with repo.joinpath(filename).open("a") as fh:
         fh.write(str(random.randint(0, 1)))  # noqa: S311
-    _git("-C", repo, "add", "-A")
-    _git("-C", repo, "commit", "-m", f"{section}: Commit with '{section}' type")
+    _git("-C", str(repo), "add", "-A")
+    _git("-C", str(repo), "commit", "-m", f"{section}: Commit with '{section}' type")
 
 
-@pytest.fixture(scope="module", name="repo")
-def git_repo(tmp_path_factory) -> Iterator[Path]:
+@pytest.fixture(scope="module", name="repo", params=(VERSIONS, VERSIONS_V))
+def git_repo(
+    tmp_path_factory: pytest.TempPathFactory,
+    request: pytest.FixtureRequest,
+) -> Iterator[Path]:
     """Pytest fixture setting up a temporary Git repository.
 
     Parameters:
         tmp_path_factory: Utility to create temporary directories.
 
     Yields:
         The path to a temporary Git repository.
     """
     tmp_path = tmp_path_factory.mktemp("git_changelog")
+    tmp_path.mkdir(exist_ok=True, parents=True)
     git = partial(_git, "-C", str(tmp_path))
     commit = partial(_commit, tmp_path, "dummy")
     git("init")
     git("config", "user.name", "dummy")
     git("config", "user.email", "dummy@example.com")
     git("remote", "add", "origin", "git@github.com:example/example")
-    for version in VERSIONS:
-        for section in AngularConvention.TYPES.keys():
+    versions = request.param
+    for version in versions:
+        for section in AngularConvention.TYPES:
             commit(section)
             commit(section)
         if version:
             git("tag", version)
     yield tmp_path
     shutil.rmtree(tmp_path)
 
 
-def test_bumping_latest(repo):
+def test_bumping_latest(repo: Path) -> None:
     """Bump latest version.
 
     Parameters:
         repo: Path to a temporary repository.
     """
     changelog = Changelog(repo, convention=AngularConvention, bump_latest=True)
     # features, no breaking changes: minor bumped
-    assert changelog.versions_list[0].planned_tag == bump(VERSIONS[-2], "minor")
+    assert changelog.versions_list[0].planned_tag is not None
+    assert changelog.versions_list[0].planned_tag.lstrip("v") == bump(
+        VERSIONS[-2],
+        "minor",
+    )
     rendered = KEEP_A_CHANGELOG.render(changelog=changelog)
     assert "Unreleased" not in rendered
 
 
-def test_not_bumping_latest(repo):
+def test_not_bumping_latest(repo: Path) -> None:
     """Don't bump latest version.
 
     Parameters:
         repo: Path to a temporary repository.
     """
     changelog = Changelog(repo, convention=AngularConvention, bump_latest=False)
     assert changelog.versions_list[0].planned_tag is None
     rendered = KEEP_A_CHANGELOG.render(changelog=changelog)
     assert "Unreleased" in rendered
 
 
-def test_rendering_custom_sections(repo):
+def test_rendering_custom_sections(repo: Path) -> None:
     """Render custom sections.
 
     Parameters:
         repo: Path to a temporary repository.
     """
     changelog = Changelog(repo, convention=AngularConvention, sections=["feat"])
     rendered = KEEP_A_CHANGELOG.render(changelog=changelog)
     for section_type, section_title in AngularConvention.TYPES.items():
         if section_type != "feat":
             assert section_title not in rendered
 
 
-def test_rendering_in_place(repo, tmp_path):  # noqa: WPS218
+def test_rendering_in_place(repo: Path, tmp_path: Path) -> None:
     """Render changelog in-place.
 
     Parameters:
         repo: Path to a temporary repository.
         tmp_path: A temporary path to write the changelog into.
     """
     output = tmp_path.joinpath("changelog.md")
@@ -111,21 +128,62 @@
         output=output.as_posix(),
         template="keepachangelog",
     )
     assert len(re.findall("<!-- insertion marker -->", rendered)) == 2
     assert "Unreleased" in rendered
     latest_tag = "91.6.14"
     assert latest_tag not in rendered
-    _git("-C", repo, "tag", latest_tag)
+    _git("-C", str(repo), "tag", latest_tag)
     build_and_render(
         str(repo),
         convention="angular",
         bump_latest=True,
         output=output.as_posix(),
         template="keepachangelog",
         in_place=True,
     )
     rendered = output.read_text()
     assert len(re.findall("<!-- insertion marker -->", rendered)) == 1
     assert "Unreleased" not in rendered
     assert latest_tag in rendered
-    _git("-C", repo, "tag", "-d", latest_tag)
+    _git("-C", str(repo), "tag", "-d", latest_tag)
+
+
+def test_no_duplicate_rendering(repo: Path, tmp_path: Path) -> None:
+    """Render changelog in-place, and check for duplicate entries.
+
+    Parameters:
+        repo: Path to a temporary repository.
+        tmp_path: A temporary path to write the changelog into.
+    """
+    output = tmp_path.joinpath("changelog.md")
+    _, rendered = build_and_render(
+        str(repo),
+        convention="angular",
+        bump_latest=True,
+        output=output.as_posix(),
+        template="keepachangelog",
+    )
+
+    # When bump_latest is True, there's only one insertion marker
+    assert len(re.findall("<!-- insertion marker -->", rendered)) == 1
+    latest_tag = "1.2.0"
+    assert latest_tag in rendered
+
+    rendered = output.read_text()
+    # The latest tag should appear exactly three times in the changelog
+    assert rendered.count(latest_tag) == 3
+
+    # Without tagging a new version, we should get an error
+    with pytest.raises(ValueError, match=r"Version .* already in changelog"):
+        build_and_render(
+            str(repo),
+            convention="angular",
+            bump_latest=True,
+            output=output.as_posix(),
+            template="keepachangelog",
+            in_place=True,
+        )
+
+    rendered = output.read_text()
+    # The latest tag should still appear exactly three times in the changelog
+    assert rendered.count(latest_tag) == 3
```

### Comparing `git-changelog-1.0.0/tests/test_providers.py` & `git_changelog-1.0.1/tests/test_providers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Test providers references parsing."""
 
+from __future__ import annotations
+
 import git_changelog
 
 text = """
 This is the subject #1
 
 This is the body. Related: #2. Also mentions #3 and #4.
 Closes #5. closed #6, #7. FIX: #89 and #10.
@@ -21,19 +23,19 @@
 A commit range: 00000000...11111111
 A snippet: $45
 Some labels: ~18, ~bug, ~"multi word label"
 Some milestones: %2, %version1, %"awesome version"
 """
 
 
-def test_github_issue_parsing():
-    """GitHub issues are correctly parsed."""  # noqa: D403 (first word *is* correctly capitalized)
+def test_github_issue_parsing() -> None:
+    """GitHub issues are correctly parsed."""  # (first word *is* correctly capitalized)
     github = git_changelog.GitHub("pawamoy", "git-changelog")
-    for ref in github.REF.keys():
+    for ref in github.REF:
         assert github.get_refs(ref, text)
 
 
-def test_gitlab_issue_parsing():
-    """GitLab issues are correctly parsed."""  # noqa: D403 (first word *is* correctly capitalized)
+def test_gitlab_issue_parsing() -> None:
+    """GitLab issues are correctly parsed."""  # (first word *is* correctly capitalized)
     gitlab = git_changelog.GitLab("pawamoy", "git-changelog")
-    for ref in gitlab.REF.keys():
+    for ref in gitlab.REF:
         assert gitlab.get_refs(ref, text)
```

### Comparing `git-changelog-1.0.0/tests/test_version.py` & `git_changelog-1.0.1/tests/test_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Test version bumping."""
 
+from __future__ import annotations
+
 import pytest
 
 from git_changelog.build import bump
 
 
 @pytest.mark.parametrize(
     ("version", "bumped"),
@@ -20,15 +22,15 @@
         ("v0.1.1", "v0.1.2"),
         ("v1.0.0", "v1.0.1"),
         ("v1.0.1", "v1.0.2"),
         ("v1.1.0", "v1.1.1"),
         ("v1.1.1", "v1.1.2"),
     ],
 )
-def test_bump_patch(version, bumped):
+def test_bump_patch(version: str, bumped: str) -> None:
     """Test default and patch version bumping.
 
     Parameters:
         version: The base version.
         bumped: The expected, bumped version.
     """
     assert bump(version) == bump(version, "patch") == bumped
@@ -49,15 +51,15 @@
         ("v0.1.1", "v0.2.0"),
         ("v1.0.0", "v1.1.0"),
         ("v1.0.1", "v1.1.0"),
         ("v1.1.0", "v1.2.0"),
         ("v1.1.1", "v1.2.0"),
     ],
 )
-def test_bump_minor(version, bumped):
+def test_bump_minor(version: str, bumped: str) -> None:
     """Test minor version bumping.
 
     Parameters:
         version: The base version.
         bumped: The expected, bumped version.
     """
     assert bump(version, "minor") == bumped
@@ -78,15 +80,15 @@
         ("v0.1.1", "v0.2.0"),
         ("v1.0.0", "v2.0.0"),
         ("v1.0.1", "v2.0.0"),
         ("v1.1.0", "v2.0.0"),
         ("v1.1.1", "v2.0.0"),
     ],
 )
-def test_bump_major(version, bumped):
+def test_bump_major(version: str, bumped: str) -> None:
     """Test major version bumping.
 
     Parameters:
         version: The base version.
         bumped: The expected, bumped version.
     """
     assert bump(version, "major") == bumped
```

### Comparing `git-changelog-1.0.0/PKG-INFO` & `git_changelog-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: git-changelog
-Version: 1.0.0
+Version: 1.0.1
 Summary: Automatic Changelog generator using Jinja2 templates.
+Keywords: git changelog changelog-generator commit-style commit-convention
+Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
-Keywords: git,changelog,changelog-generator,commit-style,commit-convention
-Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
-Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Project-URL: Homepage, https://pawamoy.github.io/git-changelog
+Project-URL: Documentation, https://pawamoy.github.io/git-changelog
 Project-URL: Changelog, https://pawamoy.github.io/git-changelog/changelog
+Project-URL: Repository, https://github.com/pawamoy/git-changelog
+Project-URL: Issues, https://github.com/pawamoy/git-changelog/issues
 Project-URL: Discussions, https://github.com/pawamoy/git-changelog/discussions
-Project-URL: Documentation, https://pawamoy.github.io/git-changelog
-Project-URL: Funding, https://github.com/sponsors/pawamoy
 Project-URL: Gitter, https://gitter.im/git-changelog/community
-Project-URL: Homepage, https://pawamoy.github.io/git-changelog
-Project-URL: Issues, https://github.com/pawamoy/git-changelog/issues
-Project-URL: Repository, https://github.com/pawamoy/git-changelog
+Project-URL: Funding, https://github.com/sponsors/pawamoy
+Requires-Python: >=3.7
+Requires-Dist: Jinja2<4,>=2.10
+Requires-Dist: semver~=2.13
+Requires-Dist: importlib-metadata; python_version < "3.8"
 Description-Content-Type: text/markdown
 
 # git-changelog
 
 [![ci](https://github.com/pawamoy/git-changelog/workflows/ci/badge.svg)](https://github.com/pawamoy/git-changelog/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/git-changelog/)
 [![pypi version](https://img.shields.io/pypi/v/git-changelog.svg)](https://pypi.org/project/git-changelog/)
@@ -210,8 +213,7 @@
                         specify the path to a directory containing a file
                         named "changelog.md".
   -T, --trailers, --git-trailers
                         Parse Git trailers in the commit message. See
                         https://git-scm.com/docs/git-interpret-trailers.
   -v, --version         Show the current version of the program and exit.
 ```
-
```

