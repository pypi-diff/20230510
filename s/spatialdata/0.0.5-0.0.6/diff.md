# Comparing `tmp/spatialdata-0.0.5.tar.gz` & `tmp/spatialdata-0.0.6.tar.gz`

## Comparing `spatialdata-0.0.5.tar` & `spatialdata-0.0.6.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.bumpversion.cfg
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.editorconfig
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.gitmodules
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.mypy.ini
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.readthedocs.yaml
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata-0.0.5/_version.py
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.github/codecov.yml
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.github/workflows/build.yaml
--rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.github/workflows/test_and_deploy.yaml
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/Makefile
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/api.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/changelog.md
--rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/conf.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/contributing.md
--rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/design_doc.md
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/index.md
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/installation.md
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/references.bib
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/references.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/_static/.gitkeep
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/_static/css/custom.css
--rw-r--r--   0        0        0    82458 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/_static/img/spatialdata_horizontal.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/_templates/autosummary/base.rst
--rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/_templates/autosummary/function.rst
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata-0.0.5/docs/extensions/typed_returns.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/__init__.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/__main__.py
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_compat.py
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_logging.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_types.py
--rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_utils.py
--rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/__init__.py
--rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/concatenate.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/data_extent.py
--rw-r--r--   0        0        0    62204 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/spatialdata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/operations/__init__.py
--rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/operations/aggregate.py
--rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/operations/rasterize.py
--rw-r--r--   0        0        0    17392 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/operations/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/query/__init__.py
--rw-r--r--   0        0        0    25187 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_core/query/spatial_query.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_io/__init__.py
--rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_io/_utils.py
--rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_io/format.py
--rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_io/io_points.py
--rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_io/io_raster.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_io/io_shapes.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_io/io_table.py
--rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/_io/io_zarr.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/dataloader/__init__.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/dataloader/_utils.py
--rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/dataloader/datasets.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/models/__init__.py
--rw-r--r--   0        0        0     5646 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/models/_utils.py
--rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/models/models.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/transformations/__init__.py
--rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/transformations/_utils.py
--rw-r--r--   0        0        0    19686 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/transformations/operations.py
--rw-r--r--   0        0        0    35159 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/transformations/transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/transformations/ngff/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/transformations/ngff/_utils.py
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/transformations/ngff/ngff_coordinate_system.py
--rw-r--r--   0        0        0    48237 2020-02-02 00:00:00.000000 spatialdata-0.0.5/src/spatialdata/transformations/ngff/ngff_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/core/operations/__init__.py
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/core/operations/test_aggregations.py
--rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/core/operations/test_rasterize.py
--rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/core/operations/test_spatialdata_operations.py
--rw-r--r--   0        0        0    19768 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/core/operations/test_transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/core/query/__init__.py
--rw-r--r--   0        0        0    14078 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/core/query/test_spatial_query.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/data/multipolygon.json
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/data/points.json
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/data/polygon.json
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/dataloader/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/dataloader/test_datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/dataloader/test_transforms.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/datasets/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/datasets/test_datasets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/io/__init__.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/io/test_format.py
--rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/io/test_readwrite.py
--rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/io/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/models/__init__.py
--rw-r--r--   0        0        0    14805 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/models/test_models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/transformations/__init__.py
--rw-r--r--   0        0        0    28221 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/transformations/test_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/transformations/ngff/__init__.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/transformations/ngff/conftest.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/transformations/ngff/test_ngff_coordinate_system.py
--rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/transformations/ngff/test_ngff_transformations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/utils/__init__.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 spatialdata-0.0.5/tests/utils/test_element_utils.py
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 spatialdata-0.0.5/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata-0.0.5/LICENSE
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 spatialdata-0.0.5/README.md
--rw-r--r--   0        0        0     4737 2020-02-02 00:00:00.000000 spatialdata-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     6090 2020-02-02 00:00:00.000000 spatialdata-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.bumpversion.cfg
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.editorconfig
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.gitmodules
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.mypy.ini
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.readthedocs.yaml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 spatialdata-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 spatialdata-0.0.6/_version.py
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.github/codecov.yml
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     2890 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.github/workflows/test_and_deploy.yaml
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/Makefile
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/api.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/changelog.md
+-rw-r--r--   0        0        0     4823 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/conf.py
+-rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/contributing.md
+-rw-r--r--   0        0        0    33373 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/design_doc.md
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/index.md
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/installation.md
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/references.bib
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/references.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_static/.gitkeep
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_static/css/custom.css
+-rw-r--r--   0        0        0    82458 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_static/img/spatialdata_horizontal.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_templates/autosummary/base.rst
+-rw-r--r--   0        0        0     1034 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/_templates/autosummary/function.rst
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 spatialdata-0.0.6/docs/extensions/typed_returns.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/__init__.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/__main__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_compat.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_logging.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_types.py
+-rw-r--r--   0        0        0     6823 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_utils.py
+-rw-r--r--   0        0        0     7375 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/__init__.py
+-rw-r--r--   0        0        0     5171 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/concatenate.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/data_extent.py
+-rw-r--r--   0        0        0    62204 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/spatialdata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/operations/__init__.py
+-rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/operations/aggregate.py
+-rw-r--r--   0        0        0    21113 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/operations/rasterize.py
+-rw-r--r--   0        0        0    17392 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/operations/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/query/__init__.py
+-rw-r--r--   0        0        0    30057 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_core/query/spatial_query.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/__init__.py
+-rw-r--r--   0        0        0    10215 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/_utils.py
+-rw-r--r--   0        0        0     7267 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/format.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_points.py
+-rw-r--r--   0        0        0     9703 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_raster.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_shapes.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_table.py
+-rw-r--r--   0        0        0     3143 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/_io/io_zarr.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/dataloader/__init__.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/dataloader/_utils.py
+-rw-r--r--   0        0        0     7066 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/dataloader/datasets.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/models/__init__.py
+-rw-r--r--   0        0        0     8150 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/models/_utils.py
+-rw-r--r--   0        0        0    28610 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/models/models.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/__init__.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/_utils.py
+-rw-r--r--   0        0        0    19686 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/operations.py
+-rw-r--r--   0        0        0    35159 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/ngff/_utils.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/ngff/ngff_coordinate_system.py
+-rw-r--r--   0        0        0    48237 2020-02-02 00:00:00.000000 spatialdata-0.0.6/src/spatialdata/transformations/ngff/ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/__init__.py
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/test_aggregations.py
+-rw-r--r--   0        0        0     3441 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/test_rasterize.py
+-rw-r--r--   0        0        0    10928 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/test_spatialdata_operations.py
+-rw-r--r--   0        0        0    19768 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/operations/test_transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/query/__init__.py
+-rw-r--r--   0        0        0    14078 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/core/query/test_spatial_query.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/data/multipolygon.json
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/data/points.json
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/data/polygon.json
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/dataloader/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/dataloader/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/dataloader/test_transforms.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/datasets/__init__.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/datasets/test_datasets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/io/__init__.py
+-rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/io/test_format.py
+-rw-r--r--   0        0        0    14718 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/io/test_readwrite.py
+-rw-r--r--   0        0        0     3814 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/io/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/models/__init__.py
+-rw-r--r--   0        0        0    14805 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/models/test_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/__init__.py
+-rw-r--r--   0        0        0    28221 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/test_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/ngff/__init__.py
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/ngff/conftest.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/ngff/test_ngff_coordinate_system.py
+-rw-r--r--   0        0        0    15405 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/transformations/ngff/test_ngff_transformations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 spatialdata-0.0.6/tests/utils/test_element_utils.py
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 spatialdata-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 spatialdata-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 spatialdata-0.0.6/README.md
+-rw-r--r--   0        0        0     4749 2020-02-02 00:00:00.000000 spatialdata-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     6358 2020-02-02 00:00:00.000000 spatialdata-0.0.6/PKG-INFO
```

### Comparing `spatialdata-0.0.5/.mypy.ini` & `spatialdata-0.0.6/.mypy.ini`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/.pre-commit-config.yaml` & `spatialdata-0.0.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/.github/workflows/build.yaml` & `spatialdata-0.0.6/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/.github/workflows/test_and_deploy.yaml` & `spatialdata-0.0.6/.github/workflows/test_and_deploy.yaml`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/Makefile` & `spatialdata-0.0.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/api.md` & `spatialdata-0.0.6/docs/api.md`

 * *Files 4% similar despite different names*

```diff
@@ -62,14 +62,16 @@
 .. autosummary::
     :toctree: generated
 
     get_model
     SpatialElement
     get_axes_names
     get_spatial_axes
