# Comparing `tmp/dbt-ai-0.1.3a0.tar.gz` & `tmp/dbt-ai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-ai-0.1.3a0.tar", last modified: Sun May  7 12:33:19 2023, max compression
+gzip compressed data, was "dbt-ai-0.2.0.tar", last modified: Wed May 10 03:46:17 2023, max compression
```

## Comparing `dbt-ai-0.1.3a0.tar` & `dbt-ai-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1069 2023-05-07 00:28:17.000000 dbt-ai-0.1.3a0/LICENSE
--rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.1.3a0/MANIFEST.in
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3428 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3226 2023-05-07 12:32:37.000000 dbt-ai-0.1.3a0/README.md
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/dbt_ai/
--rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.1.3a0/dbt_ai/__init__.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     4413 2023-05-07 12:22:42.000000 dbt-ai-0.1.3a0/dbt_ai/ai.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     8097 2023-05-07 12:33:03.000000 dbt-ai-0.1.3a0/dbt_ai/dbt.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)      565 2023-05-07 06:43:19.000000 dbt-ai-0.1.3a0/dbt_ai/helper.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1698 2023-05-07 12:04:25.000000 dbt-ai-0.1.3a0/dbt_ai/main.py
--rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.1.3a0/dbt_ai/py.typed
--rw-r--r--   0 armalite  (1000) armalite  (1000)      811 2023-05-06 13:18:50.000000 dbt-ai-0.1.3a0/dbt_ai/report.py
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/dbt_ai/templates/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3094 2023-05-06 13:45:28.000000 dbt-ai-0.1.3a0/dbt_ai/templates/report_template.html
-drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/dbt_ai.egg-info/
--rw-r--r--   0 armalite  (1000) armalite  (1000)     3428 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/PKG-INFO
--rw-r--r--   0 armalite  (1000) armalite  (1000)      384 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/SOURCES.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/dependency_links.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/entry_points.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)      193 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/requires.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-07 12:33:19.000000 dbt-ai-0.1.3a0/dbt_ai.egg-info/top_level.txt
--rw-r--r--   0 armalite  (1000) armalite  (1000)     1625 2023-05-07 12:32:39.000000 dbt-ai-0.1.3a0/pyproject.toml
--rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-07 12:33:19.557895 dbt-ai-0.1.3a0/setup.cfg
--rw-r--r--   0 armalite  (1000) armalite  (1000)      144 2023-05-06 13:15:40.000000 dbt-ai-0.1.3a0/setup.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-10 03:46:17.900000 dbt-ai-0.2.0/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1069 2023-05-07 00:28:17.000000 dbt-ai-0.2.0/LICENSE
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       71 2023-05-06 13:04:03.000000 dbt-ai-0.2.0/MANIFEST.in
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     4212 2023-05-10 03:46:17.900000 dbt-ai-0.2.0/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     4012 2023-05-10 03:46:06.000000 dbt-ai-0.2.0/README.md
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-10 03:46:17.850000 dbt-ai-0.2.0/dbt_ai/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        0 2023-05-05 05:14:16.000000 dbt-ai-0.2.0/dbt_ai/__init__.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     7603 2023-05-10 03:43:35.000000 dbt-ai-0.2.0/dbt_ai/ai.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     9524 2023-05-10 03:43:35.000000 dbt-ai-0.2.0/dbt_ai/dbt.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      565 2023-05-07 06:43:19.000000 dbt-ai-0.2.0/dbt_ai/helper.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     2247 2023-05-10 03:43:35.000000 dbt-ai-0.2.0/dbt_ai/main.py
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       80 2023-05-05 05:14:16.000000 dbt-ai-0.2.0/dbt_ai/py.typed
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      811 2023-05-06 13:18:50.000000 dbt-ai-0.2.0/dbt_ai/report.py
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-10 03:46:17.860000 dbt-ai-0.2.0/dbt_ai/templates/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     3094 2023-05-06 13:45:28.000000 dbt-ai-0.2.0/dbt_ai/templates/report_template.html
+drwxr-xr-x   0 armalite  (1000) armalite  (1000)        0 2023-05-10 03:46:17.860000 dbt-ai-0.2.0/dbt_ai.egg-info/
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     4212 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/PKG-INFO
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      384 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)        1 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       44 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/entry_points.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      193 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/requires.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       51 2023-05-10 03:46:17.000000 dbt-ai-0.2.0/dbt_ai.egg-info/top_level.txt
+-rw-r--r--   0 armalite  (1000) armalite  (1000)     1619 2023-05-10 03:45:40.000000 dbt-ai-0.2.0/pyproject.toml
+-rw-r--r--   0 armalite  (1000) armalite  (1000)       38 2023-05-10 03:46:17.900000 dbt-ai-0.2.0/setup.cfg
+-rw-r--r--   0 armalite  (1000) armalite  (1000)      144 2023-05-06 13:15:40.000000 dbt-ai-0.2.0/setup.py
```

### Comparing `dbt-ai-0.1.3a0/LICENSE` & `dbt-ai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.3a0/PKG-INFO` & `dbt-ai-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,74 +1,91 @@
-Metadata-Version: 2.1
-Name: dbt-ai
-Version: 0.1.3a0
-Summary: AI powered DBT helper application
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 # DBT AI
 
