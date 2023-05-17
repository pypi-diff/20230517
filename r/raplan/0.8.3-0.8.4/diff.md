# Comparing `tmp/raplan-0.8.3.tar.gz` & `tmp/raplan-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raplan-0.8.3.tar", max compression
+gzip compressed data, was "raplan-0.8.4.tar", max compression
```

## Comparing `raplan-0.8.3.tar` & `raplan-0.8.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35400 2022-11-24 16:39:16.549070 raplan-0.8.3/LICENSE.rst
--rw-r--r--   0        0        0     2023 2022-11-24 16:39:16.551070 raplan-0.8.3/pyproject.toml
--rw-r--r--   0        0        0      161 2022-11-24 16:39:16.551070 raplan-0.8.3/raplan/__init__.py
--rw-r--r--   0        0        0     9119 2022-11-24 16:39:16.552070 raplan-0.8.3/raplan/analysis.py
--rw-r--r--   0        0        0    16848 2022-11-24 16:39:16.552070 raplan-0.8.3/raplan/classes.py
--rw-r--r--   0        0        0     5517 2022-11-24 16:39:16.552070 raplan-0.8.3/raplan/distributions.py
--rw-r--r--   0        0        0    13233 2022-11-24 16:39:16.552070 raplan-0.8.3/raplan/excel.py
--rw-r--r--   0        0        0    12589 2022-11-24 16:39:16.552070 raplan-0.8.3/raplan/plot.py
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 raplan-0.8.3/setup.py
--rw-r--r--   0        0        0     1121 1970-01-01 00:00:00.000000 raplan-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0    35400 2022-12-12 09:58:19.716751 raplan-0.8.4/LICENSE.rst
+-rw-r--r--   0        0        0     2023 2022-12-12 09:58:19.718752 raplan-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0      161 2022-12-12 09:58:19.718752 raplan-0.8.4/raplan/__init__.py
+-rw-r--r--   0        0        0     9119 2022-12-12 09:58:19.718752 raplan-0.8.4/raplan/analysis.py
+-rw-r--r--   0        0        0    16848 2022-12-12 09:58:19.719752 raplan-0.8.4/raplan/classes.py
+-rw-r--r--   0        0        0     5517 2022-12-12 09:58:19.719752 raplan-0.8.4/raplan/distributions.py
+-rw-r--r--   0        0        0    13233 2022-12-12 09:58:19.719752 raplan-0.8.4/raplan/excel.py
+-rw-r--r--   0        0        0    12857 2022-12-12 09:58:19.719752 raplan-0.8.4/raplan/plot.py
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 raplan-0.8.4/setup.py
+-rw-r--r--   0        0        0     1125 1970-01-01 00:00:00.000000 raplan-0.8.4/PKG-INFO
```

### Comparing `raplan-0.8.3/LICENSE.rst` & `raplan-0.8.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `raplan-0.8.3/pyproject.toml` & `raplan-0.8.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raplan"
-version = "0.8.3"
+version = "0.8.4"
 description = "Ratio planning and scheduling in Python."
 authors = ["Ratio Innovations B.V. <info@ratio-case.nl>"]
 license = "GPL-3.0-or-later"
 documentation = "https://raplan.ratio-case.nl"
 repository = "https://gitlab.com/ratio-case/python/raplan"
 homepage = "https://gitlab.com/ratio-case/python/raplan"
```

### Comparing `raplan-0.8.3/raplan/analysis.py` & `raplan-0.8.4/raplan/analysis.py`

 * *Files identical despite different names*

### Comparing `raplan-0.8.3/raplan/classes.py` & `raplan-0.8.4/raplan/classes.py`

 * *Files identical despite different names*

### Comparing `raplan-0.8.3/raplan/distributions.py` & `raplan-0.8.4/raplan/distributions.py`

 * *Files identical despite different names*

### Comparing `raplan-0.8.3/raplan/excel.py` & `raplan-0.8.4/raplan/excel.py`

 * *Files identical despite different names*

### Comparing `raplan-0.8.3/raplan/plot.py` & `raplan-0.8.4/raplan/plot.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,37 @@
 
 _BAR_STYLE = dict(
     bargap=0.0,
     bargroupgap=0.1,
     barmode="relative",
 )
 
