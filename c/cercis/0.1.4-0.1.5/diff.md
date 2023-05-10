# Comparing `tmp/cercis-0.1.4.tar.gz` & `tmp/cercis-0.1.5.tar.gz`

## Comparing `cercis-0.1.4.tar` & `cercis-0.1.5.tar`

### file list

```diff
@@ -1,307 +1,362 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.4/.coveragerc
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.4/.flake8
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.4/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.4/.gitattributes
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.1.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.4/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.4/.prettierrc.yaml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.4/.readthedocs.yaml
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 cercis-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.4/Dockerfile
--rw-r--r--   0        0        0    15433 2020-02-02 00:00:00.000000 cercis-0.1.4/README.md
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cercis-0.1.4/action.yml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.4/mypy.ini
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.4/test_requirements.txt
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.4/tox.ini
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/docs-issue.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/ISSUE_TEMPLATE/style_issue.md
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/check-changelog.yml
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/fuzz.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/lint.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/test.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/upload_binary.yml
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.1.4/.github/workflows/version-check.yml
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 cercis-0.1.4/action/main.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.4/autoload/black.vim
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.4/gallery/Dockerfile
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.4/gallery/README.md
--rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.4/gallery/gallery.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.4/plugin/black.vim
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/__init__.py
--rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/check_version_and_changelog.py
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/diff_shades_gha_helper.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/fuzz.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/make_width_table.py
--rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.4/scripts/migrate-black.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.4/src/_cercis_version.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blackd/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blackd/__main__.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blackd/middlewares.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/Grammar.txt
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/PatternGrammar.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/README
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/__init__.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pygram.py
--rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pytree.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/__init__.py
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/conv.py
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/driver.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/grammar.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/literals.py
--rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/parse.py
--rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/pgen.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/token.py
--rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 cercis-0.1.4/src/blib2to3/pgen2/tokenize.py
--rw-r--r--   0        0        0    49574 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/__main__.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/_width_table.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/brackets.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/cache.py
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/comments.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/concurrency.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/const.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/debug.py
--rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/files.py
--rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/handle_ipynb_magics.py
--rw-r--r--   0        0        0    62321 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/linegen.py
--rw-r--r--   0        0        0    38672 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/lines.py
--rw-r--r--   0        0        0     7837 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/mode.py
--rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/nodes.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/numerics.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/output.py
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/py.typed
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/report.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/rusty.py
--rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/strings.py
--rw-r--r--   0        0        0    91688 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/trans.py
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/utils_line_wrapping.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.1.4/src/cercis/utils_linegen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/conftest.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/empty.toml
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/optional.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test.toml
--rw-r--r--   0        0        0   101263 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_black.py
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_blackd.py
--rw-r--r--   0        0        0    12174 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_format.py
--rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_ipynb.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_no_ipynb.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_trans.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/test_utils_line_wrapping.py
--rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/util.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/conditional_expression.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/empty_pyproject.toml
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py
--rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
--rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/edge_cases.py
--rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
--rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
--rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
--rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
--rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/pragma_comments/Black_default.py
--rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/pragma_comments/Cercis_default.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring_preview.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/more_quotes.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/configurable_cases/single_quote/torture.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/fast/pep_572_do_not_remove_parens.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/ignore_subfolders_gitignore_tests/a.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/.gitignore
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/dont_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/dont_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/include_exclude_tests/b/exclude/a.pyi
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_gitignore_tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_nested_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_nested_gitignore_tests/a/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/invalid_nested_gitignore_tests/a/a.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/non_python_notebook.ipynb
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_empty_metadata.ipynb
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_no_trailing_newline.ipynb
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_trailing_newline.ipynb
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/jupyter/notebook_without_changes.ipynb
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/async_as_identifier.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/blackd_diff.diff
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/blackd_diff.py
--rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/debug_visitor.out
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/debug_visitor.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/decorators.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/docstring_no_string_normalization.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/force_py36.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/force_pyi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/invalid_header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/linelength6.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/long_strings_flag_disabled.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/missing_final_newline.diff
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/missing_final_newline.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/nested_class_stub.pyi
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/pattern_matching_invalid.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/power_op_newline.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/python2_detection.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/string_quotes.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/miscellaneous/stub.pyi
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/x.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/a.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/c.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/child/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/child/a.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/child/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/nested_gitignore_tests/root/child/c.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/async_stmts.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/cantfit.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/comments7.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/format_unicode_escape_seq.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_dict_values.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings__east_asian_width.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings__edge_case.py
--rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings__regression.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/long_strings__type_annotations.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/multiline_strings.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/percent_precedence.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/prefer_rhs_split.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/return_annotation_brackets_string.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview/trailing_comma.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/targeting_py38.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/targeting_py39.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_10.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_11.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_8.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_9.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/project_metadata/both_pyproject.toml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/project_metadata/neither_pyproject.toml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/project_metadata/only_black_pyproject.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/project_metadata/only_metadata_pyproject.toml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/parenthesized_context_managers.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_complex.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_extras.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_generic.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_simple.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pattern_matching_style.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/pep_572_py310.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/remove_newline_after_match.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_310/starred_for_target.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_311/pep_646.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_311/pep_654.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_311/pep_654_style.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_36/numeric_literals.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_36/numeric_literals_skip_underscores.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_37/python37.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_38/pep_570.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_38/pep_572.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_38/pep_572_remove_parens.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_38/python38.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_39/pep_572_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_39/python39.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/py_39/remove_with_brackets.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/attribute_access_on_number_literals.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/beginning_backslash.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/bracketmatch.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/class_blank_parentheses.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/class_methods_new_line.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/collections.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comment_after_escaped_newline.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments2.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments3.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments4.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments5.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments6.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments8.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments9.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/comments_non_breaking_space.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/composition.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/composition_no_trailing_comma.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/docstring_preview.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/empty_lines.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/expression.diff
--rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/expression.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff2.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff3.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff4.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtonoff5.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtpass_imports.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip2.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip3.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip4.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip5.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip6.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip7.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fmtskip8.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/fstring.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/function.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/function2.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/function_trailing_comma.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/import_spacing.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/one_element_subscript.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/power_op_spacing.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/prefer_rhs_split_reformatted.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_await_parens.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_except_parens.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_for_brackets.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_newline_after_code_block_open.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/remove_parens.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/return_annotation_brackets.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/skip_magic_trailing_comma.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/slices.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/torture.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens1.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens2.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens3.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/trailing_commas_in_leading_parts.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/tricky_unicode_symbols.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/tupleassign.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/simple_cases/whitespace.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.4/tests/data/type_comments/type_comment_syntax_error.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.4/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.4/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.4/LICENSE_ORIGINAL
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 cercis-0.1.4/pyproject.toml
--rw-r--r--   0        0        0    18951 2020-02-02 00:00:00.000000 cercis-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.5/.coveragerc
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.5/.flake8
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.5/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.5/.gitattributes
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 cercis-0.1.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.5/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.5/.prettierrc.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.5/.readthedocs.yaml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 cercis-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.5/Dockerfile
+-rw-r--r--   0        0        0    21217 2020-02-02 00:00:00.000000 cercis-0.1.5/README.md
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cercis-0.1.5/action.yml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.5/mypy.ini
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.5/test_requirements.txt
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.5/tox.ini
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/docs-issue.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/ISSUE_TEMPLATE/style_issue.md
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/check-changelog.yml
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/fuzz.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/upload_binary.yml
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 cercis-0.1.5/.github/workflows/version-check.yml
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 cercis-0.1.5/action/main.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.5/autoload/black.vim
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.5/gallery/Dockerfile
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.5/gallery/README.md
+-rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.5/gallery/gallery.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.5/plugin/black.vim
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/__init__.py
+-rw-r--r--   0        0        0     2500 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/check_version_and_changelog.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/diff_shades_gha_helper.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/fuzz.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/make_width_table.py
+-rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.5/scripts/migrate-black.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.5/src/_cercis_version.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blackd/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blackd/__main__.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blackd/middlewares.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/Grammar.txt
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/PatternGrammar.txt
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/README
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/__init__.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pygram.py
+-rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pytree.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/__init__.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/conv.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/driver.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/grammar.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/literals.py
+-rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/parse.py
+-rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/pgen.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/token.py
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 cercis-0.1.5/src/blib2to3/pgen2/tokenize.py
+-rw-r--r--   0        0        0    51483 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/__main__.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/_width_table.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/brackets.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/cache.py
+-rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/comments.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/concurrency.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/const.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/debug.py
+-rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/files.py
+-rw-r--r--   0        0        0    13514 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/handle_ipynb_magics.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/indent.py
+-rw-r--r--   0        0        0    62861 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/linegen.py
+-rw-r--r--   0        0        0    39809 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/lines.py
+-rw-r--r--   0        0        0     8223 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/mode.py
+-rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/nodes.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/numerics.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/output.py
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/py.typed
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/report.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/rusty.py
+-rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/strings.py
+-rw-r--r--   0        0        0    91890 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/trans.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/utils_line_wrapping.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 cercis-0.1.5/src/cercis/utils_linegen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/conftest.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/empty.toml
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/optional.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test.toml
+-rw-r--r--   0        0        0   101263 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_black.py
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_blackd.py
+-rw-r--r--   0        0        0    14908 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_format.py
+-rw-r--r--   0        0        0    16390 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_ipynb.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_no_ipynb.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_trans.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/test_utils_line_wrapping.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/util.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/conditional_expression.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/empty_pyproject.toml
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py
+-rw-r--r--   0        0        0     4438 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
+-rw-r--r--   0        0        0     4262 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3747 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3854 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4357 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4492 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     5066 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     5337 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     5497 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     5768 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=1/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3737 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=2/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3866 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3952 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=3/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     4372 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=4/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     4946 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     5177 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     5297 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     5528 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_spaces/closing_bracket_no_extra_indent/base_indent_spaces=8/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3502 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3535 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_extra_indent/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=False.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=False_olcei=True.py
+-rw-r--r--   0        0        0     3477 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=False.py
+-rw-r--r--   0        0        0     3505 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/closing_bracket_no_extra_indent/fdei=True_olcei=True.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_1.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_2.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_3.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_4.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_5.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/indentation/use_tabs/line_length_calculation/tab_width_8.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/edge_cases.py
+-rw-r--r--   0        0        0    11060 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
+-rw-r--r--   0        0        0    22087 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py
+-rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py
+-rw-r--r--   0        0        0     2011 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py
+-rw-r--r--   0        0        0     2212 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/pragma_comments/Black_default.py
+-rw-r--r--   0        0        0    10763 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/pragma_comments/Cercis_default.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring_preview.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/more_quotes.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/configurable_cases/single_quote/torture.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/fast/pep_572_do_not_remove_parens.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/ignore_subfolders_gitignore_tests/a.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/.gitignore
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/dont_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/include_exclude_tests/b/exclude/a.pyi
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_gitignore_tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_nested_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_nested_gitignore_tests/a/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/invalid_nested_gitignore_tests/a/a.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/non_python_notebook.ipynb
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_empty_metadata.ipynb
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_no_trailing_newline.ipynb
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_trailing_newline.ipynb
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/jupyter/notebook_without_changes.ipynb
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/async_as_identifier.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/blackd_diff.diff
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/blackd_diff.py
+-rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/debug_visitor.out
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/debug_visitor.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/decorators.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/docstring_no_string_normalization.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/force_py36.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/force_pyi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/invalid_header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/linelength6.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/long_strings_flag_disabled.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/missing_final_newline.diff
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/missing_final_newline.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/nested_class_stub.pyi
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/pattern_matching_invalid.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/power_op_newline.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/python2_detection.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/string_quotes.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/miscellaneous/stub.pyi
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/x.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/a.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/child/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/child/a.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/child/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/nested_gitignore_tests/root/child/c.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/async_stmts.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/cantfit.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/comments7.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/format_unicode_escape_seq.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_dict_values.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings__east_asian_width.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings__edge_case.py
+-rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings__regression.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/long_strings__type_annotations.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/multiline_strings.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/percent_precedence.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/prefer_rhs_split.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/return_annotation_brackets_string.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview/trailing_comma.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/targeting_py38.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/targeting_py39.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_10.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_11.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_8.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_9.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/project_metadata/both_pyproject.toml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/project_metadata/neither_pyproject.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/project_metadata/only_black_pyproject.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/project_metadata/only_metadata_pyproject.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/parenthesized_context_managers.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_complex.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_extras.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_generic.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_simple.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pattern_matching_style.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/pep_572_py310.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/remove_newline_after_match.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_310/starred_for_target.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_311/pep_646.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_311/pep_654.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_311/pep_654_style.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_36/numeric_literals.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_36/numeric_literals_skip_underscores.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_37/python37.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_38/pep_570.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_38/pep_572.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_38/pep_572_remove_parens.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_38/python38.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_39/pep_572_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_39/python39.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/py_39/remove_with_brackets.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/attribute_access_on_number_literals.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/beginning_backslash.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/bracketmatch.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/class_blank_parentheses.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/class_methods_new_line.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/collections.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comment_after_escaped_newline.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments2.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments3.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments4.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments5.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments6.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments8.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments9.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/comments_non_breaking_space.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/composition.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/composition_no_trailing_comma.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/docstring_preview.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/empty_lines.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/expression.diff
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/expression.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff2.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff3.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff4.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtonoff5.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtpass_imports.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip2.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip3.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip4.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip5.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip6.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip7.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fmtskip8.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/fstring.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/function.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/function2.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/function_trailing_comma.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/import_spacing.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/one_element_subscript.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/power_op_spacing.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/prefer_rhs_split_reformatted.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_await_parens.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_except_parens.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_for_brackets.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_newline_after_code_block_open.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/remove_parens.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/return_annotation_brackets.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/skip_magic_trailing_comma.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/slices.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/torture.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens1.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens2.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens3.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/trailing_commas_in_leading_parts.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/tricky_unicode_symbols.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/tupleassign.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/simple_cases/whitespace.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.5/tests/data/type_comments/type_comment_syntax_error.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.5/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.5/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.5/LICENSE_ORIGINAL
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 cercis-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0    24988 2020-02-02 00:00:00.000000 cercis-0.1.5/PKG-INFO
```

