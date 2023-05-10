# Comparing `tmp/gpt-review-0.8.0rc597.post1.tar.gz` & `tmp/gpt-review-0.8.0rc622.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.8.0rc597.post1.tar", last modified: Tue May  9 23:05:57 2023, max compression
+gzip compressed data, was "gpt-review-0.8.0rc622.post1.tar", last modified: Wed May 10 18:50:13 2023, max compression
```

## Comparing `gpt-review-0.8.0rc597.post1.tar` & `gpt-review-0.8.0rc622.post1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0      336 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1995 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4246 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1851 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/README.md
--rw-r--r--   0        0        0     3561 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/action.yml
--rw-r--r--   0        0        0      218 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/config.summary.template.yml
--rw-r--r--   0        0        0     8346 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-09 23:05:57.039929 gpt-review-0.8.0rc597.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-09 23:05:57.039929 gpt-review-0.8.0rc597.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0     8752 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     2772 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     5769 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     3671 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0      788 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     8994 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      523 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      568 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0       33 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/__init__.py
--rw-r--r--   0        0        0      529 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_bugs.py
--rw-r--r--   0        0        0      524 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_coverage.py
--rw-r--r--   0        0        0     1177 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_prompt.py
--rw-r--r--   0        0        0      516 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_summary.py
--rw-r--r--   0        0        0      218 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     3942 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/mock.diff
--rw-r--r--   0        0        0      612 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_github.py
--rw-r--r--   0        0        0     5521 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1286 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_report.py
--rw-r--r--   0        0        0      420 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_review.py
--rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.8.0rc597.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1995 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4246 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1851 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.pypirc
+-rw-r--r--   0        0        0      450 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/action.yml
+-rw-r--r--   0        0        0      218 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/config.summary.template.yml
+-rw-r--r--   0        0        0     8501 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-10 18:50:12.809665 gpt-review-0.8.0rc622.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-10 18:50:12.809665 gpt-review-0.8.0rc622.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0     8772 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     2772 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5788 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     5769 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     3671 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0      788 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     8994 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      523 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      568 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/prompts/_bugs.py
+-rw-r--r--   0        0        0      524 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/prompts/_coverage.py
+-rw-r--r--   0        0        0     1177 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      516 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/src/gpt_review/prompts/_summary.py
+-rw-r--r--   0        0        0      218 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     5124 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/mock.diff
+-rw-r--r--   0        0        0      612 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1443 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5612 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1286 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/test_report.py
+-rw-r--r--   0        0        0      797 2023-05-10 18:50:01.697614 gpt-review-0.8.0rc622.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.8.0rc622.post1/PKG-INFO
```

### Comparing `gpt-review-0.8.0rc597.post1/.devcontainer/devcontainer.json` & `gpt-review-0.8.0rc622.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.8.0rc622.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.github/dependabot.yml` & `gpt-review-0.8.0rc622.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.github/pull_request_template.md` & `gpt-review-0.8.0rc622.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.github/workflows/codeql.yml` & `gpt-review-0.8.0rc622.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.8.0rc622.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.8.0rc622.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.github/workflows/python.yml` & `gpt-review-0.8.0rc622.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.github/workflows/test-action.yml` & `gpt-review-0.8.0rc622.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.gitignore` & `gpt-review-0.8.0rc622.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/.vscode/settings.json` & `gpt-review-0.8.0rc622.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/LICENSE` & `gpt-review-0.8.0rc622.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/README.md` & `gpt-review-0.8.0rc622.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/action.yml` & `gpt-review-0.8.0rc622.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/pyproject.toml` & `gpt-review-0.8.0rc622.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,20 @@
 
 [tool.black]
 line-length = 120
 fast = true
 
 [tool.coverage.run]
 branch = true
+omit = [
+    # Omitting files that can not be covered by tests
+    "src/gpt/__main__.py",
+    "src/gpt_review/__main__.py",
+    "src/gpt_review/main.py"
+]
 
 [tool.coverage.report]
 fail_under = 100
 
 [tool.flake8]
 max-line-length = 120
 select = "F,E,W,B,B901,B902,B903"