+    points_geopandas_to_dask_dataframe
+    points_dask_dataframe_to_geopandas
 ```
 
 ## Transformations
 
 The transformations that can be defined between elements and coordinate systems in `SpatialData`.
 
 ```{eval-rst}
```

### Comparing `spatialdata-0.0.5/docs/conf.py` & `spatialdata-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/contributing.md` & `spatialdata-0.0.6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/design_doc.md` & `spatialdata-0.0.6/docs/design_doc.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/index.md` & `spatialdata-0.0.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/installation.md` & `spatialdata-0.0.6/docs/installation.md`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/references.bib` & `spatialdata-0.0.6/docs/references.bib`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/_static/css/custom.css` & `spatialdata-0.0.6/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/_static/img/spatialdata_horizontal.png` & `spatialdata-0.0.6/docs/_static/img/spatialdata_horizontal.png`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/_templates/autosummary/class.rst` & `spatialdata-0.0.6/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/docs/extensions/typed_returns.py` & `spatialdata-0.0.6/docs/extensions/typed_returns.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/__init__.py` & `spatialdata-0.0.6/src/spatialdata/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,23 +14,24 @@
     "transformations",
     "dataloader",
     "concatenate",
     "rasterize",
     "transform",
     "aggregate",
     "bounding_box_query",
+    "polygon_query",
     "SpatialData",
     "read_zarr",
     "unpad_raster",
     "save_transformations",
 ]
 
 from spatialdata import dataloader, models, transformations
 from spatialdata._core.concatenate import concatenate
 from spatialdata._core.operations.aggregate import aggregate
 from spatialdata._core.operations.rasterize import rasterize
 from spatialdata._core.operations.transform import transform
-from spatialdata._core.query.spatial_query import bounding_box_query
+from spatialdata._core.query.spatial_query import bounding_box_query, polygon_query
 from spatialdata._core.spatialdata import SpatialData
 from spatialdata._io._utils import save_transformations
 from spatialdata._io.io_zarr import read_zarr
 from spatialdata._utils import unpad_raster
```

