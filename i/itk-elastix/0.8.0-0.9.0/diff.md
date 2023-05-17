# Comparing `tmp/itk_elastix-0.8.0-cp39-cp39-win_amd64.whl.zip` & `tmp/itk_elastix-0.9.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5922216 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     3783 b- defN 20-Nov-18 22:45 itk/ElastixPython.py
--rw-rw-rw-  2.0 fat 20115968 b- defN 20-Nov-18 22:46 itk/_ElastixPython.pyd
--rw-rw-rw-  2.0 fat    10225 b- defN 20-Nov-18 22:45 itk/elxParameterObjectPython.py
--rw-rw-rw-  2.0 fat    42275 b- defN 20-Nov-18 22:45 itk/itkElastixRegistrationMethodPython.py
--rw-rw-rw-  2.0 fat    32694 b- defN 20-Nov-18 22:45 itk/itkTransformixFilterPython.py
--rw-rw-rw-  2.0 fat     1386 b- defN 20-Nov-18 22:45 itk/Configuration/ElastixConfig.py
--rw-rw-rw-  2.0 fat    11560 b- defN 20-Nov-18 22:46 itk_elastix-0.8.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1645 b- defN 20-Nov-18 22:46 itk_elastix-0.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       98 b- defN 20-Nov-18 22:46 itk_elastix-0.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 20-Nov-18 22:46 itk_elastix-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      936 b- defN 20-Nov-18 22:46 itk_elastix-0.8.0.dist-info/RECORD
-11 files, 20220574 bytes uncompressed, 5920638 bytes compressed:  70.7%
+Zip file size: 5923291 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat     3783 b- defN 20-Dec-22 03:14 itk/ElastixPython.py
+-rw-rw-rw-  2.0 fat 20114432 b- defN 20-Dec-22 03:14 itk/_ElastixPython.pyd
+-rw-rw-rw-  2.0 fat    10225 b- defN 20-Dec-22 03:13 itk/elxParameterObjectPython.py
+-rw-rw-rw-  2.0 fat    42275 b- defN 20-Dec-22 03:14 itk/itkElastixRegistrationMethodPython.py
+-rw-rw-rw-  2.0 fat    32694 b- defN 20-Dec-22 03:14 itk/itkTransformixFilterPython.py
+-rw-rw-rw-  2.0 fat     1386 b- defN 20-Dec-22 03:13 itk/Configuration/ElastixConfig.py
+-rw-rw-rw-  2.0 fat    11560 b- defN 20-Dec-22 03:14 itk_elastix-0.9.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1639 b- defN 20-Dec-22 03:14 itk_elastix-0.9.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       93 b- defN 20-Dec-22 03:14 itk_elastix-0.9.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 20-Dec-22 03:14 itk_elastix-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      936 b- defN 20-Dec-22 03:15 itk_elastix-0.9.0.dist-info/RECORD
+11 files, 20219027 bytes uncompressed, 5921713 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: itk/itkTransformixFilterPython.py
 Comment: 
 
 Filename: itk/Configuration/ElastixConfig.py
 Comment: 
 
-Filename: itk_elastix-0.8.0.dist-info/LICENSE
+Filename: itk_elastix-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: itk_elastix-0.8.0.dist-info/METADATA
+Filename: itk_elastix-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: itk_elastix-0.8.0.dist-info/WHEEL
+Filename: itk_elastix-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: itk_elastix-0.8.0.dist-info/top_level.txt
+Filename: itk_elastix-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: itk_elastix-0.8.0.dist-info/RECORD
+Filename: itk_elastix-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## itk/itkElastixRegistrationMethodPython.py

 * *Ordering differences only*

