# Comparing `tmp/gamma-facet-2.0rc1.tar.gz` & `tmp/gamma-facet-2.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamma-facet-2.0rc1.tar", last modified: Sat Sep 24 08:22:34 2022, max compression
+gzip compressed data, was "gamma-facet-2.0rc2.tar", last modified: Tue Jan 24 11:59:13 2023, max compression
```

## Comparing `gamma-facet-2.0rc1.tar` & `gamma-facet-2.0rc2.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0      666 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      689 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     4886 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/.gitignore
--rw-r--r--   0        0        0     1131 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11358 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/LICENSE
--rw-r--r--   0        0        0    20738 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/README.rst
--rw-r--r--   0        0        0     6286 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/RELEASE_NOTES.rst
--rw-r--r--   0        0        0    25542 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/azure-pipelines.yml
--rw-r--r--   0        0        0     2294 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/condabuild/meta.yaml
--rw-r--r--   0        0        0        0 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/config/spelling.dic
--rw-r--r--   0        0        0      124 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/config/test_config.yml
--rwxr-xr-x   0        0        0       93 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/dev-setup.sh
--rw-r--r--   0        0        0      914 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/environment.yml
--rwxr-xr-x   0        0        0      380 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/make.py
--rw-r--r--   0        0        0      751 2022-09-24 08:21:01.327170 gamma-facet-2.0rc1/mypy.ini
--rw-r--r--   0        0        0     2717 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/pypi_description.rst
--rw-r--r--   0        0        0     3855 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/pyproject.toml
--rw-r--r--   0        0        0       37 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/.gitignore
--rw-r--r--   0        0        0   199639 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/auxiliary/Diabetes_getting_started_example.ipynb
--rw-r--r--   0        0        0    10223 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb
--rwxr-xr-x   0        0        0      664 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/make.py
--rw-r--r--   0        0        0   130308 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/source/_images/Facet-Simulator-BlockDiagram.png
--rw-r--r--   0        0        0    19522 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/source/_images/Facet_Logo_Plain.png
--rw-r--r--   0        0        0     5238 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/source/_images/Facet_flow.svg
--rw-r--r--   0        0        0     7117 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg
--rw-r--r--   0        0        0    23632 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/source/_images/facet_banner.png
--rw-r--r--   0        0        0     1429 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/source/_images/icons/inspect_icon.png
--rw-r--r--   0        0        0     2777 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/source/_images/icons/pipe_icon.png
--rw-r--r--   0        0        0     2718 2022-09-24 08:21:01.331170 gamma-facet-2.0rc1/sphinx/source/_images/icons/sim_icon.png
--rw-r--r--   0        0        0   117900 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/ranker_summary.png
--rw-r--r--   0        0        0    27724 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/redundancy_dendrogram.png
--rw-r--r--   0        0        0    31712 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/redundancy_matrix.png
--rw-r--r--   0        0        0    38185 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/simulation_output.png
--rw-r--r--   0        0        0    31278 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/synergy_matrix.png
--rw-r--r--   0        0        0    49407 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Andy_Shora.jpg
--rw-r--r--   0        0        0     9901 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Florent_Martin.jpg
--rw-r--r--   0        0        0    11856 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Jan_Ittner.jpg
--rw-r--r--   0        0        0     8047 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Jason_Bentley.jpg
--rw-r--r--   0        0        0    10116 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg
--rw-r--r--   0        0        0     6673 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg
--rw-r--r--   0        0        0     9583 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Malo_Grisard.jpg
--rw-r--r--   0        0        0    49773 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg
--rw-r--r--   0        0        0    10100 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg
--rw-r--r--   0        0        0    10746 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg
--rw-r--r--   0        0        0      232 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/_static/css/facet.css
--rw-r--r--   0        0        0     3673 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/about_us.rst
--rw-r--r--   0        0        0      371 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/api_landing.rst
--rw-r--r--   0        0        0      758 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/conf.py
--rw-r--r--   0        0        0    20763 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/contribution_guide.rst
--rw-r--r--   0        0        0     5693 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/faqs.rst
--rw-r--r--   0        0        0      298 2022-09-24 08:21:01.335170 gamma-facet-2.0rc1/sphinx/source/index.rst
--rw-r--r--   0        0        0  1644456 2022-09-24 08:21:01.351171 gamma-facet-2.0rc1/sphinx/source/tutorial/Classification_with_Facet.ipynb
--rw-r--r--   0        0        0   970457 2022-09-24 08:21:01.355171 gamma-facet-2.0rc1/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv
--rw-r--r--   0        0        0   232448 2022-09-24 08:21:01.355171 gamma-facet-2.0rc1/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb
--rw-r--r--   0        0        0   107691 2022-09-24 08:21:01.355171 gamma-facet-2.0rc1/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb
--rw-r--r--   0        0        0   475484 2022-09-24 08:21:01.359171 gamma-facet-2.0rc1/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb
--rw-r--r--   0        0        0   820532 2022-09-24 08:21:01.363171 gamma-facet-2.0rc1/sphinx/source/tutorial/pre_diab_nhanes.csv
--rw-r--r--   0        0        0    85389 2022-09-24 08:21:01.363171 gamma-facet-2.0rc1/sphinx/source/tutorial/water_drilling_classification_data.csv
--rw-r--r--   0        0        0     2402 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/sphinx/source/tutorials.rst
--rw-r--r--   0        0        0      601 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/__init__.py
--rw-r--r--   0        0        0      102 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/data/__init__.py
--rw-r--r--   0        0        0    11804 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/data/_sample.py
--rw-r--r--   0        0        0      272 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/data/partition/__init__.py
--rw-r--r--   0        0        0    14187 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/data/partition/_partition.py
--rw-r--r--   0        0        0      394 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/inspection/__init__.py
--rw-r--r--   0        0        0    20829 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/inspection/_explainer.py
--rw-r--r--   0        0        0     1859 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/inspection/_inspection.py
--rw-r--r--   0        0        0    42361 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/inspection/_learner_inspector.py
--rw-r--r--   0        0        0    25798 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/inspection/_shap.py
--rw-r--r--   0        0        0    24909 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/inspection/_shap_global_explanation.py
--rw-r--r--   0        0        0    10616 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/inspection/_shap_projection.py
--rw-r--r--   0        0        0        0 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/py.typed
--rw-r--r--   0        0        0      113 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/selection/__init__.py
--rw-r--r--   0        0        0    13100 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/selection/_parameters.py
--rw-r--r--   0        0        0    17587 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/selection/_selection.py
--rw-r--r--   0        0        0      107 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/selection/base/__init__.py
--rw-r--r--   0        0        0     7520 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/selection/base/_parameters.py
--rw-r--r--   0        0        0      318 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/simulation/__init__.py
--rw-r--r--   0        0        0     5452 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/simulation/_result.py
--rw-r--r--   0        0        0     9021 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/simulation/_simulation.py
--rw-r--r--   0        0        0       58 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/simulation/base/__init__.py
--rw-r--r--   0        0        0     9142 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/simulation/base/_base.py
--rw-r--r--   0        0        0       95 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/simulation/viz/__init__.py
--rw-r--r--   0        0        0     4244 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/simulation/viz/_draw.py
--rw-r--r--   0        0        0    12875 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/simulation/viz/_style.py
--rw-r--r--   0        0        0      125 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/validation/__init__.py
--rw-r--r--   0        0        0     9282 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/src/facet/validation/_validation.py
--rw-r--r--   0        0        0        0 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/__init__.py
--rw-r--r--   0        0        0    15198 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/conftest.py
--rw-r--r--   0        0        0        0 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/facet/__init__.py
--rw-r--r--   0        0        0    24768 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/facet/test_inspection.py
--rw-r--r--   0        0        0     4351 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/facet/test_partition.py
--rw-r--r--   0        0        0     4933 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/facet/test_sample.py
--rw-r--r--   0        0        0    13791 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/facet/test_selection.py
--rw-r--r--   0        0        0     1797 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/facet/test_shap_decomposition.py
--rw-r--r--   0        0        0    13806 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/facet/test_simulation.py
--rw-r--r--   0        0        0     5749 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/facet/test_validation.py
--rw-r--r--   0        0        0      263 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/paths.py
--rw-r--r--   0        0        0      216 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/test/test/test_docs.py
--rw-r--r--   0        0        0     2594 2022-09-24 08:21:01.367172 gamma-facet-2.0rc1/tox.ini
--rw-r--r--   0        0        0     4924 1970-01-01 00:00:00.000000 gamma-facet-2.0rc1/PKG-INFO
+-rw-r--r--   0        0        0      666 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      689 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     4886 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/.gitignore
+-rw-r--r--   0        0        0     1129 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11358 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/LICENSE
+-rw-r--r--   0        0        0    20819 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/README.rst
+-rw-r--r--   0        0        0     6385 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/RELEASE_NOTES.rst
+-rw-r--r--   0        0        0    25478 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/azure-pipelines.yml
+-rw-r--r--   0        0        0     2294 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/condabuild/meta.yaml
+-rw-r--r--   0        0        0        0 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/config/spelling.dic
+-rw-r--r--   0        0        0      124 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/config/test_config.yml
+-rwxr-xr-x   0        0        0       93 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/dev-setup.sh
+-rw-r--r--   0        0        0      988 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/environment.yml
+-rwxr-xr-x   0        0        0      380 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/make.py
+-rw-r--r--   0        0        0      751 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/mypy.ini
+-rw-r--r--   0        0        0     2717 2023-01-24 11:57:26.340291 gamma-facet-2.0rc2/pypi_description.rst
+-rw-r--r--   0        0        0     3875 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/.gitignore
+-rw-r--r--   0        0        0   199639 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/auxiliary/Diabetes_getting_started_example.ipynb
+-rw-r--r--   0        0        0    10223 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb
+-rwxr-xr-x   0        0        0      664 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/make.py
+-rw-r--r--   0        0        0   130308 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/Facet-Simulator-BlockDiagram.png
+-rw-r--r--   0        0        0    19522 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/Facet_Logo_Plain.png
+-rw-r--r--   0        0        0     5238 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/Facet_flow.svg
+-rw-r--r--   0        0        0     7117 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg
+-rw-r--r--   0        0        0    23632 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/facet_banner.png
+-rw-r--r--   0        0        0     1429 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/icons/inspect_icon.png
+-rw-r--r--   0        0        0     2777 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/icons/pipe_icon.png
+-rw-r--r--   0        0        0     2718 2023-01-24 11:57:26.344291 gamma-facet-2.0rc2/sphinx/source/_images/icons/sim_icon.png
+-rw-r--r--   0        0        0   117900 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/ranker_summary.png
+-rw-r--r--   0        0        0    27724 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/redundancy_dendrogram.png
+-rw-r--r--   0        0        0    31712 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/redundancy_matrix.png
+-rw-r--r--   0        0        0    38185 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/simulation_output.png
+-rw-r--r--   0        0        0    31278 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/synergy_matrix.png
+-rw-r--r--   0        0        0    49407 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Andy_Shora.jpg
+-rw-r--r--   0        0        0     9901 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Florent_Martin.jpg
+-rw-r--r--   0        0        0    11856 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Jan_Ittner.jpg
+-rw-r--r--   0        0        0     8047 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Jason_Bentley.jpg
+-rw-r--r--   0        0        0    10116 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg
+-rw-r--r--   0        0        0     6673 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg
+-rw-r--r--   0        0        0     9583 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Malo_Grisard.jpg
+-rw-r--r--   0        0        0    49773 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg
+-rw-r--r--   0        0        0    10100 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg
+-rw-r--r--   0        0        0    10746 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg
+-rw-r--r--   0        0        0      232 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/_static/css/facet.css
+-rw-r--r--   0        0        0     3673 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/about_us.rst
+-rw-r--r--   0        0        0      371 2023-01-24 11:57:26.348291 gamma-facet-2.0rc2/sphinx/source/api_landing.rst
+-rw-r--r--   0        0        0      758 2023-01-24 11:57:26.352291 gamma-facet-2.0rc2/sphinx/source/conf.py
+-rw-r--r--   0        0        0    20763 2023-01-24 11:57:26.352291 gamma-facet-2.0rc2/sphinx/source/contribution_guide.rst
+-rw-r--r--   0        0        0     5693 2023-01-24 11:57:26.352291 gamma-facet-2.0rc2/sphinx/source/faqs.rst
+-rw-r--r--   0        0        0      298 2023-01-24 11:57:26.352291 gamma-facet-2.0rc2/sphinx/source/index.rst
+-rw-r--r--   0        0        0  1644456 2023-01-24 11:57:26.364291 gamma-facet-2.0rc2/sphinx/source/tutorial/Classification_with_Facet.ipynb
+-rw-r--r--   0        0        0   970457 2023-01-24 11:57:26.368291 gamma-facet-2.0rc2/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv
+-rw-r--r--   0        0        0   232448 2023-01-24 11:57:26.368291 gamma-facet-2.0rc2/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb
+-rw-r--r--   0        0        0   107691 2023-01-24 11:57:26.368291 gamma-facet-2.0rc2/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb
+-rw-r--r--   0        0        0   475484 2023-01-24 11:57:26.372291 gamma-facet-2.0rc2/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb
+-rw-r--r--   0        0        0   820532 2023-01-24 11:57:26.376291 gamma-facet-2.0rc2/sphinx/source/tutorial/pre_diab_nhanes.csv
+-rw-r--r--   0        0        0    85389 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/sphinx/source/tutorial/water_drilling_classification_data.csv
+-rw-r--r--   0        0        0     2402 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/sphinx/source/tutorials.rst
+-rw-r--r--   0        0        0      601 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/__init__.py
+-rw-r--r--   0        0        0      102 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/data/__init__.py
+-rw-r--r--   0        0        0    11804 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/data/_sample.py
+-rw-r--r--   0        0        0      272 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/data/partition/__init__.py
+-rw-r--r--   0        0        0    14152 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/data/partition/_partition.py
+-rw-r--r--   0        0        0      394 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/__init__.py
+-rw-r--r--   0        0        0    20829 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_explainer.py
+-rw-r--r--   0        0        0     1859 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_inspection.py
+-rw-r--r--   0        0        0    42261 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_learner_inspector.py
+-rw-r--r--   0        0        0    25729 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_shap.py
+-rw-r--r--   0        0        0    24909 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_shap_global_explanation.py
+-rw-r--r--   0        0        0    10616 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/inspection/_shap_projection.py
+-rw-r--r--   0        0        0        0 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/py.typed
+-rw-r--r--   0        0        0      113 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/__init__.py
+-rw-r--r--   0        0        0    13163 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/_parameters.py
+-rw-r--r--   0        0        0    17575 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/_selection.py
+-rw-r--r--   0        0        0      107 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/base/__init__.py
+-rw-r--r--   0        0        0     7599 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/selection/base/_parameters.py
+-rw-r--r--   0        0        0      318 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/__init__.py
+-rw-r--r--   0        0        0     5452 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/_result.py
+-rw-r--r--   0        0        0     9103 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/_simulation.py
+-rw-r--r--   0        0        0       58 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/base/__init__.py
+-rw-r--r--   0        0        0     9474 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/base/_base.py
+-rw-r--r--   0        0        0       95 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/viz/__init__.py
+-rw-r--r--   0        0        0     4244 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/viz/_draw.py
+-rw-r--r--   0        0        0    12875 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/simulation/viz/_style.py
+-rw-r--r--   0        0        0      125 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/validation/__init__.py
+-rw-r--r--   0        0        0     9263 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/src/facet/validation/_validation.py
+-rw-r--r--   0        0        0        0 2023-01-24 11:57:26.380291 gamma-facet-2.0rc2/test/test/__init__.py
+-rw-r--r--   0        0        0    15366 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/conftest.py
+-rw-r--r--   0        0        0        0 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/__init__.py
+-rw-r--r--   0        0        0    24768 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_inspection.py
+-rw-r--r--   0        0        0     4351 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_partition.py
+-rw-r--r--   0        0        0     5085 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_sample.py
+-rw-r--r--   0        0        0    14023 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_selection.py
+-rw-r--r--   0        0        0     1797 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_shap_decomposition.py
+-rw-r--r--   0        0        0    13500 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_simulation.py
+-rw-r--r--   0        0        0     5524 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/facet/test_validation.py
+-rw-r--r--   0        0        0      263 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/paths.py
+-rw-r--r--   0        0        0      216 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/test/test/test_docs.py
+-rw-r--r--   0        0        0     2594 2023-01-24 11:57:26.384291 gamma-facet-2.0rc2/tox.ini
+-rw-r--r--   0        0        0     4934 1970-01-01 00:00:00.000000 gamma-facet-2.0rc2/PKG-INFO
```

### Comparing `gamma-facet-2.0rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `gamma-facet-2.0rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `gamma-facet-2.0rc2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/.gitignore` & `gamma-facet-2.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/.pre-commit-config.yaml` & `gamma-facet-2.0rc2/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
       - id: check-json
       - id: check-xml
       - id: check-yaml
         language: python_venv
         exclude: condabuild/meta.yaml
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.971
+    rev: v0.981
     hooks:
       - id: mypy
         files: src|sphinx|test
         language: python_venv
         language_version: python39
         additional_dependencies:
           - numpy~=1.22
