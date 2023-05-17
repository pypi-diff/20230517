# Comparing `tmp/freyja_plot-0.1.0.tar.gz` & `tmp/freyja_plot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freyja_plot-0.1.0.tar", max compression
+gzip compressed data, was "freyja_plot-0.2.0.tar", max compression
```

## Comparing `freyja_plot-0.1.0.tar` & `freyja_plot-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,16 @@
--rwxr-xr-x   0        0        0     1065 2023-05-01 17:02:13.516327 freyja_plot-0.1.0/LICENSE
--rwxr-xr-x   0        0        0     5930 2023-05-01 21:26:40.400041 freyja_plot-0.1.0/README.md
--rwxr-xr-x   0        0        0     1004 2023-05-01 21:27:35.768186 freyja_plot-0.1.0/example/create_test_plots.py
--rwxr-xr-x   0        0        0  3598080 2023-05-01 18:11:39.770519 freyja_plot-0.1.0/example/example_images/batch_comparison_example.html
--rwxr-xr-x   0        0        0    39533 2023-05-01 20:24:24.676588 freyja_plot-0.1.0/example/example_images/batch_comparison_example.png
--rwxr-xr-x   0        0        0    51128 2023-05-01 21:08:17.397157 freyja_plot-0.1.0/example/example_images/batch_comparison_selection_example.png
--rwxr-xr-x   0        0        0    44892 2023-05-01 20:24:24.114256 freyja_plot-0.1.0/example/example_images/superlineage_example.png
--rwxr-xr-x   0        0        0    51128 2023-05-01 21:08:20.118561 freyja_plot-0.1.0/example/test_images/batch_comparison_example.png
--rwxr-xr-x   0        0        0    29979 2023-05-01 21:08:14.277198 freyja_plot-0.1.0/example/test_images/summarized_example.png
--rwxr-xr-x   0        0        0    44892 2023-05-01 21:08:14.120984 freyja_plot-0.1.0/example/test_images/superlineage_example.png
--rwxr-xr-x   0        0        0    18144 2023-05-01 17:34:35.679310 freyja_plot-0.1.0/example/wastewater-freyja-aggregated.tsv
--rwxr-xr-x   0        0        0    30790 2023-05-01 17:46:00.523531 freyja_plot-0.1.0/example/wastewater-freyja-compare1.tsv
--rwxr-xr-x   0        0        0    23696 2023-05-01 17:46:24.707912 freyja_plot-0.1.0/example/wastewater-freyja-compare2.tsv
--rwxr-xr-x   0        0        0       96 2023-05-01 17:13:37.160319 freyja_plot-0.1.0/freyja_plot/__init__.py
--rwxr-xr-x   0        0        0    11064 2023-05-01 19:59:26.444819 freyja_plot-0.1.0/freyja_plot/freyja_plot.py
--rwxr-xr-x   0        0        0      543 2023-05-02 13:03:11.643983 freyja_plot-0.1.0/freyja_plot/main.py
--rwxr-xr-x   0        0        0       89 2023-05-01 17:14:03.847868 freyja_plot-0.1.0/freyja_plot/version.py
--rwxr-xr-x   0        0        0      678 2023-05-02 13:08:42.570534 freyja_plot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6805 1970-01-01 00:00:00.000000 freyja_plot-0.1.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1065 2023-05-01 17:02:13.516327 freyja_plot-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     6088 2023-05-16 20:41:59.765968 freyja_plot-0.2.0/README.md
+-rwxr-xr-x   0        0        0     1004 2023-05-01 21:27:35.768186 freyja_plot-0.2.0/example/create_test_plots.py
+-rwxr-xr-x   0        0        0  3598080 2023-05-01 18:11:39.770519 freyja_plot-0.2.0/example/example_images/batch_comparison_example.html
+-rwxr-xr-x   0        0        0    39533 2023-05-01 20:24:24.676588 freyja_plot-0.2.0/example/example_images/batch_comparison_example.png
+-rwxr-xr-x   0        0        0    51128 2023-05-01 21:08:17.397157 freyja_plot-0.2.0/example/example_images/batch_comparison_selection_example.png
+-rwxr-xr-x   0        0        0    44892 2023-05-01 20:24:24.114256 freyja_plot-0.2.0/example/example_images/superlineage_example.png
+-rwxr-xr-x   0        0        0    18144 2023-05-01 17:34:35.679310 freyja_plot-0.2.0/example/wastewater-freyja-aggregated.tsv
+-rwxr-xr-x   0        0        0    30790 2023-05-01 17:46:00.523531 freyja_plot-0.2.0/example/wastewater-freyja-compare1.tsv
+-rwxr-xr-x   0        0        0    23696 2023-05-01 17:46:24.707912 freyja_plot-0.2.0/example/wastewater-freyja-compare2.tsv
+-rwxr-xr-x   0        0        0       96 2023-05-01 17:13:37.160319 freyja_plot-0.2.0/freyja_plot/__init__.py
+-rwxr-xr-x   0        0        0    26782 2023-05-17 20:55:25.401722 freyja_plot-0.2.0/freyja_plot/freyja_plot.py
+-rwxr-xr-x   0        0        0      543 2023-05-02 13:03:11.643983 freyja_plot-0.2.0/freyja_plot/main.py
+-rwxr-xr-x   0        0        0       89 2023-05-01 17:14:03.847868 freyja_plot-0.2.0/freyja_plot/version.py
+-rwxr-xr-x   0        0        0      678 2023-05-16 20:05:35.590367 freyja_plot-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6963 1970-01-01 00:00:00.000000 freyja_plot-0.2.0/PKG-INFO
```

### Comparing `freyja_plot-0.1.0/LICENSE` & `freyja_plot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/README.md` & `freyja_plot-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -61,17 +61,22 @@
 ```python
 plotter.plotLineages(summarized=True,fn="summarized_lineage_abundance_example.html")
 ```
 
 To view higher level lineage assignments with the non-summarized freyja output, the `superlineage` flag can be used. The base `superlineage` is demarked level 0. Each next sublineage (to the next ".") can be attained by adding 1 for each sublineage desired. 'BA.5.1' with a requested sublineage of 0 would return 'BA.*', as would a sample with the lineage 'BA'. For less specific lineages, if the `superlineage` level gets to high, the most specific lineage possible will be returned. 'BA.5.1' with a requested sublineage of 5 would still only return 'BA.5.1'.
 ```python
 # plotting superlineage, level 0: e.g. BA.* ()
-plotter.plotLineages(superlineage=0,fn="superlineage_abundance_example.html")
+fig1 = plotter.plotLineages(superlineage=0,fn="superlineage_abundance_example.html")
 # plotting superlineage, level 2: e.g. BA.5.1.* ()
-plotter.plotLineages(superlineage=2,fn="superlineage_abundance_example.html")
+fig2 = plotter.plotLineages(superlineage=2,fn="superlineage_abundance_example.html")
+```
+
+To stack multiple lineage plots
+```python
+plotter.plotLineages([fig1,fig2],["Fig 1 Title","Fig 2 Title"],fn="combined_plots_example.html")
 ```
 
 #### Example plots
 Here's an example plot from a single batch.
 
 ![superlineage_example.png](example/example_images/superlineage_example.png?raw=true "Lineage abundance plot with superlineage=2 - png")