### Comparing `cercis-0.1.4/.pre-commit-config.yaml` & `cercis-0.1.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.pre-commit-hooks.yaml` & `cercis-0.1.5/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/CHANGELOG.md` & `cercis-0.1.5/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Change Log
 
+## [0.1.5] - 2023-05-09
+
+- Added
+  - Configurability to use tabs instead of spaces (two new options:
+    `--use-tabs` and `--tab-width`)
+  - Configurability on base indentation spaces and extra indentation at
+    different line continuation situations
+
 ## [0.1.4] - 2023-05-07
 
 - Added
   - A new configurable option: `--closing-bracket-extra-indent`
 
 ## [0.1.3] - 2023-05-07
```

### Comparing `cercis-0.1.4/Dockerfile` & `cercis-0.1.5/Dockerfile`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/README.md` & `cercis-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,31 @@
-# Cercis
+# _Cercis_
 
 [![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Red_bud_2009.jpg/320px-Red_bud_2009.jpg)](https://en.wikipedia.org/wiki/Cercis)
 
 _**Cercis**_ /ˈsɜːrsɪs/ is a Python code formatter that is more configurable
 than [Black](https://github.com/psf/black) (a popular Python code formatter).
 
 [_Cercis_](https://en.wikipedia.org/wiki/Cercis) is also the name of a
 deciduous tree that boasts vibrant pink to purple-hued flowers, which bloom in
 early spring.
 
 This code repository is forked from and directly inspired by
 [Black](https://github.com/psf/black). The original license of Black is
 included in this repository (see [LICENSE_ORIGINAL](./LICENSE_ORIGINAL)).
 
+_Cercis_ inherited Black's very comprehensive test cases, which means we are
+confident that our configurability addition does not introduce any undesirable
+side effects. We also thoroughly tested every configurable options that we
+added.
+
+In particular, via its configurable options, _Cercis_ can completely fall back
+to Black. See [Section 4.5](#45-how-to-fall-back-to-blacks-behavior) below for
+more details.
+
 ## 1. Motivations
 
 While we like the idea of auto-formatting and code readability, we take issue
 with some style choices and the lack of configurability of the Black formatter.
 Therefore, _Cercis_ aims at providing some configurability beyond Black's
 limited offering.
 
@@ -84,19 +93,23 @@
 The main difference is that _Cercis_ provides several configurable options that
 Black doesn't. Configurability is our main motivation behind creating _Cercis_.
 
 _Cercis_ offers the following configurable options:
 
 1. [Line length](#31-line-length)
 2. [Single quote vs double quote](#32-single-quote-vs-double-quote)
-3. [Extra indentation at function definition](#33-extra-indentation-at-function-definition)
-4. [Extra indentation at closing brackets](#34-closing-bracket-indentation)
-5. ["Simple" lines with long strings](#35-simple-lines-with-long-strings)
-6. [Collapse nested brackets](#36-collapse-nested-brackets)
-7. [Wrap pragma comments](#37-wrapping-long-lines-ending-with-pragma-comments)
+3. [Tabs vs spaces](#33-tabs-vs-spaces)
+4. [Base indentation spaces](#34-base-indentation-spaces)
+5. [Extra indentation at line continuation](#35-extra-indentation-at-line-continuation)
+   1. [At function definition](#351-at-function-definition---function-definition-extra-indent)
+   2. [In other line continuations](#352-in-other-line-continuations---other-line-continuation-extra-indent)
+   3. [At closing brackets](#353-at-closing-brackets---closing-bracket-extra-indent)
+6. ["Simple" lines with long strings](#36-simple-lines-with-long-strings)
+7. [Collapse nested brackets](#37-collapse-nested-brackets)
+8. [Wrap pragma comments](#38-wrapping-long-lines-ending-with-pragma-comments)
 
 The next section ([How to configure _Cercis_](#4-how-to-configure-cercis))
 contains detailed instructions of how to configure these options.
 
 ### 3.1. Line length
 
 _Cercis_ uses 79 characters as the line length limit, instead of 88 (Black's
@@ -127,15 +140,82 @@
 | Abbreviation           | `-sq`                                        |
 | Default                | `True`                                       |
 | Black's default        | `False`                                      |
 | Command line usage     | `cercis -sq=True myScript.py`                |
 | `pyproject.toml` usage | `single-quote = false` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--single-quote=False]`               |
 
-### 3.3. Extra indentation at function definition
+### 3.3. Tabs vs spaces
+
+_Cercis_ offers users the ability to use tabs rather than spaces.
+
+There are two associated options:
+
+- `--use-tabs` (bool): whether to use tabs or spaces to format the code
+
+| Option                 |                                          |
+| ---------------------- | ---------------------------------------- |
+| Name                   | `--use-tabs`                             |
+| Abbreviation           | `-tab`                                   |
+| Default                | `False`                                  |
+| Black's default        | `False`                                  |
+| Command line usage     | `cercis -tab=True myScript.py`           |
+| `pyproject.toml` usage | `use-tabs = false` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--use-tabs=False]`               |
+
+- `--tab-width` (int): when calculating line length (to determine whether to
+  wrap lines), how wide shall _Cercis_ treat each tab. Only effective when
+  `--use-tabs` is set to `True`.
+
+| Option                 |                                       |
+| ---------------------- | ------------------------------------- |
+| Name                   | `--tab-width`                         |
+| Abbreviation           | `-tw`                                 |
+| Default                | 4                                     |
+| Black's default        | N/A                                   |
+| Command line usage     | `cercis -tab=True -tw=2 myScript.py`  |
+| `pyproject.toml` usage | `tab-width = 2` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--tab-width=2]`               |
+
+### 3.4. Base indentation spaces
+
+This option defines the number of spaces that each indentation level adds. This
+option has no effect when `--use-tabs` is set to `True`.
+
+For example, if you set it to 2, contents within a `for` block is indented 2
+spaces:
+
+```python
+for i in (1, 2, 3, 4, 5):
+  print(i)
+```
+
+| Option                 |                                                     |
+| ---------------------- | --------------------------------------------------- |
+| Name                   | `--base-indentation-spaces`                         |
+| Abbreviation           | `-bis`                                              |
+| Default                | 4                                                   |
+| Black's default        | 4                                                   |
+| Command line usage     | `cercis -bis=True -tw=2 myScript.py`                |
+| `pyproject.toml` usage | `base-indentation-spaces = 2` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--base-indentation-spaces=2]`               |
+
+### 3.5. Extra indentation at line continuations
+
+There are three associated options:
+
+- `--function-definition-extra-indent`
+- `--other-line-continuation-extra-indent`
+- `--closing-bracket-extra-indent`
+
+They control whether we add an **additional** indentation level in some
+situations. Note that these options can work well with tabs
+(`--use-tabs=True`).
+
+#### 3.5.1. At function definition (`--function-definition-extra-indent`)
 
 <table>
   <tr>
     <td>
 
 ```python
 # Cercis's default style
