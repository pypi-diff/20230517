# Comparing `tmp/tti_dataset_tools-0.1.2.tar.gz` & `tmp/tti_dataset_tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tti_dataset_tools-0.1.2.tar", max compression
+gzip compressed data, was "tti_dataset_tools-0.1.3.tar", max compression
```

## Comparing `tti_dataset_tools-0.1.2.tar` & `tti_dataset_tools-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0     1089 2022-12-12 04:11:06.714273 tti_dataset_tools-0.1.2/LICENSE
--rw-r--r--   0        0        0      965 2023-03-16 05:41:16.761356 tti_dataset_tools-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       82 2022-12-13 21:32:18.296073 tti_dataset_tools-0.1.2/README.md
--rw-r--r--   0        0        0        0 2022-09-05 21:29:28.932413 tti_dataset_tools-0.1.2/src/tti_dataset_tools/__init__.py
--rw-r--r--   0        0        0      787 2023-03-16 05:19:58.029939 tti_dataset_tools-0.1.2/src/tti_dataset_tools/ColMapper.py
--rw-r--r--   0        0        0     6084 2022-12-23 05:18:12.668786 tti_dataset_tools-0.1.2/src/tti_dataset_tools/TrajectoryCleaner.py
--rw-r--r--   0        0        0      671 2023-03-16 05:19:58.032974 tti_dataset_tools-0.1.2/src/tti_dataset_tools/TrajectoryProcessor.py
--rw-r--r--   0        0        0     6472 2023-03-16 05:19:58.036974 tti_dataset_tools-0.1.2/src/tti_dataset_tools/TrajectoryTransformer.py
--rw-r--r--   0        0        0      959 2023-03-16 05:19:58.040974 tti_dataset_tools-0.1.2/src/tti_dataset_tools/TrajectoryVisualizer.py
--rw-r--r--   0        0        0      930 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.2/setup.py
--rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.3/LICENSE
+-rw-r--r--   0        0        0      965 2023-05-12 02:50:22.000000 tti_dataset_tools-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       82 2022-12-16 21:14:46.000000 tti_dataset_tools-0.1.3/README.md
+-rw-r--r--   0        0        0      245 2023-05-04 17:46:00.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/__init__.py
+-rw-r--r--   0        0        0     1012 2023-05-04 17:46:46.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/ColMapper.py
+-rw-r--r--   0        0        0     4371 2023-05-04 17:46:00.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/InfluenceAnalyzer.py
+-rw-r--r--   0        0        0        0 2023-05-04 17:45:58.510000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/models/__init__.py
+-rw-r--r--   0        0        0     6200 2023-05-04 17:46:00.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/models/CrosswalkModel.py
+-rw-r--r--   0        0        0     6615 2023-05-12 02:43:16.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryCleaner.py
+-rw-r--r--   0        0        0     1179 2023-05-04 17:46:06.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryProcessor.py
+-rw-r--r--   0        0        0     9161 2023-05-04 17:47:00.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryTransformer.py
+-rw-r--r--   0        0        0     1350 2023-05-04 17:46:06.000000 tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryVisualizer.py
+-rw-r--r--   0        0        0      958 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.3/setup.py
+-rw-r--r--   0        0        0     1059 1970-01-01 00:00:00.000000 tti_dataset_tools-0.1.3/PKG-INFO
```

### Comparing `tti_dataset_tools-0.1.2/LICENSE` & `tti_dataset_tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tti_dataset_tools-0.1.2/pyproject.toml` & `tti_dataset_tools-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tti-dataset-tools"
-version = "0.1.2"
+version = "0.1.3"
 description = "A set of tools for trajectory dataset transformation, clean-up, and augmentation"
 authors = ["Golam Md Muktadir <muktadir@ucsc.edu>"]
 license = "Mozilla Public License Version 2.0"
 include = [
     "MIT License",
 ]
```

### Comparing `tti_dataset_tools-0.1.2/src/tti_dataset_tools/ColMapper.py` & `tti_dataset_tools-0.1.3/src/tti_dataset_tools/ColMapper.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,15 +8,16 @@
             yVelCol, 
             speedCol,
             fps,
             displacementXCol='displacementX',
             displacementYCol='displacementY',
             localXCol='localX',
             localYCol='localY',
