# Comparing `tmp/e2xgrader-0.1.0.dev1.tar.gz` & `tmp/e2xgrader-0.1.0.dev3.tar.gz`

## Comparing `e2xgrader-0.1.0.dev1.tar` & `e2xgrader-0.1.0.dev3.tar`

### file list

```diff
@@ -1,218 +1,922 @@
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.babelrc
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.coveragerc
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/MANIFEST.in
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/lerna.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/nbgrader_config.py
--rw-r--r--   0        0        0   963368 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/package-lock.json
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/package.json
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/sonar-project.properties
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.github/workflows/black.yml
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.github/workflows/dispatch.yml
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.github/workflows/sonar-scan.yml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/__init__.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/__main__.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/__version__.py
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/validator.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/apps/__init__.py
--rw-r--r--   0        0        0    14279 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/apps/api.py
--rw-r--r--   0        0        0    10269 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/apps/e2xgraderapp.py
--rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/config/__init__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/converters/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/converters/converter.py
--rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/converters/generateexercise.py
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/__init__.py
--rw-r--r--   0        0        0     4371 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/collect.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/exchange.py
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/fetch_assignment.py
--rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/fetch_feedback.py
--rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/list.py
--rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/release_assignment.py
--rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/release_feedback.py
--rw-r--r--   0        0        0     7997 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/submit.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exchange/utils.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/__init__.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/exporter.py
--rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/gradeexporter.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/filters/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/exporters/filters/highlight.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/base.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/code.py
--rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/multiplechoice.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/graders/singlechoice.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/__init__.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/assignmentmodel.py
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/basemodel.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/exercisemodel.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presetmodel.py
--rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/taskmodel.py
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/taskpoolmodel.py
--rw-r--r--   0        0        0     2380 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/templatemodel.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Code (Autograded).ipynb
--rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Code (Manual).ipynb
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Diagram.ipynb
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Freetext.ipynb
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Multiple Choice.ipynb
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Single Choice.ipynb
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Upload Files.ipynb
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Footer.ipynb
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Group Info.ipynb
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Header.ipynb
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Student Info.ipynb
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/clearhiddentests.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/clearsolutions.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/extractattachments.py
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/filtercellsbyid.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/filtertests.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/overwritecells.py
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/permutetasks.py
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/saveautogrades.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/savecells.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/scramble.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/unpermutetasks.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/unscramble.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/validateextracells.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/__init__.py
--rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/addtaskheader.py
--rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/copyfiles.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/copynotebooks.py
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/filltemplate.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/generatetaskids.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/makeexercise.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/preprocessor.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/removeexercise.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/assignment_list/__init__.py
--rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/assignment_list/handlers.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/__init__.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/grader.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/__init__.py
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/apihandlers.py
--rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/authoring.py
--rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/handlers.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/editexercise.css
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/sidebar.css
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/taskcreator.css
--rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/assignments.js
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/base.js
--rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/exercises.js
--rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/makeexercise.js
--rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/taskpools.js
--rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/tasks.js
--rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/templates.js
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/assignments.tpl
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/base.tpl
--rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/editexercise.tpl
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/exercises.tpl
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tablebase.tpl
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskcreator.tpl
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskpools.tpl
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tasks.tpl
--rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/templates.tpl
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/base/__init__.py
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/base/base.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/base/handlers/base.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/__init__.py
--rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/apihandlers.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/base.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/e2xgraderapi.py
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb
--rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Diagram.ipynb
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Freetext.ipynb
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb
--rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Single Choice.ipynb
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Upload Files.ipynb
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Footer.ipynb
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Group Info.ipynb
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Header.ipynb
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Student Info.ipynb
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/conf.json
--rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/index.html.j2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/form/conf.json
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/form/index.html.j2
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/__init__.py
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/formgrader.py
--rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/handlers.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/css/eraser-solid.svg
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/css/pencil-solid.svg
--rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade.js
--rw-r--r--   0        0        0    10152 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade_models.js
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_assignments.js
--rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebook_submissions.js
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebooks.js
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_tasks.js
--rw-r--r--   0        0        0    20906 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_assignments.js
--rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_submissions.js
--rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/base.tpl
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/export_grades.tpl
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/gradebook_base.tpl
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_assignments.tpl
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_students_base.tpl
--rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_submissions.tpl
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/conf.json
--rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/formgrade_macros.html.j2
--rw-r--r--   0        0        0    12156 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/index.html.j2
--rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_assignments.tpl
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_base.tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebooks.tpl
--rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_tasks.tpl
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/nbgraderapi/__init__.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/nbgraderapi/nbgraderapi.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/validate_assignment/__init__.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/validate_assignment/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/__init__.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/test_validator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/apps/__init__.py
--rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/apps/test_e2xgraderapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/converters/__init__.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/converters/test_generateexercise.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/exporters/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/exporters/filters/__init__.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/exporters/filters/test_highlight.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/__init__.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_base.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_code.py
--rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_multiplechoice.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_singlechoice.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/__init__.py
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_assignmentmodel.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_basemodel.py
--rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_exercisemodel.py
--rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_presetmodel.py
--rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_taskmodel.py
--rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_taskpoolmodel.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_templatemodel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/__init__.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_clearhiddentests.py
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_clearsolutions.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_extractattachments.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_filtercellsbyid.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_filtertests.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_unscramble.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_validateextracells.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/__init__.py
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/base.py
--rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/test_copyfiles.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/test_copynotebooks.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/__init__.py
--rw-r--r--   0        0        0     4763 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/cells.py
--rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/test_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/__init__.py
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_extra_cells.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_nbgrader_cells.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_notebookvariableextractor.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/__init__.py
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/extra_cells.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/nbgrader_cells.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/notebookvariableextractor.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/e2xgrader/utils/utils.py
--rw-r--r--   0        0        0     1868 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/LICENSE
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/README.md
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.babelrc
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.coveragerc
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/MANIFEST.in
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/lerna.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/nbgrader_config.py
+-rw-r--r--   0        0        0   963368 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/package-lock.json
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/package.json
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/sonar-project.properties
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.github/workflows/black.yml
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.github/workflows/dispatch.yml
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.github/workflows/sonar-scan.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/10189820f507efcd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/102c20c52f1cb525
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/102e6bb50427d78
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1065f009249af252
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1077da38f8c57b72
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/10b750d20640013a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/113a48c022ec5030
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/114bbb64835f4b70
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/128f1a4f7e087586
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/12a2a19e98cc9fe6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/12ccbe17941900ba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/133a852e26cf0ebb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/14350f46ca1ad89
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1480c978da9073a7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/14dc026a990149b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/152fc0df28506da5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/15324070ed698641
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/154e58a22b762b75
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/156496192664727d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1583ed31086d9f20
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/15a04759fcd2ed8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/15a623a385458d1a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/15b2d00ed82ba863
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/15f3765c6f5ba34b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/15fb17d3facb10de
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/15fc7c75c87840bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/15ff6e6d5dfef43e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/160bb605ed260fe9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1636e447207755f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1656fc8de05c03f5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1690a84ae371016
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/16cab5c97b56f7a6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/16eee94bd97abb4f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1717e447aaa00063
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1756fb78655f519b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/181f09a6c41f519b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/18550c68d47e4ca1
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/185afd71b38b6cff
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1865bee440ddb3d6
+-rw-r--r--   0        0        0     4727 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/186f0a045689bb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/18e0ce244579a6a1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/18e4c8e60d5db36a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1909cbb79106dc9d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1962ed8d0f88ddc4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1994aa386f208836
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/19c47811a5cd00cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1a5847221ad99ad4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1a6f6e30946cdbf0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1a7cb0e13494a9e1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1aa29cc9186a4a53
+-rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1aeda3afdb87b780
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1af6a1bfbca0deaf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1bef90e05ca1e2ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1c069627357690f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1c0c5f1394a13f8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1c217bd59144583
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1c2848d5ce1eaa19
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1c58c1804220cba1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1cb521fd3cd18b0d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1cc5a114bad36c3c
+-rw-r--r--   0        0        0     2751 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1cd75c936e692819
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1dd9dff4e54f458b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1e350a33061a2b8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1ebff1aa17525744
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1f9bd62185c6d7f0
+-rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/1fd32bb5ea765a4c
+-rw-r--r--   0        0        0    11648 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2028c717ae2bf8a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2064d845c8e10e27
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/20afa49c476aa29e
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/20b193e0fe1d8452
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2116cc5e8e89083d
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/21396c190684e0c5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/218f12d01f67bc1b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/21bbee69d059e7e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/21dddb1259dda4fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/223a6aa8a15cdec6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/22d15b4806b62e9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/22e2524af4a2209f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/23de1f2895418ba1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/23fb5ee8aa4777ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2421407e8a76fab3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2441b83b74708d43
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2455e0e5b5d51912
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2473a606f0f5c9dc
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/249a2dfcc2c75ef0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/24b13740f6003c87
+-rw-r--r--   0        0        0     3434 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/24b323e9b8faff3f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/24c464ed72b0f3c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/24dc3e59282b9cb1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2595fdc764486b05
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/260e25f46662682c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/271c3123db5e832
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/27369510428cfe1b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/27560111c8764ab8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/27b52e8a1d0575eb
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/289f954eb2e23b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/28a2833271296305
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/28b6e5df6de26ff7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2965401419659c77
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/296c4718ef1f662b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/298bbc350b47247b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/29cd126ea08316df
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2a2949e4fb834aa1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2a52ff06947c834d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2a869c5371e3d770
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2aa05605e9923d46
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2b499dbc619bb4a1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2b766d3d4ae5212e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2bc68e44c54f6f64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2c1917fbf13f7021
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2c4eb7f0e166a946
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2c9d8862d6b21ba2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2d85e1a53a3327ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2e17df35b5d6aa14
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2eb8a35b9a5c0905
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2ecfab1fecf59035
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2f6b57f6d54767c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/2fea53e78ed38dc2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3059081333ff8151
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/30c2ac455b72432e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/31249af7676b1902
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/318ad9b4726a3b83
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/318c860a0680c279
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/31d3609925950f26
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/32bc24f47ec9d0e3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/32d8506f2dbd55a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/32d894c1171b4b7f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/32dbb1b5155825a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/334dd416cb02b07b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3384513817945f16
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/33aab6e3777ddda6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/33b521d789b75e7f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/34666d753ff1ee02
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/34f0212184fdd78a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/35128f17bf49a14d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/353c2dfc71b4e4f3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3557a1f4396ef90b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/35c7d826a67d8742
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/371309cef814902c
+-rw-r--r--   0        0        0    10634 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/37529992348975cd
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/37a444a038078f16
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/37dcdc57ddcecd12
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3916881183f75016
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/394b6f52819e67c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/39a7de12ad211332
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/39d53720d0f25256
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/39d8e7e92d898e45
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/39e25c57618e53f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3ae91a59f71025af
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3b0a0c8f00aa500c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3ba922edaf0fdb0a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3c6cdc97895f40fd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3c8faa4c5b95a243
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3c9727ac64cc7275
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3cd545db20c6dc3e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3d25c08deb253095
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3dd3031675d11f31
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3deffb3155f0e39a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3e4366c9021217e7
+-rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3ee91de4595bdbc5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3f106eaa811cee19
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3f220e7122ff98fc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3fcf92698d8a2d19
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/3ffcb928659b2b22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/407ad25092879cd7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/40847f64e2fa6ee5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/40cd110f7358b4eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/40f7b6320abdfe9c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/41705d8ec7333628
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4180a8cb6a3b99e7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/42165a8b93d41272
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/42492922bb829a1a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/424f91ecd101dba0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/42f759e83f12025b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4323e53578eb7722
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/433687cfc200c81
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/43ab47f8c80ae171
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/440431b7aab528b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4442674f8c5fe537
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/446f05313b1ea741
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/452ed6a9eb6e0f1d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/45df7f11dcf882d1
+-rw-r--r--   0        0        0    11485 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/47a4734d951752ab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/47ce1852d55bec50
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/480718d4442534ce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/483969fb7b0d6b1a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/483d6b79ac3ee2e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/484223f111a2de8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/48c0072f734335b2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/49177a89abfec4c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/493c44b41f478caf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4994db3208c9c0c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/49c8baf5b93f4d46
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/49de3a99c7420a35
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4a00cde96d13dce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4a768cf9fdbff454
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4a8bc3e5e94b40b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4a8d4db7235f3def
+-rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4aa5c6b48bb6616
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4aa8ecabdb588a37
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4c395fceeba86094
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4cdc4f600a3d9dfa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4ce02746975a023b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4d7486340881e21f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4df653955aa1d4da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4e438ec6ebebc20f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4e56b47c739fd3e1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4eb3cf507ba49f0d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4ee331b0d5296dea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4eeea0e50c4cb77c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/4f4cd2b0e1f2342
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/506c7933115dee3e
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5186f5492ea1f185
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5228be0983cb1703
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5327f6763cdfb9c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5336df4598dd29ac
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/534c27f3861c62f7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/53601acd78d2fbbd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5377ad827bf0aeb0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/537d7d3531590333
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/53adb3ba06c96e3c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/53c7d12bab385542
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/53e6c224c8e82451
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/540f4080927fbed0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/54b670f4fbfc6275
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/54bc0b30334a800
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/54fcd64ea63cf291
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/55b9351e02b02a95
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/55d4cf2eaa6b0c81
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/55ea2c2be4c92ac0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/560343b77f9cdc03
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/562071ec01340d8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/56e0767943aaa633
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/56f0bb4b14bc2cb4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/57b45f6b364d8754
+-rw-r--r--   0        0        0    11648 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/580d1a1ecaf291e3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/58dcd5f03524bfaa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/58ea313b4f9fc3f4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5930fd28137b312d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/59ee46e690250ae7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5a2dd17a88b801c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5ad77ac5ba1cfe47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5adac9355d0490ca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5b91ad5990e312e5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5be50a85de3c8eec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5c3b7bf93c429c3e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5cc887df65b80aeb
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5cd61732da6a40
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5cf05593c684d66b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5d12579df093af54
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5d1af70d4cb71e91
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5def3f67e69f7d8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5ed8cd38cca3e883
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5ee29970d9473c8f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/5fd39e0554330e9e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6038af04c879dd38
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6057224ac6f6155b
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/60f28eabf2401102
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6189d075e4e5e981
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/619dc269a209d26e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/61a441da8de8c895
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6207ce63a5f50efc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/62bed965d645099c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/63fb6d02ac7dd1b7
+-rw-r--r--   0        0        0    14795 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/643b86796cef8d77
+-rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/64a6eda6c5a7913a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/64e2a827a6513c8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/652cec7ae0d7540a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/65509905931b8220
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6584e310c8084e31
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/663369c5cde9e103
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/664b63c5e9c787f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6690cb5e2b4c9dd2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/66a238e8e47d4ad7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/66a4eb7eccd0f18b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/67040e654e980754
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6741801dd0816d22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/675b22b63c4b0a4d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6907a3df74629039
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/69219e67e15347c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/69419352f0f5cf49
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/69d8067684d822c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6a19dd471741375c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6a7e594ad4f85642
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6b9d6d1928eda6b2
+-rw-r--r--   0        0        0     4650 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6cdb068dd36c4151
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6d0f4e1099a3c749
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6d8b202522318bde
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6d9e5afb755c5fb9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6dd9aec3d64de007
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6e7d19db1f59194f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6efa65701c680c1b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/6f14daca434474e2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/70f001da187b555e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/716e44874789644c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/71e1dcff5d5e9545
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/720b5bdaae7429bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7232ab1259005199
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/72e69a1efa58c220
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/73f02627e48a6f2e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/73f840ac3e6ac312
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7405d3cbb9a1d5b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/744cfa52f358e004
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/745658ad901bfa8c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7493bcaafb6af964
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/74adc470ed83ddec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/74b03dd73731b429
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/758b8eff4fcf53b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/758e0520da1ce63f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/75e3b0d719945f79
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7611ab55e22653ef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/765a903c201db16
+-rw-r--r--   0        0        0    11485 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/76cf7c3f3e90745f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/779b69f0af3cfd0d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/77ecb3eaaff97f3b
+-rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/77fd15fd88c22e2d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7848ca411d2aec5a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/784e7954c404d908
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/79716fc99d5c651c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7a4cb25550d4afe4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7b36aad20d650fc8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7cf4bcbc7ea040be
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7d5d2256679835da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7d709c22122e8053
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7d7828a33ac165a9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7dba926ec01c5ea
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7dccab1b70b49836
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7e7db1badcc22ce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7ee1bf989678641c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7eea2e6a38ff06f4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7f29342765ca516c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7fe735dacf300a21
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/7fe86087dbc0e921
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/806362334baafa94
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8129d89f29213418
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/81605d1470f217b6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8221c133cc64144a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/825c076a707f66df
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/82857f0b11a3e5f8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/828a093ff1220e3e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/829bd44559e37bfa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8370f671190f4310
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/84111e95ee013fda
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/844406a15a739311
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8468512f52ff62a0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/84efaae12c3c7036
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/850aba43df3793cb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8594bcbab30a2be3
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/85dbaa9ecca1f258
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/86b561f88488510d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/86e927bd57a6acef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/86f705f12cf3e008
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/86f87160010b2ba8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/875493594d1a0f84
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/87923ddbaebb9f54
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/87d005c12e61e9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/87e7358119938ab7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/881954d5434743a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8855bf4d03ff5947
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8883f1949f0c9142
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/88cc122852ea7cc4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/891276d34bb326bb
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/893103ca79fd49b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8936ab194431fe2e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/894d2235f6c92d0f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/896e9be1abec994d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/89a487ea63531cab
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/89a9d77ace49ab9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/89f466ad86f44a55
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8b1d167c9601c120
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8b71737c07862b6c
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8b7f5eea64fc5ff5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8ba89fb7298a8894
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8cdf6cdcf1dfcc57
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8ce64c85946410ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8e276c90a80c63b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8e4dcd3bc78d7528
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8e9612f4e2bea400
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8ea5c4b794fe9f96
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8ebbb8e227a59085
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8f46fa27d2126d72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8f78ceb41d04e44c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/8f8d347e5edb4d1e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/90271c0a5b7a1bb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/91044508c76c1695
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9105b4ae5f73bd87
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/910fda6fb78e53e3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/917db35966018197
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/919926793036d316
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/92f86ad9f7595a8b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/93332b37167f951
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/939c6189173691f1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/939fa46ee2bcf1b5
+-rw-r--r--   0        0        0    11340 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/94138038ccd960d8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9455795c1f701eb8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/946c06c4b3421e62
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/94b5651c3a21da3d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/95cdc9e0d1474cc3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/97d4c809bb6d1267
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/97dc718e51edcced
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/98f1fae0e6a9cab1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9917fa37d03c8ee9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/993ff555994e636f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9965268dd5c0f052
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9988a84ab0b92078
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/999c743b910fcfca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/99dce4fe6b28409a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9d6e862a2514e38e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9d8c2a530c323e5d
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9dff64279ab7795f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9e105e8422557918
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9e279b9aa1a0516f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9ea528bd00fd435b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9f08fc9faddf802e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/9fb4ab608675f603
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a0431e5eabcc5e49
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a155cfc1692b81bb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a211d62db8f7022c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a266042a34d85fb7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a2a3be5d46095a4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a39238d0e3640725
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a43d1666649e72d5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a5453bf72885dd76
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a5cb65f537def1ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a604435c6fcca94
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a6234b4d46afbc14
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a6999895461fdd82
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a6a4d4d9e8f47a64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a6bbe21292b163ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a6eb8824710ef44f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a7119e7a29b8fa18
+-rw-r--r--   0        0        0    11423 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a7339c2b03855e0a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a795c7e3515cd1e2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a7a184455eedcbb2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a7abe5bca42633f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a7c19a15e4d7177f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a7e08fd1664914c7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a7e545fae6a6de52
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a825007e8a45af6c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a874ed6403551abd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a8ff1361c7578559
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a921254b891dac32
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a948b7909a7b17d3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a96eb6e664dd25dd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/a9eca93ed0cc08c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/aa50d6cc8ff0cb8e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/aaafd7d0be281907
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/aaefaf3d8da82590
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/abc7546334d479ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ad2301e5e8b4f638
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ad5b2ccbcfa82eda
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ad651d5952be0e8a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ad7ef4e1581a1158
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ae9dc26c386c4d24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/aed0b5dd907b1579
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/aeec3e272410edaa
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/af6d1172911b4e89
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/af91a1ee92ff1e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/afbd3bc2ec687eca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/afca6bbfb1e5b22f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b09709579bb369c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b168e444fcfa7d60
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b1e11c11d897bd51
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b31b46edddd76b45
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b340b048ee5104f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b3bec56e6d86d5ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b3c70e10b702d02
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b418865b457f5761
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b433c239464ba9dd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b464d0dd809b390f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b4e201c5b721e017
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b535c0faa061915
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b574b4c9f151564b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b5a65deaecc3409e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b5cb16a05da8040f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b61df7e684d872ef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b62af761ada44025
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b70b45a1f5b48951
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b778b438779f7d34
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b794a067810f128
+-rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b800c030271d71e2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b811025b247f7236
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b85f74493bc60c46
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b8fb7f0112bd2f77
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b9565565927b73bb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b9873d0ccc3a1e36
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b99ec5ac62bd72b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b9b3f06c61e8f061
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b9d9dfe2f4f3f34
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/b9f28b72a619c5c6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ba075ad9c533bc38
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ba877be0bc5862bc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ba8dd3286146b2c8
+-rw-r--r--   0        0        0    11648 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ba990db40695c4c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bb1dcac04558aa58
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bb3076c186c5e48c
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bb60fc63ce6802e9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bb807b59dbc4bdfd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bb8c05654ed9e9b7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bc2b5e7e52d0f484
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bc75158622377457
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bceae428d80fc265
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/be0258dfb02cf830
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/be1ddda6d4f39061
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/be2c92c76d2740ad
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/be4fda96b47058dc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bf5b7656d36257d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/bfdec7cf16642191
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c038210460d61f03
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c0c12c5ed5a1c4d5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c0f2daee3007d308
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c0faa240c1c7cdca
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c12f847e1f7e109f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c14834a03d94cda7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c1c35285ff749e19
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c230f496de5623fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c26842b025e9cd0e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c26e775cfd3499dd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c31ecbfd313817a5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c3225006ad60ac72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c353ea9c4491a398
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c388269ab4702e0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c390f81406de06a9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c4d8a74ebe67d58b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c5168342488cee45
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c5240c8dade100bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c58bc3d494caa835
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c604f7c5f1e3ebd5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c65e57c7dd7c462d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c69a7aaf33a80fc3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c69bcb4a882d9a80
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c7925727132bfa35
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c792c6fc3eae47d1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c856b21784c6e79c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c89892fe699cc3fe
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c922e1349e86dacf
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c93e0470b5916cdd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c9d0dd44192d33cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/c9d5ddb22fabed97
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ca352c3beef7d7c8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/caf7e5dcfa6bc9d7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cbe805f3c73da149
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cc3ce99c6e18e90d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cc58fb9f592bc4bd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cc6a2d087c5d64b4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cc6e6a8919f02930
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cca86acbb5e18c21
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cd820a5c908830d3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ce4387510ee1a3b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ceafd5618a35f4f9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cf2a2039834c5d72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cf4ac7dceba0b58f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/cff4748ea971a75a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d077f2812de711be
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d123f6c79d8962eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d1cf0614c2201092
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d1d28f11735c6d00
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d20dff382c70215a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d2f50ef448721c72
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d33c136d5f87fca7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d33c4750d6529287
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d355282da21c57f4
+-rw-r--r--   0        0        0    11485 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d3c281afd785ce67
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d3ed2866540e006d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d47d56f172c95268
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d50d12f599a024cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d52bca8009858378
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d566c25d9bcf6a5d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d68170a0d6785a5e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d689a4ddec4cf2a3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d68f76d689da20dd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d6c72a0cefe48a41
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d74940f52155d37a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d7fda4b87b627c57
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d81a5721be3b33e4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d834929874d754cb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d89027a3e15ec70e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d8dd41799a5819a1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d8fce08c24029ddb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/d99bff5348cdaa3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/da3f17bef9ff1452
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/da66abd474daf8a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dab63365705f2c3a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/db53eac7c4f9b45
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/db66e9921b7a863f
+-rw-r--r--   0        0        0     6887 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/db7201f35dede22c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dbb165a4f77f62f2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dc085b6ef6707fde
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dc95d536a88ff778
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dcc3a69e8cdc2491
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dcfa97f5b5de9b04
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dd1dd50de7d99c9f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dd219cea516ce16c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dd2aba3bcb45c51
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dd74ceefa0b69fbb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/de7291b28d7d5474
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/df3ee8f92bafdc4d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/df730e127d9f8f59
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/df9b632d3998a03b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/df9f24befe6e957b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/dfd1df7a05885192
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e030ca550bf6df98
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e03eeccb215c48dd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e0b20f03c0ba2a76
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e1819f8316b1bb10
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e1c37d3cfadf1e64
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e1f20d69e69dede
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e22b88f42322c55f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e263d364231cdfd6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e2efb83cf42e4e6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e2f8484e235911eb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e31187b0d2d6e1fb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e432c1886f7760da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e4cdfe843225f49d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e53d0434b38dfbfc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e54c6545e9b1b849
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e5abe659bf4ce244
+-rw-r--r--   0        0        0    11046 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e5cf3c6f5d6a07f6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e65b443e60aa12a0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e6c15f2f5d4fdc62
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e6c571fb2e0c17af
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e7463edadad452e2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e7469afc3fa8ea9d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e74bf5df7a8a3678
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e74d1f6d9d86f9ba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e7b2a64eb8c109a1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e804246f84912b80
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e8bf91c6ee4619ba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e8cd356d65e5883f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e90c00d83ce6c616
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e980fb9cf8e49de1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/e9a69e69336feba9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ea91af2e36e208b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ea9ca6d76c8cd2e1
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/eb4eec7876e6d0da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/eb4ff75cadd390e6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/eb83c97b6f0cdb39
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ebaeb2bca35fbe39
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ebd1bb294cd53311
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ec7ab93b4ded8208
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/eca7e0f8f764bdbc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ecc5ec0b6bcf62ae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/eccd87726973b0a9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ed121b06a25166b9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ed38faf72768bda4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ed6ad9f2288ecd57
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ed87be7d4e722553
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/edd5fc49464dd6f0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ef3369465951410c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/effd11ca46dbec83
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f0f808c0c87d992e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f0fadb410014ffa5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f17705e01814f8cc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f1f11dc9c78497ee
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f2191752d4ea65dd
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f2eb80dab531e444
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f315c5f98e9b715e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f329c27e29c25278
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f358dbac48fccf35
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f377c8061fe5a8b8
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f3c75ce44e2730b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f3ff627f6219a3d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f424d75538c3c91b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f4703c0d32c87dcc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f4970125eadbdbc
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f4b7bd65af024161
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f519b7e63b38f442
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f558faa8ed756ab3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f5b965ca7db4150
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f63919e0a72954d0
+-rw-r--r--   0        0        0     6163 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f6601e9cf957e003
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f6a5021a70e24e17
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f706f6e0a1e187cd
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f707d2d075567c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f7ede18bdbb88a95
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f7f964ae4ea74955
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f7fe78c710ec881f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f91a7b9bb11f1a87
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/f9f26eb41433dec0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fa216d6a179d44c0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fa598938a1ccc3d0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/faf0fb1f96110497
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fbc270d41df617ce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fbc3943a6603b64e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fc52a386c4fc2f56
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fc61ad2102387cb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fc70b58b4bcd985
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fce54a4a389c1c13
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fd0ebd01c66bbe1f
+-rw-r--r--   0        0        0    11404 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fd8ef1c845b41a08
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fdcfc4dd63763ed6
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fe1fbca3e01844e1
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fe392c6c58e71695
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fe6ef6865099e6c8
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fead50943ff7eae
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fecfec0638a3b27f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/fef8a786c45c9da0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ff19a9485c69fa47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ff1bb6cef083bbc6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ff32308b229eff24
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.ruff_cache/content/ff42ca52a3140996
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/__init__.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/__main__.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/__version__.py
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/validator.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/apps/__init__.py
+-rw-r--r--   0        0        0    14279 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/apps/api.py
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/apps/e2xgraderapp.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/config/__init__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/converters/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/converters/converter.py
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/converters/generateexercise.py
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/__init__.py
+-rw-r--r--   0        0        0     4435 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/collect.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/exchange.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/fetch_assignment.py
+-rw-r--r--   0        0        0     6604 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/fetch_feedback.py
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/list.py
+-rw-r--r--   0        0        0     5819 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/release_assignment.py
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/release_feedback.py
+-rw-r--r--   0        0        0     8007 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/submit.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exchange/utils.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exporters/__init__.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exporters/exporter.py
+-rw-r--r--   0        0        0     5034 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exporters/gradeexporter.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exporters/filters/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/exporters/filters/highlight.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/graders/__init__.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/graders/base.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/graders/code.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/graders/multiplechoice.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/graders/singlechoice.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/__init__.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/assignmentmodel.py
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/basemodel.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/exercisemodel.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presetmodel.py
+-rw-r--r--   0        0        0     3972 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/taskmodel.py
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/taskpoolmodel.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/templatemodel.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Code (Autograded).ipynb
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Code (Manual).ipynb
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Diagram.ipynb
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Freetext.ipynb
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Multiple Choice.ipynb
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Single Choice.ipynb
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Upload Files.ipynb
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/template/Footer.ipynb
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/template/Group Info.ipynb
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/template/Header.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/models/presets/template/Student Info.ipynb
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/clearhiddentests.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/clearsolutions.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/extractattachments.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/filtercellsbyid.py
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/filtertests.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/overwritecells.py
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/permutetasks.py
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/saveautogrades.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/savecells.py
+-rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/scramble.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/unpermutetasks.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/unscramble.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/validateextracells.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/__init__.py
+-rw-r--r--   0        0        0     3155 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/addtaskheader.py
+-rw-r--r--   0        0        0     3391 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/copyfiles.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/copynotebooks.py
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/filltemplate.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/generatetaskids.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/makeexercise.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/preprocessor.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/removeexercise.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/assignment_list/__init__.py
+-rw-r--r--   0        0        0     4118 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/assignment_list/handlers.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/__init__.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/grader.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/__init__.py
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/apihandlers.py
+-rw-r--r--   0        0        0     1019 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/authoring.py
+-rw-r--r--   0        0        0     3738 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/handlers.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/css/editexercise.css
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/css/sidebar.css
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/css/taskcreator.css
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/assignments.js
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/base.js
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/exercises.js
+-rw-r--r--   0        0        0     9985 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/makeexercise.js
+-rw-r--r--   0        0        0     3002 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/taskpools.js
+-rw-r--r--   0        0        0     3616 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/tasks.js
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/templates.js
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/assignments.tpl
+-rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/base.tpl
+-rw-r--r--   0        0        0     3523 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/editexercise.tpl
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/exercises.tpl
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tablebase.tpl
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskcreator.tpl
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskpools.tpl
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tasks.tpl
+-rw-r--r--   0        0        0     1228 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/templates.tpl
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/base/__init__.py
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/base/base.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/base/handlers/base.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/__init__.py
+-rw-r--r--   0        0        0     5367 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/apihandlers.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/base.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/e2xgraderapi.py
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Diagram.ipynb
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Freetext.ipynb
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb
+-rw-r--r--   0        0        0      984 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Single Choice.ipynb
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Upload Files.ipynb
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Footer.ipynb
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Group Info.ipynb
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Header.ipynb
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Student Info.ipynb
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/conf.json
+-rw-r--r--   0        0        0     8033 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/index.html.j2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/form/conf.json
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/form/index.html.j2
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/__init__.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/formgrader.py
+-rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/handlers.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/css/eraser-solid.svg
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/css/pencil-solid.svg
+-rw-r--r--   0        0        0    10212 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade.js
+-rw-r--r--   0        0        0    10152 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade_models.js
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_assignments.js
+-rw-r--r--   0        0        0     7163 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebook_submissions.js
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebooks.js
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_tasks.js
+-rw-r--r--   0        0        0    20906 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_assignments.js
+-rw-r--r--   0        0        0    11542 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_submissions.js
+-rw-r--r--   0        0        0     6587 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/base.tpl
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/export_grades.tpl
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/gradebook_base.tpl
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_assignments.tpl
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_students_base.tpl
+-rw-r--r--   0        0        0     2302 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_submissions.tpl
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/conf.json
+-rw-r--r--   0        0        0     5542 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/formgrade_macros.html.j2
+-rw-r--r--   0        0        0    12156 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/index.html.j2
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_assignments.tpl
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_base.tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebooks.tpl
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_tasks.tpl
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/nbgraderapi/__init__.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/nbgraderapi/nbgraderapi.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/validate_assignment/__init__.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/validate_assignment/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/__init__.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/test_validator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/apps/__init__.py
+-rw-r--r--   0        0        0     6879 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/apps/test_e2xgraderapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/converters/__init__.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/converters/test_generateexercise.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/exporters/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/exporters/filters/__init__.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/exporters/filters/test_highlight.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/graders/__init__.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/graders/test_base.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/graders/test_code.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/graders/test_multiplechoice.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/graders/test_singlechoice.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/models/__init__.py
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_assignmentmodel.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_basemodel.py
+-rw-r--r--   0        0        0     2656 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_exercisemodel.py
+-rw-r--r--   0        0        0     2874 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_presetmodel.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_taskmodel.py
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_taskpoolmodel.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_templatemodel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/__init__.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_clearhiddentests.py
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_clearsolutions.py
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_extractattachments.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_filtercellsbyid.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_filtertests.py
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_unscramble.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_validateextracells.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/authoring/__init__.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/authoring/base.py
+-rw-r--r--   0        0        0     3448 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/authoring/test_copyfiles.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/authoring/test_copynotebooks.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     4757 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/test_utils/cells.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/test_utils/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/utils/test_extra_cells.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/utils/test_nbgrader_cells.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/tests/utils/test_notebookvariableextractor.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/utils/__init__.py
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/utils/extra_cells.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/utils/nbgrader_cells.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/utils/notebookvariableextractor.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/e2xgrader/utils/utils.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/LICENSE
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/README.md
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 e2xgrader-0.1.0.dev3/PKG-INFO
```