```diff
@@ -65,39 +65,39 @@
 
 
 class _SwigNonDynamicMeta(type):
     """Meta class to enforce nondynamic attributes (no new attributes) for a class"""
     __setattr__ = _swig_setattr_nondynamic_class_variable(type.__setattr__)
 
 
-import itk.elxParameterObjectPython
-import itk.ITKCommonBasePython
-import itk.pyBasePython
 import itk.itkImageSourcePython
 import itk.itkImagePython
-import itk.itkPointPython
+import itk.itkRGBAPixelPython
 import itk.itkFixedArrayPython
+import itk.pyBasePython
+import itk.itkPointPython
 import itk.vnl_vectorPython
-import itk.vnl_matrixPython
 import itk.stdcomplexPython
+import itk.vnl_matrixPython
 import itk.itkVectorPython
 import itk.vnl_vector_refPython
-import itk.itkRGBAPixelPython
-import itk.itkRGBPixelPython
-import itk.itkSizePython
-import itk.itkCovariantVectorPython
-import itk.itkOffsetPython
-import itk.itkIndexPython
 import itk.itkMatrixPython
 import itk.vnl_matrix_fixedPython
+import itk.itkCovariantVectorPython
 import itk.itkSymmetricSecondRankTensorPython
+import itk.ITKCommonBasePython
 import itk.itkImageRegionPython
+import itk.itkSizePython
+import itk.itkIndexPython
+import itk.itkOffsetPython
+import itk.itkRGBPixelPython
+import itk.itkImageSourceCommonPython
 import itk.itkVectorImagePython
 import itk.itkVariableLengthVectorPython
-import itk.itkImageSourceCommonPython
+import itk.elxParameterObjectPython
 
 def itkElastixRegistrationMethodID2ID2_New():
     return itkElastixRegistrationMethodID2ID2.New()
 
 class itkElastixRegistrationMethodID2ID2(itk.itkImageSourcePython.itkImageSourceID2):
     r"""Proxy of C++ itkElastixRegistrationMethodID2ID2 class."""
```

## itk/itkTransformixFilterPython.py

 * *Ordering differences only*

```diff
@@ -65,39 +65,39 @@
 
 
 class _SwigNonDynamicMeta(type):
     """Meta class to enforce nondynamic attributes (no new attributes) for a class"""
     __setattr__ = _swig_setattr_nondynamic_class_variable(type.__setattr__)
 
 
-import itk.elxParameterObjectPython
-import itk.ITKCommonBasePython
-import itk.pyBasePython
 import itk.itkImageSourcePython
 import itk.itkImagePython
-import itk.itkPointPython
+import itk.itkRGBAPixelPython
 import itk.itkFixedArrayPython
+import itk.pyBasePython
+import itk.itkPointPython
 import itk.vnl_vectorPython
-import itk.vnl_matrixPython
 import itk.stdcomplexPython
+import itk.vnl_matrixPython
 import itk.itkVectorPython
 import itk.vnl_vector_refPython
-import itk.itkRGBAPixelPython
-import itk.itkRGBPixelPython
-import itk.itkSizePython
-import itk.itkCovariantVectorPython
-import itk.itkOffsetPython
-import itk.itkIndexPython
 import itk.itkMatrixPython
 import itk.vnl_matrix_fixedPython
+import itk.itkCovariantVectorPython
 import itk.itkSymmetricSecondRankTensorPython
+import itk.ITKCommonBasePython
 import itk.itkImageRegionPython
+import itk.itkSizePython
+import itk.itkIndexPython
+import itk.itkOffsetPython
+import itk.itkRGBPixelPython
+import itk.itkImageSourceCommonPython
 import itk.itkVectorImagePython
 import itk.itkVariableLengthVectorPython
-import itk.itkImageSourceCommonPython
+import itk.elxParameterObjectPython
 
 def itkTransformixFilterID2_New():
     return itkTransformixFilterID2.New()
 
 class itkTransformixFilterID2(itk.itkImageSourcePython.itkImageSourceID2):
     r"""Proxy of C++ itkTransformixFilterID2 class."""
```

## Comparing `itk_elastix-0.8.0.dist-info/LICENSE` & `itk_elastix-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `itk_elastix-0.8.0.dist-info/METADATA` & `itk_elastix-0.9.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: itk-elastix
-Version: 0.8.0
+Version: 0.9.0
 Summary: Provides an ITK Python interface to elastix, a toolbox for rigid and nonrigid registration of images
 Home-page: https://itk.org/
 Author: Insight Software Consortium
 Author-email: itk+community@discourse.itk.org
 License: Apache
 Download-URL: https://github.com/InsightSoftwareConsortium/ITKElastix
 Keywords: ITK InsightToolkit
@@ -22,12 +22,12 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: Android
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Dist: itk (>=5.1.1.post1)
+Requires-Dist: itk (>=5.1.2)
 
 elastix is open source software, based on the well-known Insight Segmentation and Registration Toolkit (ITK). The software consists of a collection of algorithms that are commonly used to solve (medical) image registration problems. The modular design of elastix allows the user to quickly configure, test, and compare different registration methods for a specific application.
```

