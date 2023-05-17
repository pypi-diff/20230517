# Comparing `tmp/mmis-1.36.tar.gz` & `tmp/mmis-1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mmis-1.36.tar", last modified: Sun Aug  8 14:59:00 2021, max compression
+gzip compressed data, was "dist/mmis-1.37.tar", last modified: Thu Feb 17 02:42:22 2022, max compression
```

## Comparing `mmis-1.36.tar` & `mmis-1.37.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-08 14:59:00.000000 mmis-1.36/
--rw-r--r--   0 root         (0) root         (0)      248 2021-08-08 14:59:00.000000 mmis-1.36/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      796 2020-05-19 13:37:20.000000 mmis-1.36/README.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-08 14:59:00.000000 mmis-1.36/mmis/
--rw-r--r--   0 root         (0) root         (0)     6033 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Clock.py
--rw-r--r--   0 root         (0) root         (0)    36233 2021-05-03 08:44:39.000000 mmis-1.36/mmis/CryoHeater.py
--rw-r--r--   0 root         (0) root         (0)     4497 2021-05-12 11:31:20.000000 mmis-1.36/mmis/DebugFunctions.py
--rw-r--r--   0 root         (0) root         (0)    64996 2021-07-13 12:41:09.000000 mmis-1.36/mmis/DualHeater.py
--rw-r--r--   0 root         (0) root         (0)    59247 2021-05-12 08:26:38.000000 mmis-1.36/mmis/DualHeater_default.py
--rw-r--r--   0 root         (0) root         (0)     4925 2021-08-08 14:58:13.000000 mmis-1.36/mmis/Functions.py
--rw-r--r--   0 root         (0) root         (0)    76279 2021-08-08 14:48:56.000000 mmis-1.36/mmis/GUI.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-08 14:59:00.000000 mmis-1.36/mmis/Images/
--rw-r--r--   0 root         (0) root         (0)      922 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/Connected.png
--rw-r--r--   0 root         (0) root         (0)    47718 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/DEMOico.ico
--rw-r--r--   0 root         (0) root         (0)      758 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/Disconnected.png
--rw-r--r--   0 root         (0) root         (0)    41021 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/HZlogo.png
--rw-r--r--   0 root         (0) root         (0)    24924 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/Logo.png
--rw-r--r--   0 root         (0) root         (0)     9898 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/MMIstart.png
--rw-r--r--   0 root         (0) root         (0)     3072 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/Thumbs.db
--rw-r--r--   0 root         (0) root         (0)      674 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/graph.png
--rw-r--r--   0 root         (0) root         (0)     3628 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/liquid-nitrogen.png
--rw-r--r--   0 root         (0) root         (0)      730 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Images/warning.png
--rw-r--r--   0 root         (0) root         (0)    41322 2021-05-03 08:44:39.000000 mmis-1.36/mmis/LiqN2Control.py
--rw-r--r--   0 root         (0) root         (0)    11060 2021-05-03 08:44:39.000000 mmis-1.36/mmis/RealTimeClock.py
--rw-r--r--   0 root         (0) root         (0)    92209 2021-06-02 09:35:20.000000 mmis-1.36/mmis/SampleHeater.py
--rw-r--r--   0 root         (0) root         (0)    13208 2021-05-03 08:44:39.000000 mmis-1.36/mmis/Softwareupdate.py
--rw-r--r--   0 root         (0) root         (0)     1056 2021-05-12 11:24:25.000000 mmis-1.36/mmis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2323 2021-05-03 08:44:40.000000 mmis-1.36/mmis/startup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-08-08 14:59:00.000000 mmis-1.36/mmis.egg-info/
--rw-r--r--   0 root         (0) root         (0)      248 2021-08-08 14:59:00.000000 mmis-1.36/mmis.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      658 2021-08-08 14:59:00.000000 mmis-1.36/mmis.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-08-08 14:59:00.000000 mmis-1.36/mmis.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2021-08-08 14:59:00.000000 mmis-1.36/mmis.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-08-08 14:59:00.000000 mmis-1.36/mmis.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-08-08 14:59:00.000000 mmis-1.36/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      555 2021-08-08 14:49:16.000000 mmis-1.36/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 02:42:22.000000 mmis-1.37/
+-rw-r--r--   0 root         (0) root         (0)      248 2022-02-17 02:42:22.000000 mmis-1.37/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      796 2022-02-02 04:55:56.000000 mmis-1.37/README.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 02:42:22.000000 mmis-1.37/mmis/
+-rw-r--r--   0 root         (0) root         (0)     6033 2022-02-02 04:55:57.000000 mmis-1.37/mmis/Clock.py
+-rw-r--r--   0 root         (0) root         (0)    36233 2022-02-02 04:55:57.000000 mmis-1.37/mmis/CryoHeater.py
+-rw-r--r--   0 root         (0) root         (0)     4497 2022-02-02 04:55:57.000000 mmis-1.37/mmis/DebugFunctions.py
+-rw-r--r--   0 root         (0) root         (0)    64996 2022-02-02 04:55:57.000000 mmis-1.37/mmis/DualHeater.py
+-rw-r--r--   0 root         (0) root         (0)    59247 2022-02-02 04:55:57.000000 mmis-1.37/mmis/DualHeater_default.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2022-02-02 04:55:57.000000 mmis-1.37/mmis/Functions.py
+-rw-r--r--   0 root         (0) root         (0)    76279 2022-02-17 02:39:12.000000 mmis-1.37/mmis/GUI.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 02:42:22.000000 mmis-1.37/mmis/Images/
+-rw-r--r--   0 root         (0) root         (0)      922 2022-02-02 04:55:57.000000 mmis-1.37/mmis/Images/Connected.png
+-rw-r--r--   0 root         (0) root         (0)    47718 2022-02-02 04:55:57.000000 mmis-1.37/mmis/Images/DEMOico.ico
+-rw-r--r--   0 root         (0) root         (0)      758 2022-02-02 04:55:57.000000 mmis-1.37/mmis/Images/Disconnected.png
+-rw-r--r--   0 root         (0) root         (0)    41021 2022-02-02 04:55:57.000000 mmis-1.37/mmis/Images/HZlogo.png
+-rw-r--r--   0 root         (0) root         (0)    24924 2022-02-02 04:55:58.000000 mmis-1.37/mmis/Images/Logo.png
+-rw-r--r--   0 root         (0) root         (0)     9898 2022-02-02 04:55:58.000000 mmis-1.37/mmis/Images/MMIstart.png
+-rw-r--r--   0 root         (0) root         (0)     3072 2022-02-02 04:55:58.000000 mmis-1.37/mmis/Images/Thumbs.db
+-rw-r--r--   0 root         (0) root         (0)      674 2022-02-02 04:55:57.000000 mmis-1.37/mmis/Images/graph.png
+-rw-r--r--   0 root         (0) root         (0)     3628 2022-02-02 04:55:58.000000 mmis-1.37/mmis/Images/liquid-nitrogen.png
+-rw-r--r--   0 root         (0) root         (0)      730 2022-02-02 04:55:58.000000 mmis-1.37/mmis/Images/warning.png
+-rw-r--r--   0 root         (0) root         (0)    41322 2022-02-02 04:55:57.000000 mmis-1.37/mmis/LiqN2Control.py
+-rw-r--r--   0 root         (0) root         (0)    11060 2022-02-02 04:55:57.000000 mmis-1.37/mmis/RealTimeClock.py
+-rw-r--r--   0 root         (0) root         (0)    92207 2022-02-17 02:31:18.000000 mmis-1.37/mmis/SampleHeater.py
+-rw-r--r--   0 root         (0) root         (0)    13208 2022-02-02 04:55:57.000000 mmis-1.37/mmis/Softwareupdate.py
+-rw-r--r--   0 root         (0) root         (0)     1056 2022-02-02 04:55:57.000000 mmis-1.37/mmis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2323 2022-02-02 04:55:57.000000 mmis-1.37/mmis/startup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-02-17 02:42:22.000000 mmis-1.37/mmis.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      248 2022-02-17 02:42:21.000000 mmis-1.37/mmis.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      658 2022-02-17 02:42:21.000000 mmis-1.37/mmis.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-02-17 02:42:21.000000 mmis-1.37/mmis.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2022-02-17 02:42:21.000000 mmis-1.37/mmis.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2022-02-17 02:42:21.000000 mmis-1.37/mmis.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2022-02-17 02:42:22.000000 mmis-1.37/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      555 2022-02-17 02:41:41.000000 mmis-1.37/setup.py
```

### Comparing `mmis-1.36/README.txt` & `mmis-1.37/README.txt`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Clock.py` & `mmis-1.37/mmis/Clock.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/CryoHeater.py` & `mmis-1.37/mmis/CryoHeater.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/DebugFunctions.py` & `mmis-1.37/mmis/DebugFunctions.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/DualHeater.py` & `mmis-1.37/mmis/DualHeater.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/DualHeater_default.py` & `mmis-1.37/mmis/DualHeater_default.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Functions.py` & `mmis-1.37/mmis/Functions.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/GUI.py` & `mmis-1.37/mmis/GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import memcache
 import distro
 import matplotlib.pyplot as plt
 from pandas import DataFrame
 import csv
 import warnings
 
-Version = 'v1.36' # Keep changing the version number here everytime with the new release
+Version = 'v1.37' # Keep changing the version number here everytime with the new release
 warnings.filterwarnings("ignore") # Ignores all the warnings
 
 class DataAnalysis(wx.Panel):
     '''Data Analysis Class is used to import the log file and plot the graphs.
        Also used to downsample the logfile
        inputs: Logfile with extension .CSV
        outputs: Plots of selected Parameters
```

