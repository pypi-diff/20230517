# Comparing `tmp/risingwave-0.0.6.tar.gz` & `tmp/risingwave-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risingwave-0.0.6.tar", last modified: Mon May 15 09:47:01 2023, max compression
+gzip compressed data, was "risingwave-0.0.7.tar", last modified: Wed May 17 02:34:30 2023, max compression
```

## Comparing `risingwave-0.0.6.tar` & `risingwave-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-15 09:47:01.778306 risingwave-0.0.6/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-05-15 09:47:01.778167 risingwave-0.0.6/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)     1859 2023-03-27 03:26:39.000000 risingwave-0.0.6/README.md
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-15 09:47:01.777324 risingwave-0.0.6/risingwave/
--rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.6/risingwave/__init__.py
--rw-r--r--   0 wangrunji   (501) staff       (20)    11869 2023-05-15 09:45:39.000000 risingwave-0.0.6/risingwave/udf.py
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-15 09:47:01.777966 risingwave-0.0.6/risingwave.egg-info/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2194 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)      228 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/SOURCES.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/dependency_links.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)        8 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/requires.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-05-15 09:47:01.000000 risingwave-0.0.6/risingwave.egg-info/top_level.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-05-15 09:47:01.778342 risingwave-0.0.6/setup.cfg
--rw-r--r--   0 wangrunji   (501) staff       (20)      606 2023-05-15 09:45:39.000000 risingwave-0.0.6/setup.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-17 02:34:30.191217 risingwave-0.0.7/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     2215 2023-05-17 02:34:30.191094 risingwave-0.0.7/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)     1859 2023-03-27 03:26:39.000000 risingwave-0.0.7/README.md
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-17 02:34:30.190368 risingwave-0.0.7/risingwave/
+-rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.7/risingwave/__init__.py
+-rw-r--r--   0 wangrunji   (501) staff       (20)     3120 2023-05-17 02:33:59.000000 risingwave-0.0.7/risingwave/test_udf.py
+-rw-r--r--   0 wangrunji   (501) staff       (20)    13189 2023-05-17 02:33:59.000000 risingwave-0.0.7/risingwave/udf.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-17 02:34:30.190934 risingwave-0.0.7/risingwave.egg-info/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     2215 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)      251 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/SOURCES.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/dependency_links.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       23 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/requires.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/top_level.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-05-17 02:34:30.191248 risingwave-0.0.7/setup.cfg
+-rw-r--r--   0 wangrunji   (501) staff       (20)      661 2023-05-17 02:33:59.000000 risingwave-0.0.7/setup.py
```

### Comparing `risingwave-0.0.6/PKG-INFO` & `risingwave-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: risingwave
-Version: 0.0.6
+Version: 0.0.7
 Summary: RisingWave Python API
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 
 # RisingWave Python API
 
 This library provides a Python API for creating user-defined functions (UDF) in RisingWave.
 
 Currently, RisingWave supports user-defined functions implemented as external functions.
 Users need to define functions using the API provided by this library, and then start a Python process as a UDF server.