+COLORS = [
+    "#0cc0aa",
+    "#9f3b60",
+    "#95b833",
+    "#a93713",
+    "#cfb2b0",
+    "#355952",
+    "#9085e0",
+    "#5a4b72",
+    "#da73f8",
+    "#08a9e5",
+    "#e81659",
+    "#4ed31b",
+    "#90089c",
+    "#cfa543",
+    "#ed7f61",
+    "#167b2b",
+    "#f62ef3",
+    "#4328e7",
+    "#856619",
+    "#3444bc",
+]
+
 
 @dataclass
 class Compound:
     """A fictive compound of CFP carrying items."""
 
     subjects: Sequence[Union[Component, System, Project, "Compound"]]
     name: str = "Compound"
@@ -291,18 +314,15 @@
     systems = sorted(set(p.system for p in procedures))
     system_to_index = {value: i for i, value in enumerate(systems)}
 
     procedures = sorted(
         procedures, key=lambda p: (p.kind, p.system, p.time, -p.cost, -p.duration)
     )
 
-    colors = {
-        kind: qualitative.Plotly[i % len(qualitative.Plotly)]
-        for i, kind in enumerate(kinds)
-    }
+    colors = {kind: COLORS[i % len(COLORS)] for i, kind in enumerate(kinds)}
     hm_colors = [(float(i), colors[kind]) for i, kind in enumerate(kinds)]
 
     xs = list(range(int(_times[0]), int(_times[-1] + 1)))
 
     heatmap_z: list[list[Optional[int]]] = [[None for j in xs] for i in systems]
     heatmap_text: list[list[Optional[str]]] = [[None for j in xs] for i in systems]
     for p in procedures:
```

### Comparing `raplan-0.8.3/setup.py` & `raplan-0.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
          'openpyxl>=3.0.10,<4.0.0'],
  'analysis': ['ragraph>=1.16.0,<2.0.0'],
  'excel': ['openpyxl>=3.0.10,<4.0.0'],
  'plot': ['plotly>=5.7.0,<6.0.0', 'kaleido==0.2.1']}
 
 setup_kwargs = {
     'name': 'raplan',
-    'version': '0.8.3',
+    'version': '0.8.4',
     'description': 'Ratio planning and scheduling in Python.',
     'long_description': 'None',
     'author': 'Ratio Innovations B.V.',
     'author_email': 'info@ratio-case.nl',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ratio-case/python/raplan',
```

### Comparing `raplan-0.8.3/PKG-INFO` & `raplan-0.8.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raplan
-Version: 0.8.3
+Version: 0.8.4
 Summary: Ratio planning and scheduling in Python.
 Home-page: https://gitlab.com/ratio-case/python/raplan
 License: GPL-3.0-or-later
 Author: Ratio Innovations B.V.
 Author-email: info@ratio-case.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
@@ -12,14 +12,14 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: analysis
 Provides-Extra: excel
 Provides-Extra: plot
-Requires-Dist: kaleido (==0.2.1); extra == "plot" or extra == "all"
-Requires-Dist: openpyxl (>=3.0.10,<4.0.0); extra == "excel" or extra == "all"
-Requires-Dist: plotly (>=5.7.0,<6.0.0); extra == "plot" or extra == "all"
+Requires-Dist: kaleido (==0.2.1) ; extra == "plot" or extra == "all"
+Requires-Dist: openpyxl (>=3.0.10,<4.0.0) ; extra == "excel" or extra == "all"
+Requires-Dist: plotly (>=5.7.0,<6.0.0) ; extra == "plot" or extra == "all"
 Requires-Dist: pyserde[yaml] (>=0.9.2,<0.10.0)
-Requires-Dist: ragraph (>=1.16.0,<2.0.0); extra == "analysis" or extra == "all"
+Requires-Dist: ragraph (>=1.16.0,<2.0.0) ; extra == "analysis" or extra == "all"
 Project-URL: Documentation, https://raplan.ratio-case.nl
 Project-URL: Repository, https://gitlab.com/ratio-case/python/raplan
```

