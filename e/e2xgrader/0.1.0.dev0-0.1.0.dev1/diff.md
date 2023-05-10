# Comparing `tmp/e2xgrader-0.1.0.dev0.tar.gz` & `tmp/e2xgrader-0.1.0.dev1.tar.gz`

## Comparing `e2xgrader-0.1.0.dev0.tar` & `e2xgrader-0.1.0.dev1.tar`

### file list

```diff
@@ -1,217 +1,218 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/.babelrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/.coveragerc
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/lerna.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/nbgrader_config.py
--rw-r--r--   0        0        0   963368 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/package-lock.json
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/package.json
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/sonar-project.properties
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/.github/workflows/black.yml
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/.github/workflows/dispatch.yml
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/.github/workflows/sonar-scan.yml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/__main__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/__version__.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/validator.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/apps/__init__.py
--rw-r--r--   0        0        0    14279 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/apps/api.py
--rw-r--r--   0        0        0    10269 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/apps/e2xgraderapp.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/config/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/converters/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/converters/converter.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/converters/generateexercise.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/__init__.py
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/collect.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/exchange.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/fetch_assignment.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/fetch_feedback.py
--rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/list.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/release_assignment.py
--rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/release_feedback.py
--rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/submit.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exchange/utils.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exporters/__init__.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exporters/exporter.py
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exporters/gradeexporter.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exporters/filters/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/exporters/filters/highlight.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/graders/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/graders/base.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/graders/code.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/graders/multiplechoice.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/graders/singlechoice.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/__init__.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/assignmentmodel.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/basemodel.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/exercisemodel.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presetmodel.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/taskmodel.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/taskpoolmodel.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/templatemodel.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Code (Autograded).ipynb
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Code (Manual).ipynb
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Diagram.ipynb
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Freetext.ipynb
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Multiple Choice.ipynb
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Single Choice.ipynb
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Upload Files.ipynb
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/template/Footer.ipynb
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/template/Group Info.ipynb
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/template/Header.ipynb
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/models/presets/template/Student Info.ipynb
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/clearhiddentests.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/clearsolutions.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/extractattachments.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/filtercellsbyid.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/filtertests.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/overwritecells.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/permutetasks.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/saveautogrades.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/savecells.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/scramble.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/unpermutetasks.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/unscramble.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/validateextracells.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/__init__.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/addtaskheader.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/copyfiles.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/copynotebooks.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/filltemplate.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/generatetaskids.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/makeexercise.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/preprocessor.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/removeexercise.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/assignment_list/__init__.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/assignment_list/handlers.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/__init__.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/grader.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/__init__.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/apihandlers.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/authoring.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/handlers.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/css/editexercise.css
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/css/sidebar.css
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/css/taskcreator.css
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/assignments.js
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/base.js
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/exercises.js
--rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/makeexercise.js
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/taskpools.js
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/tasks.js
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/templates.js
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/assignments.tpl
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/base.tpl
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/editexercise.tpl
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/exercises.tpl
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tablebase.tpl
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskcreator.tpl
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskpools.tpl
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tasks.tpl
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/templates.tpl
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/base/__init__.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/base/base.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/base/handlers/base.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/__init__.py
--rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/apihandlers.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/base.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/e2xgraderapi.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Diagram.ipynb
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Freetext.ipynb
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Single Choice.ipynb
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Upload Files.ipynb
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Footer.ipynb
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Group Info.ipynb
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Header.ipynb
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Student Info.ipynb
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/conf.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/index.html.j2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/form/conf.json
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/form/index.html.j2
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/formgrader.py
--rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/handlers.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/css/eraser-solid.svg
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/css/pencil-solid.svg
--rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade.js
--rw-r--r--   0        0        0    10152 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade_models.js
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_assignments.js
--rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebook_submissions.js
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebooks.js
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_tasks.js
--rw-r--r--   0        0        0    20906 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_assignments.js
--rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_submissions.js
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/base.tpl
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/export_grades.tpl
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/gradebook_base.tpl
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_assignments.tpl
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_students_base.tpl
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_submissions.tpl
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/conf.json
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/formgrade_macros.html.j2
--rw-r--r--   0        0        0    12156 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/index.html.j2
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_assignments.tpl
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_base.tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebooks.tpl
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_tasks.tpl
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/nbgraderapi/__init__.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/nbgraderapi/nbgraderapi.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/validate_assignment/__init__.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/validate_assignment/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/__init__.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/test_validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/apps/__init__.py
--rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/apps/test_e2xgraderapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/converters/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/converters/test_generateexercise.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/exporters/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/exporters/filters/__init__.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/exporters/filters/test_highlight.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/graders/__init__.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/graders/test_base.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/graders/test_code.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/graders/test_multiplechoice.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/graders/test_singlechoice.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/models/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_assignmentmodel.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_basemodel.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_exercisemodel.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_presetmodel.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_taskmodel.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_taskpoolmodel.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_templatemodel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/__init__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_clearhiddentests.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_clearsolutions.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_extractattachments.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_filtercellsbyid.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_filtertests.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_unscramble.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_validateextracells.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/authoring/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/authoring/base.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/authoring/test_copyfiles.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/authoring/test_copynotebooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/test_utils/cells.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/test_utils/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/utils/__init__.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/utils/test_extra_cells.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/utils/test_nbgrader_cells.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/tests/utils/test_notebookvariableextractor.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/utils/__init__.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/utils/extra_cells.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/utils/nbgrader_cells.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/utils/notebookvariableextractor.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/e2xgrader/utils/utils.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/LICENSE
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/README.md
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.babelrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.coveragerc
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/MANIFEST.in
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/lerna.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/nbgrader_config.py
+-rw-r--r--   0        0        0   963368 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/package-lock.json
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/package.json
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/sonar-project.properties
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.github/workflows/dispatch.yml
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.github/workflows/sonar-scan.yml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/__main__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/__version__.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/validator.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/apps/__init__.py
+-rw-r--r--   0        0        0    14279 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/apps/api.py
+-rw-r--r--   0        0        0    10269 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/apps/e2xgraderapp.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/config/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/converters/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/converters/converter.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/converters/generateexercise.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/__init__.py
+-rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/collect.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/exchange.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/fetch_assignment.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/fetch_feedback.py
+-rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/list.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/release_assignment.py
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/release_feedback.py
+-rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/submit.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/utils.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/__init__.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/exporter.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/gradeexporter.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/filters/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/filters/highlight.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/base.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/code.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/multiplechoice.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/singlechoice.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/assignmentmodel.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/basemodel.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/exercisemodel.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presetmodel.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/taskmodel.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/taskpoolmodel.py
+-rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/templatemodel.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Code (Autograded).ipynb
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Code (Manual).ipynb
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Diagram.ipynb
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Freetext.ipynb
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Multiple Choice.ipynb
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Single Choice.ipynb
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Upload Files.ipynb
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Footer.ipynb
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Group Info.ipynb
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Header.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Student Info.ipynb
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/clearhiddentests.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/clearsolutions.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/extractattachments.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/filtercellsbyid.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/filtertests.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/overwritecells.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/permutetasks.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/saveautogrades.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/savecells.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/scramble.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/unpermutetasks.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/unscramble.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/validateextracells.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/__init__.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/addtaskheader.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/copyfiles.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/copynotebooks.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/filltemplate.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/generatetaskids.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/makeexercise.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/preprocessor.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/removeexercise.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/assignment_list/__init__.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/assignment_list/handlers.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/__init__.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/grader.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/__init__.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/apihandlers.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/authoring.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/handlers.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/editexercise.css
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/sidebar.css
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/taskcreator.css
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/assignments.js
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/base.js
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/exercises.js
+-rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/makeexercise.js
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/taskpools.js
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/tasks.js
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/templates.js
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/assignments.tpl
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/base.tpl
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/editexercise.tpl
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/exercises.tpl
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tablebase.tpl
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskcreator.tpl
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskpools.tpl
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tasks.tpl
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/templates.tpl
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/base/__init__.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/base/base.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/base/handlers/base.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/__init__.py
+-rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/apihandlers.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/base.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/e2xgraderapi.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Diagram.ipynb
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Freetext.ipynb
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Single Choice.ipynb
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Upload Files.ipynb
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Footer.ipynb
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Group Info.ipynb
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Header.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Student Info.ipynb
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/conf.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/index.html.j2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/form/conf.json
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/form/index.html.j2
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/__init__.py
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/formgrader.py
+-rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/handlers.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/css/eraser-solid.svg
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/css/pencil-solid.svg
+-rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade.js
+-rw-r--r--   0        0        0    10152 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade_models.js
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_assignments.js
+-rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebook_submissions.js
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebooks.js
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_tasks.js
+-rw-r--r--   0        0        0    20906 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_assignments.js
+-rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_submissions.js
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/base.tpl
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/export_grades.tpl
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/gradebook_base.tpl
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_assignments.tpl
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_students_base.tpl
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_submissions.tpl
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/conf.json
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/formgrade_macros.html.j2
+-rw-r--r--   0        0        0    12156 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/index.html.j2
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_assignments.tpl
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_base.tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebooks.tpl
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_tasks.tpl
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/nbgraderapi/__init__.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/nbgraderapi/nbgraderapi.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/validate_assignment/__init__.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/validate_assignment/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/__init__.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/test_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/apps/__init__.py
+-rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/apps/test_e2xgraderapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/converters/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/converters/test_generateexercise.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/exporters/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/exporters/filters/__init__.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/exporters/filters/test_highlight.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/__init__.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_base.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_code.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_multiplechoice.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_singlechoice.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_assignmentmodel.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_basemodel.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_exercisemodel.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_presetmodel.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_taskmodel.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_taskpoolmodel.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_templatemodel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/__init__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_clearhiddentests.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_clearsolutions.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_extractattachments.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_filtercellsbyid.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_filtertests.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_unscramble.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_validateextracells.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/base.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/test_copyfiles.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/test_copynotebooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/cells.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_extra_cells.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_nbgrader_cells.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_notebookvariableextractor.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/__init__.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/extra_cells.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/nbgrader_cells.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/notebookvariableextractor.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/utils.py
+-rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/LICENSE
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/README.md
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/PKG-INFO
```

