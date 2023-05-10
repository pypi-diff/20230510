# Comparing `tmp/terka-1.7.2.2.tar.gz` & `tmp/terka-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terka-1.7.2.2.tar", last modified: Mon May  8 13:55:04 2023, max compression
+gzip compressed data, was "terka-1.8.0.tar", last modified: Wed May 10 19:38:21 2023, max compression
```

## Comparing `terka-1.7.2.2.tar` & `terka-1.8.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.900599 terka-1.7.2.2/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-08 13:55:04.896598 terka-1.7.2.2/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-08 13:55:04.900599 terka-1.7.2.2/setup.cfg
--rw-r--r--   0 am        (1000) am        (1000)      905 2023-05-08 13:54:13.000000 terka-1.7.2.2/setup.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/__init__.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/adapters/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/adapters/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.7.2.2/terka/adapters/orm.py
--rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/adapters/repository.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/domain/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/collaborators.py
--rw-r--r--   0 am        (1000) am        (1000)    44918 2023-05-08 13:53:31.000000 terka-1.7.2.2/terka/domain/commands.py
--rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/commentary.py
--rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/element.py
--rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.7.2.2/terka/domain/epic.py
--rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/event_history.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/domain/external_connectors/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/external_connectors/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.7.2.2/terka/domain/external_connectors/asana.py
--rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.7.2.2/terka/domain/helpers.py
--rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/project.py
--rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.7.2.2/terka/domain/sprint.py
--rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.7.2.2/terka/domain/story.py
--rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/tag.py
--rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/task.py
--rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/time_tracker.py
--rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/domain/user.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/entrypoints/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/entrypoints/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.7.2.2/terka/entrypoints/cli.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka/service_layer/
--rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/service_layer/__init__.py
--rw-r--r--   0 am        (1000) am        (1000)    30533 2023-05-03 19:48:20.000000 terka-1.7.2.2/terka/service_layer/printer.py
--rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/service_layer/services.py
--rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/service_layer/ui.py
--rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.7.2.2/terka/service_layer/vertical_layout.css
--rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.7.2.2/terka/service_layer/views.py
--rw-r--r--   0 am        (1000) am        (1000)     7907 2023-05-03 15:38:36.000000 terka-1.7.2.2/terka/utils.py
-drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-08 13:55:04.896598 terka-1.7.2.2/terka.egg-info/
--rw-r--r--   0 am        (1000) am        (1000)      294 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/PKG-INFO
--rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/SOURCES.txt
--rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/dependency_links.txt
--rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/entry_points.txt
--rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/requires.txt
--rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-08 13:55:04.000000 terka-1.7.2.2/terka.egg-info/top_level.txt
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.957159 terka-1.8.0/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-10 19:38:21.957159 terka-1.8.0/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)       38 2023-05-10 19:38:21.957159 terka-1.8.0/setup.cfg
+-rw-r--r--   0 am        (1000) am        (1000)      903 2023-05-10 19:37:49.000000 terka-1.8.0/setup.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/__init__.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/adapters/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/adapters/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    16361 2023-04-26 19:48:32.000000 terka-1.8.0/terka/adapters/orm.py
+-rw-r--r--   0 am        (1000) am        (1000)     6150 2023-04-26 19:47:22.000000 terka-1.8.0/terka/adapters/repository.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/domain/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      576 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/collaborators.py
+-rw-r--r--   0 am        (1000) am        (1000)    44829 2023-05-10 19:36:37.000000 terka-1.8.0/terka/domain/commands.py
+-rw-r--r--   0 am        (1000) am        (1000)     1643 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/commentary.py
+-rw-r--r--   0 am        (1000) am        (1000)      102 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/element.py
+-rw-r--r--   0 am        (1000) am        (1000)     1513 2023-05-01 11:31:58.000000 terka-1.8.0/terka/domain/epic.py
+-rw-r--r--   0 am        (1000) am        (1000)     1440 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/event_history.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/domain/external_connectors/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/external_connectors/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)      265 2023-04-26 19:49:46.000000 terka-1.8.0/terka/domain/external_connectors/asana.py
+-rw-r--r--   0 am        (1000) am        (1000)      356 2023-01-29 21:37:09.000000 terka-1.8.0/terka/domain/helpers.py
+-rw-r--r--   0 am        (1000) am        (1000)      892 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/project.py
+-rw-r--r--   0 am        (1000) am        (1000)     2244 2023-05-03 16:06:42.000000 terka-1.8.0/terka/domain/sprint.py
+-rw-r--r--   0 am        (1000) am        (1000)     1495 2023-05-01 11:32:09.000000 terka-1.8.0/terka/domain/story.py
+-rw-r--r--   0 am        (1000) am        (1000)      639 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/tag.py
+-rw-r--r--   0 am        (1000) am        (1000)     2082 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/task.py
+-rw-r--r--   0 am        (1000) am        (1000)      530 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/time_tracker.py
+-rw-r--r--   0 am        (1000) am        (1000)      338 2023-04-26 19:47:22.000000 terka-1.8.0/terka/domain/user.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/entrypoints/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/entrypoints/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)     6055 2023-04-30 19:45:41.000000 terka-1.8.0/terka/entrypoints/cli.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka/service_layer/
+-rw-r--r--   0 am        (1000) am        (1000)        0 2023-04-26 19:47:22.000000 terka-1.8.0/terka/service_layer/__init__.py
+-rw-r--r--   0 am        (1000) am        (1000)    31416 2023-05-10 19:34:32.000000 terka-1.8.0/terka/service_layer/printer.py
+-rw-r--r--   0 am        (1000) am        (1000)     2924 2023-04-26 19:47:22.000000 terka-1.8.0/terka/service_layer/services.py
+-rw-r--r--   0 am        (1000) am        (1000)     3882 2023-04-26 19:47:22.000000 terka-1.8.0/terka/service_layer/ui.py
+-rw-r--r--   0 am        (1000) am        (1000)      698 2023-04-26 19:47:22.000000 terka-1.8.0/terka/service_layer/vertical_layout.css
+-rw-r--r--   0 am        (1000) am        (1000)     2382 2023-04-30 10:27:47.000000 terka-1.8.0/terka/service_layer/views.py
+-rw-r--r--   0 am        (1000) am        (1000)     7907 2023-05-10 15:50:27.000000 terka-1.8.0/terka/utils.py
+drwxr-xr-x   0 am        (1000) am        (1000)        0 2023-05-10 19:38:21.953159 terka-1.8.0/terka.egg-info/
+-rw-r--r--   0 am        (1000) am        (1000)      292 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/PKG-INFO
+-rw-r--r--   0 am        (1000) am        (1000)      993 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/SOURCES.txt
+-rw-r--r--   0 am        (1000) am        (1000)        1 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/dependency_links.txt
+-rw-r--r--   0 am        (1000) am        (1000)       53 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/entry_points.txt
+-rw-r--r--   0 am        (1000) am        (1000)       52 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/requires.txt
+-rw-r--r--   0 am        (1000) am        (1000)        6 2023-05-10 19:38:21.000000 terka-1.8.0/terka.egg-info/top_level.txt
```

### Comparing `terka-1.7.2.2/setup.py` & `terka-1.8.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 HERE = pathlib.Path(__file__).parent
 # README = (HERE.parent / "README.md").read_text()
 
 setup(
     name="terka",
-    version="1.7.2.2",
+    version="1.8.0",
     description="CLI utility for creating and managing tasks in a terminal",
     # long_description=README,
     long_description_content_type="text/markdown",
     author="Andrei Markin",
     author_email="andrey.markin.ppc@gmail.com",
     license="Apache 2.0",
     url="https://github.com/AndreyMarkinPPC/terka",
```

### Comparing `terka-1.7.2.2/terka/adapters/orm.py` & `terka-1.8.0/terka/adapters/orm.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/adapters/repository.py` & `terka-1.8.0/terka/adapters/repository.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/collaborators.py` & `terka-1.8.0/terka/domain/collaborators.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/commands.py` & `terka-1.8.0/terka/domain/commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,18 +248,15 @@
                 if "all" in kwargs:
                     kwargs["status"] = "DELETED,ACTIVE,ON_HOLD,COMPLETED"
                     del kwargs["all"]
                     show_completed = True
                 else:
                     kwargs["status"] = "ACTIVE"
 
-            if (custom_sort := kwargs.get("sort")):
-                del kwargs["sort"]
-            else:
-                custom_sort = None
+            custom_sort = kwargs.pop("sort", None)
             if entity_type == "projects" and "project_id" in kwargs:
                 kwargs["id"] = kwargs.pop("project_id")
             if has_collaborators := "collaborators" in kwargs:
                 collaborator_name = kwargs["collaborators"]
                 collaborator = self.repo.list(User,
                                               {"name": collaborator_name})
                 if collaborator:
```

### Comparing `terka-1.7.2.2/terka/domain/commentary.py` & `terka-1.8.0/terka/domain/commentary.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/epic.py` & `terka-1.8.0/terka/domain/epic.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/event_history.py` & `terka-1.8.0/terka/domain/event_history.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/project.py` & `terka-1.8.0/terka/domain/project.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/sprint.py` & `terka-1.8.0/terka/domain/sprint.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/story.py` & `terka-1.8.0/terka/domain/story.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/tag.py` & `terka-1.8.0/terka/domain/tag.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/task.py` & `terka-1.8.0/terka/domain/task.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/domain/time_tracker.py` & `terka-1.8.0/terka/domain/time_tracker.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/entrypoints/cli.py` & `terka-1.8.0/terka/entrypoints/cli.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/service_layer/printer.py` & `terka-1.8.0/terka/service_layer/printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             if entities:
                 self.print_sprint(entities, repo, print_options, kwargs)
             else:
                 exit(f"No sprint with id '{task}' found!")
         if entity_type in ("epics", "stories"):
             if entities:
                 self.print_composite(entities, repo, print_options,
-                                     entity_type)
+                                     entity_type, kwargs)
             else:
                 exit(f"No {entity_type} with id '{task}' found!")
         if entity_type == "projects":
             if entities:
                 self.print_project(entities, print_options, kwargs)
             else:
                 exit(f"No project '{task}' found!")
