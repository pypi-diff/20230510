# Comparing `tmp/ghas-cli-1.4.0.tar.gz` & `tmp/ghas_cli-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghas-cli-1.4.0.tar", max compression
+gzip compressed data, was "ghas_cli-1.4.2.tar", max compression
```

## Comparing `ghas-cli-1.4.0.tar` & `ghas_cli-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1069 2022-09-15 13:46:01.810098 ghas-cli-1.4.0/LICENSE
--rw-r--r--   0        0        0     4923 2022-11-01 17:44:56.065397 ghas-cli-1.4.0/README.md
--rw-r--r--   0        0        0     1134 2023-01-16 11:50:12.520078 ghas-cli-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    32144 2023-01-16 11:50:33.116301 ghas-cli-1.4.0/src/cli.py
--rw-r--r--   0        0        0        0 2022-09-16 14:56:07.233466 ghas-cli-1.4.0/src/ghas_cli/__init__.py
--rw-r--r--   0        0        0        0 2022-09-16 14:56:07.233466 ghas-cli-1.4.0/src/ghas_cli/utils/__init__.py
--rw-r--r--   0        0        0      666 2023-01-16 11:02:11.200396 ghas-cli-1.4.0/src/ghas_cli/utils/actions.py
--rw-r--r--   0        0        0      386 2022-09-16 19:16:57.742940 ghas-cli-1.4.0/src/ghas_cli/utils/export.py
--rw-r--r--   0        0        0     2810 2022-10-11 09:42:29.318261 ghas-cli-1.4.0/src/ghas_cli/utils/issues.py
--rw-r--r--   0        0        0     1283 2023-01-16 11:49:44.795779 ghas-cli-1.4.0/src/ghas_cli/utils/network.py
--rw-r--r--   0        0        0    20536 2023-01-16 11:42:16.202903 ghas-cli-1.4.0/src/ghas_cli/utils/repositories.py
--rw-r--r--   0        0        0     1285 2023-01-16 11:49:44.795779 ghas-cli-1.4.0/src/ghas_cli/utils/roles.py
--rw-r--r--   0        0        0     1241 2022-12-16 14:44:15.613559 ghas-cli-1.4.0/src/ghas_cli/utils/secrets.py
--rw-r--r--   0        0        0     2545 2023-01-16 11:49:44.795779 ghas-cli-1.4.0/src/ghas_cli/utils/teams.py
--rw-r--r--   0        0        0     1444 2022-09-26 12:38:24.280621 ghas-cli-1.4.0/src/ghas_cli/utils/vulns.py
--rw-r--r--   0        0        0     5972 1970-01-01 00:00:00.000000 ghas-cli-1.4.0/setup.py
--rw-r--r--   0        0        0     6202 1970-01-01 00:00:00.000000 ghas-cli-1.4.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-02-08 18:00:34.563166 ghas_cli-1.4.2/LICENSE
+-rwxr-xr-x   0        0        0     4878 2023-05-10 13:28:28.804158 ghas_cli-1.4.2/README.md
+-rwxr-xr-x   0        0        0     1134 2023-05-10 13:48:57.153170 ghas_cli-1.4.2/pyproject.toml
+-rwxr-xr-x   0        0        0    33380 2023-05-10 13:28:28.829331 ghas_cli-1.4.2/src/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.643212 ghas_cli-1.4.2/src/ghas_cli/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.673123 ghas_cli-1.4.2/src/ghas_cli/utils/__init__.py
+-rwxr-xr-x   0        0        0      666 2023-02-08 18:00:34.698192 ghas_cli-1.4.2/src/ghas_cli/utils/actions.py
+-rwxr-xr-x   0        0        0      386 2023-02-08 18:00:34.713383 ghas_cli-1.4.2/src/ghas_cli/utils/export.py
+-rwxr-xr-x   0        0        0     2810 2023-02-08 18:00:34.732994 ghas_cli-1.4.2/src/ghas_cli/utils/issues.py
+-rwxr-xr-x   0        0        0     2077 2023-05-10 13:28:28.836731 ghas_cli-1.4.2/src/ghas_cli/utils/network.py
+-rwxr-xr-x   0        0        0    20456 2023-05-10 13:28:28.846062 ghas_cli-1.4.2/src/ghas_cli/utils/repositories.py
+-rwxr-xr-x   0        0        0     1285 2023-02-08 18:00:34.788075 ghas_cli-1.4.2/src/ghas_cli/utils/roles.py
+-rwxr-xr-x   0        0        0     1350 2023-05-10 13:28:28.850978 ghas_cli-1.4.2/src/ghas_cli/utils/secrets.py
+-rwxr-xr-x   0        0        0     2543 2023-05-10 13:28:28.858409 ghas_cli-1.4.2/src/ghas_cli/utils/teams.py
+-rwxr-xr-x   0        0        0     1442 2023-05-10 13:28:28.864807 ghas_cli-1.4.2/src/ghas_cli/utils/vulns.py
+-rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 ghas_cli-1.4.2/PKG-INFO
```

### Comparing `ghas-cli-1.4.0/LICENSE` & `ghas_cli-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghas-cli-1.4.0/README.md` & `ghas_cli-1.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Security-ghas-cli
+# ghas-cli
 
