# Comparing `tmp/gpt-review-0.8.0rc591.post1.tar.gz` & `tmp/gpt-review-0.8.0rc597.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.8.0rc591.post1.tar", last modified: Tue May  9 22:24:25 2023, max compression
+gzip compressed data, was "gpt-review-0.8.0rc597.post1.tar", last modified: Tue May  9 23:05:57 2023, max compression
```

## Comparing `gpt-review-0.8.0rc591.post1.tar` & `gpt-review-0.8.0rc597.post1.tar`

### file list

```diff
@@ -1,46 +1,51 @@
--rw-r--r--   0        0        0      336 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1995 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4246 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1761 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1851 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.pypirc
--rw-r--r--   0        0        0      450 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.vscode/launch.json
--rw-r--r--   0        0        0     1125 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/LICENSE
--rw-r--r--   0        0        0     3251 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/README.md
--rw-r--r--   0        0        0     3561 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/action.yml
--rw-r--r--   0        0        0      218 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/config.summary.template.yml
--rw-r--r--   0        0        0     8346 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/pyproject.toml
--rw-r--r--   0        0        0        1 2023-05-09 22:24:24.908646 gpt-review-0.8.0rc591.post1/src/gpt/__init__.py
--rw-r--r--   0        0        0      171 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/src/gpt/__main__.py
--rw-r--r--   0        0        0      366 2023-05-09 22:24:24.908646 gpt-review-0.8.0rc591.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0      171 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/src/gpt_review/__main__.py
--rw-r--r--   0        0        0     8702 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     2772 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1441 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0     5769 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/src/gpt_review/_llama_index.py
--rw-r--r--   0        0        0     3671 2023-05-09 22:24:15.772692 gpt-review-0.8.0rc591.post1/src/gpt_review/_openai.py
--rw-r--r--   0        0        0      788 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     9707 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      523 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      568 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0      218 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/config.summary.test.yml
--rw-r--r--   0        0        0     3942 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/mock.diff
--rw-r--r--   0        0        0      462 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/test_github.py
--rw-r--r--   0        0        0     5521 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      684 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/test_llama_index.py
--rw-r--r--   0        0        0     1286 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/test_openai.py
--rw-r--r--   0        0        0     1015 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/test_report.py
--rw-r--r--   0        0        0      420 2023-05-09 22:24:15.776692 gpt-review-0.8.0rc591.post1/tests/test_review.py
--rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.8.0rc591.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1995 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4246 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1761 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1851 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.pypirc
+-rw-r--r--   0        0        0      450 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.vscode/launch.json
+-rw-r--r--   0        0        0     1125 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-09 23:05:48.823740 gpt-review-0.8.0rc597.post1/LICENSE
+-rw-r--r--   0        0        0     3251 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/README.md
+-rw-r--r--   0        0        0     3561 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/action.yml
+-rw-r--r--   0        0        0      218 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/config.summary.template.yml
+-rw-r--r--   0        0        0     8346 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/pyproject.toml
+-rw-r--r--   0        0        0        1 2023-05-09 23:05:57.039929 gpt-review-0.8.0rc597.post1/src/gpt/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt/__main__.py
+-rw-r--r--   0        0        0      366 2023-05-09 23:05:57.039929 gpt-review-0.8.0rc597.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/__main__.py
+-rw-r--r--   0        0        0     8752 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     2772 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1441 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0     5769 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_llama_index.py
+-rw-r--r--   0        0        0     3671 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_openai.py
+-rw-r--r--   0        0        0      788 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     8994 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      523 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      568 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0       33 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_bugs.py
+-rw-r--r--   0        0        0      524 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_coverage.py
+-rw-r--r--   0        0        0     1177 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_prompt.py
+-rw-r--r--   0        0        0      516 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/src/gpt_review/prompts/_summary.py
+-rw-r--r--   0        0        0      218 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/config.summary.test.yml
+-rw-r--r--   0        0        0     3942 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/mock.diff
+-rw-r--r--   0        0        0      612 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5521 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      684 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_llama_index.py
+-rw-r--r--   0        0        0     1286 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_openai.py
+-rw-r--r--   0        0        0     1015 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_report.py
+-rw-r--r--   0        0        0      420 2023-05-09 23:05:48.827740 gpt-review-0.8.0rc597.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5425 1970-01-01 00:00:00.000000 gpt-review-0.8.0rc597.post1/PKG-INFO
```

### Comparing `gpt-review-0.8.0rc591.post1/.devcontainer/devcontainer.json` & `gpt-review-0.8.0rc597.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.8.0rc597.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.github/dependabot.yml` & `gpt-review-0.8.0rc597.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.github/pull_request_template.md` & `gpt-review-0.8.0rc597.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.github/workflows/codeql.yml` & `gpt-review-0.8.0rc597.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.8.0rc597.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.8.0rc597.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.github/workflows/python.yml` & `gpt-review-0.8.0rc597.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.github/workflows/test-action.yml` & `gpt-review-0.8.0rc597.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.gitignore` & `gpt-review-0.8.0rc597.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/.vscode/settings.json` & `gpt-review-0.8.0rc597.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/LICENSE` & `gpt-review-0.8.0rc597.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/README.md` & `gpt-review-0.8.0rc597.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/action.yml` & `gpt-review-0.8.0rc597.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/pyproject.toml` & `gpt-review-0.8.0rc597.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/_ask.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/_ask.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     question: List[str],
     max_tokens: int = C.MAX_TOKENS_DEFAULT,
     temperature: float = C.TEMPERATURE_DEFAULT,
     top_p: float = C.TOP_P_DEFAULT,
     frequency_penalty: float = C.FREQUENCY_PENALTY_DEFAULT,
     presence_penalty: float = C.PRESENCE_PENALTY_DEFAULT,
     files: Optional[List[str]] = None,
