# Comparing `tmp/hydra-genetics-1.1.0.tar.gz` & `tmp/hydra-genetics-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hydra-genetics-1.1.0.tar", last modified: Fri May  5 06:56:22 2023, max compression
+gzip compressed data, was "hydra-genetics-1.2.0.tar", last modified: Tue May  9 09:29:48 2023, max compression
```

## Comparing `hydra-genetics-1.1.0.tar` & `hydra-genetics-1.2.0.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33225 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/commands/prep_pipeline_env.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/linters/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/linters/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.587232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/samples.tsv
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/config/units.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/images/
--rw-r--r--   0 runner    (1001) docker     (123)    61275 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/images/hydragenetics.png
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/mkdocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/requirements.test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/Snakefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/report/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/report/describe_workflow.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/rules/
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/rules/dummy.smk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/rule-template/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/config.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/resources.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/rules.schema.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/skeleton_rule.smk
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/rule-template/softwares.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/chr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/hotspot_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/multibp.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/hydra_genetics/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/models/hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/hydra_genetics/utils/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.591232 hydra-genetics-1.1.0/hydra_genetics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 06:56:22.000000 hydra-genetics-1.1.0/hydra_genetics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/tests/utils/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/io/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/io/test_mutations_report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:22.595233 hydra-genetics-1.1.0/tests/utils/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/models/test_hotspot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/test_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/tests/utils/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-05 06:56:14.000000 hydra-genetics-1.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/hydra_genetics/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/hydra_genetics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.694166 hydra-genetics-1.2.0/hydra_genetics/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33218 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/commands/prep_pipeline_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.694166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.694166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.694166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.694166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/linters/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/linters/.snakefmt.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.694166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/linters/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/linters/report/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.694166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/conventional-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/release-please.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.682166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.tests/integration/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.tests/integration/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.tests/integration/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.tests/integration/units.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    34961 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/config/output_files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/config/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/config/samples.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/config/units.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/docs/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/docs/includes/abbreviations.md
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/docs/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/docs/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    61275 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/images/hydragenetics.png
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/mkdocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/requirements.test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/Snakefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/rules/common.smk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/scripts/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.698166 hydra-genetics-1.2.0/hydra_genetics/rule-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/rule-template/config.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/rule-template/resources.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/rule-template/rules.schema.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/rule-template/skeleton_rule.smk
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/rule-template/softwares.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/hydra_genetics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/hydra_genetics/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/io/chr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/io/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/io/hotspot_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/io/multibp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/io/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/hydra_genetics/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/models/hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/hydra_genetics/utils/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.694166 hydra-genetics-1.2.0/hydra_genetics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-09 09:29:48.000000 hydra-genetics-1.2.0/hydra_genetics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-09 09:29:48.000000 hydra-genetics-1.2.0/hydra_genetics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:29:48.000000 hydra-genetics-1.2.0/hydra_genetics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-09 09:29:48.000000 hydra-genetics-1.2.0/hydra_genetics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:29:48.000000 hydra-genetics-1.2.0/hydra_genetics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 09:29:48.000000 hydra-genetics-1.2.0/hydra_genetics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 09:29:48.000000 hydra-genetics-1.2.0/hydra_genetics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/tests/utils/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/io/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67196 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/io/test_mutations_report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:48.702166 hydra-genetics-1.2.0/tests/utils/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/models/test_hotspot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/test_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28006 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/tests/utils/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80044 2023-05-09 09:29:38.000000 hydra-genetics-1.2.0/versioneer.py
```

### Comparing `hydra-genetics-1.1.0/LICENSE.md` & `hydra-genetics-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/PKG-INFO` & `hydra-genetics-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 1.1.0
+Version: 1.2.0
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

### Comparing `hydra-genetics-1.1.0/README.md` & `hydra-genetics-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/__init__.py` & `hydra-genetics-1.2.0/hydra_genetics/__init__.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/__main__.py` & `hydra-genetics-1.2.0/hydra_genetics/__main__.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/commands/create.py` & `hydra-genetics-1.2.0/hydra_genetics/commands/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,15 @@
                 else:
                     os.makedirs(output_path)
                 continue
 
             log.debug(f"Rendering template file: '{template_fn}'")
 
             if template_fn.endswith(".png"):
-                print(template_fn)
-                shutil.copy(template_fn, output_path)
+                shutil.copy(os.path.join(template_dir, template_fn), output_path)
             else:
                 j_template = env.get_template(template_fn)
                 rendered_output = j_template.render(object_attrs)
 
                 # Write to the pipeline output file
                 with open(output_path, "w") as fh:
                     log.debug(f"Writing to output file: '{output_path}'")