-        
+            verticalDirectionCol='verticalDirection',
+            horizontalDirectionCol='horizontalDirection'
         ):
         
         self.idCol = idCol
         self.xCol = xCol
         self.yCol = yCol
         self.xVelCol = xVelCol
         self.yVelCol = yVelCol
@@ -25,8 +26,11 @@
         
         self.displacementXCol = displacementXCol
         self.displacementYCol = displacementYCol
 
         self.localXCol = localXCol
         self.localYCol = localYCol
 
+        self.verticalDirectionCol = verticalDirectionCol
+        self.horizontalDirectionCol = horizontalDirectionCol
+
         pass
```

### Comparing `tti_dataset_tools-0.1.2/src/tti_dataset_tools/TrajectoryCleaner.py` & `tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryCleaner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 from .ColMapper import ColMapper
 from .TrajectoryProcessor import TrajectoryProcessor
+import logging
 
 class TrajectoryCleaner(TrajectoryProcessor):
 
     def __init__(self,
             colMapper: ColMapper,
             minSpeed,
             maxSpeed,
@@ -35,16 +36,16 @@
         if byIQR:
             Q3 = np.quantile(summary[col], 0.75)
             Q1 = np.quantile(summary[col], 0.25)
             IQR = Q3 - Q1
             lowerBoundary = Q1 - 1.5 * IQR
             higherBoundary = Q3 + 1.5 * IQR
 
-            print("IQR value for column %s is: %s" % (col, IQR))
-            print(f"using range ({lowerBoundary}, {higherBoundary})")
+            logging.info("IQR value for column %s is: %s" % (col, IQR))
+            logging.info(f"getOutliersByCol: using range ({lowerBoundary}, {higherBoundary})")
             
 
         else:
             raise NotImplementedError("Not implemented non IQR yet")
 
 
         criterion = summary[col].map(
@@ -97,15 +98,15 @@
                 self.speedCol,
                 byIQR=byIQR,
                 returnVals=returnVals
             )
             
 
         else:
-            print(f"using range ({self.minSpeed}, {self.maxSpeed})")
+            logging.info(f"getOutliersBySpeed: using range ({self.minSpeed}, {self.maxSpeed})")
             maxVals = tracksDf[[self.idCol, self.speedCol]].groupby([self.idCol]).max()
             criterion = maxVals[self.speedCol].map(
                 lambda val: val < self.minSpeed or val > self.maxSpeed)
 
             outliers = maxVals[criterion]
 
             if returnVals:
@@ -127,16 +128,18 @@
                 byIQR=byIQR,
                 returnVals=returnVals
             )
             
 
         else:
             print(f"using min Y displacement ({self.minYDisplacement})")