-This application provides AI generated recommendations on how to improve your [DBT](https://www.getdbt.com/) models.
+An application that allows AI powered [DBT](https://www.getdbt.com/) development and recommendations for your [DBT](https://www.getdbt.com/) models.
 
 ## Features
  - Scans all dbt models and generates a report containing recommendations for each model
+   - By default only basic recommendations are provided
+   - Ability to request for more advanced recommendations
+ - Create DBT models by using AI prompts
  - Lists dbt models that are missing associated metadata e.g. in a `schema.yml` file or equivalent
- - Use AI to generate DBT models for you based on a prompt
  - DBT model lineage description is listed in the terminal (more features coming soon)
 
 ## Installation
 You can install the application here
 ```bash
-pip install dbt-ai==0.1.3a0
+pip install dbt-ai==0.2.0
 ```
 
 WARNING: This is an early phase application that may still contain bugs
 
 ## Prerequisites
- - In order to benefit from AI recommendations, you need your own OpenAI API Key with the initial version of this application
+ - In order to benefit from AI features, you need your own OpenAI API Key with the initial version of this application
     - Once you sign up to [OpenAI](https://openai.com/product) you can create an API key. 
     - Trial version gives you a certain amount of credits allowing you to make many API calls
     - Usage beyond the trial credits require billing details. [API usage pricing](https://openai.com/pricing) provides more info
  - Ideally you already have dbt project to test this out on
  - Python 3.10 or greater is required
 
 
 ## Usage
 Setting up your API key is needed for all the AI features
  - Set up your OpenAI API key as an environment variable:
 ```bash
-    export OPENAI_API_KEY="your_openai_api_key"
+export OPENAI_API_KEY="your_openai_api_key"
 ```
 
 ### Generate Recommendations (AI)
 This feature will generate the recommendation report and also inform you about any models missing metadata
+
+#### Basic Usage
+The default setting is to provide basic recommendations
   1. Run the application passing in the path to your dbt project:
 ```bash
-    dbt-ai -f path/to/dbt/project
+dbt-ai -f path/to/dbt/project
 ```
 
 For example, if you are already inside your dbt project directory, you can run:
 ```bash
-   dbt-ai -f .
+dbt-ai -f .
 ```
 
+#### Available Settings
+
+   - Database: specify which database system your dbt models are written for. Default: `snowflake`
+      - `-d` / `--database`
+      - Available values: `snowflake`, `postgres`, `redshift`, `bigquery`
+      - Usage example: 
+      ```bash
+      dbt ai -f . -d snowflake
+      ```
+   - Advanced Recommendation: Request for advanced recommendations. Default: No setting defaults to basic recommendations
+      - `-a` / `--advanced-rec`
+      - Available values: Only flag required
+      - Usage example: 
+      ```bash
+      dbt ai -f . -a 
+      ```
+      Or
+      ```bash
+      dbt ai -f . --advanced-req
+      ```
+
 Please allow some time for the AI model to process your dbt models. The application will process all dbt model files in your project and generate an HTML report with suggestions for each model. The report will be saved as dbt_model_suggestions.html within the dbt project directory. Upon generation of the report, it will be opened in a new browser tab.
 
 ### Create DBT Models from prompt (AI)
-This feature lets you specify a prompt, which creates AI generated DBT model files for your in the `models/` directory of your specified dbt project. You can assume that the AI model has access to your `sources.yml` file, if you wish to refer to any sources in your prompt. Being specific will provide better results.
+This feature lets you specify a prompt, which creates AI generated DBT model files in the `models/` directory of the specified dbt project. The AI model has access to your `sources.yml` file, if you wish to refer to any sources in your prompt. Being specific will provide better results.
  1. Run the application with the --create-models flag to specify the prompt you wish to use to create your DBT models
  ```bash
-    dbt-ai -f path/to/dbt/project --create-models 'your prompt goes here'
+dbt-ai -f path/to/dbt/project --create-models 'your prompt goes here'
  ```
 
 Here is an example:
 ```bash
-   dbt-ai -f . --create-models 'Write me a model that uses all the sources available in sources.yml and joins them together using the id column'
+dbt-ai -f . --create-models 'Write me a model that uses all the sources available in sources.yml and joins them together using the id column'
 ```
 
 ## Generated Report
 This shows an example of a report generated from a DBT project containing 3 models
 ![](images/generated_report_1.png?raw=true)
 
 ## Contributing
```

### Comparing `dbt-ai-0.1.3a0/dbt_ai/dbt.py` & `dbt-ai-0.2.0/dbt_ai/dbt.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,31 @@
+# flake8: noqa
+
 import glob
 import os
 import re
-import yaml
-import uuid
+from typing import Callable
+
 import networkx as nx
-from pyvis.network import Network
 import plotly.graph_objects as go
+import yaml
 
-from dbt_ai.ai import generate_response, generate_dalle_image, generate_models
+from dbt_ai.ai import generate_dalle_image, generate_models, generate_response, generate_response_advanced
 from dbt_ai.helper import find_yaml_files
 
 
 class DbtModelProcessor:
     """Class containing functions to process and analyse a DBT project"""
 
-    def __init__(self, dbt_project_path) -> None:
+    def __init__(self, dbt_project_path: str, database: str = "snowflake") -> None:
         self.dbt_project_path = dbt_project_path
         self.yaml_files = find_yaml_files(dbt_project_path)
         self.api_key_available = bool(os.getenv("OPENAI_API_KEY"))
         self.sources_yml_content = self.read_sources_yml(dbt_project_path)
+        self.database = database
         if not self.api_key_available:
             print("Warning: OPENAI_API_KEY is not set. Suggestion features will be unavailable.")
 
     def read_sources_yml(self, dbt_project_path: str):
         sources_yml_path = os.path.join(dbt_project_path, "models", "sources.yml")
         try:
             with open(sources_yml_path, "r") as f:
@@ -39,108 +42,126 @@
         refs = re.findall(r"ref\(['\"]([\w\.]+)['\"]\)", content)
 
         return refs
 
     def suggest_dbt_model_improvements(self, file_path: str, model_name: str) -> list:
         with open(file_path, "r") as f:
             content = f.read()
-        prompt = f"Given the following dbt model {model_name}:\n\n{content}\n\nPlease provide suggestions on how to improve this model in terms of syntax, code structure and dbt best practices such as using ref instead of hardcoding table names:"
+        prompt = f"""Given the following dbt model {model_name}:\n\n{content}\n\nPlease provide suggestions on how to improve this model in terms of syntax, code structure and dbt best practices \
+            such as using ref instead of hardcoding table names. The suggestion should be specific to db models written in the {self.database} database system: \
+            """
         response = generate_response(prompt)
         return response
 
-    def model_has_metadata(self, model_name: str) -> bool:
-        for yaml_file in self.yaml_files:
-            with open(yaml_file, "r") as f:
-                try:
-                    yaml_content = yaml.safe_load(f)
-
-                    if yaml_content:
-                        for item in yaml_content.get("models", []):
-                            if isinstance(item, dict) and item.get("name") == model_name:
-                                return True
-                except yaml.YAMLError as e:
-                    print(f"Error parsing YAML file {yaml_file}: {e}")
-
-        return False
+    def suggest_dbt_model_improvements_advanced(self, file_path: str, model_name: str) -> list:
+        with open(file_path, "r") as f:
+            content = f.read()
+        prompt = f"""Given the following dbt model {model_name}:\n\n{content}\n\n \
+            Please provide advanced suggestions on how to improve this model.
+            The suggestion should be specific to dbt models written in the {self.database} database system 
+            If there are no advanced recommendations to provide, then do not provide anything. If you are lacking context required to provide any advanced
+            recommendations then don't provide anything. Example of an advanced recommendation include suggesting Snowflake partitioning keys when you see table names 
+            being used that are very likely to be large tables e.g. invoice or journal line tables. Note that is just one example.
+                """
+        response = generate_response_advanced(prompt)
+        return response
 
-    def process_model(self, model_file: str) -> dict:
+    def process_model(self, model_file: str, advanced: bool = False):
         model_name = os.path.basename(model_file).replace(".sql", "")
 
         has_metadata = self.model_has_metadata(model_name)
         if self.api_key_available:
-            raw_suggestion = self.suggest_dbt_model_improvements(model_file, model_name)
+            if advanced:
+                raw_suggestion = self.suggest_dbt_model_improvements_advanced(model_file, model_name)
+            else:
+                raw_suggestion = self.suggest_dbt_model_improvements(model_file, model_name)
         else:
             raw_suggestion = ""
 
         refs = self.get_model_refs(model_file)
 
         return {
             "model_name": model_name,
             "metadata_exists": has_metadata,
             "suggestions": raw_suggestion,
             "refs": refs,
         }
 
-    def process_dbt_models(self):  # flake8: noqa
+    def process_dbt_models(self, advanced: bool = False):
         model_files = glob.glob(os.path.join(self.dbt_project_path, "models/**/*.sql"), recursive=True)
-        models = [self.process_model(model_file) for model_file in model_files]
+        models = [self.process_model(model_file, advanced) for model_file in model_files]
         missing_metadata = []
 
         # Check for models without metadata
         for model in models:
             if not model["metadata_exists"]:
                 missing_metadata.append(model["model_name"])
 
         return models, missing_metadata
 
+    def model_has_metadata(self, model_name: str) -> bool:
+        for yaml_file in self.yaml_files:
+            with open(yaml_file, "r") as f:
+                try:
+                    yaml_content = yaml.safe_load(f)
+
+                    if yaml_content:
+                        for item in yaml_content.get("models", []):
+                            if isinstance(item, dict) and item.get("name") == model_name:
+                                return True
+                except yaml.YAMLError as e:
+                    print(f"Error parsing YAML file {yaml_file}: {e}")
+
+        return False
+
     def generate_lineage_graph(self, models):
         # Create a directed graph
-        G = nx.DiGraph()
+        gph = nx.DiGraph()
 
         # Add nodes for each model
         for model in models:
-            G.add_node(model["model_name"], metadata_exists=model["metadata_exists"])
+            gph.add_node(model["model_name"], metadata_exists=model["metadata_exists"])
 
         # Add edges based on ref() calls
         for model in models:
             refs = model["refs"]
             for ref in refs:
-                G.add_edge(ref, model["model_name"])
+                gph.add_edge(ref, model["model_name"])
 
-        return G
+        return gph
 
-    def generate_lineage_description(self, G: nx.DiGraph) -> str:
-        nodes = list(nx.topological_sort(G))
+    def generate_lineage_description(self, gph: nx.DiGraph) -> str:
+        nodes = list(nx.topological_sort(gph))
 
         description = ""  # "The following DBT models are used:\n\n"
         for node in nodes:
-            parents = list(G.predecessors(node))
+            parents = list(gph.predecessors(node))
             if parents:
                 parent_names = ", ".join(parents)
                 description += f"{node} depends on {parent_names}\n"
             else:
                 description += f"{node} is a root node\n"
 
         return description
 
     def generate_lineage(self, dbt_models: list[dict]):
-        G = self.generate_lineage_graph(dbt_models)
-        description = self.generate_lineage_description(G)
-        return description, G
+        gph = self.generate_lineage_graph(dbt_models)
+        description = self.generate_lineage_description(gph)
+        return description, gph
 
     def generate_image(self, description: str) -> None:
         image_binary = generate_dalle_image(description)
         image_path = f"{self.dbt_project_path}/lineage.png"
         print(f"Saving generated lineage image in {image_path}")
         # Write image to file
         with open(image_path, "wb") as f:
             f.write(image_binary)
 
-    def plot_directed_graph(self, G: nx.DiGraph):
-        pos = nx.spring_layout(G, seed=42)
+    def plot_directed_graph(self, gph: nx.DiGraph):
+        pos = nx.spring_layout(gph, seed=42)
 
         node_trace = go.Scatter(
             x=[],
             y=[],
             text=[],
             mode="markers+text",
             textposition="top center",
@@ -156,28 +177,28 @@
             y=[],
             line=dict(width=2, color="#888"),
             hoverinfo="none",
             mode="lines",
             name="Edges",
         )
 
-        for node in G.nodes():
+        for node in gph.nodes():
             x, y = pos[node]
             node_trace["x"] += tuple([x])
             node_trace["y"] += tuple([y])
             node_trace["text"] += tuple([node])
 
             # set marker color and/or text label based on whether the model has metadata or not
-            if "metadata_exists" in G.nodes[node] and not G.nodes[node]["metadata_exists"]:
+            if "metadata_exists" in gph.nodes[node] and not gph.nodes[node]["metadata_exists"]:
                 node_trace["marker"]["color"] = missing_metadata_color
                 node_trace["text"] += tuple(["MISSING METADATA"])
             else:
                 node_trace["marker"]["color"] = "rgb(71, 122, 193)"
 
-        for edge in G.edges():
+        for edge in gph.edges():
             x0, y0 = pos[edge[0]]
             x1, y1 = pos[edge[1]]
             edge_trace["x"] += tuple([x0, x1, None])
             edge_trace["y"] += tuple([y0, y1, None])
 
         fig = go.Figure(data=[edge_trace, node_trace])
         fig.update_layout(
@@ -190,22 +211,22 @@
             xaxis=dict(showgrid=False, zeroline=False, showticklabels=False, range=[-1.2, 1.2]),
             yaxis=dict(showgrid=False, zeroline=False, showticklabels=False, range=[-1.2, 1.2]),
         )
 
         fig.show()
 
     def create_dbt_models(self, prompt: str) -> None:
-        print(f"Attempting to create dbt models based on prompt")
+        print("Attempting to create dbt models based on prompt")
         sources_yml = self.sources_yml_content if self.sources_yml_content else ""
         response = generate_models(prompt, sources_yml)
 
         model_delimiter = "===\n\n"
         response_lines = response[0].split(model_delimiter)
 
-        for i, model_str in enumerate(response_lines):
+        for _i, model_str in enumerate(response_lines):
             if not model_str.strip():
                 continue
 
             model_lines = model_str.strip().split("\n")
             model_name = model_lines[0].split(":")[-1].strip()
             model_content = "\n".join(model_lines[1:])
             model_content = model_content.replace("===", "")
```

### Comparing `dbt-ai-0.1.3a0/dbt_ai/helper.py` & `dbt-ai-0.2.0/dbt_ai/helper.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.3a0/dbt_ai/main.py` & `dbt-ai-0.2.0/dbt_ai/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,40 +11,54 @@
     )
     parser.add_argument("-f", "--dbt-project-path", help="Path to the dbt project directory")
     parser.add_argument(
         "--create-models",
         help="Create dbt models using the provided prompt",
         default=None,
     )
+    parser.add_argument(
+        "-a",
+        "--advanced-rec",
+        action="store_true",
+        help="Generate only advanced recommendations for dbt models",
+    )
+    parser.add_argument(
+        "-d",
+        "--database",
+        help="Specify the type of database system the dbt project is built on",
+        choices=["snowflake", "postgres", "redshift", "bigquery"],
+        default="snowflake",
+    )
     args = parser.parse_args()
 
     if not args.create_models:
-        processor = DbtModelProcessor(args.dbt_project_path)
-        models, missing_metadata = processor.process_dbt_models()
+        processor = DbtModelProcessor(args.dbt_project_path, args.database)
+
+        models, missing_metadata = processor.process_dbt_models(advanced=args.advanced_rec)
 
         output_path = os.path.join(args.dbt_project_path, "dbt_model_suggestions.html")
 
         lineage_description, graph = processor.generate_lineage(models)
         # processor.plot_directed_graph(graph)
 
         print(f"Lineage description:\n {lineage_description}")
 
         generate_html_report(models, output_path, missing_metadata)
-
-        print(f"Generated improvement suggestions report at: {output_path}")
+        advancedprint = "advanced " if args.advanced_rec else ""
+        print(f"Generated {advancedprint}improvement suggestions report at: {output_path}")
 
         models_without_metadata = [model["model_name"] for model in models if not model["metadata_exists"]]
 
         if models_without_metadata:
             print("\nThe following models are missing metadata:")
             for model_name in models_without_metadata:
                 print(f"  - {model_name}")
         else:
             print("\nAll models have associated metadata.")
     else:
-        processor = DbtModelProcessor(args.dbt_project_path)
+        processor = DbtModelProcessor(args.dbt_project_path, args.database)
         prompt = args.create_models
         processor.create_dbt_models(prompt)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dbt-ai-0.1.3a0/dbt_ai/report.py` & `dbt-ai-0.2.0/dbt_ai/report.py`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.3a0/dbt_ai/templates/report_template.html` & `dbt-ai-0.2.0/dbt_ai/templates/report_template.html`

 * *Files identical despite different names*

### Comparing `dbt-ai-0.1.3a0/pyproject.toml` & `dbt-ai-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "dbt-ai"
 description = "AI powered DBT helper application"
-version = "0.1.3-alpha"
+version = "0.2.0"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
     "dbt-snowflake~=1.4",
     "openai~=0.27",
     "pyyaml~=6.0",
     "markdown2~=2.4",
```

