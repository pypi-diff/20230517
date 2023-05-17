# Comparing `tmp/subgrounds-1.5.1.tar.gz` & `tmp/subgrounds-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subgrounds-1.5.1.tar", max compression
+gzip compressed data, was "subgrounds-1.5.2.tar", max compression
```

## Comparing `subgrounds-1.5.1.tar` & `subgrounds-1.5.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0    11357 2023-05-15 17:03:03.320694 subgrounds-1.5.1/LICENSE
--rw-r--r--   0        0        0     3855 2023-05-15 17:03:03.320694 subgrounds-1.5.1/README.md
--rw-r--r--   0        0        0     1929 2023-05-15 17:05:01.117202 subgrounds-1.5.1/pyproject.toml
--rw-r--r--   0        0        0      317 2023-05-15 17:05:01.089202 subgrounds-1.5.1/subgrounds/__init__.py
--rw-r--r--   0        0        0     4521 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/client.py
--rw-r--r--   0        0        0     1895 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/README.md
--rw-r--r--   0        0        0      349 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/dash/__init__.py
--rw-r--r--   0        0        0      399 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/dash/abcs.py
--rw-r--r--   0        0        0     3893 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/dash/components.py
--rw-r--r--   0        0        0     1285 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/plotly/__init__.py
--rw-r--r--   0        0        0     1316 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/plotly/figure.py
--rw-r--r--   0        0        0     5866 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/plotly/traces.py
--rw-r--r--   0        0        0      873 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/contrib/pyodide.py
--rw-r--r--   0        0        0      438 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/dash_wrappers.py
--rw-r--r--   0        0        0    10062 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/dataframe_utils.py
--rw-r--r--   0        0        0      395 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/errors.py
--rw-r--r--   0        0        0     1027 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/__init__.py
--rw-r--r--   0        0        0     4761 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/pagination.py
--rw-r--r--   0        0        0    12577 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/preprocess.py
--rw-r--r--   0        0        0    17155 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/strategies.py
--rw-r--r--   0        0        0     2901 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/pagination/utils.py
--rw-r--r--   0        0        0     1460 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/plotly_wrappers.py
--rw-r--r--   0        0        0    62357 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/query.py
--rw-r--r--   0        0        0    13291 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/schema.py
--rw-r--r--   0        0        0      308 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/__init__.py
--rw-r--r--   0        0        0    38891 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/fieldpath.py
--rw-r--r--   0        0        0     1669 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/filter.py
--rw-r--r--   0        0        0     4754 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/object.py
--rw-r--r--   0        0        0     2550 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgraph/subgraph.py
--rw-r--r--   0        0        0    21574 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/subgrounds.py
--rw-r--r--   0        0        0    20072 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/transform.py
--rw-r--r--   0        0        0     6981 2023-05-15 17:03:03.324694 subgrounds-1.5.1/subgrounds/utils.py
--rw-r--r--   0        0        0     5138 1970-01-01 00:00:00.000000 subgrounds-1.5.1/setup.py
--rw-r--r--   0        0        0     4932 1970-01-01 00:00:00.000000 subgrounds-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-17 00:26:12.912576 subgrounds-1.5.2/LICENSE
+-rw-r--r--   0        0        0     3855 2023-05-17 00:26:12.912576 subgrounds-1.5.2/README.md
+-rw-r--r--   0        0        0     1929 2023-05-17 00:26:38.508911 subgrounds-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0      317 2023-05-17 00:26:38.488910 subgrounds-1.5.2/subgrounds/__init__.py
+-rw-r--r--   0        0        0     4521 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/client.py
+-rw-r--r--   0        0        0     1895 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/contrib/README.md
+-rw-r--r--   0        0        0      349 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/contrib/dash/__init__.py
+-rw-r--r--   0        0        0      399 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/contrib/dash/abcs.py
+-rw-r--r--   0        0        0     3893 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/contrib/dash/components.py
+-rw-r--r--   0        0        0     1285 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/contrib/plotly/__init__.py
+-rw-r--r--   0        0        0     1316 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/contrib/plotly/figure.py
+-rw-r--r--   0        0        0     5866 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/contrib/plotly/traces.py
+-rw-r--r--   0        0        0      873 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/contrib/pyodide.py
+-rw-r--r--   0        0        0      438 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/dash_wrappers.py
+-rw-r--r--   0        0        0    10062 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/dataframe_utils.py
+-rw-r--r--   0        0        0      395 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/errors.py
+-rw-r--r--   0        0        0     1027 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/pagination/__init__.py
+-rw-r--r--   0        0        0     4761 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/pagination/pagination.py
+-rw-r--r--   0        0        0    12577 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/pagination/preprocess.py
+-rw-r--r--   0        0        0    17155 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/pagination/strategies.py
+-rw-r--r--   0        0        0     2901 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/pagination/utils.py
+-rw-r--r--   0        0        0     1460 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/plotly_wrappers.py
+-rw-r--r--   0        0        0    62357 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/query.py
+-rw-r--r--   0        0        0    13291 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/schema.py
+-rw-r--r--   0        0        0      308 2023-05-17 00:26:12.912576 subgrounds-1.5.2/subgrounds/subgraph/__init__.py
+-rw-r--r--   0        0        0    38793 2023-05-17 00:26:12.916576 subgrounds-1.5.2/subgrounds/subgraph/fieldpath.py
+-rw-r--r--   0        0        0     1669 2023-05-17 00:26:12.916576 subgrounds-1.5.2/subgrounds/subgraph/filter.py
+-rw-r--r--   0        0        0     4754 2023-05-17 00:26:12.916576 subgrounds-1.5.2/subgrounds/subgraph/object.py
+-rw-r--r--   0        0        0     2550 2023-05-17 00:26:12.916576 subgrounds-1.5.2/subgrounds/subgraph/subgraph.py
+-rw-r--r--   0        0        0    21574 2023-05-17 00:26:12.916576 subgrounds-1.5.2/subgrounds/subgrounds.py
+-rw-r--r--   0        0        0    20072 2023-05-17 00:26:12.916576 subgrounds-1.5.2/subgrounds/transform.py
+-rw-r--r--   0        0        0     6981 2023-05-17 00:26:12.916576 subgrounds-1.5.2/subgrounds/utils.py
+-rw-r--r--   0        0        0     5138 1970-01-01 00:00:00.000000 subgrounds-1.5.2/setup.py
+-rw-r--r--   0        0        0     4932 1970-01-01 00:00:00.000000 subgrounds-1.5.2/PKG-INFO
```

### Comparing `subgrounds-1.5.1/LICENSE` & `subgrounds-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/README.md` & `subgrounds-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/pyproject.toml` & `subgrounds-1.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "subgrounds"
-version = "1.5.1"
+version = "1.5.2"
 description = "A Pythonic data access layer for applications querying data from The Graph Network."
 authors = [
     "cvauclair <cvauclair@playgrounds.network>",
     "0xMochan <mochan@playgrounds.network>",
 ]
 repository = "https://github.com/0xPlaygrounds/subgrounds"
