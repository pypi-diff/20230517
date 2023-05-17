# Comparing `tmp/pyodc-1.2.0.tar.gz` & `tmp/pyodc-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodc-1.2.0.tar", last modified: Thu May 11 13:05:42 2023, max compression
+gzip compressed data, was "pyodc-1.3.0.tar", last modified: Wed May 17 13:29:33 2023, max compression
```

## Comparing `pyodc-1.2.0.tar` & `pyodc-1.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:05:42.730787 pyodc-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-05-11 13:05:18.000000 pyodc-1.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-11 13:05:18.000000 pyodc-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-11 13:05:18.000000 pyodc-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-05-11 13:05:42.730787 pyodc-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2923 2023-05-11 13:05:18.000000 pyodc-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:05:42.730787 pyodc-1.2.0/codc/
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     4308 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    11079 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/frame.py
--rw-r--r--   0 runner    (1001) docker     (122)     4718 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/lib.py
--rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/processed_odc.h
--rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-05-11 13:05:18.000000 pyodc-1.2.0/codc/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:05:42.730787 pyodc-1.2.0/pyodc/
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14921 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/codec.py
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     6386 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/encoder.py
--rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/frame.py
--rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/reader.py
--rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyodc/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-11 13:05:42.730787 pyodc-1.2.0/pyodc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-11 13:05:42.000000 pyodc-1.2.0/pyodc.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-11 13:05:18.000000 pyodc-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-11 13:05:42.730787 pyodc-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-11 13:05:18.000000 pyodc-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:29:33.162597 pyodc-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1861 2023-05-17 13:29:16.000000 pyodc-1.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-17 13:29:16.000000 pyodc-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-17 13:29:16.000000 pyodc-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-05-17 13:29:33.162597 pyodc-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2923 2023-05-17 13:29:16.000000 pyodc-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:29:33.158597 pyodc-1.3.0/codc/
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5119 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11772 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4718 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/lib.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5122 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/processed_odc.h
+-rw-r--r--   0 runner    (1001) docker     (122)     2197 2023-05-17 13:29:16.000000 pyodc-1.3.0/codc/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:29:33.162597 pyodc-1.3.0/pyodc/
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15966 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/codec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6957 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13398 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/frame.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2630 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/reader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2804 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyodc/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-17 13:29:33.162597 pyodc-1.3.0/pyodc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5706 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-17 13:29:33.000000 pyodc-1.3.0/pyodc.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-17 13:29:16.000000 pyodc-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-17 13:29:33.162597 pyodc-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1996 2023-05-17 13:29:16.000000 pyodc-1.3.0/setup.py
```

### Comparing `pyodc-1.2.0/CHANGELOG.md` & `pyodc-1.3.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `pyodc-1.2.0/LICENSE` & `pyodc-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodc-1.2.0/PKG-INFO` & `pyodc-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodc
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python interface to odc for encoding/decoding ODB-2 files.
 Home-page: https://github.com/ecmwf/pyodc
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: odc odb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyodc-1.2.0/README.md` & `pyodc-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyodc-1.2.0/codc/encoder.py` & `pyodc-1.3.0/codc/encoder.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 import pandas
 
-from .constants import DOUBLE, INTEGER, STRING
+from .constants import BITFIELD, DOUBLE, INTEGER, STRING
 from .lib import ffi, lib
 
 
-def encode_odb(df: pandas.DataFrame, f, types: dict = None, rows_per_frame=10000, properties=None, **kwargs):
+def encode_odb(
+    df: pandas.DataFrame, f, types: dict = None, rows_per_frame=10000, properties=None, bitfields: dict = None, **kwargs
+):
     """
     Encode a pandas dataframe into ODB2 format
 
     :param df: The dataframe to encode
     :param f: The file-like object into which to encode the ODB2 data
     :param types: An optional (sparse) dictionary. Each key-value pair maps the name of a column to
                   encode to an ODB2 data type to use to encode it.
     :param rows_per_frame: The maximum number of rows to encode per frame. If this number is exceeded,
                            a sequence of frames will be encoded
+    :param bitfields: A dictionary containing entries for BITFIELD columns. The values are either bitfield names, or
+                      tuple pairs of bitfield name and bitfield size
     :param kwargs: Accept extra arguments that may be used by the python pyodc encoder.
     :return:
     """
     if isinstance(f, str):
         with open(f, "wb") as freal:
             return encode_odb(df, freal, types=types, rows_per_frame=rows_per_frame, properties=properties, **kwargs)
 
@@ -39,37 +43,45 @@
             - return_arr is the column of data to encode. This may be of a different internal type/contents
               to that supplied to the function, but it will normally not be.
             - The ODB2 type to encode with.
         """
         return_arr = arr
         dtype = override_type
 
+        # Infer the column type from the data, if no column type given
+
         if dtype is None:
             if arr.dtype in ("uint64", "int64"):
                 dtype = INTEGER
             elif arr.dtype == "float64":
                 if not data.isnull().all() and all(pandas.isnull(v) or float(v).is_integer() for v in arr):
                     dtype = INTEGER
-                    return_arr = arr.fillna(value=missing_integer).astype("int64")
                 else:
                     dtype = DOUBLE
-                    return_arr = arr.fillna(value=missing_double)
             elif arr.dtype == "object":
                 if not arr.isnull().all() and all(s is None or isinstance(s, str) for s in arr):
                     dtype = STRING
                 elif arr.isnull().all():
                     dtype = INTEGER
 
+        # With an inferred, or supplied column type, massage the data into a form that can be encoded
+
         if arr.dtype == "object":
             # Map strings into an array that can be read in C
             if dtype == STRING:
                 return_arr = return_arr.astype("|S{}".format(max(8, 8 * (1 + ((max(len(s) for s in arr) - 1) // 8)))))
-            elif dtype == INTEGER:
+            elif dtype == INTEGER or dtype == BITFIELD:
                 return_arr = return_arr.fillna(value=missing_integer).astype("int64")
 
+        elif arr.dtype == "float64":
+            if dtype == INTEGER or dtype == BITFIELD:
+                return_arr = arr.fillna(value=missing_integer).astype("int64")
+            else:
+                return_arr = arr.fillna(value=missing_double)
+
         if dtype is None:
             raise ValueError("Unsupported value type: {}".format(arr.dtype))
 
         return return_arr, dtype
 
     nrows = df.shape[0]
     if types is None:
@@ -99,8 +111,14 @@
             encoder,
             i,
             data.dtype.itemsize,
             data.array.to_numpy().strides[0],
             ffi.cast("void*", data.values.ctypes.data),
         )
 
+        if bitfields and name in bitfields:
+            for bf in bitfields[name]:
+                nm = bf if isinstance(bf, str) else bf[0]
+                sz = 1 if isinstance(bf, str) else bf[1]
+                lib.odc_encoder_column_add_bitfield(encoder, i, nm.encode("utf-8"), sz)
+
     lib.odc_encode_to_file_descriptor(encoder, f.fileno(), ffi.NULL)
```

