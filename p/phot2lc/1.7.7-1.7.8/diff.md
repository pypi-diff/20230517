# Comparing `tmp/phot2lc-1.7.7.tar.gz` & `tmp/phot2lc-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phot2lc-1.7.7.tar", last modified: Thu May  4 22:31:15 2023, max compression
+gzip compressed data, was "phot2lc-1.7.8.tar", last modified: Tue May 16 23:23:36 2023, max compression
```

## Comparing `phot2lc-1.7.7.tar` & `phot2lc-1.7.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-04 22:31:15.757616 phot2lc-1.7.7/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1058 2020-06-12 15:08:44.000000 phot2lc-1.7.7/LICENSE
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-04 22:31:15.757616 phot2lc-1.7.7/PKG-INFO
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      640 2020-06-14 20:06:06.000000 phot2lc-1.7.7/README.md
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)       38 2023-05-04 22:31:15.757616 phot2lc-1.7.7/setup.cfg
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1094 2023-05-04 22:30:00.000000 phot2lc-1.7.7/setup.py
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-04 22:31:15.757616 phot2lc-1.7.7/src/
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-04 22:31:15.757616 phot2lc-1.7.7/src/phot2lc/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2020-06-12 15:54:42.000000 phot2lc-1.7.7/src/phot2lc/__init__.py
--rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     2362 2023-05-04 22:29:04.000000 phot2lc-1.7.7/src/phot2lc/addstar
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      281 2023-02-22 04:21:11.000000 phot2lc-1.7.7/src/phot2lc/config.dat
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    83643 2023-05-04 22:29:21.000000 phot2lc-1.7.7/src/phot2lc/phot2lc
--rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      314 2023-04-29 00:26:01.000000 phot2lc-1.7.7/src/phot2lc/photconfig
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    17242 2023-02-22 04:27:41.000000 phot2lc-1.7.7/src/phot2lc/photfunc.py
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     9083 2023-02-01 21:25:50.000000 phot2lc-1.7.7/src/phot2lc/quicklook
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     4266 2022-11-30 00:07:41.000000 phot2lc-1.7.7/src/phot2lc/teledat.py
--rw-r--r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5861 2023-02-09 02:35:54.000000 phot2lc-1.7.7/src/phot2lc/ucm_utils.py
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    21673 2023-05-04 22:30:42.000000 phot2lc-1.7.7/src/phot2lc/version_history.txt
--rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5981 2020-11-15 20:21:32.000000 phot2lc-1.7.7/src/phot2lc/weldlc
-drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-04 22:31:15.757616 phot2lc-1.7.7/src/phot2lc.egg-info/
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-04 22:31:15.000000 phot2lc-1.7.7/src/phot2lc.egg-info/PKG-INFO
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      421 2023-05-04 22:31:15.000000 phot2lc-1.7.7/src/phot2lc.egg-info/SOURCES.txt
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        1 2023-05-04 22:31:15.000000 phot2lc-1.7.7/src/phot2lc.egg-info/dependency_links.txt
--rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        8 2023-05-04 22:31:15.000000 phot2lc-1.7.7/src/phot2lc.egg-info/top_level.txt
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-16 23:23:36.897299 phot2lc-1.7.8/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1058 2020-06-12 15:08:44.000000 phot2lc-1.7.8/LICENSE
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-16 23:23:36.897299 phot2lc-1.7.8/PKG-INFO
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      640 2020-06-14 20:06:06.000000 phot2lc-1.7.8/README.md
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)       38 2023-05-16 23:23:36.897299 phot2lc-1.7.8/setup.cfg
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1094 2023-05-16 23:23:12.000000 phot2lc-1.7.8/setup.py
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-16 23:23:36.893299 phot2lc-1.7.8/src/
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-16 23:23:36.897299 phot2lc-1.7.8/src/phot2lc/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2020-06-12 15:54:42.000000 phot2lc-1.7.8/src/phot2lc/__init__.py
+-rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     2362 2023-05-04 22:29:04.000000 phot2lc-1.7.8/src/phot2lc/addstar
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      273 2023-05-16 23:21:56.000000 phot2lc-1.7.8/src/phot2lc/config.dat
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    84047 2023-05-16 23:21:40.000000 phot2lc-1.7.8/src/phot2lc/phot2lc
+-rwxrwxrwx   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      314 2023-04-29 00:26:01.000000 phot2lc-1.7.8/src/phot2lc/photconfig
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    17242 2023-02-22 04:27:41.000000 phot2lc-1.7.8/src/phot2lc/photfunc.py
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     9083 2023-02-01 21:25:50.000000 phot2lc-1.7.8/src/phot2lc/quicklook
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     4266 2022-11-30 00:07:41.000000 phot2lc-1.7.8/src/phot2lc/teledat.py
+-rw-r--r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5861 2023-02-09 02:35:54.000000 phot2lc-1.7.8/src/phot2lc/ucm_utils.py
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)    22556 2023-05-16 23:09:32.000000 phot2lc-1.7.8/src/phot2lc/version_history.txt
+-rwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     5981 2020-11-15 20:21:32.000000 phot2lc-1.7.8/src/phot2lc/weldlc
+drwxrwxr-x   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        0 2023-05-16 23:23:36.897299 phot2lc-1.7.8/src/phot2lc.egg-info/
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)     1219 2023-05-16 23:23:36.000000 phot2lc-1.7.8/src/phot2lc.egg-info/PKG-INFO
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)      421 2023-05-16 23:23:36.000000 phot2lc-1.7.8/src/phot2lc.egg-info/SOURCES.txt
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        1 2023-05-16 23:23:36.000000 phot2lc-1.7.8/src/phot2lc.egg-info/dependency_links.txt
+-rw-rw-r--   0 zachvanderbosch  (1000) zachvanderbosch  (1000)        8 2023-05-16 23:23:36.000000 phot2lc-1.7.8/src/phot2lc.egg-info/top_level.txt
```

### Comparing `phot2lc-1.7.7/LICENSE` & `phot2lc-1.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.7/PKG-INFO` & `phot2lc-1.7.8/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phot2lc
-Version: 1.7.7
+Version: 1.7.8
 Summary: Light curve extraction
 Home-page: https://github.com/zvanderbosch/phot2lc
 Author: Zach Vanderbosch
 Author-email: zvanderbosch@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