```

### Comparing `hydra-genetics-1.1.0/hydra_genetics/commands/prep_pipeline_env.py` & `hydra-genetics-1.2.0/hydra_genetics/commands/prep_pipeline_env.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,25 +73,25 @@
     "--new-configfile",
     prompt="path",
     required=True,
     type=str,
     help="path to update config file",
 )
 @click.option(
-    "--reference-path",
+    "--reference-paths",
     multiple=True,
     prompt="path",
     required=True,
     type=str,
     help=(
         "format oldpath:newpath, will iterate over the provided config"
         " file and replace all occurrences of oldpath with new path"
     ),
 )
-def reference_path_update(configfile, new_configfile, reference_path):
+def reference_path_update(configfile, new_configfile, reference_paths):
     def process_yaml_data(yaml_data, reference_path):
         for key in yaml_data:
             if isinstance(yaml_data[key], dict):
                 yaml_data[key] = process_yaml_data(yaml_data[key], reference_path)
             else:
                 if isinstance(yaml_data[key], str):
                     for old_path, new_path in reference_path:
```

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/integration.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/lint.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/pycodestyle.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/pytest.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/LICENSE.md` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/LICENSE.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/README.md` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/README.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/docs/index.md` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/docs/index.md`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/images/hydragenetics.png` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/images/hydragenetics.png`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/mkdocs.yaml` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml` & `hydra-genetics-1.2.0/hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -3,34 +3,44 @@
 properties:
   sample:
     type: string
     description: sample id
   type:
     type: string
     description: type of sample (N|T|R)
+    pattern: ^(N|T|R)$
   platform:
     type: string
     description: sequence platform that have been used to generate data, ex NextSeq
+  machine: 
+    type: string
+    description: machine id
   flowcell:
     type: string
     description: flowcell id
+  barcode:
+    type: string
+    description: flowcell barcode
+    pattern: "^[A-Z+-]+$"
   lane:
     type: string
     description: lane number
   fastq1:
     type: string
     description: absolute path to R1 fastq file
   fastq2:
     type: string
     description: absolute path to R2 fastq file
   adapter:
     type: string
     description: one or more sequence, separated by ","
 required:
   - adapter
+  - barcode
   - fastq1
   - fastq2
   - flowcell
   - lane
   - platform
+  - machine
   - sample
   - type
```

### Comparing `hydra-genetics-1.1.0/hydra_genetics/rule-template/config.schema.yaml` & `hydra-genetics-1.2.0/hydra_genetics/rule-template/config.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/rule-template/resources.schema.yaml` & `hydra-genetics-1.2.0/hydra_genetics/rule-template/resources.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/rule-template/rules.schema.yaml` & `hydra-genetics-1.2.0/hydra_genetics/rule-template/rules.schema.yaml`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/rule-template/skeleton_rule.smk` & `hydra-genetics-1.2.0/hydra_genetics/rule-template/skeleton_rule.smk`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/utils/io/chr.py` & `hydra-genetics-1.2.0/hydra_genetics/utils/io/chr.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/utils/io/hotspot.py` & `hydra-genetics-1.2.0/hydra_genetics/utils/io/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/utils/io/hotspot_report.py` & `hydra-genetics-1.2.0/hydra_genetics/utils/io/hotspot_report.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/utils/io/multibp.py` & `hydra-genetics-1.2.0/hydra_genetics/utils/io/multibp.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/utils/io/utils.py` & `hydra-genetics-1.2.0/hydra_genetics/utils/io/utils.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/utils/misc.py` & `hydra-genetics-1.2.0/hydra_genetics/utils/misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/utils/models/hotspot.py` & `hydra-genetics-1.2.0/hydra_genetics/utils/models/hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/utils/samples.py` & `hydra-genetics-1.2.0/hydra_genetics/utils/samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics/utils/units.py` & `hydra-genetics-1.2.0/hydra_genetics/utils/units.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/hydra_genetics.egg-info/PKG-INFO` & `hydra-genetics-1.2.0/hydra_genetics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydra-genetics
-Version: 1.1.0
+Version: 1.2.0
 Summary: Helper tools for use with hydra-genetics pipelines.
 Home-page: https://github.com/hydra-genetics/tools
 Author: Patrik Smeds
 Author-email: patrik.smeds@scilifelab.uu.se
 License: GPL-3
 Keywords: hydra-genetics,snakemake,bioinformatics,workflow,pipeline,clinical,biology,sequencing,NGS,next generation sequencing
 Description-Content-Type: text/markdown