### Comparing `pyodc-1.2.0/codc/frame.py` & `pyodc-1.3.0/codc/frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,17 @@
 
         def __eq__(self, other):
             return self.name == other.name and self.size == other.size and self.offset == other.offset
 
         def __str__(self):
             return f"bits(name={self.name}, size={self.size}, offset={self.offset})"
 
+        def __repr__(self):
+            return str(self)
+
     def __init__(self, name, idx, dtype, datasize, bitfields):
         self.name = name
         self.dtype = dtype
         self.index = idx
         self.datasize = datasize
         self.bitfields = bitfields
         assert (dtype == BITFIELD) != (bitfields is None)
@@ -192,21 +195,36 @@
 
         # If there are any bitfields that need extraction, do it here, and remove any temporarily
         # decoded columns as is possible
 
         if bitfields:
             extracted_columns = set()
             for bitfield_name, column_name, output_name in bitfields:
-                assert df[column_name].dtype == np.int64
                 col = self.column_dict[column_name]
-                bf = next((b for b in col.bitfields if b.name == bitfield_name))
+                try:
+                    bf = next((b for b in col.bitfields if b.name == bitfield_name))
+                except StopIteration:
+                    raise KeyError(f"Bitfield '{bitfield_name}' not found")
+
+                # If there are missing values in the column, then it will have been decoded as a float64 to support NaN
+                raw_column = df[column_name]
+                missing_vals = None
+                if raw_column.dtype == np.float64:
+                    missing_vals = np.isnan(raw_column)
+                    raw_column = raw_column.fillna(value=0).astype("int64")
+
                 mask = (1 << bf.size) - 1
