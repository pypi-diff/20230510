# Comparing `tmp/amazon_codeguru_jupyterlab_extension-0.0.3.tar.gz` & `tmp/amazon_codeguru_jupyterlab_extension-1.0.0.tar.gz`

## Comparing `amazon_codeguru_jupyterlab_extension-0.0.3.tar` & `amazon_codeguru_jupyterlab_extension-1.0.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/.eslintignore
--rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/.eslintrc.js
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/.prettierrc
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/.stylelintrc
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/SECURITY.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/babel.config.js
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/jest.config.js
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/package.json
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/setup.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/tsconfig.json
--rw-r--r--   0        0        0   456516 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/yarn.lock
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/_version.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/cfg.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/codeguru.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/constants.py
--rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/diagnostics.py
--rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/plugin.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/package.json
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json
--rw-r--r--   0        0        0    12496 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/606.839cc39e93f88938c736.js
--rw-r--r--   0        0        0  1808896 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/67.c97baf8a498fda49350d.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/67.c97baf8a498fda49350d.js.LICENSE.txt
--rw-r--r--   0        0        0   125329 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/703.60e17cd520b0c3ad0f9c.js
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/703.60e17cd520b0c3ad0f9c.js.LICENSE.txt
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/747.ecd0ef12675f88068557.js
--rw-r--r--   0        0        0   225367 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/860.5abb378d41ad4395b0af.js
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/910.1ab01fa00a55e966d7e8.js
--rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.60903ee90e17dc8ffe5d.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/style.js
--rw-r--r--   0        0        0   128918 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0    24553 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/configuration/boto/codeguru-security/2018-05-10/service-2.json
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/schema/plugin.json
--rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/index.ts
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/svg.d.ts
--rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/components/About.tsx
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/components/CodeScanButton.tsx
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/components/CodeScanErrorPopup.tsx
--rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/components/CodeScanStatus.tsx
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/constants/icons.ts
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/constants/index.ts
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/constants/interface.ts
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/constants/policy.ts
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/constants/region.ts
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/src/utils/index.ts
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/style/index.css
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/style/index.js
--rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/style/icons/cg-icon.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/tests/conftest.py
--rw-r--r--   0        0        0    10760 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/tests/test_diagnostics.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/tests/test_plugin.py
--rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/tests/fixtures/converted.py
--rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/tests/fixtures/finding.json
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/tests/fixtures/simple.ipynb
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/tests/fixtures/simple.py
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/playwright.config.js
--rw-r--r--   0        0        0   125819 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/yarn.lock
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts
--rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/NOTICE
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/README.md
--rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.eslintignore
+-rw-r--r--   0        0        0     1026 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.eslintrc.js
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.prettierrc
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.stylelintrc
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/SECURITY.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/babel.config.js
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/jest.config.js
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/package.json
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/setup.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tsconfig.json
+-rw-r--r--   0        0        0   456516 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/yarn.lock
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/_version.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/cfg.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/codeguru.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/constants.py
+-rw-r--r--   0        0        0     8513 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/diagnostics.py
+-rw-r--r--   0        0        0     2646 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/plugin.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/package.json
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json
+-rw-r--r--   0        0        0    12496 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/606.839cc39e93f88938c736.js
+-rw-r--r--   0        0        0  1808896 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/67.c97baf8a498fda49350d.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/67.c97baf8a498fda49350d.js.LICENSE.txt
+-rw-r--r--   0        0        0   125329 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/703.60e17cd520b0c3ad0f9c.js
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/703.60e17cd520b0c3ad0f9c.js.LICENSE.txt
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/747.ecd0ef12675f88068557.js
+-rw-r--r--   0        0        0   225367 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/860.5abb378d41ad4395b0af.js
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/910.1ab01fa00a55e966d7e8.js
+-rw-r--r--   0        0        0     8178 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.60903ee90e17dc8ffe5d.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/style.js
+-rw-r--r--   0        0        0   128918 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0    24553 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/configuration/boto/codeguru-security/2018-05-10/service-2.json
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/schema/plugin.json
+-rw-r--r--   0        0        0     6495 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/index.ts
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/svg.d.ts
+-rw-r--r--   0        0        0     5858 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/components/About.tsx
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanButton.tsx
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanErrorPopup.tsx
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanStatus.tsx
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/icons.ts
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/index.ts
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/interface.ts
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/policy.ts
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/constants/region.ts
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/src/utils/index.ts
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/style/index.css
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/style/index.js
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/style/icons/cg-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0    10760 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/test_diagnostics.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     1850 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/converted.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/finding.json
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/simple.ipynb
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/simple.py
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0   125819 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/yarn.lock
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts
+-rw-r--r--   0        0        0     1668 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/NOTICE
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/README.md
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 amazon_codeguru_jupyterlab_extension-1.0.0/PKG-INFO
```

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/.eslintrc.js` & `amazon_codeguru_jupyterlab_extension-1.0.0/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/CONTRIBUTING.md` & `amazon_codeguru_jupyterlab_extension-1.0.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/jest.config.js` & `amazon_codeguru_jupyterlab_extension-1.0.0/jest.config.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/package.json` & `amazon_codeguru_jupyterlab_extension-1.0.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9736842105263158%*

 * *Differences: {"'version'": "'1.0.0'"}*

```diff
@@ -127,9 +127,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.0.3"
+    "version": "1.0.0"
 }
