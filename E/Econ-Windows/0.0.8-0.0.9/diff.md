# Comparing `tmp/Econ_Windows-0.0.8.tar.gz` & `tmp/Econ_Windows-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Econ_Windows-0.0.8.tar", last modified: Wed May 17 11:51:41 2023, max compression
+gzip compressed data, was "Econ_Windows-0.0.9.tar", last modified: Wed May 17 11:56:26 2023, max compression
```

## Comparing `Econ_Windows-0.0.8.tar` & `Econ_Windows-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 11:51:41.444245 Econ_Windows-0.0.8/
--rw-rw-rw-   0        0        0    10998 2023-05-17 11:50:33.000000 Econ_Windows-0.0.8/Econ_Windows.cpp
-drwxrwxrwx   0        0        0        0 2023-05-17 11:51:41.436172 Econ_Windows-0.0.8/Econ_Windows.egg-info/
--rw-rw-rw-   0        0        0      162 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2023-05-17 11:51:41.436172 Econ_Windows-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-17 11:51:41.444245 Econ_Windows-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1972 2023-05-17 11:51:03.000000 Econ_Windows-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:56:26.172037 Econ_Windows-0.0.9/
+-rw-rw-rw-   0        0        0    11023 2023-05-17 11:55:09.000000 Econ_Windows-0.0.9/Econ_Windows.cpp
+drwxrwxrwx   0        0        0        0 2023-05-17 11:56:26.161923 Econ_Windows-0.0.9/Econ_Windows.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-17 11:56:26.000000 Econ_Windows-0.0.9/Econ_Windows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-17 11:56:26.000000 Econ_Windows-0.0.9/Econ_Windows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 11:56:26.000000 Econ_Windows-0.0.9/Econ_Windows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 11:51:41.000000 Econ_Windows-0.0.9/Econ_Windows.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-17 11:56:26.000000 Econ_Windows-0.0.9/Econ_Windows.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      162 2023-05-17 11:56:26.170481 Econ_Windows-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-17 11:56:26.172037 Econ_Windows-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1972 2023-05-17 11:55:34.000000 Econ_Windows-0.0.9/setup.py
```

### Comparing `Econ_Windows-0.0.8/Econ_Windows.cpp` & `Econ_Windows-0.0.9/Econ_Windows.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -219,14 +219,15 @@
 	bool getDeviceCount(uint32_t *gDeviceCount) 
 	{
 	  
 	 //printf("Device is not connected");
 	  initialize();
 	  int list = indexList;
 	  int temgDeviceCount = *gDeviceCount;
+	  temgDeviceCount = 0;
 	  if (!indexList) 
 	  {
 		 // return DEPTHVISTAError::setErrno(Result::NoDeviceConnected);
 		 printf("Device is not connected");
 		 return false;
 	  }
 	  while (list)
```

### Comparing `Econ_Windows-0.0.8/setup.py` & `Econ_Windows-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for extension in ext_modules:
         extension.extra_compile_args = ['-std=c++11', '-fPIC']
         extension.extra_link_args = ['-std=c++11', '-fPIC']
 
 # setup
 setup(
     name='Econ_Windows',
-    version='0.0.8',
+    version='0.0.9',
     author='Sulthan Amanu',
     author_email='sulthan4380@example.com',
     description='Example project using pybind11',
     ext_modules=ext_modules,
     cmdclass={'build_ext': build_ext},
     zip_safe=False,
 )
```