@@ -164,32 +244,80 @@
 ```
 
   </td>
 
   </tr>
 </table>
 
-We choose to indent an extra 4 spaces (8 in total) because it adds a clear
-visual separation between the function name and the argument list. Not adding
-extra indentation is also called out as wrong in the the official
-[PEP8 style guide](https://peps.python.org/pep-0008/#indentation).
+We choose to add an extra indentation level when wrapping a function signature
+line. This is because `def␣` happens to be 4 characters, so when the base
+indentation is 4 spaces, it can be difficult to visually distinguish the
+function name and the argument list if we don't add an extra indentation.
 
-You can override this default if necessary.
+If you set `--base-indentation-spaces` to other values than 4, this visual
+separation issue will disappear, and you may not need to turn this option on.
+
+This style is encouraged
+[in PEP8](https://peps.python.org/pep-0008/#indentation).
 
 | Option                 |                                                                 |
 | ---------------------- | --------------------------------------------------------------- |
 | Name                   | `--function-definition-extra-indent`                            |
 | Abbreviation           | `-fdei`                                                         |
 | Default                | `True`                                                          |
 | Black's default        | `False`                                                         |
 | Command line usage     | `cercis -fdei=False myScript.py`                                |
 | `pyproject.toml` usage | `function-definition-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--function-definition-extra-indent=False]`              |
 
-## 3.4. Closing bracket indentation
+#### 3.5.2. In other line continuations (`--other-line-continuation-extra-indent`)
+
+"Other line continuations" are cases other than in function definitions, such
+as:
+
+```python
+var = some_function(
+    arg1_with_long_name,
+    arg2_with_longer_name,
+)
+
+var2 = [
+    'something',
+    'something else',
+    'something more',
+]
+```
+
+So if you set this option (`--other-line-continuation-extra-indent`) to `True`,
+you can add an extra level of indentation in these cases:
+
+```python
+var = some_function(
+        arg1_with_long_name,
+        arg2_with_longer_name,
+)
+
+var2 = [
+        'something',
+        'something else',
+        'something more',
+]
+```
+
+| Option                 |                                                                     |
+| ---------------------- | ------------------------------------------------------------------- |
+| Name                   | `--other-line-continuation-extra-indent`                            |
+| Abbreviation           | `-olcei`                                                            |
+| Default                | `False`                                                             |
+| Black's default        | `False`                                                             |
+| Command line usage     | `cercis -olcei=True myScript.py`                                    |
+| `pyproject.toml` usage | `other-line-continuation-extra-indent = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [----other-line-continuation-extra-indent=False]`            |
+
+#### 3.5.3. At closing brackets (`--closing-bracket-extra-indent`)
 
 This option lets people customize where the closing bracket should be. Note
 that both styles are OK according to
 [PEP8](https://peps.python.org/pep-0008/#indentation).
 
 <table>
   <tr>
@@ -260,15 +388,15 @@
 | Abbreviation           | `-cbei`                                                     |
 | Default                | `False`                                                     |
 | Black's default        | `False`                                                     |
 | Command line usage     | `cercis -cbei=True myScript.py`                             |
 | `pyproject.toml` usage | `closing-bracket-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--closing-bracket-extra-indent=False]`              |
 
-### 3.5. "Simple" lines with long strings
+### 3.6. "Simple" lines with long strings
 
 By default, Black wraps lines that exceed length limit. But for very simple
 lines (such as assigning a long string to a variable), line wrapping is not
 necessary.
 
 <table>
   <tr>
@@ -327,15 +455,15 @@
 | Abbreviation           | `-wl`                                                     |
 | Default                | `False`                                                   |
 | Black's default        | `True`                                                    |
 | Command line usage     | `cercis -wl=True myScript.py`                             |
 | `pyproject.toml` usage | `wrap-line-with-long-string = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--wrap-line-with-long-string=False]`              |
 
-### 3.6. Collapse nested brackets
+### 3.7. Collapse nested brackets
 
 _Cercis_ by default collapses nested brackets to make the code more compact.
 
 <table>
   <tr>
     <td>
 
@@ -403,15 +531,15 @@
 | Command line usage     | `cercis -cnb=True myScript.py`                          |
 | `pyproject.toml` usage | `collapse-nested-brackets = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--collapse-nested-brackets=False]`              |
 
 The code implementation of this option comes from
 [Pyink](https://github.com/google/pyink), another forked project from Black.
 
-### 3.7. Wrapping long lines ending with pragma comments [^](#3-cerciss-code-style)
+### 3.8. Wrapping long lines ending with pragma comments
 
 "Pragma comments", in this context, mean the directives for Python linters
 usually to tell them to ignore certain errors. Pragma comments that _Cercis_
 currently recognizes include:
 
 - _noqa_: `# noqa: E501`
 - _type: ignore_: `# type: ignore[no-untyped-def]`
@@ -533,11 +661,25 @@
 means to always use the latest (including unreleased) _Cercis_ features.
 
 ### 4.4. Specify options in `tox.ini`
 
 Currently, _Cercis_ does not support a config section in `tox.ini`. Instead,
 you can specify the options in `pyproject.toml`.
 
-### 4.5. How to reproduce Black's behavior
+### 4.5. How to fall back to Black's behavior
 
-If you'd like to reproduce Black's behavior, simply set all the configurable
-options in [Section 3](#3-cerciss-code-style) to Black's default values.
+Here are the configuration options to fall back to Black's behavior. Put them
+in `pyproject.toml`:
+
+```toml
+[tool.cercis]
+line-length = 88
+single-quote = false
+use-tabs = false
+base-indentation-spaces = 4
+function-definition-extra-indent = false
+other-line-continuation-extra-indent = false
+closing-bracket-extra-indent = false
+wrap-line-with-long-string = true
+collapse-nested-brackets = false
+wrap-pragma-comments = true
+```
```

### Comparing `cercis-0.1.4/action.yml` & `cercis-0.1.5/action.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/mypy.ini` & `cercis-0.1.5/mypy.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tox.ini` & `cercis-0.1.5/tox.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/PULL_REQUEST_TEMPLATE.md` & `cercis-0.1.5/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/dependabot.yml` & `cercis-0.1.5/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/ISSUE_TEMPLATE/bug_report.md` & `cercis-0.1.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/ISSUE_TEMPLATE/config.yml` & `cercis-0.1.5/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/ISSUE_TEMPLATE/docs-issue.md` & `cercis-0.1.5/.github/ISSUE_TEMPLATE/docs-issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/ISSUE_TEMPLATE/feature_request.md` & `cercis-0.1.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/ISSUE_TEMPLATE/style_issue.md` & `cercis-0.1.5/.github/ISSUE_TEMPLATE/style_issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/workflows/check-changelog.yml` & `cercis-0.1.5/.github/workflows/check-changelog.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/workflows/docker.yml` & `cercis-0.1.5/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/workflows/fuzz.yml` & `cercis-0.1.5/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/workflows/lint.yml` & `cercis-0.1.5/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/workflows/python-package.yml` & `cercis-0.1.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/workflows/python-publish.yml` & `cercis-0.1.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/workflows/test.yml` & `cercis-0.1.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/workflows/upload_binary.yml` & `cercis-0.1.5/.github/workflows/upload_binary.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/.github/workflows/version-check.yml` & `cercis-0.1.5/.github/workflows/version-check.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/action/main.py` & `cercis-0.1.5/action/main.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/autoload/black.vim` & `cercis-0.1.5/autoload/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/gallery/README.md` & `cercis-0.1.5/gallery/README.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/gallery/gallery.py` & `cercis-0.1.5/gallery/gallery.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/plugin/black.vim` & `cercis-0.1.5/plugin/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/scripts/check_version_and_changelog.py` & `cercis-0.1.5/scripts/check_version_and_changelog.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/scripts/diff_shades_gha_helper.py` & `cercis-0.1.5/scripts/diff_shades_gha_helper.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/scripts/fuzz.py` & `cercis-0.1.5/scripts/fuzz.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/scripts/make_width_table.py` & `cercis-0.1.5/scripts/make_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/scripts/migrate-black.py` & `cercis-0.1.5/scripts/migrate-black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blackd/__init__.py` & `cercis-0.1.5/src/blackd/__init__.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blackd/middlewares.py` & `cercis-0.1.5/src/blackd/middlewares.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/Grammar.txt` & `cercis-0.1.5/src/blib2to3/Grammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/LICENSE` & `cercis-0.1.5/src/blib2to3/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/PatternGrammar.txt` & `cercis-0.1.5/src/blib2to3/PatternGrammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/README` & `cercis-0.1.5/src/blib2to3/README`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pygram.py` & `cercis-0.1.5/src/blib2to3/pygram.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pytree.py` & `cercis-0.1.5/src/blib2to3/pytree.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pgen2/conv.py` & `cercis-0.1.5/src/blib2to3/pgen2/conv.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pgen2/driver.py` & `cercis-0.1.5/src/blib2to3/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pgen2/grammar.py` & `cercis-0.1.5/src/blib2to3/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pgen2/literals.py` & `cercis-0.1.5/src/blib2to3/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pgen2/parse.py` & `cercis-0.1.5/src/blib2to3/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pgen2/pgen.py` & `cercis-0.1.5/src/blib2to3/pgen2/pgen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pgen2/token.py` & `cercis-0.1.5/src/blib2to3/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/blib2to3/pgen2/tokenize.py` & `cercis-0.1.5/src/blib2to3/pgen2/tokenize.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/__init__.py` & `cercis-0.1.5/src/cercis/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,25 @@
 
 from _cercis_version import version as __version__
 from blib2to3.pgen2 import token
 from blib2to3.pytree import Leaf, Node
 from cercis.cache import Cache, get_cache_info, read_cache, write_cache
 from cercis.comments import normalize_fmt_off
 from cercis.const import (
+    DEFAULT_BASE_INDENTATION_SPACES,
     DEFAULT_CLOSING_BRACKET_EXTRA_INDENT,
     DEFAULT_COLLAPSE_NESTED_BRACKETS,
     DEFAULT_EXCLUDES,
     DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     DEFAULT_INCLUDES,
     DEFAULT_LINE_LENGTH,
+    DEFAULT_OTHER_LINE_CONTINUATION_EXTRA_INDENT,
     DEFAULT_SINGLE_QUOTE,
+    DEFAULT_TAB_WIDTH,
+    DEFAULT_USE_TABS,
     DEFAULT_WRAP_LINE_WITH_LONG_STRING,
     DEFAULT_WRAP_PRAGMA_COMMENTS,
     STDIN_PLACEHOLDER,
 )
 from cercis.files import (
     find_project_root,
     find_pyproject_toml,
@@ -199,14 +203,25 @@
 ) -> Optional[Pattern[str]]:
     try:
         return re_compile_maybe_verbose(value) if value is not None else None
     except re.error as e:
         raise click.BadParameter(f"Not a valid regular expression: {e}") from None
 
 
+def validate_positive_integer(
+        ctx: click.Context,
+        param: click.Parameter,
+        value: Optional[int],
+) -> Optional[int]:
+    if not isinstance(value, int) or value <= 0:
+        raise click.BadParameter("Not a positive integer") from None
+
+    return value
+
+
 @click.command(
     context_settings={"help_option_names": ["-h", "--help"]},
     # While Click does set this field automatically using the docstring, mypyc
     # (annoyingly) strips 'em so we need to set it here too.
     help="The uncompromising code formatter.",
 )
 @click.option("-c", "--code", type=str, help="Format the code passed in as a string.")
@@ -215,25 +230,67 @@
     "--line-length",
     type=int,
     default=DEFAULT_LINE_LENGTH,
     help="How many characters per line to allow.",
     show_default=True,
 )
 @click.option(
+    "-tab",
+    "--use-tabs",
+    type=bool,
+    show_default=True,
+    default=DEFAULT_USE_TABS,
+    help="If True, use tabs as indentation, rather than spaces.",
+)
+@click.option(
+    "-tw",
+    "--tab-width",
+    type=int,
+    show_default=True,
+    default=DEFAULT_TAB_WIDTH,
+    callback=validate_positive_integer,
+    help=(
+        "The tab width to assume when calculating line length."
+        " This option is only effective when --use-tabs is set to True."
+        " Use a value that matches your editor's tab size setting for"
+        " consistent behaviors."
+    ),
+)
+@click.option(
+    "-bis",
+    "--base-indentation-spaces",
+    type=int,
+    show_default=True,
+    default=DEFAULT_BASE_INDENTATION_SPACES,
+    callback=validate_positive_integer,
+    help=(
+        "How many spaces to use for each indentation level."
+        " It has no effect when --use-tabs is True."
+    ),
+)
+@click.option(
     "-fdei",
     "--function-definition-extra-indent",
     type=bool,
     show_default=True,
     default=DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     help=(
         "If True, use 8 spaces as indent in function definition;"
         " otherwise, use 8 (Black's default)."
     ),
 )
 @click.option(
+    "-olcei",
+    "--other-line-continuation-extra-indent",
+    type=bool,
+    show_default=True,
+    default=DEFAULT_OTHER_LINE_CONTINUATION_EXTRA_INDENT,
+    help="If True, add an extra indentation level when wrapping longer lines.",
+)
+@click.option(
     "-cbei",
     "--closing-bracket-extra-indent",
     type=bool,
     show_default=True,
     default=DEFAULT_CLOSING_BRACKET_EXTRA_INDENT,
     help=(
         "If True, add an extra indentation level (4 or 8, depending on"
@@ -502,14 +559,18 @@
         line_length: int,
         function_definition_extra_indent: bool,
         closing_bracket_extra_indent: bool,
         single_quote: bool,
         wrap_line_with_long_string: bool,
         collapse_nested_brackets: bool,
         wrap_pragma_comments: bool,
+        base_indentation_spaces: int,
+        other_line_continuation_extra_indent: bool,
+        use_tabs: bool,
+        tab_width: int,
         target_version: List[TargetVersion],
         check: bool,
         diff: bool,
         color: bool,
         fast: bool,
         pyi: bool,
         ipynb: bool,
@@ -630,14 +691,18 @@
         python_cell_magics=set(python_cell_magics),
         function_definition_extra_indent=function_definition_extra_indent,
         closing_bracket_extra_indent=closing_bracket_extra_indent,
         single_quote=single_quote,
         wrap_line_with_long_string=wrap_line_with_long_string,
         collapse_nested_brackets=collapse_nested_brackets,
         wrap_pragma_comments=wrap_pragma_comments,
+        base_indentation_spaces=base_indentation_spaces,
+        other_line_continuation_extra_indent=other_line_continuation_extra_indent,
+        use_tabs=use_tabs,
+        tab_width=tab_width,
     )
 
     if code is not None:
         # Run in quiet mode by default with -c; the extra output isn't useful.
         # You can still pass -v to get verbose output.
         quiet = True
```

### Comparing `cercis-0.1.4/src/cercis/_width_table.py` & `cercis-0.1.5/src/cercis/_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/brackets.py` & `cercis-0.1.5/src/cercis/brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/cache.py` & `cercis-0.1.5/src/cercis/cache.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/comments.py` & `cercis-0.1.5/src/cercis/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/concurrency.py` & `cercis-0.1.5/src/cercis/concurrency.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/debug.py` & `cercis-0.1.5/src/cercis/debug.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/files.py` & `cercis-0.1.5/src/cercis/files.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/handle_ipynb_magics.py` & `cercis-0.1.5/src/cercis/handle_ipynb_magics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/linegen.py` & `cercis-0.1.5/src/cercis/linegen.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from cercis.brackets import (
     COMMA_PRIORITY,
     DOT_PRIORITY,
     get_leaves_inside_matching_brackets,
     max_delimiter_priority_in_atom,
 )
 from cercis.comments import FMT_OFF, generate_comments, list_comments
