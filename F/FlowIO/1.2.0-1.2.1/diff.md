# Comparing `tmp/FlowIO-1.2.0.tar.gz` & `tmp/FlowIO-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FlowIO-1.2.0.tar", last modified: Fri May  5 22:04:38 2023, max compression
+gzip compressed data, was "FlowIO-1.2.1.tar", last modified: Wed May 17 14:53:42 2023, max compression
```

## Comparing `FlowIO-1.2.0.tar` & `FlowIO-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-05 22:04:38.705233 FlowIO-1.2.0/
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-05 22:04:38.705233 FlowIO-1.2.0/FlowIO.egg-info/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     3273 2023-05-05 22:04:38.000000 FlowIO-1.2.0/FlowIO.egg-info/PKG-INFO
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      296 2023-05-05 22:04:38.000000 FlowIO-1.2.0/FlowIO.egg-info/SOURCES.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)        1 2023-05-05 22:04:38.000000 FlowIO-1.2.0/FlowIO.egg-info/dependency_links.txt
--rw-rw-r--   0 swhite    (1000) swhite    (1000)        7 2023-05-05 22:04:38.000000 FlowIO-1.2.0/FlowIO.egg-info/top_level.txt
--rw-r--r--   0 swhite    (1000) swhite    (1000)     1511 2019-08-08 15:31:25.000000 FlowIO-1.2.0/LICENSE
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       35 2022-05-19 17:10:53.000000 FlowIO-1.2.0/MANIFEST.in
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     3273 2023-05-05 22:04:38.705233 FlowIO-1.2.0/PKG-INFO
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     2755 2023-04-25 14:05:26.000000 FlowIO-1.2.0/README.md
-drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-05 22:04:38.705233 FlowIO-1.2.0/flowio/
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      288 2023-05-05 20:48:34.000000 FlowIO-1.2.0/flowio/__init__.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       45 2023-05-05 22:03:39.000000 FlowIO-1.2.0/flowio/_version.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    14808 2023-05-05 19:34:56.000000 FlowIO-1.2.0/flowio/create_fcs.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)      838 2023-05-05 19:34:56.000000 FlowIO-1.2.0/flowio/exceptions.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1573 2022-03-24 00:00:28.000000 FlowIO-1.2.0/flowio/fcs_keywords.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)    21450 2023-05-05 19:34:56.000000 FlowIO-1.2.0/flowio/flowdata.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     3005 2023-05-05 19:34:56.000000 FlowIO-1.2.0/flowio/utils.py
--rw-rw-r--   0 swhite    (1000) swhite    (1000)       38 2023-05-05 22:04:38.705233 FlowIO-1.2.0/setup.cfg
--rw-rw-r--   0 swhite    (1000) swhite    (1000)     1130 2022-05-19 17:10:53.000000 FlowIO-1.2.0/setup.py
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-17 14:53:42.342605 FlowIO-1.2.1/
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-17 14:53:42.342605 FlowIO-1.2.1/FlowIO.egg-info/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     3192 2023-05-17 14:53:42.000000 FlowIO-1.2.1/FlowIO.egg-info/PKG-INFO
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      296 2023-05-17 14:53:42.000000 FlowIO-1.2.1/FlowIO.egg-info/SOURCES.txt
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)        1 2023-05-17 14:53:42.000000 FlowIO-1.2.1/FlowIO.egg-info/dependency_links.txt
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)        7 2023-05-17 14:53:42.000000 FlowIO-1.2.1/FlowIO.egg-info/top_level.txt
+-rw-r--r--   0 swhite    (1000) swhite    (1000)     1511 2019-08-08 15:31:25.000000 FlowIO-1.2.1/LICENSE
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       35 2022-05-19 17:10:53.000000 FlowIO-1.2.1/MANIFEST.in
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     3192 2023-05-17 14:53:42.342605 FlowIO-1.2.1/PKG-INFO
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     2674 2023-05-17 14:51:50.000000 FlowIO-1.2.1/README.md
+drwxrwxr-x   0 swhite    (1000) swhite    (1000)        0 2023-05-17 14:53:42.342605 FlowIO-1.2.1/flowio/
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      288 2023-05-16 15:59:59.000000 FlowIO-1.2.1/flowio/__init__.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       45 2023-05-17 14:52:52.000000 FlowIO-1.2.1/flowio/_version.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    14808 2023-05-05 19:34:56.000000 FlowIO-1.2.1/flowio/create_fcs.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)      838 2023-05-05 19:34:56.000000 FlowIO-1.2.1/flowio/exceptions.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     1573 2022-03-24 00:00:28.000000 FlowIO-1.2.1/flowio/fcs_keywords.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)    24428 2023-05-17 14:26:27.000000 FlowIO-1.2.1/flowio/flowdata.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     3005 2023-05-05 19:34:56.000000 FlowIO-1.2.1/flowio/utils.py
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)       38 2023-05-17 14:53:42.342605 FlowIO-1.2.1/setup.cfg
+-rw-rw-r--   0 swhite    (1000) swhite    (1000)     1130 2022-05-19 17:10:53.000000 FlowIO-1.2.1/setup.py
```

### Comparing `FlowIO-1.2.0/FlowIO.egg-info/PKG-INFO` & `FlowIO-1.2.1/FlowIO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowIO
-Version: 1.2.0
+Version: 1.2.1
 Summary: FlowIO is a Python library for reading / writing Flow Cytometry Standard (FCS) files
 Home-page: https://github.com/whitews/flowio
 Author: Scott White
 Author-email: whitews@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -25,18 +25,18 @@
 [![Build & test (develop)](https://github.com/whitews/FlowIO/actions/workflows/tests_develop.yml/badge.svg)](https://github.com/whitews/FlowIO/actions/workflows/tests_develop.yml)
 [![Coverage](https://codecov.io/gh/whitews/FlowIO/branch/master/graph/badge.svg)](https://codecov.io/gh/whitews/flowio)
 [![Documentation Status](https://readthedocs.org/projects/flowio/badge/?version=latest)](https://flowio.readthedocs.io/en/latest/?badge=latest)
 
 ## Overview
 
 FlowIO is a Python library for reading / writing Flow Cytometry Standard (FCS) 
-files and has zero external dependencies. FlowIO is compatible with Python 3.7+ (FlowIO v0.9.9 was the last release supporting Python 2). 
+files, with zero external dependencies and is compatible with Python 3.7+.
 
 FlowIO retrieves event data exactly as it is encoded in the FCS file: as a 
-1-dimensional list without separating the events into channels or performing any preprocessing (e.g. applying gain). However, all the metadata 
+1-dimensional list without separating the events into channels or performing any preprocessing (e.g. applying gain). Metadata 
 stored in the FCS file is available as a dictionary via the 'text' attribute. Basic attributes
 are also available for commonly accessed properties. For example, the channel count 
 can be used to easily convert the event data to a multi-column NumPy array:
 
 ```
 import flowio
 import numpy
```

### Comparing `FlowIO-1.2.0/LICENSE` & `FlowIO-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FlowIO-1.2.0/PKG-INFO` & `FlowIO-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FlowIO
-Version: 1.2.0
+Version: 1.2.1
 Summary: FlowIO is a Python library for reading / writing Flow Cytometry Standard (FCS) files
 Home-page: https://github.com/whitews/flowio
 Author: Scott White
 Author-email: whitews@gmail.com
 License: BSD
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
@@ -25,18 +25,18 @@
 [![Build & test (develop)](https://github.com/whitews/FlowIO/actions/workflows/tests_develop.yml/badge.svg)](https://github.com/whitews/FlowIO/actions/workflows/tests_develop.yml)
 [![Coverage](https://codecov.io/gh/whitews/FlowIO/branch/master/graph/badge.svg)](https://codecov.io/gh/whitews/flowio)
 [![Documentation Status](https://readthedocs.org/projects/flowio/badge/?version=latest)](https://flowio.readthedocs.io/en/latest/?badge=latest)
 
 ## Overview
 
 FlowIO is a Python library for reading / writing Flow Cytometry Standard (FCS) 
-files and has zero external dependencies. FlowIO is compatible with Python 3.7+ (FlowIO v0.9.9 was the last release supporting Python 2). 
+files, with zero external dependencies and is compatible with Python 3.7+.
 
 FlowIO retrieves event data exactly as it is encoded in the FCS file: as a 
-1-dimensional list without separating the events into channels or performing any preprocessing (e.g. applying gain). However, all the metadata 
+1-dimensional list without separating the events into channels or performing any preprocessing (e.g. applying gain). Metadata 
 stored in the FCS file is available as a dictionary via the 'text' attribute. Basic attributes
 are also available for commonly accessed properties. For example, the channel count 
 can be used to easily convert the event data to a multi-column NumPy array:
 
 ```
 import flowio
 import numpy
```

### Comparing `FlowIO-1.2.0/README.md` & `FlowIO-1.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 [![Build & test (develop)](https://github.com/whitews/FlowIO/actions/workflows/tests_develop.yml/badge.svg)](https://github.com/whitews/FlowIO/actions/workflows/tests_develop.yml)
 [![Coverage](https://codecov.io/gh/whitews/FlowIO/branch/master/graph/badge.svg)](https://codecov.io/gh/whitews/flowio)
 [![Documentation Status](https://readthedocs.org/projects/flowio/badge/?version=latest)](https://flowio.readthedocs.io/en/latest/?badge=latest)
 
 ## Overview
 
 FlowIO is a Python library for reading / writing Flow Cytometry Standard (FCS) 
-files and has zero external dependencies. FlowIO is compatible with Python 3.7+ (FlowIO v0.9.9 was the last release supporting Python 2). 
+files, with zero external dependencies and is compatible with Python 3.7+.
 
 FlowIO retrieves event data exactly as it is encoded in the FCS file: as a 
-1-dimensional list without separating the events into channels or performing any preprocessing (e.g. applying gain). However, all the metadata 
+1-dimensional list without separating the events into channels or performing any preprocessing (e.g. applying gain). Metadata 
 stored in the FCS file is available as a dictionary via the 'text' attribute. Basic attributes
 are also available for commonly accessed properties. For example, the channel count 
 can be used to easily convert the event data to a multi-column NumPy array:
 
 ```
 import flowio
 import numpy
```

### Comparing `FlowIO-1.2.0/flowio/create_fcs.py` & `FlowIO-1.2.1/flowio/create_fcs.py`

 * *Files identical despite different names*

### Comparing `FlowIO-1.2.0/flowio/exceptions.py` & `FlowIO-1.2.1/flowio/exceptions.py`

 * *Files identical despite different names*

### Comparing `FlowIO-1.2.0/flowio/fcs_keywords.py` & `FlowIO-1.2.1/flowio/fcs_keywords.py`

 * *Files identical despite different names*

### Comparing `FlowIO-1.2.0/flowio/flowdata.py` & `FlowIO-1.2.1/flowio/flowdata.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,21 @@
     # noinspection PyUnresolvedReferences, PyUnboundLocalVariable
     basestring
 except NameError:
     # noinspection PyShadowingBuiltins
     basestring = str
 
 
+def _next_power_of_2(x):
+    if x == 0:
+        return 1
+    else:
+        return 2 ** (x - 1).bit_length()
+
+
 class FlowData(object):
     """
     Object representing a Flow Cytometry Standard (FCS) file.
     FCS versions 2.0, 3.0, and 3.1 are supported.
 
     Note on ignore_offset_error:
         Some FCS files incorrectly report the location of the last data byte
@@ -97,15 +104,18 @@
         self.text = self.__parse_text(
             current_offset,
             self.header['text_start'],
             self.header['text_stop']
         )
 
         if int(self.text.get("nextdata", "0")) != 0 and nextdata_offset is None:
-            raise MultipleDataSetsError()
+            self._fh.close()
+            raise MultipleDataSetsError(
+                "%s contains multiple data sets, use read_multiple_data_sets function" % self.name
+            )
 
         self.channel_count = int(self.text['par'])
         self.event_count = int(self.text['tot'])
 
         # parse analysis
         try:
             a_start = int(self.text['beginanalysis'])
@@ -303,24 +313,35 @@
         elif text['byteord'] == '4,3,2,1' or text['byteord'] == '2,1':
             order = '>'
         else:
             warn("unsupported byte order %s , using default @" % text['byteord'])
             order = '@'
             # from here on out we assume mode "l" (list)
 
-        bit_width = []
-        for i in range(1, int(text['par']) + 1):
-            bit_width.append(int(text['p%db' % i]))
-
         if data_type.lower() == 'i':
+            # For int data we need to check the bit width and range values.
+            # The PnR value specifies the max value for the channel. This
+            # value is exclusive, e.g. a value of 1024 means the highest
+            # integer value allowed is 1023. Integer data needs to be
+            # bit-masked according to this max range value.
+            bit_width_by_channel = {}
+            max_range_by_channel = {}
+            for i in range(1, int(text['par']) + 1):
+                bit_width_by_channel[i] = int(text['p%db' % i])
+
+                # Need to verify the value is a power of 2
+                tmp_max_range = int(text['p%dr' % i])
+                max_range_by_channel[i] = _next_power_of_2(tmp_max_range)
+
             data = self.__parse_int_data(
                 offset,
                 start,
                 stop,
-                bit_width,
+                bit_width_by_channel,
+                max_range_by_channel,
                 order
             )
         else:
             data = self.__parse_non_int_data(
                 offset,
                 start,
                 stop,
@@ -364,50 +385,97 @@
 
                 raise FCSParsingError("Unable to determine the correct byte offsets for event data")
 
         num_items = data_sect_size / data_type_size
 
         return num_items, stop
 
-    def __parse_int_data(self, offset, start, stop, bit_width, order):
+    def __parse_int_data(
+            self,
+            offset,
+            start,
+            stop,
+            bit_width_lut,
+            max_range_lut,
+            order
+    ):
         """Parse out and return integer list data from FCS file"""
 
-        if reduce(and_, [item in [8, 16, 32] for item in bit_width]):
-            # We have a uniform bit width for all parameters,
-            # use the first value to determine the number of actual events
-            if len(set(bit_width)) == 1:
-                data_type_size = bit_width[0] / 8
+        if reduce(and_, [item in [8, 16, 32] for item in bit_width_lut.values()]):
+            # Determine if we have uniform bit width values for all parameters.
+            # If so, use array.array for much faster parsing
+            if len(set(bit_width_lut.values())) == 1:
+                # We do have a uniform bit width, grab the 1st value to
+                # determine the number of actual events
+                bit_width = list(bit_width_lut.values())[0]
+                data_type_size = bit_width / 8
                 num_items, stop = self.__calc_data_item_count(start, stop, data_type_size)
 
+                # Here, we're reading the initial data array, but some channel
+                # data may still need bit-masking correction using max range
                 self._fh.seek(offset + start)
-                tmp = array.array(self.__format_integer(bit_width[0]))
+                tmp = array.array(self.__format_integer(bit_width))
                 tmp.fromfile(self._fh, int(num_items))
                 if order == '>':
                     tmp.byteswap()
 
-            # parameter sizes are different
-            # e.g. 8, 8, 16, 8, 32 ...
+                # If any bits higher shall be
+                # ignored using a bit mask. If the PnR value is not a power
+                # of 2, then the next power of 2 shall be used.
+                if any(2 ** bit_width_lut[c] > max_range_lut[c] for
+                       c in bit_width_lut.keys()) :
+
+                    amount_data_points = int(num_items / len(max_range_lut))
+                    
+                    # Create bit mask array matching length of our data array,
+                    # with values for every position being the max range value.
+                    bit_mask = array.array(
+                        self.__format_integer(bit_width),
+                        [mr - 1 for mr in max_range_lut.values()] * amount_data_points
+                    )
+                    new_tmp = array.array(self.__format_integer(bit_width))
+                    new_tmp.frombytes(bytes(map(lambda a,b: a&b, tmp.tobytes(), bit_mask.tobytes())))
+                    tmp = new_tmp
             else:
+                # parameter sizes are different
+                # e.g. 8, 8, 16, 8, 32 ...
                 # can't use array for heterogeneous bit widths
-                tmp = self.__extract_var_length_int(bit_width, offset, order, start, stop)
+                tmp = self.__extract_var_length_int(
+                    bit_width_lut,
+                    max_range_lut,
+                    offset,
+                    order,
+                    start,
+                    stop
+                )
 
         else:  # non standard bit width...  Does this happen?
             warn('Non-standard bit width for data segments')
             return None
+
         return tmp
 
-    def __extract_var_length_int(self, bit_width, offset, order, start, stop):
+    def __extract_var_length_int(self, bit_width_by_channel, max_range_by_channel, 
+                                 offset, order, start, stop):
         data_format = order
-        for cur_width in bit_width:
+        for cur_width in bit_width_by_channel.values():
             data_format += '%s' % self.__format_integer(cur_width)
 
         # array module doesn't have a function to heterogeneous bit widths,
         # so fall back to the slower unpack approach
         tuple_tmp = iter_unpack(data_format, self.__read_bytes(offset, start, stop))
-        tmp = [ti for t in tuple_tmp for ti in t]
+        if any(2**bit_width_by_channel[c] > max_range_by_channel[c] for 
+               c in bit_width_by_channel.keys()) :
+            tmp = []
+            for data_tuple in tuple_tmp:
+                for channel, max_range in max_range_by_channel.items():
+                    tmp.append(data_tuple[channel-1] % max_range)
+        else:
+            tmp = [ti for t in tuple_tmp for ti in t]
+        
         return tmp
 
     def __parse_non_int_data(self, offset, start, stop, data_type, order):
         """Parse out and return float or ASCII list data from FCS file"""
         data_type_size = calcsize(data_type)
         num_items, stop = self.__calc_data_item_count(start, stop, data_type_size)
```

### Comparing `FlowIO-1.2.0/flowio/utils.py` & `FlowIO-1.2.1/flowio/utils.py`

 * *Files identical despite different names*

### Comparing `FlowIO-1.2.0/setup.py` & `FlowIO-1.2.1/setup.py`

 * *Files identical despite different names*