-          - gamma-pytools~=2.0,!=2.0.0
-          - sklearndf~=2.0
+          - gamma-pytools~=2.1rc
+          - sklearndf~=2.2.dev
```

### Comparing `gamma-facet-2.0rc1/LICENSE` & `gamma-facet-2.0rc2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright 2020-2021 Boston Consulting Group
+   Copyright 2020-2023 Boston Consulting Group
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `gamma-facet-2.0rc1/README.rst` & `gamma-facet-2.0rc2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 .. image:: sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg
 
 |
 
+**Release Candidate 2.0rc available now!**
+
+|
+
 FACET is an open source library for human-explainable AI.
 It combines sophisticated model inspection and model-based simulation to enable better 
 explanations of your supervised machine learning models.
 
 FACET is composed of the following key components:
 
 +-----------------+-----------------------------------------------------------------------+
@@ -76,18 +80,18 @@
 
 Quickstart
 ----------
 
 The following quickstart guide provides a minimal example workflow to get you
 up and running with FACET.
 For additional tutorials and the API reference,
-see the `FACET documentation <https://bcg-gamma.github.io/facet/>`__.
+see the `FACET documentation <https://bcg-gamma.github.io/facet/docs-version/2-0>`__.
 
 Changes and additions to new versions are summarized in the
-`release notes <https://bcg-gamma.github.io/facet/release_notes.html>`__.
+`release notes <https://bcg-gamma.github.io/facet/docs-version/2-0/release_notes.html>`__.
 
 
 Enhanced Machine Learning Workflow
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To demonstrate the model inspection capability of FACET, we first create a
 pipeline to fit a learner. In this simple example we will use the
@@ -463,8 +467,8 @@
 
 .. |made_with_sphinx_doc| image:: https://img.shields.io/badge/Made%20with-Sphinx-1f425f.svg
    :target: https://bcg-gamma.github.io/facet/index.html
 
 .. |license_badge| image:: https://img.shields.io/badge/License-Apache%202.0-olivegreen.svg
    :target: https://opensource.org/licenses/Apache-2.0
 
-.. End-Badges
+.. End-Badges
```

### Comparing `gamma-facet-2.0rc1/RELEASE_NOTES.rst` & `gamma-facet-2.0rc2/RELEASE_NOTES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,16 @@
 - API: removed class ``FullSampleValidator``
 
 Other
 ^^^^^
 
 - API: class ``LearnerCrossfit`` is no longer needed in FACET |nbsp| 2.0 and has been
   removed
+- API: support new :obj:`~pytools.fit.fitted_only` decorator introduced in *pytools*
+  |nbsp| 2.1.
 
 
 FACET 1.2
 ---------
 
 FACET |nbsp| 1.2 adds support for *sklearndf* |nbsp| 1.2 and *scikit-learn* |nbsp| 0.24.
 It also introduces the ability to run simulations on a subsample of the data used to
```

### Comparing `gamma-facet-2.0rc1/azure-pipelines.yml` & `gamma-facet-2.0rc2/azure-pipelines.yml`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # run tests and full conda/tox build matrix every night at 4am
 schedules:
   - cron: "0 4 * * 1-5"
     displayName: Nightly full build
     branches:
       include:
-        - 1.2.x
+        - 2.0.x
 
 resources:
   repositories:
     - repository: pytools
       type: github
       endpoint: BCG-Gamma
       name: BCG-Gamma/pytools
@@ -83,15 +83,15 @@
         displayName: 'mypy'
         steps:
           - task: UsePythonVersion@0
             inputs:
               versionSpec: '3.9'
             displayName: 'use Python 3.9'
           - script: |
-              python -m pip install mypy~=0.971 numpy~=1.22 gamma-pytools~=2.0,!=2.0.0 sklearndf~=2.0
+              python -m pip install mypy~=0.981 numpy~=1.22 'gamma-pytools~=2.1rc' sklearndf~=2.2.dev
               python -m mypy src
             displayName: 'Run mypy'
 
   # detect whether the build config (pyproject.toml) was changed -> then we must run a build test
   - stage: detect_build_config_changes
     displayName: 'Pyproject.toml build config'
 
@@ -128,14 +128,16 @@
     displayName: 'Unit tests'
     dependsOn: 'detect_build_config_changes'
     variables:
       conda_build_config_changed: $[ stageDependencies.detect_build_config_changes.checkout_and_diff.outputs['diff.conda_build_config_changed'] ]
 
     jobs:
       - job:
+        timeoutInMinutes: 120
+        cancelTimeoutInMinutes: 3
         displayName: 'pytest @ develop environment'
         condition: ne(variables.source_is_release_branch, 'True')
 
         pool:
           vmImage: 'ubuntu-latest'
 
         steps:
@@ -150,18 +152,16 @@
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
                 eval "$(conda shell.bash hook)"
-
                 conda env create
                 conda activate $(project_name)-develop
-
                 export PYTHONPATH=$(System.DefaultWorkingDirectory)/src/
                 export RUN_PACKAGE_VERSION_TEST=$(project_name)
 
                 pytest \
                    --cov $(project_name) \
                    --cov-config "tox.ini" \
                    --cov-report=xml:coverage.xml --cov-report=html:htmlcov \
@@ -607,26 +607,25 @@
           - task: InstallSSHKey@0
             inputs:
               knownHostsEntry: $(knownHostsEntry)
               sshPublicKey: $(sshPublicKey)
               sshKeySecureFile: 'deploy_docs_$(project_name)'
             displayName: 'Install the deploy SSH key'
 
-          - checkout: pytools
           - checkout: self
 
           - script: dir $(Build.SourcesDirectory)
 
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
 
-                cd $(System.DefaultWorkingDirectory)/$(project_root)
+                cd $(System.DefaultWorkingDirectory)
                 echo "Checking out github-pages"
                 git checkout --track origin/github-pages
 
                 # make sure we have a docs directory
                 mkdir -p docs/docs-version
 
                 echo "Current documentation contents:"
@@ -640,22 +639,22 @@
           - task: Bash@3
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
                 eval "$(conda shell.bash hook)"
 
-                cd $(System.DefaultWorkingDirectory)/$(project_root)
+                cd $(System.DefaultWorkingDirectory)
                 echo "Checking out $(branchName)"
                 git checkout $(branchName)
 
                 conda env create
                 conda activate $(project_name)-develop
 
-                export PYTHONPATH=$(System.DefaultWorkingDirectory)/$(project_root)/src/
+                export PYTHONPATH=$(System.DefaultWorkingDirectory)/src/
 
                 python sphinx/make.py html
 
             displayName: 'Build latest documentation'
 
           - task: Bash@3
             inputs:
@@ -663,22 +662,22 @@
               script: |
                 set -eux
                 eval "$(conda shell.bash hook)"
 
                 # install the tree utility
                 sudo apt-get install tree
 
-                cd $(System.DefaultWorkingDirectory)/$(project_root)
+                cd $(System.DefaultWorkingDirectory)
 
                 echo "Restoring previous documentation to the docs directory"
                 mkdir -p docs
                 mv $(Build.ArtifactStagingDirectory)/docs-version.bak docs/docs-version
                 ls docs/docs-version
 
-                mkdir -p $(System.DefaultWorkingDirectory)/$(project_root)/sphinx/build/
+                mkdir -p $(System.DefaultWorkingDirectory)/sphinx/build/
 
                 conda activate $(project_name)-develop
                 python sphinx/make.py prepare_docs_deployment
 
                 echo "Current docs contents:"
                 tree docs
                 mv docs $(Build.ArtifactStagingDirectory)/docs
@@ -704,15 +703,15 @@
 
           - task: Bash@3
             condition: eq(variables['source_is_release_branch'], 'True')
             inputs:
               targetType: 'inline'
               script: |
                 set -eux
-                cd $(System.DefaultWorkingDirectory)/$(project_root)
+                cd $(System.DefaultWorkingDirectory)
 
                 echo "Adjusting git credentials"
                 git config --global user.name "Azure Pipelines"
                 git config --global user.email "azuredevops@microsoft.com"
                 git config --global url.ssh://git@github.com/.insteadOf https://github.com/
                 git checkout github-pages
```

