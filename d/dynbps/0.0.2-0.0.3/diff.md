# Comparing `tmp/dynbps-0.0.2.tar.gz` & `tmp/dynbps-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynbps-0.0.2.tar", last modified: Tue May 16 22:56:04 2023, max compression
+gzip compressed data, was "dist/dynbps-0.0.3.tar", last modified: Tue May 16 23:07:54 2023, max compression
```

## Comparing `dynbps-0.0.2.tar` & `dynbps-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 22:56:04.724463 dynbps-0.0.2/
--rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.2/LICENSE
--rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.2/MANIFEST.in
--rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 22:56:04.723775 dynbps-0.0.2/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      275 2023-05-16 22:34:41.000000 dynbps-0.0.2/README.md
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 22:56:04.716801 dynbps-0.0.2/dynbps/
--rw-r--r--   0 josephrilling   (501) staff       (20)     9004 2023-05-16 22:54:02.000000 dynbps-0.0.2/dynbps/BPS.py
--rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-16 22:54:02.000000 dynbps-0.0.2/dynbps/__init__.py
--rw-r--r--   0 josephrilling   (501) staff       (20)      646 2023-05-16 22:54:02.000000 dynbps-0.0.2/dynbps/_modidx.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 22:56:04.722672 dynbps-0.0.2/dynbps.egg-info/
--rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      313 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/SOURCES.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/dependency_links.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/entry_points.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.2/dynbps.egg-info/not-zip-safe
--rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/requires.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/top_level.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-16 22:53:38.000000 dynbps-0.0.2/settings.ini
--rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-16 22:56:04.724669 dynbps-0.0.2/setup.cfg
--rw-rw-r--   0 josephrilling   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 dynbps-0.0.2/setup.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 23:07:54.732763 dynbps-0.0.3/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.3/LICENSE
+-rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.3/MANIFEST.in
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 23:07:54.732203 dynbps-0.0.3/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      275 2023-05-16 22:34:41.000000 dynbps-0.0.3/README.md
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 23:07:54.720860 dynbps-0.0.3/dynbps/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     9023 2023-05-16 23:06:13.000000 dynbps-0.0.3/dynbps/BPS.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-16 23:06:13.000000 dynbps-0.0.3/dynbps/__init__.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)      646 2023-05-16 23:06:13.000000 dynbps-0.0.3/dynbps/_modidx.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 23:07:54.731301 dynbps-0.0.3/dynbps.egg-info/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      313 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/SOURCES.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/dependency_links.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/entry_points.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.3/dynbps.egg-info/not-zip-safe
+-rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/requires.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-16 23:07:54.000000 dynbps-0.0.3/dynbps.egg-info/top_level.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-16 23:05:52.000000 dynbps-0.0.3/settings.ini
+-rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-16 23:07:54.732927 dynbps-0.0.3/setup.cfg
+-rw-rw-r--   0 josephrilling   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 dynbps-0.0.3/setup.py
```

### Comparing `dynbps-0.0.2/LICENSE` & `dynbps-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.2/PKG-INFO` & `dynbps-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.2/dynbps/BPS.py` & `dynbps-0.0.3/dynbps/BPS.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,14 +160,15 @@
             '''returns upper triangle of matrix'''
             return cholesky(A, lower = False)
         a = self.a_j[-1,:]
         A = self.A_j[-1,:]
         n = self.n_j[-1,0]
         delta = self.delta
         mcmc_iter = self.mcmc_iter
+        p = self.p
         E_BPS = np.zeros(shape = [mcmc_iter, 1]) # posterior BPS mean
         V_BPS = np.zeros(shape = [mcmc_iter, 1]) # posterior BPS variance
         error = np.zeros(shape = [mcmc_iter, 1])
         mlike = np.zeros(shape = [mcmc_iter, 1])
         for i in range(self.mcmc_iter):
         # sample x(t + 1)
             lambda_ = np.sqrt(0.5 * delta[1] * n/np.random.gamma(shape = delta[1] * n/2))
```

### Comparing `dynbps-0.0.2/dynbps/_modidx.py` & `dynbps-0.0.3/dynbps/_modidx.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.2/dynbps.egg-info/PKG-INFO` & `dynbps-0.0.3/dynbps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.2/settings.ini` & `dynbps-0.0.3/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = dynbps
 lib_name = dynbps
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = dynbps
 nbs_path = nbs
 recursive = True
```

### Comparing `dynbps-0.0.2/setup.py` & `dynbps-0.0.3/setup.py`

 * *Files identical despite different names*