-                new_column = np.right_shift(df[column_name], bf.offset) & mask
+                new_column = np.right_shift(raw_column, bf.offset) & mask
                 if bf.size == 1:
                     new_column = new_column.astype(bool)
+
+                # If we have missing values, we need to recreate these
+                if missing_vals is not None:
+                    new_column[missing_vals] = np.nan
+
                 df[output_name] = new_column
                 extracted_columns.add(column_name)
 
             for column in extracted_columns:
                 if column not in original_columns:
                     del df[column]
```

### Comparing `pyodc-1.2.0/codc/lib.py` & `pyodc-1.3.0/codc/lib.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.2.0/codc/processed_odc.h` & `pyodc-1.3.0/codc/processed_odc.h`

 * *Files identical despite different names*

### Comparing `pyodc-1.2.0/codc/reader.py` & `pyodc-1.3.0/codc/reader.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.2.0/pyodc/codec.py` & `pyodc-1.3.0/pyodc/codec.py`

 * *Files 9% similar despite different names*

```diff
@@ -55,15 +55,24 @@
         Size of the decoded data in bytes.
         """
         return 8
 
     def encode_header(self, stream):
         stream.encodeString(self.column_name)
         stream.encodeInt32(self.type)
-        # TODO: Bitfield stuff goes here
+
+        if self.type == DataType.BITFIELD:
+            assert len(self.bitfield_sizes) == len(self.bitfield_names)
+            stream.encodeInt32(len(self.bitfield_names))
+            for nm in self.bitfield_names:
+                stream.encodeString(nm)
+            stream.encodeInt32(len(self.bitfield_sizes))
+            for sz in self.bitfield_sizes:
+                stream.encodeInt32(sz)
+
         stream.encodeString(self.name)
         stream.encodeInt32(1 if self.has_missing else 0)
         stream.encodeReal64(self.min)
         stream.encodeReal64(self.max)
         stream.encodeReal64(self.missing_value)
 
     @staticmethod
@@ -71,15 +80,15 @@
         has_missing = False if stream.readInt32() == 0 else True
         minval = stream.readReal64()
         maxval = stream.readReal64()
         missing_value = stream.readReal64()
         return has_missing, minval, maxval, missing_value
 
     @classmethod
-    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
+    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType, bitfields):
         raise NotImplementedError
 
     @classmethod
     def from_stream(cls, stream, column_name: str, data_type: DataType, bitfield_names, bitfield_sizes):
         has_missing, minval, maxval, missing_value = cls.read_core_header(stream)
         return cls(
             column_name,
@@ -103,16 +112,17 @@
 
 
 # n.b. The codec names match the class names
 
 
 class Constant(Codec):
     @classmethod
-    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
+    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType, bitfields):
         assert data.nunique() == 1 and not data.hasnans
+        assert not bitfields
         value = next(iter(data))
         return cls(column_name, value, value, data_type)
 
     def encode(self, stream, value):
         pass
 
     def decode(self, stream):
@@ -123,17 +133,18 @@
     @property
     def numChanges(self):
         return 0
 
 
 class ConstantString(Constant):
     @classmethod
-    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
+    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType, bitfields):
         assert data.nunique() == 1 and not data.hasnans
         assert data_type == DataType.STRING
+        assert not bitfields
 
         # n.b. This looks like it ties it to little-endian, but it doesn't. Byte order
         #      is always the same for string data, but we are 'pretending' to be a double.
         value = struct.unpack("<d", (next(iter(data)).encode("utf-8") + (b"\x00" * 8))[:8])[0]
 
         return cls(column_name, value, value, data_type)
 
@@ -143,17 +154,32 @@
 
 class NumericBase(Codec):
     _numChanges = None
     _data = None
     accepted_types = None
 
     @classmethod
-    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
+    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType, bitfields):
         assert data_type in cls.accepted_types
-        c = cls(column_name, data.min(), data.max(), data_type, has_missing=data.hasnans)
+        if bitfields:
+            assert data_type == DataType.BITFIELD
+            bitfield_names = [bf if isinstance(bf, str) else bf[0] for bf in bitfields]
+            bitfield_sizes = [1 if isinstance(bf, str) else bf[1] for bf in bitfields]
+        else:
+            bitfield_names = []
+            bitfield_sizes = []
+        c = cls(
+            column_name,
+            data.min(),
+            data.max(),
+            data_type,
+            has_missing=data.hasnans,
+            bitfield_names=bitfield_names,
+            bitfield_sizes=bitfield_sizes,
+        )
         c._data = data
         return c
 
     @property
     def numChanges(self):
         if self._numChanges is None:
             assert self._data is not None
@@ -162,17 +188,17 @@
 
 
 class ConstantOrMissing(NumericBase):
     internal_missing_value = 0xFF
     accepted_types = (DataType.INTEGER, DataType.BITFIELD)
 
     @classmethod
-    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
+    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType, bitfields):
         assert data.nunique() == 1 and data.hasnans
-        return super().from_dataframe(column_name, data, data_type)
+        return super().from_dataframe(column_name, data, data_type, bitfields)
 
     def encode(self, stream, value):
         if pd.isnull(value):
             stream.encodeUInt8(self.internal_missing_value)
         else:
             stream.encodeUInt8(0)
 
@@ -257,18 +283,18 @@
 class Int32(NumericBase):
     max_range = 0xFFFFFFFE
     accepts_missing = True
     internal_missing_value = 0x7FFFFFFF
     accepted_types = (DataType.INTEGER, DataType.BITFIELD)
 
     @classmethod
-    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
+    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType, bitfields):
         if data.min() < -0x80000000 or data.max() >= 0x7FFFFFFF:
             raise ValueError("Cannot encode integers out of range")
-        c = super().from_dataframe(column_name, data, data_type)
+        c = super().from_dataframe(column_name, data, data_type, bitfields)
         assert c.missing_value == c.internal_missing_value
         return c
 
     def encode(self, stream, value):
         if pd.isnull(value):
             stream.encodeInt32(self.internal_missing_value)
         else:
@@ -319,17 +345,18 @@
         assert values is not None
         self.values = values
         self.value_map = {value: i for i, value in enumerate(values)}
 
         super().__init__(*args, **kwargs)
 
     @classmethod
-    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType):
+    def from_dataframe(cls, column_name: str, data: pd.Series, data_type: DataType, bitfields):
         assert not data.hasnans
         assert data_type == DataType.STRING
+        assert not bitfields
         return cls(column_name, 0, 0, data_type, values=data.unique(), data=data)
 
     @classmethod
     def from_stream(cls, stream, column_name: str, data_type: DataType, bitfield_names, bitfield_sizes):
         has_missing, minval, maxval, missing_value = cls.read_core_header(stream)
         nvalues = stream.readInt32()
         values = [None] * nvalues
@@ -388,15 +415,15 @@
         stream.encodeUInt16(value)
 
     @staticmethod
     def _decode(stream):
         return stream.readUInt16()
 
 
-def select_codec(column_name: str, data: pd.Series, data_type):
+def select_codec(column_name: str, data: pd.Series, data_type, bitfields):
     # If data types are not specified, determine them from the pandas Series
 
     if data_type is None:
         if data.dtype in ["{}int{}".format(s, b) for s in ("", "u") for b in (8, 16, 32, 64)]:
             data_type = DataType.INTEGER
         elif data.dtype == "float64":
             if not data.isnull().all() and all(pd.isnull(v) or float(v).is_integer() for v in data):
@@ -459,15 +486,15 @@
         elif data.nunique() <= 256:
             codec_class = Int8String
         else:
             assert data.nunique() <= 32767
             codec_class = Int16String
 
     if codec_class is not None:
-        return codec_class.from_dataframe(column_name, data, data_type)
+        return codec_class.from_dataframe(column_name, data, data_type, bitfields)
 
     print(data)
     print(data_type)
     raise NotImplementedError
 
 
 def read_codec(stream):
```

### Comparing `pyodc-1.2.0/pyodc/constants.py` & `pyodc-1.3.0/pyodc/constants.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.2.0/pyodc/encoder.py` & `pyodc-1.3.0/pyodc/encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,82 +9,93 @@
 from .stream import BigEndianStream, LittleEndianStream
 
 
 def encode_odb(
     dataframe: pd.DataFrame,
     target,
     rows_per_frame=10000,
-    types=None,
+    types: dict = None,
     bigendian: bool = False,
     properties: dict = None,
+    bitfields: dict = None,
 ):
     """
     Encode a pandas dataframe into an ODB-2 stream
 
     Parameters:
         dataframe(DataFrame): A pandas dataframe to encode
         target(str|file): A file-like object to write the encoded data to