+from cercis.indent import Indent
 from cercis.lines import (
     Line,
     RHSResult,
     append_leaves,
     can_be_split,
     can_omit_invisible_parens,
     is_line_short_enough,
@@ -97,39 +98,51 @@
 
     def __init__(self, mode: Mode, features: Collection[Feature]) -> None:
         self.mode = mode
         self.features = features
         self.current_line: Line
         self.__post_init__()
 
-    def line(self, indent: int = 0) -> Iterator[Line]:
+    def line(self, indent: Optional[Indent] = None) -> Iterator[Line]:
         """Generate a line.
 
         If the line is empty, only emit if it makes sense.
         If the line is too long, split it first and then generate.
 
         If any lines were generated, set up a new current_line.
         """
         if not self.current_line:
-            self.current_line.depth += indent
+            if indent is Indent.DEDENT:
+                self.current_line.depth = self.current_line.depth[:-1]
+            elif indent is not None:
+                self.current_line.depth += (indent,)
+
             return  # Line is empty, don't emit. Creating a new one unnecessary.
 
         if (
             Preview.improved_async_statements_handling in self.mode
             and len(self.current_line.leaves) == 1
             and is_async_stmt_or_funcdef(self.current_line.leaves[0])
         ):
             # Special case for async def/for/with statements. `visit_async_stmt`
             # adds an `ASYNC` leaf then visits the child def/for/with statement
             # nodes. Line yields from those nodes shouldn't treat the former
             # `ASYNC` leaf as a complete line.
             return
 
         complete_line = self.current_line
-        self.current_line = Line(mode=self.mode, depth=complete_line.depth + indent)
+
+        if indent is Indent.DEDENT:
+            new_depth = complete_line.depth[:-1]
+        elif indent is not None:
+            new_depth = complete_line.depth + (indent,)
+        else:
+            new_depth = complete_line.depth
+
+        self.current_line = Line(mode=self.mode, depth=new_depth)
         yield complete_line
 
     def visit_default(self, node: LN) -> Iterator[Line]:
         """Default `visit_*()` implementation. Recurses to children of `node`."""
         if isinstance(node, Leaf):
             any_open_brackets = self.current_line.bracket_tracker.any_open_brackets()
             for comment in generate_comments(node):
@@ -176,30 +189,30 @@
                 node.append_child(rpar)
 
         yield from self.visit_default(node)
 
     def visit_INDENT(self, node: Leaf) -> Iterator[Line]:
         """Increase indentation level, maybe yield a line."""
         # In blib2to3 INDENT never holds comments.
-        yield from self.line(+1)
+        yield from self.line(Indent.BLOCK)
         yield from self.visit_default(node)
 
     def visit_DEDENT(self, node: Leaf) -> Iterator[Line]:
         """Decrease indentation level, maybe yield a line."""
         # The current line might still wait for trailing comments.  At DEDENT time
         # there won't be any (they would be prefixes on the preceding NEWLINE).
         # Emit the line then.
         yield from self.line()
 
         # While DEDENT has no value, its prefix may contain standalone comments
         # that belong to the current indentation level.  Get 'em.
         yield from self.visit_default(node)
 
         # Finally, emit the dedent.
-        yield from self.line(-1)
+        yield from self.line(Indent.DEDENT)
 
     def visit_stmt(
             self, node: Node, keywords: Set[str], parens: Set[str]
     ) -> Iterator[Line]:
         """Visit a statement.
 
         This implementation is shared for `if`, `while`, `for`, `try`, `except`,
@@ -287,17 +300,17 @@
             prev_type = child.type
 
         is_suite_like = node.parent and node.parent.type in STATEMENT
         if is_suite_like:
             if self.mode.is_pyi and is_stub_body(node):
                 yield from self.visit_default(node)
             else:
-                yield from self.line(+1)
+                yield from self.line(Indent.BLOCK)
                 yield from self.visit_default(node)
-                yield from self.line(-1)
+                yield from self.line(Indent.DEDENT)
 
         else:
             if (
                 not self.mode.is_pyi
                 or not node.parent
                 or not is_stub_suite(node.parent)
             ):
@@ -413,15 +426,15 @@
             #   docstring = docstring.strip(quote_char)
             # but that breaks on """""x""" (which is '""x').
             # So we actually need to remove the first character and the next two
             # characters but only if they are the same as the first.
             quote_len = 1 if docstring[1] != quote_char else 3
             docstring = docstring[quote_len:-quote_len]
             docstring_started_empty = not docstring
-            indent = " " * 4 * self.current_line.depth
+            indent: str = self.current_line.render_indent_chars()
 
             if is_multiline_string(leaf):
                 docstring = fix_docstring(docstring, indent)
             else:
                 docstring = docstring.strip()
 
             has_trailing_backslash = False
@@ -942,22 +955,23 @@
 
     If it's the body component, the result line is one-indented inside brackets and as
     such has its first leaf's prefix normalized and a trailing comma added when
     expected.
     """
     result = Line(mode=original.mode, depth=original.depth)
 
-    if mode.function_definition_extra_indent and original.is_def:
-        additional_depth = 2
-    else:
-        additional_depth = 1
+    additional_indent = (
+        Indent.FUNCTION_DEF_CONTINUATION
+        if original.is_def
+        else Indent.OTHER_LINE_CONTINUATION
+    )
 
     if component is _BracketSplitComponent.body:
         result.inside_brackets = True
-        result.depth += additional_depth
+        result.depth = result.depth + (additional_indent,)
 
         if leaves:
             # Since body is a new indent level, remove spurious leading whitespace.
             normalize_prefix(leaves[0], inside_brackets=True)
             # Ensure a trailing comma for imports and standalone function arguments, but
             # be careful not to add one after any comments or within type annotations.
             no_commas = (
@@ -991,15 +1005,15 @@
                     break
 
     leaves_to_track: Set[LeafID] = set()
     if component is _BracketSplitComponent.head:
         leaves_to_track = get_leaves_inside_matching_brackets(leaves)
 
     if mode.closing_bracket_extra_indent and component is _BracketSplitComponent.tail:
-        result.depth += additional_depth
+        result.depth = result.depth + (additional_indent,)
 
     # Populate the line
     for leaf in leaves:
         result.append(
             leaf,
             preformatted=True,
             track_bracket=id(leaf) in leaves_to_track,
@@ -1512,15 +1526,15 @@
     the one that needs to explode are omitted.
     """
 
     omit: Set[LeafID] = set()
     if not line.magic_trailing_comma:
         yield omit
 
-    length = 4 * line.depth
+    length: int = line.calc_total_indent_width()
     opening_bracket: Optional[Leaf] = None
     closing_bracket: Optional[Leaf] = None
     inner_brackets: Set[LeafID] = set()
     for index, leaf, leaf_length in line.enumerate_with_length(reversed=True):
         length += leaf_length
         if length > line_length:
             break
```

### Comparing `cercis-0.1.4/src/cercis/lines.py` & `cercis-0.1.5/src/cercis/lines.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Union,
     cast,
 )
 
 from blib2to3.pgen2 import token
 from blib2to3.pytree import Leaf, Node
 from cercis.brackets import COMMA_PRIORITY, DOT_PRIORITY, BracketTracker
+from cercis.indent import Indent, MultipleIndents
 from cercis.mode import Mode, Preview
 from cercis.nodes import (
     BRACKETS,
     CLOSING_BRACKETS,
     OPENING_BRACKETS,
     STANDALONE_COMMENT,
     TEST_DESCENDANTS,
@@ -49,23 +50,29 @@
 
 
 @dataclass
 class Line:
     """Holds leaves and comments. Can be printed with `str(line)`."""
 
     mode: Mode
-    depth: int = 0
+    depth: Tuple[Indent, ...] = field(default_factory=tuple)
     leaves: List[Leaf] = field(default_factory=list)
     # keys ordered like `leaves`
     comments: Dict[LeafID, List[Leaf]] = field(default_factory=dict)
     bracket_tracker: BracketTracker = field(default_factory=BracketTracker)
     inside_brackets: bool = False
     should_split_rhs: bool = False
     magic_trailing_comma: Optional[Leaf] = None
 
+    def render_indent_chars(self, for_width_calculation: bool = False) -> str:
+        return self.all_indents.render(for_width_calculation)
+
+    def calc_total_indent_width(self) -> int:
+        return self.all_indents.calc_total_width()
+
     def append(
             self, leaf: Leaf, preformatted: bool = False, track_bracket: bool = False
     ) -> None:
         """Add a new `leaf` to the end of the line.
 
         Unless `preformatted` is True, the `leaf` will receive a new consistent
         whitespace prefix and metadata applied by :class:`BracketTracker`.
@@ -110,14 +117,19 @@
                 raise ValueError(
                     "cannot append standalone comments to a populated line"
                 )
 
         self.append(leaf, preformatted=preformatted)
 
     @property
+    def all_indents(self) -> MultipleIndents:
+        """All the indentations of this line"""
+        return MultipleIndents(indents=self.depth, mode=self.mode)
+
+    @property
     def is_comment(self) -> bool:
         """Is this line a standalone comment?"""
         return len(self.leaves) == 1 and self.leaves[0].type == STANDALONE_COMMENT
 
     @property
     def is_decorator(self) -> bool:
         """Is this line a decorator?"""
@@ -495,20 +507,26 @@
             mode=self.mode,
             depth=self.depth,
             inside_brackets=self.inside_brackets,
             should_split_rhs=self.should_split_rhs,
             magic_trailing_comma=self.magic_trailing_comma,
         )
 
+    def render_as_str_for_width_calculation(self) -> str:
+        return self._str_inner(for_width_calculation=True)
+
     def __str__(self) -> str:
         """Render the line."""
+        return self._str_inner(for_width_calculation=False)
+
+    def _str_inner(self, for_width_calculation: bool = False) -> str:
         if not self:
             return "\n"
 
-        indent = "    " * self.depth
+        indent: str = self.render_indent_chars(for_width_calculation)
         leaves = iter(self.leaves)
         first = next(leaves)
         res = f"{first.prefix}{indent}{first.value}"
         for leaf in leaves:
             res += str(leaf)
         for comment in itertools.chain.from_iterable(self.comments.values()):
             res += str(comment)
@@ -607,26 +625,26 @@
 
         self.previous_line = current_line
         self.previous_block = block
         return block
 
     def _maybe_empty_lines(self, current_line: Line) -> Tuple[int, int]:
         max_allowed = 1
-        if current_line.depth == 0:
+        if len(current_line.depth) == 0:
             max_allowed = 1 if self.mode.is_pyi else 2
         if current_line.leaves:
             # Consume the first leaf's extra newlines.
             first_leaf = current_line.leaves[0]
             before = first_leaf.prefix.count("\n")
             before = min(before, max_allowed)
             first_leaf.prefix = ""
         else:
             before = 0
         depth = current_line.depth
-        while self.previous_defs and self.previous_defs[-1].depth >= depth:
+        while self.previous_defs and len(self.previous_defs[-1].depth) >= len(depth):
             if self.mode.is_pyi:
                 assert self.previous_line is not None
                 if depth and not current_line.is_def and self.previous_line.is_def:
                     # Empty lines between attributes and methods should be preserved.
                     before = min(1, before)
                 elif (
                     Preview.blank_line_after_nested_stub_class in self.mode
@@ -665,15 +683,15 @@
             return self._maybe_empty_lines_for_class_or_def(current_line, before)
 
         if (
             self.previous_line
             and self.previous_line.is_import
             and not current_line.is_import
             and not current_line.is_fmt_pass_converted(first_leaf_matches=is_import)
-            and depth == self.previous_line.depth
+            and len(depth) == len(self.previous_line.depth)
         ):
             return (before or 1), 0
 
         if (
             self.previous_line
             and self.previous_line.is_class
             and current_line.is_triple_quoted_string
@@ -696,23 +714,23 @@
         if self.previous_line.is_decorator:
             if self.mode.is_pyi and current_line.is_stub_class:
                 # Insert an empty line after a decorated stub class
                 return 0, 1
 
             return 0, 0
 
-        if self.previous_line.depth < current_line.depth and (
+        if len(self.previous_line.depth) < len(current_line.depth) and (
             self.previous_line.is_class or self.previous_line.is_def
         ):
             return 0, 0
 
         comment_to_add_newlines: Optional[LinesBlock] = None
         if (
             self.previous_line.is_comment
-            and self.previous_line.depth == current_line.depth
+            and len(self.previous_line.depth) == len(current_line.depth)
             and before == 0
         ):
             slc = self.semantic_leading_comment
             if (
                 slc is not None
                 and slc.previous_block is not None
                 and not slc.previous_block.original_line.is_class
@@ -721,17 +739,17 @@
             ):
                 comment_to_add_newlines = slc
             else:
                 return 0, 0
 
         if self.mode.is_pyi:
             if current_line.is_class or self.previous_line.is_class:
-                if self.previous_line.depth < current_line.depth:
+                if len(self.previous_line.depth) < len(current_line.depth):
                     newlines = 0
-                elif self.previous_line.depth > current_line.depth:
+                elif len(self.previous_line.depth) > len(current_line.depth):
                     newlines = 1
                 elif current_line.is_stub_class and self.previous_line.is_stub_class:
                     # No blank line between classes with an empty body
                     newlines = 0
                 else:
                     newlines = 1
             elif (
@@ -741,15 +759,15 @@
                     # In classes empty lines between attributes and methods should
                     # be preserved.
                     newlines = min(1, before)
                 else:
                     # Blank line between a block of functions (maybe with preceding
                     # decorators) and a block of non-functions
                     newlines = 1
-            elif self.previous_line.depth > current_line.depth:
+            elif len(self.previous_line.depth) > len(current_line.depth):
                 newlines = 1
             else:
                 newlines = 0
         else:
             newlines = 1 if current_line.depth else 2
         if comment_to_add_newlines is not None:
             previous_block = comment_to_add_newlines.previous_block
@@ -800,14 +818,19 @@
     For multiline strings, looks at the context around `line` to determine
     if it should be inlined or split up.
     Uses the provided `line_str` rendering, if any, otherwise computes a new one.
     """
     if not line_str:
         line_str = line_to_string(line)
 
+    if mode.use_tabs:
+        # Override previous calculation of `line_str`, because we need
+        # to treat the width of '\t' as more than 1 character
+        line_str = line.render_as_str_for_width_calculation().strip("\n")
+
     width = str_width if mode.preview else len
     if mode.wrap_pragma_comments:  # Black's default
         effective_length = width(line_str)
     else:  # Cercis's default
         effective_length = width(line_str) - line.trailing_pragma_comment_length()
 
     if Preview.multiline_string_handling not in mode:
@@ -1007,15 +1030,15 @@
 
     return False
 
 
 def _can_omit_opening_paren(line: Line, *, first: Leaf, line_length: int) -> bool:
     """See `can_omit_invisible_parens`."""
     remainder = False
-    length = 4 * line.depth
+    length: int = line.calc_total_indent_width()
     _index = -1
     for _index, leaf, leaf_length in line.enumerate_with_length():
         if leaf.type in CLOSING_BRACKETS and leaf.opening_bracket is first:
             remainder = True
         if remainder:
             length += leaf_length
             if length > line_length:
@@ -1031,15 +1054,15 @@
             return True
 
     return False
 
 
 def _can_omit_closing_paren(line: Line, *, last: Leaf, line_length: int) -> bool:
     """See `can_omit_invisible_parens`."""
-    length = 4 * line.depth
+    length: int = line.calc_total_indent_width()
     seen_other_brackets = False
     for _index, leaf, leaf_length in line.enumerate_with_length():
         length += leaf_length
         if leaf is last.opening_bracket:
             if seen_other_brackets or length <= line_length:
                 return True
```

### Comparing `cercis-0.1.4/src/cercis/mode.py` & `cercis-0.1.5/src/cercis/mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,23 @@
 
 if sys.version_info < (3, 8):
     from typing_extensions import Final
 else:
     from typing import Final
 
 from cercis.const import (
+    DEFAULT_BASE_INDENTATION_SPACES,
     DEFAULT_CLOSING_BRACKET_EXTRA_INDENT,
     DEFAULT_COLLAPSE_NESTED_BRACKETS,
     DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     DEFAULT_LINE_LENGTH,
+    DEFAULT_OTHER_LINE_CONTINUATION_EXTRA_INDENT,
     DEFAULT_SINGLE_QUOTE,
+    DEFAULT_TAB_WIDTH,
+    DEFAULT_USE_TABS,
     DEFAULT_WRAP_LINE_WITH_LONG_STRING,
     DEFAULT_WRAP_PRAGMA_COMMENTS,
 )
 
 
 class TargetVersion(Enum):
     PY33 = 3
@@ -194,14 +198,20 @@
     preview: bool = False
     function_definition_extra_indent: bool = DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT
     closing_bracket_extra_indent: bool = DEFAULT_CLOSING_BRACKET_EXTRA_INDENT
     single_quote: bool = DEFAULT_SINGLE_QUOTE
     wrap_line_with_long_string: bool = DEFAULT_WRAP_LINE_WITH_LONG_STRING
     collapse_nested_brackets: bool = DEFAULT_COLLAPSE_NESTED_BRACKETS
     wrap_pragma_comments: bool = DEFAULT_WRAP_PRAGMA_COMMENTS
+    base_indentation_spaces: int = DEFAULT_BASE_INDENTATION_SPACES
+    other_line_continuation_extra_indent: bool = (
+        DEFAULT_OTHER_LINE_CONTINUATION_EXTRA_INDENT
+    )
+    use_tabs: bool = DEFAULT_USE_TABS
+    tab_width: int = DEFAULT_TAB_WIDTH
 
     def __post_init__(self) -> None:
         if self.experimental_string_processing:
             warn(
                 "`experimental string processing` has been included in `preview`"
                 " and deprecated. Use `preview` instead.",
                 Deprecated,
```

### Comparing `cercis-0.1.4/src/cercis/nodes.py` & `cercis-0.1.5/src/cercis/nodes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/numerics.py` & `cercis-0.1.5/src/cercis/numerics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/output.py` & `cercis-0.1.5/src/cercis/output.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/parsing.py` & `cercis-0.1.5/src/cercis/parsing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/report.py` & `cercis-0.1.5/src/cercis/report.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/rusty.py` & `cercis-0.1.5/src/cercis/rusty.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/strings.py` & `cercis-0.1.5/src/cercis/strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/trans.py` & `cercis-0.1.5/src/cercis/trans.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     Sequence,
     Set,
     Tuple,
     TypeVar,
     Union,
 )
 
+from cercis.indent import Indent
+
 if sys.version_info < (3, 8):
     from typing_extensions import Final, Literal
 else:
     from typing import Literal, Final
 
 from mypy_extensions import trait
 
@@ -1097,15 +1099,15 @@
         # Finally, we use the following convenience variables:
         #
         #   P:  The leaf that is before the target string leaf.
         #   N:  The leaf that is after the target string leaf.
         #   NN: The leaf that is after N.
 
         # WMA4 the whitespace at the beginning of the line.
-        offset = line.depth * 4
+        offset: int = line.calc_total_indent_width()
 
         if is_valid_index(string_idx - 1):
             p_idx = string_idx - 1
             if (
                 LL[string_idx - 1].type == token.LPAR
                 and LL[string_idx - 1].value == ""
                 and string_idx >= 2
@@ -1451,30 +1453,30 @@
             Returns:
                 The max allowed width of the string value used for the last
                 line we will construct.  Note that this value means the width
                 rather than the number of characters (e.g., many East Asian
                 characters expand to two columns).
             """
             result = self.line_length
-            result -= line.depth * 4
+            result -= line.calc_total_indent_width()
             result -= 1 if ends_with_comma else 0
             result -= string_op_leaves_length
             return result
 
         # --- Calculate Max Break Width (for string value)
         # We start with the line length limit
         max_break_width = self.line_length
         # The last index of a string of length N is N-1.
         max_break_width -= 1
         # Leading whitespace is not present in the string value (e.g. Leaf.value).
-        max_break_width -= line.depth * 4
+        max_break_width -= line.calc_total_indent_width()
         if max_break_width < 0:
             yield TErr(
                 f"Unable to split {LL[string_idx].value} at such high of a line depth:"
-                f" {line.depth}"
+                f" {line.calc_total_indent_width()}"
             )
             return
 
         # Check if StringMerger registered any custom splits.
         custom_splits = self.pop_custom_splits(LL[string_idx].value)
         # We use them ONLY if none of them would produce lines that exceed the
         # line limit.
@@ -1889,15 +1891,17 @@
         if string_idx is not None:
             string_value = line.leaves[string_idx].value
             # If the string has neither spaces nor East Asian stops...
             if not any(
                 char == " " or char in SPLIT_SAFE_CHARS for char in string_value
             ):
                 # And will still violate the line length limit when split...
-                max_string_width = self.line_length - ((line.depth + 1) * 4)
+                max_string_width: int = self.line_length - (
+                    (line.calc_total_indent_width() + 1) * 4
+                )
                 if str_width(string_value) > max_string_width:
                     # And has no associated custom splits...
                     if not self.has_custom_splits(string_value):
                         # Then we should NOT put this string on its own line.
                         return TErr(
                             "We do not wrap long strings in parentheses when the"
                             " resultant line would still be over the specified line"
@@ -2135,15 +2139,15 @@
 
         # --- Middle (String) Line
         # We only need to yield one (possibly too long) string line, since the
         # `StringSplitter` will break it down further if necessary.
         string_value = LL[string_idx].value
         string_line = Line(
             mode=line.mode,
-            depth=line.depth + 1,
+            depth=line.depth + (Indent.OTHER_LINE_CONTINUATION,),
             inside_brackets=True,
             should_split_rhs=line.should_split_rhs,
             magic_trailing_comma=line.magic_trailing_comma,
         )
         string_leaf = Leaf(token.STRING, string_value)
         insert_str_child(string_leaf)
         string_line.append(string_leaf)
```

### Comparing `cercis-0.1.4/src/cercis/utils_line_wrapping.py` & `cercis-0.1.5/src/cercis/utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/src/cercis/utils_linegen.py` & `cercis-0.1.5/src/cercis/utils_linegen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/optional.py` & `cercis-0.1.5/tests/optional.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/test_black.py` & `cercis-0.1.5/tests/test_black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/test_blackd.py` & `cercis-0.1.5/tests/test_blackd.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/test_format.py` & `cercis-0.1.5/tests/test_format.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import itertools
 import re
 from dataclasses import replace
 from typing import Any, Iterator
 from unittest.mock import patch
 
 import pytest
 
@@ -334,7 +335,103 @@
         ("Cercis_default.py", False),
         ("Black_default.py", True),
     ],
 )
 def test_wrap_pragma_comments(filename: str, wrap: bool) -> None:
     mode = replace(DEFAULT_MODE, wrap_pragma_comments=wrap, line_length=80)
     check_file("configurable_cases/pragma_comments", filename, mode)
+
+
+@pytest.mark.parametrize(
+    "closing_bracket_extra_indent, base_indent_spaces, fdei, olcei",
+    list(
+        itertools.product(  # each list here corresponds to 1 argument above
+            [False, True],
+            [1, 2, 3, 4, 8],
+            [False, True],
+            [False, True],
+        )
+    ),
+)
+def test_indent_levels__use_spaces(
+        closing_bracket_extra_indent: bool,
+        base_indent_spaces: int,
+        fdei: bool,
+        olcei: bool,
+) -> None:
+    mode = replace(
+        DEFAULT_MODE,
+        line_length=80,
+        base_indentation_spaces=base_indent_spaces,
+        function_definition_extra_indent=fdei,
+        other_line_continuation_extra_indent=olcei,
+        closing_bracket_extra_indent=closing_bracket_extra_indent,
+    )
+    parent_folder = "configurable_cases/indentation/use_spaces"
+    folder = (
+        f"{parent_folder}/closing_bracket_extra_indent"
+        if closing_bracket_extra_indent
+        else f"{parent_folder}/closing_bracket_no_extra_indent"
+    )
+    check_file(
+        f"{folder}/base_indent_spaces={base_indent_spaces}",
+        f"fdei={fdei}_olcei={olcei}",
+        mode,
+    )
+
+
+@pytest.mark.parametrize(
+    "closing_bracket_extra_indent, fdei, olcei",
+    list(
+        itertools.product(  # each list here corresponds to 1 argument above
+            [False, True],
+            [False, True],
+            [False, True],
+        )
+    ),
+)
+def test_indent_levels__use_tabs(
+        closing_bracket_extra_indent: bool,
+        fdei: bool,
+        olcei: bool,
+) -> None:
+    mode = replace(
+        DEFAULT_MODE,
+        line_length=80,
+        use_tabs=True,
+        function_definition_extra_indent=fdei,
+        other_line_continuation_extra_indent=olcei,
+        closing_bracket_extra_indent=closing_bracket_extra_indent,
+    )
+    parent_folder = "use_tabs"
+    folder = (
+        f"{parent_folder}/closing_bracket_extra_indent"
+        if closing_bracket_extra_indent
+        else f"{parent_folder}/closing_bracket_no_extra_indent"
+    )
+    check_file(
+        f"configurable_cases/indentation/{folder}",
+        f"fdei={fdei}_olcei={olcei}",
+        mode,
+    )
+
+
+@pytest.mark.parametrize(
+    "tab_width",
+    [1, 2, 3, 4, 5, 8],
+)
+def test_line_length_calculation_with_tabs(tab_width: int) -> None:
+    mode = replace(
+        DEFAULT_MODE,
+        line_length=80,
+        use_tabs=True,
+        tab_width=tab_width,
+        function_definition_extra_indent=False,
+        other_line_continuation_extra_indent=False,
+        closing_bracket_extra_indent=False,
+    )
+    filename = f"tab_width_{tab_width}"
+    check_file(
+        "configurable_cases/indentation/use_tabs/line_length_calculation",
+        filename,
+        mode,
+    )
```

### Comparing `cercis-0.1.4/tests/test_ipynb.py` & `cercis-0.1.5/tests/test_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/test_no_ipynb.py` & `cercis-0.1.5/tests/test_no_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/test_trans.py` & `cercis-0.1.5/tests/test_trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/test_utils_line_wrapping.py` & `cercis-0.1.5/tests/test_utils_line_wrapping.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/util.py` & `cercis-0.1.5/tests/util.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/conditional_expression.py` & `cercis-0.1.5/tests/data/conditional_expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py` & `cercis-0.1.5/tests/data/configurable_cases/closing_bracket_indent/extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py` & `cercis-0.1.5/tests/data/configurable_cases/closing_bracket_indent/no_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py` & `cercis-0.1.5/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py` & `cercis-0.1.5/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/edge_cases.py` & `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/edge_cases.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py` & `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py` & `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py` & `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py` & `cercis-0.1.5/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py` & `cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py` & `cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py` & `cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py` & `cercis-0.1.5/tests/data/configurable_cases/nested_brackets/nested_brackets_explodes__Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/pragma_comments/Black_default.py` & `cercis-0.1.5/tests/data/configurable_cases/pragma_comments/Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/pragma_comments/Cercis_default.py` & `cercis-0.1.5/tests/data/configurable_cases/pragma_comments/Cercis_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring.py` & `cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/single_quote/docstring_preview.py` & `cercis-0.1.5/tests/data/configurable_cases/single_quote/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/single_quote/more_quotes.py` & `cercis-0.1.5/tests/data/configurable_cases/single_quote/more_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/single_quote/string_prefixes.py` & `cercis-0.1.5/tests/data/configurable_cases/single_quote/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/configurable_cases/single_quote/torture.py` & `cercis-0.1.5/tests/data/configurable_cases/single_quote/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/jupyter/notebook_no_trailing_newline.ipynb` & `cercis-0.1.5/tests/data/jupyter/notebook_no_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/jupyter/notebook_trailing_newline.ipynb` & `cercis-0.1.5/tests/data/jupyter/notebook_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/jupyter/notebook_without_changes.ipynb` & `cercis-0.1.5/tests/data/jupyter/notebook_without_changes.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/debug_visitor.out` & `cercis-0.1.5/tests/data/miscellaneous/debug_visitor.out`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/debug_visitor.py` & `cercis-0.1.5/tests/data/miscellaneous/debug_visitor.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/decorators.py` & `cercis-0.1.5/tests/data/miscellaneous/decorators.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/docstring_no_string_normalization.py` & `cercis-0.1.5/tests/data/miscellaneous/docstring_no_string_normalization.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff` & `cercis-0.1.5/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/force_py36.py` & `cercis-0.1.5/tests/data/miscellaneous/force_py36.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/force_pyi.py` & `cercis-0.1.5/tests/data/miscellaneous/force_pyi.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/long_strings_flag_disabled.py` & `cercis-0.1.5/tests/data/miscellaneous/long_strings_flag_disabled.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/python2_detection.py` & `cercis-0.1.5/tests/data/miscellaneous/python2_detection.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/string_quotes.py` & `cercis-0.1.5/tests/data/miscellaneous/string_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/miscellaneous/stub.pyi` & `cercis-0.1.5/tests/data/miscellaneous/stub.pyi`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/cantfit.py` & `cercis-0.1.5/tests/data/preview/cantfit.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/comments7.py` & `cercis-0.1.5/tests/data/preview/comments7.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/format_unicode_escape_seq.py` & `cercis-0.1.5/tests/data/preview/format_unicode_escape_seq.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/long_dict_values.py` & `cercis-0.1.5/tests/data/preview/long_dict_values.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/long_strings.py` & `cercis-0.1.5/tests/data/preview/long_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/long_strings__east_asian_width.py` & `cercis-0.1.5/tests/data/preview/long_strings__east_asian_width.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/long_strings__edge_case.py` & `cercis-0.1.5/tests/data/preview/long_strings__edge_case.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/long_strings__regression.py` & `cercis-0.1.5/tests/data/preview/long_strings__regression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/long_strings__type_annotations.py` & `cercis-0.1.5/tests/data/preview/long_strings__type_annotations.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/multiline_strings.py` & `cercis-0.1.5/tests/data/preview/multiline_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/prefer_rhs_split.py` & `cercis-0.1.5/tests/data/preview/prefer_rhs_split.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview/trailing_comma.py` & `cercis-0.1.5/tests/data/preview/trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview_context_managers/targeting_py38.py` & `cercis-0.1.5/tests/data/preview_context_managers/targeting_py38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview_context_managers/targeting_py39.py` & `cercis-0.1.5/tests/data/preview_context_managers/targeting_py39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_10.py` & `cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_10.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_11.py` & `cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_11.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_8.py` & `cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/preview_context_managers/auto_detect/features_3_9.py` & `cercis-0.1.5/tests/data/preview_context_managers/auto_detect/features_3_9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_310/parenthesized_context_managers.py` & `cercis-0.1.5/tests/data/py_310/parenthesized_context_managers.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_310/pattern_matching_complex.py` & `cercis-0.1.5/tests/data/py_310/pattern_matching_complex.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_310/pattern_matching_extras.py` & `cercis-0.1.5/tests/data/py_310/pattern_matching_extras.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_310/pattern_matching_generic.py` & `cercis-0.1.5/tests/data/py_310/pattern_matching_generic.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_310/pattern_matching_simple.py` & `cercis-0.1.5/tests/data/py_310/pattern_matching_simple.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_310/pattern_matching_style.py` & `cercis-0.1.5/tests/data/py_310/pattern_matching_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_311/pep_646.py` & `cercis-0.1.5/tests/data/py_311/pep_646.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_311/pep_654.py` & `cercis-0.1.5/tests/data/py_311/pep_654.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_311/pep_654_style.py` & `cercis-0.1.5/tests/data/py_311/pep_654_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_36/numeric_literals.py` & `cercis-0.1.5/tests/data/py_36/numeric_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_37/python37.py` & `cercis-0.1.5/tests/data/py_37/python37.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_38/pep_570.py` & `cercis-0.1.5/tests/data/py_38/pep_570.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_38/pep_572.py` & `cercis-0.1.5/tests/data/py_38/pep_572.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_38/pep_572_remove_parens.py` & `cercis-0.1.5/tests/data/py_38/pep_572_remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_38/python38.py` & `cercis-0.1.5/tests/data/py_38/python38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_39/python39.py` & `cercis-0.1.5/tests/data/py_39/python39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/py_39/remove_with_brackets.py` & `cercis-0.1.5/tests/data/py_39/remove_with_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/attribute_access_on_number_literals.py` & `cercis-0.1.5/tests/data/simple_cases/attribute_access_on_number_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/class_blank_parentheses.py` & `cercis-0.1.5/tests/data/simple_cases/class_blank_parentheses.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/class_methods_new_line.py` & `cercis-0.1.5/tests/data/simple_cases/class_methods_new_line.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/collections.py` & `cercis-0.1.5/tests/data/simple_cases/collections.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/comments.py` & `cercis-0.1.5/tests/data/simple_cases/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/comments2.py` & `cercis-0.1.5/tests/data/simple_cases/comments2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/comments3.py` & `cercis-0.1.5/tests/data/simple_cases/comments3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/comments4.py` & `cercis-0.1.5/tests/data/simple_cases/comments4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/comments5.py` & `cercis-0.1.5/tests/data/simple_cases/comments5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/comments6.py` & `cercis-0.1.5/tests/data/simple_cases/comments6.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/comments9.py` & `cercis-0.1.5/tests/data/simple_cases/comments9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/comments_non_breaking_space.py` & `cercis-0.1.5/tests/data/simple_cases/comments_non_breaking_space.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/composition.py` & `cercis-0.1.5/tests/data/simple_cases/composition.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/composition_no_trailing_comma.py` & `cercis-0.1.5/tests/data/simple_cases/composition_no_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/docstring.py` & `cercis-0.1.5/tests/data/simple_cases/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/docstring_preview.py` & `cercis-0.1.5/tests/data/simple_cases/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/empty_lines.py` & `cercis-0.1.5/tests/data/simple_cases/empty_lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/expression.diff` & `cercis-0.1.5/tests/data/simple_cases/expression.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/expression.py` & `cercis-0.1.5/tests/data/simple_cases/expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/fmtonoff.py` & `cercis-0.1.5/tests/data/simple_cases/fmtonoff.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/fmtonoff2.py` & `cercis-0.1.5/tests/data/simple_cases/fmtonoff2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/fmtonoff5.py` & `cercis-0.1.5/tests/data/simple_cases/fmtonoff5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/fmtskip2.py` & `cercis-0.1.5/tests/data/simple_cases/fmtskip2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/fmtskip8.py` & `cercis-0.1.5/tests/data/simple_cases/fmtskip8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/fstring.py` & `cercis-0.1.5/tests/data/simple_cases/fstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/function.py` & `cercis-0.1.5/tests/data/simple_cases/function.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/function2.py` & `cercis-0.1.5/tests/data/simple_cases/function2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/function_trailing_comma.py` & `cercis-0.1.5/tests/data/simple_cases/function_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/import_spacing.py` & `cercis-0.1.5/tests/data/simple_cases/import_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/one_element_subscript.py` & `cercis-0.1.5/tests/data/simple_cases/one_element_subscript.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/power_op_spacing.py` & `cercis-0.1.5/tests/data/simple_cases/power_op_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/prefer_rhs_split_reformatted.py` & `cercis-0.1.5/tests/data/simple_cases/prefer_rhs_split_reformatted.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/remove_await_parens.py` & `cercis-0.1.5/tests/data/simple_cases/remove_await_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/remove_except_parens.py` & `cercis-0.1.5/tests/data/simple_cases/remove_except_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/remove_for_brackets.py` & `cercis-0.1.5/tests/data/simple_cases/remove_for_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/remove_newline_after_code_block_open.py` & `cercis-0.1.5/tests/data/simple_cases/remove_newline_after_code_block_open.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/remove_parens.py` & `cercis-0.1.5/tests/data/simple_cases/remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/return_annotation_brackets.py` & `cercis-0.1.5/tests/data/simple_cases/return_annotation_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/skip_magic_trailing_comma.py` & `cercis-0.1.5/tests/data/simple_cases/skip_magic_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/slices.py` & `cercis-0.1.5/tests/data/simple_cases/slices.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/string_prefixes.py` & `cercis-0.1.5/tests/data/simple_cases/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/torture.py` & `cercis-0.1.5/tests/data/simple_cases/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens1.py` & `cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/trailing_comma_optional_parens3.py` & `cercis-0.1.5/tests/data/simple_cases/trailing_comma_optional_parens3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/tests/data/simple_cases/trailing_commas_in_leading_parts.py` & `cercis-0.1.5/tests/data/simple_cases/trailing_commas_in_leading_parts.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/LICENSE` & `cercis-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/LICENSE_ORIGINAL` & `cercis-0.1.5/LICENSE_ORIGINAL`

 * *Files identical despite different names*

### Comparing `cercis-0.1.4/pyproject.toml` & `cercis-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 [build-system]
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cercis"
-version = "0.1.4"
+version = "0.1.5"
 description = "A more configurable Python code formatter"
 license = { text = "MIT" }
 requires-python = ">=3.7"
 authors = [
   { name = "Łukasz Langa", email = "lukasz@langa.pl" },
   { name = "jsh9", email = "" },
 ]
```

### Comparing `cercis-0.1.4/PKG-INFO` & `cercis-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cercis
-Version: 0.1.4
+Version: 0.1.5
 Summary: A more configurable Python code formatter
 Project-URL: Changelog, https://github.com/jsh9/cercis/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/jsh9/cercis
 Author: jsh9
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 License-File: LICENSE
@@ -40,29 +40,38 @@
 Provides-Extra: jupyter
 Requires-Dist: ipython>=7.8.0; extra == 'jupyter'
 Requires-Dist: tokenize-rt>=3.2.0; extra == 'jupyter'
 Provides-Extra: uvloop
 Requires-Dist: uvloop>=0.15.2; extra == 'uvloop'
 Description-Content-Type: text/markdown
 
-# Cercis
+# _Cercis_
 
 [![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Red_bud_2009.jpg/320px-Red_bud_2009.jpg)](https://en.wikipedia.org/wiki/Cercis)
 
 _**Cercis**_ /ˈsɜːrsɪs/ is a Python code formatter that is more configurable
 than [Black](https://github.com/psf/black) (a popular Python code formatter).
 
 [_Cercis_](https://en.wikipedia.org/wiki/Cercis) is also the name of a
 deciduous tree that boasts vibrant pink to purple-hued flowers, which bloom in
 early spring.
 
 This code repository is forked from and directly inspired by
 [Black](https://github.com/psf/black). The original license of Black is
 included in this repository (see [LICENSE_ORIGINAL](./LICENSE_ORIGINAL)).
 
+_Cercis_ inherited Black's very comprehensive test cases, which means we are
+confident that our configurability addition does not introduce any undesirable
+side effects. We also thoroughly tested every configurable options that we
+added.
+
+In particular, via its configurable options, _Cercis_ can completely fall back
+to Black. See [Section 4.5](#45-how-to-fall-back-to-blacks-behavior) below for
+more details.
+
 ## 1. Motivations
 
 While we like the idea of auto-formatting and code readability, we take issue
 with some style choices and the lack of configurability of the Black formatter.
 Therefore, _Cercis_ aims at providing some configurability beyond Black's
 limited offering.
 
@@ -130,19 +139,23 @@
 The main difference is that _Cercis_ provides several configurable options that
 Black doesn't. Configurability is our main motivation behind creating _Cercis_.
 
 _Cercis_ offers the following configurable options:
 
 1. [Line length](#31-line-length)
 2. [Single quote vs double quote](#32-single-quote-vs-double-quote)
-3. [Extra indentation at function definition](#33-extra-indentation-at-function-definition)
-4. [Extra indentation at closing brackets](#34-closing-bracket-indentation)
-5. ["Simple" lines with long strings](#35-simple-lines-with-long-strings)
-6. [Collapse nested brackets](#36-collapse-nested-brackets)
-7. [Wrap pragma comments](#37-wrapping-long-lines-ending-with-pragma-comments)
+3. [Tabs vs spaces](#33-tabs-vs-spaces)
+4. [Base indentation spaces](#34-base-indentation-spaces)
+5. [Extra indentation at line continuation](#35-extra-indentation-at-line-continuation)
+   1. [At function definition](#351-at-function-definition---function-definition-extra-indent)
+   2. [In other line continuations](#352-in-other-line-continuations---other-line-continuation-extra-indent)
+   3. [At closing brackets](#353-at-closing-brackets---closing-bracket-extra-indent)
+6. ["Simple" lines with long strings](#36-simple-lines-with-long-strings)
+7. [Collapse nested brackets](#37-collapse-nested-brackets)
+8. [Wrap pragma comments](#38-wrapping-long-lines-ending-with-pragma-comments)
 
 The next section ([How to configure _Cercis_](#4-how-to-configure-cercis))
 contains detailed instructions of how to configure these options.
 
 ### 3.1. Line length
 
 _Cercis_ uses 79 characters as the line length limit, instead of 88 (Black's
@@ -173,15 +186,82 @@
 | Abbreviation           | `-sq`                                        |
 | Default                | `True`                                       |
 | Black's default        | `False`                                      |
 | Command line usage     | `cercis -sq=True myScript.py`                |
 | `pyproject.toml` usage | `single-quote = false` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--single-quote=False]`               |
 
-### 3.3. Extra indentation at function definition
+### 3.3. Tabs vs spaces
+
+_Cercis_ offers users the ability to use tabs rather than spaces.
+
+There are two associated options:
+
+- `--use-tabs` (bool): whether to use tabs or spaces to format the code
+
+| Option                 |                                          |
+| ---------------------- | ---------------------------------------- |
+| Name                   | `--use-tabs`                             |
+| Abbreviation           | `-tab`                                   |
+| Default                | `False`                                  |
+| Black's default        | `False`                                  |
+| Command line usage     | `cercis -tab=True myScript.py`           |
+| `pyproject.toml` usage | `use-tabs = false` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--use-tabs=False]`               |
+
+- `--tab-width` (int): when calculating line length (to determine whether to
+  wrap lines), how wide shall _Cercis_ treat each tab. Only effective when
+  `--use-tabs` is set to `True`.
+
+| Option                 |                                       |
+| ---------------------- | ------------------------------------- |
+| Name                   | `--tab-width`                         |
+| Abbreviation           | `-tw`                                 |
+| Default                | 4                                     |
+| Black's default        | N/A                                   |
+| Command line usage     | `cercis -tab=True -tw=2 myScript.py`  |
+| `pyproject.toml` usage | `tab-width = 2` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--tab-width=2]`               |
+
+### 3.4. Base indentation spaces
+
+This option defines the number of spaces that each indentation level adds. This
+option has no effect when `--use-tabs` is set to `True`.
+
+For example, if you set it to 2, contents within a `for` block is indented 2
+spaces:
+
+```python
+for i in (1, 2, 3, 4, 5):
+  print(i)
+```
+
+| Option                 |                                                     |
+| ---------------------- | --------------------------------------------------- |
+| Name                   | `--base-indentation-spaces`                         |
+| Abbreviation           | `-bis`                                              |
+| Default                | 4                                                   |
+| Black's default        | 4                                                   |
+| Command line usage     | `cercis -bis=True -tw=2 myScript.py`                |
+| `pyproject.toml` usage | `base-indentation-spaces = 2` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--base-indentation-spaces=2]`               |
+
+### 3.5. Extra indentation at line continuations
+
+There are three associated options:
+
+- `--function-definition-extra-indent`
+- `--other-line-continuation-extra-indent`
+- `--closing-bracket-extra-indent`
+
+They control whether we add an **additional** indentation level in some
+situations. Note that these options can work well with tabs
+(`--use-tabs=True`).
+
+#### 3.5.1. At function definition (`--function-definition-extra-indent`)
 
 <table>
   <tr>
     <td>
 
 ```python
 # Cercis's default style
@@ -210,32 +290,80 @@
 ```
 
   </td>
 
   </tr>
 </table>
 
-We choose to indent an extra 4 spaces (8 in total) because it adds a clear
-visual separation between the function name and the argument list. Not adding
-extra indentation is also called out as wrong in the the official
-[PEP8 style guide](https://peps.python.org/pep-0008/#indentation).
+We choose to add an extra indentation level when wrapping a function signature
+line. This is because `def␣` happens to be 4 characters, so when the base
+indentation is 4 spaces, it can be difficult to visually distinguish the
+function name and the argument list if we don't add an extra indentation.
 
-You can override this default if necessary.
+If you set `--base-indentation-spaces` to other values than 4, this visual
+separation issue will disappear, and you may not need to turn this option on.
+
+This style is encouraged
+[in PEP8](https://peps.python.org/pep-0008/#indentation).
 
 | Option                 |                                                                 |
 | ---------------------- | --------------------------------------------------------------- |
 | Name                   | `--function-definition-extra-indent`                            |
 | Abbreviation           | `-fdei`                                                         |
 | Default                | `True`                                                          |
 | Black's default        | `False`                                                         |
 | Command line usage     | `cercis -fdei=False myScript.py`                                |
 | `pyproject.toml` usage | `function-definition-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--function-definition-extra-indent=False]`              |
 
-## 3.4. Closing bracket indentation
+#### 3.5.2. In other line continuations (`--other-line-continuation-extra-indent`)
+
+"Other line continuations" are cases other than in function definitions, such
+as:
+
+```python
+var = some_function(
+    arg1_with_long_name,
+    arg2_with_longer_name,
+)
+
+var2 = [
+    'something',
+    'something else',
+    'something more',
+]
+```
+
+So if you set this option (`--other-line-continuation-extra-indent`) to `True`,
+you can add an extra level of indentation in these cases:
+
+```python
+var = some_function(
+        arg1_with_long_name,
+        arg2_with_longer_name,
+)
+
+var2 = [
+        'something',
+        'something else',
+        'something more',
+]
+```
+
+| Option                 |                                                                     |
+| ---------------------- | ------------------------------------------------------------------- |
+| Name                   | `--other-line-continuation-extra-indent`                            |
+| Abbreviation           | `-olcei`                                                            |
+| Default                | `False`                                                             |
+| Black's default        | `False`                                                             |
+| Command line usage     | `cercis -olcei=True myScript.py`                                    |
+| `pyproject.toml` usage | `other-line-continuation-extra-indent = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [----other-line-continuation-extra-indent=False]`            |
+
+#### 3.5.3. At closing brackets (`--closing-bracket-extra-indent`)
 
 This option lets people customize where the closing bracket should be. Note
 that both styles are OK according to
 [PEP8](https://peps.python.org/pep-0008/#indentation).
 
 <table>
   <tr>
@@ -306,15 +434,15 @@
 | Abbreviation           | `-cbei`                                                     |
 | Default                | `False`                                                     |
 | Black's default        | `False`                                                     |
 | Command line usage     | `cercis -cbei=True myScript.py`                             |
 | `pyproject.toml` usage | `closing-bracket-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--closing-bracket-extra-indent=False]`              |
 
-### 3.5. "Simple" lines with long strings
+### 3.6. "Simple" lines with long strings
 
 By default, Black wraps lines that exceed length limit. But for very simple
 lines (such as assigning a long string to a variable), line wrapping is not
 necessary.
 
 <table>
   <tr>
@@ -373,15 +501,15 @@
 | Abbreviation           | `-wl`                                                     |
 | Default                | `False`                                                   |
 | Black's default        | `True`                                                    |
 | Command line usage     | `cercis -wl=True myScript.py`                             |
 | `pyproject.toml` usage | `wrap-line-with-long-string = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--wrap-line-with-long-string=False]`              |
 
-### 3.6. Collapse nested brackets
+### 3.7. Collapse nested brackets
 
 _Cercis_ by default collapses nested brackets to make the code more compact.
 
 <table>
   <tr>
     <td>
 
@@ -449,15 +577,15 @@
 | Command line usage     | `cercis -cnb=True myScript.py`                          |
 | `pyproject.toml` usage | `collapse-nested-brackets = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--collapse-nested-brackets=False]`              |
 
 The code implementation of this option comes from
 [Pyink](https://github.com/google/pyink), another forked project from Black.
 
-### 3.7. Wrapping long lines ending with pragma comments [^](#3-cerciss-code-style)
+### 3.8. Wrapping long lines ending with pragma comments
 
 "Pragma comments", in this context, mean the directives for Python linters
 usually to tell them to ignore certain errors. Pragma comments that _Cercis_
 currently recognizes include:
 
 - _noqa_: `# noqa: E501`
 - _type: ignore_: `# type: ignore[no-untyped-def]`
@@ -579,20 +707,42 @@
 means to always use the latest (including unreleased) _Cercis_ features.
 
 ### 4.4. Specify options in `tox.ini`
 
 Currently, _Cercis_ does not support a config section in `tox.ini`. Instead,
 you can specify the options in `pyproject.toml`.
 
-### 4.5. How to reproduce Black's behavior
+### 4.5. How to fall back to Black's behavior
 
-If you'd like to reproduce Black's behavior, simply set all the configurable
-options in [Section 3](#3-cerciss-code-style) to Black's default values.
+Here are the configuration options to fall back to Black's behavior. Put them
+in `pyproject.toml`:
+
+```toml
+[tool.cercis]
+line-length = 88
+single-quote = false
+use-tabs = false
+base-indentation-spaces = 4
+function-definition-extra-indent = false
+other-line-continuation-extra-indent = false
+closing-bracket-extra-indent = false
+wrap-line-with-long-string = true
+collapse-nested-brackets = false
+wrap-pragma-comments = true
+```
 # Change Log
 
+## [0.1.5] - 2023-05-09
+
+- Added
+  - Configurability to use tabs instead of spaces (two new options:
+    `--use-tabs` and `--tab-width`)
+  - Configurability on base indentation spaces and extra indentation at
+    different line continuation situations
+
 ## [0.1.4] - 2023-05-07
 
 - Added
   - A new configurable option: `--closing-bracket-extra-indent`
 
 ## [0.1.3] - 2023-05-07
```