```

### Comparing `subgrounds-1.5.1/subgrounds/client.py` & `subgrounds-1.5.2/subgrounds/client.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/contrib/README.md` & `subgrounds-1.5.2/subgrounds/contrib/README.md`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/contrib/dash/components.py` & `subgrounds-1.5.2/subgrounds/contrib/dash/components.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/contrib/plotly/__init__.py` & `subgrounds-1.5.2/subgrounds/contrib/plotly/__init__.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/contrib/plotly/figure.py` & `subgrounds-1.5.2/subgrounds/contrib/plotly/figure.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/contrib/plotly/traces.py` & `subgrounds-1.5.2/subgrounds/contrib/plotly/traces.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/contrib/pyodide.py` & `subgrounds-1.5.2/subgrounds/contrib/pyodide.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/dataframe_utils.py` & `subgrounds-1.5.2/subgrounds/dataframe_utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/pagination/__init__.py` & `subgrounds-1.5.2/subgrounds/pagination/__init__.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/pagination/pagination.py` & `subgrounds-1.5.2/subgrounds/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/pagination/preprocess.py` & `subgrounds-1.5.2/subgrounds/pagination/preprocess.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/pagination/strategies.py` & `subgrounds-1.5.2/subgrounds/pagination/strategies.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/pagination/utils.py` & `subgrounds-1.5.2/subgrounds/pagination/utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/plotly_wrappers.py` & `subgrounds-1.5.2/subgrounds/plotly_wrappers.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/query.py` & `subgrounds-1.5.2/subgrounds/query.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/schema.py` & `subgrounds-1.5.2/subgrounds/schema.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/subgraph/fieldpath.py` & `subgrounds-1.5.2/subgrounds/subgraph/fieldpath.py`

 * *Files 1% similar despite different names*