### Comparing `mmis-1.36/mmis/Images/Connected.png` & `mmis-1.37/mmis/Images/Connected.png`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Images/DEMOico.ico` & `mmis-1.37/mmis/Images/DEMOico.ico`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Images/Disconnected.png` & `mmis-1.37/mmis/Images/Disconnected.png`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Images/HZlogo.png` & `mmis-1.37/mmis/Images/HZlogo.png`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Images/Logo.png` & `mmis-1.37/mmis/Images/Logo.png`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Images/MMIstart.png` & `mmis-1.37/mmis/Images/MMIstart.png`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Images/Thumbs.db` & `mmis-1.37/mmis/Images/Thumbs.db`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Images/graph.png` & `mmis-1.37/mmis/Images/graph.png`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Images/liquid-nitrogen.png` & `mmis-1.37/mmis/Images/liquid-nitrogen.png`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/Images/warning.png` & `mmis-1.37/mmis/Images/warning.png`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/LiqN2Control.py` & `mmis-1.37/mmis/LiqN2Control.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/RealTimeClock.py` & `mmis-1.37/mmis/RealTimeClock.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/SampleHeater.py` & `mmis-1.37/mmis/SampleHeater.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         
         self.button1 = wx.Button(self, label="Start Calibration", pos=(640, 20), size = (140,40), id = -1)
         self.Bind(wx.EVT_BUTTON, self.ON_CALIBRATE_R0, self.button1)
         self.button1.Bind(wx.EVT_UPDATE_UI, self.on_update_pause_button)
         self.button1.SetForegroundColour('black')
         
         self.lblname3 = wx.StaticText(self, label = "T-Max(C):", pos = (40,140))