### Comparing `gamma-facet-2.0rc1/condabuild/meta.yaml` & `gamma-facet-2.0rc2/condabuild/meta.yaml`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/environment.yml` & `gamma-facet-2.0rc2/environment.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 name: facet-develop
 channels:
   - conda-forge
   - bcg_gamma
 dependencies:
   # run
   - boruta_py ~= 0.3
-  - gamma-pytools ~= 2.0.4
-  - joblib ~= 1.1
-  - lightgbm ~= 3.3
-  - matplotlib ~= 3.5
-  - numpy ~= 1.22
-  - pandas ~= 1.4
-  - python ~= 3.9
-  - scikit-learn ~= 1.1
-  - scipy ~= 1.8
+  - gamma-pytools >= 2.1rc1, <3a
+  - joblib ~= 1.2
+  - lightgbm ~= 3.3.4
+  - matplotlib ~= 3.6.3
+  - numpy ~= 1.23.5
+  - pandas ~= 1.5.3
+  - python ~= 3.9.15
+  - scikit-learn ~= 1.2.0
+  - scipy ~= 1.10.0
   - shap ~= 0.41
-  - sklearndf ~= 2.0
+  - sklearndf >= 2.2rc, < 3a
   # build/test
-  - conda-build ~= 3.21
-  - conda-verify ~= 3.1
-  - docutils ~= 0.17
-  - flit ~= 3.0
-  - jinja2 ~= 2.11
+  - conda-build ~= 3.23.3
+  - conda-verify ~= 3.1.1
+  - docutils ~= 0.17.1
+  - flit ~= 3.8.0
+  - jinja2 ~= 2.11.3
   - markupsafe ~= 2.0.1  # markupsafe 2.1 breaks support for jinja2
-  - m2r ~= 0.2
-  - pluggy ~= 0.13
-  - pre-commit ~= 2.20
-  - pytest ~= 7.1
-  - pytest-cov ~= 2.12
-  - pyyaml ~= 5.4
-  - toml ~= 0.10
-  - tox ~= 3.24
-  - yaml ~= 0.2
+  - m2r ~= 0.3.1
+  - pluggy ~= 0.13.1
+  - pre-commit ~= 2.21.0
+  - pytest ~= 7.2.1
+  - pytest-cov ~= 2.12.1
+  - pyyaml ~= 5.4.1
+  - toml ~= 0.10.2
+  - tox ~= 3.27.1
+  - yaml ~= 0.2.5
   # sphinx
   - nbsphinx ~= 0.8.9
-  - sphinx ~= 4.5
-  - sphinx-autodoc-typehints ~= 1.19
+  - sphinx ~= 4.5.0
+  - sphinx-autodoc-typehints ~= 1.19.2
   - pydata-sphinx-theme ~= 0.8.1
   # notebooks
-  - ipywidgets ~= 8.0
-  - jupyterlab ~= 3.2
-  - openpyxl ~= 3.0
-  - seaborn ~= 0.11
-  - tableone ~= 0.7
+  - ipywidgets ~= 8.0.4
+  - jupyterlab ~= 3.5.2
+  - openpyxl ~= 3.0.10
+  - seaborn ~= 0.12.2
+  - tableone ~= 0.7.12
```

### Comparing `gamma-facet-2.0rc1/mypy.ini` & `gamma-facet-2.0rc2/mypy.ini`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/pypi_description.rst` & `gamma-facet-2.0rc2/pypi_description.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/pyproject.toml` & `gamma-facet-2.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 author = "Boston Consulting Group (BCG)"
 home-page = "https://github.com/BCG-Gamma/facet"
 description-file = "pypi_description.rst"
 dist-name = "gamma-facet"
 license = "Apache Software License v2.0"
 
 requires = [
-    "gamma-pytools  ~=2.0.4",
+    "gamma-pytools  >=2.1rc,<3a",
     "matplotlib     ~=3.0",
     "numpy          >=1.21,<2a",  # cannot use ~= due to conda bug
     "packaging      >=20",
     "pandas         ~=1.0",
     "scipy          ~=1.2",
     "shap           >=0.34,<0.42a",
-    "sklearndf      ~=2.0",
+    "sklearndf      >=2.2rc,<3a",
 ]
 
 requires-python = ">=3.7,<4a"
 
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Science/Research",
@@ -70,46 +70,46 @@
 
 [build]
 # comma-separated list of packages to be built from source in pip min builds
 no-binary.min = ["matplotlib", "shap"]
 
 [build.matrix.min]
 # direct requirements of gamma-facet
-gamma-pytools  = "~=2.0.4"
+gamma-pytools  = "~=2.1rc"
 matplotlib     = "~=3.0.3"
 numpy          = "==1.21.6"  # cannot use ~= due to conda bug
 packaging      = "~=20.9"
 pandas         = "~=1.0.5"
 python         = ">=3.7.12,<3.8a"    # cannot use ~= due to conda bug
 scipy          = "~=1.4.1"
 shap           = "~=0.34.0"
-sklearndf      = "~=2.0.1"
+sklearndf      = "~=2.2rc"
 # additional minimum requirements of sklearndf
 boruta         = "~=0.3.0"
 lightgbm       = "~=3.0.0"
-scikit-learn   = "~=0.21.3"
+scikit-learn   = "~=0.24.2"
 xgboost        = "~=1.5"
 # additional minimum requirements of gamma-pytools
 joblib         = "~=0.14.1"
 typing_inspect = "~=0.4.0"
 # additional minimum requirements of shap
 ipython        = "==7.0"
 numba          = "~=0.55"  # required to support numpy 1.21
 
 [build.matrix.max]
 # direct requirements of gamma-facet
-gamma-pytools  = "~=2.0.4"
+gamma-pytools  = ">=2.1rc,<3a"
 matplotlib     = "~=3.5"
 numpy          = ">=1.22,<2a"  # cannot use ~= due to conda bug
 packaging      = ">=20"
 pandas         = "~=1.4"
 python         = ">=3.9,<4a"   # cannot use ~= due to conda bug
 scipy          = "~=1.8"
 shap           = "~=0.41"
-sklearndf      = "~=2.1"
+sklearndf      = ">=2.2rc,<3a"
 # additional maximum requirements of sklearndf
 boruta         = "~=0.3"
 lightgbm       = "~=3.3"
 scikit-learn   = "~=1.1"
 xgboost        = "~=1.5"
 # additional maximum requirements of gamma-pytools
 joblib         = "~=1.1"
```

### Comparing `gamma-facet-2.0rc1/sphinx/auxiliary/Diabetes_getting_started_example.ipynb` & `gamma-facet-2.0rc2/sphinx/auxiliary/Diabetes_getting_started_example.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb` & `gamma-facet-2.0rc2/sphinx/auxiliary/Facet_sphinx_tutorial_template.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/make.py` & `gamma-facet-2.0rc2/sphinx/make.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 """
 Make sphinx documentation using the pytools make utility
 """
 import os
 from urllib import request
 
-BRANCH = "2.0.x"
+BRANCH = "2.1.x"
 
 
 if __name__ == "__main__":
 
     # noinspection PyUnusedLocal
     def run_make(branch: str, working_directory: str) -> None:
         """Stub, overwritten by bootstrap.py"""
```

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/Facet-Simulator-BlockDiagram.png` & `gamma-facet-2.0rc2/sphinx/source/_images/Facet-Simulator-BlockDiagram.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/Facet_Logo_Plain.png` & `gamma-facet-2.0rc2/sphinx/source/_images/Facet_Logo_Plain.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/Facet_flow.svg` & `gamma-facet-2.0rc2/sphinx/source/_images/Facet_flow.svg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg` & `gamma-facet-2.0rc2/sphinx/source/_images/Gamma_Facet_Logo_RGB_LB.svg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/facet_banner.png` & `gamma-facet-2.0rc2/sphinx/source/_images/facet_banner.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/icons/inspect_icon.png` & `gamma-facet-2.0rc2/sphinx/source/_images/icons/inspect_icon.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/icons/pipe_icon.png` & `gamma-facet-2.0rc2/sphinx/source/_images/icons/pipe_icon.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/icons/sim_icon.png` & `gamma-facet-2.0rc2/sphinx/source/_images/icons/sim_icon.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/ranker_summary.png` & `gamma-facet-2.0rc2/sphinx/source/_images/ranker_summary.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/redundancy_dendrogram.png` & `gamma-facet-2.0rc2/sphinx/source/_images/redundancy_dendrogram.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/redundancy_matrix.png` & `gamma-facet-2.0rc2/sphinx/source/_images/redundancy_matrix.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/simulation_output.png` & `gamma-facet-2.0rc2/sphinx/source/_images/simulation_output.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/synergy_matrix.png` & `gamma-facet-2.0rc2/sphinx/source/_images/synergy_matrix.png`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Andy_Shora.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Andy_Shora.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Florent_Martin.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Florent_Martin.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Jan_Ittner.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Jan_Ittner.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Jason_Bentley.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Jason_Bentley.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Joerg_Schneider.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Konstantin_Hemker.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Malo_Grisard.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Malo_Grisard.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Mateusz_Sokol.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Ricardo_Kennedy.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg` & `gamma-facet-2.0rc2/sphinx/source/_images/team_contributors/Sithan_Kanna.jpg`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/about_us.rst` & `gamma-facet-2.0rc2/sphinx/source/about_us.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/conf.py` & `gamma-facet-2.0rc2/sphinx/source/conf.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/contribution_guide.rst` & `gamma-facet-2.0rc2/sphinx/source/contribution_guide.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/faqs.rst` & `gamma-facet-2.0rc2/sphinx/source/faqs.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/tutorial/Classification_with_Facet.ipynb` & `gamma-facet-2.0rc2/sphinx/source/tutorial/Classification_with_Facet.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv` & `gamma-facet-2.0rc2/sphinx/source/tutorial/KAGGLE-Telco-Customer-Churn.csv`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb` & `gamma-facet-2.0rc2/sphinx/source/tutorial/Model_simulation_deep_dive.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb` & `gamma-facet-2.0rc2/sphinx/source/tutorial/Scikit-learn_classifier_summaries_using_FACET.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb` & `gamma-facet-2.0rc2/sphinx/source/tutorial/Water_Drilling_Incident_Classification_with_Facet.ipynb`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/tutorial/pre_diab_nhanes.csv` & `gamma-facet-2.0rc2/sphinx/source/tutorial/pre_diab_nhanes.csv`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/tutorial/water_drilling_classification_data.csv` & `gamma-facet-2.0rc2/sphinx/source/tutorial/water_drilling_classification_data.csv`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/sphinx/source/tutorials.rst` & `gamma-facet-2.0rc2/sphinx/source/tutorials.rst`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/src/facet/__init__.py` & `gamma-facet-2.0rc2/src/facet/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Human-explainable AI.
 
 This is the class and function reference of FACET for advanced model selection,
 inspection, and simulation.
 """
 
 