```

### Comparing `freyja_plot-0.1.0/example/create_test_plots.py` & `freyja_plot-0.2.0/example/create_test_plots.py`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/example/example_images/batch_comparison_example.html` & `freyja_plot-0.2.0/example/example_images/batch_comparison_example.html`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/example/example_images/batch_comparison_example.png` & `freyja_plot-0.2.0/example/example_images/batch_comparison_example.png`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/example/example_images/batch_comparison_selection_example.png` & `freyja_plot-0.2.0/example/example_images/batch_comparison_selection_example.png`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/example/example_images/superlineage_example.png` & `freyja_plot-0.2.0/example/example_images/superlineage_example.png`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/example/wastewater-freyja-aggregated.tsv` & `freyja_plot-0.2.0/example/wastewater-freyja-aggregated.tsv`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/example/wastewater-freyja-compare1.tsv` & `freyja_plot-0.2.0/example/wastewater-freyja-compare1.tsv`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/example/wastewater-freyja-compare2.tsv` & `freyja_plot-0.2.0/example/wastewater-freyja-compare2.tsv`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/freyja_plot/main.py` & `freyja_plot-0.2.0/freyja_plot/main.py`

 * *Files identical despite different names*

### Comparing `freyja_plot-0.1.0/pyproject.toml` & `freyja_plot-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "freyja-plot"
-version = "0.1.0"
+version = "0.2.0"
 description = "Plotting lineage abundance for individual samples from aggregated freyja demix results"
 authors = ["Sam Kunkleman <skunklem@uncc.edu>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "freyja_plot"},
     {include = "example"}
```

### Comparing `freyja_plot-0.1.0/PKG-INFO` & `freyja_plot-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freyja-plot
-Version: 0.1.0
+Version: 0.2.0
 Summary: Plotting lineage abundance for individual samples from aggregated freyja demix results
 Home-page: https://github.com/enviro-lab/freyja-plot.git
 License: MIT
 Keywords: freyja,plot,lineage,abundance,covid
 Author: Sam Kunkleman
 Author-email: skunklem@uncc.edu
 Requires-Python: >=3.8,<4.0
@@ -83,17 +83,22 @@
 ```python
 plotter.plotLineages(summarized=True,fn="summarized_lineage_abundance_example.html")
 ```
 
 To view higher level lineage assignments with the non-summarized freyja output, the `superlineage` flag can be used. The base `superlineage` is demarked level 0. Each next sublineage (to the next ".") can be attained by adding 1 for each sublineage desired. 'BA.5.1' with a requested sublineage of 0 would return 'BA.*', as would a sample with the lineage 'BA'. For less specific lineages, if the `superlineage` level gets to high, the most specific lineage possible will be returned. 'BA.5.1' with a requested sublineage of 5 would still only return 'BA.5.1'.
 ```python
 # plotting superlineage, level 0: e.g. BA.* ()
-plotter.plotLineages(superlineage=0,fn="superlineage_abundance_example.html")
+fig1 = plotter.plotLineages(superlineage=0,fn="superlineage_abundance_example.html")
 # plotting superlineage, level 2: e.g. BA.5.1.* ()
-plotter.plotLineages(superlineage=2,fn="superlineage_abundance_example.html")
+fig2 = plotter.plotLineages(superlineage=2,fn="superlineage_abundance_example.html")
+```
+
+To stack multiple lineage plots
+```python
+plotter.plotLineages([fig1,fig2],["Fig 1 Title","Fig 2 Title"],fn="combined_plots_example.html")
 ```
 
 #### Example plots
 Here's an example plot from a single batch.
 
 ![superlineage_example.png](example/example_images/superlineage_example.png?raw=true "Lineage abundance plot with superlineage=2 - png")
```