### Comparing `spatialdata-0.0.5/src/spatialdata/__main__.py` & `spatialdata-0.0.6/src/spatialdata/__main__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_compat.py` & `spatialdata-0.0.6/src/spatialdata/_compat.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_logging.py` & `spatialdata-0.0.6/src/spatialdata/_logging.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_utils.py` & `spatialdata-0.0.6/src/spatialdata/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/datasets.py` & `spatialdata-0.0.6/src/spatialdata/datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_core/concatenate.py` & `spatialdata-0.0.6/src/spatialdata/_core/concatenate.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_core/data_extent.py` & `spatialdata-0.0.6/src/spatialdata/_core/data_extent.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_core/spatialdata.py` & `spatialdata-0.0.6/src/spatialdata/_core/spatialdata.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_core/operations/aggregate.py` & `spatialdata-0.0.6/src/spatialdata/_core/operations/aggregate.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_core/operations/rasterize.py` & `spatialdata-0.0.6/src/spatialdata/_core/operations/rasterize.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_core/operations/transform.py` & `spatialdata-0.0.6/src/spatialdata/_core/operations/transform.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_io/_utils.py` & `spatialdata-0.0.6/src/spatialdata/_io/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_io/format.py` & `spatialdata-0.0.6/src/spatialdata/_io/format.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_io/io_points.py` & `spatialdata-0.0.6/src/spatialdata/_io/io_points.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_io/io_raster.py` & `spatialdata-0.0.6/src/spatialdata/_io/io_raster.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_io/io_shapes.py` & `spatialdata-0.0.6/src/spatialdata/_io/io_shapes.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_io/io_table.py` & `spatialdata-0.0.6/src/spatialdata/_io/io_table.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/_io/io_zarr.py` & `spatialdata-0.0.6/src/spatialdata/_io/io_zarr.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/dataloader/_utils.py` & `spatialdata-0.0.6/src/spatialdata/dataloader/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/dataloader/datasets.py` & `spatialdata-0.0.6/src/spatialdata/dataloader/datasets.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/models/__init__.py` & `spatialdata-0.0.6/src/spatialdata/models/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,14 +4,16 @@
     C,
     SpatialElement,
     X,
     Y,
     Z,
     get_axes_names,
     get_spatial_axes,