-[![CodeQL](https://github.com/Malwarebytes/Security-ghas-cli/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Malwarebytes/Security-ghas-cli/actions/workflows/codeql-analysis.yml)
+[![CodeQL](https://github.com/Malwarebytes/ghas-cli/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Malwarebytes/ghas-cli/actions/workflows/codeql-analysis.yml)
 
 CLI utility to interact with [GitHub Advanced Security](https://docs.github.com/en/enterprise-cloud@latest/get-started/learning-about-github/about-github-advanced-security) (_"GHAS"_).
 
 It allows to deploy GHAS features individually or at scale, while taking into account each repository configuration.
 
 More specifically, it automates the following:
 
@@ -23,15 +23,15 @@
 To follow your deployment, `ghas-cli` outputs results in a csv file indicating the deployment status of each feature for each repository.
 
 You can work on a single repository or on thousands of them. In that case, `ghas-cli` does its best to overcome [GitHub's rate limits](https://docs.github.com/en/enterprise-cloud@latest/rest/rate-limit)...
 
 
 ## Installation
 
-Builds are available in the [`Releases`](https://github.com/Malwarebytes/Security-ghas-cli/releases) tab.
+Builds are available in the [`Releases`](https://github.com/Malwarebytes/ghas-cli/releases) tab.
 
 * Pypi:
 
 ```bash
 pip install ghas-cli
 ```
 
@@ -41,15 +41,15 @@
 python -m pip install /full/path/to/ghas-cli-xxx.whl
 
 # e.g: python3 -m pip install Downloads/ghas-cli-0.5.0-none-any.whl
 ```
 
 ## Usage
 
-`ghas-cli -h` or see the [wiki](https://github.com/Malwarebytes/Security-ghas-cli/wiki).
+`ghas-cli -h` or see the [wiki](https://github.com/Malwarebytes/ghas-cli/wiki).
 
 
 ## Development
 
 ### Build
 
 [Install Poetry](https://python-poetry.org/docs/#installation) first, then:
```

### Comparing `ghas-cli-1.4.0/pyproject.toml` & `ghas_cli-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ghas-cli"
-version = "1.4.0"
+version = "1.4.2"
 description = "Command line interface to interact with GitHub Advanced Security."
 authors = ["jboursier <jboursier@malwarebytes.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Malwarebytes/ghas-cli"
 documentation = "https://github.com/Malwarebytes/ghas-cli/wiki"
 repository = "https://github.com/Malwarebytes/ghas-cli"
```

### Comparing `ghas-cli-1.4.0/src/cli.py` & `ghas_cli-1.4.2/src/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python3
 
 __author__ = "jboursier"
-__copyright__ = "Copyright 2022, Malwarebytes"
-__version__ = "1.4.0"
+__copyright__ = "Copyright 2023, Malwarebytes"
+__version__ = "1.4.2"
 __maintainer__ = "jboursier"
 __email__ = "jboursier@malwarebytes.com"
 __status__ = "Production"
 
 try:
     import click
     import json
@@ -415,15 +415,14 @@
         return False
 
     # 1. Get list repositories passed as argument
     res = input_repos_list.readlines()
 
     print(len(res))
     for repo in res:
-
         repo = repo.rstrip("\n")
 
         # 2. get default branch
         default_branch = repositories.get_default_branch(
             organization=organization, token=token, repository=repo
         )
         if not default_branch:
@@ -549,14 +548,15 @@
         for repo in team_repos:
             click.echo(repo.to_json())
     elif "list" == format:
         for repo in team_repos:
             click.echo(f"{repo.orga}/{repo.name}")
 
 
+
 @teams_cli.command("permissions")
 @click.option("-o", "--organization", prompt="Organization name", type=str)
 @click.option("-s", "--team", prompt="Team slug", type=str)
 @click.option("-r", "--repository", prompt="Repository name", type=str)
 @click.option(
     "-t",
     "--token",
@@ -574,14 +574,15 @@
     team_repo_perms = teams.get_repo_perms(
         team=team, repo=repository, organization=organization, token=token
     )
 
     click.echo(team_repo_perms)
 
 
+
 ##########
 # Issues #
 ##########
 
 
 @cli.group(name="issues")
 def issues_cli() -> None:
@@ -752,24 +753,53 @@
     type=str,
     default=None,
     hide_input=True,
     confirmation_prompt=False,
     show_envvar=True,
 )
 @click.option("-o", "--organization", prompt="Organization name", type=str)
+@click.option(
+    "-f",
+    "--secrets-filter",
+    prompt=True,
+    type=click.Choice(
+        [
+            "all",
+            "atlassian_api_token",
+            "slack_incoming_webhook_url",
+            "github_ssh_private_key",
+            "slack_api_token",
+            "mailgun_api_key",
+            "firebase_cloud_messaging_server_key",
+            "jfrog_platform_api_key",
+            "google_api_key",
+            "azure_storage_account_key",
+            "new_relic_license_key",
+            "github_personal_access_token",
+            "sendgrid_api_key",
+            "azure_devops_personal_access_token",
+            "jfrog_platform_access_token",
+            "google_cloud_private_key_id",
+            "google_oauth_access_token",
+        ]
+    ),
+    default="all",
+    hide_input=False,
+)
 def secret_alerts_export(
-    state: str, output_csv: Any, token: str, organization: str
+    state: str, output_csv: Any, token: str, organization: str, secrets_filter: str
 ) -> None:
     """Export secrets to a csv"""
 
-    secrets_list = secrets.export_secrets(state, token, organization)
+    secrets_list = secrets.export_secrets(state, token, organization, secrets_filter)
     for secret in secrets_list:
         output_csv.write(
             f"{secret['state']}, {secret['resolution']}, {secret['resolved_at']}, {secret['repository_full_name']}, {secret['url']}, {secret['secret_type']}, {secret['secret']}\n"
         )
+    print(f"Retrieved {len(secrets_list)} secrets.")
 
 
 ##############
 # Dependabot #
 ##############
 
 
@@ -893,15 +923,14 @@
     name: str,
     description: str,
     base_role: str,
     permission: List,
     organization: str,
     token: str,
 ) -> None:
-
     if roles.create_role(
         name, description, base_role, permissions, organization, token
     ):
         click.echo(f"Custom role {name} created with success!")
     else:
         click.echo(f"Failure to create the custom role {name}.")
 
@@ -1046,17 +1075,16 @@
     with open("./templates/codeql.md", "r") as f:
         template_codeql = f.read()
 
     print(
         f"Enabling Actions ({actions_enable}), Secret Scanner ({secretscanner}), Push Protection ({pushprotection}), Dependabot ({dependabot}), CodeQL ({codeql}), Dependency Reviewer ({reviewer}) to {len(repos_list)} repositories."
     )
 
-    for repo in repos_list:
-
-        repo = repo.rstrip("\n")
+    for repo_name in repos_list:
+        repo = repo_name.rstrip("\n")
         issue_secretscanner_res = None
         issue_pushprotection_res = None
         issue_dependabot_res = None
         issue_codeql_res = None
         actions_res = None
         secretscanner_res = None
         pushprotection_res = None
@@ -1164,18 +1192,19 @@
 )
 @click.option("-o", "--organization", prompt="Organization name", type=str)
 def mass_archive(
     input_repos_list: Any,
     organization: str,
     token: str,
 ) -> None:
+    """Create an issue to inform that repositories will be archived at a specific date."""
+
     repos_list = input_repos_list.readlines()
 
     for repo in repos_list:
-
         repo = repo.rstrip("\n")
 
         click.echo(f"{repo}...", nl=False)
 
         if repositories.archive(
             organization=organization, token=token, repository=repo
         ):
@@ -1188,40 +1217,50 @@
 @click.argument("input_repos_list", type=click.File("r"))
 @click.option(
     "-u",
     "--archived_date",
     prompt="Target date when the repositories will be archived",
     type=str,
 )
+@click.option(
+    "-t",
+    "--token",
+    prompt=False,
+    type=str,
+    default=None,
+    hide_input=True,
+    confirmation_prompt=False,
+    show_envvar=True,
+)
+@click.option("-o", "--organization", prompt="Organization name", type=str)
 def mass_issue_archive(
     input_repos_list: Any,
     archived_date: str,
     organization: str,
     token: str,
 ) -> None:
     """Create an issue to inform that repositories will be archived at a specific date."""
 
     repos_list = input_repos_list.readlines()
 
     for repo in repos_list:
-
         repo = repo.rstrip("\n")
 
         issue_res = issues.create(
             title=f"This repository will be archived on {archived_date}  :warning: :wastebasket:",
             content=f"""
 Hello,
 
 Due to inactivity, this repository will be archived automatically on {archived_date}.
 
 This means that it will become read-only: `git clone` will still work, and the repository can be unarchived at anytime if needed.
 
 For more information, see https://docs.github.com/en/repositories/archiving-a-github-repository/archiving-repositories#about-repository-archival
 
-If you think this is a mistake, please inform the Security team *ASAP* on Slack at `#github-appsec-security.`
+If you think this is a mistake, please inform the Security team *ASAP* on Slack at `#github-appsec-security`.
 
 Thanks! :handshake:""",
             repository=repo,
             organization=organization,
             token=token,
         )
         if issue_res:
```

### Comparing `ghas-cli-1.4.0/src/ghas_cli/utils/actions.py` & `ghas_cli-1.4.2/src/ghas_cli/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ghas-cli-1.4.0/src/ghas_cli/utils/issues.py` & `ghas_cli-1.4.2/src/ghas_cli/utils/issues.py`

 * *Files identical despite different names*

### Comparing `ghas-cli-1.4.0/src/ghas_cli/utils/repositories.py` & `ghas_cli-1.4.2/src/ghas_cli/utils/repositories.py`

 * *Files 8% similar despite different names*

```diff
@@ -160,30 +160,27 @@
     while True:
         params = {
             "type": f"{status}",
             "sort": "full_name",
             "per_page": 100,
             "page": page,
         }
-        repos = requests.get(
+        repos = network.get(
             url=f"https://api.github.com/orgs/{organization}/repos",
             params=params,
             headers=headers,
         )
-        if network.check_rate_limit(repos):
-            break
 
         if repos.status_code != 200:
             break
-
+    
         if [] == repos.json():
             break
 
         for r in repos.json():
-
             repo = Repository()
             repo.load_json(r, token=token)
             # repo.load_json(r, token=None)
 
             if language != "" and repo.main_language != language:
                 print(
                     f"{repo.name} ignored because of language: {language} vs. {repo.main_language}"
@@ -221,15 +218,15 @@
     token: str, organization: str, repository_name: str, default_branch: str
 ) -> Any:
     """
     Return the latest commit date on the default branch
     """
     headers = network.get_github_headers(token)
 
-    branch_res = requests.get(
+    branch_res = network.get(
         url=f"https://api.github.com/repos/{organization}/{repository_name}/branches/{default_branch}",
         headers=headers,
     )
 
     if branch_res.status_code != 200:
         return False
 
@@ -241,33 +238,32 @@
 
 
 def archive(organization: str, token: str, repository: str) -> bool:
     headers = network.get_github_headers(token)
 
     payload = {"archived": True}
 
-    status = requests.patch(
+    status = network.patch(
         url=f"https://api.github.com/repos/{organization}/{repository}",
         headers=headers,
         json=payload,
     )
 
     if status.status_code != 200:
         return False
     else:
         return True
 
 
 def check_dependabot_alerts_enabled(
     token: str, organization: str, repository_name: str
 ) -> bool:
-
     headers = network.get_github_headers(token)
 
-    status = requests.get(
+    status = network.get(
         url=f"https://api.github.com/orgs/{organization}/repos/vulnerability-alerts",
         headers=headers,
     )
 
     if status.status_code != 204:
         return False
     else:
@@ -282,15 +278,15 @@
             "advanced_security": {
                 "status": "enabled",
             },
             "secret_scanning": {"status": "enabled"},
         }
     }
 
-    status = requests.patch(
+    status = network.patch(
         url=f"https://api.github.com/repos/{organization}/{repository}",
         headers=headers,
         json=payload,
     )
 
     if status.status_code != 200:
         return False
@@ -309,50 +305,50 @@
                 "status": "enabled",
             },
             "secret_scanning": {"status": "enabled"},
             "secret_scanning_push_protection": {"status": "enabled"},
         }
     }
 
-    status = requests.patch(
+    status = network.patch(
         url=f"https://api.github.com/repos/{organization}/{repository}",
         headers=headers,
         json=payload,
     )
 
     if status.status_code != 200:
         return False
     else:
         return True
 
 
 def enable_dependabot(organization: str, token: str, repository: str) -> bool:
     headers = network.get_github_headers(token)
 
-    status_alerts = requests.put(
+    status_alerts = network.put(
         url=f"https://api.github.com/repos/{organization}/{repository}/vulnerability-alerts",
         headers=headers,
     )
 
-    status_fixes = requests.put(
+    status_fixes = network.put(
         url=f"https://api.github.com/repos/{organization}/{repository}/automated-security-fixes",
         headers=headers,
     )
 
     if status_alerts.status_code != 204 and status_fixes != 204:
         return False
     else:
         return True
 
 
 def get_default_branch(organization: str, token: str, repository: str) -> str:
     """Get the default branch slug for a repository"""
     headers = network.get_github_headers(token)
 
-    repo = requests.get(
+    repo = network.get(
         url=f"https://api.github.com/repos/{organization}/{repository}",
         headers=headers,
     )
     if repo.status_code != 200:
         return False
 
     repo = repo.json()
@@ -371,15 +367,15 @@
 ) -> List:
     """Get the main language for a repository"""
 
     interpreted_languages = {"javascript", "python", "ruby"}
     aliased_interpreted_languages = {"typescript": "javascript"}
 
     headers = network.get_github_headers(token)
-    languages = requests.get(
+    languages = network.get(
         url=f"https://api.github.com/repos/{organization}/{repository}/languages",
         headers=headers,
     )
     if languages.status_code != 200:
         return ["default"]
 
     lang = set()
@@ -456,15 +452,15 @@
 
     # Get the default branch
     default_branch = get_default_branch(organization, token, repository)
     if not default_branch:
         return False
 
     # Create a branch
-    branch_resp = requests.get(
+    branch_resp = network.get(
         url=f"https://api.github.com/repos/{organization}/{repository}/git/refs/heads",
         headers=headers,
     )
     if branch_resp.status_code != 200:
         return False
 
     refs = branch_resp.json()
@@ -477,39 +473,38 @@
         return False
 
     payload = {
         "ref": f"refs/heads/{target_branch}",
         "sha": sha1,
     }
 
-    branch_resp = requests.post(
+    branch_resp = network.post(
         url=f"https://api.github.com/repos/{organization}/{repository}/git/refs",
         headers=headers,
         json=payload,
     )
 
     if branch_resp.status_code != 201:
         return False
 
     # Create commit
     languages = get_languages(
         organization, token, repository, only_interpreted=True, only_codeql=True
     )
 
     for language in languages:
-
         # Workflow config
         lang, template = load_codeql_base64_template(language, default_branch)
         payload = {
             "message": f"Enable CodeQL analysis for {language}",
             "content": template,
             "branch": target_branch,
         }
 
-        commit_resp = requests.put(
+        commit_resp = network.put(
             url=f"https://api.github.com/repos/{organization}/{repository}/contents/.github/workflows/codeql-analysis-{lang}.yml",
             headers=headers,
             json=payload,
         )
 
         if commit_resp.status_code != 201:
             return False
@@ -518,15 +513,15 @@
         lang, template = load_codeql_config_base64_template(language)
         payload = {
             "message": f"Enable CodeQL config file for {language}",
             "content": template,
             "branch": target_branch,
         }
 
-        commit_resp = requests.put(
+        commit_resp = network.put(
             url=f"https://api.github.com/repos/{organization}/{repository}/contents/.github/codeql/codeql-config-{lang}.yml",
             headers=headers,
             json=payload,
         )
         if commit_resp.status_code != 201:
             return False
 
@@ -537,15 +532,15 @@
         "head": target_branch,
         "base": default_branch,
     }
 
     # Retry if rate-limited
     i = 0
     while i < network.RETRIES:
-        pr_resp = requests.post(
+        pr_resp = network.post(
             url=f"https://api.github.com/repos/{organization}/{repository}/pulls",
             headers=headers,
             json=payload,
         )
         if pr_resp.status_code == 201:
             return True
 
@@ -585,15 +580,15 @@
 
     # Get the default branch
     default_branch = get_default_branch(organization, token, repository)
     if not default_branch:
         return False
 
     # Create a branch
-    branch_resp = requests.get(
+    branch_resp = network.get(
         url=f"https://api.github.com/repos/{organization}/{repository}/git/refs/heads",
         headers=headers,
     )
     if branch_resp.status_code != 200:
         return False
 
     refs = branch_resp.json()
@@ -606,15 +601,15 @@
         return False
 
     payload = {
         "ref": f"refs/heads/{target_branch}",
         "sha": sha1,
     }
 
-    branch_resp = requests.post(
+    branch_resp = network.post(
         url=f"https://api.github.com/repos/{organization}/{repository}/git/refs",
         headers=headers,
         json=payload,
     )
 
     if branch_resp.status_code != 201:
         return False
@@ -623,15 +618,15 @@
     template = load_dependency_review_base64_template()
     payload = {
         "message": f"Enable Dependency reviewer",
         "content": template,
         "branch": target_branch,
     }
 
-    commit_resp = requests.put(
+    commit_resp = network.put(
         url=f"https://api.github.com/repos/{organization}/{repository}/contents/.github/workflows/dependency_enforcement.yml",
         headers=headers,
         json=payload,
     )
     if commit_resp.status_code != 201:
         return False
 
@@ -642,15 +637,15 @@
         "head": target_branch,
         "base": default_branch,
     }
 
     # Retry if rate-limited
     i = 0
     while i < network.RETRIES:
-        pr_resp = requests.post(
+        pr_resp = network.post(
             url=f"https://api.github.com/repos/{organization}/{repository}/pulls",
             headers=headers,
             json=payload,
         )
 
         if pr_resp.status_code == 201:
             return True
```

### Comparing `ghas-cli-1.4.0/src/ghas_cli/utils/roles.py` & `ghas_cli-1.4.2/src/ghas_cli/utils/roles.py`

 * *Files identical despite different names*

### Comparing `ghas-cli-1.4.0/src/ghas_cli/utils/secrets.py` & `ghas_cli-1.4.2/src/ghas_cli/utils/secrets.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 
 from typing import List
 import requests
 
 from . import network
 
 
-def export_secrets(state: str, token: str, organization: str) -> List:
+def export_secrets(
+    state: str, token: str, organization: str, secrets_filter: str
+) -> List:
     """Get all secrets from the organization"""
 
     headers = network.get_github_headers(token)
 
     secret_list = []
     page = 1
     while True:
         params = {"state": state, "per_page": 100, "page": page}
 
         secrets = requests.get(
             url=f"https://api.github.com/orgs/{organization}/secret-scanning/alerts",
             params=params,
             headers=headers,
         )
+
         if network.check_rate_limit(secrets):
             break
         if secrets.status_code != 200:
             break
 
         if not secrets.json():
             break
@@ -36,12 +39,12 @@
             s["resolution"] = secret["resolution"]
             s["resolved_at"] = secret["resolved_at"]
             s["repository_full_name"] = secret["repository"]["full_name"]
             s["url"] = secret["url"]
             s["secret_type"] = secret["secret_type"]
             s["secret"] = secret["secret"]
 
-            secret_list.append(s)
+            if secrets_filter is "all" or s["secret_type"] == secrets_filter:
+                secret_list.append(s)
 
         page += 1
-
     return secret_list
```

### Comparing `ghas-cli-1.4.0/src/ghas_cli/utils/teams.py` & `ghas_cli-1.4.2/src/ghas_cli/utils/teams.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
     headers = network.get_github_headers(token)
 
     repos_list = []
     page = 1
 
     while True:
-
         params = {"per_page": 100, "page": page}
         repos = requests.get(
             url=f"https://api.github.com/orgs/{organization}/teams/{team_slug}/repos",
             params=params,
             headers=headers,
         )
         if network.check_rate_limit(repos):
@@ -48,15 +47,14 @@
 
     headers = network.get_github_headers(token)
 
     teams_list = []
     page = 1
 
     while True:
-
         params = {"per_page": 100, "page": page}
 
         teams_res = requests.get(
             url=f"https://api.github.com/orgs/{organization}/teams",
             params=params,
             headers=headers,
         )
```

### Comparing `ghas-cli-1.4.0/src/ghas_cli/utils/vulns.py` & `ghas_cli-1.4.2/src/ghas_cli/utils/vulns.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,20 +13,18 @@
     """Get CodeQL alerts for one or several repositories"""
 
     headers = network.get_github_headers(token)
 
     repositories_alerts = {}
 
     for repo in repos:
-
         alerts_repo = []
         page = 1
 
         while True:
-
             params = {"state": "open", "per_page": 100, "page": page}
             alerts = requests.get(
                 url=f"https://api.github.com/repos/{organization}/{repo.name}/code-scanning/alerts",
                 params=params,
                 headers=headers,
             )
             if network.check_rate_limit(alerts):
```

### Comparing `ghas-cli-1.4.0/PKG-INFO` & `ghas_cli-1.4.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghas-cli
-Version: 1.4.0
+Version: 1.4.2
 Summary: Command line interface to interact with GitHub Advanced Security.
 Home-page: https://github.com/Malwarebytes/ghas-cli
 License: MIT
 Keywords: security,cli,github,utility
 Author: jboursier
 Author-email: jboursier@malwarebytes.com
 Requires-Python: >=3.7,<4
@@ -16,28 +16,29 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: click (>=8)
 Requires-Dist: colorama
 Requires-Dist: configparser
 Requires-Dist: python-magic
 Requires-Dist: requests
 Requires-Dist: urllib3 (>=1.26.12,<2.0.0)
 Project-URL: Documentation, https://github.com/Malwarebytes/ghas-cli/wiki
 Project-URL: Repository, https://github.com/Malwarebytes/ghas-cli
 Description-Content-Type: text/markdown
 
-# Security-ghas-cli
+# ghas-cli
 
-[![CodeQL](https://github.com/Malwarebytes/Security-ghas-cli/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Malwarebytes/Security-ghas-cli/actions/workflows/codeql-analysis.yml)
+[![CodeQL](https://github.com/Malwarebytes/ghas-cli/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/Malwarebytes/ghas-cli/actions/workflows/codeql-analysis.yml)
 
 CLI utility to interact with [GitHub Advanced Security](https://docs.github.com/en/enterprise-cloud@latest/get-started/learning-about-github/about-github-advanced-security) (_"GHAS"_).
 
 It allows to deploy GHAS features individually or at scale, while taking into account each repository configuration.
 
 More specifically, it automates the following:
 
@@ -56,15 +57,15 @@
 To follow your deployment, `ghas-cli` outputs results in a csv file indicating the deployment status of each feature for each repository.
 
 You can work on a single repository or on thousands of them. In that case, `ghas-cli` does its best to overcome [GitHub's rate limits](https://docs.github.com/en/enterprise-cloud@latest/rest/rate-limit)...
 
 
 ## Installation
 
-Builds are available in the [`Releases`](https://github.com/Malwarebytes/Security-ghas-cli/releases) tab.
+Builds are available in the [`Releases`](https://github.com/Malwarebytes/ghas-cli/releases) tab.
 
 * Pypi:
 
 ```bash
 pip install ghas-cli
 ```
 
@@ -74,15 +75,15 @@
 python -m pip install /full/path/to/ghas-cli-xxx.whl
 
 # e.g: python3 -m pip install Downloads/ghas-cli-0.5.0-none-any.whl
 ```
 
 ## Usage
 
-`ghas-cli -h` or see the [wiki](https://github.com/Malwarebytes/Security-ghas-cli/wiki).
+`ghas-cli -h` or see the [wiki](https://github.com/Malwarebytes/ghas-cli/wiki).
 
 
 ## Development
 
 ### Build
 
 [Install Poetry](https://python-poetry.org/docs/#installation) first, then:
```