```

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/_ask.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/_ask.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     """
     openai.api_type = os.environ["OPENAI_API_TYPE"] = "azure"
     openai.api_version = os.environ["OPENAI_API_VERSION"] = "2023-03-15-preview"
 
     if os.getenv("AZURE_OPENAI_API"):
         openai.api_base = os.environ["OPENAI_API_BASE"] = os.getenv("AZURE_OPENAI_API")  # type: ignore
         openai.api_key = os.environ["OPENAI_API_KEY"] = os.getenv("AZURE_OPENAI_API_KEY")  # type: ignore
-    else:
+    else:  # pragma: no cover
         kv_client = SecretClient(
             vault_url=os.getenv("AZURE_KEY_VAULT_URL", DEFAULT_KEY_VAULT), credential=DefaultAzureCredential()
         )
         openai.api_base = os.environ["OPENAI_API_BASE"] = kv_client.get_secret("azure-open-ai").value  # type: ignore
         openai.api_key = os.environ["OPENAI_API_KEY"] = kv_client.get_secret("azure-openai-key").value  # type: ignore
```

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/_git.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/_github.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/_github.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,39 +41,34 @@
 
         response = requests.get(
             f"https://api.github.com/repos/{patch_repo}/pulls/{patch_pr}", headers=headers, timeout=10
         )
         return response.text
 
     @staticmethod
-    def _post_pr_comment(review, git_commit_hash=None, link=None, access_token=None) -> requests.Response:
+    def _post_pr_comment(review, git_commit_hash: str, link: str, access_token: str) -> requests.Response:
         """
         Post a comment to a PR.
 
         Args:
             review (str): The review.
             git_commit_hash (str): The git commit hash.
             link (str): The link to the PR.
             access_token (str): The GitHub access token.
 
         Returns:
             requests.Response: The response.
         """
-        git_commit_hash = git_commit_hash or os.getenv("GIT_COMMIT_HASH")
         data = {"body": review, "commit_id": git_commit_hash, "event": "COMMENT"}
         data = json.dumps(data)
 
-        pr_link = link or os.getenv("LINK")
-        if not isinstance(pr_link, str):
-            raise ValueError("PR link not found, set the LINK environment variable.")
-        owner = pr_link.split("/")[-4]
-        repo = pr_link.split("/")[-3]
-        pr_number = pr_link.split("/")[-1]
+        owner = link.split("/")[-4]
+        repo = link.split("/")[-3]
+        pr_number = link.split("/")[-1]
 
-        access_token = access_token or os.getenv("GITHUB_TOKEN")
         headers = {
             "Accept": "application/vnd.github+json",
             "authorization": f"Bearer {access_token}",
         }
         response = requests.get(
             f"https://api.github.com/repos/{owner}/{repo}/pulls/{pr_number}/reviews", headers=headers, timeout=10
         )
@@ -105,28 +100,39 @@
                 data=data,
                 timeout=10,
             )
         logging.debug(response.json())
         return response
 
     @staticmethod
-    def post_pr_summary(pr_patch) -> None:
-        """Get a review of a PR.
+    def post_pr_summary(pr_patch) -> Dict[str, str]:
+        """
+        Get a review of a PR.
+
         Args:
             pr_patch (str): The patch of the PR.
+
         Returns:
