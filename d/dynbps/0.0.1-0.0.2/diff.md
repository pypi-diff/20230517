# Comparing `tmp/dynbps-0.0.1.tar.gz` & `tmp/dynbps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dynbps-0.0.1.tar", last modified: Tue May 16 22:39:42 2023, max compression
+gzip compressed data, was "dist/dynbps-0.0.2.tar", last modified: Tue May 16 22:56:04 2023, max compression
```

## Comparing `dynbps-0.0.1.tar` & `dynbps-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 22:39:42.732050 dynbps-0.0.1/
--rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.1/LICENSE
--rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.1/MANIFEST.in
--rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 22:39:42.730993 dynbps-0.0.1/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      275 2023-05-16 22:34:41.000000 dynbps-0.0.1/README.md
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 22:39:42.713644 dynbps-0.0.1/dynbps/
--rw-r--r--   0 josephrilling   (501) staff       (20)     8969 2023-05-16 22:35:50.000000 dynbps-0.0.1/dynbps/BPS.py
--rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-16 22:35:50.000000 dynbps-0.0.1/dynbps/__init__.py
--rw-r--r--   0 josephrilling   (501) staff       (20)      646 2023-05-16 22:35:50.000000 dynbps-0.0.1/dynbps/_modidx.py
-drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 22:39:42.729218 dynbps-0.0.1/dynbps.egg-info/
--rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 22:39:42.000000 dynbps-0.0.1/dynbps.egg-info/PKG-INFO
--rw-r--r--   0 josephrilling   (501) staff       (20)      313 2023-05-16 22:39:42.000000 dynbps-0.0.1/dynbps.egg-info/SOURCES.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 22:39:42.000000 dynbps-0.0.1/dynbps.egg-info/dependency_links.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-16 22:39:42.000000 dynbps-0.0.1/dynbps.egg-info/entry_points.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.1/dynbps.egg-info/not-zip-safe
--rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-16 22:39:42.000000 dynbps-0.0.1/dynbps.egg-info/requires.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-16 22:39:42.000000 dynbps-0.0.1/dynbps.egg-info/top_level.txt
--rw-r--r--   0 josephrilling   (501) staff       (20)      958 2023-05-16 21:50:41.000000 dynbps-0.0.1/settings.ini
--rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-16 22:39:42.732508 dynbps-0.0.1/setup.cfg
--rw-rw-r--   0 josephrilling   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 dynbps-0.0.1/setup.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 22:56:04.724463 dynbps-0.0.2/
+-rw-r--r--   0 josephrilling   (501) staff       (20)    11357 2023-05-16 21:26:28.000000 dynbps-0.0.2/LICENSE
+-rw-rw-r--   0 josephrilling   (501) staff       (20)      111 2023-04-27 10:12:58.000000 dynbps-0.0.2/MANIFEST.in
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 22:56:04.723775 dynbps-0.0.2/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      275 2023-05-16 22:34:41.000000 dynbps-0.0.2/README.md
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 22:56:04.716801 dynbps-0.0.2/dynbps/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     9004 2023-05-16 22:54:02.000000 dynbps-0.0.2/dynbps/BPS.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)       22 2023-05-16 22:54:02.000000 dynbps-0.0.2/dynbps/__init__.py
+-rw-r--r--   0 josephrilling   (501) staff       (20)      646 2023-05-16 22:54:02.000000 dynbps-0.0.2/dynbps/_modidx.py
+drwxr-xr-x   0 josephrilling   (501) staff       (20)        0 2023-05-16 22:56:04.722672 dynbps-0.0.2/dynbps.egg-info/
+-rw-r--r--   0 josephrilling   (501) staff       (20)     1042 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/PKG-INFO
+-rw-r--r--   0 josephrilling   (501) staff       (20)      313 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/SOURCES.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/dependency_links.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)       34 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/entry_points.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        1 2023-05-16 21:36:56.000000 dynbps-0.0.2/dynbps.egg-info/not-zip-safe
+-rw-r--r--   0 josephrilling   (501) staff       (20)       35 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/requires.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)        7 2023-05-16 22:56:04.000000 dynbps-0.0.2/dynbps.egg-info/top_level.txt
+-rw-r--r--   0 josephrilling   (501) staff       (20)      830 2023-05-16 22:53:38.000000 dynbps-0.0.2/settings.ini
+-rw-r--r--   0 josephrilling   (501) staff       (20)       38 2023-05-16 22:56:04.724669 dynbps-0.0.2/setup.cfg
+-rw-rw-r--   0 josephrilling   (501) staff       (20)     2596 2023-04-27 10:12:58.000000 dynbps-0.0.2/setup.py
```

### Comparing `dynbps-0.0.1/LICENSE` & `dynbps-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.1/PKG-INFO` & `dynbps-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.1/dynbps/BPS.py` & `dynbps-0.0.2/dynbps/BPS.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,15 @@
         def chol(A):
             '''returns upper triangle of matrix'''
             return cholesky(A, lower = False)
         a = self.a_j[-1,:]
         A = self.A_j[-1,:]
         n = self.n_j[-1,0]
         delta = self.delta
+        mcmc_iter = self.mcmc_iter
         E_BPS = np.zeros(shape = [mcmc_iter, 1]) # posterior BPS mean
         V_BPS = np.zeros(shape = [mcmc_iter, 1]) # posterior BPS variance
         error = np.zeros(shape = [mcmc_iter, 1])
         mlike = np.zeros(shape = [mcmc_iter, 1])
         for i in range(self.mcmc_iter):
         # sample x(t + 1)
             lambda_ = np.sqrt(0.5 * delta[1] * n/np.random.gamma(shape = delta[1] * n/2))
```

### Comparing `dynbps-0.0.1/dynbps/_modidx.py` & `dynbps-0.0.2/dynbps/_modidx.py`

 * *Files identical despite different names*

### Comparing `dynbps-0.0.1/dynbps.egg-info/PKG-INFO` & `dynbps-0.0.2/dynbps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynbps
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python code for Dynamic BPS
 Home-page: https://github.com/josephrilling/dynbps
 Author: josephrilling
 Author-email: tun52698@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `dynbps-0.0.1/setup.py` & `dynbps-0.0.2/setup.py`

 * *Files identical despite different names*