-        columns(dict): A dictionary of (optional) column-name : constant :class:`.DataType` pairs, or ``None``
+        types(dict): A dictionary of (optional) column-name : constant :class:`.DataType` pairs, or ``None``
         bigendian(bool): Encode in big-endian byte order if ``True``
         properties(dict): Encode a dictionary of supplied properties
+        bitfields(dict): A dictionary containing entries for BITFIELD columns. The values are either bitfield names, or
+                         tuple pairs of bitfield name and bitfield size
     """
     if isinstance(target, str):
         with open(target, "wb") as real_target:
             return encode_odb(
                 dataframe,
                 real_target,
                 rows_per_frame=rows_per_frame,
                 types=types,
                 bigendian=bigendian,
                 properties=properties,
+                bitfields=bitfields,
             )
 
     column_order = None
 
     # Split the dataframe into chunks of appropriate size
     for i, sub_df in dataframe.groupby(np.arange(len(dataframe)) // rows_per_frame):
         column_order = encode_single_dataframe(
             sub_df,
             target,
             types=types,
             column_order=column_order,
             bigendian=bigendian,
             properties=(properties or {}),
+            bitfields=bitfields,
         )
 
 
 def encode_single_dataframe(
     dataframe: pd.DataFrame,
     target,
     types: dict = None,
     column_order: list = None,
     bigendian: bool = False,
     properties: dict = None,
+    bitfields: dict = None,
 ):
     """
     Encode a single dataframe into an ODB-2 stream
 
     Parameters:
         dataframe(DataFrame): A pandas dataframe to encode
         target(str|file): A file-like object to write the encoded data to
