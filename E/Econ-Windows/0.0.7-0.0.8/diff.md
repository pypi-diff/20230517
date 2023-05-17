# Comparing `tmp/Econ_Windows-0.0.7.tar.gz` & `tmp/Econ_Windows-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Econ_Windows-0.0.7.tar", last modified: Wed May 17 07:43:36 2023, max compression
+gzip compressed data, was "Econ_Windows-0.0.8.tar", last modified: Wed May 17 11:51:41 2023, max compression
```

## Comparing `Econ_Windows-0.0.7.tar` & `Econ_Windows-0.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 07:43:36.350328 Econ_Windows-0.0.7/
--rw-rw-rw-   0        0        0    11084 2023-05-17 07:42:34.000000 Econ_Windows-0.0.7/Econ_Windows.cpp
-drwxrwxrwx   0        0        0        0 2023-05-17 07:43:36.350328 Econ_Windows-0.0.7/Econ_Windows.egg-info/
--rw-rw-rw-   0        0        0      162 2023-05-17 07:43:36.000000 Econ_Windows-0.0.7/Econ_Windows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-17 07:43:36.000000 Econ_Windows-0.0.7/Econ_Windows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 07:43:36.000000 Econ_Windows-0.0.7/Econ_Windows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 07:43:36.000000 Econ_Windows-0.0.7/Econ_Windows.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-17 07:43:36.000000 Econ_Windows-0.0.7/Econ_Windows.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2023-05-17 07:43:36.350328 Econ_Windows-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-17 07:43:36.350328 Econ_Windows-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1972 2023-05-17 07:43:16.000000 Econ_Windows-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 11:51:41.444245 Econ_Windows-0.0.8/
+-rw-rw-rw-   0        0        0    10998 2023-05-17 11:50:33.000000 Econ_Windows-0.0.8/Econ_Windows.cpp
+drwxrwxrwx   0        0        0        0 2023-05-17 11:51:41.436172 Econ_Windows-0.0.8/Econ_Windows.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-17 11:51:41.000000 Econ_Windows-0.0.8/Econ_Windows.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      162 2023-05-17 11:51:41.436172 Econ_Windows-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-17 11:51:41.444245 Econ_Windows-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1972 2023-05-17 11:51:03.000000 Econ_Windows-0.0.8/setup.py
```

### Comparing `Econ_Windows-0.0.7/Econ_Windows.cpp` & `Econ_Windows-0.0.8/Econ_Windows.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -218,29 +218,29 @@
   
 	bool getDeviceCount(uint32_t *gDeviceCount) 
 	{
 	  
 	 //printf("Device is not connected");
 	  initialize();
 	  int list = indexList;
-	  *gDeviceCount = 0;
+	  int temgDeviceCount = *gDeviceCount;
 	  if (!indexList) 
 	  {
 		 // return DEPTHVISTAError::setErrno(Result::NoDeviceConnected);
 		 printf("Device is not connected");
 		 return false;
 	  }
 	  while (list)
 	  {
 		  printf("Before list =  %d\n",list);
 		  list &= (list - 1);
 		  printf("After list =  %d\n",list);
-		  printf("Before gdevice list =  %d\n",*gDeviceCount);
-		  *gDeviceCount += 1;
-		  printf("After gdevice list =  %d\n",*gDeviceCount);
+		  printf("Before gdevice list =  %d\n",temgDeviceCount);
+		  temgDeviceCount += 1;
+		  printf("After gdevice list =  %d\n",temgDeviceCount);
 	  }
 	  return true;
   }
   
 	bool getDeviceListInfo(uint32_t deviceCount,DeviceInfo* gDevicesList) 
 	{
 	  for (uint32_t index = 0; index < deviceCount; index++) 
@@ -380,16 +380,14 @@
 		  //return DEPTHVISTAError::setErrno(Result::NotInitialized);
 		  printf("NotInitialized");
 			  return false;
 	  }
   }
   
   
+  
 	PYBIND11_MODULE(Econ_Windows, m)
 	{
     	m.def("getDeviceInfo", &getDeviceInfo, "getDeviceInfo");
-    	//m.def("getDeviceCount", &getDeviceCount, "getDeviceCount");
-		 m.def("getDeviceCount", [](uint32_t *gDeviceCount) {
-        return getDeviceCount(gDeviceCount);
-    });
+    	m.def("getDeviceCount", &getDeviceCount, "getDeviceCount");
 		m.def("getDeviceListInfo", &getDeviceListInfo, "getDeviceListInfo");
 	}
```

### Comparing `Econ_Windows-0.0.7/setup.py` & `Econ_Windows-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for extension in ext_modules:
         extension.extra_compile_args = ['-std=c++11', '-fPIC']
         extension.extra_link_args = ['-std=c++11', '-fPIC']
 
 # setup
 setup(
     name='Econ_Windows',
-    version='0.0.7',
+    version='0.0.8',
     author='Sulthan Amanu',
     author_email='sulthan4380@example.com',
     description='Example project using pybind11',
     ext_modules=ext_modules,
     cmdclass={'build_ext': build_ext},
     zip_safe=False,
 )
```