-        self.SET_Tmax = wx.SpinCtrlDouble(self, size=(160,40), min = 0, max = 800, inc = 0.1, value='800.0', pos = (200,130))
+        self.SET_Tmax = wx.SpinCtrlDouble(self, size=(160,40), min = 0, max = 1200, inc = 0.1, value='1200.0', pos = (200,130))
         self.SET_Tmax.SetDigits(3)
         self.SET_Tmax.SetBackgroundColour('white')
 
         self.button3 = wx.Button(self, label="Set", pos=(380, 130), size = (100,40), id = -1)
         self.Bind(wx.EVT_BUTTON, self.ON_SET_TMAX,self.button3)
         self.button3.SetForegroundColour('black')
         self.button3.SetBackgroundColour(wx.Colour(211,211,211))
@@ -777,15 +777,15 @@
         self.five.SetFont(self.font1)
         self.grid.Add(self.five, pos=(3,1))
 
         # Static text and num control box -  to set the value of temperature
         self.button6 = wx.Button(self, label = 'Set(\u00b0C)', size = (57,35), id=5)
         self.button6.Bind(wx.EVT_BUTTON, self.SetResistance)
         self.button6.SetBackgroundColour(wx.Colour(211,211,211))
-        self.one = wx.SpinCtrlDouble(self, size=(140,-1), min =-300, max = 800, inc = 0.1, value='80.00')
+        self.one = wx.SpinCtrlDouble(self, size=(140,-1), min =-300, max = 1200, inc = 0.1, value='80.00')
         self.one.SetDigits(3)
         self.one.SetBackgroundColour('white')
 
         self.button7 = wx.Button(self, label = 'Set(mW)', size = (65,35), id=7)
         self.button7.Bind(wx.EVT_BUTTON, self.SetPower)
         self.button7.SetBackgroundColour(wx.Colour(211,211,211))
         self.six = wx.SpinCtrlDouble(self, size=(140,-1), min =0, max = 50, inc = 0.1, value='1.0')
