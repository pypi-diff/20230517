# Comparing `tmp/statscend-0.1.7.tar.gz` & `tmp/statscend-0.1.8.tar.gz`

## Comparing `statscend-0.1.7.tar` & `statscend-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.7/.DS_Store
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/__init__.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/bn_logistic_regression.py
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/datasets.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/linear_regression.py
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/mn_logistic_regression.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 statscend-0.1.7/statscend/ordinal_regression.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.7/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.7/LICENSE
--rw-r--r--   0        0        0    13214 2020-02-02 00:00:00.000000 statscend-0.1.7/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.7/pyproject.toml
--rw-r--r--   0        0        0    15140 2020-02-02 00:00:00.000000 statscend-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 statscend-0.1.8/.DS_Store
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/__init__.py
+-rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/bn_logistic_regression.py
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/datasets.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/linear_regression.py
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/mn_logistic_regression.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 statscend-0.1.8/statscend/ordinal_regression.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 statscend-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 statscend-0.1.8/LICENSE
+-rw-r--r--   0        0        0    13432 2020-02-02 00:00:00.000000 statscend-0.1.8/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 statscend-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0    15358 2020-02-02 00:00:00.000000 statscend-0.1.8/PKG-INFO
```

### Comparing `statscend-0.1.7/.DS_Store` & `statscend-0.1.8/.DS_Store`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 0000 0001 4275 6431 0000 1000 0000 0800  ....Bud1........
 00000010: 0000 1000 0000 040a 0000 0000 0000 0000  ................
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
 00000040: 0000 0000 0000 0002 0000 0000 0000 0008  ................
 00000050: 0000 0001 0000 1000 6277 7370 626c 6f62  ........bwspblob
-00000060: 0000 00c9 0000 0000 0000 0000 0000 0000  ................
+00000060: 0000 00c8 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -60,56 +60,56 @@
 000003b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000003f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000400: 0000 0000 0000 0000 0000 0008 0000 0004  ................
 00000410: 0064 0069 0073 0074 6277 7370 626c 6f62  .d.i.s.tbwspblob
-00000420: 0000 00c9 6270 6c69 7374 3030 d701 0203  ....bplist00....
+00000420: 0000 00c8 6270 6c69 7374 3030 d701 0203  ....bplist00....
 00000430: 0405 0607 0809 0909 090d 095d 5368 6f77  ...........]Show
 00000440: 5374 6174 7573 4261 725b 5368 6f77 5061  StatusBar[ShowPa
 00000450: 7468 6261 725b 5368 6f77 546f 6f6c 6261  thbar[ShowToolba
 00000460: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
 00000470: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
 00000480: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
 00000490: 735b 5368 6f77 5369 6465 6261 7208 0909  s[ShowSidebar...
-000004a0: 0909 5f10 187b 7b32 3639 2c20 3134 367d  .._..{{269, 146}
-000004b0: 2c20 7b37 3730 2c20 3530 357d 7d09 0817  , {770, 505}}...
-000004c0: 2531 3d49 606d 797a 7b7c 7d7e 9900 0000  %1=I`myz{|}~....
-000004d0: 0000 0001 0100 0000 0000 0000 0f00 0000  ................
-000004e0: 0000 0000 0000 0000 0000 0000 9a00 0000  ................
-000004f0: 0400 6400 6900 7300 7476 5372 6e6c 6f6e  ..d.i.s.tvSrnlon
-00000500: 6700 0000 0100 0000 0900 7300 7400 6100  g.........s.t.a.
-00000510: 7400 7300 6300 6500 6e00 6462 7773 7062  t.s.c.e.n.dbwspb
-00000520: 6c6f 6200 0000 c962 706c 6973 7430 30d7  lob....bplist00.
-00000530: 0102 0304 0506 0708 0909 0909 0d09 5d53  ..............]S
-00000540: 686f 7753 7461 7475 7342 6172 5b53 686f  howStatusBar[Sho
-00000550: 7750 6174 6862 6172 5b53 686f 7754 6f6f  wPathbar[ShowToo
-00000560: 6c62 6172 5b53 686f 7754 6162 5669 6577  lbar[ShowTabView
-00000570: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
-00000580: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
-00000590: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
-000005a0: 0809 0909 095f 1018 7b7b 3135 372c 2032  ....._..{{157, 2
-000005b0: 3030 7d2c 207b 3737 302c 2035 3035 7d7d  00}, {770, 505}}
-000005c0: 0908 1725 313d 4960 6d79 7a7b 7c7d 7e99  ...%1=I`myz{|}~.
-000005d0: 0000 0000 0000 0101 0000 0000 0000 000f  ................
-000005e0: 0000 0000 0000 0000 0000 0000 0000 009a  ................
-000005f0: 0000 0009 0073 0074 0061 0074 0073 0063  .....s.t.a.t.s.c
-00000600: 0065 006e 0064 6c67 3153 636f 6d70 0000  .e.n.dlg1Scomp..
-00000610: 0000 0000 0000 0000 0009 0073 0074 0061  ...........s.t.a
-00000620: 0074 0073 0063 0065 006e 0064 6d6f 4444  .t.s.c.e.n.dmoDD
-00000630: 626c 6f62 0000 0008 a325 a8d1 5eed c441  blob.....%..^..A
-00000640: 0000 0009 0073 0074 0061 0074 0073 0063  .....s.t.a.t.s.c
-00000650: 0065 006e 0064 6d6f 6444 626c 6f62 0000  .e.n.dmodDblob..
-00000660: 0008 a325 a8d1 5eed c441 0000 0009 0073  ...%..^..A.....s
-00000670: 0074 0061 0074 0073 0063 0065 006e 0064  .t.a.t.s.c.e.n.d
-00000680: 7068 3153 636f 6d70 0000 0000 0000 0000  ph1Scomp........
-00000690: 0000 0009 0073 0074 0061 0074 0073 0063  .....s.t.a.t.s.c
-000006a0: 0065 006e 0064 7653 726e 6c6f 6e67 0000  .e.n.dvSrnlong..
-000006b0: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+000004a0: 0909 5f10 177b 7b38 302c 2031 3937 7d2c  .._..{{80, 197},
+000004b0: 207b 3731 332c 2035 3035 7d7d 0908 1725   {713, 505}}...%
+000004c0: 313d 4960 6d79 7a7b 7c7d 7e98 0000 0000  1=I`myz{|}~.....
+000004d0: 0000 0101 0000 0000 0000 000f 0000 0000  ................
+000004e0: 0000 0000 0000 0000 0000 0099 0000 0004  ................
+000004f0: 0064 0069 0073 0074 7653 726e 6c6f 6e67  .d.i.s.tvSrnlong
+00000500: 0000 0001 0000 0009 0073 0074 0061 0074  .........s.t.a.t
+00000510: 0073 0063 0065 006e 0064 6277 7370 626c  .s.c.e.n.dbwspbl
+00000520: 6f62 0000 00c9 6270 6c69 7374 3030 d701  ob....bplist00..
+00000530: 0203 0405 0607 0809 0909 090d 095d 5368  .............]Sh
+00000540: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00000550: 5061 7468 6261 725b 5368 6f77 546f 6f6c  Pathbar[ShowTool
+00000560: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
+00000570: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
+00000580: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
+00000590: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
+000005a0: 0909 0909 5f10 187b 7b31 3537 2c20 3230  ...._..{{157, 20
+000005b0: 307d 2c20 7b37 3730 2c20 3530 357d 7d09  0}, {770, 505}}.
+000005c0: 0817 2531 3d49 606d 797a 7b7c 7d7e 9900  ..%1=I`myz{|}~..
+000005d0: 0000 0000 0001 0100 0000 0000 0000 0f00  ................
+000005e0: 0000 0000 0000 0000 0000 0000 0000 9a00  ................
+000005f0: 0000 0900 7300 7400 6100 7400 7300 6300  ....s.t.a.t.s.c.
+00000600: 6500 6e00 646c 6731 5363 6f6d 7000 0000  e.n.dlg1Scomp...
+00000610: 0000 0000 0000 0000 0900 7300 7400 6100  ..........s.t.a.
+00000620: 7400 7300 6300 6500 6e00 646d 6f44 4462  t.s.c.e.n.dmoDDb
+00000630: 6c6f 6200 0000 08a3 25a8 d15e edc4 4100  lob.....%..^..A.
+00000640: 0000 0900 7300 7400 6100 7400 7300 6300  ....s.t.a.t.s.c.
+00000650: 6500 6e00 646d 6f64 4462 6c6f 6200 0000  e.n.dmodDblob...
+00000660: 08a3 25a8 d15e edc4 4100 0000 0900 7300  ..%..^..A.....s.
+00000670: 7400 6100 7400 7300 6300 6500 6e00 6470  t.a.t.s.c.e.n.dp
+00000680: 6831 5363 6f6d 7000 0000 0000 0000 0000  h1Scomp.........
+00000690: 0000 0900 7300 7400 6100 7400 7300 6300  ....s.t.a.t.s.c.
+000006a0: 6500 6e00 6476 5372 6e6c 6f6e 6700 0000  e.n.dvSrnlong...
+000006b0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 000006c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000006f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000700: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000710: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000720: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `statscend-0.1.7/statscend/bn_logistic_regression.py` & `statscend-0.1.8/statscend/bn_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.7/statscend/datasets.py` & `statscend-0.1.8/statscend/datasets.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.7/statscend/linear_regression.py` & `statscend-0.1.8/statscend/linear_regression.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,13 +61,21 @@
     r_squared_adj = model.rsquared_adj.round(3)
 
     overall_model_fit = [['R', 'R-squared', 'Adj. R-squared', 'F-statistic', 'p-value', 'df-model', 'df-resid'],
                          [r, r_squared, r_squared_adj, fvalue, pvalue, df_model, df_resid]]
     overall_model_fit = pd.DataFrame(
         overall_model_fit[1:], columns=overall_model_fit[0])
 
+    # Table 5 Residuals table
+    fittedvalues = model.fittedvalues
+    residuals = model.resid
+    residuals_table = pd.DataFrame(
+        {'Fitted Values': model.fittedvalues, 'Residuals': model.resid})
+
     results = {}
     results['overall_model_fit'] = overall_model_fit
-    results['summary_table'] = summary_table.round(3)
+    # results['summary_table'] = summary_table.round(3)
     results['coefficients_table'] = coefficients_table.round(3)
     results['diagnostics_table'] = diagnostics_table.round(3)
+    results['residuals_table'] = residuals_table
+
     return results
```

### Comparing `statscend-0.1.7/statscend/mn_logistic_regression.py` & `statscend-0.1.8/statscend/mn_logistic_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.7/statscend/ordinal_regression.py` & `statscend-0.1.8/statscend/ordinal_regression.py`

 * *Files identical despite different names*

### Comparing `statscend-0.1.7/LICENSE` & `statscend-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `statscend-0.1.7/README.md` & `statscend-0.1.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,18 @@
 
 - overall_model_fit: Pandas DataFrame<br/>
   A table that includes the overall model fit statistics such as R, R-squared, Adj. R-squared, F-statistic, p-value, df-model and df-resid.
 
 - coefficients_table : Pandas DataFrame<br/>
   A table of the regression coefficients, including the unstandardized coefficients, their standard errors, the standardized coefficients, and the p-values.
 
-- summary_table : Pandas DataFrame<br/>
-  A summary of the regression results, including the dependent variable, the R-squared value, the adjusted R-squared value, the F-statistic, and the p-value.
-
 - diagnostics_table : Pandas DataFrame<br/>
   A table of diagnostic statistics for the regression, including the Omnibus test, the Durbin-Watson statistic, the Jarque-Bera test, and the condition number.
+- residuals_table : Pandas DataFrame <br/>
+  A table containing the fitted values and residuals of the regression model. The "Fitted Values" column represents the predicted values obtained from the regression model for the corresponding input variables. The "Residuals" column represents the difference between the actual values and the predicted values, indicating the deviation or error in the model's predictions.
 
 #### Examples
 
 Simple Linear Regression
 
 `result = linear_regression(data=penguins, x='bill_depth_mm', y='body_mass_g')`
```

### Comparing `statscend-0.1.7/pyproject.toml` & `statscend-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "statscend"
-version = "0.1.7"
+version = "0.1.8"
 license = {file = "LICENSE"}
 authors = [
   { name="Hashim Puthiyakath", email="hashputhiyakath@gmail.com" },
 ]
 description = "A Python package for performing various statistical analyses"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `statscend-0.1.7/PKG-INFO` & `statscend-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: statscend
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python package for performing various statistical analyses
 Project-URL: Homepage, https://github.com/hashimputhiyakath/statscend
 Project-URL: Bug Tracker, https://github.com/hashimputhiyakath/statscend/issues
 Author-email: Hashim Puthiyakath <hashputhiyakath@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Hashim Puthiyakath
@@ -112,19 +112,18 @@
 
 - overall_model_fit: Pandas DataFrame<br/>
   A table that includes the overall model fit statistics such as R, R-squared, Adj. R-squared, F-statistic, p-value, df-model and df-resid.
 
 - coefficients_table : Pandas DataFrame<br/>
   A table of the regression coefficients, including the unstandardized coefficients, their standard errors, the standardized coefficients, and the p-values.
 
-- summary_table : Pandas DataFrame<br/>
-  A summary of the regression results, including the dependent variable, the R-squared value, the adjusted R-squared value, the F-statistic, and the p-value.
-
 - diagnostics_table : Pandas DataFrame<br/>
   A table of diagnostic statistics for the regression, including the Omnibus test, the Durbin-Watson statistic, the Jarque-Bera test, and the condition number.
+- residuals_table : Pandas DataFrame <br/>
+  A table containing the fitted values and residuals of the regression model. The "Fitted Values" column represents the predicted values obtained from the regression model for the corresponding input variables. The "Residuals" column represents the difference between the actual values and the predicted values, indicating the deviation or error in the model's predictions.
 
 #### Examples
 
 Simple Linear Regression
 
 `result = linear_regression(data=penguins, x='bill_depth_mm', y='body_mass_g')`
```