```diff
@@ -226,14 +226,15 @@
     for fmeta in object_.fields:
         if not fmeta.type_.is_list and len(fmeta.arguments) == 0:
             match subgraph._schema.type_of_typeref(fmeta.type_):
                 case TypeMeta.ObjectMeta() | TypeMeta.InterfaceMeta():
                     yield subgraph.__getattribute__(object_.name).__getattribute__(
                         fmeta.name
                     ).id
+
                 case _:
                     yield subgraph.__getattribute__(object_.name).__getattribute__(
                         fmeta.name
                     )
 
 
 @dataclass
@@ -452,21 +453,19 @@
         """
 
         def fmt_arg(name, raw_arg):
             match (name, raw_arg):
                 case ("where", [Filter(), *_] as filters):
                     return Filter.to_dict(filters)
                 case ("orderBy", FieldPath() as fpath):
-                    match fpath._leaf:
-                        case TypeMeta.FieldMeta() as fmeta:
-                            return fmeta.name
-                        case _:
-                            raise Exception(
-                                f"Cannot use non field {fpath} as orderBy argument"
-                            )
+                    if paths := fpath._name_path():
+                        return "__".join(paths)
+                    raise Exception(
+                        f"Cannot use empty paths as orderBy argument {fpath}"
+                    )
                 case _:
                     return raw_arg
 
         match self._leaf:
             case TypeMeta.FieldMeta():
                 args = {key: fmt_arg(key, val) for key, val in args.items()}
                 self._path[-1] = (args, self._path[-1][1])
```

### Comparing `subgrounds-1.5.1/subgrounds/subgraph/filter.py` & `subgrounds-1.5.2/subgrounds/subgraph/filter.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/subgraph/object.py` & `subgrounds-1.5.2/subgrounds/subgraph/object.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/subgraph/subgraph.py` & `subgrounds-1.5.2/subgrounds/subgraph/subgraph.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/subgrounds.py` & `subgrounds-1.5.2/subgrounds/subgrounds.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/transform.py` & `subgrounds-1.5.2/subgrounds/transform.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/subgrounds/utils.py` & `subgrounds-1.5.2/subgrounds/utils.py`

 * *Files identical despite different names*