### Comparing `phot2lc-1.7.7/README.md` & `phot2lc-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.7/setup.py` & `phot2lc-1.7.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phot2lc",
-    version="1.7.7",
+    version="1.7.8",
     author="Zach Vanderbosch",
     author_email="zvanderbosch@gmail.com",
     description="Light curve extraction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zvanderbosch/phot2lc",
     packages=setuptools.find_packages('src'),
```

### Comparing `phot2lc-1.7.7/src/phot2lc/addstar` & `phot2lc-1.7.8/src/phot2lc/addstar`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.7/src/phot2lc/phot2lc` & `phot2lc-1.7.8/src/phot2lc/phot2lc`

 * *Files 0% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     mpl.use('QT5agg')
 else:                          # Other
     mpl.use('TKagg')
 
 
 # Import Standard Packages
 import os
+import pwd
 import json
 import argparse
 import warnings
 import itertools
 import numpy as np
 import pandas as pd
 from glob import glob
@@ -109,40 +110,41 @@
 config_path = os.path.dirname(os.path.realpath(phot2lc.teledat.__file__))
 config_dat = []
 with open(config_path + "/config.dat") as f:
     for l in f.readlines():
         config_dat.append(l.strip("\n").split("=")[-1].strip())
 
 
-# Name for whoever is running phot2lc
-author = config_dat[0]
 # File containing the list of images being analyzed
 list_name = config_dat[1]
 # Optional File containing initial guesses at source locations.
 tloc_name = config_dat[2]
 # Base filename for photometry output from pipelines
 phot_basename = config_dat[3]
 # Path to file containing object names + coordinates
 star_dat_filename = config_dat[4] 
 
 
 
 # Defualt arguments for argparse
