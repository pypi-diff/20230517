# Comparing `tmp/arraykit-0.3.4.tar.gz` & `tmp/arraykit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arraykit-0.3.4.tar", last modified: Tue May  2 17:47:36 2023, max compression
+gzip compressed data, was "arraykit-0.4.0.tar", last modified: Tue May 16 21:35:42 2023, max compression
```

## Comparing `arraykit-0.3.4.tar` & `arraykit-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 17:47:36.086742 arraykit-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-02 17:47:29.000000 arraykit-0.3.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-02 17:47:29.000000 arraykit-0.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-02 17:47:36.086742 arraykit-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-05-02 17:47:29.000000 arraykit-0.3.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 17:47:36.082742 arraykit-0.3.4/arraykit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-02 17:47:35.000000 arraykit-0.3.4/arraykit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-02 17:47:36.000000 arraykit-0.3.4/arraykit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-02 17:47:35.000000 arraykit-0.3.4/arraykit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-02 17:47:35.000000 arraykit-0.3.4/arraykit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-02 17:47:35.000000 arraykit-0.3.4/arraykit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-02 17:47:36.086742 arraykit-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-05-02 17:47:29.000000 arraykit-0.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 17:47:36.082742 arraykit-0.3.4/src/
--rw-r--r--   0 runner    (1001) docker     (122)     1264 2023-05-02 17:47:29.000000 arraykit-0.3.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   145666 2023-05-02 17:47:29.000000 arraykit-0.3.4/src/_arraykit.c
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-02 17:47:36.086742 arraykit-0.3.4/test/
--rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_array_go.py
--rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_delimited_to_arrays.py
--rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_delimited_to_arrays_integration.py
--rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_delimited_to_arrays_property.py
--rw-r--r--   0 runner    (1001) docker     (122)     1806 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_pyi.py
--rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_split_after_count.py
--rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_type_discovery.py
--rw-r--r--   0 runner    (1001) docker     (122)    26140 2023-05-02 17:47:29.000000 arraykit-0.3.4/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:35:42.821501 arraykit-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-05-16 21:35:38.000000 arraykit-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-16 21:35:38.000000 arraykit-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-16 21:35:42.821501 arraykit-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3731 2023-05-16 21:35:38.000000 arraykit-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:35:42.817501 arraykit-0.4.0/arraykit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1178 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      495 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-05-16 21:35:42.000000 arraykit-0.4.0/arraykit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-16 21:35:42.821501 arraykit-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2698 2023-05-16 21:35:38.000000 arraykit-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:35:42.817501 arraykit-0.4.0/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-05-16 21:35:38.000000 arraykit-0.4.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   174826 2023-05-16 21:35:38.000000 arraykit-0.4.0/src/_arraykit.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-16 21:35:42.821501 arraykit-0.4.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     3129 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_array_go.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16629 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_block_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49054 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_delimited_to_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1974 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_delimited_to_arrays_integration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_delimited_to_arrays_property.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1957 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_pyi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4935 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_split_after_count.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28073 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_type_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26140 2023-05-16 21:35:38.000000 arraykit-0.4.0/test/test_util.py
```

### Comparing `arraykit-0.3.4/LICENSE.txt` & `arraykit-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.4/PKG-INFO` & `arraykit-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.3.4
+Version: 0.4.0
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.3.4/README.rst` & `arraykit-0.4.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -34,14 +34,28 @@
 
 
 
 What is New in ArrayKit
 -------------------------
 
 
+0.4.0
+............
+
+Added ``BlockIndex``, a tool to be used by ``TypeBlocks`` for mapping realized column positions to arrays.
+
+Corrected potential issue in ``AK_CPL_resize_buffer`` that could segfault for very large offsets.
+
+
+0.3.4
+............
+
+Simplified implementation of ``NaTType`` identification in ``isna_element()``.
+
+
 0.3.3
 ............
 
 Corrected potential memory leak in ``isna_element()``.
 
 
 0.3.2
```

### Comparing `arraykit-0.3.4/arraykit.egg-info/PKG-INFO` & `arraykit-0.4.0/arraykit.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: arraykit
-Version: 0.3.4
+Version: 0.4.0
 Summary: Array utilities for StaticFrame
 Home-page: https://github.com/static-frame/arraykit
 Author: Christopher Ariza, Brandt Bucher, Charles Burkland
 License: MIT
 Description: The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
         
         Code: https://github.com/static-frame/arraykit
```

### Comparing `arraykit-0.3.4/setup.py` & `arraykit-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 import os
 import typing as tp
 from setuptools import Extension  # type: ignore
 from setuptools import setup
 from pathlib import Path
 
