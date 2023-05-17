# Comparing `tmp/mmcb-avt-0.0.89.tar.gz` & `tmp/mmcb-avt-0.0.90.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmcb-avt-0.0.89.tar", last modified: Fri May 12 10:50:20 2023, max compression
+gzip compressed data, was "mmcb-avt-0.0.90.tar", last modified: Wed May 17 14:46:21 2023, max compression
```

## Comparing `mmcb-avt-0.0.89.tar` & `mmcb-avt-0.0.90.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 10:50:20.393566 mmcb-avt-0.0.89/
--rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.89/LICENSE
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-12 10:50:20.392777 mmcb-avt-0.0.89/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.89/README.md
--rw-r--r--   0 avt        (501) staff       (20)      104 2022-05-30 11:29:45.000000 mmcb-avt-0.0.89/pyproject.toml
--rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-12 10:50:20.393788 mmcb-avt-0.0.89/setup.cfg
--rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-12 10:49:59.000000 mmcb-avt-0.0.89/setup.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 10:50:20.346208 mmcb-avt-0.0.89/src/
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 10:50:20.385772 mmcb-avt-0.0.89/src/mmcb/
--rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.89/src/mmcb/__init__.py
--rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-11 14:41:48.000000 mmcb-avt-0.0.89/src/mmcb/common.py
--rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.89/src/mmcb/configure_environment.py
--rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.89/src/mmcb/dat2plot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.89/src/mmcb/dat2root.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33679 2023-05-10 15:18:59.000000 mmcb-avt-0.0.89/src/mmcb/detect.py
--rwx------   0 avt        (501) staff       (20)     3052 2023-05-11 14:44:06.000000 mmcb-avt-0.0.89/src/mmcb/dmm.py
--rw-r--r--   0 avt        (501) staff       (20)     4545 2023-05-12 10:00:32.000000 mmcb-avt-0.0.89/src/mmcb/dmm_interface.py
--rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.89/src/mmcb/iv.py
--rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.89/src/mmcb/lexicon.py
--rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.89/src/mmcb/liveplot.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.89/src/mmcb/log2dat.py
--rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.89/src/mmcb/peltier.py
--rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.89/src/mmcb/psuset.py
--rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.89/src/mmcb/psustat.py
--rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.89/src/mmcb/sense.py
--rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.89/src/mmcb/sensors.py
--rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.89/src/mmcb/sensors_mod.py
--rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.89/src/mmcb/sequence.py
--rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.89/src/mmcb/ult80.py
-drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-12 10:50:20.391787 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/
--rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/PKG-INFO
--rw-r--r--   0 avt        (501) staff       (20)      672 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/SOURCES.txt
--rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/dependency_links.txt
--rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/entry_points.txt
--rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/requires.txt
--rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-12 10:50:20.000000 mmcb-avt-0.0.89/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-17 14:46:21.216019 mmcb-avt-0.0.90/
+-rw-r--r--   0 avt        (501) staff       (20)    13827 2023-02-01 15:48:35.000000 mmcb-avt-0.0.90/LICENSE
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-17 14:46:21.215093 mmcb-avt-0.0.90/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)     7797 2023-05-12 10:49:39.000000 mmcb-avt-0.0.90/README.md
+-rw-r--r--   0 avt        (501) staff       (20)      104 2023-05-17 14:30:45.000000 mmcb-avt-0.0.90/pyproject.toml
+-rw-r--r--   0 avt        (501) staff       (20)       38 2023-05-17 14:46:21.216295 mmcb-avt-0.0.90/setup.cfg
+-rw-r--r--   0 avt        (501) staff       (20)     2591 2023-05-17 14:46:04.000000 mmcb-avt-0.0.90/setup.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-17 14:46:21.174008 mmcb-avt-0.0.90/src/
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-17 14:46:21.206995 mmcb-avt-0.0.90/src/mmcb/
+-rw-r--r--   0 avt        (501) staff       (20)        0 2022-05-29 13:37:50.000000 mmcb-avt-0.0.90/src/mmcb/__init__.py
+-rw-r--r--   0 avt        (501) staff       (20)    93158 2023-05-11 14:41:48.000000 mmcb-avt-0.0.90/src/mmcb/common.py
+-rw-r--r--   0 avt        (501) staff       (20)    32486 2023-02-22 19:41:25.000000 mmcb-avt-0.0.90/src/mmcb/configure_environment.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    14416 2023-03-16 13:06:31.000000 mmcb-avt-0.0.90/src/mmcb/dat2plot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     9078 2023-03-06 10:10:59.000000 mmcb-avt-0.0.90/src/mmcb/dat2root.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33782 2023-05-17 14:29:51.000000 mmcb-avt-0.0.90/src/mmcb/detect.py
+-rwx------   0 avt        (501) staff       (20)     3235 2023-05-17 14:42:59.000000 mmcb-avt-0.0.90/src/mmcb/dmm.py
+-rw-r--r--   0 avt        (501) staff       (20)     4688 2023-05-17 14:29:45.000000 mmcb-avt-0.0.90/src/mmcb/dmm_interface.py
+-rwxr-xr-x   0 avt        (501) staff       (20)   112129 2023-03-06 09:12:53.000000 mmcb-avt-0.0.90/src/mmcb/iv.py
+-rw-r--r--   0 avt        (501) staff       (20)    24909 2023-05-11 15:25:26.000000 mmcb-avt-0.0.90/src/mmcb/lexicon.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    12231 2023-03-08 10:55:33.000000 mmcb-avt-0.0.90/src/mmcb/liveplot.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7040 2023-03-08 10:54:40.000000 mmcb-avt-0.0.90/src/mmcb/log2dat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)     7889 2023-02-01 16:03:37.000000 mmcb-avt-0.0.90/src/mmcb/peltier.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    33621 2023-03-06 10:22:31.000000 mmcb-avt-0.0.90/src/mmcb/psuset.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    21883 2023-03-06 09:13:15.000000 mmcb-avt-0.0.90/src/mmcb/psustat.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    13517 2023-03-16 13:05:30.000000 mmcb-avt-0.0.90/src/mmcb/sense.py
+-rw-r--r--   0 avt        (501) staff       (20)    40226 2023-03-21 22:25:32.000000 mmcb-avt-0.0.90/src/mmcb/sensors.py
+-rw-r--r--   0 avt        (501) staff       (20)    40258 2023-03-16 14:01:16.000000 mmcb-avt-0.0.90/src/mmcb/sensors_mod.py
+-rw-r--r--   0 avt        (501) staff       (20)    17705 2023-03-08 09:27:13.000000 mmcb-avt-0.0.90/src/mmcb/sequence.py
+-rwxr-xr-x   0 avt        (501) staff       (20)    17659 2023-03-06 09:10:49.000000 mmcb-avt-0.0.90/src/mmcb/ult80.py
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-17 14:46:21.212838 mmcb-avt-0.0.90/src/mmcb_avt.egg-info/
+-rw-r--r--   0 avt        (501) staff       (20)     9020 2023-05-17 14:46:21.000000 mmcb-avt-0.0.90/src/mmcb_avt.egg-info/PKG-INFO
+-rw-r--r--   0 avt        (501) staff       (20)      694 2023-05-17 14:46:21.000000 mmcb-avt-0.0.90/src/mmcb_avt.egg-info/SOURCES.txt
+-rw-r--r--   0 avt        (501) staff       (20)        1 2023-05-17 14:46:21.000000 mmcb-avt-0.0.90/src/mmcb_avt.egg-info/dependency_links.txt
+-rw-r--r--   0 avt        (501) staff       (20)      330 2023-05-17 14:46:21.000000 mmcb-avt-0.0.90/src/mmcb_avt.egg-info/entry_points.txt
+-rw-r--r--   0 avt        (501) staff       (20)      226 2023-05-17 14:46:21.000000 mmcb-avt-0.0.90/src/mmcb_avt.egg-info/requires.txt
+-rw-r--r--   0 avt        (501) staff       (20)        5 2023-05-17 14:46:21.000000 mmcb-avt-0.0.90/src/mmcb_avt.egg-info/top_level.txt
+drwxr-xr-x   0 avt        (501) staff       (20)        0 2023-05-17 14:46:21.213739 mmcb-avt-0.0.90/tests/
+-rw-r--r--   0 avt        (501) staff       (20)      137 2023-05-14 12:24:42.000000 mmcb-avt-0.0.90/tests/test_lexicon.py
```

### Comparing `mmcb-avt-0.0.89/LICENSE` & `mmcb-avt-0.0.90/LICENSE`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/PKG-INFO` & `mmcb-avt-0.0.90/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.89
+Version: 0.0.90
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.89/README.md` & `mmcb-avt-0.0.90/README.md`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/setup.py` & `mmcb-avt-0.0.90/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="mmcb-avt",
-    version="0.0.89",
+    version="0.0.90",
     author="Alan Taylor, Manex Ormazabal",
     author_email="avt@hep.ph.liv.ac.uk",
     maintainer="Alan Taylor",
     maintainer_email="avt@hep.ph.liv.ac.uk",
     description="ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