+default_author = config_dat[0]
 default_telescope = config_dat[5]
 default_source = config_dat[6]
 default_image = None if config_dat[7] == 'None' else config_dat[7]
 default_object = None if config_dat[8] == 'None' else config_dat[8]
 
 
 #############################################################
 ## Generate arguments for command line parsing
 
 parser = argparse.ArgumentParser()
 parser.add_argument('-c', '--codes',action='store_true',
                     help="If invoked, print list of available telescope codes.")
+parser.add_argument('-a', '--author',type=str,default=default_author,
+                    help="Name of phot2lc user.")
 parser.add_argument('-t', '--telescope',type=str,default=default_telescope,
                     help="Code name for telescope used.")
 parser.add_argument('-s', '--source',type=str,default=default_source,
                     help="Source of photometry (ccd_hsp or maestro)")
 parser.add_argument('-p', '--photname',type=str,default=phot_basename,
                     help="Base filename for photometry output files.")
 parser.add_argument('-i', '--image',type=str,default=default_image,
@@ -150,14 +152,20 @@
 parser.add_argument('-o', '--object',type=str,default=default_object,
                     help="Name of object. If None, get object from FITS header.")
 parser.add_argument('-b', '--barycorr',action='store_false',
                     help="If invoked, do NOT perform barycentric corrections.")
 args = parser.parse_args()
 
 
+# Set author to system username if selected
+author = args.author
+if author == 'sys-user':
+	author = pwd.getpwuid(os.getuid()).pw_name
+
+
 #############################################################
 # Perform checks on command line inputs
 
 # Load list containing telescope information
 telinfo = get_telinfo()
 
 # Currently supported codes, telescopes, instruments
@@ -326,19 +334,28 @@
             else:
                 break
     df = pd.read_csv(phot_names[0],
         header=None, delim_whitespace=True, skiprows=skip_rows)
     Nphotobj = int((len(df.columns)-7)/14)
 
     # Generate column names that are consistent with HiPERCAM colnames
-    baseColnames = ['name','MJD','MJDok','Exptim','CCD','mfwhm','mbeta']
-    objColnames = ['naper','x','y','xm','ym','exm','eym','counts','countse',
-    'sky','nsky','nrej','worst','flag']
-
-    allobjColnames = [['{}_{}'.format(cname,x+1) for cname in objColnames] for x in range(Nphotobj)]
+    baseColnames = [
+    	'name','MJD','MJDok','Exptim',
+    	'CCD','mfwhm','mbeta'
+    ]
+    objColnames = [
+    	'naper','x','y','xm','ym','exm','eym',
+    	'counts','countse','sky','nsky','nrej',
+    	'worst','flag'
+    ]
+
+    allobjColnames = [
+    	['{}_{}'.format(cname,x+1) for cname in objColnames] 
+    	for x in range(Nphotobj)
+    ]
     colnames = baseColnames + list(itertools.chain.from_iterable(allobjColnames))
     df.columns = colnames
 
     # Remove any rows containing NaN-valued counts
     check_columns = [c for c in df.columns if "counts_" in c]
     df = df.dropna(subset=check_columns).reset_index(drop=True)
 
@@ -458,18 +475,22 @@
         tloc[i,1] = float(xy[1].strip()) + float(xyoff[1].strip())
 
 
 # Check to make sure this object has an entry in stars.dat file
 star_dat = pd.read_csv(star_dat_filename,header=None,delim_whitespace=True,dtype=str)
 obj_idx = star_dat.index[star_dat.iloc[:,0] == obj_name]
 if len(obj_idx) == 0:
-    print("\nWARNING: No objects by name of '{}' found in '{}'\n".format(obj_name,star_dat_filename))
+    print("\nWARNING: No objects by name of '{}' found in '{}'\n".format(
+    	obj_name,star_dat_filename)
+    )
     sys.exit(1)
 elif len(obj_idx) > 1:
-    print("\nWARNING: Multiple entries for '{}' found in '{}'\n".format(obj_name,star_dat_filename))
+    print("\nWARNING: Multiple entries for '{}' found in '{}'\n".format(
+    	obj_name,star_dat_filename)
+    )
     sys.exit(1)
 
 
 #############################################################
 # Show the first image along with marked targets/comps
 # Get Data & Header Info for first image
 if psource == 'ucm':
@@ -512,23 +533,34 @@
 
 # Show the first image
 im.imshow(image0, cmap='gray',vmin=vmin0, vmax=vmax0)
 
 # Plot marker for each object
 for i in range(len(tloc)):
     if i == 0:
-        im.plot(tloc[i,0],tloc[i,1],
-                ls='None',marker='o',ms=13,mew=2.0,mec='c',mfc='None')
-        im.text(tloc[i,0],tloc[i,1]+0.055*imrows,'Target',
-                ha='center',fontsize=12,**fonta)
+        im.plot(
+        	tloc[i,0],tloc[i,1],
+            ls='None',marker='o',ms=13,
+            mew=2.0,mec='c',mfc='None'
+        )
+        im.text(
+        	tloc[i,0],tloc[i,1]+0.055*imrows,
+        	'Target',ha='center',fontsize=12,**fonta
+        )
     else:
-        im.plot(tloc[i,0],tloc[i,1],
-                ls='None',marker='o',ms=13,mew=2.0,mec='m',mfc='None')
-        im.text(tloc[i,0],tloc[i,1]+0.055*imrows,'Comp {}'.format(i),
-                ha='center',fontsize=12,**fonta)
+        im.plot(
+        	tloc[i,0],tloc[i,1],
+            ls='None',marker='o',ms=13,
+            mew=2.0,mec='m',mfc='None'
+        )
+        im.text(
+        	tloc[i,0],tloc[i,1]+0.055*imrows,
+        	'Comp {}'.format(i),
+            ha='center',fontsize=12,**fonta
+        )
 
 # Make Axes invisible
 plt.axis("off")
 
 # Add title
 titleim = '{}'.format(fits_list[0].split("/")[-1])
 im.set_title(titleim,loc='center',fontsize=14,**fontb)
```

### Comparing `phot2lc-1.7.7/src/phot2lc/photfunc.py` & `phot2lc-1.7.8/src/phot2lc/photfunc.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.7/src/phot2lc/quicklook` & `phot2lc-1.7.8/src/phot2lc/quicklook`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.7/src/phot2lc/teledat.py` & `phot2lc-1.7.8/src/phot2lc/teledat.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.7/src/phot2lc/ucm_utils.py` & `phot2lc-1.7.8/src/phot2lc/ucm_utils.py`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.7/src/phot2lc/version_history.txt` & `phot2lc-1.7.8/src/phot2lc/version_history.txt`

 * *Files 2% similar despite different names*

```diff
@@ -546,15 +546,33 @@
 ---------------------------
 > Better handling of NaN values in HiPERCAM and 
   ULTRACAM output.
 > Better information print out from the addstar 
   command line function.
 
 
-
+ Version 1.7.8 (2023 May 16)
+----------------------------
+> Changed how the light curve "author" is handled. The
+  default now is to use your system username, which
+  happens when the "author" parameter in the config.dat
+  file is set to "sys-user". You can change this parameter
+  to any custom value you like by running the photconfig
+  script as usual, or there is now a command line option
+  -a/--author for phot2lc which allows you to override 
+  the value in the config.dat file, e.g.:
+  
+      phot2lc --author 'Zach Vanderbosch'
+      
+  This update makes it easier for multiple people to use
+  the same phot2lc installation, e.g. on a computer that
+  a whole research group may use to store and reduce 
+  their data. Now, different users no longer have to run
+  the photconfig script to change the author name in order
+  to get the correct author metadata into the .lc file.
```

### Comparing `phot2lc-1.7.7/src/phot2lc/weldlc` & `phot2lc-1.7.8/src/phot2lc/weldlc`

 * *Files identical despite different names*

### Comparing `phot2lc-1.7.7/src/phot2lc.egg-info/PKG-INFO` & `phot2lc-1.7.8/src/phot2lc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phot2lc
-Version: 1.7.7
+Version: 1.7.8
 Summary: Light curve extraction
 Home-page: https://github.com/zvanderbosch/phot2lc
 Author: Zach Vanderbosch
 Author-email: zvanderbosch@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
```