@@ -101,21 +101,25 @@
                 print(f"No task with id '{task}' found!")
 
     def print_entities(self, entities, type, repo, custom_sort, print_options):
         if type == "projects":
             entities.sort(key=self._sort_open_tasks, reverse=True)
             self.print_project(entities, print_options)
         elif type == "tasks":
-            if custom_sort:
+            if custom_sort and custom_sort not in ("status", "priority"):
                 entities.sort(key=lambda c: getattr(c, custom_sort),
                               reverse=False)
+            elif custom_sort == "status":
+                entities.sort(key=lambda c: c.status.value,
+                              reverse=True)
+            elif custom_sort == "priority":
+                entities.sort(key=lambda c: c.priority.value,
+                              reverse=True)
             else:
-                entities.sort(key=lambda c:
-                              (c.status.value, c.priority.value
-                               if hasattr(c.priority, "value") else 0),
+                entities.sort(key=lambda c: (c.status.value, c.priority.value),
                               reverse=True)
             self.print_task(entities=entities,
                             repo=repo,
                             print_options=print_options,
                             custom_sort=custom_sort)
         elif type == "tags":
             self.print_tag(entities=entities)
@@ -163,15 +167,15 @@
             table.add_column(column)
         for entity in entities:
             table.add_row(f"[red]{entity.id}[/red]",
                           entity.date.strftime("%Y-%m-%d %H:%M"), entity.text)
         if table.row_count:
             self.console.print(table)
 
-    def print_composite(self, entities, repo, print_options, composite_type):
+    def print_composite(self, entities, repo, print_options, composite_type, kwargs=None):
         table = Table(box=self.box, title=composite_type.upper(), expand=True)
         for column in ("id", "name", "description", "project", "tasks"):
             table.add_column(column, style="bold")
         for i, entity in enumerate(entities):
             tasks = []
             completed_tasks = []
             for entity_task in entity.tasks:
@@ -192,20 +196,22 @@
         if table.row_count:
             self.console.print(table)
         if print_options.show_tasks and tasks:
             self.print_task(entities=tasks,
                             repo=repo,
                             print_options=print_options,
                             show_window=False,
-                            view_level=composite_type[:-1])
+                            view_level=composite_type[:-1],
+                            kwargs=kwargs)
         if print_options.show_tasks and completed_tasks:
             self.print_task(entities=completed_tasks,
                             repo=repo,
                             print_options=print_options,
-                            show_window=False)
+                            show_window=False,
+                            kwargs=kwargs)
         if i == 0 and print_options.show_commentaries and (
                 commentaries := entity.commentaries):
             self.print_commentaries(commentaries)
 
     def print_sprint(self, entities, repo, print_options, kwargs=None):
         table = Table(box=rich.box.SQUARE_DOUBLE_HEAD)
         for column in ("id", "start_date", "end_date", "goal", "status",
@@ -368,19 +374,19 @@
             self.console.print("[green]Inactive projects[/green]")
             self.console.print(non_active_projects)
         non_task_view_options = deepcopy(print_options)
         non_task_view_options.show_tasks = False
         if print_options.show_epics and (epics := entity.epics):
             self.console.print("")
             self.print_composite(epics, self.repo, non_task_view_options,
-                                 "epics")
+                                 "epics", kwargs)
         if print_options.show_stories and (stories := entity.stories):
             self.console.print("")
             self.print_composite(stories, self.repo, non_task_view_options,
-                                 "stories")
+                                 "stories", kwargs)
         if print_options.show_tasks and (tasks := entity.tasks):
             task_print_options = deepcopy(print_options)
             task_print_options.show_commentaries = False
             self.console.print("")
             self.print_task(entities=tasks,
                             repo=self.repo,
                             print_options=task_print_options,
@@ -414,19 +420,26 @@
         # if (entities[0].status.name == "DONE"):
         #     console.print(f"[green]task is completed on [/green]")
         # else:
         #     active_in_days = datetime.now() - entities[0].creation_date
         #     console.print(f"[blue]task is active {active_in_days.days} days[/blue]")
         entities = list(entities)
         if kwargs:
+            custom_sort = custom_sort or kwargs.pop("sort", None)
             entities = self._get_filtered_entities(entities, kwargs)
         if not story_points:
-            if custom_sort:
+            if custom_sort and custom_sort not in ("status", "priority"):
                 entities.sort(key=lambda c: getattr(c, custom_sort),
                               reverse=False)
+            elif custom_sort == "status":
+                entities.sort(key=lambda c: c.status.value,
+                              reverse=True)
+            elif custom_sort == "priority":
+                entities.sort(key=lambda c: c.priority.value,
+                              reverse=True)
             else:
                 entities.sort(key=lambda c: (c.status.value, c.priority.value),
                               reverse=True)
         table, completed_tasks, completed_story_points = self._print_task(
             table=table,
             entities=entities,
             default_columns=default_columns,
@@ -541,25 +554,28 @@
                     table,
                     entities,
                     default_columns,
                     repo,
                     story_points=None,
                     all_tasks=True,
                     show_window=True,
-                    view_level="tasks"):
+                    view_level="tasks",
+                    custom_sort=None):
         if all_tasks:
             completed_tasks = []
         else:
             completed_tasks = None
             completed_story_points = None
+        if not custom_sort:
+            custom_sort = "status"
         if story_points:
             completed_story_points = []
             entities = [(entity, story_point) for entity, story_point in
                         sorted(zip(entities, story_points),
-                               key=lambda x: x[0].status.value,
+                               key=lambda x: getattr(x[0], custom_sort),
                                reverse=True)]
         else:
             completed_story_points = None
         for column in default_columns:
             table.add_column(column)
         for entity in entities:
             if story_points:
```

### Comparing `terka-1.7.2.2/terka/service_layer/services.py` & `terka-1.8.0/terka/service_layer/services.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/service_layer/ui.py` & `terka-1.8.0/terka/service_layer/ui.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/service_layer/vertical_layout.css` & `terka-1.8.0/terka/service_layer/vertical_layout.css`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/service_layer/views.py` & `terka-1.8.0/terka/service_layer/views.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka/utils.py` & `terka-1.8.0/terka/utils.py`

 * *Files identical despite different names*

### Comparing `terka-1.7.2.2/terka.egg-info/SOURCES.txt` & `terka-1.8.0/terka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

