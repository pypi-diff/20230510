# Comparing `tmp/pontos-23.5.1.tar.gz` & `tmp/pontos-23.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pontos-23.5.1.tar", max compression
+gzip compressed data, was "pontos-23.5.2.tar", max compression
```

## Comparing `pontos-23.5.1.tar` & `pontos-23.5.2.tar`

### file list

```diff
@@ -1,251 +1,251 @@
--rw-r--r--   0        0        0    35149 2023-05-09 06:59:43.236978 pontos-23.5.1/LICENSE
--rw-r--r--   0        0        0     3836 2023-05-09 06:59:43.236978 pontos-23.5.1/README.md
--rw-r--r--   0        0        0    97053 2023-05-09 06:59:43.240978 pontos-23.5.1/poetry.lock
--rw-r--r--   0        0        0       32 2023-05-09 06:59:43.240978 pontos-23.5.1/poetry.toml
--rw-r--r--   0        0        0      791 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/__init__.py
--rw-r--r--   0        0        0      968 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/changelog/__init__.py
--rw-r--r--   0        0        0     9914 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/changelog/conventional_commits.py
--rw-r--r--   0        0        0      965 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/changelog/errors.py
--rw-r--r--   0        0        0     4393 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/changelog/main.py
--rw-r--r--   0        0        0      806 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/errors.py
--rw-r--r--   0        0        0      882 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/git/__init__.py
--rw-r--r--   0        0        0    16153 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/git/git.py
--rw-r--r--   0        0        0     2538 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/git/status.py
--rw-r--r--   0        0        0      760 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/__init__.py
--rw-r--r--   0        0        0     1154 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/__init__.py
--rw-r--r--   0        0        0     2239 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/argparser.py
--rw-r--r--   0        0        0     1472 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/cmds.py
--rw-r--r--   0        0        0     7327 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/core.py
--rw-r--r--   0        0        0     2426 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/env.py
--rw-r--r--   0        0        0      861 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/errors.py
--rw-r--r--   0        0        0     4173 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/event.py
--rw-r--r--   0        0        0     1100 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/actions/main.py
--rw-r--r--   0        0        0     2047 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/api/__init__.py
--rw-r--r--   0        0        0     5531 2023-05-09 06:59:43.240978 pontos-23.5.1/pontos/github/api/api.py
--rw-r--r--   0        0        0     6196 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/artifacts.py
--rw-r--r--   0        0        0    34561 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/branch.py
--rw-r--r--   0        0        0     9395 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/client.py
--rw-r--r--   0        0        0     1844 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/contents.py
--rw-r--r--   0        0        0      845 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/errors.py
--rw-r--r--   0        0        0     1320 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/helper.py
--rw-r--r--   0        0        0     2813 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/labels.py
--rw-r--r--   0        0        0    10311 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/organizations.py
--rw-r--r--   0        0        0    13090 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/pull_requests.py
--rw-r--r--   0        0        0    11942 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/release.py
--rw-r--r--   0        0        0    21512 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/repositories.py
--rw-r--r--   0        0        0     3276 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/search.py
--rw-r--r--   0        0        0     6004 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/tags.py
--rw-r--r--   0        0        0    15207 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/teams.py
--rw-r--r--   0        0        0     9182 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/api/workflows.py
--rw-r--r--   0        0        0    11128 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/argparser.py
--rw-r--r--   0        0        0     8863 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/cmds.py
--rw-r--r--   0        0        0     1347 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/main.py
--rw-r--r--   0        0        0     1114 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/__init__.py
--rw-r--r--   0        0        0     2336 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/artifact.py
--rw-r--r--   0        0        0     7532 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/base.py
--rw-r--r--   0        0        0     6915 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/branch.py
--rw-r--r--   0        0        0    16573 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/organization.py
--rw-r--r--   0        0        0    14248 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/pull_request.py
--rw-r--r--   0        0        0     4607 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/release.py
--rw-r--r--   0        0        0     4299 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/search.py
--rw-r--r--   0        0        0     4606 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/tag.py
--rw-r--r--   0        0        0    11477 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/models/workflow.py
--rw-r--r--   0        0        0      790 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/pr_template.md
--rw-r--r--   0        0        0     3207 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/script/__init__.py
--rw-r--r--   0        0        0      835 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/script/errors.py
--rw-r--r--   0        0        0     4854 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/script/load.py
--rw-r--r--   0        0        0     1495 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/github/script/parser.py
--rw-r--r--   0        0        0    14685 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/helper.py
--rw-r--r--   0        0        0     6211 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/models/__init__.py
--rw-r--r--   0        0        0      821 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/__init__.py
--rw-r--r--   0        0        0     4660 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/api.py
--rw-r--r--   0        0        0     2149 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/cpe/__init__.py
--rw-r--r--   0        0        0     6708 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/cpe/api.py
--rw-r--r--   0        0        0     2618 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/cve/__init__.py
--rw-r--r--   0        0        0    10802 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/cve/api.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/__init__.py
--rw-r--r--   0        0        0     2973 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/cpe.py
--rw-r--r--   0        0        0     7250 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/cve.py
--rw-r--r--   0        0        0     3254 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/cvss_v2.py
--rw-r--r--   0        0        0     4471 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/nvd/models/cvss_v3.py
--rw-r--r--   0        0        0     3561 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/pontos.py
--rw-r--r--   0        0        0        0 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/py.typed
--rw-r--r--   0        0        0     1164 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/release/__init__.py
--rw-r--r--   0        0        0     2472 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/release/helper.py
--rw-r--r--   0        0        0     2127 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/release/main.py
--rw-r--r--   0        0        0     8333 2023-05-09 06:59:43.244978 pontos-23.5.1/pontos/release/parser.py
--rw-r--r--   0        0        0    14408 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/release/release.py
--rw-r--r--   0        0        0    12499 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/release/sign.py
--rw-r--r--   0        0        0      886 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/terminal/__init__.py
--rw-r--r--   0        0        0     1770 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/terminal/null.py
--rw-r--r--   0        0        0     4717 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/terminal/rich.py
--rw-r--r--   0        0        0     9416 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/terminal/terminal.py
--rw-r--r--   0        0        0     7231 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/testing/__init__.py
--rw-r--r--   0        0        0      773 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/__init__.py
--rw-r--r--   0        0        0      838 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/__main__.py
--rw-r--r--   0        0        0      102 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       97 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       90 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       93 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       97 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       97 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      224 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       90 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       90 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
--rw-r--r--   0        0        0      100 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       85 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      117 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      117 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0       92 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-only/template.c
--rw-r--r--   0        0        0       92 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-only/template.h
--rw-r--r--   0        0        0      219 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-only/template.nasl
--rw-r--r--   0        0        0      101 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
--rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
--rw-r--r--   0        0        0      101 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
--rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.c
--rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
--rw-r--r--   0        0        0       92 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.go
--rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.h
--rw-r--r--   0        0        0       96 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.js
--rw-r--r--   0        0        0      223 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
--rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.po
--rw-r--r--   0        0        0       89 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.py
--rw-r--r--   0        0        0       99 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
--rw-r--r--   0        0        0       84 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
--rw-r--r--   0        0        0      116 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
--rw-r--r--   0        0        0      116 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
--rw-r--r--   0        0        0    12122 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/updateheader/updateheader.py
--rw-r--r--   0        0        0     1067 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/__init__.py
--rw-r--r--   0        0        0      816 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/__main__.py
--rw-r--r--   0        0        0      103 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/__version__.py
--rw-r--r--   0        0        0     8837 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/_calculator.py
--rw-r--r--   0        0        0     1508 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/__init__.py
--rw-r--r--   0        0        0     2723 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_cargo.py
--rw-r--r--   0        0        0     7752 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_cmake.py
--rw-r--r--   0        0        0     2553 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_command.py
--rw-r--r--   0        0        0     3792 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_go.py
--rw-r--r--   0        0        0     6263 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_javascript.py
--rw-r--r--   0        0        0     8216 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/commands/_python.py
--rw-r--r--   0        0        0      961 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/errors.py
--rw-r--r--   0        0        0     2812 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/helper.py
--rw-r--r--   0        0        0     3692 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/main.py
--rw-r--r--   0        0        0     4163 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/parser.py
--rw-r--r--   0        0        0     3750 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/project.py
--rw-r--r--   0        0        0     2163 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/schemes/__init__.py
--rw-r--r--   0        0        0    13439 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/schemes/_pep440.py
--rw-r--r--   0        0        0     2159 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/schemes/_scheme.py
--rw-r--r--   0        0        0    16043 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/schemes/_semantic.py
--rw-r--r--   0        0        0     5317 2023-05-09 06:59:43.248978 pontos-23.5.1/pontos/version/version.py
--rw-r--r--   0        0        0     2895 2023-05-09 06:59:43.248978 pontos-23.5.1/pyproject.toml
--rw-r--r--   0        0        0     1872 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/artifacts-download.py
--rw-r--r--   0        0        0     1862 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/artifacts.py
--rw-r--r--   0        0        0     1605 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/branchprotection.py
--rw-r--r--   0        0        0     5606 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/create-repository.py
--rw-r--r--   0        0        0     2212 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/enforce-admins.py
--rw-r--r--   0        0        0     1834 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/lock-branch.py
--rw-r--r--   0        0        0     2577 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/members.py
--rw-r--r--   0        0        0     2179 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/release-assets-download.py
--rw-r--r--   0        0        0     2294 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/repositories.py
--rw-r--r--   0        0        0     6717 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/search-repositories.py
--rw-r--r--   0        0        0     3689 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/team-repositories.py
--rw-r--r--   0        0        0     1654 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/teams.py
--rw-r--r--   0        0        0     2789 2023-05-09 06:59:43.248978 pontos-23.5.1/scripts/github/workflow-runs.py
--rw-r--r--   0        0        0     1518 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/__init__.py
--rw-r--r--   0        0        0     1031 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/changelog/__init__.py
--rw-r--r--   0        0        0      375 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/changelog/changelog.toml
--rw-r--r--   0        0        0    17750 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/changelog/test_conventional_commits.py
--rw-r--r--   0        0        0     1925 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/changelog/test_parser.py
--rw-r--r--   0        0        0       69 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/fake_pyproject.toml
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/git/__init__.py
--rw-r--r--   0        0        0    28296 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/git/test_git.py
--rw-r--r--   0        0        0     4215 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/git/test_status.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/__init__.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/__init__.py
--rw-r--r--   0        0        0    29628 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/test-pull-request-event.json
--rw-r--r--   0        0        0     5430 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/test_core.py
--rw-r--r--   0        0        0     3534 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/test_env.py
--rw-r--r--   0        0        0     2086 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/actions/test_event.py
--rw-r--r--   0        0        0     1232 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/api/__init__.py
--rw-r--r--   0        0        0    20021 2023-05-09 06:59:43.248978 pontos-23.5.1/tests/github/api/pr-files.json
--rw-r--r--   0        0        0     5624 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/release-response.json
--rw-r--r--   0        0        0    12076 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_artifacts.py
--rw-r--r--   0        0        0    20096 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_branch.py
--rw-r--r--   0        0        0     9619 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_client.py
--rw-r--r--   0        0        0     2087 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_contents.py
--rw-r--r--   0        0        0     2801 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_labels.py
--rw-r--r--   0        0        0    71096 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_organizations.py
--rw-r--r--   0        0        0    58514 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_pull_requests.py
--rw-r--r--   0        0        0    17774 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_release.py
--rw-r--r--   0        0        0    37847 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_repositories.py
--rw-r--r--   0        0        0    24490 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_search.py
--rw-r--r--   0        0        0     9471 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_tags.py
--rw-r--r--   0        0        0    39045 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_teams.py
--rw-r--r--   0        0        0   129346 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/api/test_workflows.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/__init__.py
--rw-r--r--   0        0        0     3210 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_artifact.py
--rw-r--r--   0        0        0     9831 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_base.py
--rw-r--r--   0        0        0    31873 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_branch.py
--rw-r--r--   0        0        0    19874 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_organization.py
--rw-r--r--   0        0        0    80894 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_pull_request.py
--rw-r--r--   0        0        0    12062 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_release.py
--rw-r--r--   0        0        0     2216 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_search.py
--rw-r--r--   0        0        0     3400 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_tag.py
--rw-r--r--   0        0        0    41463 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/models/test_workflow.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/script/__init__.py
--rw-r--r--   0        0        0     3520 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/script/test_load.py
--rw-r--r--   0        0        0     2052 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/script/test_parser.py
--rw-r--r--   0        0        0     6371 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/test_argparser.py
--rw-r--r--   0        0        0     9562 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/github/test_cmds.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/models/__init__.py
--rw-r--r--   0        0        0     6424 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/models/test_models.py
--rw-r--r--   0        0        0     2505 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/__init__.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/cpe/__init__.py
--rw-r--r--   0        0        0    11271 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/cpe/test_api.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/cve/__init__.py
--rw-r--r--   0        0        0    26602 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/cve/test_api.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/models/__init__.py
--rw-r--r--   0        0        0     3706 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/models/test_cpe.py
--rw-r--r--   0        0        0    25911 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/models/test_cve.py
--rw-r--r--   0        0        0     3994 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/nvd/test_api.py
--rw-r--r--   0        0        0      721 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/__init__.py
--rw-r--r--   0        0        0     3265 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/test_helper.py
--rw-r--r--   0        0        0     9077 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/test_parser.py
--rw-r--r--   0        0        0    83503 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/test_release.py
--rw-r--r--   0        0        0    25286 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/test_sign.py
--rw-r--r--   0        0        0      345 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/release/v1.2.3.md
--rw-r--r--   0        0        0      745 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/terminal/__init__.py
--rw-r--r--   0        0        0     6653 2023-05-09 06:59:43.252978 pontos-23.5.1/tests/terminal/test_terminal.py
--rw-r--r--   0        0        0    19355 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/test_helper.py
--rw-r--r--   0        0        0     1685 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/test_pontos.py
--rw-r--r--   0        0        0      716 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/testing/__init__.py
--rw-r--r--   0        0        0     7785 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/testing/test_testing.py
--rw-r--r--   0        0        0      721 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/updateheader/__init__.py
--rw-r--r--   0        0        0    15842 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/updateheader/test_header.py
--rw-r--r--   0        0        0     1031 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/__init__.py
--rw-r--r--   0        0        0      727 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/__init__.py
--rw-r--r--   0        0        0     3847 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_cargo.py
--rw-r--r--   0        0        0    11322 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_cmake.py
--rw-r--r--   0        0        0    10400 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_go.py
--rw-r--r--   0        0        0    15371 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_javascript.py
--rw-r--r--   0        0        0    16667 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/commands/test_python.py
--rw-r--r--   0        0        0      727 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/schemes/__init__.py
--rw-r--r--   0        0        0    25525 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/schemes/test_pep440.py
--rw-r--r--   0        0        0    27735 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/schemes/test_semantic.py
--rw-r--r--   0        0        0      919 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_commands.py
--rw-r--r--   0        0        0     1096 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_errors.py
--rw-r--r--   0        0        0     7621 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_helper.py
--rw-r--r--   0        0        0    10908 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_main.py
--rw-r--r--   0        0        0     1131 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_parser.py
--rw-r--r--   0        0        0     6187 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_project.py
--rw-r--r--   0        0        0     1791 2023-05-09 06:59:43.256978 pontos-23.5.1/tests/version/test_version.py
--rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.5.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-10 11:10:28.776647 pontos-23.5.2/LICENSE
+-rw-r--r--   0        0        0     3836 2023-05-10 11:10:28.776647 pontos-23.5.2/README.md
+-rw-r--r--   0        0        0    97053 2023-05-10 11:10:28.780647 pontos-23.5.2/poetry.lock
+-rw-r--r--   0        0        0       32 2023-05-10 11:10:28.780647 pontos-23.5.2/poetry.toml
+-rw-r--r--   0        0        0      791 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/__init__.py
+-rw-r--r--   0        0        0      968 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/changelog/__init__.py
+-rw-r--r--   0        0        0     9995 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/changelog/conventional_commits.py
+-rw-r--r--   0        0        0      965 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/changelog/errors.py
+-rw-r--r--   0        0        0     4393 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/changelog/main.py
+-rw-r--r--   0        0        0      806 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/errors.py
+-rw-r--r--   0        0        0      882 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/git/__init__.py
+-rw-r--r--   0        0        0    16153 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/git/git.py
+-rw-r--r--   0        0        0     2538 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/git/status.py
+-rw-r--r--   0        0        0      760 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/__init__.py
+-rw-r--r--   0        0        0     1154 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/__init__.py
+-rw-r--r--   0        0        0     2239 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/argparser.py
+-rw-r--r--   0        0        0     1472 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/cmds.py
+-rw-r--r--   0        0        0     7327 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/core.py
+-rw-r--r--   0        0        0     2426 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/env.py
+-rw-r--r--   0        0        0      861 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/errors.py
+-rw-r--r--   0        0        0     4173 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/event.py
+-rw-r--r--   0        0        0     1100 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/actions/main.py
+-rw-r--r--   0        0        0     2047 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/__init__.py
+-rw-r--r--   0        0        0     5531 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/api.py
+-rw-r--r--   0        0        0     6196 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/artifacts.py
+-rw-r--r--   0        0        0    34561 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/branch.py
+-rw-r--r--   0        0        0     9395 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/client.py
+-rw-r--r--   0        0        0     1844 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/contents.py
+-rw-r--r--   0        0        0      845 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/errors.py
+-rw-r--r--   0        0        0     1320 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/helper.py
+-rw-r--r--   0        0        0     2813 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/labels.py
+-rw-r--r--   0        0        0    10311 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/organizations.py
+-rw-r--r--   0        0        0    13090 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/pull_requests.py
+-rw-r--r--   0        0        0    11942 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/release.py
+-rw-r--r--   0        0        0    21512 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/repositories.py
+-rw-r--r--   0        0        0     3276 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/search.py
+-rw-r--r--   0        0        0     6004 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/tags.py
+-rw-r--r--   0        0        0    15207 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/teams.py
+-rw-r--r--   0        0        0     9182 2023-05-10 11:10:28.784647 pontos-23.5.2/pontos/github/api/workflows.py
+-rw-r--r--   0        0        0    11128 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/argparser.py
+-rw-r--r--   0        0        0     8863 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/cmds.py
+-rw-r--r--   0        0        0     1347 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/main.py
+-rw-r--r--   0        0        0     1114 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/__init__.py
+-rw-r--r--   0        0        0     2336 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/artifact.py
+-rw-r--r--   0        0        0     7532 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/base.py
+-rw-r--r--   0        0        0     6915 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/branch.py
+-rw-r--r--   0        0        0    16573 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/organization.py
+-rw-r--r--   0        0        0    14248 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/pull_request.py
+-rw-r--r--   0        0        0     4607 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/release.py
+-rw-r--r--   0        0        0     4299 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/search.py
+-rw-r--r--   0        0        0     4606 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/tag.py
+-rw-r--r--   0        0        0    11477 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/models/workflow.py
+-rw-r--r--   0        0        0      790 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/pr_template.md
+-rw-r--r--   0        0        0     3207 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/script/__init__.py
+-rw-r--r--   0        0        0      835 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/script/errors.py
+-rw-r--r--   0        0        0     4854 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/script/load.py
+-rw-r--r--   0        0        0     1495 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/github/script/parser.py
+-rw-r--r--   0        0        0    14685 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/helper.py
+-rw-r--r--   0        0        0     6211 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/models/__init__.py
+-rw-r--r--   0        0        0      821 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/__init__.py
+-rw-r--r--   0        0        0     4660 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/api.py
+-rw-r--r--   0        0        0     2149 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0     6708 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/cpe/api.py
+-rw-r--r--   0        0        0     2618 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    10802 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/cve/api.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/__init__.py
+-rw-r--r--   0        0        0     2973 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/cpe.py
+-rw-r--r--   0        0        0     7250 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/cve.py
+-rw-r--r--   0        0        0     3254 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/cvss_v2.py
+-rw-r--r--   0        0        0     4471 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/nvd/models/cvss_v3.py
+-rw-r--r--   0        0        0     3561 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/pontos.py
+-rw-r--r--   0        0        0        0 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/py.typed
+-rw-r--r--   0        0        0     1164 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/__init__.py
+-rw-r--r--   0        0        0     2472 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/helper.py
+-rw-r--r--   0        0        0     2127 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/main.py
+-rw-r--r--   0        0        0     8333 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/parser.py
+-rw-r--r--   0        0        0    14408 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/release.py
+-rw-r--r--   0        0        0    12499 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/release/sign.py
+-rw-r--r--   0        0        0      886 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/terminal/__init__.py
+-rw-r--r--   0        0        0     1770 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/terminal/null.py
+-rw-r--r--   0        0        0     4717 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/terminal/rich.py
+-rw-r--r--   0        0        0     9416 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/terminal/terminal.py
+-rw-r--r--   0        0        0     7231 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/testing/__init__.py
+-rw-r--r--   0        0        0      773 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/__init__.py
+-rw-r--r--   0        0        0      838 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/__main__.py
+-rw-r--r--   0        0        0      102 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       97 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       90 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       93 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       97 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       97 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      224 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       90 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       90 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0      100 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       85 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      117 2023-05-10 11:10:28.788647 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      117 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/AGPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0       92 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-only/template.c
+-rw-r--r--   0        0        0       92 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-only/template.h
+-rw-r--r--   0        0        0      219 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-only/template.nasl
+-rw-r--r--   0        0        0      101 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.cmake
+-rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-2.0-or-later/template.xsl
+-rw-r--r--   0        0        0      101 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.bash
+-rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.c
+-rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.cmake
+-rw-r--r--   0        0        0       92 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.go
+-rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.h
+-rw-r--r--   0        0        0       96 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.js
+-rw-r--r--   0        0        0      223 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.nasl
+-rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.po
+-rw-r--r--   0        0        0       89 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.py
+-rw-r--r--   0        0        0       99 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.sh
+-rw-r--r--   0        0        0       84 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.txt
+-rw-r--r--   0        0        0      116 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xml
+-rw-r--r--   0        0        0      116 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/templates/GPL-3.0-or-later/template.xsl
+-rw-r--r--   0        0        0    12122 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/updateheader/updateheader.py
+-rw-r--r--   0        0        0     1067 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/__init__.py
+-rw-r--r--   0        0        0      816 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/__main__.py
+-rw-r--r--   0        0        0      103 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/__version__.py
+-rw-r--r--   0        0        0     8837 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/_calculator.py
+-rw-r--r--   0        0        0     1508 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/__init__.py
+-rw-r--r--   0        0        0     2723 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_cargo.py
+-rw-r--r--   0        0        0     7752 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_cmake.py
+-rw-r--r--   0        0        0     2553 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_command.py
+-rw-r--r--   0        0        0     3792 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_go.py
+-rw-r--r--   0        0        0     6263 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_javascript.py
+-rw-r--r--   0        0        0     8216 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/commands/_python.py
+-rw-r--r--   0        0        0      961 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/errors.py
+-rw-r--r--   0        0        0     2812 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/helper.py
+-rw-r--r--   0        0        0     3692 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/main.py
+-rw-r--r--   0        0        0     4163 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/parser.py
+-rw-r--r--   0        0        0     3750 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/project.py
+-rw-r--r--   0        0        0     2163 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/schemes/__init__.py
+-rw-r--r--   0        0        0    13439 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/schemes/_pep440.py
+-rw-r--r--   0        0        0     2159 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/schemes/_scheme.py
+-rw-r--r--   0        0        0    16043 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/schemes/_semantic.py
+-rw-r--r--   0        0        0     5317 2023-05-10 11:10:28.792646 pontos-23.5.2/pontos/version/version.py
+-rw-r--r--   0        0        0     2895 2023-05-10 11:10:28.792646 pontos-23.5.2/pyproject.toml
+-rw-r--r--   0        0        0     1872 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/artifacts-download.py
+-rw-r--r--   0        0        0     1862 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/artifacts.py
+-rw-r--r--   0        0        0     1605 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/branchprotection.py
+-rw-r--r--   0        0        0     5606 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/create-repository.py
+-rw-r--r--   0        0        0     2212 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/enforce-admins.py
+-rw-r--r--   0        0        0     1834 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/lock-branch.py
+-rw-r--r--   0        0        0     2577 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/members.py
+-rw-r--r--   0        0        0     2179 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/release-assets-download.py
+-rw-r--r--   0        0        0     2294 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/repositories.py
+-rw-r--r--   0        0        0     6717 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/search-repositories.py
+-rw-r--r--   0        0        0     3689 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/team-repositories.py
+-rw-r--r--   0        0        0     1654 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/teams.py
+-rw-r--r--   0        0        0     2789 2023-05-10 11:10:28.792646 pontos-23.5.2/scripts/github/workflow-runs.py
+-rw-r--r--   0        0        0     1518 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/changelog/__init__.py
+-rw-r--r--   0        0        0      375 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/changelog/changelog.toml
+-rw-r--r--   0        0        0    17925 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/changelog/test_conventional_commits.py
+-rw-r--r--   0        0        0     1925 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/changelog/test_parser.py
+-rw-r--r--   0        0        0       69 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/fake_pyproject.toml
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/git/__init__.py
+-rw-r--r--   0        0        0    28296 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/git/test_git.py
+-rw-r--r--   0        0        0     4215 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/git/test_status.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/github/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/github/actions/__init__.py
+-rw-r--r--   0        0        0    29628 2023-05-10 11:10:28.792646 pontos-23.5.2/tests/github/actions/test-pull-request-event.json
+-rw-r--r--   0        0        0     5430 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/actions/test_core.py
+-rw-r--r--   0        0        0     3534 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/actions/test_env.py
+-rw-r--r--   0        0        0     2086 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/actions/test_event.py
+-rw-r--r--   0        0        0     1232 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/__init__.py
+-rw-r--r--   0        0        0    20021 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/pr-files.json
+-rw-r--r--   0        0        0     5624 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/release-response.json
+-rw-r--r--   0        0        0    12076 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_artifacts.py
+-rw-r--r--   0        0        0    20096 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_branch.py
+-rw-r--r--   0        0        0     9619 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_client.py
+-rw-r--r--   0        0        0     2087 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_contents.py
+-rw-r--r--   0        0        0     2801 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_labels.py
+-rw-r--r--   0        0        0    71096 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_organizations.py
+-rw-r--r--   0        0        0    58514 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_pull_requests.py
+-rw-r--r--   0        0        0    17774 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_release.py
+-rw-r--r--   0        0        0    37847 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_repositories.py
+-rw-r--r--   0        0        0    24490 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_search.py
+-rw-r--r--   0        0        0     9471 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_tags.py
+-rw-r--r--   0        0        0    39045 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_teams.py
+-rw-r--r--   0        0        0   129346 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/api/test_workflows.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/__init__.py
+-rw-r--r--   0        0        0     3210 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_artifact.py
+-rw-r--r--   0        0        0     9831 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_base.py
+-rw-r--r--   0        0        0    31873 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_branch.py
+-rw-r--r--   0        0        0    19874 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_organization.py
+-rw-r--r--   0        0        0    80894 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_pull_request.py
+-rw-r--r--   0        0        0    12062 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_release.py
+-rw-r--r--   0        0        0     2216 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_search.py
+-rw-r--r--   0        0        0     3400 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_tag.py
+-rw-r--r--   0        0        0    41463 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/models/test_workflow.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/script/__init__.py
+-rw-r--r--   0        0        0     3520 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/script/test_load.py
+-rw-r--r--   0        0        0     2052 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/script/test_parser.py
+-rw-r--r--   0        0        0     6371 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/test_argparser.py
+-rw-r--r--   0        0        0     9562 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/github/test_cmds.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/models/__init__.py
+-rw-r--r--   0        0        0     6424 2023-05-10 11:10:28.796646 pontos-23.5.2/tests/models/test_models.py
+-rw-r--r--   0        0        0     2505 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/cpe/__init__.py
+-rw-r--r--   0        0        0    11271 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/cpe/test_api.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/cve/__init__.py
+-rw-r--r--   0        0        0    26602 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/cve/test_api.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/models/__init__.py
+-rw-r--r--   0        0        0     3706 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/models/test_cpe.py
+-rw-r--r--   0        0        0    25911 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/models/test_cve.py
+-rw-r--r--   0        0        0     3994 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/nvd/test_api.py
+-rw-r--r--   0        0        0      721 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/__init__.py
+-rw-r--r--   0        0        0     3265 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/test_helper.py
+-rw-r--r--   0        0        0     9077 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/test_parser.py
+-rw-r--r--   0        0        0    83503 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/test_release.py
+-rw-r--r--   0        0        0    25286 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/test_sign.py
+-rw-r--r--   0        0        0      345 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/release/v1.2.3.md
+-rw-r--r--   0        0        0      745 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/terminal/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/terminal/test_terminal.py
+-rw-r--r--   0        0        0    19355 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/test_helper.py
+-rw-r--r--   0        0        0     1685 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/test_pontos.py
+-rw-r--r--   0        0        0      716 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/testing/__init__.py
+-rw-r--r--   0        0        0     7785 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/testing/test_testing.py
+-rw-r--r--   0        0        0      721 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/updateheader/__init__.py
+-rw-r--r--   0        0        0    15842 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/updateheader/test_header.py
+-rw-r--r--   0        0        0     1031 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/__init__.py
+-rw-r--r--   0        0        0      727 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/__init__.py
+-rw-r--r--   0        0        0     3847 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_cargo.py
+-rw-r--r--   0        0        0    11322 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_cmake.py
+-rw-r--r--   0        0        0    10400 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_go.py
+-rw-r--r--   0        0        0    15371 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_javascript.py
+-rw-r--r--   0        0        0    16667 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/commands/test_python.py
+-rw-r--r--   0        0        0      727 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/schemes/__init__.py
+-rw-r--r--   0        0        0    25525 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/schemes/test_pep440.py
+-rw-r--r--   0        0        0    27735 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/schemes/test_semantic.py
+-rw-r--r--   0        0        0      919 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_commands.py
+-rw-r--r--   0        0        0     1096 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_errors.py
+-rw-r--r--   0        0        0     7621 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_helper.py
+-rw-r--r--   0        0        0    10908 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_main.py
+-rw-r--r--   0        0        0     1131 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_parser.py
+-rw-r--r--   0        0        0     6187 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_project.py
+-rw-r--r--   0        0        0     1791 2023-05-10 11:10:28.800646 pontos-23.5.2/tests/version/test_version.py
+-rw-r--r--   0        0        0     5303 1970-01-01 00:00:00.000000 pontos-23.5.2/PKG-INFO
```

### Comparing `pontos-23.5.1/LICENSE` & `pontos-23.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/README.md` & `pontos-23.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/poetry.lock` & `pontos-23.5.2/poetry.lock`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/__init__.py` & `pontos-23.5.2/pontos/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/changelog/__init__.py` & `pontos-23.5.2/pontos/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/changelog/conventional_commits.py` & `pontos-23.5.2/pontos/changelog/conventional_commits.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 ADDRESS = "https://github.com/"
 
 DEFAULT_CHANGELOG_CONFIG = """commit_types = [
     { message = "^add", group = "Added"},
     { message = "^remove", group = "Removed"},
     { message = "^change", group = "Changed"},
     { message = "^fix", group = "Bug Fixes"},
+    { message = "^deps", group = "Dependencies"},
 ]
 """
 
 
 @runtime_checkable
 class SupportsStr(Protocol):
     @abstractmethod
@@ -55,16 +56,18 @@
         "v1.2.3" and "v2.0.0" using the default config settings.
 
         .. code-block:: python
 
             from pontos.changelog import ChangelogBuilder
 
             builder = ChangelogBuilder(space="my-org", project="my-project)
-            changelog = builder.create_changelog
-                last_version="1.2.3", next_version="2.0.0")
+            changelog = builder.create_changelog(
+                last_version="1.2.3",
+                next_version="2.0.0",
+            )
     """
 
     def __init__(
         self,
         *,
         space: str,
         project: str,
```