@@ -798,15 +798,15 @@
         self.seven = wx.SpinCtrlDouble(self, size=(140,-1), min =-100, max = 100, inc = 0.1, value='10.0')
         self.seven.SetDigits(3)
         self.seven.SetBackgroundColour('white')
 
         self.button11 = wx.Button(self, label = 'set end(\u00b0C)', size = (90,30), id=15) # Set set point temperature
         self.button11.Bind(wx.EVT_BUTTON, self.SetFinalTemperature)
         self.button11.SetBackgroundColour(wx.Colour(211,211,211))
-        self.eight = wx.SpinCtrlDouble(self, size=(140,-1), min =-300, max = 800, inc = 0.1, value='80.00')
+        self.eight = wx.SpinCtrlDouble(self, size=(140,-1), min =-300, max = 1200, inc = 0.1, value='80.00')
         self.eight.SetDigits(3)
         self.eight.SetBackgroundColour('white')
 
         # Static text and text control box - set the value to display the number of values on X -axis
         self.lblname3 = wx.StaticText(self, label = "X-Scale")
         self.grid.Add(self.lblname3, pos = (1,0))
         self.three = wx.TextCtrl(self, id = 6, size = (70,30), style = wx.TE_PROCESS_ENTER)
@@ -1374,15 +1374,15 @@
         self.dpi = 60
         self.fig = Figure((5.0, 5.1), dpi = self.dpi)
 
         self.axes = self.fig.add_subplot(111)
         self.axes.set_facecolor('black')
         self.axes.set_title('Temperature acquisition', size = 15)
         self.axes.set_xlabel('Samples', size = 12)
-        self.axes.set_ylabel('Ambient Temperature (C)', size = 15)
+        self.axes.set_ylabel('Sample Heater (C)', size = 15)
 
         pylab.setp(self.axes.get_xticklabels(), fontsize=12)
         pylab.setp(self.axes.get_yticklabels(), fontsize=12)
         
         self.plot_data = self.axes.plot(
             self.data,
             linewidth=1,
```

### Comparing `mmis-1.36/mmis/Softwareupdate.py` & `mmis-1.37/mmis/Softwareupdate.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/__init__.py` & `mmis-1.37/mmis/__init__.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis/startup.py` & `mmis-1.37/mmis/startup.py`

 * *Files identical despite different names*

### Comparing `mmis-1.36/mmis.egg-info/SOURCES.txt` & `mmis-1.37/mmis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmis-1.36/setup.py` & `mmis-1.37/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 #with open("README.md", "r") as fh:
     #long_description = fh.read()
 
 setuptools.setup(
     name='mmis',
-    version='1.36',
+    version='1.37',
     author='Rajeev Bheemireddy TUDelft-DEMO',
     description='control software for the Modular Microscope Instrument',
     #long_description=long_description,
     packages=['mmis'],
     #download_url=['https://homepage.tudelft.nl/6w77j/MMI/MMI.tar.gz'],
     package_data={'mmis':['Images/*.*']},
     install_requires=['python-memcached', 'pyPubSub', 'distro', 'beautifulsoup4'],
```