+    points_dask_dataframe_to_geopandas,
+    points_geopandas_to_dask_dataframe,
     validate_axes,
     validate_axis_name,
 )
 from spatialdata.models.models import (
     Image2DModel,
     Image3DModel,
     Labels2DModel,
@@ -36,8 +38,10 @@
     "validate_axes",
     "validate_axis_name",
     "X",
     "Y",
     "Z",
     "C",
     "get_axes_names",
+    "points_geopandas_to_dask_dataframe",
+    "points_dask_dataframe_to_geopandas",
 ]
```

### Comparing `spatialdata-0.0.5/src/spatialdata/models/models.py` & `spatialdata-0.0.6/src/spatialdata/models/models.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/transformations/__init__.py` & `spatialdata-0.0.6/src/spatialdata/transformations/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/transformations/_utils.py` & `spatialdata-0.0.6/src/spatialdata/transformations/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/transformations/operations.py` & `spatialdata-0.0.6/src/spatialdata/transformations/operations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/transformations/transformations.py` & `spatialdata-0.0.6/src/spatialdata/transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/transformations/ngff/_utils.py` & `spatialdata-0.0.6/src/spatialdata/transformations/ngff/_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/transformations/ngff/ngff_coordinate_system.py` & `spatialdata-0.0.6/src/spatialdata/transformations/ngff/ngff_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/src/spatialdata/transformations/ngff/ngff_transformations.py` & `spatialdata-0.0.6/src/spatialdata/transformations/ngff/ngff_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/conftest.py` & `spatialdata-0.0.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/core/operations/test_aggregations.py` & `spatialdata-0.0.6/tests/core/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/core/operations/test_rasterize.py` & `spatialdata-0.0.6/tests/core/operations/test_rasterize.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/core/operations/test_spatialdata_operations.py` & `spatialdata-0.0.6/tests/core/operations/test_spatialdata_operations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/core/operations/test_transform.py` & `spatialdata-0.0.6/tests/core/operations/test_transform.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/core/query/test_spatial_query.py` & `spatialdata-0.0.6/tests/core/query/test_spatial_query.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/data/multipolygon.json` & `spatialdata-0.0.6/tests/data/multipolygon.json`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/data/polygon.json` & `spatialdata-0.0.6/tests/data/polygon.json`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/io/test_format.py` & `spatialdata-0.0.6/tests/io/test_format.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/io/test_readwrite.py` & `spatialdata-0.0.6/tests/io/test_readwrite.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/io/test_utils.py` & `spatialdata-0.0.6/tests/io/test_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/models/test_models.py` & `spatialdata-0.0.6/tests/models/test_models.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/transformations/test_transformations.py` & `spatialdata-0.0.6/tests/transformations/test_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/transformations/ngff/conftest.py` & `spatialdata-0.0.6/tests/transformations/ngff/conftest.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/transformations/ngff/test_ngff_coordinate_system.py` & `spatialdata-0.0.6/tests/transformations/ngff/test_ngff_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/transformations/ngff/test_ngff_transformations.py` & `spatialdata-0.0.6/tests/transformations/ngff/test_ngff_transformations.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/tests/utils/test_element_utils.py` & `spatialdata-0.0.6/tests/utils/test_element_utils.py`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/LICENSE` & `spatialdata-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialdata-0.0.5/README.md` & `spatialdata-0.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ## Contact
 
 For questions and help requests, you can reach out in the [scverse discourse][scverse-discourse].
 If you found a bug, please use the [issue tracker][issue-tracker].
 
 ## Citation
 
-> t.b.a
+[L Marconato*, G Palla*, KA Yamauchi*, I Virshup*, E Heidari, T Treis, M Toth, R Shrestha, H Vöhringer, W Huber, M Gerstung, J Moore, FJ Theis, O Stegle, bioRxiv, 2023](https://www.biorxiv.org/content/10.1101/2023.05.05.539647v1). \* = equal contribution
 
 <!-- Links -->
 
 [scverse-discourse]: https://discourse.scverse.org/
 [issue-tracker]: https://github.com/scverse/spatialdata/issues
 [changelog]: https://spatialdata.readthedocs.io/latest/changelog.html
 [design doc]: https://scverse-spatialdata.readthedocs.io/en/latest/design_doc.html
```