-            maxVals = tracksDf[[self.idCol, self.displacementYCol]].groupby([self.idCol]).max()
-            criterion = maxVals[self.displacementYCol].map(
+            col = self.displacementYCol
+
+            maxVals = tracksDf[[self.idCol, col]].groupby([self.idCol]).max()
+            criterion = maxVals[col].map(
                 lambda val: val < self.minYDisplacement)
 
             outliers = maxVals[criterion]
 
             if returnVals:
                 return outliers
             else:
@@ -214,12 +217,29 @@
         criterion = tracksDf[self.idCol].map(
             lambda trackId: trackId not in outlierIds)
         
         return tracksDf[criterion].copy()
 
 
 
+    def cleanByCol(self, 
+            tracksDf:pd.DataFrame, 
+            col:str,
+            byIQR=False,
+        ) -> pd.DataFrame:
+
+        outlierIds = self.getMaxOutliersByCol(
+            tracksDf,
+            col=col,
+            byIQR=byIQR
+        )
+        criterion = tracksDf[self.idCol].map(
+            lambda trackId: trackId not in outlierIds)
+        
+        return tracksDf[criterion].copy()
+    
+    #endregion
```

### Comparing `tti_dataset_tools-0.1.2/src/tti_dataset_tools/TrajectoryTransformer.py` & `tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryTransformer.py`

 * *Files 27% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 
         return trackDf[self.xCol] - originX, trackDf[self.yCol] - originY
         
 
     def translateAllToLocalSource(self,
             tracksDf:pd.DataFrame
         ):
-        """Will group by idCol and translate based on the first row of each track. We cannot make parallel updates for multiple pedestrians as the query would require sql.
+        """Will group by idCol and translate based on the first row of each track. 
+        We cannot make parallel updates for multiple pedestrians as the query would require sql.
+        Assumes all tracks start on a sidewalk
 
         Args:
             trackDf (pd.DataFrame): _description_
             idCol (_type_): track id column. 
             xCol (_type_): _description_
             yCol (_type_): _description_
 
@@ -51,25 +53,36 @@
 
         allTrackIds = tracksDf[self.idCol].unique()
 
         localXSeres = []
         localYSeres = []
 
         for trackId in allTrackIds:
+            # print(f"translating track {trackId}")
             trackDf = tracksDf[tracksDf[self.idCol] == trackId]
             X, Y = self.translateOneToLocalSource(trackDf)
             localXSeres.append(X)
             localYSeres.append(Y)
         
 
         tracksDf[self.localXCol] = pd.concat(localXSeres)
         tracksDf[self.localYCol] = pd.concat(localYSeres)
 
+
+        for trackId in allTrackIds:
+            trackDf = tracksDf[tracksDf[self.idCol] == trackId]
+            self.__validateLocalSource(trackDf)
+
         pass
 
+    def __validateLocalSource(self, trackDf: pd.DataFrame):
+        firstRow = trackDf.iloc[0]
+        if firstRow[self.localXCol] != 0.0 or firstRow[self.localYCol] != 0.0:
+            raise Exception(f"track {firstRow[self.idCol]} has incorrect local source {firstRow[self.localXCol]}, {firstRow[self.localYCol]}")
+        
 
     # derived cols
     
     
     def getTimeDerivativeForOne(self, aTrack: pd.DataFrame, onCol):
         derivativeSeries = aTrack[onCol].rolling(window=2).apply(
             lambda values: (values.iloc[0] - values.iloc[1]) / (1 / self.fps))
@@ -132,42 +145,104 @@
         ):
 
         tracksDf["speed"] = tracksDf.apply(
             lambda row: math.sqrt(row[self.xVelCol] ** 2 + row[self.yVelCol] ** 2),
             axis=1
         )
 
+    def deriveDisplacementsForOne(self, trackDf: pd.DataFrame):
+        xCol = self.xCol
+        yCol = self.yCol
+        firstRow = trackDf.iloc[0]
+        firstX = firstRow[xCol]
+        firstY = firstRow[yCol]
+
+        return (trackDf[self.xCol] - firstX).abs(), (trackDf[self.yCol] - firstY).abs()
 
     def deriveDisplacements(self,
-            tracksDf:pd.DataFrame
+            tracksDf:pd.DataFrame,
+            localAxis=False
         ):
+        """
+        Derives the displacements from the first point of each track
+        """
 
-        # displacement wrt the first row
-        firstRow = tracksDf.iloc[0]
-        firstX = firstRow[self.xCol]
-        firstY = firstRow[self.yCol]
+        xCol = self.xCol
+        yCol = self.yCol
 
-        tracksDf[self.displacementXCol] = tracksDf.apply(
-            lambda row: abs(firstX - row[self.xCol]),
-            axis=1
-        )
+        if localAxis:
+            xCol = self.localXCol
+            yCol = self.localYCol
+
+        # # displacement wrt the first row
+        # firstRow = tracksDf.iloc[0]
+        # firstX = firstRow[xCol]
+        # firstY = firstRow[yCol]
+
+        # tracksDf[self.displacementXCol] = tracksDf.apply(
+        #     lambda row: abs(firstX - row[xCol]),
+        #     axis=1
+        # )
+
+        # tracksDf[self.displacementYCol] = tracksDf.apply(
+        #     lambda row: abs(firstY - row[yCol]),
+        #     axis=1
+        # )
 
-        tracksDf[self.displacementYCol] = tracksDf.apply(
-            lambda row: abs(firstY - row[self.yCol]),
-            axis=1
-        )
+        allTrackIds = tracksDf[self.idCol].unique()
+
+        dXSeres = []
+        dYSeres = []
+
+        for trackId in allTrackIds:
+            trackDf = tracksDf[tracksDf[self.idCol] == trackId]
+            X, Y = self.deriveDisplacementsForOne(trackDf)
+            dXSeres.append(X)
+            dYSeres.append(Y)
+        
+
+        tracksDf[self.displacementXCol] = pd.concat(dXSeres)
+        tracksDf[self.displacementYCol] = pd.concat(dYSeres)
+
+        for trackId in allTrackIds:
+            trackDf = tracksDf[tracksDf[self.idCol] == trackId]
+            self.__validateDisplacement(trackDf)
 
     
+    def deriveDisplacementsInLC(self,
+            tracksDf:pd.DataFrame
+        ):
+        return self.deriveDisplacements(tracksDf, localAxis=True)
+
+
+        
+    def __validateDisplacement(self, trackDf: pd.DataFrame):
+        
+        firstRow = trackDf.iloc[0]
+        if firstRow[self.displacementXCol] != 0.0 or firstRow[self.displacementYCol] != 0.0:
+            raise Exception(f"track {firstRow[self.idCol]} has incorrect local source displacement {firstRow[self.displacementXCol]}, {firstRow[self.displacementYCol]}")
+        
+        
+
     def rotate(self, trackDf: pd.DataFrame) -> Tuple[pd.Series, pd.Series]:
         """rotation is y=-y and x=-x. Does inplace transformation on localX, localY
 
         Args:
             trackDf (pd.DataFrame): A single track
         """
 
+        raise NotImplemented("Not implemented error")
+    
+    def rotate180(self, trackDf: pd.DataFrame) -> Tuple[pd.Series, pd.Series]:
+        """rotation is y=-y and x=-x. Does inplace transformation on localX, localY
+
+        Args:
+            trackDf (pd.DataFrame): A single track
+        """
+
         X = -trackDf[self.localXCol]
         Y = -trackDf[self.localYCol]
 
         return X, Y
 
     def flipAlongY(self, trackDf: pd.DataFrame):
         """Flips along the y axis (negates x coordinates). Does inplace transformation on localX, localY
@@ -186,8 +261,11 @@
         Args:
             trackDf (pd.DataFrame): A single track
 
         """
         # TODO
         pass
 
+    
+    
+
```

### Comparing `tti_dataset_tools-0.1.2/src/tti_dataset_tools/TrajectoryVisualizer.py` & `tti_dataset_tools-0.1.3/src/tti_dataset_tools/TrajectoryVisualizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 from typing import *
 import os
 import matplotlib.pyplot as plt
+import seaborn as sns
 import numpy as np
 
 class TrajectoryVisualizer:
 
     
     def show(self, df: pd.DataFrame, idCol, xCol, yCol, trackIds=None, colorCol=None):
         
@@ -24,7 +25,18 @@
             # plot direction
             lastRow = trackDf.tail(1)
             endPoint = (lastRow[xCol] , lastRow[yCol])
             plt.plot(endPoint[0], endPoint[1], marker='x')
         
         ax.set_aspect('equal', adjustable='box')
         plt.show()
+
+    
+    def showBreakpointVals(self, breakpointXVals:Dict[float, List[float]]):
+        X = []
+        Y = []
+        for y in breakpointXVals:
+            Y.extend([y] * len(breakpointXVals[y]))
+            X.extend(breakpointXVals[y])
+        ax = sns.scatterplot(x=X, y=Y, alpha=0.2)
+        ax.set_aspect('equal', adjustable='box')
+        plt.show()
```

### Comparing `tti_dataset_tools-0.1.2/setup.py` & `tti_dataset_tools-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['tti_dataset_tools']
+['tti_dataset_tools', 'tti_dataset_tools.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.20.3,<2.0.0', 'pandas>=1.5.2,<2.0.0', 'shapely>=1.7.1,<1.8.0']
 
 setup_kwargs = {
     'name': 'tti-dataset-tools',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'A set of tools for trajectory dataset transformation, clean-up, and augmentation',
     'long_description': '# A set of tools for trajectory dataset transformation, clean-up, and augmentation',
     'author': 'Golam Md Muktadir',
     'author_email': 'muktadir@ucsc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/adhocmaster/TTI-dataset-tools',
```

### Comparing `tti_dataset_tools-0.1.2/PKG-INFO` & `tti_dataset_tools-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tti-dataset-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of tools for trajectory dataset transformation, clean-up, and augmentation
 Home-page: https://github.com/adhocmaster/TTI-dataset-tools
 License: Mozilla Public License Version 2.0
 Keywords: Trajectory Dataset,Trajectory Analysis,Trajectory Transformation,Trajectory Augmentation
 Author: Golam Md Muktadir
 Author-email: muktadir@ucsc.edu
 Requires-Python: >=3.8.0,<4.0.0
```