### Comparing `e2xgrader-0.1.0.dev0/nbgrader_config.py` & `e2xgrader-0.1.0.dev1/nbgrader_config.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/package-lock.json` & `e2xgrader-0.1.0.dev1/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9165793870887429%*

 * *Differences: {"'dependencies'": "{'@e2xgrader/assignment-view-celltoolbar': {'requires': {'@e2xgrader/cells': "*

 * *                   "'0.1.0-dev1', '@e2xgrader/utils': '0.1.0-dev1'}}, "*

 * *                   "'@e2xgrader/authoring-menubar': {'requires': {'@e2xgrader/api': '0.1.0-dev1', "*

 * *                   "'@e2xgrader/menubar': '0.1.0-dev1', '@e2xgrader/utils': '0.1.0-dev1'}}, "*

 * *                   "'@e2xgrader/cell-extension': {'requires': {'@e2xgrader/cells': '0.1.0-dev1'}}, "*

 * *                   "'@e2xgrader/create-assignm […]*

```diff
@@ -1258,37 +1258,37 @@
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/api"
         },
         "@e2xgrader/assignment-view-celltoolbar": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/cells": "0.1.0-dev0",
-                "@e2xgrader/utils": "0.1.0-dev0",
+                "@e2xgrader/cells": "0.1.0-dev1",
+                "@e2xgrader/utils": "0.1.0-dev1",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/assignment-view-celltoolbar"
         },
         "@e2xgrader/authoring-menubar": {
             "requires": {
-                "@e2xgrader/api": "0.1.0-dev0",
-                "@e2xgrader/menubar": "0.1.0-dev0",
-                "@e2xgrader/utils": "0.1.0-dev0",
+                "@e2xgrader/api": "0.1.0-dev1",
+                "@e2xgrader/menubar": "0.1.0-dev1",
+                "@e2xgrader/utils": "0.1.0-dev1",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/authoring-menubar"
         },
         "@e2xgrader/cell-extension": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/cells": "0.1.0-dev0",
+                "@e2xgrader/cells": "0.1.0-dev1",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/cell-extension"
         },
@@ -1301,26 +1301,26 @@
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/cells"
         },
         "@e2xgrader/create-assignment-celltoolbar": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/cells": "0.1.0-dev0",
-                "@e2xgrader/utils": "0.1.0-dev0",
+                "@e2xgrader/cells": "0.1.0-dev1",
+                "@e2xgrader/utils": "0.1.0-dev1",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/create-assignment-celltoolbar"
         },
         "@e2xgrader/exam-menubar": {
             "requires": {
-                "@e2xgrader/menubar": "0.1.0-dev0",
+                "@e2xgrader/menubar": "0.1.0-dev1",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/exam-menubar"
         },
         "@e2xgrader/menubar": {
             "requires": {
@@ -1328,39 +1328,39 @@
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/menubar"
         },
         "@e2xgrader/notebook-extensions": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/assignment-view-celltoolbar": "0.1.0-dev0",
-                "@e2xgrader/authoring-menubar": "0.1.0-dev0",
-                "@e2xgrader/cell-extension": "0.1.0-dev0",
-                "@e2xgrader/create-assignment-celltoolbar": "0.1.0-dev0",
-                "@e2xgrader/exam-menubar": "0.1.0-dev0",
-                "@e2xgrader/restricted-assignment-notebook": "0.1.0-dev0",
-                "@e2xgrader/restricted-exam-notebook": "0.1.0-dev0",
+                "@e2xgrader/assignment-view-celltoolbar": "0.1.0-dev1",
+                "@e2xgrader/authoring-menubar": "0.1.0-dev1",
+                "@e2xgrader/cell-extension": "0.1.0-dev1",
+                "@e2xgrader/create-assignment-celltoolbar": "0.1.0-dev1",
+                "@e2xgrader/exam-menubar": "0.1.0-dev1",
+                "@e2xgrader/restricted-assignment-notebook": "0.1.0-dev1",
+                "@e2xgrader/restricted-exam-notebook": "0.1.0-dev1",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/notebook-extensions"
         },
         "@e2xgrader/restricted-assignment-notebook": {
             "requires": {
-                "@e2xgrader/utils": "0.1.0-dev0",
+                "@e2xgrader/utils": "0.1.0-dev1",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/restricted-assignment-notebook"
         },
         "@e2xgrader/restricted-exam-notebook": {
             "requires": {
-                "@e2xgrader/utils": "0.1.0-dev0",
+                "@e2xgrader/utils": "0.1.0-dev1",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/restricted-exam-notebook"
         },
         "@e2xgrader/tree-extensions": {
             "requires": {
@@ -10775,15 +10775,15 @@
                 "babel-preset-env": "^1.7.0",
                 "lerna": "^5.3.0",
                 "prettier": "^2.7.1"
             },
             "hasInstallScript": true,
             "license": "MIT",
             "name": "e2xgrader",
-            "version": "0.1.0-dev0",
+            "version": "0.1.0-dev1",
             "workspaces": [
                 "packages/*"
             ]
         },
         "node_modules/@ampproject/remapping": {
             "dependencies": {
                 "@jridgewell/gen-mapping": "^0.1.0",
@@ -24444,31 +24444,31 @@
         "packages/api": {
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/api",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/assignment-view-celltoolbar": {
             "dependencies": {
-                "@e2xgrader/cells": "0.1.0-dev0",
-                "@e2xgrader/utils": "0.1.0-dev0"
+                "@e2xgrader/cells": "0.1.0-dev1",
+                "@e2xgrader/utils": "0.1.0-dev1"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/assignment-view-celltoolbar",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/authoring": {
             "dependencies": {
                 "@e2xgrader/api": "*",
                 "@emotion/react": "^11.9.3",
                 "@emotion/styled": "^11.9.3",
                 "@fontsource/roboto": "^4.5.7",
@@ -24485,68 +24485,68 @@
             },
             "extraneous": true,
             "name": "@e2xgrader/authoring",
             "version": "0.1.0"
         },
         "packages/authoring-menubar": {
             "dependencies": {
-                "@e2xgrader/api": "0.1.0-dev0",
-                "@e2xgrader/menubar": "0.1.0-dev0",
-                "@e2xgrader/utils": "0.1.0-dev0"
+                "@e2xgrader/api": "0.1.0-dev1",
+                "@e2xgrader/menubar": "0.1.0-dev1",
+                "@e2xgrader/utils": "0.1.0-dev1"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/authoring-menubar",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/cell-extension": {
             "dependencies": {
-                "@e2xgrader/cells": "0.1.0-dev0"
+                "@e2xgrader/cells": "0.1.0-dev1"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/cell-extension",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/cells": {
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/cells",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/create-assignment-celltoolbar": {
             "dependencies": {
-                "@e2xgrader/cells": "0.1.0-dev0",
-                "@e2xgrader/utils": "0.1.0-dev0"
+                "@e2xgrader/cells": "0.1.0-dev1",
+                "@e2xgrader/utils": "0.1.0-dev1"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/create-assignment-celltoolbar",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/create-assignment-extension": {
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "@e2xgrader/cells": "*",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
@@ -24556,32 +24556,32 @@
             "extraneous": true,
             "license": "ISC",
             "name": "@e2xgrader/create-assignment-extension",
             "version": "0.1.0.dev0"
         },
         "packages/exam-menubar": {
             "dependencies": {
-                "@e2xgrader/menubar": "0.1.0-dev0"
+                "@e2xgrader/menubar": "0.1.0-dev1"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/exam-menubar",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/menubar": {
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/menubar",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/nbextensions": {
             "devDependencies": {
                 "babel-cli": "^6.26.0",
                 "babel-core": "^6.26.3",
                 "babel-plugin-transform-class-properties": "^6.24.1",
                 "babel-preset-env": "^1.7.0"
@@ -24599,75 +24599,75 @@
             "extraneous": true,
             "license": "MIT",
             "name": "@e2xgrader/nbgrader-utils",
             "version": "0.1.0.dev0"
         },
         "packages/notebook-extensions": {
             "dependencies": {
-                "@e2xgrader/assignment-view-celltoolbar": "0.1.0-dev0",
-                "@e2xgrader/authoring-menubar": "0.1.0-dev0",
-                "@e2xgrader/cell-extension": "0.1.0-dev0",
-                "@e2xgrader/create-assignment-celltoolbar": "0.1.0-dev0",
-                "@e2xgrader/exam-menubar": "0.1.0-dev0",
-                "@e2xgrader/restricted-assignment-notebook": "0.1.0-dev0",
-                "@e2xgrader/restricted-exam-notebook": "0.1.0-dev0"
+                "@e2xgrader/assignment-view-celltoolbar": "0.1.0-dev1",
+                "@e2xgrader/authoring-menubar": "0.1.0-dev1",
+                "@e2xgrader/cell-extension": "0.1.0-dev1",
+                "@e2xgrader/create-assignment-celltoolbar": "0.1.0-dev1",
+                "@e2xgrader/exam-menubar": "0.1.0-dev1",
+                "@e2xgrader/restricted-assignment-notebook": "0.1.0-dev1",
+                "@e2xgrader/restricted-exam-notebook": "0.1.0-dev1"
             },
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/notebook-extensions",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/restricted-assignment-notebook": {
             "dependencies": {
-                "@e2xgrader/utils": "0.1.0-dev0"
+                "@e2xgrader/utils": "0.1.0-dev1"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/restricted-assignment-notebook",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/restricted-exam-notebook": {
             "dependencies": {
-                "@e2xgrader/utils": "0.1.0-dev0"
+                "@e2xgrader/utils": "0.1.0-dev1"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/restricted-exam-notebook",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/tree-extensions": {
             "devDependencies": {
                 "@babel/preset-env": "^7.16.11",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "ISC",
             "name": "@e2xgrader/tree-extensions",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         },
         "packages/utils": {
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/utils",
-            "version": "0.1.0-dev0"
+            "version": "0.1.0-dev1"
         }
     },
     "requires": true,
-    "version": "0.1.0-dev0"
+    "version": "0.1.0-dev1"
 }
```

### Comparing `e2xgrader-0.1.0.dev0/package.json` & `e2xgrader-0.1.0.dev1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.0-dev1'"}*

```diff
@@ -30,12 +30,12 @@
     },
     "scripts": {
         "build": "lerna run build",
         "install": "lerna run bootstrap",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:files": "prettier --write"
     },
-    "version": "0.1.0-dev0",
+    "version": "0.1.0-dev1",
     "workspaces": [
         "packages/*"
     ]
 }
```

### Comparing `e2xgrader-0.1.0.dev0/.github/workflows/dispatch.yml` & `e2xgrader-0.1.0.dev1/.github/workflows/dispatch.yml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/.github/workflows/python-package.yml` & `e2xgrader-0.1.0.dev1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/.github/workflows/sonar-scan.yml` & `e2xgrader-0.1.0.dev1/.github/workflows/sonar-scan.yml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/__init__.py` & `e2xgrader-0.1.0.dev1/e2xgrader/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/validator.py` & `e2xgrader-0.1.0.dev1/e2xgrader/validator.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/apps/api.py` & `e2xgrader-0.1.0.dev1/e2xgrader/apps/api.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/apps/e2xgraderapp.py` & `e2xgrader-0.1.0.dev1/e2xgrader/apps/e2xgraderapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/config/__init__.py` & `e2xgrader-0.1.0.dev1/e2xgrader/config/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/converters/converter.py` & `e2xgrader-0.1.0.dev1/e2xgrader/converters/converter.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/converters/generateexercise.py` & `e2xgrader-0.1.0.dev1/e2xgrader/converters/generateexercise.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/__init__.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/collect.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/collect.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/exchange.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/exchange.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/fetch_assignment.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/fetch_assignment.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/fetch_feedback.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/fetch_feedback.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/list.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/list.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/release_assignment.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/release_assignment.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/release_feedback.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/release_feedback.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/submit.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/submit.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exchange/utils.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exchange/utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exporters/exporter.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exporters/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,24 @@
         ]
         # The notebook seems to sometimes set exclude_input to true
         self.exclude_input = False
 
     @property
     def template_paths(self):
         return super()._template_paths() + [
-            os.path.join(
-                os.path.dirname(__file__),
-                "..",
-                "server_extensions",
-                "formgrader",
-                "templates",
+            os.path.abspath(
+                os.path.join(
+                    os.path.dirname(__file__),
+                    "..",
+                    "server_extensions",
+                    "grader",
+                    "apps",
+                    "formgrader",
+                    "templates",
+                )
             )
         ]
 
     @pass_context
     def to_choicecell(self, context, source):
         cell = context.get("cell", {})
         soup = BeautifulSoup(source, "html.parser")
```

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exporters/gradeexporter.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exporters/gradeexporter.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/exporters/filters/highlight.py` & `e2xgrader-0.1.0.dev1/e2xgrader/exporters/filters/highlight.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/graders/base.py` & `e2xgrader-0.1.0.dev1/e2xgrader/graders/base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/graders/code.py` & `e2xgrader-0.1.0.dev1/e2xgrader/graders/code.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/graders/multiplechoice.py` & `e2xgrader-0.1.0.dev1/e2xgrader/graders/multiplechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/graders/singlechoice.py` & `e2xgrader-0.1.0.dev1/e2xgrader/graders/singlechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/assignmentmodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/models/assignmentmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/basemodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/exercisemodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/models/exercisemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presetmodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presetmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/taskmodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/models/taskmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/taskpoolmodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/models/taskpoolmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/templatemodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/models/templatemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Code (Autograded).ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Code (Autograded).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Code (Manual).ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Code (Manual).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Diagram.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Diagram.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Freetext.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Freetext.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Multiple Choice.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Multiple Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Single Choice.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Single Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/questions/Upload Files.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Upload Files.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/template/Footer.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Footer.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/template/Group Info.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Group Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/template/Header.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Header.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/models/presets/template/Student Info.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Student Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/__init__.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/clearhiddentests.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/clearhiddentests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/clearsolutions.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/clearsolutions.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/extractattachments.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/extractattachments.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/filtercellsbyid.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/filtercellsbyid.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/filtertests.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/filtertests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/overwritecells.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/overwritecells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/permutetasks.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/permutetasks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/saveautogrades.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/saveautogrades.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/savecells.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/savecells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/scramble.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/scramble.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/unpermutetasks.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/unpermutetasks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/unscramble.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/unscramble.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/validateextracells.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/validateextracells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/addtaskheader.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/addtaskheader.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/copyfiles.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/copyfiles.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/copynotebooks.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/copynotebooks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/filltemplate.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/filltemplate.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/generatetaskids.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/generatetaskids.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/makeexercise.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/makeexercise.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/preprocessors/authoring/removeexercise.py` & `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/removeexercise.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/assignment_list/handlers.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/assignment_list/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/grader.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/grader.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/apihandlers.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/apihandlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/authoring.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/authoring.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/handlers.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/css/editexercise.css` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/editexercise.css`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/css/sidebar.css` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/sidebar.css`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/css/taskcreator.css` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/taskcreator.css`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/assignments.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/assignments.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/base.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/base.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/exercises.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/exercises.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/makeexercise.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/makeexercise.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/taskpools.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/taskpools.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/tasks.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/tasks.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/static/js/templates.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/templates.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/assignments.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/assignments.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/base.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/base.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/editexercise.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/editexercise.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/exercises.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/exercises.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tablebase.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tablebase.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskcreator.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskcreator.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskpools.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskpools.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tasks.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tasks.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/templates.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/templates.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/base/base.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/base/base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/apihandlers.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/apihandlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/e2xgraderapi.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/e2xgraderapi.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Diagram.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Diagram.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Freetext.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Freetext.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Single Choice.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Single Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Upload Files.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Upload Files.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Footer.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Footer.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Group Info.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Group Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Header.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Header.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Student Info.ipynb` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Student Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/index.html.j2` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/index.html.j2`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/formgrader.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/formgrader.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/handlers.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/css/eraser-solid.svg` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/css/eraser-solid.svg`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/css/pencil-solid.svg` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/css/pencil-solid.svg`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade_models.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade_models.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_assignments.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_assignments.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebook_submissions.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebook_submissions.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebooks.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebooks.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_tasks.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_tasks.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_assignments.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_assignments.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_submissions.js` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_submissions.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/base.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/base.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/export_grades.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/export_grades.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_assignments.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_assignments.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_submissions.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_submissions.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/formgrade_macros.html.j2` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/formgrade_macros.html.j2`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/index.html.j2` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/index.html.j2`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_assignments.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_assignments.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebooks.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebooks.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_tasks.tpl` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_tasks.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/grader/apps/nbgraderapi/nbgraderapi.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/nbgraderapi/nbgraderapi.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/server_extensions/validate_assignment/handlers.py` & `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/validate_assignment/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/test_validator.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/apps/test_e2xgraderapp.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/apps/test_e2xgraderapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/converters/test_generateexercise.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/converters/test_generateexercise.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/exporters/filters/test_highlight.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/exporters/filters/test_highlight.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/graders/test_base.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/graders/test_code.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_code.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/graders/test_multiplechoice.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_multiplechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/graders/test_singlechoice.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_singlechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_assignmentmodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_assignmentmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_basemodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_basemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_exercisemodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_exercisemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_presetmodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_presetmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_taskmodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_taskmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_taskpoolmodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_taskpoolmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/models/test_templatemodel.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_templatemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_clearhiddentests.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_clearhiddentests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_clearsolutions.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_clearsolutions.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_extractattachments.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_extractattachments.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_filtercellsbyid.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_filtercellsbyid.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_filtertests.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_filtertests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_unscramble.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_unscramble.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/test_validateextracells.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_validateextracells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/authoring/base.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/authoring/test_copyfiles.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/test_copyfiles.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/preprocessors/authoring/test_copynotebooks.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/test_copynotebooks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/test_utils/cells.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/test_utils/test_utils.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/utils/test_extra_cells.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_extra_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/utils/test_nbgrader_cells.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_nbgrader_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/tests/utils/test_notebookvariableextractor.py` & `e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_notebookvariableextractor.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/utils/extra_cells.py` & `e2xgrader-0.1.0.dev1/e2xgrader/utils/extra_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/e2xgrader/utils/nbgrader_cells.py` & `e2xgrader-0.1.0.dev1/e2xgrader/utils/nbgrader_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/.gitignore` & `e2xgrader-0.1.0.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/LICENSE` & `e2xgrader-0.1.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/README.md` & `e2xgrader-0.1.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev0/pyproject.toml` & `e2xgrader-0.1.0.dev1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -17,14 +17,19 @@
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
     "nbgrader==0.7.1",
+    "jupyter-core<4.11.2",
+    "jupyter-client<7.4",
+    "jupyter-server<1.20",
+    "nbconvert>=6.5",
+    "notebook>=6,<6.5",
     "beautifulsoup4",
     "pandas"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://e2x.inf.h-brs.de"
@@ -57,15 +62,15 @@
 ]
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.1.0-dev0"
+current = "0.1.0-dev1"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `e2xgrader-0.1.0.dev0/PKG-INFO` & `e2xgrader-0.1.0.dev1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2xgrader
-Version: 0.1.0.dev0
+Version: 0.1.0.dev1
 Summary: An addon for nbgrader
 Project-URL: Documentation, https://e2x.inf.h-brs.de
 Project-URL: Issues, https://github.com/Digiklausur/e2xgrader/issues
 Project-URL: Source, https://github.com/Digiklausur/e2xgrader
 Author-email: Tim Metzler <tim.metzler@h-brs.de>
 License-Expression: MIT
 License-File: LICENSE
@@ -12,15 +12,20 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
 Requires-Dist: beautifulsoup4
+Requires-Dist: jupyter-client<7.4
+Requires-Dist: jupyter-core<4.11.2
+Requires-Dist: jupyter-server<1.20
+Requires-Dist: nbconvert>=6.5
 Requires-Dist: nbgrader==0.7.1
+Requires-Dist: notebook<6.5,>=6
 Requires-Dist: pandas
 Provides-Extra: dev
 Requires-Dist: hatchling; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: tbump; extra == 'dev'
 Description-Content-Type: text/markdown
```

