# Comparing `tmp/stanhelper-1.1.0-py3-none-any.whl.zip` & `tmp/stanhelper-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6098 bytes, number of entries: 7
+Zip file size: 6117 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 20-May-06 21:05 stanhelper/__init__.py
--rw-r--r--  2.0 unx    13855 b- defN 20-May-06 21:05 stanhelper/stanhelper.py
--rw-r--r--  2.0 unx     1071 b- defN 20-May-06 21:42 stanhelper-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      375 b- defN 20-May-06 21:42 stanhelper-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 20-May-06 21:42 stanhelper-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 20-May-06 21:42 stanhelper-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      558 b- defN 20-May-06 21:42 stanhelper-1.1.0.dist-info/RECORD
-7 files, 15962 bytes uncompressed, 5104 bytes compressed:  68.0%
+-rw-r--r--  2.0 unx    13902 b- defN 21-Mar-08 21:52 stanhelper/stanhelper.py
+-rw-r--r--  2.0 unx     1071 b- defN 21-Mar-08 21:54 stanhelper-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      375 b- defN 21-Mar-08 21:54 stanhelper-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Mar-08 21:54 stanhelper-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 21-Mar-08 21:54 stanhelper-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      558 b- defN 21-Mar-08 21:54 stanhelper-1.2.0.dist-info/RECORD
+7 files, 16009 bytes uncompressed, 5123 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: stanhelper/__init__.py
 Comment: 
 
 Filename: stanhelper/stanhelper.py
 Comment: 
 
-Filename: stanhelper-1.1.0.dist-info/LICENSE
+Filename: stanhelper-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: stanhelper-1.1.0.dist-info/METADATA
+Filename: stanhelper-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: stanhelper-1.1.0.dist-info/WHEEL
+Filename: stanhelper-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: stanhelper-1.1.0.dist-info/top_level.txt
+Filename: stanhelper-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: stanhelper-1.1.0.dist-info/RECORD
+Filename: stanhelper-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stanhelper/stanhelper.py

```diff
@@ -19,15 +19,15 @@
 
     # check method
     if method not in ['sample', 'optimize', 'variational']:
         raise RuntimeError(f'{method} must be either sample, optimize, '
                            'or variational.')
 
     # check that stan_binary_path is a file
-    if not os.path.isfile(stan_binary_path):
+    if not os.path.isfile(stan_binary_path) or not os.access(stan_binary_path, os.X_OK):
         raise RuntimeError(f'{stan_binary_path} is not a valid file.')
 
     # save input data to a temporary Rdump file
     input_data_rdump_file = NamedTemporaryFile()
     write_rdump(input_data, input_data_rdump_file.name)
 
     # create temporary output file
@@ -208,15 +208,15 @@
     for entry in column_names_split:
         if len(entry[1:]) != 0:
             par_names[entry[0]] = entry[1:]
         else:
             par_names[entry[0]] = [1]
 
     # get first line of parameters
-    first_line = df.ix[0].values
+    first_line = df.iloc[0].values
     first_line_pars = {}
     ofs = 0
     for par in par_names:
         shape = tuple([int(x) for x in par_names[par]])
         jump_ahead = reduce(mul, shape)
         if len(shape) != 1:
             first_line_pars[par] = np.reshape(first_line[ofs:ofs + jump_ahead],
@@ -373,15 +373,15 @@
 def read_rdump(filename: str) -> dict:
     """
     Read data formatted using the R dump format.
     """
     contents = open(filename).read().strip()
     names = [name.strip() for name in re.findall(r'^(\w+) <-', contents,
              re.MULTILINE)]
-    values = [value.strip() for value in re.split('\w+ +<-', contents)
+    values = [value.strip() for value in re.split(r'\w+ +<-', contents)
               if value]
     if len(values) != len(names):
         raise ValueError('Unable to pair variable names to values.')
     d = {}
     for name, value in zip(names, values):
         d[name.strip()] = _rdump_value_to_numpy(value.strip())
     return d
```

## Comparing `stanhelper-1.1.0.dist-info/LICENSE` & `stanhelper-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `stanhelper-1.1.0.dist-info/RECORD` & `stanhelper-1.2.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 stanhelper/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-stanhelper/stanhelper.py,sha256=bea45_UGqWPSpUmpLNi-Dt3IwPKcu4Q0hvDml7B6dLA,13855
-stanhelper-1.1.0.dist-info/LICENSE,sha256=K4CaPvlp8Oe8soOIOadXbxFbfFvDMKQdtrz3gmbwwSQ,1071
-stanhelper-1.1.0.dist-info/METADATA,sha256=iJdYeUtwxcf6gFCcHA3SYj_9tbHgnqCQ2UGpzOYbKGQ,375
-stanhelper-1.1.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-stanhelper-1.1.0.dist-info/top_level.txt,sha256=tM61275-bhTQSwdW-anJ9qtT3ZSl2YDX3dTe8elRDwU,11
-stanhelper-1.1.0.dist-info/RECORD,,
+stanhelper/stanhelper.py,sha256=OQofSR2gvcDv0XFmNj0BpXAXvgEWvF9ei--Wny4xU2s,13902
+stanhelper-1.2.0.dist-info/LICENSE,sha256=K4CaPvlp8Oe8soOIOadXbxFbfFvDMKQdtrz3gmbwwSQ,1071
+stanhelper-1.2.0.dist-info/METADATA,sha256=fjyvMtuyqYXALY6eS7Szv6F3TS2aOaSfZF4hYcsMCIU,375
+stanhelper-1.2.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+stanhelper-1.2.0.dist-info/top_level.txt,sha256=tM61275-bhTQSwdW-anJ9qtT3ZSl2YDX3dTe8elRDwU,11
+stanhelper-1.2.0.dist-info/RECORD,,
```