### Comparing `e2xgrader-0.1.0.dev1/nbgrader_config.py` & `e2xgrader-0.1.0.dev3/nbgrader_config.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/package-lock.json` & `e2xgrader-0.1.0.dev3/package-lock.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9165793870887429%*

 * *Differences: {"'dependencies'": "{'@e2xgrader/assignment-view-celltoolbar': {'requires': {'@e2xgrader/cells': "*

 * *                   "'0.1.0-dev3', '@e2xgrader/utils': '0.1.0-dev3'}}, "*

 * *                   "'@e2xgrader/authoring-menubar': {'requires': {'@e2xgrader/api': '0.1.0-dev3', "*

 * *                   "'@e2xgrader/menubar': '0.1.0-dev3', '@e2xgrader/utils': '0.1.0-dev3'}}, "*

 * *                   "'@e2xgrader/cell-extension': {'requires': {'@e2xgrader/cells': '0.1.0-dev3'}}, "*

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
-                "@e2xgrader/cells": "0.1.0-dev1",
-                "@e2xgrader/utils": "0.1.0-dev1",
+                "@e2xgrader/cells": "0.1.0-dev3",
+                "@e2xgrader/utils": "0.1.0-dev3",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/assignment-view-celltoolbar"
         },
         "@e2xgrader/authoring-menubar": {
             "requires": {
-                "@e2xgrader/api": "0.1.0-dev1",
-                "@e2xgrader/menubar": "0.1.0-dev1",
-                "@e2xgrader/utils": "0.1.0-dev1",
+                "@e2xgrader/api": "0.1.0-dev3",
+                "@e2xgrader/menubar": "0.1.0-dev3",
+                "@e2xgrader/utils": "0.1.0-dev3",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/authoring-menubar"
         },
         "@e2xgrader/cell-extension": {
             "requires": {
                 "@babel/preset-env": "^7.16.11",
-                "@e2xgrader/cells": "0.1.0-dev1",
+                "@e2xgrader/cells": "0.1.0-dev3",
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
-                "@e2xgrader/cells": "0.1.0-dev1",
-                "@e2xgrader/utils": "0.1.0-dev1",
+                "@e2xgrader/cells": "0.1.0-dev3",
+                "@e2xgrader/utils": "0.1.0-dev3",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/create-assignment-celltoolbar"
         },
         "@e2xgrader/exam-menubar": {
             "requires": {
-                "@e2xgrader/menubar": "0.1.0-dev1",
+                "@e2xgrader/menubar": "0.1.0-dev3",
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
-                "@e2xgrader/assignment-view-celltoolbar": "0.1.0-dev1",
-                "@e2xgrader/authoring-menubar": "0.1.0-dev1",
-                "@e2xgrader/cell-extension": "0.1.0-dev1",
-                "@e2xgrader/create-assignment-celltoolbar": "0.1.0-dev1",
-                "@e2xgrader/exam-menubar": "0.1.0-dev1",
-                "@e2xgrader/restricted-assignment-notebook": "0.1.0-dev1",
-                "@e2xgrader/restricted-exam-notebook": "0.1.0-dev1",
+                "@e2xgrader/assignment-view-celltoolbar": "0.1.0-dev3",
+                "@e2xgrader/authoring-menubar": "0.1.0-dev3",
+                "@e2xgrader/cell-extension": "0.1.0-dev3",
+                "@e2xgrader/create-assignment-celltoolbar": "0.1.0-dev3",
+                "@e2xgrader/exam-menubar": "0.1.0-dev3",
+                "@e2xgrader/restricted-assignment-notebook": "0.1.0-dev3",
+                "@e2xgrader/restricted-exam-notebook": "0.1.0-dev3",
                 "css-loader": "^6.6.0",
                 "style-loader": "^3.3.1",
                 "webpack": "^5.70.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/notebook-extensions"
         },
         "@e2xgrader/restricted-assignment-notebook": {
             "requires": {
-                "@e2xgrader/utils": "0.1.0-dev1",
+                "@e2xgrader/utils": "0.1.0-dev3",
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "version": "file:packages/restricted-assignment-notebook"
         },
         "@e2xgrader/restricted-exam-notebook": {
             "requires": {
-                "@e2xgrader/utils": "0.1.0-dev1",
+                "@e2xgrader/utils": "0.1.0-dev3",
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
-            "version": "0.1.0-dev1",
+            "version": "0.1.0-dev3",
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
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
         },
         "packages/assignment-view-celltoolbar": {
             "dependencies": {
-                "@e2xgrader/cells": "0.1.0-dev1",
-                "@e2xgrader/utils": "0.1.0-dev1"
+                "@e2xgrader/cells": "0.1.0-dev3",
+                "@e2xgrader/utils": "0.1.0-dev3"
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
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
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
-                "@e2xgrader/api": "0.1.0-dev1",
-                "@e2xgrader/menubar": "0.1.0-dev1",
-                "@e2xgrader/utils": "0.1.0-dev1"
+                "@e2xgrader/api": "0.1.0-dev3",
+                "@e2xgrader/menubar": "0.1.0-dev3",
+                "@e2xgrader/utils": "0.1.0-dev3"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/authoring-menubar",
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
         },
         "packages/cell-extension": {
             "dependencies": {
-                "@e2xgrader/cells": "0.1.0-dev1"
+                "@e2xgrader/cells": "0.1.0-dev3"
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
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
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
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
         },
         "packages/create-assignment-celltoolbar": {
             "dependencies": {
-                "@e2xgrader/cells": "0.1.0-dev1",
-                "@e2xgrader/utils": "0.1.0-dev1"
+                "@e2xgrader/cells": "0.1.0-dev3",
+                "@e2xgrader/utils": "0.1.0-dev3"
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
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
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
-                "@e2xgrader/menubar": "0.1.0-dev1"
+                "@e2xgrader/menubar": "0.1.0-dev3"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/exam-menubar",
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
         },
         "packages/menubar": {
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/menubar",
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
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
-                "@e2xgrader/assignment-view-celltoolbar": "0.1.0-dev1",
-                "@e2xgrader/authoring-menubar": "0.1.0-dev1",
-                "@e2xgrader/cell-extension": "0.1.0-dev1",
-                "@e2xgrader/create-assignment-celltoolbar": "0.1.0-dev1",
-                "@e2xgrader/exam-menubar": "0.1.0-dev1",
-                "@e2xgrader/restricted-assignment-notebook": "0.1.0-dev1",
-                "@e2xgrader/restricted-exam-notebook": "0.1.0-dev1"
+                "@e2xgrader/assignment-view-celltoolbar": "0.1.0-dev3",
+                "@e2xgrader/authoring-menubar": "0.1.0-dev3",
+                "@e2xgrader/cell-extension": "0.1.0-dev3",
+                "@e2xgrader/create-assignment-celltoolbar": "0.1.0-dev3",
+                "@e2xgrader/exam-menubar": "0.1.0-dev3",
+                "@e2xgrader/restricted-assignment-notebook": "0.1.0-dev3",
+                "@e2xgrader/restricted-exam-notebook": "0.1.0-dev3"
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
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
         },
         "packages/restricted-assignment-notebook": {
             "dependencies": {
-                "@e2xgrader/utils": "0.1.0-dev1"
+                "@e2xgrader/utils": "0.1.0-dev3"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/restricted-assignment-notebook",
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
         },
         "packages/restricted-exam-notebook": {
             "dependencies": {
-                "@e2xgrader/utils": "0.1.0-dev1"
+                "@e2xgrader/utils": "0.1.0-dev3"
             },
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/restricted-exam-notebook",
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
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
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
         },
         "packages/utils": {
             "devDependencies": {
                 "webpack": "^5.73.0",
                 "webpack-cli": "^4.9.2"
             },
             "license": "MIT",
             "name": "@e2xgrader/utils",
-            "version": "0.1.0-dev1"
+            "version": "0.1.0-dev3"
         }
     },
     "requires": true,
-    "version": "0.1.0-dev1"
+    "version": "0.1.0-dev3"
 }
```

### Comparing `e2xgrader-0.1.0.dev1/package.json` & `e2xgrader-0.1.0.dev3/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.1.0-dev3'"}*

```diff
@@ -30,12 +30,12 @@
     },
     "scripts": {
         "build": "lerna run build",
         "install": "lerna run bootstrap",
         "prettier": "prettier --write \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md}\"",
         "prettier:files": "prettier --write"
     },
-    "version": "0.1.0-dev1",
+    "version": "0.1.0-dev3",
     "workspaces": [
         "packages/*"
     ]
 }
```

### Comparing `e2xgrader-0.1.0.dev1/.github/workflows/dispatch.yml` & `e2xgrader-0.1.0.dev3/.github/workflows/dispatch.yml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/.github/workflows/python-package.yml` & `e2xgrader-0.1.0.dev3/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/.github/workflows/sonar-scan.yml` & `e2xgrader-0.1.0.dev3/.github/workflows/sonar-scan.yml`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/__init__.py` & `e2xgrader-0.1.0.dev3/e2xgrader/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/validator.py` & `e2xgrader-0.1.0.dev3/e2xgrader/validator.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/apps/api.py` & `e2xgrader-0.1.0.dev3/e2xgrader/apps/api.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/apps/e2xgraderapp.py` & `e2xgrader-0.1.0.dev3/e2xgrader/apps/e2xgraderapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,19 +162,19 @@
 class Manager:
     def __init__(self):
         self.extension_manager = ExtensionManager()
         parser = ArgumentParser(
             description="E2X extension manager.",
             usage=dedent(
                 """
-                                             e2xgrader <command> [<args>]
+                e2xgrader <command> [<args>]
 
-                                             Available sub commands are:
-                                               activate      activate a specific mode (teacher, student, student-exam)
-                                               deactivate    deactivate all extensions"""
+                Available sub commands are:
+                activate      activate a specific mode (teacher, student, student-exam)
+                deactivate    deactivate all extensions"""
             ),
         )
 
         parser.add_argument("command", help="Subcommand to run")
 
         args = parser.parse_args(sys.argv[1:2])
         if not hasattr(self, args.command):
@@ -184,20 +184,20 @@
         getattr(self, args.command)()
 
     def activate(self):
         parser = ArgumentParser(
             description="Activate different modes",
             usage=dedent(
                 """
-                                             e2xgrader activate <mode> [--sys-prefix] [--user]
+                e2xgrader activate <mode> [--sys-prefix] [--user]
 
-                                             Available modes are:
-                                               teacher         activate the grader and all teaching extensions
-                                               student         activate the student extensions
-                                               student_exam    activate the student extensions in exam mode"""
+                Available modes are:
+                teacher         activate the grader and all teaching extensions
+                student         activate the student extensions
+                student_exam    activate the student extensions in exam mode"""
             ),
         )
         # prefixing the argument with -- means it's optional
         parser.add_argument(
             "mode",
             help="Which mode to activate, can be teacher, student or student-exam",
         )
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/config/__init__.py` & `e2xgrader-0.1.0.dev3/e2xgrader/config/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/converters/converter.py` & `e2xgrader-0.1.0.dev3/e2xgrader/converters/converter.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/converters/generateexercise.py` & `e2xgrader-0.1.0.dev3/e2xgrader/converters/generateexercise.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/__init__.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/collect.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exchange/collect.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,25 @@
 class E2xExchangeCollect(E2xExchange, ExchangeCollect):
     update = Bool(
         False, help="Update existing submissions with ones that have newer timestamps."
     ).tag(config=True)
 
     before_duedate = Bool(
         False,
-        help="Collect the last submission before due date or the last submission if no submission before due date.",
+        help=(
+            "Collect the last submission before due date or the last submission\n"
+            "if no submission before due date."
+        ),
     ).tag(config=True)
 
     check_owner = Bool(
         default_value=True,
-        help="Whether to cross-check the student_id with the UNIX-owner of the submitted directory.",
+        help=(
+            "Whether to cross-check the student_id with the UNIX-owner of the submitted directory."
+        ),
     ).tag(config=True)
 
     def init_submissions(self):
         if self.personalized_inbound:
             self.log.info("Collecting from restricted submit dirs")
             submit_dirs = [
                 username
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/exchange.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exchange/exchange.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/fetch_assignment.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exchange/fetch_assignment.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/fetch_feedback.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exchange/fetch_feedback.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/list.py` & `e2xgrader-0.1.0.dev3/.ruff_cache/content/3ee91de4595bdbc5`

 * *Files 2% similar despite different names*

```diff
@@ -1,696 +1,708 @@
-00000000: 696d 706f 7274 2067 6c6f 620a 696d 706f  import glob.impo
-00000010: 7274 2068 6173 686c 6962 0a69 6d70 6f72  rt hashlib.impor
-00000020: 7420 6f73 0a69 6d70 6f72 7420 7265 0a0a  t os.import re..
-00000030: 6672 6f6d 206e 6267 7261 6465 722e 6578  from nbgrader.ex
-00000040: 6368 616e 6765 2e64 6566 6175 6c74 2069  change.default i
-00000050: 6d70 6f72 7420 4578 6368 616e 6765 4c69  mport ExchangeLi
-00000060: 7374 0a66 726f 6d20 6e62 6772 6164 6572  st.from nbgrader
-00000070: 2e75 7469 6c73 2069 6d70 6f72 7420 6d61  .utils import ma
-00000080: 6b65 5f75 6e69 7175 655f 6b65 792c 206e  ke_unique_key, n
-00000090: 6f74 6562 6f6f 6b5f 6861 7368 0a0a 6672  otebook_hash..fr
-000000a0: 6f6d 202e 6578 6368 616e 6765 2069 6d70  om .exchange imp
-000000b0: 6f72 7420 4532 7845 7863 6861 6e67 650a  ort E2xExchange.
-000000c0: 0a0a 6465 6620 5f63 6865 636b 7375 6d28  ..def _checksum(
-000000d0: 7061 7468 293a 0a20 2020 206d 203d 2068  path):.    m = h
-000000e0: 6173 686c 6962 2e6d 6435 2829 0a20 2020  ashlib.md5().   
-000000f0: 206d 2e75 7064 6174 6528 6f70 656e 2870   m.update(open(p
-00000100: 6174 682c 2022 7262 2229 2e72 6561 6428  ath, "rb").read(
-00000110: 2929 0a20 2020 2072 6574 7572 6e20 6d2e  )).    return m.
-00000120: 6865 7864 6967 6573 7428 290a 0a0a 6465  hexdigest()...de
-00000130: 6620 5f67 6574 5f6b 6579 2869 6e66 6f29  f _get_key(info)
-00000140: 3a0a 2020 2020 7265 7475 726e 2069 6e66  :.    return inf
-00000150: 6f5b 2263 6f75 7273 655f 6964 225d 2c20  o["course_id"], 
-00000160: 696e 666f 5b22 7374 7564 656e 745f 6964  info["student_id
-00000170: 225d 2c20 696e 666f 5b22 6173 7369 676e  "], info["assign
-00000180: 6d65 6e74 5f69 6422 5d0a 0a0a 6465 6620  ment_id"]...def 
-00000190: 5f6d 6174 6368 5f6b 6579 2869 6e66 6f2c  _match_key(info,
-000001a0: 206b 6579 293a 0a20 2020 2072 6574 7572   key):.    retur
-000001b0: 6e20 280a 2020 2020 2020 2020 696e 666f  n (.        info
-000001c0: 5b22 636f 7572 7365 5f69 6422 5d20 3d3d  ["course_id"] ==
-000001d0: 206b 6579 5b30 5d0a 2020 2020 2020 2020   key[0].        
-000001e0: 616e 6420 696e 666f 5b22 7374 7564 656e  and info["studen
-000001f0: 745f 6964 225d 203d 3d20 6b65 795b 315d  t_id"] == key[1]
-00000200: 0a20 2020 2020 2020 2061 6e64 2069 6e66  .        and inf
-00000210: 6f5b 2261 7373 6967 6e6d 656e 745f 6964  o["assignment_id
-00000220: 225d 203d 3d20 6b65 795b 325d 0a20 2020  "] == key[2].   
-00000230: 2029 0a0a 0a63 6c61 7373 2045 3278 4578   )...class E2xEx
-00000240: 6368 616e 6765 4c69 7374 2845 3278 4578  changeList(E2xEx
-00000250: 6368 616e 6765 2c20 4578 6368 616e 6765  change, Exchange
-00000260: 4c69 7374 293a 0a20 2020 2064 6566 2069  List):.    def i
-00000270: 6e69 745f 6465 7374 2873 656c 6629 3a0a  nit_dest(self):.
-00000280: 2020 2020 2020 2020 636f 7572 7365 5f69          course_i
-00000290: 6420 3d20 7365 6c66 2e63 6f75 7273 6564  d = self.coursed
-000002a0: 6972 2e63 6f75 7273 655f 6964 2069 6620  ir.course_id if 
-000002b0: 7365 6c66 2e63 6f75 7273 6564 6972 2e63  self.coursedir.c
-000002c0: 6f75 7273 655f 6964 2065 6c73 6520 222a  ourse_id else "*
-000002d0: 220a 2020 2020 2020 2020 6173 7369 676e  ".        assign
-000002e0: 6d65 6e74 5f69 6420 3d20 280a 2020 2020  ment_id = (.    
-000002f0: 2020 2020 2020 2020 7365 6c66 2e63 6f75          self.cou
-00000300: 7273 6564 6972 2e61 7373 6967 6e6d 656e  rsedir.assignmen
-00000310: 745f 6964 2069 6620 7365 6c66 2e63 6f75  t_id if self.cou
-00000320: 7273 6564 6972 2e61 7373 6967 6e6d 656e  rsedir.assignmen
-00000330: 745f 6964 2065 6c73 6520 222a 220a 2020  t_id else "*".  
-00000340: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00000350: 7374 7564 656e 745f 6964 203d 2073 656c  student_id = sel
-00000360: 662e 636f 7572 7365 6469 722e 7374 7564  f.coursedir.stud
-00000370: 656e 745f 6964 2069 6620 7365 6c66 2e63  ent_id if self.c
-00000380: 6f75 7273 6564 6972 2e73 7475 6465 6e74  oursedir.student
-00000390: 5f69 6420 656c 7365 2022 2a22 0a0a 2020  _id else "*"..  
-000003a0: 2020 2020 2020 6966 2073 656c 662e 696e        if self.in
-000003b0: 626f 756e 643a 0a20 2020 2020 2020 2020  bound:.         
-000003c0: 2020 2070 6174 7465 726e 203d 206f 732e     pattern = os.
-000003d0: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
-000003e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000003f0: 726f 6f74 2c0a 2020 2020 2020 2020 2020  root,.          
-00000400: 2020 2020 2020 636f 7572 7365 5f69 642c        course_id,
-00000410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000420: 2073 656c 662e 696e 626f 756e 645f 6469   self.inbound_di
-00000430: 7265 6374 6f72 792c 0a20 2020 2020 2020  rectory,.       
-00000440: 2020 2020 2020 2020 2022 7b7d 2b7b 7d2b           "{}+{}+
-00000450: 2a22 2e66 6f72 6d61 7428 7374 7564 656e  *".format(studen
-00000460: 745f 6964 2c20 6173 7369 676e 6d65 6e74  t_id, assignment
-00000470: 5f69 6429 2c0a 2020 2020 2020 2020 2020  _id),.          
-00000480: 2020 290a 2020 2020 2020 2020 656c 6966    ).        elif
-00000490: 2073 656c 662e 6361 6368 6564 3a0a 2020   self.cached:.  
-000004a0: 2020 2020 2020 2020 2020 7061 7474 6572            patter
-000004b0: 6e20 3d20 6f73 2e70 6174 682e 6a6f 696e  n = os.path.join
-000004c0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000004d0: 2020 7365 6c66 2e63 6163 6865 2c20 636f    self.cache, co
-000004e0: 7572 7365 5f69 642c 2022 7b7d 2b7b 7d2b  urse_id, "{}+{}+
-000004f0: 2a22 2e66 6f72 6d61 7428 7374 7564 656e  *".format(studen
-00000500: 745f 6964 2c20 6173 7369 676e 6d65 6e74  t_id, assignment
-00000510: 5f69 6429 0a20 2020 2020 2020 2020 2020  _id).           
-00000520: 2029 0a20 2020 2020 2020 2065 6c73 653a   ).        else:
-00000530: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00000540: 7365 6c66 2e70 6572 736f 6e61 6c69 7a65  self.personalize
-00000550: 645f 6f75 7462 6f75 6e64 3a0a 2020 2020  d_outbound:.    
-00000560: 2020 2020 2020 2020 2020 2020 2320 6c69              # li
-00000570: 7374 2061 6c6c 2061 7373 6967 6e6d 656e  st all assignmen
-00000580: 7473 2068 6572 650a 2020 2020 2020 2020  ts here.        
-00000590: 2020 2020 2020 2020 7061 7474 6572 6e20          pattern 
-000005a0: 3d20 6f73 2e70 6174 682e 6a6f 696e 280a  = os.path.join(.
-000005b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005c0: 2020 2020 7365 6c66 2e72 6f6f 742c 0a20      self.root,. 
-000005d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005e0: 2020 2063 6f75 7273 655f 6964 2c0a 2020     course_id,.  
-000005f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000600: 2020 7365 6c66 2e6f 7574 626f 756e 645f    self.outbound_
-00000610: 6469 7265 6374 6f72 792c 0a20 2020 2020  directory,.     
-00000620: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000630: 7475 6465 6e74 5f69 642c 0a20 2020 2020  tudent_id,.     
-00000640: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00000650: 7b7d 222e 666f 726d 6174 2861 7373 6967  {}".format(assig
-00000660: 6e6d 656e 745f 6964 292c 0a20 2020 2020  nment_id),.     
-00000670: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00000680: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00000690: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000006a0: 6174 7465 726e 203d 206f 732e 7061 7468  attern = os.path
-000006b0: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
-000006c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000006d0: 726f 6f74 2c0a 2020 2020 2020 2020 2020  root,.          
-000006e0: 2020 2020 2020 2020 2020 636f 7572 7365            course
-000006f0: 5f69 642c 0a20 2020 2020 2020 2020 2020  _id,.           
-00000700: 2020 2020 2020 2020 2073 656c 662e 6f75           self.ou
-00000710: 7462 6f75 6e64 5f64 6972 6563 746f 7279  tbound_directory
-00000720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000730: 2020 2020 2020 227b 7d22 2e66 6f72 6d61        "{}".forma
-00000740: 7428 6173 7369 676e 6d65 6e74 5f69 6429  t(assignment_id)
-00000750: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00000760: 2020 290a 0a20 2020 2020 2020 2073 656c    )..        sel
-00000770: 662e 6173 7369 676e 6d65 6e74 7320 3d20  f.assignments = 
-00000780: 736f 7274 6564 2867 6c6f 622e 676c 6f62  sorted(glob.glob
-00000790: 2870 6174 7465 726e 2929 0a0a 2020 2020  (pattern))..    
-000007a0: 6465 6620 7061 7273 655f 6173 7369 676e  def parse_assign
-000007b0: 6d65 6e74 2873 656c 662c 2061 7373 6967  ment(self, assig
-000007c0: 6e6d 656e 7429 3a0a 2020 2020 2020 2020  nment):.        
-000007d0: 6966 2073 656c 662e 696e 626f 756e 643a  if self.inbound:
-000007e0: 0a20 2020 2020 2020 2020 2020 2072 6567  .            reg
-000007f0: 6578 7020 3d20 280a 2020 2020 2020 2020  exp = (.        
-00000800: 2020 2020 2020 2020 7222 2e2a 2f28 3f50          r".*/(?P
-00000810: 3c63 6f75 7273 655f 6964 3e2e 2a29 2f22  <course_id>.*)/"
-00000820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000830: 202b 2073 656c 662e 696e 626f 756e 645f   + self.inbound_
-00000840: 6469 7265 6374 6f72 790a 2020 2020 2020  directory.      
-00000850: 2020 2020 2020 2020 2020 2b20 7222 2f28            + r"/(
-00000860: 3f50 3c73 7475 6465 6e74 5f69 643e 5b5e  ?P<student_id>[^
-00000870: 2b5d 2a29 5c2b 283f 503c 6173 7369 676e  +]*)\+(?P<assign
-00000880: 6d65 6e74 5f69 643e 5b5e 2b5d 2a29 5c2b  ment_id>[^+]*)\+
-00000890: 283f 503c 7469 6d65 7374 616d 703e 5b5e  (?P<timestamp>[^
-000008a0: 2b5d 2a29 283f 503c 7261 6e64 6f6d 5f73  +]*)(?P<random_s
-000008b0: 7472 696e 673e 5c2b 2e2a 293f 220a 2020  tring>\+.*)?".  
-000008c0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000008d0: 2020 2020 656c 6966 2073 656c 662e 6361      elif self.ca
-000008e0: 6368 6564 3a0a 2020 2020 2020 2020 2020  ched:.          
-000008f0: 2020 7265 6765 7870 203d 2072 222e 2a2f    regexp = r".*/
-00000900: 283f 503c 636f 7572 7365 5f69 643e 2e2a  (?P<course_id>.*
-00000910: 292f 283f 503c 7374 7564 656e 745f 6964  )/(?P<student_id
-00000920: 3e2e 2a29 5c2b 283f 503c 6173 7369 676e  >.*)\+(?P<assign
-00000930: 6d65 6e74 5f69 643e 2e2a 295c 2b28 3f50  ment_id>.*)\+(?P
-00000940: 3c74 696d 6573 7461 6d70 3e2e 2a29 220a  <timestamp>.*)".
-00000950: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00000960: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00000970: 662e 7065 7273 6f6e 616c 697a 6564 5f6f  f.personalized_o
-00000980: 7574 626f 756e 643a 0a20 2020 2020 2020  utbound:.       
-00000990: 2020 2020 2020 2020 2072 6567 6578 7020           regexp 
-000009a0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000009b0: 2020 2020 2020 2020 7222 2e2a 2f28 3f50          r".*/(?P
-000009c0: 3c63 6f75 7273 655f 6964 3e2e 2a29 2f22  <course_id>.*)/"
-000009d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000009e0: 2020 2020 202b 2073 656c 662e 6f75 7462       + self.outb
-000009f0: 6f75 6e64 5f64 6972 6563 746f 7279 0a20  ound_directory. 
-00000a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a10: 2020 202b 2072 222f 283f 503c 7374 7564     + r"/(?P<stud
-00000a20: 656e 745f 6964 3e2e 2a29 220a 2020 2020  ent_id>.*)".    
-00000a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a40: 2b20 7222 2f28 3f50 3c61 7373 6967 6e6d  + r"/(?P<assignm
-00000a50: 656e 745f 6964 3e2e 2a29 220a 2020 2020  ent_id>.*)".    
-00000a60: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00000a70: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00000a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000a90: 7265 6765 7870 203d 2028 0a20 2020 2020  regexp = (.     
-00000aa0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00000ab0: 222e 2a2f 283f 503c 636f 7572 7365 5f69  ".*/(?P<course_i
-00000ac0: 643e 2e2a 292f 220a 2020 2020 2020 2020  d>.*)/".        
-00000ad0: 2020 2020 2020 2020 2020 2020 2b20 7365              + se
-00000ae0: 6c66 2e6f 7574 626f 756e 645f 6469 7265  lf.outbound_dire
-00000af0: 6374 6f72 790a 2020 2020 2020 2020 2020  ctory.          
-00000b00: 2020 2020 2020 2020 2020 2b20 7222 2f28            + r"/(
-00000b10: 3f50 3c61 7373 6967 6e6d 656e 745f 6964  ?P<assignment_id
-00000b20: 3e2e 2a29 220a 2020 2020 2020 2020 2020  >.*)".          
-00000b30: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00000b40: 206d 203d 2072 652e 6d61 7463 6828 7265   m = re.match(re
-00000b50: 6765 7870 2c20 6173 7369 676e 6d65 6e74  gexp, assignment
-00000b60: 290a 2020 2020 2020 2020 6966 206d 2069  ).        if m i
-00000b70: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00000b80: 2020 2020 7261 6973 6520 5275 6e74 696d      raise Runtim
-00000b90: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00000ba0: 2020 2020 2020 2020 2243 6f75 6c64 206e          "Could n
-00000bb0: 6f74 206d 6174 6368 2027 2573 2720 7769  ot match '%s' wi
-00000bc0: 7468 2072 6567 6578 7020 2725 7327 222c  th regexp '%s'",
-00000bd0: 2061 7373 6967 6e6d 656e 742c 2072 6567   assignment, reg
-00000be0: 6578 700a 2020 2020 2020 2020 2020 2020  exp.            
-00000bf0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00000c00: 6e20 6d2e 6772 6f75 7064 6963 7428 290a  n m.groupdict().
-00000c10: 0a20 2020 2064 6566 2070 6172 7365 5f61  .    def parse_a
-00000c20: 7373 6967 6e6d 656e 7473 2873 656c 6629  ssignments(self)
-00000c30: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00000c40: 662e 636f 7572 7365 6469 722e 7374 7564  f.coursedir.stud
-00000c50: 656e 745f 6964 3a0a 2020 2020 2020 2020  ent_id:.        
-00000c60: 2020 2020 636f 7572 7365 7320 3d20 7365      courses = se
-00000c70: 6c66 2e61 7574 6865 6e74 6963 6174 6f72  lf.authenticator
-00000c80: 2e67 6574 5f73 7475 6465 6e74 5f63 6f75  .get_student_cou
-00000c90: 7273 6573 2873 656c 662e 636f 7572 7365  rses(self.course
-00000ca0: 6469 722e 7374 7564 656e 745f 6964 290a  dir.student_id).
-00000cb0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00000cc0: 2020 2020 2020 2020 2020 636f 7572 7365            course
-00000cd0: 7320 3d20 4e6f 6e65 0a0a 2020 2020 2020  s = None..      
-00000ce0: 2020 6173 7369 676e 6d65 6e74 7320 3d20    assignments = 
-00000cf0: 5b5d 0a20 2020 2020 2020 2072 656c 6561  [].        relea
-00000d00: 7365 645f 6173 7369 676e 6d65 6e74 7320  sed_assignments 
-00000d10: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-00000d20: 2070 6174 6820 696e 2073 656c 662e 6173   path in self.as
-00000d30: 7369 676e 6d65 6e74 733a 0a20 2020 2020  signments:.     
-00000d40: 2020 2020 2020 2069 6e66 6f20 3d20 7365         info = se
-00000d50: 6c66 2e70 6172 7365 5f61 7373 6967 6e6d  lf.parse_assignm
-00000d60: 656e 7428 7061 7468 290a 2020 2020 2020  ent(path).      
-00000d70: 2020 2020 2020 2320 6966 2067 7261 6465        # if grade
-00000d80: 7220 616e 6420 7468 6520 6173 7369 676e  r and the assign
-00000d90: 6d65 6e74 2069 7320 616c 7265 6164 7920  ment is already 
-00000da0: 6b6e 6f77 6e20 6173 2072 656c 6561 7365  known as release
-00000db0: 6420 6173 7369 676e 6d65 6e74 2c20 736b  d assignment, sk
-00000dc0: 6970 206c 6f6f 6b69 6e67 0a20 2020 2020  ip looking.     
-00000dd0: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-00000de0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00000df0: 2e70 6572 736f 6e61 6c69 7a65 645f 6f75  .personalized_ou
-00000e00: 7462 6f75 6e64 0a20 2020 2020 2020 2020  tbound.         
-00000e10: 2020 2020 2020 2061 6e64 2073 656c 662e         and self.
-00000e20: 6772 6164 6572 0a20 2020 2020 2020 2020  grader.         
-00000e30: 2020 2020 2020 2061 6e64 2069 6e66 6f5b         and info[
-00000e40: 2261 7373 6967 6e6d 656e 745f 6964 225d  "assignment_id"]
-00000e50: 2069 6e20 7265 6c65 6173 6564 5f61 7373   in released_ass
-00000e60: 6967 6e6d 656e 7473 0a20 2020 2020 2020  ignments.       
-00000e70: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00000e80: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
-00000e90: 2e64 6562 7567 280a 2020 2020 2020 2020  .debug(.        
-00000ea0: 2020 2020 2020 2020 2020 2020 2247 7261              "Gra
-00000eb0: 6465 7220 726f 6c65 2061 6e64 2070 6572  der role and per
-00000ec0: 736f 6e61 6c69 7a65 642d 6f75 7462 6f75  sonalized-outbou
-00000ed0: 6e64 2061 7265 2065 6e61 626c 6564 2c20  nd are enabled, 
-00000ee0: 616e 6420 7468 6520 6173 7369 676e 6d65  and the assignme
-00000ef0: 6e74 2069 7320 6b6e 6f77 6e20 746f 2062  nt is known to b
-00000f00: 6520 7265 6c65 6173 6564 2061 6c72 6561  e released alrea
-00000f10: 6479 220a 2020 2020 2020 2020 2020 2020  dy".            
-00000f20: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00000f30: 2020 2020 2020 636f 6e74 696e 7565 0a0a        continue..
-00000f40: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00000f50: 6f75 7273 6573 2069 7320 6e6f 7420 4e6f  ourses is not No
-00000f60: 6e65 2061 6e64 2069 6e66 6f5b 2263 6f75  ne and info["cou
-00000f70: 7273 655f 6964 225d 206e 6f74 2069 6e20  rse_id"] not in 
-00000f80: 636f 7572 7365 733a 0a20 2020 2020 2020  courses:.       
-00000f90: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00000fa0: 650a 0a20 2020 2020 2020 2020 2020 2069  e..            i
-00000fb0: 6620 7365 6c66 2e70 6174 685f 696e 636c  f self.path_incl
-00000fc0: 7564 6573 5f63 6f75 7273 653a 0a20 2020  udes_course:.   
-00000fd0: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-00000fe0: 6967 6e6d 656e 745f 6469 7220 3d20 6f73  ignment_dir = os
-00000ff0: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
-00001000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001010: 7365 6c66 2e61 7373 6967 6e6d 656e 745f  self.assignment_
-00001020: 6469 722c 2069 6e66 6f5b 2263 6f75 7273  dir, info["cours
-00001030: 655f 6964 225d 2c20 696e 666f 5b22 6173  e_id"], info["as
-00001040: 7369 676e 6d65 6e74 5f69 6422 5d0a 2020  signment_id"].  
-00001050: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-00001060: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00001070: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001080: 2020 6173 7369 676e 6d65 6e74 5f64 6972    assignment_dir
-00001090: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-000010a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000010b0: 2020 2020 2073 656c 662e 6173 7369 676e       self.assign
-000010c0: 6d65 6e74 5f64 6972 2c20 696e 666f 5b22  ment_dir, info["
-000010d0: 6173 7369 676e 6d65 6e74 5f69 6422 5d0a  assignment_id"].
-000010e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010f0: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
-00001100: 6620 7365 6c66 2e69 6e62 6f75 6e64 206f  f self.inbound o
-00001110: 7220 7365 6c66 2e63 6163 6865 643a 0a20  r self.cached:. 
-00001120: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001130: 6e66 6f5b 2273 7461 7475 7322 5d20 3d20  nfo["status"] = 
-00001140: 2273 7562 6d69 7474 6564 220a 2020 2020  "submitted".    
-00001150: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00001160: 5b22 7061 7468 225d 203d 2070 6174 680a  ["path"] = path.
-00001170: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00001180: 206f 732e 7061 7468 2e65 7869 7374 7328   os.path.exists(
-00001190: 6173 7369 676e 6d65 6e74 5f64 6972 293a  assignment_dir):
-000011a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000011b0: 2069 6e66 6f5b 2273 7461 7475 7322 5d20   info["status"] 
-000011c0: 3d20 2266 6574 6368 6564 220a 2020 2020  = "fetched".    
-000011d0: 2020 2020 2020 2020 2020 2020 696e 666f              info
-000011e0: 5b22 7061 7468 225d 203d 206f 732e 7061  ["path"] = os.pa
-000011f0: 7468 2e61 6273 7061 7468 2861 7373 6967  th.abspath(assig
-00001200: 6e6d 656e 745f 6469 7229 0a20 2020 2020  nment_dir).     
-00001210: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00001220: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
-00001230: 6f5b 2273 7461 7475 7322 5d20 3d20 2272  o["status"] = "r
-00001240: 656c 6561 7365 6422 0a20 2020 2020 2020  eleased".       
-00001250: 2020 2020 2020 2020 2069 6e66 6f5b 2270           info["p
-00001260: 6174 6822 5d20 3d20 7061 7468 0a20 2020  ath"] = path.   
-00001270: 2020 2020 2020 2020 2020 2020 2023 2075               # u
-00001280: 7064 6174 6520 7265 6c65 6173 6564 2061  pdate released a
-00001290: 7373 6967 6e6d 656e 7473 0a20 2020 2020  ssignments.     
-000012a0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-000012b0: 6c66 2e70 6572 736f 6e61 6c69 7a65 645f  lf.personalized_
-000012c0: 6f75 7462 6f75 6e64 2061 6e64 2073 656c  outbound and sel
-000012d0: 662e 6772 6164 6572 3a0a 2020 2020 2020  f.grader:.      
-000012e0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000012f0: 6c65 6173 6564 5f61 7373 6967 6e6d 656e  leased_assignmen
-00001300: 7473 2e61 7070 656e 6428 696e 666f 5b22  ts.append(info["
-00001310: 6173 7369 676e 6d65 6e74 5f69 6422 5d29  assignment_id"])
-00001320: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00001330: 2073 656c 662e 7265 6d6f 7665 3a0a 2020   self.remove:.  
-00001340: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00001350: 666f 5b22 7374 6174 7573 225d 203d 2022  fo["status"] = "
-00001360: 7265 6d6f 7665 6422 0a0a 2020 2020 2020  removed"..      
-00001370: 2020 2020 2020 6e6f 7465 626f 6f6b 7320        notebooks 
-00001380: 3d20 736f 7274 6564 2867 6c6f 622e 676c  = sorted(glob.gl
-00001390: 6f62 286f 732e 7061 7468 2e6a 6f69 6e28  ob(os.path.join(
-000013a0: 696e 666f 5b22 7061 7468 225d 2c20 222a  info["path"], "*
-000013b0: 2e69 7079 6e62 2229 2929 0a20 2020 2020  .ipynb"))).     
-000013c0: 2020 2020 2020 2069 6620 6e6f 7420 6e6f         if not no
-000013d0: 7465 626f 6f6b 733a 0a20 2020 2020 2020  tebooks:.       
-000013e0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-000013f0: 672e 7761 726e 696e 6728 224e 6f20 6e6f  g.warning("No no
-00001400: 7465 626f 6f6b 7320 666f 756e 6420 696e  tebooks found in
-00001410: 207b 7d22 2e66 6f72 6d61 7428 696e 666f   {}".format(info
-00001420: 5b22 7061 7468 225d 2929 0a0a 2020 2020  ["path"]))..    
-00001430: 2020 2020 2020 2020 696e 666f 5b22 6e6f          info["no
-00001440: 7465 626f 6f6b 7322 5d20 3d20 5b5d 0a20  tebooks"] = []. 
-00001450: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
-00001460: 6f74 6562 6f6f 6b20 696e 206e 6f74 6562  otebook in noteb
-00001470: 6f6f 6b73 3a0a 2020 2020 2020 2020 2020  ooks:.          
-00001480: 2020 2020 2020 6e62 5f69 6e66 6f20 3d20        nb_info = 
-00001490: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
-000014a0: 2020 2020 2020 226e 6f74 6562 6f6f 6b5f        "notebook_
-000014b0: 6964 223a 206f 732e 7061 7468 2e73 706c  id": os.path.spl
-000014c0: 6974 6578 7428 6f73 2e70 6174 682e 7370  itext(os.path.sp
-000014d0: 6c69 7428 6e6f 7465 626f 6f6b 295b 315d  lit(notebook)[1]
-000014e0: 295b 305d 2c0a 2020 2020 2020 2020 2020  )[0],.          
-000014f0: 2020 2020 2020 2020 2020 2270 6174 6822            "path"
-00001500: 3a20 6f73 2e70 6174 682e 6162 7370 6174  : os.path.abspat
-00001510: 6828 6e6f 7465 626f 6f6b 292c 0a20 2020  h(notebook),.   
-00001520: 2020 2020 2020 2020 2020 2020 207d 0a20               }. 
-00001530: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00001540: 6620 696e 666f 5b22 7374 6174 7573 225d  f info["status"]
-00001550: 2021 3d20 2273 7562 6d69 7474 6564 223a   != "submitted":
-00001560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001570: 2020 2020 2069 6e66 6f5b 226e 6f74 6562       info["noteb
-00001580: 6f6f 6b73 225d 2e61 7070 656e 6428 6e62  ooks"].append(nb
-00001590: 5f69 6e66 6f29 0a20 2020 2020 2020 2020  _info).         
-000015a0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-000015b0: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
-000015c0: 2020 2020 206e 625f 696e 666f 5b22 6861       nb_info["ha
-000015d0: 735f 6c6f 6361 6c5f 6665 6564 6261 636b  s_local_feedback
-000015e0: 225d 203d 2046 616c 7365 0a20 2020 2020  "] = False.     
-000015f0: 2020 2020 2020 2020 2020 206e 625f 696e             nb_in
-00001600: 666f 5b22 6861 735f 6578 6368 616e 6765  fo["has_exchange
-00001610: 5f66 6565 6462 6163 6b22 5d20 3d20 4661  _feedback"] = Fa
-00001620: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00001630: 2020 2020 6e62 5f69 6e66 6f5b 226c 6f63      nb_info["loc
-00001640: 616c 5f66 6565 6462 6163 6b5f 7061 7468  al_feedback_path
-00001650: 225d 203d 204e 6f6e 650a 2020 2020 2020  "] = None.      
-00001660: 2020 2020 2020 2020 2020 6e62 5f69 6e66            nb_inf
-00001670: 6f5b 2266 6565 6462 6163 6b5f 7570 6461  o["feedback_upda
-00001680: 7465 6422 5d20 3d20 4661 6c73 650a 0a20  ted"] = False.. 
-00001690: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000016a0: 2043 6865 636b 2077 6865 7468 6572 2066   Check whether f
-000016b0: 6565 6462 6163 6b20 6861 7320 6265 656e  eedback has been
-000016c0: 2066 6574 6368 6564 2061 6c72 6561 6479   fetched already
-000016d0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000016e0: 2020 6c6f 6361 6c5f 6665 6564 6261 636b    local_feedback
-000016f0: 5f64 6972 203d 206f 732e 7061 7468 2e6a  _dir = os.path.j
-00001700: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-00001710: 2020 2020 2020 2020 2061 7373 6967 6e6d           assignm
-00001720: 656e 745f 6469 722c 2022 6665 6564 6261  ent_dir, "feedba
-00001730: 636b 222c 2069 6e66 6f5b 2274 696d 6573  ck", info["times
-00001740: 7461 6d70 225d 0a20 2020 2020 2020 2020  tamp"].         
-00001750: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00001760: 2020 2020 2020 2020 206c 6f63 616c 5f66           local_f
-00001770: 6565 6462 6163 6b5f 7061 7468 203d 206f  eedback_path = o
-00001780: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017a0: 206c 6f63 616c 5f66 6565 6462 6163 6b5f   local_feedback_
-000017b0: 6469 722c 2022 7b30 7d2e 6874 6d6c 222e  dir, "{0}.html".
-000017c0: 666f 726d 6174 286e 625f 696e 666f 5b22  format(nb_info["
-000017d0: 6e6f 7465 626f 6f6b 5f69 6422 5d29 0a20  notebook_id"]). 
-000017e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000017f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001800: 2068 6173 5f6c 6f63 616c 5f66 6565 6462   has_local_feedb
-00001810: 6163 6b20 3d20 6f73 2e70 6174 682e 6973  ack = os.path.is
-00001820: 6669 6c65 286c 6f63 616c 5f66 6565 6462  file(local_feedb
-00001830: 6163 6b5f 7061 7468 290a 2020 2020 2020  ack_path).      
-00001840: 2020 2020 2020 2020 2020 6966 2068 6173            if has
-00001850: 5f6c 6f63 616c 5f66 6565 6462 6163 6b3a  _local_feedback:
-00001860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001870: 2020 2020 206c 6f63 616c 5f66 6565 6462       local_feedb
-00001880: 6163 6b5f 6368 6563 6b73 756d 203d 205f  ack_checksum = _
-00001890: 6368 6563 6b73 756d 286c 6f63 616c 5f66  checksum(local_f
-000018a0: 6565 6462 6163 6b5f 7061 7468 290a 2020  eedback_path).  
-000018b0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-000018c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000018d0: 2020 2020 2020 2020 6c6f 6361 6c5f 6665          local_fe
-000018e0: 6564 6261 636b 5f63 6865 636b 7375 6d20  edback_checksum 
-000018f0: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
-00001900: 2020 2020 2020 2020 2320 416c 736f 206c          # Also l
-00001910: 6f6f 6b20 746f 2073 6565 2069 6620 7468  ook to see if th
-00001920: 6572 6520 6973 2066 6565 6462 6163 6b20  ere is feedback 
-00001930: 6176 6169 6c61 626c 6520 746f 2066 6574  available to fet
-00001940: 6368 2e0a 2020 2020 2020 2020 2020 2020  ch..            
-00001950: 2020 2020 2320 616e 6420 6368 6563 6b20      # and check 
-00001960: 7768 6574 6865 7220 7065 7273 6f6e 616c  whether personal
-00001970: 697a 6564 2d66 6565 6462 6163 6b20 6973  ized-feedback is
-00001980: 2065 6e61 626c 6564 0a20 2020 2020 2020   enabled.       
-00001990: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-000019a0: 2e70 6572 736f 6e61 6c69 7a65 645f 6665  .personalized_fe
-000019b0: 6564 6261 636b 3a0a 2020 2020 2020 2020  edback:.        
-000019c0: 2020 2020 2020 2020 2020 2020 6578 6368              exch
-000019d0: 616e 6765 5f66 6565 6462 6163 6b5f 7061  ange_feedback_pa
-000019e0: 7468 203d 206f 732e 7061 7468 2e6a 6f69  th = os.path.joi
-000019f0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00001a00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00001a10: 726f 6f74 2c0a 2020 2020 2020 2020 2020  root,.          
-00001a20: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00001a30: 666f 5b22 636f 7572 7365 5f69 6422 5d2c  fo["course_id"],
-00001a40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001a50: 2020 2020 2020 2020 2073 656c 662e 6665           self.fe
-00001a60: 6564 6261 636b 5f64 6972 6563 746f 7279  edback_directory
-00001a70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001a80: 2020 2020 2020 2020 2020 696e 666f 5b22            info["
-00001a90: 7374 7564 656e 745f 6964 225d 2c0a 2020  student_id"],.  
-00001aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ab0: 2020 2020 2020 696e 666f 5b22 6173 7369        info["assi
-00001ac0: 676e 6d65 6e74 5f69 6422 5d2c 0a20 2020  gnment_id"],.   
-00001ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ae0: 2020 2020 2022 7b30 7d2e 6874 6d6c 222e       "{0}.html".
-00001af0: 666f 726d 6174 286e 625f 696e 666f 5b22  format(nb_info["
-00001b00: 6e6f 7465 626f 6f6b 5f69 6422 5d29 2c0a  notebook_id"]),.
+00000000: 0000 0000 0000 0000 0100 0000 0000 0000  ................
+00000010: 0b00 0000 0000 0000 4c69 6e65 546f 6f4c  ........LineTooL
+00000020: 6f6e 6724 0000 0000 0000 004c 696e 6520  ong$.......Line 
+00000030: 746f 6f20 6c6f 6e67 2028 3130 3520 3e20  too long (105 > 
+00000040: 3130 3020 6368 6172 6163 7465 7273 2900  100 characters).
+00000050: aa09 0000 af09 0000 0000 0000 0000 0000  ................
+00000060: 00aa 0900 0001 0000 0000 0000 0042 0000  .............B..
+00000070: 0000 0000 002f 686f 6d65 2f6e 6172 662f  ...../home/narf/
+00000080: 5072 6f6a 6563 7473 2f65 3278 2f72 6570  Projects/e2x/rep
+00000090: 6f73 2f65 3278 6772 6164 6572 2f65 3278  os/e2xgrader/e2x
+000000a0: 6772 6164 6572 2f65 7863 6861 6e67 652f  grader/exchange/
+000000b0: 6c69 7374 2e70 797d 2b00 0000 0000 0069  list.py}+......i
+000000c0: 6d70 6f72 7420 676c 6f62 0a69 6d70 6f72  mport glob.impor
+000000d0: 7420 6861 7368 6c69 620a 696d 706f 7274  t hashlib.import
+000000e0: 206f 730a 696d 706f 7274 2072 650a 0a66   os.import re..f
+000000f0: 726f 6d20 6e62 6772 6164 6572 2e65 7863  rom nbgrader.exc
+00000100: 6861 6e67 652e 6465 6661 756c 7420 696d  hange.default im
+00000110: 706f 7274 2045 7863 6861 6e67 654c 6973  port ExchangeLis
+00000120: 740a 6672 6f6d 206e 6267 7261 6465 722e  t.from nbgrader.
+00000130: 7574 696c 7320 696d 706f 7274 206d 616b  utils import mak
+00000140: 655f 756e 6971 7565 5f6b 6579 2c20 6e6f  e_unique_key, no
+00000150: 7465 626f 6f6b 5f68 6173 680a 0a66 726f  tebook_hash..fro
+00000160: 6d20 2e65 7863 6861 6e67 6520 696d 706f  m .exchange impo
+00000170: 7274 2045 3278 4578 6368 616e 6765 0a0a  rt E2xExchange..
+00000180: 0a64 6566 205f 6368 6563 6b73 756d 2870  .def _checksum(p
+00000190: 6174 6829 3a0a 2020 2020 6d20 3d20 6861  ath):.    m = ha
+000001a0: 7368 6c69 622e 6d64 3528 290a 2020 2020  shlib.md5().    
+000001b0: 6d2e 7570 6461 7465 286f 7065 6e28 7061  m.update(open(pa
+000001c0: 7468 2c20 2272 6222 292e 7265 6164 2829  th, "rb").read()
+000001d0: 290a 2020 2020 7265 7475 726e 206d 2e68  ).    return m.h
+000001e0: 6578 6469 6765 7374 2829 0a0a 0a64 6566  exdigest()...def
+000001f0: 205f 6765 745f 6b65 7928 696e 666f 293a   _get_key(info):
+00000200: 0a20 2020 2072 6574 7572 6e20 696e 666f  .    return info
+00000210: 5b22 636f 7572 7365 5f69 6422 5d2c 2069  ["course_id"], i
+00000220: 6e66 6f5b 2273 7475 6465 6e74 5f69 6422  nfo["student_id"
+00000230: 5d2c 2069 6e66 6f5b 2261 7373 6967 6e6d  ], info["assignm
+00000240: 656e 745f 6964 225d 0a0a 0a64 6566 205f  ent_id"]...def _
+00000250: 6d61 7463 685f 6b65 7928 696e 666f 2c20  match_key(info, 
+00000260: 6b65 7929 3a0a 2020 2020 7265 7475 726e  key):.    return
+00000270: 2028 0a20 2020 2020 2020 2069 6e66 6f5b   (.        info[
+00000280: 2263 6f75 7273 655f 6964 225d 203d 3d20  "course_id"] == 
+00000290: 6b65 795b 305d 0a20 2020 2020 2020 2061  key[0].        a
+000002a0: 6e64 2069 6e66 6f5b 2273 7475 6465 6e74  nd info["student
+000002b0: 5f69 6422 5d20 3d3d 206b 6579 5b31 5d0a  _id"] == key[1].
+000002c0: 2020 2020 2020 2020 616e 6420 696e 666f          and info
+000002d0: 5b22 6173 7369 676e 6d65 6e74 5f69 6422  ["assignment_id"
+000002e0: 5d20 3d3d 206b 6579 5b32 5d0a 2020 2020  ] == key[2].    
+000002f0: 290a 0a0a 636c 6173 7320 4532 7845 7863  )...class E2xExc
+00000300: 6861 6e67 654c 6973 7428 4532 7845 7863  hangeList(E2xExc
+00000310: 6861 6e67 652c 2045 7863 6861 6e67 654c  hange, ExchangeL
+00000320: 6973 7429 3a0a 2020 2020 6465 6620 696e  ist):.    def in
+00000330: 6974 5f64 6573 7428 7365 6c66 293a 0a20  it_dest(self):. 
+00000340: 2020 2020 2020 2063 6f75 7273 655f 6964         course_id
+00000350: 203d 2073 656c 662e 636f 7572 7365 6469   = self.coursedi
+00000360: 722e 636f 7572 7365 5f69 6420 6966 2073  r.course_id if s
+00000370: 656c 662e 636f 7572 7365 6469 722e 636f  elf.coursedir.co
+00000380: 7572 7365 5f69 6420 656c 7365 2022 2a22  urse_id else "*"
+00000390: 0a20 2020 2020 2020 2061 7373 6967 6e6d  .        assignm
+000003a0: 656e 745f 6964 203d 2028 0a20 2020 2020  ent_id = (.     
+000003b0: 2020 2020 2020 2073 656c 662e 636f 7572         self.cour
+000003c0: 7365 6469 722e 6173 7369 676e 6d65 6e74  sedir.assignment
+000003d0: 5f69 6420 6966 2073 656c 662e 636f 7572  _id if self.cour
+000003e0: 7365 6469 722e 6173 7369 676e 6d65 6e74  sedir.assignment
+000003f0: 5f69 6420 656c 7365 2022 2a22 0a20 2020  _id else "*".   
+00000400: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00000410: 7475 6465 6e74 5f69 6420 3d20 7365 6c66  tudent_id = self
+00000420: 2e63 6f75 7273 6564 6972 2e73 7475 6465  .coursedir.stude
+00000430: 6e74 5f69 6420 6966 2073 656c 662e 636f  nt_id if self.co
+00000440: 7572 7365 6469 722e 7374 7564 656e 745f  ursedir.student_
+00000450: 6964 2065 6c73 6520 222a 220a 0a20 2020  id else "*"..   
+00000460: 2020 2020 2069 6620 7365 6c66 2e69 6e62       if self.inb
+00000470: 6f75 6e64 3a0a 2020 2020 2020 2020 2020  ound:.          
+00000480: 2020 7061 7474 6572 6e20 3d20 6f73 2e70    pattern = os.p
+00000490: 6174 682e 6a6f 696e 280a 2020 2020 2020  ath.join(.      
+000004a0: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+000004b0: 6f6f 742c 0a20 2020 2020 2020 2020 2020  oot,.           
+000004c0: 2020 2020 2063 6f75 7273 655f 6964 2c0a       course_id,.
+000004d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004e0: 7365 6c66 2e69 6e62 6f75 6e64 5f64 6972  self.inbound_dir
+000004f0: 6563 746f 7279 2c0a 2020 2020 2020 2020  ectory,.        
+00000500: 2020 2020 2020 2020 227b 7d2b 7b7d 2b2a          "{}+{}+*
+00000510: 222e 666f 726d 6174 2873 7475 6465 6e74  ".format(student
+00000520: 5f69 642c 2061 7373 6967 6e6d 656e 745f  _id, assignment_
+00000530: 6964 292c 0a20 2020 2020 2020 2020 2020  id),.           
+00000540: 2029 0a20 2020 2020 2020 2065 6c69 6620   ).        elif 
+00000550: 7365 6c66 2e63 6163 6865 643a 0a20 2020  self.cached:.   
+00000560: 2020 2020 2020 2020 2070 6174 7465 726e           pattern
+00000570: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+00000580: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000590: 2073 656c 662e 6361 6368 652c 2063 6f75   self.cache, cou
+000005a0: 7273 655f 6964 2c20 227b 7d2b 7b7d 2b2a  rse_id, "{}+{}+*
+000005b0: 222e 666f 726d 6174 2873 7475 6465 6e74  ".format(student
+000005c0: 5f69 642c 2061 7373 6967 6e6d 656e 745f  _id, assignment_
+000005d0: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
+000005e0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+000005f0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+00000600: 656c 662e 7065 7273 6f6e 616c 697a 6564  elf.personalized
+00000610: 5f6f 7574 626f 756e 643a 0a20 2020 2020  _outbound:.     
+00000620: 2020 2020 2020 2020 2020 2023 206c 6973             # lis
+00000630: 7420 616c 6c20 6173 7369 676e 6d65 6e74  t all assignment
+00000640: 7320 6865 7265 0a20 2020 2020 2020 2020  s here.         
+00000650: 2020 2020 2020 2070 6174 7465 726e 203d         pattern =
+00000660: 206f 732e 7061 7468 2e6a 6f69 6e28 0a20   os.path.join(. 
+00000670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000680: 2020 2073 656c 662e 726f 6f74 2c0a 2020     self.root,.  
+00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006a0: 2020 636f 7572 7365 5f69 642c 0a20 2020    course_id,.   
+000006b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000006c0: 2073 656c 662e 6f75 7462 6f75 6e64 5f64   self.outbound_d
+000006d0: 6972 6563 746f 7279 2c0a 2020 2020 2020  irectory,.      
+000006e0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+000006f0: 7564 656e 745f 6964 2c0a 2020 2020 2020  udent_id,.      
+00000700: 2020 2020 2020 2020 2020 2020 2020 227b                "{
+00000710: 7d22 2e66 6f72 6d61 7428 6173 7369 676e  }".format(assign
+00000720: 6d65 6e74 5f69 6429 2c0a 2020 2020 2020  ment_id),.      
+00000730: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00000740: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00000750: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00000760: 7474 6572 6e20 3d20 6f73 2e70 6174 682e  ttern = os.path.
+00000770: 6a6f 696e 280a 2020 2020 2020 2020 2020  join(.          
+00000780: 2020 2020 2020 2020 2020 7365 6c66 2e72            self.r
+00000790: 6f6f 742c 0a20 2020 2020 2020 2020 2020  oot,.           
+000007a0: 2020 2020 2020 2020 2063 6f75 7273 655f           course_
+000007b0: 6964 2c0a 2020 2020 2020 2020 2020 2020  id,.            
+000007c0: 2020 2020 2020 2020 7365 6c66 2e6f 7574          self.out
+000007d0: 626f 756e 645f 6469 7265 6374 6f72 792c  bound_directory,
+000007e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000007f0: 2020 2020 2022 7b7d 222e 666f 726d 6174       "{}".format
+00000800: 2861 7373 6967 6e6d 656e 745f 6964 292c  (assignment_id),
+00000810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000820: 2029 0a0a 2020 2020 2020 2020 7365 6c66   )..        self
+00000830: 2e61 7373 6967 6e6d 656e 7473 203d 2073  .assignments = s
+00000840: 6f72 7465 6428 676c 6f62 2e67 6c6f 6228  orted(glob.glob(
+00000850: 7061 7474 6572 6e29 290a 0a20 2020 2064  pattern))..    d
+00000860: 6566 2070 6172 7365 5f61 7373 6967 6e6d  ef parse_assignm
+00000870: 656e 7428 7365 6c66 2c20 6173 7369 676e  ent(self, assign
+00000880: 6d65 6e74 293a 0a20 2020 2020 2020 2063  ment):.        c
+00000890: 6f75 7273 655f 6964 203d 2072 222e 2a2f  ourse_id = r".*/
+000008a0: 283f 503c 636f 7572 7365 5f69 643e 2e2a  (?P<course_id>.*
+000008b0: 292f 220a 2020 2020 2020 2020 6966 2073  )/".        if s
+000008c0: 656c 662e 696e 626f 756e 643a 0a20 2020  elf.inbound:.   
+000008d0: 2020 2020 2020 2020 2072 6567 6578 7020           regexp 
+000008e0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+000008f0: 2020 2020 636f 7572 7365 5f69 640a 2020      course_id.  
+00000900: 2020 2020 2020 2020 2020 2020 2020 2b20                + 
+00000910: 7365 6c66 2e69 6e62 6f75 6e64 5f64 6972  self.inbound_dir
+00000920: 6563 746f 7279 0a20 2020 2020 2020 2020  ectory.         
+00000930: 2020 2020 2020 202b 2072 222f 283f 503c         + r"/(?P<
+00000940: 7374 7564 656e 745f 6964 3e5b 5e2b 5d2a  student_id>[^+]*
+00000950: 295c 2b22 0a20 2020 2020 2020 2020 2020  )\+".           
+00000960: 2020 2020 202b 2072 2228 3f50 3c61 7373       + r"(?P<ass
+00000970: 6967 6e6d 656e 745f 6964 3e5b 5e2b 5d2a  ignment_id>[^+]*
+00000980: 295c 2b22 0a20 2020 2020 2020 2020 2020  )\+".           
+00000990: 2020 2020 202b 2072 2228 3f50 3c74 696d       + r"(?P<tim
+000009a0: 6573 7461 6d70 3e5b 5e2b 5d2a 2922 0a20  estamp>[^+]*)". 
+000009b0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+000009c0: 2072 2228 3f50 3c72 616e 646f 6d5f 7374   r"(?P<random_st
+000009d0: 7269 6e67 3e5c 2b2e 2a29 3f22 0a20 2020  ring>\+.*)?".   
+000009e0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000009f0: 2020 2065 6c69 6620 7365 6c66 2e63 6163     elif self.cac
+00000a00: 6865 643a 0a20 2020 2020 2020 2020 2020  hed:.           
+00000a10: 2072 6567 6578 7020 3d20 7222 2e2a 2f28   regexp = r".*/(
+00000a20: 3f50 3c63 6f75 7273 655f 6964 3e2e 2a29  ?P<course_id>.*)
+00000a30: 2f28 3f50 3c73 7475 6465 6e74 5f69 643e  /(?P<student_id>
+00000a40: 2e2a 295c 2b28 3f50 3c61 7373 6967 6e6d  .*)\+(?P<assignm
+00000a50: 656e 745f 6964 3e2e 2a29 5c2b 283f 503c  ent_id>.*)\+(?P<
+00000a60: 7469 6d65 7374 616d 703e 2e2a 2922 0a20  timestamp>.*)". 
+00000a70: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00000a80: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00000a90: 2e70 6572 736f 6e61 6c69 7a65 645f 6f75  .personalized_ou
+00000aa0: 7462 6f75 6e64 3a0a 2020 2020 2020 2020  tbound:.        
+00000ab0: 2020 2020 2020 2020 7265 6765 7870 203d          regexp =
+00000ac0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+00000ad0: 2020 2020 2020 2063 6f75 7273 655f 6964         course_id
+00000ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00000af0: 2020 2020 202b 2073 656c 662e 6f75 7462       + self.outb
+00000b00: 6f75 6e64 5f64 6972 6563 746f 7279 0a20  ound_directory. 
+00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b20: 2020 202b 2072 222f 283f 503c 7374 7564     + r"/(?P<stud
+00000b30: 656e 745f 6964 3e2e 2a29 220a 2020 2020  ent_id>.*)".    
+00000b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b50: 2b20 7222 2f28 3f50 3c61 7373 6967 6e6d  + r"/(?P<assignm
+00000b60: 656e 745f 6964 3e2e 2a29 220a 2020 2020  ent_id>.*)".    
+00000b70: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00000b80: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00000b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000ba0: 7265 6765 7870 203d 2063 6f75 7273 655f  regexp = course_
+00000bb0: 6964 202b 2073 656c 662e 6f75 7462 6f75  id + self.outbou
+00000bc0: 6e64 5f64 6972 6563 746f 7279 202b 2072  nd_directory + r
+00000bd0: 222f 283f 503c 6173 7369 676e 6d65 6e74  "/(?P<assignment
+00000be0: 5f69 643e 2e2a 2922 0a0a 2020 2020 2020  _id>.*)"..      
+00000bf0: 2020 6d20 3d20 7265 2e6d 6174 6368 2872    m = re.match(r
+00000c00: 6567 6578 702c 2061 7373 6967 6e6d 656e  egexp, assignmen
+00000c10: 7429 0a20 2020 2020 2020 2069 6620 6d20  t).        if m 
+00000c20: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00000c30: 2020 2020 2072 6169 7365 2052 756e 7469       raise Runti
+00000c40: 6d65 4572 726f 7228 0a20 2020 2020 2020  meError(.       
+00000c50: 2020 2020 2020 2020 2022 436f 756c 6420           "Could 
+00000c60: 6e6f 7420 6d61 7463 6820 2725 7327 2077  not match '%s' w
+00000c70: 6974 6820 7265 6765 7870 2027 2573 2722  ith regexp '%s'"
+00000c80: 2c20 6173 7369 676e 6d65 6e74 2c20 7265  , assignment, re
+00000c90: 6765 7870 0a20 2020 2020 2020 2020 2020  gexp.           
+00000ca0: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
+00000cb0: 726e 206d 2e67 726f 7570 6469 6374 2829  rn m.groupdict()
+00000cc0: 0a0a 2020 2020 6465 6620 7061 7273 655f  ..    def parse_
+00000cd0: 6173 7369 676e 6d65 6e74 7328 7365 6c66  assignments(self
+00000ce0: 293a 0a20 2020 2020 2020 2069 6620 7365  ):.        if se
+00000cf0: 6c66 2e63 6f75 7273 6564 6972 2e73 7475  lf.coursedir.stu
+00000d00: 6465 6e74 5f69 643a 0a20 2020 2020 2020  dent_id:.       
+00000d10: 2020 2020 2063 6f75 7273 6573 203d 2073       courses = s
+00000d20: 656c 662e 6175 7468 656e 7469 6361 746f  elf.authenticato
+00000d30: 722e 6765 745f 7374 7564 656e 745f 636f  r.get_student_co
+00000d40: 7572 7365 7328 7365 6c66 2e63 6f75 7273  urses(self.cours
+00000d50: 6564 6972 2e73 7475 6465 6e74 5f69 6429  edir.student_id)
+00000d60: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00000d70: 2020 2020 2020 2020 2020 2063 6f75 7273             cours
+00000d80: 6573 203d 204e 6f6e 650a 0a20 2020 2020  es = None..     
+00000d90: 2020 2061 7373 6967 6e6d 656e 7473 203d     assignments =
+00000da0: 205b 5d0a 2020 2020 2020 2020 7265 6c65   [].        rele
+00000db0: 6173 6564 5f61 7373 6967 6e6d 656e 7473  ased_assignments
+00000dc0: 203d 205b 5d0a 2020 2020 2020 2020 666f   = [].        fo
+00000dd0: 7220 7061 7468 2069 6e20 7365 6c66 2e61  r path in self.a
+00000de0: 7373 6967 6e6d 656e 7473 3a0a 2020 2020  ssignments:.    
+00000df0: 2020 2020 2020 2020 696e 666f 203d 2073          info = s
+00000e00: 656c 662e 7061 7273 655f 6173 7369 676e  elf.parse_assign
+00000e10: 6d65 6e74 2870 6174 6829 0a20 2020 2020  ment(path).     
+00000e20: 2020 2020 2020 2023 2069 6620 6772 6164         # if grad
+00000e30: 6572 2061 6e64 2074 6865 2061 7373 6967  er and the assig
+00000e40: 6e6d 656e 7420 6973 2061 6c72 6561 6479  nment is already
+00000e50: 206b 6e6f 776e 2061 7320 7265 6c65 6173   known as releas
+00000e60: 6564 2061 7373 6967 6e6d 656e 742c 2073  ed assignment, s
+00000e70: 6b69 7020 6c6f 6f6b 696e 670a 2020 2020  kip looking.    
+00000e80: 2020 2020 2020 2020 6966 2028 0a20 2020          if (.   
+00000e90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00000ea0: 662e 7065 7273 6f6e 616c 697a 6564 5f6f  f.personalized_o
+00000eb0: 7574 626f 756e 640a 2020 2020 2020 2020  utbound.        
+00000ec0: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
+00000ed0: 2e67 7261 6465 720a 2020 2020 2020 2020  .grader.        
+00000ee0: 2020 2020 2020 2020 616e 6420 696e 666f          and info
+00000ef0: 5b22 6173 7369 676e 6d65 6e74 5f69 6422  ["assignment_id"
+00000f00: 5d20 696e 2072 656c 6561 7365 645f 6173  ] in released_as
+00000f10: 7369 676e 6d65 6e74 730a 2020 2020 2020  signments.      
+00000f20: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+00000f30: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+00000f40: 672e 6465 6275 6728 0a20 2020 2020 2020  g.debug(.       
+00000f50: 2020 2020 2020 2020 2020 2020 2022 4772               "Gr
+00000f60: 6164 6572 2072 6f6c 6520 616e 6420 7065  ader role and pe
+00000f70: 7273 6f6e 616c 697a 6564 2d6f 7574 626f  rsonalized-outbo
+00000f80: 756e 6420 6172 6520 656e 6162 6c65 642c  und are enabled,
+00000f90: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00000fa0: 2020 2020 2020 2022 616e 6420 7468 6520         "and the 
+00000fb0: 6173 7369 676e 6d65 6e74 2069 7320 6b6e  assignment is kn
+00000fc0: 6f77 6e20 746f 2062 6520 7265 6c65 6173  own to be releas
+00000fd0: 6564 2061 6c72 6561 6479 220a 2020 2020  ed already".    
+00000fe0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00000ff0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00001000: 6e74 696e 7565 0a0a 2020 2020 2020 2020  ntinue..        
+00001010: 2020 2020 6966 2063 6f75 7273 6573 2069      if courses i
+00001020: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2069  s not None and i
+00001030: 6e66 6f5b 2263 6f75 7273 655f 6964 225d  nfo["course_id"]
+00001040: 206e 6f74 2069 6e20 636f 7572 7365 733a   not in courses:
+00001050: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001060: 2063 6f6e 7469 6e75 650a 0a20 2020 2020   continue..     
+00001070: 2020 2020 2020 2069 6620 7365 6c66 2e70         if self.p
+00001080: 6174 685f 696e 636c 7564 6573 5f63 6f75  ath_includes_cou
+00001090: 7273 653a 0a20 2020 2020 2020 2020 2020  rse:.           
+000010a0: 2020 2020 2061 7373 6967 6e6d 656e 745f       assignment_
+000010b0: 6469 7220 3d20 6f73 2e70 6174 682e 6a6f  dir = os.path.jo
+000010c0: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+000010d0: 2020 2020 2020 2020 7365 6c66 2e61 7373          self.ass
+000010e0: 6967 6e6d 656e 745f 6469 722c 2069 6e66  ignment_dir, inf
+000010f0: 6f5b 2263 6f75 7273 655f 6964 225d 2c20  o["course_id"], 
+00001100: 696e 666f 5b22 6173 7369 676e 6d65 6e74  info["assignment
+00001110: 5f69 6422 5d0a 2020 2020 2020 2020 2020  _id"].          
+00001120: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00001130: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00001140: 2020 2020 2020 2020 2020 6173 7369 676e            assign
+00001150: 6d65 6e74 5f64 6972 203d 206f 732e 7061  ment_dir = os.pa
+00001160: 7468 2e6a 6f69 6e28 0a20 2020 2020 2020  th.join(.       
+00001170: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00001180: 662e 6173 7369 676e 6d65 6e74 5f64 6972  f.assignment_dir
+00001190: 2c20 696e 666f 5b22 6173 7369 676e 6d65  , info["assignme
+000011a0: 6e74 5f69 6422 5d0a 2020 2020 2020 2020  nt_id"].        
+000011b0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+000011c0: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+000011d0: 6e62 6f75 6e64 206f 7220 7365 6c66 2e63  nbound or self.c
+000011e0: 6163 6865 643a 0a20 2020 2020 2020 2020  ached:.         
+000011f0: 2020 2020 2020 2069 6e66 6f5b 2273 7461         info["sta
+00001200: 7475 7322 5d20 3d20 2273 7562 6d69 7474  tus"] = "submitt
+00001210: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
+00001220: 2020 2020 696e 666f 5b22 7061 7468 225d      info["path"]
+00001230: 203d 2070 6174 680a 2020 2020 2020 2020   = path.        
+00001240: 2020 2020 656c 6966 206f 732e 7061 7468      elif os.path
+00001250: 2e65 7869 7374 7328 6173 7369 676e 6d65  .exists(assignme
+00001260: 6e74 5f64 6972 293a 0a20 2020 2020 2020  nt_dir):.       
+00001270: 2020 2020 2020 2020 2069 6e66 6f5b 2273           info["s
+00001280: 7461 7475 7322 5d20 3d20 2266 6574 6368  tatus"] = "fetch
+00001290: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
+000012a0: 2020 2020 696e 666f 5b22 7061 7468 225d      info["path"]
+000012b0: 203d 206f 732e 7061 7468 2e61 6273 7061   = os.path.abspa
+000012c0: 7468 2861 7373 6967 6e6d 656e 745f 6469  th(assignment_di
+000012d0: 7229 0a20 2020 2020 2020 2020 2020 2065  r).            e
+000012e0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+000012f0: 2020 2020 2069 6e66 6f5b 2273 7461 7475       info["statu
+00001300: 7322 5d20 3d20 2272 656c 6561 7365 6422  s"] = "released"
+00001310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001320: 2069 6e66 6f5b 2270 6174 6822 5d20 3d20   info["path"] = 
+00001330: 7061 7468 0a20 2020 2020 2020 2020 2020  path.           
+00001340: 2020 2020 2023 2075 7064 6174 6520 7265       # update re
+00001350: 6c65 6173 6564 2061 7373 6967 6e6d 656e  leased assignmen
+00001360: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
+00001370: 2020 2069 6620 7365 6c66 2e70 6572 736f     if self.perso
+00001380: 6e61 6c69 7a65 645f 6f75 7462 6f75 6e64  nalized_outbound
+00001390: 2061 6e64 2073 656c 662e 6772 6164 6572   and self.grader
+000013a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000013b0: 2020 2020 2020 7265 6c65 6173 6564 5f61        released_a
+000013c0: 7373 6967 6e6d 656e 7473 2e61 7070 656e  ssignments.appen
+000013d0: 6428 696e 666f 5b22 6173 7369 676e 6d65  d(info["assignme
+000013e0: 6e74 5f69 6422 5d29 0a0a 2020 2020 2020  nt_id"])..      
+000013f0: 2020 2020 2020 6966 2073 656c 662e 7265        if self.re
+00001400: 6d6f 7665 3a0a 2020 2020 2020 2020 2020  move:.          
+00001410: 2020 2020 2020 696e 666f 5b22 7374 6174        info["stat
+00001420: 7573 225d 203d 2022 7265 6d6f 7665 6422  us"] = "removed"
+00001430: 0a0a 2020 2020 2020 2020 2020 2020 6e6f  ..            no
+00001440: 7465 626f 6f6b 7320 3d20 736f 7274 6564  tebooks = sorted
+00001450: 2867 6c6f 622e 676c 6f62 286f 732e 7061  (glob.glob(os.pa
+00001460: 7468 2e6a 6f69 6e28 696e 666f 5b22 7061  th.join(info["pa
+00001470: 7468 225d 2c20 222a 2e69 7079 6e62 2229  th"], "*.ipynb")
+00001480: 2929 0a20 2020 2020 2020 2020 2020 2069  )).            i
+00001490: 6620 6e6f 7420 6e6f 7465 626f 6f6b 733a  f not notebooks:
+000014a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000014b0: 2073 656c 662e 6c6f 672e 7761 726e 696e   self.log.warnin
+000014c0: 6728 224e 6f20 6e6f 7465 626f 6f6b 7320  g("No notebooks 
+000014d0: 666f 756e 6420 696e 207b 7d22 2e66 6f72  found in {}".for
+000014e0: 6d61 7428 696e 666f 5b22 7061 7468 225d  mat(info["path"]
+000014f0: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+00001500: 696e 666f 5b22 6e6f 7465 626f 6f6b 7322  info["notebooks"
+00001510: 5d20 3d20 5b5d 0a20 2020 2020 2020 2020  ] = [].         
+00001520: 2020 2066 6f72 206e 6f74 6562 6f6f 6b20     for notebook 
+00001530: 696e 206e 6f74 6562 6f6f 6b73 3a0a 2020  in notebooks:.  
+00001540: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
+00001550: 5f69 6e66 6f20 3d20 7b0a 2020 2020 2020  _info = {.      
+00001560: 2020 2020 2020 2020 2020 2020 2020 226e                "n
+00001570: 6f74 6562 6f6f 6b5f 6964 223a 206f 732e  otebook_id": os.
+00001580: 7061 7468 2e73 706c 6974 6578 7428 6f73  path.splitext(os
+00001590: 2e70 6174 682e 7370 6c69 7428 6e6f 7465  .path.split(note
+000015a0: 626f 6f6b 295b 315d 295b 305d 2c0a 2020  book)[1])[0],.  
+000015b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000015c0: 2020 2270 6174 6822 3a20 6f73 2e70 6174    "path": os.pat
+000015d0: 682e 6162 7370 6174 6828 6e6f 7465 626f  h.abspath(notebo
+000015e0: 6f6b 292c 0a20 2020 2020 2020 2020 2020  ok),.           
+000015f0: 2020 2020 207d 0a20 2020 2020 2020 2020       }.         
+00001600: 2020 2020 2020 2069 6620 696e 666f 5b22         if info["
+00001610: 7374 6174 7573 225d 2021 3d20 2273 7562  status"] != "sub
+00001620: 6d69 7474 6564 223a 0a20 2020 2020 2020  mitted":.       
+00001630: 2020 2020 2020 2020 2020 2020 2069 6e66               inf
+00001640: 6f5b 226e 6f74 6562 6f6f 6b73 225d 2e61  o["notebooks"].a
+00001650: 7070 656e 6428 6e62 5f69 6e66 6f29 0a20  ppend(nb_info). 
+00001660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001670: 2020 2063 6f6e 7469 6e75 650a 0a20 2020     continue..   
+00001680: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
+00001690: 696e 666f 5b22 6861 735f 6c6f 6361 6c5f  info["has_local_
+000016a0: 6665 6564 6261 636b 225d 203d 2046 616c  feedback"] = Fal
+000016b0: 7365 0a20 2020 2020 2020 2020 2020 2020  se.             
+000016c0: 2020 206e 625f 696e 666f 5b22 6861 735f     nb_info["has_
+000016d0: 6578 6368 616e 6765 5f66 6565 6462 6163  exchange_feedbac
+000016e0: 6b22 5d20 3d20 4661 6c73 650a 2020 2020  k"] = False.    
+000016f0: 2020 2020 2020 2020 2020 2020 6e62 5f69              nb_i
+00001700: 6e66 6f5b 226c 6f63 616c 5f66 6565 6462  nfo["local_feedb
+00001710: 6163 6b5f 7061 7468 225d 203d 204e 6f6e  ack_path"] = Non
+00001720: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00001730: 2020 6e62 5f69 6e66 6f5b 2266 6565 6462    nb_info["feedb
+00001740: 6163 6b5f 7570 6461 7465 6422 5d20 3d20  ack_updated"] = 
+00001750: 4661 6c73 650a 0a20 2020 2020 2020 2020  False..         
+00001760: 2020 2020 2020 2023 2043 6865 636b 2077         # Check w
+00001770: 6865 7468 6572 2066 6565 6462 6163 6b20  hether feedback 
+00001780: 6861 7320 6265 656e 2066 6574 6368 6564  has been fetched
+00001790: 2061 6c72 6561 6479 2e0a 2020 2020 2020   already..      
+000017a0: 2020 2020 2020 2020 2020 6c6f 6361 6c5f            local_
+000017b0: 6665 6564 6261 636b 5f64 6972 203d 206f  feedback_dir = o
+000017c0: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+000017d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017e0: 2061 7373 6967 6e6d 656e 745f 6469 722c   assignment_dir,
+000017f0: 2022 6665 6564 6261 636b 222c 2069 6e66   "feedback", inf
+00001800: 6f5b 2274 696d 6573 7461 6d70 225d 0a20  o["timestamp"]. 
+00001810: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00001820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001830: 206c 6f63 616c 5f66 6565 6462 6163 6b5f   local_feedback_
+00001840: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+00001850: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+00001860: 2020 2020 2020 2020 206c 6f63 616c 5f66           local_f
+00001870: 6565 6462 6163 6b5f 6469 722c 2022 7b30  eedback_dir, "{0
+00001880: 7d2e 6874 6d6c 222e 666f 726d 6174 286e  }.html".format(n
+00001890: 625f 696e 666f 5b22 6e6f 7465 626f 6f6b  b_info["notebook
+000018a0: 5f69 6422 5d29 0a20 2020 2020 2020 2020  _id"]).         
+000018b0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+000018c0: 2020 2020 2020 2020 2068 6173 5f6c 6f63           has_loc
+000018d0: 616c 5f66 6565 6462 6163 6b20 3d20 6f73  al_feedback = os
+000018e0: 2e70 6174 682e 6973 6669 6c65 286c 6f63  .path.isfile(loc
+000018f0: 616c 5f66 6565 6462 6163 6b5f 7061 7468  al_feedback_path
+00001900: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00001910: 2020 6966 2068 6173 5f6c 6f63 616c 5f66    if has_local_f
+00001920: 6565 6462 6163 6b3a 0a20 2020 2020 2020  eedback:.       
+00001930: 2020 2020 2020 2020 2020 2020 206c 6f63               loc
+00001940: 616c 5f66 6565 6462 6163 6b5f 6368 6563  al_feedback_chec
+00001950: 6b73 756d 203d 205f 6368 6563 6b73 756d  ksum = _checksum
+00001960: 286c 6f63 616c 5f66 6565 6462 6163 6b5f  (local_feedback_
+00001970: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+00001980: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00001990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019a0: 6c6f 6361 6c5f 6665 6564 6261 636b 5f63  local_feedback_c
+000019b0: 6865 636b 7375 6d20 3d20 4e6f 6e65 0a0a  hecksum = None..
+000019c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019d0: 2320 416c 736f 206c 6f6f 6b20 746f 2073  # Also look to s
+000019e0: 6565 2069 6620 7468 6572 6520 6973 2066  ee if there is f
+000019f0: 6565 6462 6163 6b20 6176 6169 6c61 626c  eedback availabl
+00001a00: 6520 746f 2066 6574 6368 2e0a 2020 2020  e to fetch..    
+00001a10: 2020 2020 2020 2020 2020 2020 2320 616e              # an
+00001a20: 6420 6368 6563 6b20 7768 6574 6865 7220  d check whether 
+00001a30: 7065 7273 6f6e 616c 697a 6564 2d66 6565  personalized-fee
+00001a40: 6462 6163 6b20 6973 2065 6e61 626c 6564  dback is enabled
+00001a50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001a60: 2069 6620 7365 6c66 2e70 6572 736f 6e61   if self.persona
+00001a70: 6c69 7a65 645f 6665 6564 6261 636b 3a0a  lized_feedback:.
+00001a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a90: 2020 2020 6578 6368 616e 6765 5f66 6565      exchange_fee
+00001aa0: 6462 6163 6b5f 7061 7468 203d 206f 732e  dback_path = os.
+00001ab0: 7061 7468 2e6a 6f69 6e28 0a20 2020 2020  path.join(.     
+00001ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ad0: 2020 2073 656c 662e 726f 6f74 2c0a 2020     self.root,.  
+00001ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001af0: 2020 2020 2020 696e 666f 5b22 636f 7572        info["cour
+00001b00: 7365 5f69 6422 5d2c 0a20 2020 2020 2020  se_id"],.       
 00001b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b20: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00001b30: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00001b20: 2073 656c 662e 6665 6564 6261 636b 5f64   self.feedback_d
+00001b30: 6972 6563 746f 7279 2c0a 2020 2020 2020  irectory,.      
 00001b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b50: 756e 6971 7565 5f6b 6579 203d 206d 616b  unique_key = mak
-00001b60: 655f 756e 6971 7565 5f6b 6579 280a 2020  e_unique_key(.  
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 2020 2020 2020 696e 666f 5b22 636f 7572        info["cour
-00001b90: 7365 5f69 6422 5d2c 0a20 2020 2020 2020  se_id"],.       
-00001ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001bb0: 2069 6e66 6f5b 2261 7373 6967 6e6d 656e   info["assignmen
-00001bc0: 745f 6964 225d 2c0a 2020 2020 2020 2020  t_id"],.        
-00001bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001be0: 6e62 5f69 6e66 6f5b 226e 6f74 6562 6f6f  nb_info["noteboo
-00001bf0: 6b5f 6964 225d 2c0a 2020 2020 2020 2020  k_id"],.        
-00001c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c10: 696e 666f 5b22 7374 7564 656e 745f 6964  info["student_id
-00001c20: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-00001c30: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00001c40: 5b22 7469 6d65 7374 616d 7022 5d2c 0a20  ["timestamp"],. 
-00001c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001c60: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-00001c70: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-00001c80: 672e 6465 6275 6728 2255 6e69 7175 6520  g.debug("Unique 
-00001c90: 6b65 7920 6973 3a20 7b7d 222e 666f 726d  key is: {}".form
-00001ca0: 6174 2875 6e69 7175 655f 6b65 7929 290a  at(unique_key)).
-00001cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001cc0: 2020 2020 6e62 5f68 6173 6820 3d20 6e6f      nb_hash = no
-00001cd0: 7465 626f 6f6b 5f68 6173 6828 6e6f 7465  tebook_hash(note
-00001ce0: 626f 6f6b 2c20 756e 6971 7565 5f6b 6579  book, unique_key
-00001cf0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00001d00: 2020 2020 2020 6578 6368 616e 6765 5f66        exchange_f
-00001d10: 6565 6462 6163 6b5f 7061 7468 203d 206f  eedback_path = o
-00001d20: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+00001b50: 2020 696e 666f 5b22 7374 7564 656e 745f    info["student_
+00001b60: 6964 225d 2c0a 2020 2020 2020 2020 2020  id"],.          
+00001b70: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00001b80: 666f 5b22 6173 7369 676e 6d65 6e74 5f69  fo["assignment_i
+00001b90: 6422 5d2c 0a20 2020 2020 2020 2020 2020  d"],.           
+00001ba0: 2020 2020 2020 2020 2020 2020 2022 7b30               "{0
+00001bb0: 7d2e 6874 6d6c 222e 666f 726d 6174 286e  }.html".format(n
+00001bc0: 625f 696e 666f 5b22 6e6f 7465 626f 6f6b  b_info["notebook
+00001bd0: 5f69 6422 5d29 2c0a 2020 2020 2020 2020  _id"]),.        
+00001be0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00001bf0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00001c00: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00001c10: 2020 2020 2020 2020 756e 6971 7565 5f6b          unique_k
+00001c20: 6579 203d 206d 616b 655f 756e 6971 7565  ey = make_unique
+00001c30: 5f6b 6579 280a 2020 2020 2020 2020 2020  _key(.          
+00001c40: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00001c50: 666f 5b22 636f 7572 7365 5f69 6422 5d2c  fo["course_id"],
+00001c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001c70: 2020 2020 2020 2020 2069 6e66 6f5b 2261           info["a
+00001c80: 7373 6967 6e6d 656e 745f 6964 225d 2c0a  ssignment_id"],.
+00001c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001ca0: 2020 2020 2020 2020 6e62 5f69 6e66 6f5b          nb_info[
+00001cb0: 226e 6f74 6562 6f6f 6b5f 6964 225d 2c0a  "notebook_id"],.
+00001cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cd0: 2020 2020 2020 2020 696e 666f 5b22 7374          info["st
+00001ce0: 7564 656e 745f 6964 225d 2c0a 2020 2020  udent_id"],.    
+00001cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d00: 2020 2020 696e 666f 5b22 7469 6d65 7374      info["timest
+00001d10: 616d 7022 5d2c 0a20 2020 2020 2020 2020  amp"],.         
+00001d20: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
 00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d40: 2020 2020 2073 656c 662e 726f 6f74 2c0a       self.root,.
-00001d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d60: 2020 2020 2020 2020 696e 666f 5b22 636f          info["co
-00001d70: 7572 7365 5f69 6422 5d2c 0a20 2020 2020  urse_id"],.     
-00001d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d90: 2020 2073 656c 662e 6665 6564 6261 636b     self.feedback
-00001da0: 5f64 6972 6563 746f 7279 2c0a 2020 2020  _directory,.    
-00001db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001dc0: 2020 2020 227b 307d 2e68 746d 6c22 2e66      "{0}.html".f
-00001dd0: 6f72 6d61 7428 6e62 5f68 6173 6829 2c0a  ormat(nb_hash),.
-00001de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001df0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00001e00: 2020 2020 2020 2068 6173 5f65 7863 6861         has_excha
-00001e10: 6e67 655f 6665 6564 6261 636b 203d 206f  nge_feedback = o
-00001e20: 732e 7061 7468 2e69 7366 696c 6528 6578  s.path.isfile(ex
-00001e30: 6368 616e 6765 5f66 6565 6462 6163 6b5f  change_feedback_
-00001e40: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
-00001e50: 2020 2020 2020 6966 206e 6f74 2068 6173        if not has
-00001e60: 5f65 7863 6861 6e67 655f 6665 6564 6261  _exchange_feedba
-00001e70: 636b 3a0a 2020 2020 2020 2020 2020 2020  ck:.            
-00001e80: 2020 2020 2020 2020 2320 5472 7920 6c6f          # Try lo
-00001e90: 6f6b 696e 6720 666f 7220 6c65 6761 6379  oking for legacy
-00001ea0: 2066 6565 6462 6163 6b2e 0a20 2020 2020   feedback..     
-00001eb0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00001ec0: 625f 6861 7368 203d 206e 6f74 6562 6f6f  b_hash = noteboo
-00001ed0: 6b5f 6861 7368 286e 6f74 6562 6f6f 6b29  k_hash(notebook)
-00001ee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001ef0: 2020 2020 2065 7863 6861 6e67 655f 6665       exchange_fe
-00001f00: 6564 6261 636b 5f70 6174 6820 3d20 6f73  edback_path = os
-00001f10: 2e70 6174 682e 6a6f 696e 280a 2020 2020  .path.join(.    
-00001f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f30: 2020 2020 7365 6c66 2e72 6f6f 742c 0a20      self.root,. 
+00001d40: 2073 656c 662e 6c6f 672e 6465 6275 6728   self.log.debug(
+00001d50: 2255 6e69 7175 6520 6b65 7920 6973 3a20  "Unique key is: 
+00001d60: 7b7d 222e 666f 726d 6174 2875 6e69 7175  {}".format(uniqu
+00001d70: 655f 6b65 7929 290a 2020 2020 2020 2020  e_key)).        
+00001d80: 2020 2020 2020 2020 2020 2020 6e62 5f68              nb_h
+00001d90: 6173 6820 3d20 6e6f 7465 626f 6f6b 5f68  ash = notebook_h
+00001da0: 6173 6828 6e6f 7465 626f 6f6b 2c20 756e  ash(notebook, un
+00001db0: 6971 7565 5f6b 6579 290a 2020 2020 2020  ique_key).      
+00001dc0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00001dd0: 6368 616e 6765 5f66 6565 6462 6163 6b5f  change_feedback_
+00001de0: 7061 7468 203d 206f 732e 7061 7468 2e6a  path = os.path.j
+00001df0: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
+00001e00: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00001e10: 662e 726f 6f74 2c0a 2020 2020 2020 2020  f.root,.        
+00001e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001e30: 696e 666f 5b22 636f 7572 7365 5f69 6422  info["course_id"
+00001e40: 5d2c 0a20 2020 2020 2020 2020 2020 2020  ],.             
+00001e50: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00001e60: 6665 6564 6261 636b 5f64 6972 6563 746f  feedback_directo
+00001e70: 7279 2c0a 2020 2020 2020 2020 2020 2020  ry,.            
+00001e80: 2020 2020 2020 2020 2020 2020 227b 307d              "{0}
+00001e90: 2e68 746d 6c22 2e66 6f72 6d61 7428 6e62  .html".format(nb
+00001ea0: 5f68 6173 6829 2c0a 2020 2020 2020 2020  _hash),.        
+00001eb0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00001ec0: 2020 2020 2020 2020 2020 2020 2020 2068                 h
+00001ed0: 6173 5f65 7863 6861 6e67 655f 6665 6564  as_exchange_feed
+00001ee0: 6261 636b 203d 206f 732e 7061 7468 2e69  back = os.path.i
+00001ef0: 7366 696c 6528 6578 6368 616e 6765 5f66  sfile(exchange_f
+00001f00: 6565 6462 6163 6b5f 7061 7468 290a 2020  eedback_path).  
+00001f10: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00001f20: 206e 6f74 2068 6173 5f65 7863 6861 6e67   not has_exchang
+00001f30: 655f 6665 6564 6261 636b 3a0a 2020 2020  e_feedback:.    
 00001f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f50: 2020 2020 2020 2069 6e66 6f5b 2263 6f75         info["cou
-00001f60: 7273 655f 6964 225d 2c0a 2020 2020 2020  rse_id"],.      
-00001f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001f80: 2020 2266 6565 6462 6163 6b22 2c0a 2020    "feedback",.  
-00001f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001fa0: 2020 2020 2020 227b 307d 2e68 746d 6c22        "{0}.html"
-00001fb0: 2e66 6f72 6d61 7428 6e62 5f68 6173 6829  .format(nb_hash)
-00001fc0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00001fd0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00001fe0: 2020 2020 2020 2020 2020 2020 6861 735f              has_
-00001ff0: 6578 6368 616e 6765 5f66 6565 6462 6163  exchange_feedbac
-00002000: 6b20 3d20 6f73 2e70 6174 682e 6973 6669  k = os.path.isfi
-00002010: 6c65 2865 7863 6861 6e67 655f 6665 6564  le(exchange_feed
-00002020: 6261 636b 5f70 6174 6829 0a20 2020 2020  back_path).     
-00002030: 2020 2020 2020 2020 2020 2069 6620 6861             if ha
-00002040: 735f 6578 6368 616e 6765 5f66 6565 6462  s_exchange_feedb
-00002050: 6163 6b3a 0a20 2020 2020 2020 2020 2020  ack:.           
-00002060: 2020 2020 2020 2020 2065 7863 6861 6e67           exchang
-00002070: 655f 6665 6564 6261 636b 5f63 6865 636b  e_feedback_check
-00002080: 7375 6d20 3d20 5f63 6865 636b 7375 6d28  sum = _checksum(
-00002090: 6578 6368 616e 6765 5f66 6565 6462 6163  exchange_feedbac
-000020a0: 6b5f 7061 7468 290a 2020 2020 2020 2020  k_path).        
-000020b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000020c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000020d0: 2020 6578 6368 616e 6765 5f66 6565 6462    exchange_feedb
-000020e0: 6163 6b5f 6368 6563 6b73 756d 203d 204e  ack_checksum = N
-000020f0: 6f6e 650a 0a20 2020 2020 2020 2020 2020  one..           
-00002100: 2020 2020 206e 625f 696e 666f 5b22 6861       nb_info["ha
-00002110: 735f 6c6f 6361 6c5f 6665 6564 6261 636b  s_local_feedback
-00002120: 225d 203d 2068 6173 5f6c 6f63 616c 5f66  "] = has_local_f
-00002130: 6565 6462 6163 6b0a 2020 2020 2020 2020  eedback.        
-00002140: 2020 2020 2020 2020 6e62 5f69 6e66 6f5b          nb_info[
-00002150: 2268 6173 5f65 7863 6861 6e67 655f 6665  "has_exchange_fe
-00002160: 6564 6261 636b 225d 203d 2068 6173 5f65  edback"] = has_e
-00002170: 7863 6861 6e67 655f 6665 6564 6261 636b  xchange_feedback
-00002180: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002190: 2069 6620 6861 735f 6c6f 6361 6c5f 6665   if has_local_fe
-000021a0: 6564 6261 636b 3a0a 2020 2020 2020 2020  edback:.        
-000021b0: 2020 2020 2020 2020 2020 2020 6e62 5f69              nb_i
-000021c0: 6e66 6f5b 226c 6f63 616c 5f66 6565 6462  nfo["local_feedb
-000021d0: 6163 6b5f 7061 7468 225d 203d 206c 6f63  ack_path"] = loc
-000021e0: 616c 5f66 6565 6462 6163 6b5f 7061 7468  al_feedback_path
-000021f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002200: 2069 6620 6861 735f 6c6f 6361 6c5f 6665   if has_local_fe
-00002210: 6564 6261 636b 2061 6e64 2068 6173 5f65  edback and has_e
-00002220: 7863 6861 6e67 655f 6665 6564 6261 636b  xchange_feedback
-00002230: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002240: 2020 2020 2020 6e62 5f69 6e66 6f5b 2266        nb_info["f
-00002250: 6565 6462 6163 6b5f 7570 6461 7465 6422  eedback_updated"
-00002260: 5d20 3d20 280a 2020 2020 2020 2020 2020  ] = (.          
-00002270: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-00002280: 6368 616e 6765 5f66 6565 6462 6163 6b5f  change_feedback_
-00002290: 6368 6563 6b73 756d 2021 3d20 6c6f 6361  checksum != loca
-000022a0: 6c5f 6665 6564 6261 636b 5f63 6865 636b  l_feedback_check
-000022b0: 7375 6d0a 2020 2020 2020 2020 2020 2020  sum.            
-000022c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000022d0: 2020 2020 2020 2020 2020 696e 666f 5b22            info["
-000022e0: 6e6f 7465 626f 6f6b 7322 5d2e 6170 7065  notebooks"].appe
-000022f0: 6e64 286e 625f 696e 666f 290a 0a20 2020  nd(nb_info)..   
-00002300: 2020 2020 2020 2020 2069 6620 696e 666f           if info
-00002310: 5b22 7374 6174 7573 225d 203d 3d20 2273  ["status"] == "s
-00002320: 7562 6d69 7474 6564 223a 0a20 2020 2020  ubmitted":.     
-00002330: 2020 2020 2020 2020 2020 2069 6620 696e             if in
-00002340: 666f 5b22 6e6f 7465 626f 6f6b 7322 5d3a  fo["notebooks"]:
-00002350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002360: 2020 2020 2023 204c 6973 7420 6665 6564       # List feed
-00002370: 6261 636b 2069 6620 7468 6572 6520 6578  back if there ex
-00002380: 6973 7473 2066 6f72 206f 6e65 206f 6620  ists for one of 
-00002390: 7468 6520 6e6f 7465 626f 6f6b 7320 6669  the notebooks fi
-000023a0: 6c65 7320 696e 2070 6174 680a 2020 2020  les in path.    
-000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023c0: 6861 735f 6c6f 6361 6c5f 6665 6564 6261  has_local_feedba
-000023d0: 636b 203d 2061 6e79 280a 2020 2020 2020  ck = any(.      
-000023e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000023f0: 2020 5b6e 625b 2268 6173 5f6c 6f63 616c    [nb["has_local
-00002400: 5f66 6565 6462 6163 6b22 5d20 666f 7220  _feedback"] for 
-00002410: 6e62 2069 6e20 696e 666f 5b22 6e6f 7465  nb in info["note
-00002420: 626f 6f6b 7322 5d5d 0a20 2020 2020 2020  books"]].       
-00002430: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-00002440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002450: 2020 2068 6173 5f65 7863 6861 6e67 655f     has_exchange_
-00002460: 6665 6564 6261 636b 203d 2061 6e79 280a  feedback = any(.
-00002470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002480: 2020 2020 2020 2020 5b6e 625b 2268 6173          [nb["has
-00002490: 5f65 7863 6861 6e67 655f 6665 6564 6261  _exchange_feedba
-000024a0: 636b 225d 2066 6f72 206e 6220 696e 2069  ck"] for nb in i
-000024b0: 6e66 6f5b 226e 6f74 6562 6f6f 6b73 225d  nfo["notebooks"]
-000024c0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-000024d0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000024e0: 2020 2020 2020 2020 2020 2020 6665 6564              feed
-000024f0: 6261 636b 5f75 7064 6174 6564 203d 2061  back_updated = a
-00002500: 6e79 280a 2020 2020 2020 2020 2020 2020  ny(.            
-00002510: 2020 2020 2020 2020 2020 2020 5b6e 625b              [nb[
-00002520: 2266 6565 6462 6163 6b5f 7570 6461 7465  "feedback_update
-00002530: 6422 5d20 666f 7220 6e62 2069 6e20 696e  d"] for nb in in
-00002540: 666f 5b22 6e6f 7465 626f 6f6b 7322 5d5d  fo["notebooks"]]
-00002550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002560: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00002570: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00002580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002590: 2068 6173 5f6c 6f63 616c 5f66 6565 6462   has_local_feedb
-000025a0: 6163 6b20 3d20 4661 6c73 650a 2020 2020  ack = False.    
-000025b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025c0: 6861 735f 6578 6368 616e 6765 5f66 6565  has_exchange_fee
-000025d0: 6462 6163 6b20 3d20 4661 6c73 650a 2020  dback = False.  
-000025e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025f0: 2020 6665 6564 6261 636b 5f75 7064 6174    feedback_updat
-00002600: 6564 203d 2046 616c 7365 0a0a 2020 2020  ed = False..    
-00002610: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00002620: 5b22 6861 735f 6c6f 6361 6c5f 6665 6564  ["has_local_feed
-00002630: 6261 636b 225d 203d 2068 6173 5f6c 6f63  back"] = has_loc
-00002640: 616c 5f66 6565 6462 6163 6b0a 2020 2020  al_feedback.    
-00002650: 2020 2020 2020 2020 2020 2020 696e 666f              info
-00002660: 5b22 6861 735f 6578 6368 616e 6765 5f66  ["has_exchange_f
-00002670: 6565 6462 6163 6b22 5d20 3d20 6861 735f  eedback"] = has_
-00002680: 6578 6368 616e 6765 5f66 6565 6462 6163  exchange_feedbac
-00002690: 6b0a 2020 2020 2020 2020 2020 2020 2020  k.              
-000026a0: 2020 696e 666f 5b22 6665 6564 6261 636b    info["feedback
-000026b0: 5f75 7064 6174 6564 225d 203d 2066 6565  _updated"] = fee
-000026c0: 6462 6163 6b5f 7570 6461 7465 640a 2020  dback_updated.  
-000026d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-000026e0: 2068 6173 5f6c 6f63 616c 5f66 6565 6462   has_local_feedb
-000026f0: 6163 6b3a 0a20 2020 2020 2020 2020 2020  ack:.           
-00002700: 2020 2020 2020 2020 2069 6e66 6f5b 226c           info["l
-00002710: 6f63 616c 5f66 6565 6462 6163 6b5f 7061  ocal_feedback_pa
-00002720: 7468 225d 203d 206f 732e 7061 7468 2e6a  th"] = os.path.j
-00002730: 6f69 6e28 0a20 2020 2020 2020 2020 2020  oin(.           
-00002740: 2020 2020 2020 2020 2020 2020 2061 7373               ass
-00002750: 6967 6e6d 656e 745f 6469 722c 2022 6665  ignment_dir, "fe
-00002760: 6564 6261 636b 222c 2069 6e66 6f5b 2274  edback", info["t
-00002770: 696d 6573 7461 6d70 225d 0a20 2020 2020  imestamp"].     
-00002780: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00002790: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000027a0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000027b0: 2020 2020 2020 2020 2020 2069 6e66 6f5b             info[
-000027c0: 226c 6f63 616c 5f66 6565 6462 6163 6b5f  "local_feedback_
-000027d0: 7061 7468 225d 203d 204e 6f6e 650a 0a20  path"] = None.. 
-000027e0: 2020 2020 2020 2020 2020 2061 7373 6967             assig
-000027f0: 6e6d 656e 7473 2e61 7070 656e 6428 696e  nments.append(in
-00002800: 666f 290a 0a20 2020 2020 2020 2023 2070  fo)..        # p
-00002810: 6172 7469 7469 6f6e 2074 6865 2061 7373  artition the ass
-00002820: 6967 6e6d 656e 7473 2069 6e74 6f20 6772  ignments into gr
-00002830: 6f75 7073 2066 6f72 2063 6f75 7273 652f  oups for course/
-00002840: 7374 7564 656e 742f 6173 7369 676e 6d65  student/assignme
-00002850: 6e74 0a20 2020 2020 2020 2069 6620 7365  nt.        if se
-00002860: 6c66 2e69 6e62 6f75 6e64 206f 7220 7365  lf.inbound or se
-00002870: 6c66 2e63 6163 6865 643a 0a20 2020 2020  lf.cached:.     
-00002880: 2020 2020 2020 2061 7373 6967 6e6d 656e         assignmen
-00002890: 745f 6b65 7973 203d 2073 6f72 7465 6428  t_keys = sorted(
-000028a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000028b0: 206c 6973 7428 7365 7428 5b5f 6765 745f   list(set([_get_
-000028c0: 6b65 7928 696e 666f 2920 666f 7220 696e  key(info) for in
-000028d0: 666f 2069 6e20 6173 7369 676e 6d65 6e74  fo in assignment
-000028e0: 735d 2929 0a20 2020 2020 2020 2020 2020  s])).           
-000028f0: 2029 0a20 2020 2020 2020 2020 2020 2061   ).            a
-00002900: 7373 6967 6e6d 656e 745f 7375 626d 6973  ssignment_submis
-00002910: 7369 6f6e 7320 3d20 5b5d 0a20 2020 2020  sions = [].     
-00002920: 2020 2020 2020 2066 6f72 206b 6579 2069         for key i
-00002930: 6e20 6173 7369 676e 6d65 6e74 5f6b 6579  n assignment_key
-00002940: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00002950: 2020 2073 7562 6d69 7373 696f 6e73 203d     submissions =
-00002960: 205b 7820 666f 7220 7820 696e 2061 7373   [x for x in ass
-00002970: 6967 6e6d 656e 7473 2069 6620 5f6d 6174  ignments if _mat
-00002980: 6368 5f6b 6579 2878 2c20 6b65 7929 5d0a  ch_key(x, key)].
-00002990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029a0: 7375 626d 6973 7369 6f6e 7320 3d20 736f  submissions = so
-000029b0: 7274 6564 2873 7562 6d69 7373 696f 6e73  rted(submissions
-000029c0: 2c20 6b65 793d 6c61 6d62 6461 2078 3a20  , key=lambda x: 
-000029d0: 785b 2274 696d 6573 7461 6d70 225d 290a  x["timestamp"]).
-000029e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000029f0: 696e 666f 203d 207b 0a20 2020 2020 2020  info = {.       
-00002a00: 2020 2020 2020 2020 2020 2020 2022 636f               "co
-00002a10: 7572 7365 5f69 6422 3a20 6b65 795b 305d  urse_id": key[0]
-00002a20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00002a30: 2020 2020 2020 2273 7475 6465 6e74 5f69        "student_i
-00002a40: 6422 3a20 6b65 795b 315d 2c0a 2020 2020  d": key[1],.    
-00002a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002a60: 2261 7373 6967 6e6d 656e 745f 6964 223a  "assignment_id":
-00002a70: 206b 6579 5b32 5d2c 0a20 2020 2020 2020   key[2],.       
-00002a80: 2020 2020 2020 2020 2020 2020 2022 7374               "st
-00002a90: 6174 7573 223a 2073 7562 6d69 7373 696f  atus": submissio
-00002aa0: 6e73 5b30 5d5b 2273 7461 7475 7322 5d2c  ns[0]["status"],
-00002ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002ac0: 2020 2020 2022 7375 626d 6973 7369 6f6e       "submission
-00002ad0: 7322 3a20 7375 626d 6973 7369 6f6e 732c  s": submissions,
-00002ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002af0: 207d 0a20 2020 2020 2020 2020 2020 2020   }.             
-00002b00: 2020 2061 7373 6967 6e6d 656e 745f 7375     assignment_su
-00002b10: 626d 6973 7369 6f6e 732e 6170 7065 6e64  bmissions.append
-00002b20: 2869 6e66 6f29 0a20 2020 2020 2020 2020  (info).         
-00002b30: 2020 2061 7373 6967 6e6d 656e 7473 203d     assignments =
-00002b40: 2061 7373 6967 6e6d 656e 745f 7375 626d   assignment_subm
-00002b50: 6973 7369 6f6e 730a 0a20 2020 2020 2020  issions..       
-00002b60: 2072 6574 7572 6e20 6173 7369 676e 6d65   return assignme
-00002b70: 6e74 730a                                nts.
+00001f50: 2320 5472 7920 6c6f 6f6b 696e 6720 666f  # Try looking fo
+00001f60: 7220 6c65 6761 6379 2066 6565 6462 6163  r legacy feedbac
+00001f70: 6b2e 0a20 2020 2020 2020 2020 2020 2020  k..             
+00001f80: 2020 2020 2020 206e 625f 6861 7368 203d         nb_hash =
+00001f90: 206e 6f74 6562 6f6f 6b5f 6861 7368 286e   notebook_hash(n
+00001fa0: 6f74 6562 6f6f 6b29 0a20 2020 2020 2020  otebook).       
+00001fb0: 2020 2020 2020 2020 2020 2020 2065 7863               exc
+00001fc0: 6861 6e67 655f 6665 6564 6261 636b 5f70  hange_feedback_p
+00001fd0: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
+00001fe0: 696e 280a 2020 2020 2020 2020 2020 2020  in(.            
+00001ff0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00002000: 2e72 6f6f 742c 0a20 2020 2020 2020 2020  .root,.         
+00002010: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002020: 6e66 6f5b 2263 6f75 7273 655f 6964 225d  nfo["course_id"]
+00002030: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00002040: 2020 2020 2020 2020 2020 2266 6565 6462            "feedb
+00002050: 6163 6b22 2c0a 2020 2020 2020 2020 2020  ack",.          
+00002060: 2020 2020 2020 2020 2020 2020 2020 227b                "{
+00002070: 307d 2e68 746d 6c22 2e66 6f72 6d61 7428  0}.html".format(
+00002080: 6e62 5f68 6173 6829 2c0a 2020 2020 2020  nb_hash),.      
+00002090: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000020a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000020b0: 2020 2020 6861 735f 6578 6368 616e 6765      has_exchange
+000020c0: 5f66 6565 6462 6163 6b20 3d20 6f73 2e70  _feedback = os.p
+000020d0: 6174 682e 6973 6669 6c65 2865 7863 6861  ath.isfile(excha
+000020e0: 6e67 655f 6665 6564 6261 636b 5f70 6174  nge_feedback_pat
+000020f0: 6829 0a20 2020 2020 2020 2020 2020 2020  h).             
+00002100: 2020 2069 6620 6861 735f 6578 6368 616e     if has_exchan
+00002110: 6765 5f66 6565 6462 6163 6b3a 0a20 2020  ge_feedback:.   
+00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002130: 2065 7863 6861 6e67 655f 6665 6564 6261   exchange_feedba
+00002140: 636b 5f63 6865 636b 7375 6d20 3d20 5f63  ck_checksum = _c
+00002150: 6865 636b 7375 6d28 6578 6368 616e 6765  hecksum(exchange
+00002160: 5f66 6565 6462 6163 6b5f 7061 7468 290a  _feedback_path).
+00002170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002180: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00002190: 2020 2020 2020 2020 2020 6578 6368 616e            exchan
+000021a0: 6765 5f66 6565 6462 6163 6b5f 6368 6563  ge_feedback_chec
+000021b0: 6b73 756d 203d 204e 6f6e 650a 0a20 2020  ksum = None..   
+000021c0: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
+000021d0: 696e 666f 5b22 6861 735f 6c6f 6361 6c5f  info["has_local_
+000021e0: 6665 6564 6261 636b 225d 203d 2068 6173  feedback"] = has
+000021f0: 5f6c 6f63 616c 5f66 6565 6462 6163 6b0a  _local_feedback.
+00002200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002210: 6e62 5f69 6e66 6f5b 2268 6173 5f65 7863  nb_info["has_exc
+00002220: 6861 6e67 655f 6665 6564 6261 636b 225d  hange_feedback"]
+00002230: 203d 2068 6173 5f65 7863 6861 6e67 655f   = has_exchange_
+00002240: 6665 6564 6261 636b 0a20 2020 2020 2020  feedback.       
+00002250: 2020 2020 2020 2020 2069 6620 6861 735f           if has_
+00002260: 6c6f 6361 6c5f 6665 6564 6261 636b 3a0a  local_feedback:.
+00002270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002280: 2020 2020 6e62 5f69 6e66 6f5b 226c 6f63      nb_info["loc
+00002290: 616c 5f66 6565 6462 6163 6b5f 7061 7468  al_feedback_path
+000022a0: 225d 203d 206c 6f63 616c 5f66 6565 6462  "] = local_feedb
+000022b0: 6163 6b5f 7061 7468 0a20 2020 2020 2020  ack_path.       
+000022c0: 2020 2020 2020 2020 2069 6620 6861 735f           if has_
+000022d0: 6c6f 6361 6c5f 6665 6564 6261 636b 2061  local_feedback a
+000022e0: 6e64 2068 6173 5f65 7863 6861 6e67 655f  nd has_exchange_
+000022f0: 6665 6564 6261 636b 3a0a 2020 2020 2020  feedback:.      
+00002300: 2020 2020 2020 2020 2020 2020 2020 6e62                nb
+00002310: 5f69 6e66 6f5b 2266 6565 6462 6163 6b5f  _info["feedback_
+00002320: 7570 6461 7465 6422 5d20 3d20 280a 2020  updated"] = (.  
+00002330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002340: 2020 2020 2020 6578 6368 616e 6765 5f66        exchange_f
+00002350: 6565 6462 6163 6b5f 6368 6563 6b73 756d  eedback_checksum
+00002360: 2021 3d20 6c6f 6361 6c5f 6665 6564 6261   != local_feedba
+00002370: 636b 5f63 6865 636b 7375 6d0a 2020 2020  ck_checksum.    
+00002380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002390: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000023a0: 2020 696e 666f 5b22 6e6f 7465 626f 6f6b    info["notebook
+000023b0: 7322 5d2e 6170 7065 6e64 286e 625f 696e  s"].append(nb_in
+000023c0: 666f 290a 0a20 2020 2020 2020 2020 2020  fo)..           
+000023d0: 2069 6620 696e 666f 5b22 7374 6174 7573   if info["status
+000023e0: 225d 203d 3d20 2273 7562 6d69 7474 6564  "] == "submitted
+000023f0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00002400: 2020 2069 6620 696e 666f 5b22 6e6f 7465     if info["note
+00002410: 626f 6f6b 7322 5d3a 0a20 2020 2020 2020  books"]:.       
+00002420: 2020 2020 2020 2020 2020 2020 2023 204c               # L
+00002430: 6973 7420 6665 6564 6261 636b 2069 6620  ist feedback if 
+00002440: 7468 6572 6520 6578 6973 7473 2066 6f72  there exists for
+00002450: 206f 6e65 206f 6620 7468 6520 6e6f 7465   one of the note
+00002460: 626f 6f6b 7320 6669 6c65 7320 696e 2070  books files in p
+00002470: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
+00002480: 2020 2020 2020 2020 6861 735f 6c6f 6361          has_loca
+00002490: 6c5f 6665 6564 6261 636b 203d 2061 6e79  l_feedback = any
+000024a0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000024b0: 2020 2020 2020 2020 2020 5b6e 625b 2268            [nb["h
+000024c0: 6173 5f6c 6f63 616c 5f66 6565 6462 6163  as_local_feedbac
+000024d0: 6b22 5d20 666f 7220 6e62 2069 6e20 696e  k"] for nb in in
+000024e0: 666f 5b22 6e6f 7465 626f 6f6b 7322 5d5d  fo["notebooks"]]
+000024f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002500: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00002510: 2020 2020 2020 2020 2020 2068 6173 5f65             has_e
+00002520: 7863 6861 6e67 655f 6665 6564 6261 636b  xchange_feedback
+00002530: 203d 2061 6e79 280a 2020 2020 2020 2020   = any(.        
+00002540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002550: 5b6e 625b 2268 6173 5f65 7863 6861 6e67  [nb["has_exchang
+00002560: 655f 6665 6564 6261 636b 225d 2066 6f72  e_feedback"] for
+00002570: 206e 6220 696e 2069 6e66 6f5b 226e 6f74   nb in info["not
+00002580: 6562 6f6f 6b73 225d 5d0a 2020 2020 2020  ebooks"]].      
+00002590: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000025a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025b0: 2020 2020 6665 6564 6261 636b 5f75 7064      feedback_upd
+000025c0: 6174 6564 203d 2061 6e79 280a 2020 2020  ated = any(.    
+000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000025e0: 2020 2020 5b6e 625b 2266 6565 6462 6163      [nb["feedbac
+000025f0: 6b5f 7570 6461 7465 6422 5d20 666f 7220  k_updated"] for 
+00002600: 6e62 2069 6e20 696e 666f 5b22 6e6f 7465  nb in info["note
+00002610: 626f 6f6b 7322 5d5d 0a20 2020 2020 2020  books"]].       
+00002620: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00002630: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00002640: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00002650: 2020 2020 2020 2020 2068 6173 5f6c 6f63           has_loc
+00002660: 616c 5f66 6565 6462 6163 6b20 3d20 4661  al_feedback = Fa
+00002670: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00002680: 2020 2020 2020 2020 6861 735f 6578 6368          has_exch
+00002690: 616e 6765 5f66 6565 6462 6163 6b20 3d20  ange_feedback = 
+000026a0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+000026b0: 2020 2020 2020 2020 2020 6665 6564 6261            feedba
+000026c0: 636b 5f75 7064 6174 6564 203d 2046 616c  ck_updated = Fal
+000026d0: 7365 0a0a 2020 2020 2020 2020 2020 2020  se..            
+000026e0: 2020 2020 696e 666f 5b22 6861 735f 6c6f      info["has_lo
+000026f0: 6361 6c5f 6665 6564 6261 636b 225d 203d  cal_feedback"] =
+00002700: 2068 6173 5f6c 6f63 616c 5f66 6565 6462   has_local_feedb
+00002710: 6163 6b0a 2020 2020 2020 2020 2020 2020  ack.            
+00002720: 2020 2020 696e 666f 5b22 6861 735f 6578      info["has_ex
+00002730: 6368 616e 6765 5f66 6565 6462 6163 6b22  change_feedback"
+00002740: 5d20 3d20 6861 735f 6578 6368 616e 6765  ] = has_exchange
+00002750: 5f66 6565 6462 6163 6b0a 2020 2020 2020  _feedback.      
+00002760: 2020 2020 2020 2020 2020 696e 666f 5b22            info["
+00002770: 6665 6564 6261 636b 5f75 7064 6174 6564  feedback_updated
+00002780: 225d 203d 2066 6565 6462 6163 6b5f 7570  "] = feedback_up
+00002790: 6461 7465 640a 2020 2020 2020 2020 2020  dated.          
+000027a0: 2020 2020 2020 6966 2068 6173 5f6c 6f63        if has_loc
+000027b0: 616c 5f66 6565 6462 6163 6b3a 0a20 2020  al_feedback:.   
+000027c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027d0: 2069 6e66 6f5b 226c 6f63 616c 5f66 6565   info["local_fee
+000027e0: 6462 6163 6b5f 7061 7468 225d 203d 206f  dback_path"] = o
+000027f0: 732e 7061 7468 2e6a 6f69 6e28 0a20 2020  s.path.join(.   
+00002800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002810: 2020 2020 2061 7373 6967 6e6d 656e 745f       assignment_
+00002820: 6469 722c 2022 6665 6564 6261 636b 222c  dir, "feedback",
+00002830: 2069 6e66 6f5b 2274 696d 6573 7461 6d70   info["timestamp
+00002840: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
+00002850: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00002860: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00002870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002880: 2020 2069 6e66 6f5b 226c 6f63 616c 5f66     info["local_f
+00002890: 6565 6462 6163 6b5f 7061 7468 225d 203d  eedback_path"] =
+000028a0: 204e 6f6e 650a 0a20 2020 2020 2020 2020   None..         
+000028b0: 2020 2061 7373 6967 6e6d 656e 7473 2e61     assignments.a
+000028c0: 7070 656e 6428 696e 666f 290a 0a20 2020  ppend(info)..   
+000028d0: 2020 2020 2023 2070 6172 7469 7469 6f6e       # partition
+000028e0: 2074 6865 2061 7373 6967 6e6d 656e 7473   the assignments
+000028f0: 2069 6e74 6f20 6772 6f75 7073 2066 6f72   into groups for
+00002900: 2063 6f75 7273 652f 7374 7564 656e 742f   course/student/
+00002910: 6173 7369 676e 6d65 6e74 0a20 2020 2020  assignment.     
+00002920: 2020 2069 6620 7365 6c66 2e69 6e62 6f75     if self.inbou
+00002930: 6e64 206f 7220 7365 6c66 2e63 6163 6865  nd or self.cache
+00002940: 643a 0a20 2020 2020 2020 2020 2020 2061  d:.            a
+00002950: 7373 6967 6e6d 656e 745f 6b65 7973 203d  ssignment_keys =
+00002960: 2073 6f72 7465 6428 0a20 2020 2020 2020   sorted(.       
+00002970: 2020 2020 2020 2020 206c 6973 7428 7365           list(se
+00002980: 7428 5b5f 6765 745f 6b65 7928 696e 666f  t([_get_key(info
+00002990: 2920 666f 7220 696e 666f 2069 6e20 6173  ) for info in as
+000029a0: 7369 676e 6d65 6e74 735d 2929 0a20 2020  signments])).   
+000029b0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+000029c0: 2020 2020 2020 2061 7373 6967 6e6d 656e         assignmen
+000029d0: 745f 7375 626d 6973 7369 6f6e 7320 3d20  t_submissions = 
+000029e0: 5b5d 0a20 2020 2020 2020 2020 2020 2066  [].            f
+000029f0: 6f72 206b 6579 2069 6e20 6173 7369 676e  or key in assign
+00002a00: 6d65 6e74 5f6b 6579 733a 0a20 2020 2020  ment_keys:.     
+00002a10: 2020 2020 2020 2020 2020 2073 7562 6d69             submi
+00002a20: 7373 696f 6e73 203d 205b 7820 666f 7220  ssions = [x for 
+00002a30: 7820 696e 2061 7373 6967 6e6d 656e 7473  x in assignments
+00002a40: 2069 6620 5f6d 6174 6368 5f6b 6579 2878   if _match_key(x
+00002a50: 2c20 6b65 7929 5d0a 2020 2020 2020 2020  , key)].        
+00002a60: 2020 2020 2020 2020 7375 626d 6973 7369          submissi
+00002a70: 6f6e 7320 3d20 736f 7274 6564 2873 7562  ons = sorted(sub
+00002a80: 6d69 7373 696f 6e73 2c20 6b65 793d 6c61  missions, key=la
+00002a90: 6d62 6461 2078 3a20 785b 2274 696d 6573  mbda x: x["times
+00002aa0: 7461 6d70 225d 290a 2020 2020 2020 2020  tamp"]).        
+00002ab0: 2020 2020 2020 2020 696e 666f 203d 207b          info = {
+00002ac0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002ad0: 2020 2020 2022 636f 7572 7365 5f69 6422       "course_id"
+00002ae0: 3a20 6b65 795b 305d 2c0a 2020 2020 2020  : key[0],.      
+00002af0: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00002b00: 7475 6465 6e74 5f69 6422 3a20 6b65 795b  tudent_id": key[
+00002b10: 315d 2c0a 2020 2020 2020 2020 2020 2020  1],.            
+00002b20: 2020 2020 2020 2020 2261 7373 6967 6e6d          "assignm
+00002b30: 656e 745f 6964 223a 206b 6579 5b32 5d2c  ent_id": key[2],
+00002b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002b50: 2020 2020 2022 7374 6174 7573 223a 2073       "status": s
+00002b60: 7562 6d69 7373 696f 6e73 5b30 5d5b 2273  ubmissions[0]["s
+00002b70: 7461 7475 7322 5d2c 0a20 2020 2020 2020  tatus"],.       
+00002b80: 2020 2020 2020 2020 2020 2020 2022 7375               "su
+00002b90: 626d 6973 7369 6f6e 7322 3a20 7375 626d  bmissions": subm
+00002ba0: 6973 7369 6f6e 732c 0a20 2020 2020 2020  issions,.       
+00002bb0: 2020 2020 2020 2020 207d 0a20 2020 2020           }.     
+00002bc0: 2020 2020 2020 2020 2020 2061 7373 6967             assig
+00002bd0: 6e6d 656e 745f 7375 626d 6973 7369 6f6e  nment_submission
+00002be0: 732e 6170 7065 6e64 2869 6e66 6f29 0a20  s.append(info). 
+00002bf0: 2020 2020 2020 2020 2020 2061 7373 6967             assig
+00002c00: 6e6d 656e 7473 203d 2061 7373 6967 6e6d  nments = assignm
+00002c10: 656e 745f 7375 626d 6973 7369 6f6e 730a  ent_submissions.
+00002c20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00002c30: 6173 7369 676e 6d65 6e74 730a            assignments.
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/release_assignment.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exchange/release_assignment.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/release_feedback.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exchange/release_feedback.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/submit.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exchange/submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,16 @@
             dest_path,
             fileperms=(S_IRUSR | S_IWUSR | S_IRGRP | S_IROTH),
             dirperms=(
                 S_IRUSR | S_IWUSR | S_IXUSR | S_IRGRP | S_IXGRP | S_IROTH | S_IXOTH
             ),
         )
 
-        # Make this 0777=ugo=rwx so the instructor can delete later. Hidden from other users by the timestamp.
+        # Make this 0777=ugo=rwx so the instructor can delete later.
+        # Hidden from other users by the timestamp.
         os.chmod(
             dest_path,
             S_IRUSR
             | S_IWUSR
             | S_IXUSR
             | S_IRGRP
             | S_IWGRP
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exchange/utils.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exchange/utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exporters/exporter.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exporters/exporter.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exporters/gradeexporter.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exporters/gradeexporter.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/exporters/filters/highlight.py` & `e2xgrader-0.1.0.dev3/e2xgrader/exporters/filters/highlight.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/graders/base.py` & `e2xgrader-0.1.0.dev3/e2xgrader/graders/base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/graders/code.py` & `e2xgrader-0.1.0.dev3/e2xgrader/graders/code.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/graders/multiplechoice.py` & `e2xgrader-0.1.0.dev3/e2xgrader/graders/multiplechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/graders/singlechoice.py` & `e2xgrader-0.1.0.dev3/e2xgrader/graders/singlechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/assignmentmodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/models/assignmentmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/basemodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/models/basemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/exercisemodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/models/exercisemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presetmodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presetmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/taskmodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/models/taskmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/taskpoolmodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/models/taskpoolmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/templatemodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/models/templatemodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,18 @@
                 os.makedirs(os.path.join(self.base_path(), name, "img"), exist_ok=True)
                 os.makedirs(os.path.join(self.base_path(), name, "data"), exist_ok=True)
                 filename = "{}.ipynb".format(name)
                 nb = nbformat.v4.new_notebook()
                 nb.metadata["nbassignment"] = {"type": "template"}
                 cell = new_read_only_cell(
                     grade_id="HeaderA",
-                    source="### This is a header cell\n\nIt will always appear at the top of the notebook",
+                    source=(
+                        "### This is a header cell\n\n"
+                        "It will always appear at the top of the notebook"
+                    ),
                 )
                 cell.metadata["nbassignment"] = {"type": "header"}
                 nb.cells = [cell]
                 path = os.path.join(self.base_path(), name, filename)
                 nbformat.write(nb, path)
                 return {"success": True, "path": os.path.join("notebooks", path)}
         else:
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Code (Autograded).ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Code (Autograded).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Code (Manual).ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Code (Manual).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Diagram.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Diagram.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Freetext.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Freetext.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Multiple Choice.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Multiple Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Single Choice.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Single Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/questions/Upload Files.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/questions/Upload Files.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Footer.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/template/Footer.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Group Info.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/template/Group Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Header.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/template/Header.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/models/presets/template/Student Info.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/models/presets/template/Student Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/__init__.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/clearhiddentests.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/clearhiddentests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/clearsolutions.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/clearsolutions.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/extractattachments.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/extractattachments.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/filtercellsbyid.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/filtercellsbyid.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/filtertests.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/filtertests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/overwritecells.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/overwritecells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/permutetasks.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/permutetasks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/saveautogrades.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/saveautogrades.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/savecells.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/savecells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/scramble.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/scramble.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/unpermutetasks.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/unpermutetasks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/unscramble.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/unscramble.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/validateextracells.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/validateextracells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/addtaskheader.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/addtaskheader.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/copyfiles.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/copyfiles.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/copynotebooks.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/copynotebooks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/filltemplate.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/filltemplate.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/generatetaskids.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/generatetaskids.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/makeexercise.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/makeexercise.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/preprocessors/authoring/removeexercise.py` & `e2xgrader-0.1.0.dev3/e2xgrader/preprocessors/authoring/removeexercise.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/assignment_list/handlers.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/assignment_list/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/grader.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/grader.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/apihandlers.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/apihandlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/authoring.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/authoring.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/handlers.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/editexercise.css` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/css/editexercise.css`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/sidebar.css` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/css/sidebar.css`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/css/taskcreator.css` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/css/taskcreator.css`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/assignments.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/assignments.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/base.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/base.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/exercises.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/exercises.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/makeexercise.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/makeexercise.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/taskpools.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/taskpools.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/tasks.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/tasks.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/static/js/templates.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/static/js/templates.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/assignments.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/assignments.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/base.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/base.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/editexercise.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/editexercise.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/exercises.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/exercises.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tablebase.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tablebase.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskcreator.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskcreator.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskpools.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/taskpools.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tasks.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/tasks.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/templates.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/authoring/templates/authoring/templates.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/base/base.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/base/base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/apihandlers.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/apihandlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/e2xgraderapi.py` & `e2xgrader-0.1.0.dev3/.ruff_cache/content/f2eb80dab531e444`

 * *Files 26% similar despite different names*

```diff
@@ -1,41 +1,57 @@
-00000000: 696d 706f 7274 206f 730a 0a66 726f 6d20  import os..from 
-00000010: 6e62 6772 6164 6572 2e61 7070 732e 6261  nbgrader.apps.ba
-00000020: 7365 6170 7020 696d 706f 7274 204e 6247  seapp import NbG
-00000030: 7261 6465 720a 6672 6f6d 206e 6267 7261  rader.from nbgra
-00000040: 6465 722e 7365 7276 6572 5f65 7874 656e  der.server_exten
-00000050: 7369 6f6e 732e 666f 726d 6772 6164 6572  sions.formgrader
-00000060: 2e61 7069 6861 6e64 6c65 7273 2069 6d70  .apihandlers imp
-00000070: 6f72 7420 6465 6661 756c 745f 6861 6e64  ort default_hand
-00000080: 6c65 7273 0a0a 6672 6f6d 2065 3278 6772  lers..from e2xgr
-00000090: 6164 6572 2e73 6572 7665 725f 6578 7465  ader.server_exte
-000000a0: 6e73 696f 6e73 2e67 7261 6465 722e 6170  nsions.grader.ap
-000000b0: 7073 2e62 6173 6520 696d 706f 7274 2042  ps.base import B
-000000c0: 6173 6541 7070 0a0a 6672 6f6d 202e 6170  aseApp..from .ap
-000000d0: 6968 616e 646c 6572 7320 696d 706f 7274  ihandlers import
-000000e0: 2064 6566 6175 6c74 5f68 616e 646c 6572   default_handler
-000000f0: 730a 0a0a 636c 6173 7320 4532 7847 7261  s...class E2xGra
-00000100: 6465 7241 7069 284e 6247 7261 6465 722c  derApi(NbGrader,
-00000110: 2042 6173 6541 7070 293a 0a20 2020 2074   BaseApp):.    t
-00000120: 656d 706c 6174 655f 7061 7468 203d 206f  emplate_path = o
-00000130: 732e 7061 7468 2e6a 6f69 6e28 6f73 2e70  s.path.join(os.p
-00000140: 6174 682e 6469 726e 616d 6528 5f5f 6669  ath.dirname(__fi
-00000150: 6c65 5f5f 292c 2022 7465 6d70 6c61 7465  le__), "template
-00000160: 7322 290a 0a20 2020 2064 6566 205f 5f69  s")..    def __i
-00000170: 6e69 745f 5f28 7365 6c66 2c20 2a2a 6b77  nit__(self, **kw
-00000180: 6172 6773 293a 0a20 2020 2020 2020 204e  args):.        N
-00000190: 6247 7261 6465 722e 5f5f 696e 6974 5f5f  bGrader.__init__
-000001a0: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
-000001b0: 0a20 2020 2020 2020 2042 6173 6541 7070  .        BaseApp
-000001c0: 2e5f 5f69 6e69 745f 5f28 7365 6c66 2c20  .__init__(self, 
-000001d0: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
-000001e0: 6566 206c 6f61 645f 6170 7028 7365 6c66  ef load_app(self
-000001f0: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00000200: 6c6f 672e 696e 666f 2822 4c6f 6164 696e  log.info("Loadin
-00000210: 6720 7468 6520 6532 7867 7261 6465 7220  g the e2xgrader 
-00000220: 6170 6920 6170 7022 290a 2020 2020 2020  api app").      
-00000230: 2020 7365 6c66 2e61 6464 5f74 656d 706c    self.add_templ
-00000240: 6174 655f 7061 7468 2873 656c 662e 7465  ate_path(self.te
-00000250: 6d70 6c61 7465 5f70 6174 6829 0a20 2020  mplate_path).   
-00000260: 2020 2020 2073 656c 662e 6164 645f 6861       self.add_ha
-00000270: 6e64 6c65 7273 2864 6566 6175 6c74 5f68  ndlers(default_h
-00000280: 616e 646c 6572 7329 0a                   andlers).
+00000000: 0000 0000 0000 0000 0100 0000 0000 0000  ................
+00000010: 1400 0000 0000 0000 5265 6465 6669 6e65  ........Redefine
+00000020: 6457 6869 6c65 556e 7573 6564 3500 0000  dWhileUnused5...
+00000030: 0000 0000 5265 6465 6669 6e69 7469 6f6e  ....Redefinition
+00000040: 206f 6620 756e 7573 6564 2060 6465 6661   of unused `defa
+00000050: 756c 745f 6861 6e64 6c65 7273 6020 6672  ult_handlers` fr
+00000060: 6f6d 206c 696e 6520 3400 e100 0000 f100  om line 4.......
+00000070: 0000 0000 0000 0000 0000 00e1 0000 0001  ................
+00000080: 0000 0000 0000 006c 0000 0000 0000 002f  .......l......./
+00000090: 686f 6d65 2f6e 6172 662f 5072 6f6a 6563  home/narf/Projec
+000000a0: 7473 2f65 3278 2f72 6570 6f73 2f65 3278  ts/e2x/repos/e2x
+000000b0: 6772 6164 6572 2f65 3278 6772 6164 6572  grader/e2xgrader
+000000c0: 2f73 6572 7665 725f 6578 7465 6e73 696f  /server_extensio
+000000d0: 6e73 2f67 7261 6465 722f 6170 7073 2f65  ns/grader/apps/e
+000000e0: 3278 6772 6164 6572 6170 692f 6532 7867  2xgraderapi/e2xg
+000000f0: 7261 6465 7261 7069 2e70 7989 0200 0000  raderapi.py.....
+00000100: 0000 0069 6d70 6f72 7420 6f73 0a0a 6672  ...import os..fr
+00000110: 6f6d 206e 6267 7261 6465 722e 6170 7073  om nbgrader.apps
+00000120: 2e62 6173 6561 7070 2069 6d70 6f72 7420  .baseapp import 
+00000130: 4e62 4772 6164 6572 0a66 726f 6d20 6e62  NbGrader.from nb
+00000140: 6772 6164 6572 2e73 6572 7665 725f 6578  grader.server_ex
+00000150: 7465 6e73 696f 6e73 2e66 6f72 6d67 7261  tensions.formgra
+00000160: 6465 722e 6170 6968 616e 646c 6572 7320  der.apihandlers 
+00000170: 696d 706f 7274 2064 6566 6175 6c74 5f68  import default_h
+00000180: 616e 646c 6572 730a 0a66 726f 6d20 6532  andlers..from e2
+00000190: 7867 7261 6465 722e 7365 7276 6572 5f65  xgrader.server_e
+000001a0: 7874 656e 7369 6f6e 732e 6772 6164 6572  xtensions.grader
+000001b0: 2e61 7070 732e 6261 7365 2069 6d70 6f72  .apps.base impor
+000001c0: 7420 4261 7365 4170 700a 0a66 726f 6d20  t BaseApp..from 
+000001d0: 2e61 7069 6861 6e64 6c65 7273 2069 6d70  .apihandlers imp
+000001e0: 6f72 7420 6465 6661 756c 745f 6861 6e64  ort default_hand
+000001f0: 6c65 7273 0a0a 0a63 6c61 7373 2045 3278  lers...class E2x
+00000200: 4772 6164 6572 4170 6928 4e62 4772 6164  GraderApi(NbGrad
+00000210: 6572 2c20 4261 7365 4170 7029 3a0a 2020  er, BaseApp):.  
+00000220: 2020 7465 6d70 6c61 7465 5f70 6174 6820    template_path 
+00000230: 3d20 6f73 2e70 6174 682e 6a6f 696e 286f  = os.path.join(o
+00000240: 732e 7061 7468 2e64 6972 6e61 6d65 285f  s.path.dirname(_
+00000250: 5f66 696c 655f 5f29 2c20 2274 656d 706c  _file__), "templ
+00000260: 6174 6573 2229 0a0a 2020 2020 6465 6620  ates")..    def 
+00000270: 5f5f 696e 6974 5f5f 2873 656c 662c 202a  __init__(self, *
+00000280: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+00000290: 2020 4e62 4772 6164 6572 2e5f 5f69 6e69    NbGrader.__ini
+000002a0: 745f 5f28 7365 6c66 2c20 2a2a 6b77 6172  t__(self, **kwar
+000002b0: 6773 290a 2020 2020 2020 2020 4261 7365  gs).        Base
+000002c0: 4170 702e 5f5f 696e 6974 5f5f 2873 656c  App.__init__(sel
+000002d0: 662c 202a 2a6b 7761 7267 7329 0a0a 2020  f, **kwargs)..  
+000002e0: 2020 6465 6620 6c6f 6164 5f61 7070 2873    def load_app(s
+000002f0: 656c 6629 3a0a 2020 2020 2020 2020 7365  elf):.        se
+00000300: 6c66 2e6c 6f67 2e69 6e66 6f28 224c 6f61  lf.log.info("Loa
+00000310: 6469 6e67 2074 6865 2065 3278 6772 6164  ding the e2xgrad
+00000320: 6572 2061 7069 2061 7070 2229 0a20 2020  er api app").   
+00000330: 2020 2020 2073 656c 662e 6164 645f 7465       self.add_te
+00000340: 6d70 6c61 7465 5f70 6174 6828 7365 6c66  mplate_path(self
+00000350: 2e74 656d 706c 6174 655f 7061 7468 290a  .template_path).
+00000360: 2020 2020 2020 2020 7365 6c66 2e61 6464          self.add
+00000370: 5f68 616e 646c 6572 7328 6465 6661 756c  _handlers(defaul
+00000380: 745f 6861 6e64 6c65 7273 290a            t_handlers).
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Autograded).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Code (Manual).ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Diagram.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Diagram.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Freetext.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Freetext.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Multiple Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Single Choice.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Single Choice.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Upload Files.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/questions/Upload Files.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Footer.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Footer.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Group Info.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Group Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Header.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Header.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Student Info.ipynb` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/presets/template/Student Info.ipynb`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/index.html.j2` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/e2xgraderapi/templates/feedback/index.html.j2`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/formgrader.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/formgrader.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class FormgradeApp(NbGrader, BaseApp):
     template_path = os.path.join(os.path.dirname(__file__), "templates")
     static_path = os.path.join(os.path.dirname(__file__), "static")
 
     def __init__(self, **kwargs):
         NbGrader.__init__(self, **kwargs)
         BaseApp.__init__(self, **kwargs)
-        self.load_config_file()
+        self.initialize([])
         if not self.config.has_key(
             "HTMLExporter"
         ) or not self.config.HTMLExporter.has_key("template_name"):
             self.config.HTMLExporter.template_name = "formgrade"
 
     def load_app(self):
         self.log.info("Loading the formgrader app")
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/handlers.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/handlers.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/css/eraser-solid.svg` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/css/eraser-solid.svg`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/css/pencil-solid.svg` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/css/pencil-solid.svg`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade_models.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/formgrade_models.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_assignments.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_assignments.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebook_submissions.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebook_submissions.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebooks.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_notebooks.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_tasks.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/gradebook_tasks.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_assignments.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_assignments.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_submissions.js` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/static/js/manage_submissions.js`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/base.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/base.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/export_grades.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/export_grades.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_assignments.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_assignments.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_submissions.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/manage_submissions.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/formgrade_macros.html.j2` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/formgrade_macros.html.j2`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/index.html.j2` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/formgrade/index.html.j2`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_assignments.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_assignments.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebook_submissions.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebooks.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_notebooks.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_tasks.tpl` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/formgrader/templates/task_view/gradebook_tasks.tpl`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/grader/apps/nbgraderapi/nbgraderapi.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/grader/apps/nbgraderapi/nbgraderapi.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/server_extensions/validate_assignment/handlers.py` & `e2xgrader-0.1.0.dev3/e2xgrader/server_extensions/validate_assignment/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 "The notebook '{}' uses a newer version "
                 "of the nbgrader metadata format. Please update your version of "
                 "nbgrader to the latest version to be able to use this notebook."
             ).format(fullpath)
             self.log.error(msg)
             retvalue = {"success": False, "value": msg}
 
-        except:
+        except Exception:
             self.log.error(traceback.format_exc())
             retvalue = {"success": False, "value": traceback.format_exc()}
 
         else:
             retvalue = {"success": True, "value": result}
 
         return retvalue
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/test_validator.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/apps/test_e2xgraderapp.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/apps/test_e2xgraderapp.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/converters/test_generateexercise.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/converters/test_generateexercise.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/exporters/filters/test_highlight.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/exporters/filters/test_highlight.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_base.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/graders/test_base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_code.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/graders/test_code.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_multiplechoice.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/graders/test_multiplechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/graders/test_singlechoice.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/graders/test_singlechoice.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_assignmentmodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_assignmentmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_basemodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_basemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_exercisemodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_exercisemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_presetmodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_presetmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_taskmodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_taskmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_taskpoolmodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_taskpoolmodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/models/test_templatemodel.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/models/test_templatemodel.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_clearhiddentests.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_clearhiddentests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_clearsolutions.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_clearsolutions.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_extractattachments.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_extractattachments.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_filtercellsbyid.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_filtercellsbyid.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_filtertests.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_filtertests.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_unscramble.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_unscramble.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,18 @@
         self.nb.cells.extend(
             [
                 new_manually_graded_markdown_cell(
                     source="Here we want to replace {{ myvar1   }}!"
                 ),
                 new_readonly_code_cell(source="# Here we want to replace {{myvar2 }}"),
                 new_manually_graded_code_cell(
-                    source="# Here we want to replace everything {{myvar1}} {{ myvar2 }} and {{ somevar }}"
+                    source=(
+                        "# Here we want to replace everything {{myvar1}} "
+                        "{{ myvar2 }} and {{ somevar }}"
+                    )
                 ),
             ]
         )
 
     def test_unscramble(self):
         nb = deepcopy(self.nb)
         processed_nb, _ = Unscramble().preprocess(nb, {})
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/test_validateextracells.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/test_validateextracells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/base.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/authoring/base.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/test_copyfiles.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/authoring/test_copyfiles.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/preprocessors/authoring/test_copynotebooks.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/preprocessors/authoring/test_copynotebooks.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/cells.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/test_utils/cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Union
+from typing import Any, Dict, Union
 
 from nbformat.notebooknode import NotebookNode
 from nbformat.v4 import new_code_cell, new_markdown_cell
 
 
 def nbgrader_metadata(**kwargs) -> Dict[str, Union[int, str, bool]]:
     """Create an nbgrader metadata dictionary
```

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/test_utils/test_utils.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/test_utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_extra_cells.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/utils/test_extra_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_nbgrader_cells.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/utils/test_nbgrader_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/tests/utils/test_notebookvariableextractor.py` & `e2xgrader-0.1.0.dev3/e2xgrader/tests/utils/test_notebookvariableextractor.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/utils/extra_cells.py` & `e2xgrader-0.1.0.dev3/e2xgrader/utils/extra_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/e2xgrader/utils/nbgrader_cells.py` & `e2xgrader-0.1.0.dev3/e2xgrader/utils/nbgrader_cells.py`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/.gitignore` & `e2xgrader-0.1.0.dev3/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -130,7 +130,10 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+
+# vscode
+.vscode/
```

### Comparing `e2xgrader-0.1.0.dev1/LICENSE` & `e2xgrader-0.1.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/README.md` & `e2xgrader-0.1.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `e2xgrader-0.1.0.dev1/pyproject.toml` & `e2xgrader-0.1.0.dev3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,21 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
-    "nbgrader==0.7.1",
-    "jupyter-core<4.11.2",
-    "jupyter-client<7.4",
-    "jupyter-server<1.20",
+    "nbgrader==0.7.*",
     "nbconvert>=6.5",
-    "notebook>=6,<6.5",
-    "beautifulsoup4",
+    "notebook>=6,<7",
+    "jupyter-server<2",
+    "jupyter-core<5",
+    "ipykernel<6.19",
+    "nbclient<0.6.4",
     "pandas"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://e2x.inf.h-brs.de"
 Issues = "https://github.com/Digiklausur/e2xgrader/issues"
@@ -62,15 +62,15 @@
 ]
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.1.0-dev1"
+current = "0.1.0-dev3"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
@@ -94,8 +94,12 @@
 
 [[tool.tbump.file]]
 src = "packages/*/package.json"
 search = '"version": "{current_version}'
 
 [[tool.tbump.file]]
 src = "packages/*/package.json"
-search = '"@e2xgrader/\w+": "{current_version}'
+search = '"@e2xgrader/[\w-]+": "{current_version}'
+
+[tool.ruff]
+line-length = 100
+exclude = ["nbgrader_config.py"]
```

### Comparing `e2xgrader-0.1.0.dev1/PKG-INFO` & `e2xgrader-0.1.0.dev3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: e2xgrader
-Version: 0.1.0.dev1
+Version: 0.1.0.dev3
 Summary: An addon for nbgrader
 Project-URL: Documentation, https://e2x.inf.h-brs.de
 Project-URL: Issues, https://github.com/Digiklausur/e2xgrader/issues
 Project-URL: Source, https://github.com/Digiklausur/e2xgrader
 Author-email: Tim Metzler <tim.metzler@h-brs.de>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.7
-Requires-Dist: beautifulsoup4
-Requires-Dist: jupyter-client<7.4
-Requires-Dist: jupyter-core<4.11.2
-Requires-Dist: jupyter-server<1.20
+Requires-Dist: ipykernel<6.19
+Requires-Dist: jupyter-core<5
+Requires-Dist: jupyter-server<2
+Requires-Dist: nbclient<0.6.4
 Requires-Dist: nbconvert>=6.5
-Requires-Dist: nbgrader==0.7.1
-Requires-Dist: notebook<6.5,>=6
+Requires-Dist: nbgrader==0.7.*
+Requires-Dist: notebook<7,>=6
 Requires-Dist: pandas
 Provides-Extra: dev
 Requires-Dist: hatchling; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: tbump; extra == 'dev'
 Description-Content-Type: text/markdown
```