### Comparing `pontos-23.5.1/pontos/changelog/errors.py` & `pontos-23.5.2/pontos/changelog/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/changelog/main.py` & `pontos-23.5.2/pontos/changelog/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/errors.py` & `pontos-23.5.2/pontos/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/git/__init__.py` & `pontos-23.5.2/pontos/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/git/git.py` & `pontos-23.5.2/pontos/git/git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/git/status.py` & `pontos-23.5.2/pontos/git/status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/__init__.py` & `pontos-23.5.2/pontos/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/actions/__init__.py` & `pontos-23.5.2/pontos/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/actions/argparser.py` & `pontos-23.5.2/pontos/github/actions/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/actions/cmds.py` & `pontos-23.5.2/pontos/github/actions/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/actions/core.py` & `pontos-23.5.2/pontos/github/actions/core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/actions/env.py` & `pontos-23.5.2/pontos/github/actions/env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/actions/errors.py` & `pontos-23.5.2/pontos/github/actions/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/actions/event.py` & `pontos-23.5.2/pontos/github/actions/event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/actions/main.py` & `pontos-23.5.2/pontos/github/actions/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/__init__.py` & `pontos-23.5.2/pontos/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/api.py` & `pontos-23.5.2/pontos/github/api/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/artifacts.py` & `pontos-23.5.2/pontos/github/api/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/branch.py` & `pontos-23.5.2/pontos/github/api/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/client.py` & `pontos-23.5.2/pontos/github/api/client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/contents.py` & `pontos-23.5.2/pontos/github/api/contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/errors.py` & `pontos-23.5.2/pontos/github/api/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/helper.py` & `pontos-23.5.2/pontos/github/api/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/labels.py` & `pontos-23.5.2/pontos/github/api/labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/organizations.py` & `pontos-23.5.2/pontos/github/api/organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/pull_requests.py` & `pontos-23.5.2/pontos/github/api/pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/release.py` & `pontos-23.5.2/pontos/github/api/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/repositories.py` & `pontos-23.5.2/pontos/github/api/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/search.py` & `pontos-23.5.2/pontos/github/api/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/tags.py` & `pontos-23.5.2/pontos/github/api/tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/teams.py` & `pontos-23.5.2/pontos/github/api/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/api/workflows.py` & `pontos-23.5.2/pontos/github/api/workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/argparser.py` & `pontos-23.5.2/pontos/github/argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/cmds.py` & `pontos-23.5.2/pontos/github/cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/main.py` & `pontos-23.5.2/pontos/github/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/__init__.py` & `pontos-23.5.2/pontos/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/artifact.py` & `pontos-23.5.2/pontos/github/models/artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/base.py` & `pontos-23.5.2/pontos/github/models/base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/branch.py` & `pontos-23.5.2/pontos/github/models/branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/organization.py` & `pontos-23.5.2/pontos/github/models/organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/pull_request.py` & `pontos-23.5.2/pontos/github/models/pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/release.py` & `pontos-23.5.2/pontos/github/models/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/search.py` & `pontos-23.5.2/pontos/github/models/search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/tag.py` & `pontos-23.5.2/pontos/github/models/tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/models/workflow.py` & `pontos-23.5.2/pontos/github/models/workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/pr_template.md` & `pontos-23.5.2/pontos/github/pr_template.md`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/script/__init__.py` & `pontos-23.5.2/pontos/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/script/errors.py` & `pontos-23.5.2/pontos/github/script/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/script/load.py` & `pontos-23.5.2/pontos/github/script/load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/github/script/parser.py` & `pontos-23.5.2/pontos/github/script/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/helper.py` & `pontos-23.5.2/pontos/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/models/__init__.py` & `pontos-23.5.2/pontos/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/__init__.py` & `pontos-23.5.2/pontos/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/api.py` & `pontos-23.5.2/pontos/nvd/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/cpe/__init__.py` & `pontos-23.5.2/pontos/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/cpe/api.py` & `pontos-23.5.2/pontos/nvd/cpe/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/cve/__init__.py` & `pontos-23.5.2/pontos/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/cve/api.py` & `pontos-23.5.2/pontos/nvd/cve/api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/models/__init__.py` & `pontos-23.5.2/pontos/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/models/cpe.py` & `pontos-23.5.2/pontos/nvd/models/cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/models/cve.py` & `pontos-23.5.2/pontos/nvd/models/cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/models/cvss_v2.py` & `pontos-23.5.2/pontos/nvd/models/cvss_v2.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/nvd/models/cvss_v3.py` & `pontos-23.5.2/pontos/nvd/models/cvss_v3.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/pontos.py` & `pontos-23.5.2/pontos/pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/release/__init__.py` & `pontos-23.5.2/pontos/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/release/helper.py` & `pontos-23.5.2/pontos/release/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/release/main.py` & `pontos-23.5.2/pontos/release/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/release/parser.py` & `pontos-23.5.2/pontos/release/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/release/release.py` & `pontos-23.5.2/pontos/release/release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/release/sign.py` & `pontos-23.5.2/pontos/release/sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/terminal/__init__.py` & `pontos-23.5.2/pontos/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/terminal/null.py` & `pontos-23.5.2/pontos/terminal/null.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/terminal/rich.py` & `pontos-23.5.2/pontos/terminal/rich.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/terminal/terminal.py` & `pontos-23.5.2/pontos/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/testing/__init__.py` & `pontos-23.5.2/pontos/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/updateheader/__init__.py` & `pontos-23.5.2/pontos/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/updateheader/__main__.py` & `pontos-23.5.2/pontos/updateheader/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/updateheader/updateheader.py` & `pontos-23.5.2/pontos/updateheader/updateheader.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/__init__.py` & `pontos-23.5.2/pontos/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/__main__.py` & `pontos-23.5.2/pontos/version/__main__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/_calculator.py` & `pontos-23.5.2/pontos/version/_calculator.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/commands/__init__.py` & `pontos-23.5.2/pontos/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/commands/_cargo.py` & `pontos-23.5.2/pontos/version/commands/_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/commands/_cmake.py` & `pontos-23.5.2/pontos/version/commands/_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/commands/_command.py` & `pontos-23.5.2/pontos/version/commands/_command.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/commands/_go.py` & `pontos-23.5.2/pontos/version/commands/_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/commands/_javascript.py` & `pontos-23.5.2/pontos/version/commands/_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/commands/_python.py` & `pontos-23.5.2/pontos/version/commands/_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/errors.py` & `pontos-23.5.2/pontos/version/errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/helper.py` & `pontos-23.5.2/pontos/version/helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/main.py` & `pontos-23.5.2/pontos/version/main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/parser.py` & `pontos-23.5.2/pontos/version/parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/project.py` & `pontos-23.5.2/pontos/version/project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/schemes/__init__.py` & `pontos-23.5.2/pontos/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/schemes/_pep440.py` & `pontos-23.5.2/pontos/version/schemes/_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/schemes/_scheme.py` & `pontos-23.5.2/pontos/version/schemes/_scheme.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/schemes/_semantic.py` & `pontos-23.5.2/pontos/version/schemes/_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pontos/version/version.py` & `pontos-23.5.2/pontos/version/version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/pyproject.toml` & `pontos-23.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pontos"
-version = "23.5.1"
+version = "23.5.2"
 description = "Common utilities and tools maintained by Greenbone Networks"
 authors = ["Greenbone AG <info@greenbone.net>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://github.com/greenbone/pontos/"
 repository = "https://github.com/greenbone/pontos/"
 documentation = "https://greenbone.github.io/pontos/"
```

### Comparing `pontos-23.5.1/scripts/github/artifacts-download.py` & `pontos-23.5.2/scripts/github/artifacts-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/artifacts.py` & `pontos-23.5.2/scripts/github/artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/branchprotection.py` & `pontos-23.5.2/scripts/github/branchprotection.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/create-repository.py` & `pontos-23.5.2/scripts/github/create-repository.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/enforce-admins.py` & `pontos-23.5.2/scripts/github/enforce-admins.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/lock-branch.py` & `pontos-23.5.2/scripts/github/lock-branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/members.py` & `pontos-23.5.2/scripts/github/members.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/release-assets-download.py` & `pontos-23.5.2/scripts/github/release-assets-download.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/repositories.py` & `pontos-23.5.2/scripts/github/repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/search-repositories.py` & `pontos-23.5.2/scripts/github/search-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/team-repositories.py` & `pontos-23.5.2/scripts/github/team-repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/teams.py` & `pontos-23.5.2/scripts/github/teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/scripts/github/workflow-runs.py` & `pontos-23.5.2/scripts/github/workflow-runs.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/__init__.py` & `pontos-23.5.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/changelog/__init__.py` & `pontos-23.5.2/tests/changelog/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/changelog/test_conventional_commits.py` & `pontos-23.5.2/tests/changelog/test_conventional_commits.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     stdout: bytes
 
 
 class ChangelogBuilderTestCase(unittest.TestCase):
     maxDiff = None
 
     @patch("pontos.changelog.conventional_commits.Git", autospec=True)
-    def test_changelog_builder(self, git_mock: MagicMock):
+    def test_changelog_builder_with_config(self, git_mock: MagicMock):
         today = datetime.today().strftime("%Y-%m-%d")
 
         own_path = Path(__file__).absolute().parent
         config_toml = own_path / "changelog.toml"
 
         git_mock.return_value.list_tags.return_value = ["v0.0.1"]
         git_mock.return_value.log.return_value = [
@@ -356,14 +356,15 @@
             "8abcd3d Adding bar baz",
             "1337abc Change: bar to baz",
             "42a42a4 Remove: foo bar again",
             "fedcba8 Test: bar baz testing",
             "dead901 Refactor: bar baz ref",
             "fedcba8 Fix: bar baz fixing",
             "d0c4d0c Doc: bar baz documenting",
+            "a1c5a0b Deps: Update foo from 1.2.3 to 3.2.1",
         ]
 
         changelog_builder = ChangelogBuilder(
             space="foo",
             project="bar",
         )
         expected_output = f"""## [0.0.2] - {today}
@@ -377,14 +378,17 @@
 
 ## Changed
 * bar to baz [1337abc](https://github.com/foo/bar/commit/1337abc)
 
 ## Bug Fixes
 * bar baz fixing [fedcba8](https://github.com/foo/bar/commit/fedcba8)
 
+## Dependencies
+* Update foo from 1.2.3 to 3.2.1 [a1c5a0b](https://github.com/foo/bar/commit/a1c5a0b)
+
 [0.0.2]: https://github.com/foo/bar/compare/v0.0.1...v0.0.2"""
 
         changelog = changelog_builder.create_changelog(
             last_version="0.0.1", next_version="0.0.2"
         )
         self.assertEqual(changelog, expected_output)
```

### Comparing `pontos-23.5.1/tests/changelog/test_parser.py` & `pontos-23.5.2/tests/changelog/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/git/__init__.py` & `pontos-23.5.2/tests/git/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/git/test_git.py` & `pontos-23.5.2/tests/git/test_git.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/git/test_status.py` & `pontos-23.5.2/tests/git/test_status.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/__init__.py` & `pontos-23.5.2/tests/github/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/actions/__init__.py` & `pontos-23.5.2/tests/github/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/actions/test-pull-request-event.json` & `pontos-23.5.2/tests/github/actions/test-pull-request-event.json`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/actions/test_core.py` & `pontos-23.5.2/tests/github/actions/test_core.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/actions/test_env.py` & `pontos-23.5.2/tests/github/actions/test_env.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/actions/test_event.py` & `pontos-23.5.2/tests/github/actions/test_event.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/__init__.py` & `pontos-23.5.2/tests/github/api/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/pr-files.json` & `pontos-23.5.2/tests/github/api/pr-files.json`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/release-response.json` & `pontos-23.5.2/tests/github/api/release-response.json`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_artifacts.py` & `pontos-23.5.2/tests/github/api/test_artifacts.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_branch.py` & `pontos-23.5.2/tests/github/api/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_client.py` & `pontos-23.5.2/tests/github/api/test_client.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_contents.py` & `pontos-23.5.2/tests/github/api/test_contents.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_labels.py` & `pontos-23.5.2/tests/github/api/test_labels.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_organizations.py` & `pontos-23.5.2/tests/github/api/test_organizations.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_pull_requests.py` & `pontos-23.5.2/tests/github/api/test_pull_requests.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_release.py` & `pontos-23.5.2/tests/github/api/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_repositories.py` & `pontos-23.5.2/tests/github/api/test_repositories.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_search.py` & `pontos-23.5.2/tests/github/api/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_tags.py` & `pontos-23.5.2/tests/github/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_teams.py` & `pontos-23.5.2/tests/github/api/test_teams.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/api/test_workflows.py` & `pontos-23.5.2/tests/github/api/test_workflows.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/__init__.py` & `pontos-23.5.2/tests/github/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/test_artifact.py` & `pontos-23.5.2/tests/github/models/test_artifact.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/test_base.py` & `pontos-23.5.2/tests/github/models/test_base.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/test_branch.py` & `pontos-23.5.2/tests/github/models/test_branch.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/test_organization.py` & `pontos-23.5.2/tests/github/models/test_organization.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/test_pull_request.py` & `pontos-23.5.2/tests/github/models/test_pull_request.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/test_release.py` & `pontos-23.5.2/tests/github/models/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/test_search.py` & `pontos-23.5.2/tests/github/models/test_search.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/test_tag.py` & `pontos-23.5.2/tests/github/models/test_tag.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/models/test_workflow.py` & `pontos-23.5.2/tests/github/models/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/script/__init__.py` & `pontos-23.5.2/tests/github/script/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/script/test_load.py` & `pontos-23.5.2/tests/github/script/test_load.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/script/test_parser.py` & `pontos-23.5.2/tests/github/script/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/test_argparser.py` & `pontos-23.5.2/tests/github/test_argparser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/github/test_cmds.py` & `pontos-23.5.2/tests/github/test_cmds.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/models/__init__.py` & `pontos-23.5.2/tests/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/models/test_models.py` & `pontos-23.5.2/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/nvd/__init__.py` & `pontos-23.5.2/tests/nvd/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/nvd/cpe/__init__.py` & `pontos-23.5.2/tests/nvd/cpe/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/nvd/cpe/test_api.py` & `pontos-23.5.2/tests/nvd/cpe/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/nvd/cve/__init__.py` & `pontos-23.5.2/tests/nvd/cve/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/nvd/cve/test_api.py` & `pontos-23.5.2/tests/nvd/cve/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/nvd/models/__init__.py` & `pontos-23.5.2/tests/nvd/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/nvd/models/test_cpe.py` & `pontos-23.5.2/tests/nvd/models/test_cpe.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/nvd/models/test_cve.py` & `pontos-23.5.2/tests/nvd/models/test_cve.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/nvd/test_api.py` & `pontos-23.5.2/tests/nvd/test_api.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/release/__init__.py` & `pontos-23.5.2/tests/release/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/release/test_helper.py` & `pontos-23.5.2/tests/release/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/release/test_parser.py` & `pontos-23.5.2/tests/release/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/release/test_release.py` & `pontos-23.5.2/tests/release/test_release.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/release/test_sign.py` & `pontos-23.5.2/tests/release/test_sign.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/terminal/__init__.py` & `pontos-23.5.2/tests/terminal/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/terminal/test_terminal.py` & `pontos-23.5.2/tests/terminal/test_terminal.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/test_helper.py` & `pontos-23.5.2/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/test_pontos.py` & `pontos-23.5.2/tests/test_pontos.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/testing/__init__.py` & `pontos-23.5.2/tests/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/testing/test_testing.py` & `pontos-23.5.2/tests/testing/test_testing.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/updateheader/__init__.py` & `pontos-23.5.2/tests/updateheader/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/updateheader/test_header.py` & `pontos-23.5.2/tests/updateheader/test_header.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/__init__.py` & `pontos-23.5.2/tests/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/commands/__init__.py` & `pontos-23.5.2/tests/version/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/commands/test_cargo.py` & `pontos-23.5.2/tests/version/commands/test_cargo.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/commands/test_cmake.py` & `pontos-23.5.2/tests/version/commands/test_cmake.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/commands/test_go.py` & `pontos-23.5.2/tests/version/commands/test_go.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/commands/test_javascript.py` & `pontos-23.5.2/tests/version/commands/test_javascript.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/commands/test_python.py` & `pontos-23.5.2/tests/version/commands/test_python.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/schemes/__init__.py` & `pontos-23.5.2/tests/version/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/schemes/test_pep440.py` & `pontos-23.5.2/tests/version/schemes/test_pep440.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/schemes/test_semantic.py` & `pontos-23.5.2/tests/version/schemes/test_semantic.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/test_commands.py` & `pontos-23.5.2/tests/version/test_commands.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/test_errors.py` & `pontos-23.5.2/tests/version/test_errors.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/test_helper.py` & `pontos-23.5.2/tests/version/test_helper.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/test_main.py` & `pontos-23.5.2/tests/version/test_main.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/test_parser.py` & `pontos-23.5.2/tests/version/test_parser.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/test_project.py` & `pontos-23.5.2/tests/version/test_project.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/tests/version/test_version.py` & `pontos-23.5.2/tests/version/test_version.py`

 * *Files identical despite different names*

### Comparing `pontos-23.5.1/PKG-INFO` & `pontos-23.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pontos
-Version: 23.5.1
+Version: 23.5.2
 Summary: Common utilities and tools maintained by Greenbone Networks
 Home-page: https://github.com/greenbone/pontos/
 License: GPL-3.0-or-later
 Author: Greenbone AG
 Author-email: info@greenbone.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