-__version__ = "2.0rc1"
+__version__ = "2.0rc2"
 
 __logo__ = (
     r"""
     _         ____    _                         _       ___        __   ___ _____
  _-´ _-      / ___\  / \    /\  /\   /\  /\    / \     |     /\   /  ` |      |
 | ,-´ , |   | | __  / _ \  /  \/  \ /  \/  \  / _ \    |___ /  \ |     |__    |
 | | | | |   | |_] |/ ___ \/ /\  /\ \ /\  /\ \/ ___ \   |   /----\|     |      |
```

### Comparing `gamma-facet-2.0rc1/src/facet/data/_sample.py` & `gamma-facet-2.0rc2/src/facet/data/_sample.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/src/facet/data/partition/_partition.py` & `gamma-facet-2.0rc2/src/facet/data/partition/_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from abc import ABCMeta, abstractmethod
 from typing import Any, Generic, Optional, Sequence, Tuple, TypeVar, Union, cast
 
 import numpy as np
 import numpy.typing as npt
 
 from pytools.api import AllTracker, inheritdoc
-from pytools.fit import FittableMixin
+from pytools.fit import FittableMixin, fitted_only
 
 log = logging.getLogger(__name__)
 
 __all__ = [
     "Partitioner",
     "RangePartitioner",
     "ContinuousRangePartitioner",
@@ -95,30 +95,30 @@
     def max_partitions(self) -> int:
         """
         The maximum number of partitions to be generated by this partitioner.
         """
         return self._max_partitions
 
     @property
+    @fitted_only
     def partitions_(self) -> Sequence[T_Values]:
         """
         The values representing the partitions.
         """
 
-        self.ensure_fitted()
         assert self._partitions is not None, ASSERTION__PARTITIONER_IS_FITTED
         return self._partitions
 
     @property
+    @fitted_only
     def frequencies_(self) -> npt.NDArray[np.int_]:
         """
         The count of values allocated to each partition.
         """
 
-        self.ensure_fitted()
         assert self._frequencies is not None, ASSERTION__PARTITIONER_IS_FITTED
         return self._frequencies
 
     @property
     @abstractmethod
     def is_categorical(self) -> bool:
         """
@@ -173,34 +173,34 @@
     def is_categorical(self) -> bool:
         """
         ``False``
         """
         return False
 
     @property
+    @fitted_only
     def partition_bounds_(self) -> Sequence[Tuple[T_Values_Scalar, T_Values_Scalar]]:
         """
         Return the endpoints of the intervals that delineate each partition.
 
         :return: sequence of tuples (x, y) for every partition, where x is the
             inclusive lower bound of a partition range, and y is the exclusive upper
             bound of a partition range
         """
 
-        self.ensure_fitted()
         assert self._partition_bounds is not None, ASSERTION__PARTITIONER_IS_FITTED
         return self._partition_bounds
 
     @property
+    @fitted_only
     def partition_width_(self) -> T_Values_Scalar:
         """
         The width of each partition.
         """
 
-        self.ensure_fitted()
         assert self._step is not None, ASSERTION__PARTITIONER_IS_FITTED
         return self._step
 
     def fit(  # type: ignore[override]
         self: T_RangePartitioner,
         values: npt.NDArray[T_Values_Numeric],
         *,
```

### Comparing `gamma-facet-2.0rc1/src/facet/inspection/_explainer.py` & `gamma-facet-2.0rc2/src/facet/inspection/_explainer.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/src/facet/inspection/_inspection.py` & `gamma-facet-2.0rc2/src/facet/inspection/_inspection.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/src/facet/inspection/_learner_inspector.py` & `gamma-facet-2.0rc2/src/facet/inspection/_learner_inspector.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import pandas as pd
 from scipy.cluster import hierarchy
 from scipy.spatial import distance
 from sklearn.base import is_classifier
 
 from pytools.api import AllTracker, inheritdoc
 from pytools.data import LinkageTree, Matrix
-from pytools.fit import FittableMixin
+from pytools.fit import FittableMixin, fitted_only
 from pytools.parallelization import ParallelizableMixin
 from sklearndf import ClassifierDF, LearnerDF, RegressorDF
 from sklearndf.pipeline import LearnerPipelineDF
 
 from ..data import Sample
 from ._explainer import ExplainerFactory, TreeExplainerFactory
 from ._inspection import ShapPlotData
@@ -308,92 +308,93 @@
         self._shap_calculator = shap_calculator
         self._shap_global_projector = shap_global_projector
 
         return self
 
     @property
     def _shap_global_explainer(self) -> ShapGlobalExplainer:
-        self.ensure_fitted()
         assert self._shap_global_projector is not None, ASSERTION__INSPECTOR_IS_FITTED
         return self._shap_global_projector
 
     @property
     def is_fitted(self) -> bool:
         """[see superclass]"""
         return self._sample is not None
 
     @property
+    @fitted_only
     def sample_(self) -> Sample:
         """
         The background sample used to fit this inspector.
         """
 
-        self.ensure_fitted()
         assert self._sample is not None, ASSERTION__INSPECTOR_IS_FITTED
         return self._sample
 
     @property
+    @fitted_only
     def output_names_(self) -> Sequence[str]:
         """
         The names of the outputs explained by this inspector.
 
         For regressors, these are the names of the target columns.
 
         For binary classifiers, this is a list of length 1 with the name of a single
         class, since the SHAP values of the second class can be trivially derived as
         the negation of the SHAP values of the first class.
 
         For non-binary classifiers, this is the list of all classes.
         """
 
-        self.ensure_fitted()
         assert (
             self._shap_calculator is not None
             and self._shap_calculator.output_names_ is not None
         ), ASSERTION__INSPECTOR_IS_FITTED
         return self._shap_calculator.output_names_
 
     @property
+    @fitted_only
     def features_(self) -> List[str]:
         """
         The names of the features used to fit the learner pipeline explained by this
         inspector.
         """
         return cast(List[str], self.pipeline.feature_names_out_.to_list())
 
+    @fitted_only
     def shap_values(self) -> Union[pd.DataFrame, List[pd.DataFrame]]:
         """
         Calculate the SHAP values for all observations and features.
 
         Returns a data frame of SHAP values where each row corresponds to an
         observation, and each column corresponds to a feature.
 
         :return: a data frame with SHAP values
         """
 
-        self.ensure_fitted()
         assert self._shap_calculator is not None, ASSERTION__INSPECTOR_IS_FITTED
         return self.__split_multi_output_df(self._shap_calculator.get_shap_values())
 
+    @fitted_only
     def shap_interaction_values(self) -> Union[pd.DataFrame, List[pd.DataFrame]]:
         """
         Calculate the SHAP interaction values for all observations and pairs of
         features.
 
         Returns a data frame of SHAP interaction values where each row corresponds to an
         observation and a feature (identified by a hierarchical index with two levels),
         and each column corresponds to a feature.
 
         :return: a data frame with SHAP interaction values
         """
-        self.ensure_fitted()
         return self.__split_multi_output_df(
             self.__shap_interaction_values_calculator.get_shap_interaction_values()
         )
 
+    @fitted_only
     def feature_importance(
         self, *, method: str = "rms"
     ) -> Union[pd.Series, pd.DataFrame]:
         """
         Calculate the relative importance of each feature based on SHAP values.
 
         The importance values of all features always add up to `1.0`.
@@ -404,16 +405,14 @@
         :param method: method for calculating feature importance. Supported methods
             are ``rms`` (root of mean squares, default), ``mav`` (mean absolute
             values)
         :return: a series of length `n_features` for single-output models, or a
             data frame of shape (n_features, n_outputs) for multi-output models
         """
 
-        self.ensure_fitted()
-
         methods = {"rms", "mav"}
         if method not in methods:
             raise ValueError(f'arg method="{method}" must be one of {methods}')
 
         assert self._shap_calculator is not None
         shap_matrix: pd.DataFrame = self._shap_calculator.get_shap_values()
         weight: Optional[pd.Series] = self.sample_.weight
@@ -442,14 +441,15 @@
         else:
             assert (
                 abs_importance.index.nlevels == 2
             ), "2 index levels in place for multi-output models"
 
             return _normalize_importance(abs_importance.unstack(level=0))
 
+    @fitted_only
     def feature_synergy_matrix(
         self,
         *,
         absolute: bool = False,
         symmetrical: bool = False,
         clustered: bool = True,
     ) -> Union[FloatMatrix, List[FloatMatrix]]:
@@ -482,23 +482,22 @@
             such that synergy between adjacent rows and columns is maximised; if
             ``False``, keep rows and columns in the original features order
             (default: ``True``)
         :return: feature synergy matrix as a data frame of shape
             `(n_features, n_features)`, or a list of data frames for multiple outputs
         """
 
-        self.ensure_fitted()
-
         return self.__feature_affinity_matrix(
             explainer_fn=self.__interaction_explainer.synergy,
             absolute=absolute,
             symmetrical=symmetrical,
             clustered=clustered,
         )
 
+    @fitted_only
     def feature_redundancy_matrix(
         self,
         *,
         absolute: bool = False,
         symmetrical: bool = False,
         clustered: bool = True,
     ) -> Union[FloatMatrix, List[FloatMatrix]]:
@@ -530,23 +529,23 @@
         :param clustered: if ``True``, reorder the rows and columns of the matrix
             such that redundancy between adjacent rows and columns is maximised; if
             ``False``, keep rows and columns in the original features order
             (default: ``True``)
         :return: feature redundancy matrix as a data frame of shape
             `(n_features, n_features)`, or a list of data frames for multiple outputs
         """
-        self.ensure_fitted()
 
         return self.__feature_affinity_matrix(
             explainer_fn=self.__interaction_explainer.redundancy,
             absolute=absolute,
             symmetrical=symmetrical,
             clustered=clustered,
         )
 
+    @fitted_only
     def feature_association_matrix(
         self,
         *,
         absolute: bool = False,
         symmetrical: bool = False,
         clustered: bool = True,
     ) -> Union[FloatMatrix, List[FloatMatrix]]:
@@ -581,101 +580,100 @@
             such that association between adjacent rows and columns is maximised; if
             ``False``, keep rows and columns in the original features order
             (default: ``True``)
         :return: feature association matrix as a data frame of shape
             `(n_features, n_features)`, or a list of data frames for multiple outputs
         """
 
-        self.ensure_fitted()
-
         return self.__feature_affinity_matrix(
             explainer_fn=self._shap_global_explainer.association,
             absolute=absolute,
             symmetrical=symmetrical,
             clustered=clustered,
         )
 
+    @fitted_only
     def feature_synergy_linkage(self) -> Union[LinkageTree, List[LinkageTree]]:
         """
         Calculate a linkage tree based on the :meth:`.feature_synergy_matrix`.
 
         The linkage tree can be used to render a dendrogram indicating clusters of
         synergistic features.
 
         In the case of multi-target regression and non-binary classification, returns
         a list of linkage trees per target or class.
 
         :return: linkage tree of feature synergies; list of linkage trees
             for multi-target regressors or non-binary classifiers
         """
 
-        self.ensure_fitted()
         feature_affinity_matrix = self.__interaction_explainer.synergy(
             symmetrical=True, absolute=False
         )
         assert (
             feature_affinity_matrix is not None
         ), ASSERTION__SHAP_INTERACTION_SUPPORTED
 
         return self.__linkages_from_affinity_matrices(
             feature_affinity_matrix=feature_affinity_matrix
         )
 
+    @fitted_only
     def feature_redundancy_linkage(self) -> Union[LinkageTree, List[LinkageTree]]:
         """
         Calculate a linkage tree based on the :meth:`.feature_redundancy_matrix`.
 
         The linkage tree can be used to render a dendrogram indicating clusters of
         redundant features.
 
         In the case of multi-target regression and non-binary classification, returns
         a list of linkage trees per target or class.
 
         :return: linkage tree of feature redundancies; list of linkage trees
             for multi-target regressors or non-binary classifiers
         """
 
-        self.ensure_fitted()
         feature_affinity_matrix = self.__interaction_explainer.redundancy(
             symmetrical=True, absolute=False
         )
         assert (
             feature_affinity_matrix is not None
         ), ASSERTION__SHAP_INTERACTION_SUPPORTED
 
         return self.__linkages_from_affinity_matrices(
             feature_affinity_matrix=feature_affinity_matrix
         )
 
+    @fitted_only
     def feature_association_linkage(self) -> Union[LinkageTree, List[LinkageTree]]:
         """
         Calculate a linkage tree based on the :meth:`.feature_association_matrix`.
 
         The linkage tree can be used to render a dendrogram indicating clusters of
         associated features.
 
         In the case of multi-target regression and non-binary classification, returns
         a list of linkage trees per target or class.
 
         :return: linkage tree of feature associations; list of linkage trees
             for multi-target regressors or non-binary classifiers
         """
 
-        self.ensure_fitted()
         feature_affinity_matrix = self._shap_global_explainer.association(
             absolute=False, symmetrical=True
         )
         assert (
             feature_affinity_matrix is not None
         ), ASSERTION__SHAP_INTERACTION_SUPPORTED
 
         return self.__linkages_from_affinity_matrices(
             feature_affinity_matrix=feature_affinity_matrix
         )
 
+    @fitted_only
     def feature_interaction_matrix(self) -> Union[FloatMatrix, List[FloatMatrix]]:
         """
         Calculate relative shap interaction values for all feature pairings.
 
         Shap interactions quantify direct interactions between pairs of features.
         For a quantification of overall interaction (including indirect interactions
         across more than two features), see :meth:`.feature_synergy_matrix`.
@@ -773,14 +771,15 @@
         )[np.newaxis, :, :]
 
         # create a data frame from the feature matrix
         return self.__arrays_to_matrix(
             interaction_matrix, value_label="relative shap interaction"
         )
 
+    @fitted_only
     def shap_plot_data(self) -> ShapPlotData:
         """
         Consolidate SHAP values and corresponding feature values from this inspector
         for use in SHAP plots offered by the
         `shap <https://shap.readthedocs.io/en/stable/>`__ package.
 
         The `shap` package provides functions for creating various SHAP plots.
```

### Comparing `gamma-facet-2.0rc1/src/facet/inspection/_shap.py` & `gamma-facet-2.0rc2/src/facet/inspection/_shap.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Any, Generic, List, Optional, Sequence, TypeVar, Union, cast
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
 from pytools.api import AllTracker, inheritdoc
-from pytools.fit import FittableMixin
+from pytools.fit import FittableMixin, fitted_only
 from pytools.parallelization import ParallelizableMixin
 from sklearndf.pipeline import (
     ClassifierPipelineDF,
     LearnerPipelineDF,
     RegressorPipelineDF,
 )
 
@@ -129,17 +129,15 @@
         :param fit_params: additional fit parameters (unused)
         :return: self
         """
 
         # reset fit in case we get an exception along the way
         self.shap_ = None
 
-        self.feature_index_ = self.pipeline.feature_names_out_.rename(
-            Sample.IDX_FEATURE
-        )
+        self.feature_index_ = self.pipeline.final_estimator.feature_names_in_
         self.output_names_ = self._get_output_names(sample)
         self.sample_ = sample
 
         # calculate shap values and re-order the observation index to match the
         # sequence in the original training sample
         shap_df: pd.DataFrame = self._get_shap(sample)
 
@@ -332,17 +330,17 @@
 class ShapValuesCalculator(
     ShapCalculator[T_LearnerPipelineDF], Generic[T_LearnerPipelineDF], metaclass=ABCMeta
 ):
     """
     Base class for calculating SHAP contribution values.
     """
 
+    @fitted_only
     def get_shap_values(self) -> pd.DataFrame:
         """[see superclass]"""
-        self.ensure_fitted()
         return self.shap_
 
     def get_shap_interaction_values(self) -> pd.DataFrame:
         """
         Not implemented.
 
         :return: (never returns anything)
@@ -401,40 +399,40 @@
 class ShapInteractionValuesCalculator(
     ShapCalculator[T_LearnerPipelineDF], Generic[T_LearnerPipelineDF], metaclass=ABCMeta
 ):
     """
     Base class for calculating SHAP interaction values.
     """
 
+    @fitted_only
     def get_shap_values(self) -> pd.DataFrame:
         """[see superclass]"""
 
-        self.ensure_fitted()
         assert self.shap_ is not None, ASSERTION__CALCULATOR_IS_FITTED
         return self.shap_.groupby(level=0).sum()
 
+    @fitted_only
     def get_shap_interaction_values(self) -> pd.DataFrame:
         """[see superclass]"""
 
-        self.ensure_fitted()
         assert self.shap_ is not None, ASSERTION__CALCULATOR_IS_FITTED
         return self.shap_
 
+    @fitted_only
     def get_diagonals(self) -> pd.DataFrame:
         """
         The get_diagonals of all SHAP interaction matrices, of shape
         (n_observations, n_outputs * n_features).
 
         :return: SHAP interaction values with shape
             (n_observations * n_features, n_outputs * n_features), i.e., for each
             observation and output we get the feature interaction values of size
             n_features * n_features.
         """
 
-        self.ensure_fitted()
         assert (
             self.shap_ is not None
             and self.sample_ is not None
             and self.feature_index_ is not None
         ), ASSERTION__CALCULATOR_IS_FITTED
 
         n_observations = len(self.sample_)
```

### Comparing `gamma-facet-2.0rc1/src/facet/inspection/_shap_global_explanation.py` & `gamma-facet-2.0rc2/src/facet/inspection/_shap_global_explanation.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/src/facet/inspection/_shap_projection.py` & `gamma-facet-2.0rc2/src/facet/inspection/_shap_projection.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from abc import ABCMeta, abstractmethod
 from typing import Any, Optional, Tuple, TypeVar
 
 import numpy as np
 import numpy.typing as npt
 
 from pytools.api import AllTracker, inheritdoc
+from pytools.fit import fitted_only
 
 from ._shap import ShapCalculator
 from ._shap_global_explanation import (
     AffinityMatrix,
     ShapContext,
     ShapGlobalExplainer,
     ShapInteractionGlobalExplainer,
@@ -62,18 +63,18 @@
     Base class for global pairwise model explanations based on SHAP vector projection.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.association_: Optional[AffinityMatrix] = None
 
+    @fitted_only
     def association(self, absolute: bool, symmetrical: bool) -> npt.NDArray[np.float_]:
         """[see superclass]"""
 
-        self.ensure_fitted()
         assert self.association_ is not None
         return self.association_.get_values(symmetrical=symmetrical, absolute=absolute)
 
     def _fit(self, shap_calculator: ShapCalculator[Any]) -> None:
         self._reset_fit()
         self._calculate(self._get_context(shap_calculator=shap_calculator))
 
@@ -151,25 +152,25 @@
 
     def __init__(self) -> None:
         super().__init__()
 
         self.synergy_: Optional[AffinityMatrix] = None
         self.redundancy_: Optional[AffinityMatrix] = None
 
+    @fitted_only
     def synergy(self, symmetrical: bool, absolute: bool) -> npt.NDArray[np.float_]:
         """[see superclass]"""
 
-        self.ensure_fitted()
         assert self.synergy_ is not None, "Projector is fitted"
         return self.synergy_.get_values(symmetrical=symmetrical, absolute=absolute)
 
+    @fitted_only
     def redundancy(self, symmetrical: bool, absolute: bool) -> npt.NDArray[np.float_]:
         """[see superclass]"""
 
-        self.ensure_fitted()
         assert self.redundancy_ is not None, "Projector is fitted"
         return self.redundancy_.get_values(symmetrical=symmetrical, absolute=absolute)
 
     def _get_context(self, shap_calculator: ShapCalculator[Any]) -> ShapContext:
         return ShapInteractionValueContext(shap_calculator=shap_calculator)
 
     def _calculate(self, context: ShapContext) -> None:
```

### Comparing `gamma-facet-2.0rc1/src/facet/selection/_parameters.py` & `gamma-facet-2.0rc2/src/facet/selection/_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,18 @@
 ParameterDict = Dict[str, ParameterSet]
 
 try:
     rv_frozen = next(
         t for t in type(stats.uniform()).mro() if t.__name__ == "rv_frozen"
     )
 except StopIteration:
-    raise AssertionError("stats.uniform() is based on class rv_frozen")
+    warnings.warn(
+        "stats.uniform() should be based on class rv_frozen", category=UserWarning
+    )
+    rv_frozen = type(None)
 
 
 #
 # Type variables
 #
 
 T_Estimator_co = TypeVar("T_Estimator_co", covariant=True, bound=EstimatorDF)
```

### Comparing `gamma-facet-2.0rc1/src/facet/selection/_selection.py` & `gamma-facet-2.0rc2/src/facet/selection/_selection.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import numpy.typing as npt
 import pandas as pd
 from sklearn.base import BaseEstimator
 from sklearn.metrics import get_scorer
 from sklearn.model_selection import BaseCrossValidator, GridSearchCV
 
 from pytools.api import AllTracker, inheritdoc, to_list
-from pytools.fit import FittableMixin
+from pytools.fit import FittableMixin, fitted_only
 from pytools.parallelization import ParallelizableMixin
 from sklearndf import EstimatorDF
 from sklearndf.pipeline import LearnerPipelineDF
 
 from facet.data import Sample
 from facet.selection import MultiEstimatorParameterSpace, ParameterSpace
 from facet.selection.base import BaseParameterSpace, CandidateEstimatorDF
@@ -275,19 +275,19 @@
 
     @property
     def is_fitted(self) -> bool:
         """[see superclass]"""
         return self.searcher_ is not None
 
     @property
+    @fitted_only
     def best_estimator_(self) -> T_EstimatorDF:
         """
         The model which obtained the best ranking score, fitted on the entire sample.
         """
-        self.ensure_fitted()
         searcher = self.searcher_
         assert searcher is not None, "Ranker is fitted"
 
         if searcher.refit:
             best_estimator = searcher.best_estimator_
             while isinstance(best_estimator, CandidateEstimatorDF):
                 # unpack the candidate estimator
@@ -346,27 +346,26 @@
         if sample.weight is not None:
             fit_params = {ARG_SAMPLE_WEIGHT: sample.weight, **fit_params}
 
         searcher.fit(X=sample.features, y=sample.target, groups=groups, **fit_params)
 
         return self
 
+    @fitted_only
     def summary_report(self, *, sort_by: Optional[str] = None) -> pd.DataFrame:
         """
         Create a summary table of the scores achieved by all learners in the grid
         search, sorted by ranking score in descending order.
 
         :param sort_by: name of the column to sort the report by, in ascending order,
             if the column is present (default: ``"%%SORT_COLUMN%%"``)
 
         :return: the summary report of the grid search as a data frame
         """
 
-        self.ensure_fitted()
-
         if sort_by is None:
             sort_by = self._DEFAULT_REPORT_SORT_COLUMN
 
         assert self.searcher_ is not None, "Ranker is fitted"
 
         # get the raw CV results
         cv_results: Dict[str, Any] = self.searcher_.cv_results_
```

### Comparing `gamma-facet-2.0rc1/src/facet/selection/base/_parameters.py` & `gamma-facet-2.0rc2/src/facet/selection/base/_parameters.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 #
 # Type variables
 #
 
 T_CandidateEstimatorDF = TypeVar("T_CandidateEstimatorDF", bound="CandidateEstimatorDF")
-T_Estimator = TypeVar("T_Estimator", bound=EstimatorDF)
+T_Estimator = TypeVar("T_Estimator", covariant=True, bound=EstimatorDF)
 
 
 #
 # Ensure all symbols introduced below are included in __all__
 #
 
 __tracker = AllTracker(globals())
@@ -146,17 +146,15 @@
         # get the estimator candidate; raise an attribute error if it has not been set
 
         if self.candidate is None:
             raise AttributeError("no candidate has been assigned")
         else:
             return self.candidate
 
-    @property
-    def classes_(self) -> Union[npt.NDArray[Any], List[npt.NDArray[Any]]]:
-        """[see superclass]"""
+    def _get_classes(self) -> Union[npt.NDArray[Any], List[npt.NDArray[Any]]]:
         return self._get_candidate().classes_
 
     # noinspection PyPep8Naming
     def predict_proba(
         self, X: pd.DataFrame, **predict_params: Any
     ) -> Union[pd.DataFrame, List[pd.DataFrame]]:
         """[see superclass]"""
@@ -220,14 +218,17 @@
     def _estimator_type(self) -> str:
         # noinspection PyProtectedMember
         return self.candidate._estimator_type  # type: ignore
 
     def _get_features_in(self) -> pd.Index:
         return self._get_candidate().feature_names_in_
 
+    def _get_outputs(self) -> Optional[List[str]]:
+        return self._get_candidate()._get_outputs()
+
     def _get_n_outputs(self) -> int:
         return self._get_candidate().n_outputs_
 
     def _get_features_original(self) -> pd.Series:
         return self._get_candidate().feature_names_original_
```

### Comparing `gamma-facet-2.0rc1/src/facet/simulation/_result.py` & `gamma-facet-2.0rc2/src/facet/simulation/_result.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/src/facet/simulation/_simulation.py` & `gamma-facet-2.0rc2/src/facet/simulation/_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,20 +252,24 @@
         The baseline of uplift simulations is always ``0.0``
 
         :return: 0.0
         """
         return 0.0
 
     def simulate_feature(
-        self, feature_name: str, *, partitioner: Partitioner[T_Values]
+        self,
+        feature_name: str,
+        *,
+        partitioner: Partitioner[T_Values],
+        **partitioner_params: Any,
     ) -> UnivariateSimulationResult[T_Values]:
         """[see superclass]"""
 
         result = super().simulate_feature(
-            feature_name=feature_name, partitioner=partitioner
+            feature_name=feature_name, partitioner=partitioner, **partitioner_params
         )
 
         # offset the mean values to get uplift instead of absolute outputs
         result.data.loc[
             :,
             [
                 UnivariateSimulationResult.COL_MEAN,
```

### Comparing `gamma-facet-2.0rc1/src/facet/simulation/base/_base.py` & `gamma-facet-2.0rc2/src/facet/simulation/base/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,31 +129,39 @@
 
     # add parallelization parameters to __init__ docstring
     __init__.__doc__ = cast(str, __init__.__doc__) + cast(
         str, ParallelizableMixin.__init__.__doc__
     )
 
     def simulate_feature(
-        self, feature_name: str, *, partitioner: Partitioner[T_Value]
+        self,
+        feature_name: str,
+        *,
+        partitioner: Partitioner[T_Value],
+        **partitioner_params: Any,
     ) -> UnivariateSimulationResult[T_Value]:
         """
         Simulate the average target uplift when fixing the value of the given feature
         across all observations.
 
+        Simulations are run for a set of values determined by the given partitioner,
+        which is fitted to the observed values for the feature being simulated.
+
         :param feature_name: the feature to run the simulation for
         :param partitioner: the partitioner of feature values to run simulations for
+        :param partitioner_params: additional parameters to pass to the partitioner
         :return: a mapping of output names to simulation results
         """
 
         sample = self.sample
 
         mean, sem = self._simulate_feature_with_values(
             feature_name=feature_name,
             simulation_values=partitioner.fit(
-                sample.features.loc[:, feature_name]
+                sample.features.loc[:, feature_name], **partitioner_params
             ).partitions_,
         )
         return UnivariateSimulationResult(
             partitioner=partitioner,
             mean=mean,
             sem=sem,
             feature_name=feature_name,
```

### Comparing `gamma-facet-2.0rc1/src/facet/simulation/viz/_draw.py` & `gamma-facet-2.0rc2/src/facet/simulation/viz/_draw.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/src/facet/simulation/viz/_style.py` & `gamma-facet-2.0rc2/src/facet/simulation/viz/_style.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/src/facet/validation/_validation.py` & `gamma-facet-2.0rc2/src/facet/validation/_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Core implementation of :mod:`facet.validation`.
 """
 import warnings
 from abc import ABCMeta, abstractmethod
-from typing import Any, Generator, Iterator, Optional, Tuple, Union, cast
+from typing import Any, Generator, Optional, Tuple, Union, cast
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 from sklearn.model_selection import BaseCrossValidator
 from sklearn.utils import check_random_state
 
@@ -133,15 +133,15 @@
         :return: an array of integer indices with shape ``[n_samples]``
         """
         pass
 
     # noinspection PyPep8Naming
     def _iter_test_indices(
         self, X: Any = None, y: Any = None, groups: Any = None
-    ) -> Iterator[Any]:
+    ) -> None:
         # adding this stub just so all abstract methods are implemented
         pass
 
 
 class BootstrapCV(BaseBootstrapCV):
     """
     Bootstrapping cross-validation.
```

### Comparing `gamma-facet-2.0rc1/test/test/conftest.py` & `gamma-facet-2.0rc2/test/test/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 import pytest
 from numpy.testing import assert_allclose, assert_array_equal
 from sklearn import datasets
+from sklearn.datasets import fetch_california_housing
 from sklearn.model_selection import BaseCrossValidator, GridSearchCV, KFold
 from sklearn.utils import Bunch
 
 from sklearndf import TransformerDF
 from sklearndf.classification import RandomForestClassifierDF
 from sklearndf.pipeline import ClassifierPipelineDF, RegressorPipelineDF
 from sklearndf.regression import (
@@ -54,16 +55,16 @@
 N_BOOTSTRAPS = 30
 
 STEP_IMPUTE = "impute"
 STEP_ONE_HOT_ENCODE = "one-hot-encode"
 
 
 @pytest.fixture  # type: ignore
-def boston_target() -> str:
-    return "price"
+def california_target() -> str:
+    return "MedHouseVal"
 
 
 @pytest.fixture  # type: ignore
 def iris_target_name() -> str:
     return "species"
 
 
@@ -209,15 +210,15 @@
 @pytest.fixture  # type: ignore
 def preprocessed_feature_names(
     best_lgbm_model: RegressorPipelineDF[LGBMRegressorDF],
 ) -> Set[str]:
     """
     Names of all features after preprocessing
     """
-    return set(best_lgbm_model.feature_names_out_)
+    return set(best_lgbm_model.final_estimator.feature_names_in_)
 
 
 @pytest.fixture  # type: ignore
 def regressor_inspector(
     best_lgbm_model: RegressorPipelineDF[LGBMRegressorDF], sample: Sample, n_jobs: int
 ) -> LearnerInspector[RegressorPipelineDF[LGBMRegressorDF]]:
     inspector = LearnerInspector(
@@ -257,27 +258,30 @@
             )
         )
 
     return ColumnTransformerDF(transformers=column_transforms)
 
 
 @pytest.fixture  # type: ignore
-def boston_df(boston_target: str) -> pd.DataFrame:
+def california_df(california_target: str) -> pd.DataFrame:
     #  load sklearn test-data and convert to pd
-    boston: Bunch = datasets.load_boston()
+    california: Bunch = fetch_california_housing()
 
     return pd.DataFrame(
-        data=np.c_[boston.data, boston.target],
-        columns=[*boston.feature_names, boston_target],
+        data=np.c_[california.data, california.target],
+        columns=[*california.feature_names, california_target],
     )
 
 
 @pytest.fixture  # type: ignore
-def sample(boston_df: pd.DataFrame, boston_target: str) -> Sample:
-    return Sample(observations=boston_df.iloc[:100, :], target_name=boston_target)
+def sample(california_df: pd.DataFrame, california_target: str) -> Sample:
+    return Sample(
+        observations=california_df.sample(n=100, random_state=42),
+        target_name=california_target,
+    )
 
 
 @pytest.fixture  # type: ignore
 def iris_df(iris_target_name: str) -> pd.DataFrame:
     #  load sklearn test-data and convert to pd
     iris: Bunch = datasets.load_iris()
 
@@ -360,15 +364,15 @@
     """
 
     scores_actual: pd.Series = ranking.loc[:, COL_SCORE].values[: len(scores_expected)]
 
     assert_allclose(
         scores_actual,
         scores_expected,
-        rtol=0.01,
+        rtol=0.015,
         err_msg=(
             f"unexpected scores: got {scores_actual} but expected {scores_expected}"
         ),
     )
 
     col_learner = COL_CLASSIFIER if is_classifier else COL_REGRESSOR
```

### Comparing `gamma-facet-2.0rc1/test/test/facet/test_inspection.py` & `gamma-facet-2.0rc2/test/test/facet/test_inspection.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         RegressorPipelineDF[LGBMRegressorDF], GridSearchCV
     ]
 ) -> None:
     check_ranking(
         ranking=regressor_selector.summary_report(),
         is_classifier=False,
         scores_expected=(
-            [0.820, 0.818, 0.808, 0.806, 0.797, 0.768, 0.652, 0.651, 0.651, 0.651]
+            [0.578, 0.530, 0.310, 0.308, 0.294, 0.226, 0.217, 0.217, 0.217, 0.217]
         ),
         params_expected=None,
     )
 
 
 def test_model_inspection(
     best_lgbm_model: RegressorPipelineDF[LGBMRegressorDF],
```

### Comparing `gamma-facet-2.0rc1/test/test/facet/test_partition.py` & `gamma-facet-2.0rc2/test/test/facet/test_partition.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/test/test/facet/test_sample.py` & `gamma-facet-2.0rc2/test/test/facet/test_sample.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,112 +5,114 @@
 import pytest
 from joblib import Parallel, delayed
 from pandas.testing import assert_frame_equal
 
 from facet.data import Sample
 
 
-def test_sample_init(boston_df: pd.DataFrame, boston_target: str) -> None:
+def test_sample_init(california_df: pd.DataFrame, california_target: str) -> None:
     # check handling of various invalid inputs
 
     # 1. sample parameter
     # 1.1 None
     with pytest.raises(ValueError):
         # noinspection PyTypeChecker
-        Sample(observations=None, target_name=boston_target)
+        Sample(observations=None, target_name=california_target)
 
     # 1.2 not a DF
     with pytest.raises(ValueError):
         # noinspection PyTypeChecker
-        Sample(observations=[], target_name=boston_target)
+        Sample(observations=[], target_name=california_target)
 
     # 2. no valid target specified
     with pytest.raises(TypeError):
         # noinspection PyTypeChecker
-        Sample(observations=boston_df, target_name=None)  # type: ignore
+        Sample(observations=california_df, target_name=None)  # type: ignore
 
     # store list of feature columns:
-    f_columns = list(boston_df.columns)
-    f_columns.remove(boston_target)
+    f_columns = list(california_df.columns)
+    f_columns.remove(california_target)
 
     # 2.1 invalid feature column specified
     with pytest.raises(KeyError):
         f_columns_invalid = f_columns.copy()
         f_columns_invalid.append("doesnt_exist")
         Sample(
-            observations=boston_df,
+            observations=california_df,
             feature_names=f_columns_invalid,
-            target_name=boston_target,
+            target_name=california_target,
         )
 
     # 2.2 invalid target column specified
     with pytest.raises(KeyError):
         Sample(
-            observations=boston_df,
+            observations=california_df,
             feature_names=f_columns,
             target_name="doesnt_exist",
         )
 
     # 3. column is target and also feature
     with pytest.raises(KeyError):
         f_columns_invalid = f_columns.copy()
-        f_columns_invalid.append(boston_target)
+        f_columns_invalid.append(california_target)
         Sample(
-            observations=boston_df,
+            observations=california_df,
             feature_names=f_columns_invalid,
-            target_name=boston_target,
+            target_name=california_target,
         )
 
     # 4. weight column is not defined
     with pytest.raises(KeyError):
         Sample(
-            observations=boston_df,
-            target_name=boston_target,
+            observations=california_df,
+            target_name=california_target,
             weight_name="doesnt_exist",
         )
 
 
-def test_sample(boston_df: pd.DataFrame, boston_target: str) -> None:
+def test_sample(california_df: pd.DataFrame, california_target: str) -> None:
     # define various assertions we want to test:
     def run_assertions(sample: Sample) -> None:
-        assert sample.target.name == boston_target
+        assert sample.target.name == california_target
         assert sample.weight is not None
-        assert sample.weight.name == boston_target
-        assert boston_target not in sample.feature_names
-        assert len(sample.feature_names) == len(boston_df.columns) - 1
+        assert sample.weight.name == california_target
+        assert california_target not in sample.feature_names
+        assert len(sample.feature_names) == len(california_df.columns) - 1
 
         assert type(sample.target) == pd.Series
         assert type(sample.weight) == pd.Series
         assert type(sample.features) == pd.DataFrame
 
         assert len(sample.target) == len(sample.features)
 
     # test explicit setting of all fields
-    feature_columns = list(boston_df.drop(columns=boston_target).columns)
+    feature_columns = list(california_df.drop(columns=california_target).columns)
     s = Sample(
-        observations=boston_df,
-        target_name=boston_target,
+        observations=california_df,
+        target_name=california_target,
         feature_names=feature_columns,
-        weight_name=boston_target,
+        weight_name=california_target,
     )
 
     # _rank_learners the checks on s:
     run_assertions(s)
 
     # test implicit setting of features by only giving the target
     s2 = Sample(
-        observations=boston_df, target_name=boston_target, weight_name=boston_target
+        observations=california_df,
+        target_name=california_target,
+        weight_name=california_target,
     )
 
     # _rank_learners the checks on s2:
     run_assertions(s2)
 
     # test numerical features
     features_numerical = s.features.select_dtypes(np.number).columns
-    assert "LSTAT" in features_numerical
+    assert "HouseAge" in features_numerical
 
     # test categorical features
     features_non_numerical = s.features.select_dtypes(object).columns
     assert len(features_non_numerical) == 0
 
     # assert feature completeness
     assert (
@@ -119,15 +121,15 @@
             .union(set(features_non_numerical))
             .difference(s.feature_names)
         )
         == 0
     )
 
     # test length
-    assert len(s) == len(boston_df)
+    assert len(s) == len(california_df)
 
     # test select_observations
     sub = s2.subsample(iloc=[0, 1, 2, 3])
     assert len(sub) == 4
 
     # test subset of features
     assert_frame_equal(
@@ -152,10 +154,10 @@
         TypeError,
         match=(
             "^all column names in arg observations must be strings, "
             "but included: int$"
         ),
     ):
         Sample(
-            boston_df.set_axis([*boston_df.columns[1:], 1], axis=1),
-            target_name=boston_target,
+            california_df.set_axis([*california_df.columns[1:], 1], axis=1),
+            target_name=california_target,
         )
```

### Comparing `gamma-facet-2.0rc1/test/test/facet/test_selection.py` & `gamma-facet-2.0rc2/test/test/facet/test_selection.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,45 +38,45 @@
 def test_learner_selector(
     regressor_parameters: List[ParameterSpace[RegressorPipelineDF[LGBMRegressorDF]]],
     sample: Sample,
     n_jobs: int,
 ) -> None:
 
     expected_scores = [
-        0.840,
-        0.837,
-        0.812,
-        0.793,
-        0.790,
-        0.777,
-        0.758,
-        0.758,
-        0.758,
-        0.758,
+        0.669,
+        0.649,
+        0.493,
+        0.477,
+        0.464,
+        0.451,
+        0.448,
+        0.448,
+        0.448,
+        0.448,
     ]
     expected_learners: List[str] = [
         cls.__name__
         for cls in (
+            LinearRegressionDF,
+            LinearRegressionDF,
             RandomForestRegressorDF,
             RandomForestRegressorDF,
-            LinearRegressionDF,
             AdaBoostRegressorDF,
             AdaBoostRegressorDF,
-            LinearRegressionDF,
             LGBMRegressorDF,
             LGBMRegressorDF,
             LGBMRegressorDF,
             LGBMRegressorDF,
         )
     ]
     expected_parameters = {
-        0: dict(n_estimators=80),
-        1: dict(n_estimators=50),
-        3: dict(n_estimators=50),
-        4: dict(n_estimators=80),
+        0: dict(fit_intercept=True),
+        1: dict(fit_intercept=False),
+        3: dict(n_estimators=80),
+        4: dict(n_estimators=50),
     }
 
     # define the circular cross validator with just 5 splits (to speed up testing)
     cv = BootstrapCV(n_splits=5, random_state=42)
 
     with pytest.raises(
         TypeError,
@@ -275,16 +275,24 @@
     def regressor_repr(model: Id) -> Expression:
         return Id.RegressorPipelineDF(
             preprocessing=Id.ColumnTransformerDF(
                 transformers=[
                     (
                         "impute",
                         Id.SimpleImputerDF(strategy="median"),
-                        ["CRIM", "ZN", "INDUS", "CHAS", "NOX", "RM", "AGE"]
-                        + ["DIS", "RAD", "TAX", "PTRATIO", "B", "LSTAT"],
+                        [
+                            "MedInc",
+                            "HouseAge",
+                            "AveRooms",
+                            "AveBedrms",
+                            "Population",
+                            "AveOccup",
+                            "Latitude",
+                            "Longitude",
+                        ],
                     )
                 ]
             ),
             regressor=model(random_state=42),
         )
 
     assert freeze(mps.to_expression()) == freeze(
```

### Comparing `gamma-facet-2.0rc1/test/test/facet/test_shap_decomposition.py` & `gamma-facet-2.0rc2/test/test/facet/test_shap_decomposition.py`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/test/test/facet/test_simulation.py` & `gamma-facet-2.0rc2/test/test/facet/test_simulation.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,140 +69,144 @@
     )
 
 
 def test_univariate_target_simulation(
     target_simulator: UnivariateTargetSimulator,
 ) -> None:
 
-    parameterized_feature = "LSTAT"
+    parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     simulation_result: UnivariateSimulationResult[
         np.float_
     ] = target_simulator.simulate_feature(
         feature_name=parameterized_feature,
         partitioner=partitioner,
     )
 
     # test simulation results
 
     index = pd.Index(
-        data=[0.0, 5.0, 10.0, 15.0, 20.0, 25.0],
+        data=[0.0, 10.0, 20.0, 30.0, 40.0, 50.0],
         name=UnivariateSimulationResult.IDX_PARTITION,
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_LOWER_BOUND],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_LOWER_BOUND].round(
+            4
+        ),
         pd.Series(
-            [24.98646, 24.98646, 21.15398, 20.23877, 20.23877, 20.23877],
+            [1.4621, 1.4621, 1.6542, 1.9865, 2.2322, 2.2322],
             name=UnivariateSimulationResult.COL_LOWER_BOUND,
             index=index,
         ),
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_MEAN],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_MEAN].round(4),
         pd.Series(
-            [25.4571, 25.4571, 21.67744, 20.81063, 20.81063, 20.81063],
+            [1.5430, 1.5430, 1.7444, 2.0929, 2.3398, 2.3398],
             name=UnivariateSimulationResult.COL_MEAN,
             index=index,
         ),
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_UPPER_BOUND],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_UPPER_BOUND].round(
+            5
+        ),
         pd.Series(
-            [25.92774, 25.92774, 22.2009, 21.38249, 21.38249, 21.38249],
+            [1.62397, 1.62397, 1.8346, 2.19933, 2.44734, 2.44734],
             name=UnivariateSimulationResult.COL_UPPER_BOUND,
             index=index,
         ),
     )
 
     assert_array_equal(
-        simulation_result.partitioner.frequencies_, [1, 31, 37, 19, 8, 1]
+        simulation_result.partitioner.frequencies_, [1, 9, 23, 32, 23, 12]
     )
 
     SimulationDrawer(style="text").draw(
         data=target_simulator.simulate_feature(
             feature_name=parameterized_feature, partitioner=partitioner
         )
     )
 
 
 def test_univariate_target_subsample_simulation_80(
     model: RegressorPipelineDF[LGBMRegressorDF], subsample: Sample, n_jobs: int
 ) -> None:
 
-    parameterized_feature = "LSTAT"
+    parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     target_simulator = UnivariateTargetSimulator(
         model=model, sample=subsample, confidence_level=0.8, n_jobs=n_jobs, verbose=50
     )
 
     simulation_result: UnivariateSimulationResult[
         np.float_
     ] = target_simulator.simulate_feature(
         feature_name=parameterized_feature,
         partitioner=partitioner,
+        lower_bound=3.8,
     )
 
     # test simulation results
 
     index = pd.Index(
-        data=[2.0, 4.0, 6.0, 8.0, 10.0, 12.0, 14.0, 16.0, 18.0],
+        data=[0.0, 10.0, 20.0, 30.0, 40.0, 50.0],
         name=UnivariateSimulationResult.IDX_PARTITION,
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_LOWER_BOUND],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_LOWER_BOUND].round(
+            5
+        ),
         pd.Series(
-            [25.05676, 25.05676, 25.05676, 22.96243, 21.43395]
-            + [21.21544, 20.76824, 20.49282, 20.49282],
+            [1.63804, 1.63804, 1.86338, 2.23901, 2.44907, 2.44907],
             name=UnivariateSimulationResult.COL_LOWER_BOUND,
             index=index,
         ),
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_MEAN],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_MEAN].round(5),
         pd.Series(
-            [25.642227, 25.642227, 25.642227, 23.598706, 22.067057]
-            + [21.864828, 21.451056, 21.195954, 21.195954],
+            [1.74114, 1.74114, 1.97514, 2.36965, 2.58642, 2.58642],
             name=UnivariateSimulationResult.COL_MEAN,
             index=index,
         ),
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_UPPER_BOUND],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_UPPER_BOUND].round(
+            5
+        ),
         pd.Series(
-            [26.22769, 26.22769, 26.22769, 24.23498, 22.70016]
-            + [22.51422, 22.13387, 21.89909, 21.89909],
+            [1.84423, 1.84423, 2.08689, 2.50029, 2.72377, 2.72377],
             name=UnivariateSimulationResult.COL_UPPER_BOUND,
             index=index,
         ),
     )
 
-    assert_array_equal(
-        simulation_result.partitioner.frequencies_, [1, 4, 9, 10, 10, 6, 2, 1, 4]
-    )
+    assert_array_equal(simulation_result.partitioner.frequencies_, [2, 5, 18, 8, 11, 6])
 
     SimulationDrawer(style="text").draw(
         data=target_simulator.simulate_feature(
             feature_name=parameterized_feature, partitioner=partitioner
         )
     )
 
 
 def test_univariate_uplift_subsample_simulation_95(
     model: RegressorPipelineDF[LGBMRegressorDF], subsample: Sample, n_jobs: int
 ) -> None:
 
-    parameterized_feature = "LSTAT"
+    parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     target_simulator = UnivariateUpliftSimulator(
         model=model, sample=subsample, confidence_level=0.95, n_jobs=n_jobs, verbose=50
     )
 
     simulation_result: UnivariateSimulationResult[
@@ -211,127 +215,126 @@
         feature_name=parameterized_feature,
         partitioner=partitioner,
     )
 
     # test simulation results
 
     index = pd.Index(
-        data=[2.0, 4.0, 6.0, 8.0, 10.0, 12.0, 14.0, 16.0, 18.0],
+        data=[0.0, 10.0, 20.0, 30.0, 40.0, 50.0],
         name=UnivariateSimulationResult.IDX_PARTITION,
     )
 
     assert_series_equal(
         simulation_result.data.loc[:, UnivariateSimulationResult.COL_LOWER_BOUND].round(
             6
         ),
         pd.Series(
-            [1.800835, 1.800835, 1.800835, -0.320393, -1.847194]
-            + [-2.074327, -2.539217, -2.825394, -2.825394],
+            [-0.47617, -0.47617, -0.255413, 0.110223, 0.316729, 0.316729],
             name=UnivariateSimulationResult.COL_LOWER_BOUND,
             index=index,
         ),
     )
 
     assert_series_equal(
         simulation_result.data.loc[:, UnivariateSimulationResult.COL_MEAN].round(6),
         pd.Series(
-            [2.696227, 2.696227, 2.696227, 0.652706, -0.878943]
-            + [-1.081172, -1.494944, -1.750046, -1.750046],
+            [-0.318501, -0.318501, -0.084503, 0.310012, 0.526783, 0.526783],
             name=UnivariateSimulationResult.COL_MEAN,
             index=index,
         ),
     )
 
     assert_series_equal(
         simulation_result.data.loc[:, UnivariateSimulationResult.COL_UPPER_BOUND].round(
             6
         ),
         pd.Series(
-            [3.59162, 3.59162, 3.59162, 1.625805, 0.089307]
-            + [-0.088017, -0.450671, -0.674698, -0.674698],
+            [-0.160831, -0.160831, 0.086407, 0.509801, 0.736836, 0.736836],
             name=UnivariateSimulationResult.COL_UPPER_BOUND,
             index=index,
         ),
     )
 
-    assert_array_equal(
-        simulation_result.partitioner.frequencies_, [1, 4, 9, 10, 10, 6, 2, 1, 4]
-    )
+    assert_array_equal(simulation_result.partitioner.frequencies_, [2, 5, 18, 8, 11, 6])
 
     SimulationDrawer(style="text").draw(
         data=target_simulator.simulate_feature(
             feature_name=parameterized_feature, partitioner=partitioner
         )
     )
 
 
 def test_univariate_uplift_simulation(
     uplift_simulator: UnivariateUpliftSimulator,
 ) -> None:
 
-    parameterized_feature = "LSTAT"
+    parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     simulation_result: UnivariateSimulationResult[
         np.float_
     ] = uplift_simulator.simulate_feature(
         feature_name=parameterized_feature,
         partitioner=partitioner,
     )
 
     # test simulation results
 
     index = pd.Index(
-        data=[0.0, 5.0, 10.0, 15.0, 20.0, 25.0],
+        data=[0.0, 10.0, 20.0, 30.0, 40.0, 50.0],
         name=UnivariateSimulationResult.IDX_PARTITION,
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_LOWER_BOUND],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_LOWER_BOUND].round(
+            5
+        ),
         pd.Series(
-            [2.677461, 2.677461, -1.155017, -2.070234, -2.070234, -2.070234],
+            [-0.48552, -0.48552, -0.2934, 0.03889, 0.28455, 0.28455],
             name=UnivariateSimulationResult.COL_LOWER_BOUND,
             index=index,
         ),
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_MEAN],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_MEAN].round(5),
         pd.Series(
-            [3.148100, 3.148100, -0.631560, -1.498371, -1.498371, -1.498371],
+            [-0.40459, -0.40459, -0.20322, 0.14529, 0.39212, 0.39212],
             name=UnivariateSimulationResult.COL_MEAN,
             index=index,
         ),
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_UPPER_BOUND],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_UPPER_BOUND].round(
+            5
+        ),
         pd.Series(
-            [3.618739, 3.618739, -0.108103, -0.926508, -0.926508, -0.926508],
+            [-0.32367, -0.32367, -0.11304, 0.25169, 0.4997, 0.4997],
             name=UnivariateSimulationResult.COL_UPPER_BOUND,
             index=index,
         ),
     )
 
     assert_array_equal(
-        simulation_result.partitioner.frequencies_, [1, 31, 37, 19, 8, 1]
+        simulation_result.partitioner.frequencies_, [1, 9, 23, 32, 23, 12]
     )
 
     SimulationDrawer(style="text").draw(
         data=uplift_simulator.simulate_feature(
             feature_name=parameterized_feature, partitioner=partitioner
         )
     )
 
 
 def test_univariate_uplift_subsample_simulation(
     model: RegressorPipelineDF[LGBMRegressorDF], subsample: Sample, n_jobs: int
 ) -> None:
 
-    parameterized_feature = "LSTAT"
+    parameterized_feature = "HouseAge"
     partitioner = ContinuousRangePartitioner(max_partitions=10)
 
     uplift_simulator = UnivariateUpliftSimulator(
         model=model, sample=subsample, confidence_level=0.8, n_jobs=n_jobs, verbose=50
     )
 
     simulation_result: UnivariateSimulationResult[
@@ -339,51 +342,50 @@
     ] = uplift_simulator.simulate_feature(
         feature_name=parameterized_feature, partitioner=partitioner
     )
 
     # test simulation results
 
     index = pd.Index(
-        data=[2.0, 4.0, 6.0, 8.0, 10.0, 12.0, 14.0, 16.0, 18.0],
+        data=[0.0, 10.0, 20.0, 30.0, 40.0, 50.0],
         name=UnivariateSimulationResult.IDX_PARTITION,
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_LOWER_BOUND],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_LOWER_BOUND].round(
+            5
+        ),
         pd.Series(
-            [2.110762, 2.110762, 2.110762, 0.0164306, -1.512048]
-            + [-1.730561, -2.177757, -2.453179, -2.453179],
+            [-0.4216, -0.4216, -0.19626, 0.17938, 0.38944, 0.38944],
             name=UnivariateSimulationResult.COL_LOWER_BOUND,
             index=index,
         ),
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_MEAN],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_MEAN].round(5),
         pd.Series(
-            [2.696227, 2.696227, 2.696227, 0.652706, -0.878943]
-            + [-1.081172, -1.494944, -1.750046, -1.750046],
+            [-0.3185, -0.3185, -0.0845, 0.31001, 0.52678, 0.52678],
             name=UnivariateSimulationResult.COL_MEAN,
             index=index,
         ),
     )
 
     assert_series_equal(
-        simulation_result.data.loc[:, UnivariateSimulationResult.COL_UPPER_BOUND],
+        simulation_result.data.loc[:, UnivariateSimulationResult.COL_UPPER_BOUND].round(
+            5
+        ),
         pd.Series(
-            [3.281693, 3.281693, 3.281693, 1.288981, -0.245838]
-            + [-0.431783, -0.81213, -1.046914, -1.046914],
+            [-0.21541, -0.21541, 0.02725, 0.44065, 0.66413, 0.66413],
             name=UnivariateSimulationResult.COL_UPPER_BOUND,
             index=index,
         ),
     )
 
-    assert_array_equal(
-        simulation_result.partitioner.frequencies_, [1, 4, 9, 10, 10, 6, 2, 1, 4]
-    )
+    assert_array_equal(simulation_result.partitioner.frequencies_, [2, 5, 18, 8, 11, 6])
 
     SimulationDrawer(style="text").draw(data=simulation_result)
 
 
 def test_univariate_probability_simulation(
     iris_classifier_binary: ClassifierPipelineDF[RandomForestClassifierDF],
     iris_sample_binary: Sample,
```

### Comparing `gamma-facet-2.0rc1/test/test/facet/test_validation.py` & `gamma-facet-2.0rc2/test/test/facet/test_validation.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 import numpy as np
 import numpy.typing as npt
 import pytest
 from sklearn import datasets, svm, tree
 from sklearn.model_selection import GridSearchCV
 
-from sklearndf import __sklearn_0_22__, __sklearn_version__
-
 from facet.validation import BootstrapCV, StratifiedBootstrapCV
 
 
 def test_bootstrap_cv_init() -> None:
     # filter out warnings triggered by sk-learn/numpy
 
     warnings.filterwarnings("ignore", message="numpy.dtype size changed")
@@ -84,19 +82,15 @@
     # define parameters and pipeline
 
     parameters = {"kernel": ("linear", "rbf"), "C": [1, 10]}
     svc = svm.SVC(gamma="scale")
 
     # use the defined my_cv bootstrap CV within GridSearchCV
 
-    if __sklearn_version__ < __sklearn_0_22__:
-        # noinspection PyArgumentList
-        clf = GridSearchCV(svc, parameters, cv=my_cv, iid=False)
-    else:
-        clf = GridSearchCV(svc, parameters, cv=my_cv)
+    clf = GridSearchCV(svc, parameters, cv=my_cv)
     clf.fit(iris.data, iris.target)
 
     # test if the number of received splits is correct
 
     assert (
         clf.n_splits_ == 50
     ), "50 splits should have been generated by the bootstrap CV"
```

### Comparing `gamma-facet-2.0rc1/tox.ini` & `gamma-facet-2.0rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `gamma-facet-2.0rc1/PKG-INFO` & `gamma-facet-2.0rc2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gamma-facet
-Version: 2.0rc1
+Version: 2.0rc2
 Summary: Human-explainable AI.
 Home-page: https://github.com/BCG-Gamma/facet
 License: Apache Software License v2.0
 Author: Boston Consulting Group (BCG)
 Requires-Python: >=3.7,<4a
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,22 +16,22 @@
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: gamma-pytools  ~=2.0.4
+Requires-Dist: gamma-pytools  >=2.1rc,<3a
 Requires-Dist: matplotlib     ~=3.0
 Requires-Dist: numpy          >=1.21,<2a
 Requires-Dist: packaging      >=20
 Requires-Dist: pandas         ~=1.0
 Requires-Dist: scipy          ~=1.2
 Requires-Dist: shap           >=0.34,<0.42a
-Requires-Dist: sklearndf      ~=2.0
+Requires-Dist: sklearndf      >=2.2rc,<3a
 Requires-Dist: sphinx ~= 4.5 ; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints ~= 1.19 ; extra == "docs"
 Requires-Dist: pydata-sphinx-theme ~= 0.8.1 ; extra == "docs"
 Requires-Dist: jinja2 ~= 2.11 ; extra == "docs"
 Requires-Dist: nbsphinx ~= 0.8.9 ; extra == "docs"
 Requires-Dist: jupyter == 1 ; extra == "docs"
 Requires-Dist: docutils ~= 0.17 ; extra == "docs"
```