```

### Comparing `risingwave-0.0.6/README.md` & `risingwave-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `risingwave-0.0.6/risingwave/udf.py` & `risingwave-0.0.7/risingwave/udf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,54 +1,68 @@
 from typing import *
 import pyarrow as pa
 import pyarrow.flight
 import pyarrow.parquet
 import inspect
 import traceback
 import json
+from concurrent.futures import ThreadPoolExecutor
+import concurrent
 
 
 class UserDefinedFunction:
     """
     Base interface for user-defined function.
     """
 
     _name: str
     _input_schema: pa.Schema
     _result_schema: pa.Schema
+    _io_threads: Optional[int]
+    _executor: Optional[ThreadPoolExecutor]
 
     def eval_batch(self, batch: pa.RecordBatch) -> Iterator[pa.RecordBatch]:
         """
         Apply the function on a batch of inputs.
         """
         return iter([])
 
 
 class ScalarFunction(UserDefinedFunction):
     """
     Base interface for user-defined scalar function. A user-defined scalar functions maps zero, one,
     or multiple scalar values to a new scalar value.
     """
 
+    def __init__(self, *args, **kwargs):
+        self._io_threads = kwargs.pop("io_threads")
+        self._executor = ThreadPoolExecutor(max_workers=self._io_threads) if self._io_threads is not None else None
+        super().__init__(*args, **kwargs)
+
     def eval(self, *args) -> Any:
         """
         Method which defines the logic of the scalar function.
         """
         pass
 
     def eval_batch(self, batch: pa.RecordBatch) -> Iterator[pa.RecordBatch]:
         # parse value from json string for jsonb columns
         inputs = [[v.as_py() for v in array] for array in batch]
         inputs = [
             _process_input_array(array, type)
             for array, type in zip(inputs, self._input_schema.types)
         ]
-
-        # evaluate the function for each row
-        column = [self.eval(*[col[i] for col in inputs]) for i in range(batch.num_rows)]
+        if self._executor is not None:
+            # evaluate the function for each row
+            tasks = [self._executor.submit(self._func, *[col[i] for col in inputs])
+                    for i in range(batch.num_rows)]
+            column = [future.result() for future in concurrent.futures.as_completed(tasks)]
+        else:
+            # evaluate the function for each row
+            column = [self.eval(*[col[i] for col in inputs]) for i in range(batch.num_rows)]
 
         # convert value to json for jsonb columns
         if self._result_schema.types[0] == pa.large_string():
             column = [(json.dumps(v) if v is not None else None) for v in column]
         array = pa.array(column, type=self._result_schema.types[0])
         yield pa.RecordBatch.from_arrays([array], schema=self._result_schema)
 
@@ -128,34 +142,34 @@
 class UserDefinedScalarFunctionWrapper(ScalarFunction):
     """
     Base Wrapper for Python user-defined scalar function.
     """
 
     _func: Callable
 
-    def __init__(self, func, input_types, result_type, name=None):
+    def __init__(self, func, input_types, result_type, name=None, io_threads=None):
         self._func = func
         self._input_schema = pa.schema(
             zip(
                 inspect.getfullargspec(func)[0],
                 [_to_data_type(t) for t in _to_list(input_types)],
             )
         )
         self._result_schema = pa.schema([("output", _to_data_type(result_type))])
         self._name = name or (
             func.__name__ if hasattr(func, "__name__") else func.__class__.__name__
         )
+        super().__init__(io_threads=io_threads)
 
     def __call__(self, *args):
         return self._func(*args)
 
     def eval(self, *args):
         return self._func(*args)
 
-
 class UserDefinedTableFunctionWrapper(TableFunction):
     """
     Base Wrapper for Python user-defined table function.
     """
 
     _func: Callable
 
@@ -177,46 +191,58 @@
 
     def __call__(self, *args):
         return self._func(*args)
 
     def eval(self, *args):
         return self._func(*args)
 
-
 def _to_list(x):
     if isinstance(x, list):
         return x
     else:
         return [x]
 
 
 def udf(
     input_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
     result_type: Union[str, pa.DataType],
     name: Optional[str] = None,
+    io_threads: Optional[int] = None,
 ) -> Callable:
     """
     Annotation for creating a user-defined scalar function.
 
     Parameters:
     - input_types: A list of strings or Arrow data types that specifies the input data types.
     - result_type: A string or an Arrow data type that specifies the return value type.
     - name: An optional string specifying the function name. If not provided, the original name will be used.
+    - io_threads: Number of I/O threads used per data chunk for I/O bound functions.
 
     Example:
     ```
     @udf(input_types=['INT', 'INT'], result_type='INT')
     def gcd(x, y):
         while y != 0:
             (x, y) = (y, x % y)
         return x
     ```
+
+    I/O bound Example:
+    ```
+    @udf(input_types=['INT'], result_type='INT', io_threads=64)
+    def external_api(x):
+        response = requests.get(my_endpoint + '?param=' + x)
+        return response["data"]
+    ```
     """
 
-    return lambda f: UserDefinedScalarFunctionWrapper(f, input_types, result_type, name)
+    if io_threads is not None and io_threads > 1:
+        return lambda f: UserDefinedScalarFunctionWrapper(f, input_types, result_type, name, io_threads=io_threads)
+    else:
+        return lambda f: UserDefinedScalarFunctionWrapper(f, input_types, result_type, name)
 
 
 def udtf(
     input_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
     result_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
     name: Optional[str] = None,
 ) -> Callable:
```

### Comparing `risingwave-0.0.6/risingwave.egg-info/PKG-INFO` & `risingwave-0.0.7/risingwave.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: risingwave
-Version: 0.0.6
+Version: 0.0.7
 Summary: RisingWave Python API
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: test
 
 # RisingWave Python API
 
 This library provides a Python API for creating user-defined functions (UDF) in RisingWave.
 
 Currently, RisingWave supports user-defined functions implemented as external functions.
 Users need to define functions using the API provided by this library, and then start a Python process as a UDF server.
```

### Comparing `risingwave-0.0.6/setup.py` & `risingwave-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="risingwave",
-    version="0.0.6",
+    version="0.0.7",
     author="RisingWave Labs",
     description="RisingWave Python API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/risingwavelabs/risingwave",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "License :: OSI Approved :: Apache Software License",
     ],
     python_requires=">=3.8",
-    install_requires=["pyarrow"],
+    install_requires=['pyarrow'],
+    extras_require={
+        'test': ['pytest']
+    },
 )
```