-            str: The review of the PR.
+            Dict[str, str]: The review.
         """
         review = _summarize_files(pr_patch)
         logging.debug(review)
 
-        if os.getenv("LINK"):
-            _GitHubClient._post_pr_comment(review)
-        else:
-            logging.warning("No PR to post too")
+        link = os.getenv("LINK")
+        git_commit_hash = os.getenv("GIT_COMMIT_HASH")
+        access_token = os.getenv("GITHUB_TOKEN")
+
+        if link and git_commit_hash and access_token:
+            _GitHubClient._post_pr_comment(
+                review=review, git_commit_hash=git_commit_hash, link=link, access_token=access_token
+            )
+            return {"response": "PR posted"}
+
+        logging.warning("No PR to post too")
+        return {"response": "No PR to post too"}
 
 
 def _github_review(repository=None, pull_request=None, access_token=None) -> Dict[str, str]:
     """Review GitHub PR with Open AI, and post response as a comment."""
     diff = _GitHubClient.get_pr_diff(repository, pull_request, access_token)
     _GitHubClient.post_pr_summary(diff)
     return {"response": "Review posted as a comment."}
```

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/_llama_index.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/_openai.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/_repository.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/_review.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/constants.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/main.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_bugs.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/prompts/_bugs.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_coverage.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/prompts/_coverage.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_prompt.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/prompts/_prompt.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_summary.py` & `gpt-review-0.8.0rc622.post1/src/gpt_review/prompts/_summary.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/tests/mock.diff` & `gpt-review-0.8.0rc622.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/tests/test_git.py` & `gpt-review-0.8.0rc622.post1/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/tests/test_github.py` & `gpt-review-0.8.0rc622.post1/tests/test_github.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,37 +7,42 @@
     """Test the GitHub API call."""
     diff = _GitHubClient.get_pr_diff(patch_repo=patch_repo, patch_pr=patch_pr)
     assert diff.startswith(starts_with)
 
 
 def post_pr_comment_test() -> None:
     """Test the GitHub API call."""
-    response = _GitHubClient._post_pr_comment(
-        "test",
-        git_commit_hash="a9da0c1e65f1102bc2ae16abed7b6a66400a5bde",
-        link="https://github.com/microsoft/gpt-review/pull/1",
-    )
+    response = _GitHubClient.post_pr_summary("test")
     assert response
 
 
-@pytest.mark.skip(reason="Creds for action missing on build server")
 @pytest.mark.integration
-def test_int_pr_diff() -> None:
+def test_int_pr_diff(mock_github) -> None:
     """Integration Test for GitHub API diff call."""
-    get_pr_diff_test("diff --git a/.devcontainer/Dockerfile b/.devcontainer/Dockerfile", "microsoft/gpt-review", 1)
+    get_pr_diff_test("diff --git a/README.md b/README.md", "microsoft/gpt-review", 1)
 
 
-def test_pr_diff(mock_github) -> None:
+def test_pr_diff(mock_openai, mock_github) -> None:
     """Unit Test for GitHub API diff call."""
     get_pr_diff_test("diff --git a/README.md b/README.md")
 
 
-@pytest.mark.skip(reason="Creds for action missing on build server")
 @pytest.mark.integration
-def test_int_pr_comment() -> None:
+def test_int_pr_comment(mock_github) -> None:
     """Integration Test for GitHub API comment call."""
     post_pr_comment_test()
 
 
-def test_pr_comment(mock_github) -> None:
+@pytest.mark.integration
+def test_int_pr_update(mock_github, mock_github_comment) -> None:
+    """Integration Test for updating GitHub API comment call."""
+    post_pr_comment_test()
+
+
+def test_pr_comment(mock_openai, mock_github) -> None:
     """Unit Test for GitHub API comment call."""
     post_pr_comment_test()
+
+
+def test_pr_update(mock_openai, mock_github, mock_github_comment) -> None:
+    """Unit Test for updating GitHub API comment call."""
+    post_pr_comment_test()
```

### Comparing `gpt-review-0.8.0rc597.post1/tests/test_gpt_cli.py` & `gpt-review-0.8.0rc622.post1/tests/test_gpt_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     # CLICase("git commit --gpt4"),
 ]
 
 REVIEW_COMMANDS = [
     CLICase("review --help"),
     CLICase("review diff --help"),
     CLICase("review diff --diff tests/mock.diff --config tests/config.summary.test.yml"),
+    CLICase("review diff --diff tests/mock.diff --config tests/config.summary.extra.yml"),
 ]
 
 ARGS = ROOT_COMMANDS + ASK_COMMANDS + GIT_COMMANDS + GITHUB_COMMANDS + REVIEW_COMMANDS
 ARGS_DICT = {arg.command: arg for arg in ARGS}
 
 MODULE_COMMANDS = [
     CLICase("python -m gpt --version"),
```

### Comparing `gpt-review-0.8.0rc597.post1/tests/test_llama_index.py` & `gpt-review-0.8.0rc622.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/tests/test_openai.py` & `gpt-review-0.8.0rc622.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/tests/test_report.py` & `gpt-review-0.8.0rc622.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc597.post1/PKG-INFO` & `gpt-review-0.8.0rc622.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.8.0rc597.post1
+Version: 0.8.0rc622.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.8.0rc597.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.8.0rc622.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