-AK_VERSION = '0.3.4'
+AK_VERSION = '0.4.0'
 
 def get_long_description() -> str:
     return '''The ArrayKit library provides utilities for creating and transforming NumPy arrays, implementing performance-critical StaticFrame operations as Python C extensions.
 
 Code: https://github.com/static-frame/arraykit
 
 Packages: https://pypi.org/project/arraykit
```

### Comparing `arraykit-0.3.4/src/__init__.py` & `arraykit-0.4.0/src/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # pylint: disable=W0611
 # pylint: disable=E0401
 # pylint: disable=C0414
 
 from ._arraykit import __version__
 from ._arraykit import ArrayGO as ArrayGO
+from ._arraykit import BlockIndex as BlockIndex
+from ._arraykit import ErrorInitBlocks as ErrorInitBlocks
+
 from ._arraykit import immutable_filter as immutable_filter
 from ._arraykit import mloc as mloc
 from ._arraykit import name_filter as name_filter
 from ._arraykit import shape_filter as shape_filter
 from ._arraykit import column_2d_filter as column_2d_filter
 from ._arraykit import column_1d_filter as column_1d_filter
 from ._arraykit import row_1d_filter as row_1d_filter
```

### Comparing `arraykit-0.3.4/src/_arraykit.c` & `arraykit-0.4.0/src/_arraykit.c`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+
 # include "Python.h"
 # include "structmember.h"
 # include "stdbool.h"
 # include "limits.h"
-// # include "stdlib.h"
 
 # define PY_ARRAY_UNIQUE_SYMBOL AK_ARRAY_API
 # define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
 
 # include "numpy/arrayobject.h"
 # include "numpy/arrayscalars.h"
 # include "numpy/halffloat.h"
@@ -14,15 +14,15 @@
 //------------------------------------------------------------------------------
 // Macros
 
 //------------------------------------------------------------------------------
 // Given a PyObject, raise if not an array.
 # define AK_CHECK_NUMPY_ARRAY(O)                                              \
     if (!PyArray_Check(O)) {                                                  \
-        return PyErr_Format(PyExc_TypeError, "expected numpy array (got %s)", \
+        return PyErr_Format(PyExc_TypeError, "Expected NumPy array (got %s)", \
                             Py_TYPE(O)->tp_name);                             \
     }
 
 // Given a PyObject, raise if not an array or is not one or two dimensional.
 # define AK_CHECK_NUMPY_ARRAY_1D_2D(O)                    \
     do {                                                  \
         AK_CHECK_NUMPY_ARRAY(O)                           \
@@ -1226,15 +1226,15 @@
 
     AK_TypeParser *type_parser;
     bool type_parser_field_active;
     bool type_parser_line_active;
 
 } AK_CodePointLine;
 
-// on error return NULL
+// Returns NULL on error.
 AK_CodePointLine*
 AK_CPL_New(bool type_parse, Py_UCS4 tsep, Py_UCS4 decc)
 {
     AK_CodePointLine *cpl = (AK_CodePointLine*)PyMem_Malloc(sizeof(AK_CodePointLine));
     if (cpl == NULL) return (AK_CodePointLine*)PyErr_NoMemory();
 
     cpl->buffer_count = 0;
@@ -1288,38 +1288,43 @@
 }
 
 //------------------------------------------------------------------------------
 // CodePointLine: Mutation
 
 // Returns 0 on success, -1 on failure.
 static inline int
-AK_CPL_resize_buffer(AK_CodePointLine* cpl, Py_ssize_t count)
-{
-    if (AK_UNLIKELY((cpl->buffer_count + count) >= cpl->buffer_capacity)) {
-        // realloc
-        cpl->buffer_capacity *= 2; // needs to be max of this or element_length
+AK_CPL_resize_buffer(AK_CodePointLine* cpl, Py_ssize_t increment) {
+    Py_ssize_t target = cpl->buffer_count + increment;
+    if (AK_UNLIKELY(target >= cpl->buffer_capacity)) {
+        while (cpl->buffer_capacity < target) {
+            cpl->buffer_capacity <<= 1;
+        }
         cpl->buffer = PyMem_Realloc(cpl->buffer,
                 sizeof(Py_UCS4) * cpl->buffer_capacity);
-        if (cpl->buffer == NULL) return -1;
-
+        if (cpl->buffer == NULL) {
+            return -1;
+        }
         cpl->buffer_current_ptr = cpl->buffer + cpl->buffer_count;
     }
     return 0;
 }
 
+
+// NOTE: we only add one offset at time, so this does not need to take an increment argument.
 static inline int
-AK_CPL_resize_offsets(AK_CodePointLine* cpl)
-{
+AK_CPL_resize_offsets(AK_CodePointLine* cpl) {
     // increment by at most one, so only need to check if equal
     if (AK_UNLIKELY(cpl->offsets_count == cpl->offsets_capacity)) {
         // realloc
-        cpl->offsets_capacity *= 2;
+        cpl->offsets_capacity <<= 1;
         cpl->offsets = PyMem_Realloc(cpl->offsets,
                 sizeof(Py_ssize_t) * cpl->offsets_capacity);
-        if (cpl->offsets == NULL) return -1;
+        if (cpl->offsets == NULL) {
+            return -1;
+        }
     }
     return 0;
 }
 
 // Given a PyUnicode PyObject representing a complete field, load the string content into the CPL. Used for iterable_str_to_array_1d. Returns 0 on success, -1 on error.
 static inline int
 AK_CPL_AppendField(AK_CodePointLine* cpl, PyObject* field)
@@ -1327,15 +1332,17 @@
     if (!PyUnicode_Check(field)) { // NOTE: this permits subclasses, consider
         PyErr_SetString(PyExc_TypeError, "elements must be strings");
         return -1;
     }
     Py_ssize_t element_length = PyUnicode_GET_LENGTH(field);
 
     // if we cannot fit field length, resize
-    if (AK_CPL_resize_buffer(cpl, element_length)) return -1;
+    if (AK_CPL_resize_buffer(cpl, element_length)) {
+        return -1;
+    }
 
     // we write the field directly into the CPL buffer
     if(PyUnicode_AsUCS4(field,
             cpl->buffer_current_ptr,
             cpl->buffer + cpl->buffer_capacity - cpl->buffer_current_ptr,
             0) == NULL) { // last zero means do not copy null
         return -1;
@@ -3228,37 +3235,35 @@
     return PyLong_FromVoidPtr(PyArray_DATA((PyArrayObject *)a));
 }
 
 //------------------------------------------------------------------------------
 // filter functions
 
 static PyObject *
-immutable_filter(PyObject *Py_UNUSED(m), PyObject *a)
-{
+immutable_filter(PyObject *Py_UNUSED(m), PyObject *a) {
     AK_CHECK_NUMPY_ARRAY(a);
     return (PyObject *)AK_ImmutableFilter((PyArrayObject *)a);
 }
 
 
 static PyObject *
-name_filter(PyObject *Py_UNUSED(m), PyObject *n)
-{
+name_filter(PyObject *Py_UNUSED(m), PyObject *n) {
     if (AK_UNLIKELY(PyObject_Hash(n) == -1)) {
-        return PyErr_Format(PyExc_TypeError, "unhashable name (type '%s')",
-                            Py_TYPE(n)->tp_name);
+        return PyErr_Format(PyExc_TypeError,
+                "unhashable name (type '%s')",
+                Py_TYPE(n)->tp_name);
     }
     Py_INCREF(n);
     return n;
 }
 
 // Represent a 1D array as a 2D array with length as rows of a single-column array.
 // https://stackoverflow.com/questions/56182259/how-does-one-acces-numpy-multidimensionnal-array-in-c-extensions
 static PyObject *
-shape_filter(PyObject *Py_UNUSED(m), PyObject *a)
-{
+shape_filter(PyObject *Py_UNUSED(m), PyObject *a) {
     AK_CHECK_NUMPY_ARRAY_1D_2D(a);
     PyArrayObject *array = (PyArrayObject *)a;
 
     npy_intp size0 = PyArray_DIM(array, 0);
     // If 1D array, set size for axis 1 at 1, else use 2D array to get the size of axis 1
     npy_intp size1 = PyArray_NDIM(array) == 1 ? 1 : PyArray_DIM(array, 1);
     return Py_BuildValue("ii", size0, size1);
@@ -3354,25 +3359,25 @@
 //------------------------------------------------------------------------------
 // type resolution
 
 static PyObject *
 resolve_dtype(PyObject *Py_UNUSED(m), PyObject *args)
 {
     PyArray_Descr *d1, *d2;
-    if (!PyArg_ParseTuple(args, "O!O!:resolve_dtype",
-            &PyArrayDescr_Type, &d1, &PyArrayDescr_Type, &d2))
-    {
+    if (!PyArg_ParseTuple(args,
+            "O!O!:resolve_dtype",
+            &PyArrayDescr_Type, &d1,
+            &PyArrayDescr_Type, &d2)) {
         return NULL;
     }
     return (PyObject *)AK_ResolveDTypes(d1, d2);
 }
 
 static PyObject *
-resolve_dtype_iter(PyObject *Py_UNUSED(m), PyObject *arg)
-{
+resolve_dtype_iter(PyObject *Py_UNUSED(m), PyObject *arg) {
     return (PyObject *)AK_ResolveDTypeIter(arg);
 }
 
 //------------------------------------------------------------------------------
 // general utility
 
 static char *first_true_1d_kwarg_names[] = {
@@ -4101,14 +4106,959 @@
     fail:
         Py_DECREF(element_locations);
         Py_DECREF(order_found);
         return NULL;
 }
 
 //------------------------------------------------------------------------------
+// BlockIndex
+//------------------------------------------------------------------------------
+
+static PyTypeObject BlockIndexType;
+static PyObject *ErrorInitBlocks;
+
+// NOTE: we use platform size types here, which are appropriate for the values, but might pose issues if trying to pass pickles between 32 and 64 bit machines.
+typedef struct BlockIndexRecord {
+    Py_ssize_t block; // signed
+    Py_ssize_t column;
+} BlockIndexRecord;
+
+typedef struct BlockIndexObject {
+    PyObject_VAR_HEAD
+    Py_ssize_t block_count;
+    Py_ssize_t row_count;
+    Py_ssize_t bir_count;
+    Py_ssize_t bir_capacity;
+    BlockIndexRecord* bir;
+    PyArray_Descr* dtype;
+} BlockIndexObject;
+
+
+// Returns a new reference to tuple. Returns NULL on error.
+static PyObject*
+AK_BI_item(BlockIndexObject* self, Py_ssize_t i) {
+    if (!((size_t)i < (size_t)self->bir_count)) {
+        PyErr_SetString(PyExc_IndexError, "index out of range");
+        return NULL;
+    }
+    BlockIndexRecord* biri = &self->bir[i];
+    return Py_BuildValue("nn", biri->block, biri->column); // maybe NULL
+}
+
+//------------------------------------------------------------------------------
+// BI Iterator
+static PyTypeObject BIIterType;
+
+typedef struct BIIterObject {
+    PyObject_VAR_HEAD
+    BlockIndexObject *bi;
+    int8_t reversed;
+    Py_ssize_t pos; // current index state, mutated in-place
+} BIIterObject;
+
+static PyObject *
+BIIter_new(BlockIndexObject *bi, int8_t reversed) {
+    BIIterObject *bii = PyObject_New(BIIterObject, &BIIterType);
+    if (!bii) {
+        return NULL;
+    }
+    Py_INCREF(bi);
+    bii->bi = bi;
+    bii->reversed = reversed;
+    bii->pos = 0;
+    return (PyObject *)bii;
+}
+
+static void
+BIIter_dealloc(BIIterObject *self) {
+    Py_DECREF(self->bi);
+    Py_TYPE(self)->tp_free((PyObject *)self);
+}
+
+static BIIterObject *
+BIIter_iter(BIIterObject *self) {
+    Py_INCREF(self);
+    return self;
+}
+
+static PyObject *
+BIIter_iternext(BIIterObject *self) {
+    Py_ssize_t i;
+    if (self->reversed) {
+        i = self->bi->bir_count - ++self->pos;
+        if (i < 0) {
+            return NULL;
+        }
+    }
+    else {
+        i = self->pos++;
+    }
+    if (self->bi->bir_count <= i) {
+        return NULL;
+    }
+    return AK_BI_item(self->bi, i); // return new ref
+}
+
+static PyObject *
+BIIter_reversed(BIIterObject *self) {
+    return BIIter_new(self->bi, !self->reversed);
+}
+
+static PyObject *
+BIIter_length_hint(BIIterObject *self) {
+    // this works for reversed as we use self->pos to subtract from length
+    Py_ssize_t len = Py_MAX(0, self->bi->bir_count - self->pos);
+    return PyLong_FromSsize_t(len);
+}
+
+static PyMethodDef BIIter_methods[] = {
+    {"__length_hint__", (PyCFunction)BIIter_length_hint, METH_NOARGS, NULL},
+    {"__reversed__", (PyCFunction)BIIter_reversed, METH_NOARGS, NULL},
+    {NULL},
+};
+
+static PyTypeObject BIIterType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_basicsize = sizeof(BIIterObject),
+    .tp_dealloc = (destructor) BIIter_dealloc,
+    .tp_iter = (getiterfunc) BIIter_iter,
+    .tp_iternext = (iternextfunc) BIIter_iternext,
+    .tp_methods = BIIter_methods,
+    .tp_name = "arraykit.BlockIndexIterator",
+};
+
+
+//------------------------------------------------------------------------------
+// BI Iterator sequence selection
+static PyTypeObject BIIterSeqType;
+static PyTypeObject BIIterSliceType;
+static PyTypeObject BIIterBooleanType;
+
+
+typedef enum BIIterSelectorKind {
+    BIIS_SEQUENCE, // BIIterSeqType
+    BIIS_SLICE,
+    BIIS_BOOLEAN, // BIIterBooleanType
+    BIIS_UNKNOWN
+} BIIterSelectorKind;
+
+
+static PyObject *
+BIIterSelector_new(BlockIndexObject *bi,
+        PyObject* selector,
+        int8_t reversed,
+        BIIterSelectorKind kind
+        );
+
+typedef struct BIIterSeqObject {
+    PyObject_VAR_HEAD
+    BlockIndexObject *bi;
+    int8_t reversed;
+    PyObject* selector;
+    Py_ssize_t pos; // current pos in sequence, mutated in-place
+    Py_ssize_t len;
+    int8_t is_array;
+} BIIterSeqObject;
+
+static void
+BIIterSeq_dealloc(BIIterSeqObject *self) {
+    Py_DECREF(self->bi);
+    Py_DECREF(self->selector);
+    Py_TYPE(self)->tp_free((PyObject *)self);
+}
+
+static BIIterSeqObject *
+BIIterSeq_iter(BIIterSeqObject *self) {
+    Py_INCREF(self);
+    return self;
+}
+
+static PyObject *
+BIIterSeq_iternext(BIIterSeqObject *self) {
+    Py_ssize_t i;
+    if (self->reversed) {
+        i = self->len - ++self->pos;
+        if (i < 0) {
+            return NULL;
+        }
+    }
+    else {
+        i = self->pos++;
+    }
+    if (self->len <= i) {
+        return NULL;
+    }
+    // use i to get index from selector
+    Py_ssize_t t = 0;
+    if (self->is_array) {
+        PyArrayObject *a = (PyArrayObject *)self->selector;
+        switch (PyArray_TYPE(a)) { // type of passed in array
+            case NPY_INT64:
+                t = *(npy_int64*)PyArray_GETPTR1(a, i);
+                break;
+            case NPY_INT32:
+                t = *(npy_int32*)PyArray_GETPTR1(a, i);
+                break;
+            case NPY_INT16:
+                t = *(npy_int16*)PyArray_GETPTR1(a, i);
+                break;
+            case NPY_INT8:
+                t = *(npy_int8*)PyArray_GETPTR1(a, i);
+                break;
+            case NPY_UINT64:
+                t = *(npy_uint64*)PyArray_GETPTR1(a, i);
+                break;
+            case NPY_UINT32:
+                t = *(npy_uint32*)PyArray_GETPTR1(a, i);
+                break;
+            case NPY_UINT16:
+                t = *(npy_uint16*)PyArray_GETPTR1(a, i);
+                break;
+            case NPY_UINT8:
+                t = *(npy_uint8*)PyArray_GETPTR1(a, i);
+                break;
+        }
+    }
+    else { // is a list
+        PyObject* o = PyList_GET_ITEM(self->selector, i); // borrow
+        if (PyNumber_Check(o)) { // handles scalars
+            t = PyNumber_AsSsize_t(o, NULL);
+        }
+        else {
+            PyErr_SetString(PyExc_TypeError, "element type not suitable for indexing");
+            return NULL;
+        }
+    }
+    return AK_BI_item(self->bi, t); // return new ref
+}
+
+static PyObject *
+BIIterSeq_reversed(BIIterSeqObject *self) {
+    return BIIterSelector_new(self->bi, self->selector, !self->reversed, BIIS_SEQUENCE);
+}
+
+static PyObject *
+BIIterSeq_length_hint(BIIterSeqObject *self) {
+    // this works for reversed as we use self-> index to subtract from length
+    Py_ssize_t len = Py_MAX(0, self->len - self->pos);
+    return PyLong_FromSsize_t(len);
+}
+
+static PyMethodDef BIiterSeq_methods[] = {
+    {"__length_hint__", (PyCFunction)BIIterSeq_length_hint, METH_NOARGS, NULL},
+    {"__reversed__", (PyCFunction)BIIterSeq_reversed, METH_NOARGS, NULL},
+    {NULL},
+};
+
+static PyTypeObject BIIterSeqType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_basicsize = sizeof(BIIterSeqObject),
+    .tp_dealloc = (destructor) BIIterSeq_dealloc,
+    .tp_iter = (getiterfunc) BIIterSeq_iter,
+    .tp_iternext = (iternextfunc) BIIterSeq_iternext,
+    .tp_methods = BIiterSeq_methods,
+    .tp_name = "arraykit.BlockIndexIteratorSequence",
+};
+
+//------------------------------------------------------------------------------
+// BI Iterator slice selection
+
+typedef struct BIIterSliceObject {
+    PyObject_VAR_HEAD
+    BlockIndexObject *bi;
+    int8_t reversed;
+    PyObject* selector; // slice
+    Py_ssize_t count; // count of , mutated in-place
+    // these are the normalized values truncated to the span of the bir_count; len is the realized length after extraction; step is always set to 1 if missing; len is 0 if no realized values
+    Py_ssize_t pos;
+    Py_ssize_t step;
+    Py_ssize_t len;
+} BIIterSliceObject;
+
+static void
+BIIterSlice_dealloc(BIIterSliceObject *self) {
+    Py_DECREF(self->bi);
+    Py_DECREF(self->selector);
+    Py_TYPE(self)->tp_free((PyObject *)self);
+}
+
+static BIIterSliceObject *
+BIIterSlice_iter(BIIterSliceObject *self) {
+    Py_INCREF(self);
+    return self;
+}
+
+static PyObject *
+BIIterSlice_iternext(BIIterSliceObject *self) {
+    if (self->len == 0 || self->count >= self->len) {
+        return NULL;
+    }
+    Py_ssize_t i = self->pos;
+    self->pos += self->step;
+    self->count++; // by counting index we we do not need to compare to stop
+    return AK_BI_item(self->bi, i); // return new ref
+}
+
+static PyObject *
+BIIterSlice_reversed(BIIterSliceObject *self) {
+    return BIIterSelector_new(self->bi, self->selector, !self->reversed, BIIS_SLICE);
+}
+
+static PyObject *
+BIIterSlice_length_hint(BIIterSliceObject *self) {
+    // this works for reversed as we use self-> index to subtract from length
+    Py_ssize_t len = Py_MAX(0, self->len - self->count);
+    return PyLong_FromSsize_t(len);
+}
+
+static PyMethodDef BIiterSlice_methods[] = {
+    {"__length_hint__", (PyCFunction)BIIterSlice_length_hint, METH_NOARGS, NULL},
+    {"__reversed__", (PyCFunction)BIIterSlice_reversed, METH_NOARGS, NULL},
+    {NULL},
+};
+
+static PyTypeObject BIIterSliceType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_basicsize = sizeof(BIIterSliceObject),
+    .tp_dealloc = (destructor) BIIterSlice_dealloc,
+    .tp_iter = (getiterfunc) BIIterSlice_iter,
+    .tp_iternext = (iternextfunc) BIIterSlice_iternext,
+    .tp_methods = BIiterSlice_methods,
+    .tp_name = "arraykit.BlockIndexIteratorSlice",
+};
+
+//------------------------------------------------------------------------------
+// BI Iterator Boolean array selection
+
+typedef struct BIIterBooleanObject {
+    PyObject_VAR_HEAD
+    BlockIndexObject *bi;
+    int8_t reversed;
+    PyObject* selector;
+    Py_ssize_t pos; // current index, mutated in-place
+    Py_ssize_t len;
+} BIIterBooleanObject;
+
+static void
+BIIterBoolean_dealloc(BIIterBooleanObject *self) {
+    Py_DECREF(self->bi);
+    Py_DECREF(self->selector);
+    Py_TYPE(self)->tp_free((PyObject *)self);
+}
+
+static BIIterBooleanObject *
+BIIterBoolean_iter(BIIterBooleanObject *self) {
+    Py_INCREF(self);
+    return self;
+}
+
+static PyObject *
+BIIterBoolean_iternext(BIIterBooleanObject *self) {
+    npy_bool v = 0;
+    Py_ssize_t i = -1;
+    PyArrayObject* a = (PyArrayObject*) self->selector;
+
+    if (!self->reversed) {
+        while (self->pos < self->len) {
+            v = *(npy_bool*)PyArray_GETPTR1(a, self->pos);
+            if (v) {
+                i = self->pos;
+                self->pos++;
+                break;
+            }
+            self->pos++;
+        }
+    }
+    else { // reversed
+        while (self->pos >= 0) {
+            v = *(npy_bool*)PyArray_GETPTR1(a, self->pos);
+            if (v) {
+                i = self->pos;
+                self->pos--;
+                break;
+            }
+            self->pos--;
+        }
+    }
+    if (i != -1) {
+        return AK_BI_item(self->bi, i); // return new ref
+    }
+    return NULL; // no True remain
+}
+
+static PyObject *
+BIIterBoolean_reversed(BIIterBooleanObject *self) {
+    return BIIterSelector_new(self->bi, self->selector, !self->reversed, BIIS_BOOLEAN);
+}
+
+// NOTE: no length hint given as we would have to traverse whole array and count True... not sure it is worht it.
+static PyMethodDef BIiterBoolean_methods[] = {
+    // {"__length_hint__", (PyCFunction)BIIterBoolean_length_hint, METH_NOARGS, NULL},
+    {"__reversed__", (PyCFunction)BIIterBoolean_reversed, METH_NOARGS, NULL},
+    {NULL},
+};
+
+static PyTypeObject BIIterBooleanType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    .tp_basicsize = sizeof(BIIterBooleanObject),
+    .tp_dealloc = (destructor) BIIterBoolean_dealloc,
+    .tp_iter = (getiterfunc) BIIterBoolean_iter,
+    .tp_iternext = (iternextfunc) BIIterBoolean_iternext,
+    .tp_methods = BIiterBoolean_methods,
+    .tp_name = "arraykit.BlockIndexIteratorBoolean",
+};
+
+
+//------------------------------------------------------------------------------
+
+// NOTE: this constructor returns one of three different PyObject types. We do this to consolidate error reporting and type checks.
+static PyObject *
+BIIterSelector_new(BlockIndexObject *bi,
+        PyObject* selector,
+        int8_t reversed,
+        BIIterSelectorKind kind
+        ) {
+
+    int8_t is_array = 0;
+    Py_ssize_t len = -1;
+    Py_ssize_t pos = 0;
+    Py_ssize_t stop = 0;
+    Py_ssize_t step = 0;
+
+    if (PyArray_Check(selector)) {
+        if (kind == BIIS_SLICE) {
+            PyErr_SetString(PyExc_TypeError, "Arrays cannot be used as selectors for slice iterators");
+            return NULL;
+        }
+        is_array = 1;
+        PyArrayObject *a = (PyArrayObject *)selector;
+        if (PyArray_NDIM(a) != 1) {
+            PyErr_SetString(PyExc_TypeError, "Arrays must be 1-dimensional");
+            return NULL;
+        }
+        len = PyArray_SIZE(a);
+        char k = PyArray_DESCR(a)->kind;
+        if (kind == BIIS_UNKNOWN) {
+            if (k == 'i' || k == 'u') {
+                kind = BIIS_SEQUENCE;
+            }
+            else if (k == 'b') {
+                kind = BIIS_BOOLEAN;
+            }
+            else {
+                PyErr_SetString(PyExc_TypeError, "Arrays kind not supported");
+                return NULL;
+            }
+        }
+        else if (kind == BIIS_SEQUENCE && k != 'i' && k != 'u') {
+            PyErr_SetString(PyExc_TypeError, "Arrays must integer kind");
+            return NULL;
+        }
+        else if (kind == BIIS_BOOLEAN && k != 'b') {
+            PyErr_SetString(PyExc_TypeError, "Arrays must Boolean kind");
+            return NULL;
+        }
+        if (kind == BIIS_BOOLEAN && len != bi->bir_count) {
+            PyErr_SetString(PyExc_TypeError, "Boolean arrays must match BlockIndex size");
+            return NULL;
+        }
+    }
+    else if (PySlice_Check(selector)) {
+        if (kind == BIIS_UNKNOWN) {
+            kind = BIIS_SLICE;
+        }
+        else if (kind != BIIS_SLICE) {
+            PyErr_SetString(PyExc_TypeError, "Slices cannot be used as selectors for this type of iterator");
+            return NULL;
+        }
+        if (PySlice_Unpack(selector, &pos, &stop, &step)) {
+            return NULL;
+        }
+        len = PySlice_AdjustIndices(bi->bir_count, &pos, &stop, step);
+        if (reversed) {
+            pos += (step * (len - 1));
+            step *= -1;
+        }
+        // AK_DEBUG_MSG_OBJ("resolved slice", Py_BuildValue("nnnn", pos, stop, step, len));
+    }
+    else if (PyList_CheckExact(selector)) {
+        if (kind == BIIS_UNKNOWN) {
+            kind = BIIS_SEQUENCE;
+        }
+        else if (kind != BIIS_SEQUENCE) {
+            PyErr_SetString(PyExc_TypeError, "Lists cannot be used as for non-sequence iterators");
+            return NULL;
+        }
+        len = PyList_GET_SIZE(selector);
+    }
+    else {
+        PyErr_SetString(PyExc_TypeError, "Input type not supported");
+        return NULL;
+    }
+
+    PyObject *bii = NULL;
+    switch (kind) {
+        case BIIS_SEQUENCE: {
+            BIIterSeqObject* it = PyObject_New(BIIterSeqObject, &BIIterSeqType);
+            if (it == NULL) {goto error;}
+            it->bi = bi;
+            it->selector = selector;
+            it->reversed = reversed;
+            it->len = len;
+            it->pos = 0;
+            it->is_array = is_array;
+            bii = (PyObject*)it;
+            break;
+        }
+        case BIIS_SLICE: {
+            BIIterSliceObject* it = PyObject_New(BIIterSliceObject, &BIIterSliceType);
+            if (it == NULL) {goto error;}
+            it->bi = bi;
+            it->selector = selector;
+            it->reversed = reversed;
+            it->len = len;
+            it->pos = pos;
+            it->step = step;
+            it->count = 0;
+            bii = (PyObject*)it;
+            break;
+        }
+        case BIIS_BOOLEAN: {
+            BIIterBooleanObject* it = PyObject_New(BIIterBooleanObject, &BIIterBooleanType);
+            if (it == NULL) {goto error;}
+            it->bi = bi;
+            it->selector = selector;
+            it->reversed = reversed;
+            it->len = len;
+            it->pos = reversed ? len - 1 : 0;
+            bii = (PyObject*)it;
+            break;
+        }
+        case BIIS_UNKNOWN:
+            goto error; // should not get here!
+    }
+    Py_INCREF(bi);
+    Py_INCREF(selector);
+    return bii;
+error:
+    // nothing shold be increfed when we get here
+    return NULL;
+}
+
+
+
+//------------------------------------------------------------------------------
+
+// Returns 0 on succes, -1 on error.
+int
+AK_BI_BIR_new(BlockIndexObject* bi) {
+    BlockIndexRecord* bir = (BlockIndexRecord*)PyMem_Malloc(
+            sizeof(BlockIndexRecord) * bi->bir_capacity);
+    if (bir == NULL) {
+        return -1;
+    }
+    bi->bir = bir;
+    return 0;
+}
+
+static inline int
+AK_BI_BIR_resize(BlockIndexObject* bi, Py_ssize_t increment) {
+    Py_ssize_t target = bi->bir_count + increment;
+    Py_ssize_t capacity = bi->bir_capacity;
+    if (AK_UNLIKELY(target >= capacity)) {
+        while (capacity < target) {
+            capacity <<= 1; // get 2x the size
+        }
+        bi->bir = PyMem_Realloc(bi->bir,
+                sizeof(BlockIndexRecord) * capacity);
+        if (bi->bir == NULL) {
+            return -1;
+        }
+        bi->bir_capacity = capacity;
+    }
+    return 0;
+}
+
+
+PyDoc_STRVAR(
+    BlockIndex_doc,
+    "\n"
+    "A grow only, reference lookup of realized columns to block, block columns."
+);
+
+static PyObject *
+BlockIndex_new(PyTypeObject *cls, PyObject *args, PyObject *kwargs) {
+    BlockIndexObject *self = (BlockIndexObject *)cls->tp_alloc(cls, 0);
+    if (!self) {
+        return NULL;
+    }
+    return (PyObject *)self;
+}
+
+// Returns 0 on success, -1 on error.
+int
+BlockIndex_init(PyObject *self, PyObject *args, PyObject *kwargs) {
+    // PyTypeObject* cls = Py_TYPE(self); // borrowed ref
+    // const char *name = cls->tp_name;
+    BlockIndexObject* bi = (BlockIndexObject*)self;
+
+    Py_ssize_t block_count = 0;
+    Py_ssize_t row_count = -1; // mark as unset
+    Py_ssize_t bir_count = 0;
+    Py_ssize_t bir_capacity = 8;
+    PyObject* bir_bytes = NULL;
+    PyObject* dtype = NULL;
+
+    if (!PyArg_ParseTuple(args,
+            "|nnnnO!O:__init__",
+            &block_count,
+            &row_count,
+            &bir_count,
+            &bir_capacity,
+            &PyBytes_Type, &bir_bytes,
+            &dtype)) {
+        return -1;
+    }
+    if (bir_count > bir_capacity) {
+        PyErr_SetString(PyExc_ValueError, "record count exceeds capacity");
+        return -1;
+    }
+    // handle all Py_ssize_t
+    bi->block_count = block_count;
+    bi->row_count = row_count;
+    bi->bir_count = bir_count;
+    bi->bir_capacity = bir_capacity;
+
+    // Load the bi->bir struct array, if defined
+    bi->bir = NULL;
+    // always set bi to capacity defined at this point
+    if (AK_BI_BIR_new(bi)) {
+        return -1;
+    }
+    if (bir_bytes != NULL) {
+        // already know bir is a bytes object
+        char* data = PyBytes_AS_STRING(bir_bytes);
+        memcpy(bi->bir, data, bi->bir_count * sizeof(BlockIndexRecord));
+        // bir_bytes is a borrowed ref
+    }
+
+    bi->dtype = NULL;
+    if (dtype != NULL && dtype != Py_None) {
+        if (PyArray_DescrCheck(dtype)) {
+            Py_INCREF(dtype);
+            bi->dtype = (PyArray_Descr*)dtype;
+        }
+        else {
+            PyErr_SetString(PyExc_TypeError, "dtype argument must be a dtype");
+            return -1;
+        }
+    }
+    return 0;
+}
+
+static void
+BlockIndex_dealloc(BlockIndexObject *self) {
+    if (self->bir != NULL) {
+        PyMem_Free(self->bir);
+    }
+    if (self->dtype != NULL) {
+        Py_DECREF((PyObject*)self->dtype);
+    }
+    Py_TYPE(self)->tp_free((PyObject *)self);
+}
+
+static PyObject *
+BlockIndex_repr(BlockIndexObject *self) {
+    PyObject* dt = self->dtype == NULL ? Py_None : (PyObject*) self->dtype;
+    return PyUnicode_FromFormat("<%s(blocks: %i, rows: %i, columns: %i, dtype: %R)>",
+            Py_TYPE(self)->tp_name,
+            self->block_count,
+            self->row_count,
+            self->bir_count,
+            dt);
+}
+
+// Returns NULL on error, None otherwise. This checks and raises on non-array inputs, dimensions other than 1 or 2.
+static PyObject *
+BlockIndex_register(BlockIndexObject *self, PyObject *value) {
+    if (!PyArray_Check(value)) {
+        PyErr_Format(ErrorInitBlocks, "Found non-array block: %R", value);
+        return NULL;
+    }
+    PyArrayObject *a = (PyArrayObject *)value;
+    int ndim = PyArray_NDIM(a);
+
+    if (ndim < 1 || ndim > 2) {
+        PyErr_Format(ErrorInitBlocks, "Array block has invalid dimensions: %i", ndim);
+        return NULL;
+    }
+    Py_ssize_t increment = ndim == 1 ? 1 : PyArray_DIM(a, 1);
+
+    // assign alignment on first observation; otherwise take
+    Py_ssize_t alignment = PyArray_DIM(a, 0);
+    if (self->row_count == -1) {
+        self->row_count = alignment;
+    }
+    else if (self->row_count != alignment) {
+        PyErr_Format(ErrorInitBlocks,
+                "Array block has unaligned row count: found %i, expected %i",
+                alignment,
+                self->row_count);
+        return NULL;
+    }
+
+    PyArray_Descr* dt = PyArray_DESCR(a); // borrowed ref
+    if (self->dtype == NULL) {
+        Py_INCREF((PyObject*)dt);
+        self->dtype = dt;
+    }
+    else if (!PyDataType_ISOBJECT(self->dtype)) {
+        PyArray_Descr* dtr = AK_ResolveDTypes(self->dtype, dt); // new ref
+        Py_DECREF((PyObject*)self->dtype);
+        self->dtype = dtr;
+    }
+
+    // create space for increment new records
+    if (AK_BI_BIR_resize(self, increment)) {
+        return NULL;
+    };
+    BlockIndexRecord* bir = self->bir;
+    Py_ssize_t bc = self->block_count;
+
+    for (Py_ssize_t i = 0; i < increment; i++) {
+        bir[self->bir_count] = (BlockIndexRecord){bc, i};
+        self->bir_count++;
+    }
+    self->block_count++;
+    Py_RETURN_NONE;
+}
+
+
+static PyObject*
+BlockIndex_to_list(BlockIndexObject *self, PyObject *Py_UNUSED(unused)) {
+    PyObject* list = PyList_New(self->bir_count);
+    if (list == NULL) {
+        return NULL;
+    }
+    BlockIndexRecord* bir = self->bir;
+
+    for (Py_ssize_t i = 0; i < self->bir_count; i++) {
+        PyObject* item = Py_BuildValue("nn", bir[i].block, bir[i].column);
+        if (item == NULL) {
+            Py_DECREF(list);
+            return NULL;
+        }
+        // set_item steals reference
+        PyList_SET_ITEM(list, i, item);
+    }
+    return list;
+}
+
+
+// Returns NULL on error
+static PyObject*
+AK_BI_to_bytes(BlockIndexObject *self) {
+    Py_ssize_t size = self->bir_count * sizeof(BlockIndexRecord);
+    // bytes might be null on error
+    PyObject* bytes = PyBytes_FromStringAndSize((const char*)self->bir, size);
+    return bytes;
+}
+
+
+// Returns NULL on error
+static PyObject*
+BlockIndex_to_bytes(BlockIndexObject *self, PyObject *Py_UNUSED(unused)) {
+    return AK_BI_to_bytes(self);
+}
+
+
+// Returns NULL on error, PyObject* otherwise.
+static PyObject*
+BlockIndex_getstate(BlockIndexObject *self) {
+    PyObject* bi = AK_BI_to_bytes(self);
+    if (bi == NULL) {
+        return NULL;
+    }
+    PyObject* dt = self->dtype == NULL ? Py_None : (PyObject*) self->dtype;
+
+    // state might be NULL on failure; assume exception set
+    PyObject* state = Py_BuildValue("nnnnOO",
+            self->block_count,
+            self->row_count,
+            self->bir_count,
+            self->bir_capacity,
+            bi,
+            dt); // increfs passed object
+
+    Py_DECREF(bi);
+    return state;
+}
+
+
+// State returned here is a tuple of keys, suitable for usage as an `args` argument.
+static PyObject*
+BlockIndex_setstate(BlockIndexObject *self, PyObject *state)
+{
+    if (!PyTuple_CheckExact(state) || !PyTuple_GET_SIZE(state)) {
+        PyErr_SetString(PyExc_ValueError, "Unexpected pickled object.");
+        return NULL;
+    }
+    BlockIndex_init((PyObject*)self, state, NULL);
+    Py_RETURN_NONE;
+}
+
+
+static PyObject *
+BlockIndex_copy(BlockIndexObject *self, PyObject *Py_UNUSED(unused))
+{
+    PyTypeObject* cls = Py_TYPE(self); // borrowed ref
+    BlockIndexObject *bi = (BlockIndexObject *)cls->tp_alloc(cls, 0);
+    if (bi == NULL) {
+        return NULL;
+    }
+    bi->block_count = self->block_count;
+    bi->row_count = self->row_count;
+    bi->bir_count = self->bir_count;
+    bi->bir_capacity = self->bir_capacity;
+
+    bi->bir = NULL;
+    AK_BI_BIR_new(bi); // do initial alloc to self->bir_capacity
+    memcpy(bi->bir,
+            self->bir,
+            self->bir_count * sizeof(BlockIndexRecord));
+
+    bi->dtype = NULL;
+    if (self->dtype != NULL) {
+        bi->dtype = self->dtype;
+        Py_INCREF((PyObject*)bi->dtype);
+    }
+    return (PyObject *)bi;
+}
+
+static PyObject*
+BlockIndex_iter(BlockIndexObject* self) {
+    return BIIter_new(self, 0);
+}
+
+
+static PyObject *
+BlockIndex_shape_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
+    return Py_BuildValue("nn", self->row_count, self->bir_count);
+}
+
+static PyObject *
+BlockIndex_dtype_getter(BlockIndexObject *self, void* Py_UNUSED(closure)){
+    if (self->dtype != NULL) {
+        Py_INCREF(self->dtype);
+        return (PyObject*)self->dtype;
+    }
+    Py_RETURN_NONE;
+}
+
+static struct PyGetSetDef BlockIndex_getset[] = {
+    {"shape", (getter)BlockIndex_shape_getter, NULL, NULL, NULL},
+    {"dtype", (getter)BlockIndex_dtype_getter, NULL, NULL, NULL},
+    {NULL},
+};
+
+
+static Py_ssize_t
+BlockIndex_length(BlockIndexObject *self){
+    return self->bir_count;
+}
+
+
+static PyObject *
+BlockIndex_sizeof(BlockIndexObject *self) {
+    return PyLong_FromSsize_t(
+        Py_TYPE(self)->tp_basicsize
+        + (self->bir_capacity) * sizeof(BlockIndexRecord)
+    );
+}
+
+
+// Given an index, return just the block index.
+static PyObject*
+BlockIndex_get_block(BlockIndexObject *self, PyObject *key){
+    if (PyNumber_Check(key)) {
+        Py_ssize_t i = PyNumber_AsSsize_t(key, NULL);
+        if (!((size_t)i < (size_t)self->bir_count)) {
+            PyErr_SetString(PyExc_IndexError, "index out of range");
+            return NULL;
+        }
+        return PyLong_FromSsize_t(self->bir[i].block); // maybe NULL, exception will be set
+    }
+    PyErr_SetString(PyExc_TypeError, "An integer is required.");
+    return NULL;
+}
+
+// Given an index, return just the column index.
+static PyObject*
+BlockIndex_get_column(BlockIndexObject *self, PyObject *key){
+    if (PyNumber_Check(key)) {
+        Py_ssize_t i = PyNumber_AsSsize_t(key, NULL);
+        if (!((size_t)i < (size_t)self->bir_count)) {
+            PyErr_SetString(PyExc_IndexError, "index out of range");
+            return NULL;
+        }
+        return PyLong_FromSsize_t(self->bir[i].column); // maybe NULL, exception will be set
+    }
+    PyErr_SetString(PyExc_TypeError, "An integer is required.");
+    return NULL;
+}
+
+
+// Given key, return an iterator of a selection.
+static PyObject*
+BlockIndex_iter_select(BlockIndexObject *self, PyObject *selector){
+    return BIIterSelector_new(self, selector, 0, BIIS_UNKNOWN);
+}
+
+
+static PySequenceMethods BlockIndex_as_sequece = {
+    .sq_length = (lenfunc)BlockIndex_length,
+    .sq_item = (ssizeargfunc)AK_BI_item,
+};
+
+static PyMethodDef BlockIndex_methods[] = {
+    // {"__getitem__", (PyCFunction)BlockIndex_subscript, METH_O, NULL},
+    {"register", (PyCFunction)BlockIndex_register, METH_O, NULL},
+    {"__getstate__", (PyCFunction) BlockIndex_getstate, METH_NOARGS, NULL},
+    {"__setstate__", (PyCFunction) BlockIndex_setstate, METH_O, NULL},
+    {"__sizeof__", (PyCFunction) BlockIndex_sizeof, METH_NOARGS, NULL},
+    {"to_list", (PyCFunction)BlockIndex_to_list, METH_NOARGS, NULL},
+    {"to_bytes", (PyCFunction)BlockIndex_to_bytes, METH_NOARGS, NULL},
+    {"copy", (PyCFunction)BlockIndex_copy, METH_NOARGS, NULL},
+    {"get_block", (PyCFunction) BlockIndex_get_block, METH_O, NULL},
+    {"get_column", (PyCFunction) BlockIndex_get_column, METH_O, NULL},
+    {"iter_select", (PyCFunction) BlockIndex_iter_select, METH_O, NULL},
+    // {"__getnewargs__", (PyCFunction)BlockIndex_getnewargs, METH_NOARGS, NULL},
+    {NULL},
+};
+
+static PyTypeObject BlockIndexType = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    // .tp_as_mapping = &BlockIndex_as_mapping,
+    .tp_as_sequence = &BlockIndex_as_sequece,
+    .tp_basicsize = sizeof(BlockIndexObject), // this does not get size of struct
+    .tp_dealloc = (destructor)BlockIndex_dealloc,
+    .tp_doc = BlockIndex_doc,
+    .tp_flags = Py_TPFLAGS_DEFAULT,
+    .tp_getset = BlockIndex_getset,
+    .tp_iter = (getiterfunc)BlockIndex_iter,
+    .tp_methods = BlockIndex_methods,
+    .tp_name = "arraykit.BlockIndex",
+    .tp_new = BlockIndex_new,
+    .tp_init = BlockIndex_init,
+    .tp_repr = (reprfunc) BlockIndex_repr,
+    // .tp_traverse = (traverseproc)BlockIndex_traverse,
+};
+
+
+//------------------------------------------------------------------------------
 // ArrayGO
 //------------------------------------------------------------------------------
 
 typedef struct {
     PyObject_VAR_HEAD
     PyObject *array;
     PyObject *list;
@@ -4425,34 +5375,48 @@
     .m_methods = arraykit_methods,
 };
 
 PyObject *
 PyInit__arraykit(void)
 {
     import_array();
-    PyObject *m = PyModule_Create(&arraykit_module);
+
+    ErrorInitBlocks = PyErr_NewExceptionWithDoc(
+            "arraykit.ErrorInitBlocks",
+            "RuntimeError error in block initialization.",
+            PyExc_RuntimeError,
+            NULL);
+    if (ErrorInitBlocks == NULL) {
+        return NULL;
+    }
 
     PyObject *copy = PyImport_ImportModule("copy");
-    if (!copy) {
-        Py_XDECREF(m);
+    if (copy == NULL) {
         return NULL;
     }
     PyObject *deepcopy = PyObject_GetAttrString(copy, "deepcopy");
     Py_DECREF(copy);
-    if (!deepcopy) {
-        Py_XDECREF(m);
+    if (deepcopy == NULL) {
         return NULL;
     }
 
+    PyObject *m = PyModule_Create(&arraykit_module);
     if (!m ||
         PyModule_AddStringConstant(m, "__version__", Py_STRINGIFY(AK_VERSION)) ||
+        PyType_Ready(&BlockIndexType) ||
+        PyType_Ready(&BIIterType) ||
+        PyType_Ready(&BIIterSeqType) ||
+        PyType_Ready(&BIIterSliceType) ||
+        PyType_Ready(&BIIterBooleanType) ||
         PyType_Ready(&ArrayGOType) ||
+        PyModule_AddObject(m, "BlockIndex", (PyObject *) &BlockIndexType) ||
         PyModule_AddObject(m, "ArrayGO", (PyObject *) &ArrayGOType) ||
-        PyModule_AddObject(m, "deepcopy", deepcopy))
-    {
+        PyModule_AddObject(m, "deepcopy", deepcopy) ||
+        PyModule_AddObject(m, "ErrorInitBlocks", ErrorInitBlocks)
+    ){
         Py_DECREF(deepcopy);
         Py_XDECREF(m);
         return NULL;
     }
     return m;
 }
```

### Comparing `arraykit-0.3.4/test/test_array_go.py` & `arraykit-0.4.0/test/test_array_go.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.4/test/test_delimited_to_arrays.py` & `arraykit-0.4.0/test/test_delimited_to_arrays.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.4/test/test_delimited_to_arrays_integration.py` & `arraykit-0.4.0/test/test_delimited_to_arrays_integration.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.4/test/test_delimited_to_arrays_property.py` & `arraykit-0.4.0/test/test_delimited_to_arrays_property.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.4/test/test_pyi.py` & `arraykit-0.4.0/test/test_pyi.py`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,17 @@
         classes: tp.Dict[str: tp.List[str]] = {}
 
         for name in dir(module):
             if not cls._valid_name(name):
                 continue
             obj = getattr(module, name)
             if isinstance(obj, type): # a class
+                if name == ak.ErrorInitBlocks.__name__:
+                    # skip as there is Python version variability
+                    continue
                 classes[name] = []
                 for part_name in dir(obj):
                     if not cls._valid_name(part_name):
                         continue
                     part_obj = getattr(obj, part_name)
                     if callable(part_obj):
                         classes[name].append(part_name)
```

### Comparing `arraykit-0.3.4/test/test_split_after_count.py` & `arraykit-0.4.0/test/test_split_after_count.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.4/test/test_type_discovery.py` & `arraykit-0.4.0/test/test_type_discovery.py`

 * *Files identical despite different names*

### Comparing `arraykit-0.3.4/test/test_util.py` & `arraykit-0.4.0/test/test_util.py`

 * *Files identical despite different names*