```

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/tsconfig.json` & `amazon_codeguru_jupyterlab_extension-1.0.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/yarn.lock` & `amazon_codeguru_jupyterlab_extension-1.0.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/codeguru.py` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/codeguru.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/diagnostics.py` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/diagnostics.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/parseNotebookIntoScript.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/plugin.py` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/plugin.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/package.json` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/package.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/package.json.orig`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/schemas/@aws/amazon-codeguru-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/606.839cc39e93f88938c736.js` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/606.839cc39e93f88938c736.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/67.c97baf8a498fda49350d.js` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/67.c97baf8a498fda49350d.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/703.60e17cd520b0c3ad0f9c.js` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/703.60e17cd520b0c3ad0f9c.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/747.ecd0ef12675f88068557.js` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/747.ecd0ef12675f88068557.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/860.5abb378d41ad4395b0af.js` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/860.5abb378d41ad4395b0af.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/910.1ab01fa00a55e966d7e8.js` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/910.1ab01fa00a55e966d7e8.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.60903ee90e17dc8ffe5d.js` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/remoteEntry.60903ee90e17dc8ffe5d.js`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/amazon_codeguru_jupyterlab_extension/labextension/static/third-party-licenses.json` & `amazon_codeguru_jupyterlab_extension-1.0.0/amazon_codeguru_jupyterlab_extension/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/configuration/boto/codeguru-security/2018-05-10/service-2.json` & `amazon_codeguru_jupyterlab_extension-1.0.0/configuration/boto/codeguru-security/2018-05-10/service-2.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/schema/plugin.json` & `amazon_codeguru_jupyterlab_extension-1.0.0/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/src/index.ts` & `amazon_codeguru_jupyterlab_extension-1.0.0/src/index.ts`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/src/components/About.tsx` & `amazon_codeguru_jupyterlab_extension-1.0.0/src/components/About.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/src/components/CodeScanButton.tsx` & `amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanButton.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/src/components/CodeScanErrorPopup.tsx` & `amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanErrorPopup.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/src/components/CodeScanStatus.tsx` & `amazon_codeguru_jupyterlab_extension-1.0.0/src/components/CodeScanStatus.tsx`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/style/base.css` & `amazon_codeguru_jupyterlab_extension-1.0.0/style/base.css`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/style/icons/cg-icon.svg` & `amazon_codeguru_jupyterlab_extension-1.0.0/style/icons/cg-icon.svg`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/tests/conftest.py` & `amazon_codeguru_jupyterlab_extension-1.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/tests/test_diagnostics.py` & `amazon_codeguru_jupyterlab_extension-1.0.0/tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/tests/test_plugin.py` & `amazon_codeguru_jupyterlab_extension-1.0.0/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/tests/fixtures/converted.py` & `amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/converted.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/tests/fixtures/finding.json` & `amazon_codeguru_jupyterlab_extension-1.0.0/tests/fixtures/finding.json`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/README.md` & `amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/jupyter_server_test_config.py` & `amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/yarn.lock` & `amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/yarn.lock`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts` & `amazon_codeguru_jupyterlab_extension-1.0.0/ui-tests/tests/amazon_codeguru_jupyterlab_extension.spec.ts`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/.gitignore` & `amazon_codeguru_jupyterlab_extension-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/LICENSE` & `amazon_codeguru_jupyterlab_extension-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/README.md` & `amazon_codeguru_jupyterlab_extension-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/pyproject.toml` & `amazon_codeguru_jupyterlab_extension-1.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amazon_codeguru_jupyterlab_extension-0.0.3/PKG-INFO` & `amazon_codeguru_jupyterlab_extension-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon_codeguru_jupyterlab_extension
-Version: 0.0.3
+Version: 1.0.0
 Summary: Security, code quality, and ML recommendations
 Project-URL: Homepage, https://github.com/aws/amazon-codeguru-jupyterlab-extension
 Project-URL: Bug Tracker, https://github.com/aws/amazon-codeguru-jupyterlab-extension/issues
 Project-URL: Repository, https://github.com/aws/amazon-codeguru-jupyterlab-extension.git
 License-File: LICENSE
 License-File: NOTICE
 Classifier: Framework :: Jupyter
```