### Comparing `spatialdata-0.0.5/pyproject.toml` & `spatialdata-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "shapely>=2.0.1",
     "rich",
     "pyarrow",
     "typing_extensions>=4.0.0",
     "dask-image",
     "networkx",
     "xarray-spatial>=0.3.5",
+    "tqdm",
 ]
 
 [project.optional-dependencies]
 dev = [
     "bump2version",
 ]
 docs = [
```

### Comparing `spatialdata-0.0.5/PKG-INFO` & `spatialdata-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialdata
-Version: 0.0.5
+Version: 0.0.6
 Summary: Spatial data format.
 Project-URL: Documentation, https://spatialdata.readthedocs.io/
 Project-URL: Source, https://github.com/scverse/spatialdata.git
 Project-URL: Home-page, https://github.com/scverse/spatialdata.git
 Author: scverse
 Maintainer-email: scverse <giov.pll@gmail.com>
 License: BSD 3-Clause License
@@ -46,14 +46,15 @@
 Requires-Dist: numpy
 Requires-Dist: ome-zarr>=0.7.0
 Requires-Dist: pyarrow
 Requires-Dist: pygeos
 Requires-Dist: rich
 Requires-Dist: shapely>=2.0.1
 Requires-Dist: spatial-image>=0.3.0
+Requires-Dist: tqdm
 Requires-Dist: typing-extensions>=4.0.0
 Requires-Dist: xarray
 Requires-Dist: xarray-schema
 Requires-Dist: xarray-spatial>=0.3.5
 Requires-Dist: zarr
 Provides-Extra: dev
 Requires-Dist: bump2version; extra == 'dev'
@@ -112,15 +113,15 @@
 ## Contact
 
 For questions and help requests, you can reach out in the [scverse discourse][scverse-discourse].
 If you found a bug, please use the [issue tracker][issue-tracker].
 
 ## Citation
 
-> t.b.a
+[L Marconato*, G Palla*, KA Yamauchi*, I Virshup*, E Heidari, T Treis, M Toth, R Shrestha, H Vöhringer, W Huber, M Gerstung, J Moore, FJ Theis, O Stegle, bioRxiv, 2023](https://www.biorxiv.org/content/10.1101/2023.05.05.539647v1). \* = equal contribution
 
 <!-- Links -->
 
 [scverse-discourse]: https://discourse.scverse.org/
 [issue-tracker]: https://github.com/scverse/spatialdata/issues
 [changelog]: https://spatialdata.readthedocs.io/latest/changelog.html
 [design doc]: https://scverse-spatialdata.readthedocs.io/en/latest/design_doc.html
```