### Comparing `subgrounds-1.5.1/setup.py` & `subgrounds-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
          'pyodide-http>=0.2.1,<0.3.0'],
  'dash': ['dash>=2.3.1,<3.0.0'],
  'plotly': ['plotly>=5.14.1,<6.0.0'],
  'pyodide': ['pyodide-http>=0.2.1,<0.3.0']}
 
 setup_kwargs = {
     'name': 'subgrounds',
-    'version': '1.5.1',
+    'version': '1.5.2',
     'description': 'A Pythonic data access layer for applications querying data from The Graph Network.',
     'long_description': "# Subgrounds\n<!-- [![GitHub Actions](https://github.com/0xPlaygrounds/subgrounds/workflows/CI/badge.svg)](https://github.com/0xPlaygrounds/subgrounds/actions) -->\n[![PyPI](https://img.shields.io/pypi/v/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/subgrounds.svg)](https://pypi.org/project/subgrounds/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n<br>\n\n[![Discord](https://img.shields.io/discord/896944341598208070?color=7289DA&label=discord&logo=discord&logoColor=fff)](https://discord.gg/gMSSh5bjvk)\n[![Twitter Follow](https://img.shields.io/badge/Playgrounds-Analytics-31fa1f2Playgrounds0x?color=%231fa1f2&logo=Twitter&logoColor=1fa1f2&style=flat)](https://twitter.com/Playgrounds0x)\n\n[![Open Notebook in Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/0xPlaygrounds/jupyter-stacks-subgrounds/HEAD?labpath=index.ipynb)\n[![Github Codepsaces](https://img.shields.io/badge/Github-Codespaces-24292f.svg?logo=Github)](https://codespaces.new/0xPlaygrounds/subgrounds-template?quickstart=1)\n\n<!-- start elevator-pitch -->\nAn intuitive python library for interfacing with Subgraphs.\n\n## Features\n- **Simple**: Leverage a Pythonic API to easily build queries and transformations without the need for raw GraphQL manipulation.\n- **Automated**: Automatically handle pagination and schema introspection for effortless data retrieval.\n- **Powerful**: Create sophisticated queries using the `SyntheticFields` transformation system.\n\n<!-- end elevator-pitch -->\n\n## Resources\n- [**Subgrounds Docs**](http://docs.playgrounds.network/): User guide and API documentation\n- [**Examples**](https://github.com/0xPlaygrounds/subgrounds/tree/main/examples): A list of examples showcasing Subgrounds integration with Dash and Plotly\n- [**Community projects**](http://docs.playgrounds.network/subgrounds/examples/): An ever growing list of projects created by our community members\n- [**MetricsDAO Subgrounds Workshop**](https://docs.metricsdao.xyz/get-involved/workshops/2022-03-30+-subgrounds-workshop-series): Subgrounds workshop series hosted by MetricsDAO \n\n## Installation\n> Subgrounds **requires** atleast Python 3.10+\n\nSubgrounds is available on PyPi. To install it, run the following:<br>\n`pip install subgrounds`.\n\nSubgrounds also comes bundled with extra modules that may require extra libraries. You can get all functionality of `subgrounds` via the following:<br>\n`pip install subgrounds[all]`.\n\n## Simple example\n<!-- start simple-example -->\n```python\n>>> from subgrounds import Subgrounds\n\n>>> sg = Subgrounds()\n\n>>> # Load\n>>> aave_v2 = sg.load_subgraph('https://api.thegraph.com/subgraphs/name/messari/aave-v2-ethereum')\n\n>>> # Construct the query\n>>> latest = aave_v2.Query.markets(\n  orderBy=aave_v2.Market.totalValueLockedUSD,\n  orderDirection='desc',\n  first=5,\n)\n\n>>> # Return query to a dataframe\n>>> sg.query_df([\n  latest.name,\n  latest.totalValueLockedUSD,\n])\n                  markets_name  markets_totalValueLockedUSD\n0  Aave interest bearing STETH                 1.522178e+09\n1   Aave interest bearing WETH                 1.221299e+09\n2   Aave interest bearing USDC                 8.140547e+08\n3   Aave interest bearing WBTC                 6.615692e+08\n4   Aave interest bearing USDT                 3.734017e+08\n```\n<!-- end simple-example -->\n\n\n## About Us\nPlaygrounds Analytics is a data solutions company providing serverless on-chain data infrastructures and services for data teams, analysts, and engineers. Checkout us out [here](https://playgrounds.network/) to learn more!\n\n\n## Acknowledgments\nThis software project would not be possible without the support of The Graph Foundation. You can learn more about The Graph and its mission [here](https://thegraph.com/).\n",
     'author': 'cvauclair',
     'author_email': 'cvauclair@playgrounds.network',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xPlaygrounds/subgrounds',
```

### Comparing `subgrounds-1.5.1/PKG-INFO` & `subgrounds-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subgrounds
-Version: 1.5.1
+Version: 1.5.2
 Summary: A Pythonic data access layer for applications querying data from The Graph Network.
 Home-page: https://github.com/0xPlaygrounds/subgrounds
 Keywords: graph,subgrounds,graphql,subgraph
 Author: cvauclair
 Author-email: cvauclair@playgrounds.network
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