-        columns(dict): A dictionary of (optional) column-name : constant :class:`.DataType` pairs, or ``None``
+        types(dict): A dictionary of (optional) column-name : constant :class:`.DataType` pairs, or ``None``
         column_order(list): A list of column names specifying the encode order. If ``None``, optimise according
                             to the rate of value changes in the columns
         bigendian(bool): Encode in big-endian byte order if ``True``
         properties(dict): Encode a dictionary of supplied properties
+        bitfields(dict): A dictionary containing entries for BITFIELD columns. The values are either bitfield names, or
+                         tuple pairs of bitfield name and bitfield size
 
     Returns:
         list: The column order used for encoding as a list of column names
 
     :meta private:
     """
 
     stream_class = BigEndianStream if bigendian else LittleEndianStream
 
-    codecs = [select_codec(name, data, (types or {}).get(name, None)) for name, data in dataframe.items()]
+    codecs = [
+        select_codec(name, data, (types or {}).get(name, None), (bitfields or {}).get(name, None))
+        for name, data in dataframe.items()
+    ]
 
     # If a column order has been specified, sort the codecs according to it. otherwise sort
     # the codecs for the most efficient use of the given data
 
     if column_order:
         assert len(column_order) == len(set(column_order))
         assert set(column_order) == set(c.column_name for c in codecs)
```

### Comparing `pyodc-1.2.0/pyodc/frame.py` & `pyodc-1.3.0/pyodc/frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,14 +78,17 @@
 
         def __eq__(self, other):
             return self.name == other.name and self.size == other.size and self.offset == other.offset
 
         def __str__(self):
             return f"bits(name={self.name}, size={self.size}, offset={self.offset})"
 
+        def __repr__(self):
+            return str(self)
+
     def __init__(self, name, idx, dtype, datasize, bitfields):
         self.name = name
         self.dtype = dtype
         self.index = idx
         self.datasize = datasize
         self.bitfields = bitfields
 
@@ -279,21 +282,36 @@
 
         # If there are any bitfields that need extraction, do it here, and remove any temporarily
         # decoded columns as is possible
 
         if bitfields:
             extracted_columns = set()
             for bitfield_name, column_name, output_name in bitfields:
-                assert df[column_name].dtype == np.int64
                 col = self.column_dict[column_name]
-                bf = next((b for b in col.bitfields if b.name == bitfield_name))
+                try:
+                    bf = next((b for b in col.bitfields if b.name == bitfield_name))
+                except StopIteration:
+                    raise KeyError(f"Bitfield '{bitfield_name}' not found")
+
+                # If there are missing values in the column, then it will have been decoded as a float64 to support NaN
+                raw_column = df[column_name]
+                missing_vals = None
+                if raw_column.dtype == np.float64:
+                    missing_vals = np.isnan(raw_column)
+                    raw_column = raw_column.fillna(value=0).astype("int64")
+
                 mask = (1 << bf.size) - 1
-                new_column = np.right_shift(df[column_name], bf.offset) & mask
+                new_column = np.right_shift(raw_column, bf.offset) & mask
                 if bf.size == 1:
                     new_column = new_column.astype(bool)
+
+                # If we have missing values, we need to recreate these
+                if missing_vals is not None:
+                    new_column[missing_vals] = np.nan
+
                 df[output_name] = new_column
                 extracted_columns.add(column_name)
 
             for column in extracted_columns:
                 if column not in original_columns:
                     del df[column]
 
@@ -328,14 +346,19 @@
                 if len(splitname) == 2:
                     name, table = splitname
                     if name in columns:
                         if name in output:
                             raise KeyError("Ambiguous short column name '{}' requested".format(name))
                         output[name] = output_col
 
+        if columns:
+            for name in columns:
+                if name not in output:
+                    raise KeyError(f"Requested columns '{name}' not found")
+
         lastDecoded = [0] * self._numberOfColumns
 
         lastStartCol = None
         for row in range(self._numberOfRows):
             startCol = self._stream.readMarker()
 
             if lastStartCol is None:
@@ -359,15 +382,15 @@
                 last = output_cols[col][-1]
                 output_cols[col].extend(last for _ in range(self._numberOfRows - lastDecoded[col] - 1))
 
         df = pd.DataFrame(output)
 
         if len(self._trailingAggregatedFrames) > 0:
             return pd.concat(
-                [df] + [f.dataframe(columns) for f in self._trailingAggregatedFrames],
+                [df] + [f._dataframe_internal(columns) for f in self._trailingAggregatedFrames],
                 copy=False,
                 axis=0,
                 ignore_index=True,
             )
         else:
             return df
```

### Comparing `pyodc-1.2.0/pyodc/reader.py` & `pyodc-1.3.0/pyodc/reader.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.2.0/pyodc/stream.py` & `pyodc-1.3.0/pyodc/stream.py`

 * *Files identical despite different names*

### Comparing `pyodc-1.2.0/pyodc.egg-info/PKG-INFO` & `pyodc-1.3.0/pyodc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodc
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Python interface to odc for encoding/decoding ODB-2 files.
 Home-page: https://github.com/ecmwf/pyodc
 Author: European Centre for Medium-Range Weather Forecasts (ECMWF)
 Author-email: software.support@ecmwf.int
 License: Apache License Version 2.0
 Keywords: odc odb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyodc-1.2.0/setup.py` & `pyodc-1.3.0/setup.py`

 * *Files identical despite different names*