### Comparing `mmcb-avt-0.0.89/src/mmcb/common.py` & `mmcb-avt-0.0.90/src/mmcb/common.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/configure_environment.py` & `mmcb-avt-0.0.90/src/mmcb/configure_environment.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/dat2plot.py` & `mmcb-avt-0.0.90/src/mmcb/dat2plot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/dat2root.py` & `mmcb-avt-0.0.90/src/mmcb/dat2root.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/detect.py` & `mmcb-avt-0.0.90/src/mmcb/detect.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,17 +797,17 @@
             response = ser.readline().lower()
         except serial.SerialException:
             print(f'cannot access serial port {port}')
         else:
             if b'keithley' in response:
                 try:
                     release_delay = 0.01
-                    parts = response.decode('utf-8').split(',')
-                    manufacturer = parts[0]
                     # ['KEITHLEY INSTRUMENTS', 'MODEL DMM6500', '04592428', '1.7.12b']
+                    parts = response.decode('utf-8').lower().split(',')
+                    manufacturer = parts[0].split()[0]
                     model = parts[1].split()[-1]
                     serial_number = parts[2]
                     detected = True
                     channels = ['']
                     settings = ser.get_settings()
                     retval = (
                         'instrument',
@@ -916,23 +916,24 @@
     detect devices present on the serial ports, that are attached via
     FTDI USB to RS232 adaptors
     """
     args = check_arguments()
 
     ports = [com.device for com in stlp.comports() if common.rs232_port_is_valid(com)]
     if not ports:
-        sys.exit('No usable serial ports found')
+        all_ports = ', '.join(com.device for com in stlp.comports())
+        sys.exit(f'No usable serial ports found: {all_ports}')
 
     tests = collections.OrderedDict(
         {
+            'dmm_6500': find_dmm_6500,
             'lvpsu': find_lvpsu,
             'lvpsu_hmp4040': find_lvpsu_hmp4040,
             'hvpsu': find_hvpsu,
             'hvpsu_2614b': find_hvpsu_2614b,
-            'dmm_6500': find_dmm_6500,
             'controller': find_controller,
             'controller_smc': find_controller_smc,
         }
     )
 
     # define serial port connection settings for each device
     # see https://pyserial.readthedocs.io/en/latest/pyserial_api.html
@@ -953,17 +954,17 @@
         },
         'hvpsu_2614b': {
             'baudrate': 57600,
             'xonxoff': False,
             'rtscts': False,
         },
         'dmm_6500': {
-            'baudrate': 57600,
+            'baudrate': 38400,
             'xonxoff': False,
-            'rtscts': True,
+            'rtscts': False,
         },
         'controller': {
             'baudrate': 19200,
             'xonxoff': False,
             'rtscts': False,
         },
         'controller_smc': {
```

### Comparing `mmcb-avt-0.0.89/src/mmcb/dmm.py` & `mmcb-avt-0.0.90/src/mmcb/dmm.py`

 * *Files 10% similar despite different names*

```diff
@@ -71,39 +71,47 @@
 
 def main():
     """ Read values from the Keithley DMM6500 """
 
     args = check_arguments()
 
     dmm = dmm_interface.Dmm6500()
+    if dmm.init_failed:
+        print('could not initialise serial port')
+        return 3
+
     configure = {
             'capacitance': dmm.configure_read_capacitance,
             'currentac': dmm.configure_read_ac_current,
             'currentdc': dmm.configure_read_dc_current,
             'resistance': dmm.configure_read_resistance,
             'temperature': dmm.configure_read_temperature,
             'voltagedc': dmm.configure_read_dc_voltage,
             'voltageac': dmm.configure_read_ac_voltage,
     }
 
     # AC quantities sometimes return None on the first attempt
     retries = 3
 
+    success = []
     for function, required in vars(args).items():
         if not required:
             continue
 
         configure[function]()
 
         value = None
         for _ in range(retries):
             value = dmm.read_value()
             if value is not None:
+                success.append(True)
                 break
             time.sleep(0.1)
 
         print(f'{function}, {common.si_prefix(value)}, {value}')
 
+    return 0 if any(success) else 3
+
 
 ##############################################################################
 if __name__ == '__main__':
     sys.exit(main())
```

### Comparing `mmcb-avt-0.0.89/src/mmcb/dmm_interface.py` & `mmcb-avt-0.0.90/src/mmcb/dmm_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,20 +72,24 @@
 
     try:
         _channel = _channels[0]
     except IndexError:
         pass
 
     def __init__(self):
-        self._ser = serial.Serial(port=self._channel.port)
-        self._finalizer = weakref.finalize(self, self._ser.close)
-        self._ser.apply_settings(self._channel.config)
-
-        self._ser.reset_input_buffer()
-        self._ser.reset_output_buffer()
+        try:
+            self._ser = serial.Serial(port=self._channel.port)
+        except OSError:
+            self.init_failed = True
+        else:
+            self.init_failed = False
+            self._finalizer = weakref.finalize(self, self._ser.close)
+            self._ser.apply_settings(self._channel.config)
+            self._ser.reset_input_buffer()
+            self._ser.reset_output_buffer()
 
     def remove(self):
         """manual garbage collection: close serial port"""
         self._finalizer()
 
     @property
     def removed(self):
```

### Comparing `mmcb-avt-0.0.89/src/mmcb/iv.py` & `mmcb-avt-0.0.90/src/mmcb/iv.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/lexicon.py` & `mmcb-avt-0.0.90/src/mmcb/lexicon.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/liveplot.py` & `mmcb-avt-0.0.90/src/mmcb/liveplot.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/log2dat.py` & `mmcb-avt-0.0.90/src/mmcb/log2dat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/peltier.py` & `mmcb-avt-0.0.90/src/mmcb/peltier.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/psuset.py` & `mmcb-avt-0.0.90/src/mmcb/psuset.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/psustat.py` & `mmcb-avt-0.0.90/src/mmcb/psustat.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/sense.py` & `mmcb-avt-0.0.90/src/mmcb/sense.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/sensors.py` & `mmcb-avt-0.0.90/src/mmcb/sensors.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/sensors_mod.py` & `mmcb-avt-0.0.90/src/mmcb/sensors_mod.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/sequence.py` & `mmcb-avt-0.0.90/src/mmcb/sequence.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb/ult80.py` & `mmcb-avt-0.0.90/src/mmcb/ult80.py`

 * *Files identical despite different names*

### Comparing `mmcb-avt-0.0.89/src/mmcb_avt.egg-info/PKG-INFO` & `mmcb-avt-0.0.90/src/mmcb_avt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmcb-avt
-Version: 0.0.89
+Version: 0.0.90
 Summary: ATLAS ITK Pixels Multi-Module Cycling Box environmental monitoring/control.
 Home-page: https://gitlab.ph.liv.ac.uk/avt/atlas-itk-pmmcb
 Author: Alan Taylor, Manex Ormazabal
 Author-email: avt@hep.ph.liv.ac.uk
 Maintainer: Alan Taylor
 Maintainer-email: avt@hep.ph.liv.ac.uk
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mmcb-avt-0.0.89/src/mmcb_avt.egg-info/SOURCES.txt` & `mmcb-avt-0.0.90/src/mmcb_avt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -23,8 +23,9 @@
 src/mmcb/sequence.py
 src/mmcb/ult80.py
 src/mmcb_avt.egg-info/PKG-INFO
 src/mmcb_avt.egg-info/SOURCES.txt
 src/mmcb_avt.egg-info/dependency_links.txt
 src/mmcb_avt.egg-info/entry_points.txt
 src/mmcb_avt.egg-info/requires.txt
-src/mmcb_avt.egg-info/top_level.txt
+src/mmcb_avt.egg-info/top_level.txt
+tests/test_lexicon.py
```