```

### Comparing `hydra-genetics-1.1.0/hydra_genetics.egg-info/SOURCES.txt` & `hydra-genetics-1.2.0/hydra_genetics.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 hydra_genetics.egg-info/not-zip-safe
 hydra_genetics.egg-info/requires.txt
 hydra_genetics.egg-info/top_level.txt
 hydra_genetics/commands/__init__.py
 hydra_genetics/commands/create.py
 hydra_genetics/commands/prep_pipeline_env.py
 hydra_genetics/pipeline-template/.gitignore
+hydra_genetics/pipeline-template/.readthedocs.yaml
 hydra_genetics/pipeline-template/LICENSE.md
 hydra_genetics/pipeline-template/README.md
 hydra_genetics/pipeline-template/mkdocs.yaml
 hydra_genetics/pipeline-template/requirements.test.txt
 hydra_genetics/pipeline-template/requirements.txt
 hydra_genetics/pipeline-template/.github/CODEOWNERS
 hydra_genetics/pipeline-template/.github/PULL_REQUEST_TEMPLATE.md
@@ -39,30 +40,30 @@
 hydra_genetics/pipeline-template/.github/workflows/snakefmt.yaml
 hydra_genetics/pipeline-template/.github/workflows/snakemake-dry-run.yaml
 hydra_genetics/pipeline-template/.tests/integration/config.yaml
 hydra_genetics/pipeline-template/.tests/integration/resources.yaml
 hydra_genetics/pipeline-template/.tests/integration/samples.tsv
 hydra_genetics/pipeline-template/.tests/integration/units.tsv
 hydra_genetics/pipeline-template/config/config.yaml
+hydra_genetics/pipeline-template/config/output_files.json
 hydra_genetics/pipeline-template/config/resources.yaml
 hydra_genetics/pipeline-template/config/samples.tsv
 hydra_genetics/pipeline-template/config/units.tsv
 hydra_genetics/pipeline-template/docs/extra.css
 hydra_genetics/pipeline-template/docs/index.md
 hydra_genetics/pipeline-template/docs/intro.md
 hydra_genetics/pipeline-template/docs/requirements.txt
 hydra_genetics/pipeline-template/docs/softwares.md
 hydra_genetics/pipeline-template/docs/includes/abbreviations.md
 hydra_genetics/pipeline-template/images/hydragenetics.png
 hydra_genetics/pipeline-template/workflow/Snakefile
 hydra_genetics/pipeline-template/workflow/notebooks/describe_jupyter_notebook.txt
-hydra_genetics/pipeline-template/workflow/report/describe_workflow.rst
 hydra_genetics/pipeline-template/workflow/rules/common.smk
-hydra_genetics/pipeline-template/workflow/rules/dummy.smk
 hydra_genetics/pipeline-template/workflow/schemas/config.schema.yaml
+hydra_genetics/pipeline-template/workflow/schemas/output_files.schema.yaml
 hydra_genetics/pipeline-template/workflow/schemas/resources.schema.yaml
 hydra_genetics/pipeline-template/workflow/schemas/rules.schema.yaml
 hydra_genetics/pipeline-template/workflow/schemas/samples.schema.yaml
 hydra_genetics/pipeline-template/workflow/schemas/units.schema.yaml
 hydra_genetics/pipeline-template/workflow/scripts/dummy.py
 hydra_genetics/pipeline-template/workflow/scripts/test_dummy.py
 hydra_genetics/rule-template/config.schema.yaml
```

### Comparing `hydra-genetics-1.1.0/setup.py` & `hydra-genetics-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/tests/utils/io/test_hotspot.py` & `hydra-genetics-1.2.0/tests/utils/io/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/tests/utils/io/test_mutations_report.py` & `hydra-genetics-1.2.0/tests/utils/io/test_mutations_report.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/tests/utils/models/test_hotspot.py` & `hydra-genetics-1.2.0/tests/utils/models/test_hotspot.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/tests/utils/test_misc.py` & `hydra-genetics-1.2.0/tests/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/tests/utils/test_resources.py` & `hydra-genetics-1.2.0/tests/utils/test_resources.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/tests/utils/test_samples.py` & `hydra-genetics-1.2.0/tests/utils/test_samples.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/tests/utils/test_units.py` & `hydra-genetics-1.2.0/tests/utils/test_units.py`

 * *Files identical despite different names*

### Comparing `hydra-genetics-1.1.0/versioneer.py` & `hydra-genetics-1.2.0/versioneer.py`

 * *Files identical despite different names*

