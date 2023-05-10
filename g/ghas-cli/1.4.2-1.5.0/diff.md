# Comparing `tmp/ghas_cli-1.4.2.tar.gz` & `tmp/ghas_cli-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghas_cli-1.4.2.tar", max compression
+gzip compressed data, was "ghas_cli-1.5.0.tar", max compression
```

## Comparing `ghas_cli-1.4.2.tar` & `ghas_cli-1.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0     1069 2023-02-08 18:00:34.563166 ghas_cli-1.4.2/LICENSE
--rwxr-xr-x   0        0        0     4878 2023-05-10 13:28:28.804158 ghas_cli-1.4.2/README.md
--rwxr-xr-x   0        0        0     1134 2023-05-10 13:48:57.153170 ghas_cli-1.4.2/pyproject.toml
--rwxr-xr-x   0        0        0    33380 2023-05-10 13:28:28.829331 ghas_cli-1.4.2/src/cli.py
--rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.643212 ghas_cli-1.4.2/src/ghas_cli/__init__.py
--rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.673123 ghas_cli-1.4.2/src/ghas_cli/utils/__init__.py
--rwxr-xr-x   0        0        0      666 2023-02-08 18:00:34.698192 ghas_cli-1.4.2/src/ghas_cli/utils/actions.py
--rwxr-xr-x   0        0        0      386 2023-02-08 18:00:34.713383 ghas_cli-1.4.2/src/ghas_cli/utils/export.py
--rwxr-xr-x   0        0        0     2810 2023-02-08 18:00:34.732994 ghas_cli-1.4.2/src/ghas_cli/utils/issues.py
--rwxr-xr-x   0        0        0     2077 2023-05-10 13:28:28.836731 ghas_cli-1.4.2/src/ghas_cli/utils/network.py
--rwxr-xr-x   0        0        0    20456 2023-05-10 13:28:28.846062 ghas_cli-1.4.2/src/ghas_cli/utils/repositories.py
--rwxr-xr-x   0        0        0     1285 2023-02-08 18:00:34.788075 ghas_cli-1.4.2/src/ghas_cli/utils/roles.py
--rwxr-xr-x   0        0        0     1350 2023-05-10 13:28:28.850978 ghas_cli-1.4.2/src/ghas_cli/utils/secrets.py
--rwxr-xr-x   0        0        0     2543 2023-05-10 13:28:28.858409 ghas_cli-1.4.2/src/ghas_cli/utils/teams.py
--rwxr-xr-x   0        0        0     1442 2023-05-10 13:28:28.864807 ghas_cli-1.4.2/src/ghas_cli/utils/vulns.py
--rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 ghas_cli-1.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-02-08 18:00:34.563166 ghas_cli-1.5.0/LICENSE
+-rwxr-xr-x   0        0        0     4878 2023-05-10 13:28:28.804158 ghas_cli-1.5.0/README.md
+-rwxr-xr-x   0        0        0     1134 2023-05-10 17:42:46.091602 ghas_cli-1.5.0/pyproject.toml
+-rwxr-xr-x   0        0        0    33392 2023-05-10 17:42:57.305520 ghas_cli-1.5.0/src/cli.py
+-rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.643212 ghas_cli-1.5.0/src/ghas_cli/__init__.py
+-rwxr-xr-x   0        0        0        0 2023-02-08 18:00:34.673123 ghas_cli-1.5.0/src/ghas_cli/utils/__init__.py
+-rwxr-xr-x   0        0        0      666 2023-02-08 18:00:34.698192 ghas_cli-1.5.0/src/ghas_cli/utils/actions.py
+-rwxr-xr-x   0        0        0      417 2023-05-10 17:42:10.795557 ghas_cli-1.5.0/src/ghas_cli/utils/export.py
+-rwxr-xr-x   0        0        0     2810 2023-02-08 18:00:34.732994 ghas_cli-1.5.0/src/ghas_cli/utils/issues.py
+-rwxr-xr-x   0        0        0     2120 2023-05-10 17:42:10.801997 ghas_cli-1.5.0/src/ghas_cli/utils/network.py
+-rwxr-xr-x   0        0        0    21717 2023-05-10 17:42:10.811903 ghas_cli-1.5.0/src/ghas_cli/utils/repositories.py
+-rwxr-xr-x   0        0        0     1285 2023-02-08 18:00:34.788075 ghas_cli-1.5.0/src/ghas_cli/utils/roles.py
+-rwxr-xr-x   0        0        0     1350 2023-05-10 17:42:10.817870 ghas_cli-1.5.0/src/ghas_cli/utils/secrets.py
+-rwxr-xr-x   0        0        0     2575 2023-05-10 17:42:10.825735 ghas_cli-1.5.0/src/ghas_cli/utils/teams.py
+-rwxr-xr-x   0        0        0     1442 2023-05-10 13:28:28.864807 ghas_cli-1.5.0/src/ghas_cli/utils/vulns.py
+-rw-r--r--   0        0        0     6208 1970-01-01 00:00:00.000000 ghas_cli-1.5.0/PKG-INFO
```

### Comparing `ghas_cli-1.4.2/LICENSE` & `ghas_cli-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.4.2/README.md` & `ghas_cli-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.4.2/pyproject.toml` & `ghas_cli-1.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ghas-cli"
-version = "1.4.2"
+version = "1.5.0"
 description = "Command line interface to interact with GitHub Advanced Security."
 authors = ["jboursier <jboursier@malwarebytes.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Malwarebytes/ghas-cli"
 documentation = "https://github.com/Malwarebytes/ghas-cli/wiki"
 repository = "https://github.com/Malwarebytes/ghas-cli"
```

### Comparing `ghas_cli-1.4.2/src/cli.py` & `ghas_cli-1.5.0/src/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python3
 
 __author__ = "jboursier"
 __copyright__ = "Copyright 2023, Malwarebytes"
-__version__ = "1.4.2"
+__version__ = "1.5.0"
 __maintainer__ = "jboursier"
 __email__ = "jboursier@malwarebytes.com"
 __status__ = "Production"
 
 try:
     import click
     import json
     from typing import Dict, Any, List
     from datetime import datetime
+    import logging
+
+    logging.getLogger().setLevel(level=logging.INFO)
 except ImportError:
     import sys
 
-    print("Missing dependencies. Please reach @jboursier if needed.")
+    logging.error("Missing dependencies. Please reach @jboursier if needed.")
     sys.exit(255)
 
 from ghas_cli.utils import repositories, vulns, teams, issues, actions, roles, secrets
 
 
 def main() -> None:
     try:
@@ -413,15 +416,15 @@
     except Exception:
         click.echo(f"Invalid time: {last_updated_before}")
         return False
 
     # 1. Get list repositories passed as argument
     res = input_repos_list.readlines()
 
-    print(len(res))
+    logging.info(len(res))
     for repo in res:
         repo = repo.rstrip("\n")
 
         # 2. get default branch
         default_branch = repositories.get_default_branch(
             organization=organization, token=token, repository=repo
         )
@@ -548,15 +551,14 @@
         for repo in team_repos:
             click.echo(repo.to_json())
     elif "list" == format:
         for repo in team_repos:
             click.echo(f"{repo.orga}/{repo.name}")
 
 
-
 @teams_cli.command("permissions")
 @click.option("-o", "--organization", prompt="Organization name", type=str)
 @click.option("-s", "--team", prompt="Team slug", type=str)
 @click.option("-r", "--repository", prompt="Repository name", type=str)
 @click.option(
     "-t",
     "--token",
@@ -574,15 +576,14 @@
     team_repo_perms = teams.get_repo_perms(
         team=team, repo=repository, organization=organization, token=token
     )
 
     click.echo(team_repo_perms)
 
 
-
 ##########
 # Issues #
 ##########
 
 
 @cli.group(name="issues")
 def issues_cli() -> None:
@@ -791,15 +792,15 @@
     """Export secrets to a csv"""
 
     secrets_list = secrets.export_secrets(state, token, organization, secrets_filter)
     for secret in secrets_list:
         output_csv.write(
             f"{secret['state']}, {secret['resolution']}, {secret['resolved_at']}, {secret['repository_full_name']}, {secret['url']}, {secret['secret_type']}, {secret['secret']}\n"
         )
-    print(f"Retrieved {len(secrets_list)} secrets.")
+    logging.info(f"Retrieved {len(secrets_list)} secrets.")
 
 
 ##############
 # Dependabot #
 ##############
 
 
@@ -919,15 +920,15 @@
     show_envvar=True,
 )
 @click.option("-o", "--organization", prompt="Organization name", type=str)
 def roles_add(
     name: str,
     description: str,
     base_role: str,
-    permission: List,
+    permissions: List,
     organization: str,
     token: str,
 ) -> None:
     if roles.create_role(
         name, description, base_role, permissions, organization, token
     ):
         click.echo(f"Custom role {name} created with success!")
@@ -1071,33 +1072,33 @@
     with open("./templates/secret_scanner_push_protection.md", "r") as f:
         template_pushprotection = f.read()
     with open("./templates/dependabot.md", "r") as f:
         template_dependabot = f.read()
     with open("./templates/codeql.md", "r") as f:
         template_codeql = f.read()
 
-    print(
+    logging.info(
         f"Enabling Actions ({actions_enable}), Secret Scanner ({secretscanner}), Push Protection ({pushprotection}), Dependabot ({dependabot}), CodeQL ({codeql}), Dependency Reviewer ({reviewer}) to {len(repos_list)} repositories."
     )
 
-    for repo_name in repos_list:
-        repo = repo_name.rstrip("\n")
+    for repo in repos_list:
+        repo = repo.rstrip("\n")
         issue_secretscanner_res = None
         issue_pushprotection_res = None
         issue_dependabot_res = None
         issue_codeql_res = None
         actions_res = None
         secretscanner_res = None
         pushprotection_res = None
         dependabot_res = None
         codeql_res = None
         reviewer_res = None
         mend_res = 0
 
-        print(f"{repo}....", end="")
+        logging.info(f"{repo}....")
 
         if actions_enable:
             actions_res = actions.set_permissions(
                 repository_name=repo,
                 organization=organization,
                 token=token,
                 enabled=True,
@@ -1164,15 +1165,15 @@
                 mend_res = issues.close_issues(
                     issue_numbers=issues_res,
                     repository=repo,
                     organization=organization,
                     token=token,
                 )
 
-        print(
+        logging.info(
             f"Done: {actions_res},{secretscanner_res}, {pushprotection_res}, {dependabot_res}, {codeql_res}, {reviewer_res}, {issue_secretscanner_res}, {issue_pushprotection_res}, {issue_dependabot_res}, {issue_codeql_res}, {mend_res}"
         )
         # CSV columns
         # Organization, repo_name, Actions Enabled?, SS enabled?, PushProtection Enabled?, Dependabot Enabled?, CodeQL enabled?, Dep Reviewer Enabled?, Issue SS created?, Issue PP created?, Issue Dependabot created?, Issue CodeQL created?, Mend issues closed
         output_csv.write(
             f"{organization},{repo},{actions_res},{secretscanner_res}, {pushprotection_res}, {dependabot_res}, {codeql_res}, {reviewer_res}, {issue_secretscanner_res}, {issue_pushprotection_res}, {issue_dependabot_res}, {issue_codeql_res}, {mend_res}\n"
         )
@@ -1192,16 +1193,14 @@
 )
 @click.option("-o", "--organization", prompt="Organization name", type=str)
 def mass_archive(
     input_repos_list: Any,
     organization: str,
     token: str,
 ) -> None:
-    """Create an issue to inform that repositories will be archived at a specific date."""
-
     repos_list = input_repos_list.readlines()
 
     for repo in repos_list:
         repo = repo.rstrip("\n")
 
         click.echo(f"{repo}...", nl=False)
 
@@ -1322,15 +1321,15 @@
             team_repos = teams.get_repositories(team, organization, token)
 
             # List teams' permissions + filter only Write
             for repo in team_repos:
                 perms = teams.get_repo_perms(team, repo.name, organization, token)
                 if "write" == perms[-1]:
                     write_perms.append([team, repo.name, perms[-1]])
-                    print([team, repo.name, perms[-1]])
+                    logging.info([team, repo.name, perms[-1]])
                     output_perms_list.write(f"{team}, {repo.name}, {perms[-1]}\n")
 
     # Assign the Developer role
     for perms in write_perms:
         if roles.assign_role(
             team=perms[0],
             role=permission,
```

### Comparing `ghas_cli-1.4.2/src/ghas_cli/utils/actions.py` & `ghas_cli-1.5.0/src/ghas_cli/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.4.2/src/ghas_cli/utils/issues.py` & `ghas_cli-1.5.0/src/ghas_cli/utils/issues.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.4.2/src/ghas_cli/utils/network.py` & `ghas_cli-1.5.0/src/ghas_cli/utils/network.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python3
 
 from typing import Any, Dict
 from datetime import datetime
 import time
 import requests
+import logging
 
 # If the rate-limit is reached, sleep X seconds
 SLEEP_1_MINUTE = 60
 
 # Sleep x seconds between two requests
 SLEEP_BETWEEN_REQUESTS = 2
 
@@ -24,51 +25,57 @@
         "X-GitHub-Api-Version": "2022-11-28",  # https://docs.github.com/en/rest/overview/api-versions#supported-api-versions
     }
 
 
 def check_rate_limit(response: Any) -> bool:
     if "0" == response.headers["x-ratelimit-remaining"]:
         reset_time = datetime.fromtimestamp(int(response.headers["x-ratelimit-reset"]))
-        print(
+        logging.warn(
             f"Rate limit reached: {response.headers['x-ratelimit-remaining']}/{response.headers['x-ratelimit-limit']} - {reset_time}"
         )
 
         time.sleep(int(response.headers["x-ratelimit-remaining"]))
         return True
 
     if response.status_code == 403:
         # This can be secondary rate limit or SSO error
-        print(response.json()["message"])
+        logging.warn(response.json()["message"])
         return True
 
     time.sleep(SLEEP_BETWEEN_REQUESTS)
     return False
 
+
 def check_unauthorized(response: Any):
     if response.status_code == 401:
-        print(response.json()["message"])
+        logging.error(response.json()["message"])
         return False
     return True
 
+
 def check_response(response: any):
     check_rate_limit(response)
     check_unauthorized(response)
 
+
 def get(*args, **kwargs):
     response = requests.get(*args, **kwargs)
     check_response(response)
     return response
 
+
 def post(*args, **kwargs):
     response = requests.post(*args, **kwargs)
     check_response(response)
     return response
 
+
 def put(*args, **kwargs):
     response = requests.put(*args, **kwargs)
     check_response(response)
     return response
 
+
 def patch(*args, **kwargs):
     response = requests.patch(*args, **kwargs)
     check_response(response)
     return response
```

### Comparing `ghas_cli-1.4.2/src/ghas_cli/utils/repositories.py` & `ghas_cli-1.5.0/src/ghas_cli/utils/repositories.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
 #!/usr/bin/env python3
 
 from typing import List, Any
 import base64
-import requests
 from . import network
 import time
 import datetime
+import logging
 
 
 class Repository:
     def __init__(
         self,
         name="",
         orga="Malwarebytes",
@@ -58,15 +58,15 @@
             self.orga = obj["owner"]["login"]
         else:
             self.orga = ""
         self.owner = obj["owner"]["login"]
         self.url = obj["html_url"]
         self.description = obj["description"]
         self.main_language = obj["language"]
-        self.languages = get_languages(self.orga, token, self.name, False, False)
+        self.languages = get_languages(self.orga, token, self.name)
         self.default_branch = obj["default_branch"]
         try:
             self.license = obj["license"]["spdx_id"]
         except Exception:
             self.license = None
         self.archived = obj["archived"]
         self.disabled = obj["disabled"]
@@ -168,45 +168,45 @@
             url=f"https://api.github.com/orgs/{organization}/repos",
             params=params,
             headers=headers,
         )
 
         if repos.status_code != 200:
             break
-    
+
         if [] == repos.json():
             break
 
         for r in repos.json():
             repo = Repository()
             repo.load_json(r, token=token)
             # repo.load_json(r, token=None)
 
             if language != "" and repo.main_language != language:
-                print(
+                logging.info(
                     f"{repo.name} ignored because of language: {language} vs. {repo.main_language}"
                 )
                 continue
             if default_branch != "" and repo.default_branch != default_branch:
-                print(
+                logging.info(
                     f"{repo.name} ignored because of default branch: {default_branch} vs. {repo.default_branch}"
                 )
                 continue
             if license != "" and repo.license != license:
-                print(
+                logging.info(
                     f"{repo.name} ignored because of license: {license} vs. {repo.license}"
                 )
                 continue
             if repo.archived != archived:
-                print(
+                logging.info(
                     f"{repo.name} ignored because of archived: {archived} vs. {repo.archived}"
                 )
                 continue
             if repo.disabled != disabled:
-                print(
+                logging.info(
                     f"{repo.name} ignored because of license: {archived} vs. {repo.archived}"
                 )
                 continue
 
             repos_list.append(repo)
 
         page += 1
@@ -358,112 +358,73 @@
         return False
 
 
 def get_languages(
     organization: str,
     token: str,
     repository: str,
-    only_interpreted: False,
-    only_codeql: False,
+    only_codeql: bool = False,
 ) -> List:
     """Get the main language for a repository"""
 
-    interpreted_languages = {"javascript", "python", "ruby"}
-    aliased_interpreted_languages = {"typescript": "javascript"}
+    codeql_languages = ["cpp", "csharp", "go", "java", "javascript", "python", "ruby"]
+    codeql_aliased_languages = {
+        "typescript": "javascript",
+        "kotlin": "java",
+        "c#": "csharp",
+        "c++": "cpp",
+    }
 
     headers = network.get_github_headers(token)
-    languages = network.get(
+    languages_resp = network.get(
         url=f"https://api.github.com/repos/{organization}/{repository}/languages",
         headers=headers,
     )
-    if languages.status_code != 200:
+
+    if languages_resp.status_code != 200:
+        logging.warn(f"Received status code {languages_resp.status_code} while retrieving repository languages.")
         return ["default"]
 
-    lang = set()
-    for l in languages.json():
-        if only_interpreted:
-            if l.lower() in interpreted_languages:
-                lang.add(l.lower())
-            else:
-                if only_codeql:
-                    try:
-                        lang.add(aliased_interpreted_languages[l.lower()])
-                    except Exception as e:
-                        continue
+    languages = list()
+    for language in [l.lower() for l in languages_resp.json()]:
+        if only_codeql:
+            if language in codeql_languages:
+                languages.append(language)
+            elif language in codeql_aliased_languages:
+                languages.append(codeql_aliased_languages[language])
         else:
-            lang.add(l.lower())
+            languages.append(language)
 
-    if not lang:
-        return ["default"]
-    else:
-        return list(lang)
+    return languages
 
 
-def load_codeql_base64_template(language: str, default_branch: str = "main") -> tuple:
-    language = language.lower()
-    try:
-        with open(f"./templates/codeql-analysis-{language.lower()}.yml", "r") as f:
-            # Ugly af but `yaml` transforms `on:` to `True:` which is obviously annoying to parse GitHub Actions files..
-            template = f.readlines()
-            template_new = ""
-            for l in template:
-                if l == '    branches: ["main"]\n':
-                    template_new += f"    branches: ['{default_branch}']\n"
-                else:
-                    template_new += l
-    except Exception as e:
-        with open(f"./templates/codeql-analysis-default.yml", "r") as f:
-            language = "default"
-            template = f.readlines()
-            template_new = ""
-            for l in template:
-                if l == '    branches: ["main"]\n':
-                    template_new += f"    branches: ['{default_branch}']\n"
-                else:
-                    template_new += l
-    return language, str(
-        base64.b64encode(template_new.encode(encoding="utf-8")), "utf-8"
-    )
+def load_codeql_base64_template(
+    languages: List, branches: List = ["main"]
+) -> str:
+    with open(f"./templates/codeql-analysis-default.yml", "r") as f:
+        data = "".join(f.readlines())
+        data = data.replace("""branches: [ ]""", f"""branches: [{', '.join(f"'branch'" for branch in branches)   }]""")
+        data = data.replace("""language: [ ]""", f"""language: {languages}""")
+        return base64.b64encode(data.encode("utf-8")).decode("utf-8")
 
 
-def load_codeql_config_base64_template(language: str) -> tuple:
-    language = language.lower()
-    try:
-        with open(f"./templates/codeql-config-{language.lower()}.yml", "r") as f:
-            template = f.read()
-    except Exception as e:
-        with open(f"./templates/codeql-config-default.yml", "r") as f:
-            template = f.read()
-    return language, str(base64.b64encode(template.encode(encoding="utf-8")), "utf-8")
-
-
-def create_codeql_pr(
-    organization: str,
-    token: str,
-    repository: str,
-    target_branch: str = "appsec-ghas-codeql_enable",
-) -> bool:
-    """
-    1. Retrieve the repository languages. Select the `codeql-analysis.yml` file for that language.
-    2. Create a branch
-    3. Push a .github/workflows/codeql-analysis.yml to the repository on that branch
-    3. Create an associated PR
-    """
-    headers = network.get_github_headers(token)
+def load_codeql_config_base64_template() -> str:
+    with open(f"./templates/codeql-config-default.yml", "r") as f:
+        template = f.read()
+        return base64.b64encode(template.encode(encoding="utf-8")).decode("utf-8")
 
-    # Get the default branch
-    default_branch = get_default_branch(organization, token, repository)
-    if not default_branch:
-        return False
 
-    # Create a branch
+def create_branch(
+    headers, organization: str, repository: str, default_branch: str, target_branch: str
+):
     branch_resp = network.get(
         url=f"https://api.github.com/repos/{organization}/{repository}/git/refs/heads",
         headers=headers,
     )
+
     if branch_resp.status_code != 200:
         return False
 
     refs = branch_resp.json()
     sha1 = ""
     for ref in refs:
         if ref["ref"] == f"refs/heads/{default_branch}":
@@ -479,81 +440,151 @@
 
     branch_resp = network.post(
         url=f"https://api.github.com/repos/{organization}/{repository}/git/refs",
         headers=headers,
         json=payload,
     )
 
-    if branch_resp.status_code != 201:
+    if branch_resp.status_code == 422:
+        logging.error("Branch already exists")
         return False
 
-    # Create commit
-    languages = get_languages(
-        organization, token, repository, only_interpreted=True, only_codeql=True
+    if branch_resp.status_code == 201:
+        return True
+
+    return False
+
+
+def create_codeql_pr(
+    organization: str,
+    token: str,
+    repository: str,
+    target_branch: str = "appsec-ghas-codeql_enable",
+) -> bool:
+    """
+    1. Retrieve the repository languages. Select the `codeql-analysis.yml` file for that language.
+    2. Create a branch
+    3. Push a .github/workflows/codeql-analysis.yml to the repository on that branch
+    3. Create an associated PR
+    """
+    headers = network.get_github_headers(token)
+
+    # Get the default branch
+    default_branch = get_default_branch(organization, token, repository)
+    if not default_branch:
+        return False
+
+    # Create a branch
+    new_branch = create_branch(
+        headers, organization, repository, default_branch, target_branch
     )
 
-    for language in languages:
-        # Workflow config
-        lang, template = load_codeql_base64_template(language, default_branch)
-        payload = {
-            "message": f"Enable CodeQL analysis for {language}",
-            "content": template,
-            "branch": target_branch,
-        }
+    if not new_branch:
+        logging.error(f"Couldn't create branch {target_branch}")
+        return False
 
-        commit_resp = network.put(
-            url=f"https://api.github.com/repos/{organization}/{repository}/contents/.github/workflows/codeql-analysis-{lang}.yml",
-            headers=headers,
-            json=payload,
+    # Create commit
+
+    languages = get_languages(organization, token, repository, only_codeql=True)
+
+    # Workflow config
+    template = load_codeql_base64_template(languages, [default_branch])
+    workflow_commit_payload = {
+        "message": f"Create CodeQL analysis workflow",
+        "content": template,
+        "branch": target_branch,
+        "sha": get_file_sha(
+            organization, repository, headers, ".github/workflows/codeql.yml"
+        ),
+    }
+
+    if workflow_commit_payload["sha"]:
+        workflow_commit_payload["message"] = "Update CodeQL analysis workflow"
+
+    workflow_commit_resp = network.put(
+        url=f"https://api.github.com/repos/{organization}/{repository}/contents/.github/workflows/codeql.yml",
+        headers=headers,
+        json=workflow_commit_payload,
+    )
+
+    if workflow_commit_resp.status_code not in [200, 201]:
+        logging.error(
+            f"Commit response for CodeQL workflow: {workflow_commit_resp.status_code}"
         )
+        return False
 
-        if commit_resp.status_code != 201:
-            return False
+    # CodeQL config file
+    template = load_codeql_config_base64_template()
+    config_commit_payload = {
+        "message": f"Create CodeQL config file",
+        "content": template,
+        "branch": target_branch,
+        "sha": get_file_sha(
+            organization,
+            repository,
+            headers,
+            ".github/codeql/codeql-config-default.yml",
+        ),
+    }
 
-        # CodeQL config file
-        lang, template = load_codeql_config_base64_template(language)
-        payload = {
-            "message": f"Enable CodeQL config file for {language}",
-            "content": template,
-            "branch": target_branch,
-        }
+    if config_commit_payload["sha"]:
+        config_commit_payload["message"] = "Update CodeQL config file"
 
-        commit_resp = network.put(
-            url=f"https://api.github.com/repos/{organization}/{repository}/contents/.github/codeql/codeql-config-{lang}.yml",
-            headers=headers,
-            json=payload,
+    config_commit_resp = network.put(
+        url=f"https://api.github.com/repos/{organization}/{repository}/contents/.github/codeql/codeql-config-default.yml",
+        headers=headers,
+        json=config_commit_payload,
+    )
+
+    if config_commit_resp.status_code not in [200, 201]:
+        logging.error(
+            f"Commit response for CodeQL config: {config_commit_resp.status_code}"
         )
-        if commit_resp.status_code != 201:
-            return False
+        return False
 
-    # Create PR
-    payload = {
-        "title": "Security Code Scanning - configuration files",
-        "body": f"This PR creates the Security scanning (CodeQL) configuration files for your repository languages ({languages}).\n\n We also just opened an informative issue in this repository to give you the context and assistance you need. In most cases you will be able to merge this PR as is and start benefiting from security scanning right away, as a check in each PR, and in the [Security tab](https://github.com/{organization}/{repository}/security/code-scanning) of this repository. \nHowever, we encourage you to review the configuration files and tag @{organization}/security-appsec (or `#github-appsec-security` on Slack) if you have any questions.\n\nWe are here to help! :thumbsup:\n\n - Application Security team.",
+    is_config_update = (
+        workflow_commit_payload["sha"] != None or config_commit_payload["sha"] != None
+    )
+
+    pr_payload = {
         "head": target_branch,
         "base": default_branch,
     }
 
+    if is_config_update:
+        logging.info(f"Updating configuration for {repository}")
+        pr_payload["title"] = "Security Code Scanning - updated configuration files"
+        pr_payload[
+            "body"
+        ] = f"This PR updates the Security scanning (CodeQL) configuration files for your repository languages ({', '.join(languages)}).We also just opened an informative issue in this repository to give you the context and assistance you need. In most cases you will be able to merge this PR as is and start benefiting from security scanning right away, as a check in each PR, and in the [Security tab](https://github.com/{organization}/{repository}/security/code-scanning) of this repository. \nHowever, we encourage you to review the configuration files and tag @{organization}/security-appsec (or `#github-appsec-security` on Slack) if you have any questions.\n\nWe are here to help! :thumbsup:\n\n - Application Security team."
+    else:
+        logging.info(f"Creating configuration for {repository}")
+        pr_payload["title"] = "Security Code Scanning - configuration files"
+        pr_payload[
+            "body"
+        ] = f"This PR creates the Security scanning (CodeQL) configuration files for your repository languages ({', '.join(languages)}).\n\n We also just opened an informative issue in this repository to give you the context and assistance you need. In most cases you will be able to merge this PR as is and start benefiting from security scanning right away, as a check in each PR, and in the [Security tab](https://github.com/{organization}/{repository}/security/code-scanning) of this repository. \nHowever, we encourage you to review the configuration files and tag @{organization}/security-appsec (or `#github-appsec-security` on Slack) if you have any questions.\n\nWe are here to help! :thumbsup:\n\n - Application Security team."
+
     # Retry if rate-limited
     i = 0
     while i < network.RETRIES:
         pr_resp = network.post(
             url=f"https://api.github.com/repos/{organization}/{repository}/pulls",
             headers=headers,
-            json=payload,
+            json=pr_payload,
         )
         if pr_resp.status_code == 201:
             return True
 
         if network.check_rate_limit(pr_resp):
             time.sleep(network.SLEEP_1_MINUTE)
 
         i += 1
 
     if pr_resp.status_code != 201:
+        print(pr_resp.json())
         return False
 
     return True
 
 
 ###### Dependency Review
 
@@ -580,45 +611,23 @@
 
     # Get the default branch
     default_branch = get_default_branch(organization, token, repository)
     if not default_branch:
         return False
 
     # Create a branch
-    branch_resp = network.get(
-        url=f"https://api.github.com/repos/{organization}/{repository}/git/refs/heads",
-        headers=headers,
-    )
-    if branch_resp.status_code != 200:
-        return False
-
-    refs = branch_resp.json()
-    sha1 = ""
-    for ref in refs:
-        if ref["ref"] == f"refs/heads/{default_branch}":
-            sha1 = ref["object"]["sha"]
-
-    if sha1 == "":
-        return False
 
-    payload = {
-        "ref": f"refs/heads/{target_branch}",
-        "sha": sha1,
-    }
-
-    branch_resp = network.post(
-        url=f"https://api.github.com/repos/{organization}/{repository}/git/refs",
-        headers=headers,
-        json=payload,
+    new_branch = create_branch(
+        headers, organization, repository, default_branch, target_branch
     )
 
-    if branch_resp.status_code != 201:
+    if not new_branch:
         return False
 
-    # Create commit
+    # # Create commit
     template = load_dependency_review_base64_template()
     payload = {
         "message": f"Enable Dependency reviewer",
         "content": template,
         "branch": target_branch,
     }
 
@@ -655,7 +664,17 @@
 
         i += 1
 
     if pr_resp.status_code != 201:
         return False
 
     return True
+
+
+def get_file_sha(organization, repository, headers, file):
+    file_resp = network.get(
+        url=f"https://api.github.com/repos/{organization}/{repository}/contents/{file}",
+        headers=headers,
+    )
+    if file_resp.status_code == 200:
+        return file_resp.json()["sha"]
+    return None
```

### Comparing `ghas_cli-1.4.2/src/ghas_cli/utils/roles.py` & `ghas_cli-1.5.0/src/ghas_cli/utils/roles.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.4.2/src/ghas_cli/utils/secrets.py` & `ghas_cli-1.5.0/src/ghas_cli/utils/secrets.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,12 +39,12 @@
             s["resolution"] = secret["resolution"]
             s["resolved_at"] = secret["resolved_at"]
             s["repository_full_name"] = secret["repository"]["full_name"]
             s["url"] = secret["url"]
             s["secret_type"] = secret["secret_type"]
             s["secret"] = secret["secret"]
 
-            if secrets_filter is "all" or s["secret_type"] == secrets_filter:
+            if secrets_filter == "all" or s["secret_type"] == secrets_filter:
                 secret_list.append(s)
 
         page += 1
     return secret_list
```

### Comparing `ghas_cli-1.4.2/src/ghas_cli/utils/teams.py` & `ghas_cli-1.5.0/src/ghas_cli/utils/teams.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,16 @@
             url=f"https://api.github.com/orgs/{organization}/teams/{team_slug}/repos",
             params=params,
             headers=headers,
         )
         if network.check_rate_limit(repos):
             break
 
-        # print(repos.status_code)
-        # print(repos.content)
+        # logging.debug(repos.status_code)
+        # logging.debug(repos.content)
         if repos.status_code != 200:
             break
 
         if [] == repos.json():
             break
 
         for r in repos.json():
@@ -83,19 +83,19 @@
     headers = network.get_github_headers(token)
 
     headers["accept"] = "application/vnd.github.v3.repository+json"
     teams_res = requests.get(
         url=f"https://api.github.com/orgs/{organization}/teams/{team}/repos/{organization}/{repo}",
         headers=headers,
     )
-    # print(teams_res.status_code)
+    # logging.debug(teams_res.status_code)
     if network.check_rate_limit(teams_res):
         return []
     if teams_res.status_code != 200:
         return []
 
     if [] == teams_res.json():
         return []
 
-    # print(teams_res.json()["role_name"])
+    # logging.debug(teams_res.json()["role_name"])
 
     return [teams_res.json()["permissions"], teams_res.json()["role_name"]]
```

### Comparing `ghas_cli-1.4.2/src/ghas_cli/utils/vulns.py` & `ghas_cli-1.5.0/src/ghas_cli/utils/vulns.py`

 * *Files identical despite different names*

### Comparing `ghas_cli-1.4.2/PKG-INFO` & `ghas_cli-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghas-cli
-Version: 1.4.2
+Version: 1.5.0
 Summary: Command line interface to interact with GitHub Advanced Security.
 Home-page: https://github.com/Malwarebytes/ghas-cli
 License: MIT
 Keywords: security,cli,github,utility
 Author: jboursier
 Author-email: jboursier@malwarebytes.com
 Requires-Python: >=3.7,<4
```