+    messages=None,
     fast: bool = False,
     large: bool = False,
     directory: Optional[str] = None,
     required_exts: Optional[List[str]] = None,
     hidden: bool = False,
     recursive: bool = False,
     repository: Optional[str] = None,
@@ -98,14 +99,15 @@
             max_tokens=max_tokens,
             temperature=temperature,
             top_p=top_p,
             frequency_penalty=frequency_penalty,
             presence_penalty=presence_penalty,
             fast=fast,
             large=large,
+            messages=messages,
         )
     return {"response": response}
 
 
 def _load_azure_openai_context() -> None:
     """
     Load the Azure OpenAI context.
```

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/_git.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/_github.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/_llama_index.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/_openai.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/_repository.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/_review.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/_review.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,17 @@
 
 from knack.arguments import ArgumentsContext
 from knack import CLICommandsLoader
 from knack.commands import CommandGroup
 
 from gpt_review._ask import _ask
 from gpt_review._command import GPTCommandGroup
-
-SUMMARIZE_PROMPT = """Summarize the following file changed in a pull request submitted by a developer on GitHub,
-focusing on major modifications, additions, deletions, and any significant updates within the files. Do not include the
-file name in the summary and list the summary with bullet points"""
-TEST_COVERAGE_PROMPT = """You are an experienced software developer. Generate unit test cases for the code submitted in
-the pull request, ensuring comprehensive coverage of all functions, methods, and scenarios to validate the correctness
-and reliability of the implementation."""
-BUGS_PROMPT = """Provide a concise summary of the bug found in the code, describing its characteristics, location, and
-potential effects on the overall functionality and performance of the application. Present the potential issues and
-errors first, following by the most important findings, in your summary"""
+from gpt_review.prompts._bugs import BugPrompt
+from gpt_review.prompts._coverage import CoveragePrompt
+from gpt_review.prompts._summary import SummaryPrompt
 
 _CHECKS = {
     "SUMMARY_CHECKS": [
         {
             "flag": "SUMMARY_SUGGEST",
             "header": "Suggestions",
             "goal": "Any suggestions for improving the changes in this PR?",
@@ -129,19 +122,16 @@
     Args:
         diff (str): The file to summarize.
 
     Returns:
         str: The summary of the file.
     """
     git_file = GitFile(diff.split(" b/")[0], diff)
-    prompt = f"""
-{SUMMARIZE_PROMPT}
-{diff}
-"""
-    response = _ask([prompt], temperature=0.0)
+    messages = SummaryPrompt().get_messages(diff)
+    response = _ask(question=[], messages=messages, temperature=0.0)
     return f"""
 ### {git_file.file_name}
 {response}
 """
 
 
 def _split_diff(git_diff):
@@ -170,40 +160,31 @@
     files = {}
     for diff in _split_diff(git_diff):
         path = diff.split(" b/")[0]
         git_file = GitFile(path.split("/")[len(path.split("/")) - 1], diff)
 
         files[git_file.file_name] = git_file
 
-    prompt = f"""
-```
-{git_diff}
-```
-{TEST_COVERAGE_PROMPT}
-"""
+    messages = CoveragePrompt().get_messages(git_diff)
 
-    return _ask([prompt], temperature=0.0, max_tokens=1500)["response"]
+    return _ask([], messages=messages, temperature=0.0, max_tokens=1500)["response"]
 
 
 def _summarize_bugs_in_pr(git_diff) -> str:
     """
     Summarize bugs that may be introduced.
 
     Args:
         git_diff (str): The git diff to split.
 
     Returns:
         response (str): The response from GPT-4.
     """
-    gpt4_big_prompot = f"""
-{BUGS_PROMPT}
-
-{git_diff}
-"""
-    response = _ask([gpt4_big_prompot])
+    messages = BugPrompt().get_messages(git_diff)
+    response = _ask([], messages=messages)
     logging.info(response["response"])
     return response["response"]
 
 
 def _summarize_risk(git_diff) -> str:
     """
     Summarize potential risks.
```

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/constants.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/constants.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/src/gpt_review/main.py` & `gpt-review-0.8.0rc597.post1/src/gpt_review/main.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/tests/conftest.py` & `gpt-review-0.8.0rc597.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/tests/mock.diff` & `gpt-review-0.8.0rc597.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/tests/test_github.py` & `gpt-review-0.8.0rc597.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/tests/test_gpt_cli.py` & `gpt-review-0.8.0rc597.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/tests/test_llama_index.py` & `gpt-review-0.8.0rc597.post1/tests/test_llama_index.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/tests/test_openai.py` & `gpt-review-0.8.0rc597.post1/tests/test_openai.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/tests/test_report.py` & `gpt-review-0.8.0rc597.post1/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.8.0rc591.post1/PKG-INFO` & `gpt-review-0.8.0rc597.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.8.0rc591.post1
+Version: 0.8.0rc597.post1
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
-Metadata-Version: 2.1 Name: gpt-review Version: 0.8.0rc591.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.8.0rc597.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.8.1 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

