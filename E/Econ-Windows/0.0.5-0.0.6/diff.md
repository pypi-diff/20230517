# Comparing `tmp/Econ_Windows-0.0.5.tar.gz` & `tmp/Econ_Windows-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Econ_Windows-0.0.5.tar", last modified: Tue May 16 16:13:10 2023, max compression
+gzip compressed data, was "Econ_Windows-0.0.6.tar", last modified: Tue May 16 16:28:39 2023, max compression
```

## Comparing `Econ_Windows-0.0.5.tar` & `Econ_Windows-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 16:13:10.504791 Econ_Windows-0.0.5/
--rw-rw-rw-   0        0        0    10922 2023-05-16 16:12:35.000000 Econ_Windows-0.0.5/Econ_Windows.cpp
-drwxrwxrwx   0        0        0        0 2023-05-16 16:13:10.501144 Econ_Windows-0.0.5/Econ_Windows.egg-info/
--rw-rw-rw-   0        0        0      162 2023-05-16 16:13:10.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-16 16:13:10.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 16:13:10.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-16 15:52:20.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-05-16 16:13:10.000000 Econ_Windows-0.0.5/Econ_Windows.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      162 2023-05-16 16:13:10.502834 Econ_Windows-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-16 16:13:10.504791 Econ_Windows-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1972 2023-05-16 16:09:58.000000 Econ_Windows-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 16:28:39.244473 Econ_Windows-0.0.6/
+-rw-rw-rw-   0        0        0    10954 2023-05-16 16:27:46.000000 Econ_Windows-0.0.6/Econ_Windows.cpp
+drwxrwxrwx   0        0        0        0 2023-05-16 16:28:39.241473 Econ_Windows-0.0.6/Econ_Windows.egg-info/
+-rw-rw-rw-   0        0        0      162 2023-05-16 16:28:39.000000 Econ_Windows-0.0.6/Econ_Windows.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-16 16:28:39.000000 Econ_Windows-0.0.6/Econ_Windows.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 16:28:39.000000 Econ_Windows-0.0.6/Econ_Windows.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-16 15:52:20.000000 Econ_Windows-0.0.6/Econ_Windows.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       13 2023-05-16 16:28:39.000000 Econ_Windows-0.0.6/Econ_Windows.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      162 2023-05-16 16:28:39.243473 Econ_Windows-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-16 16:28:39.244473 Econ_Windows-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1972 2023-05-16 16:28:29.000000 Econ_Windows-0.0.6/setup.py
```

### Comparing `Econ_Windows-0.0.5/Econ_Windows.cpp` & `Econ_Windows-0.0.6/Econ_Windows.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -173,20 +173,20 @@
 						  printf("While loop - pid_substr != NULL - wcsncpy_s(extrctd_pid, pid_substr + 4, 4);\n");
 					  }
 						
 
 					  if ((wcscmp(wcsupr(extrctd_vid), TOF_VID) == 0) && (wcscmp(wcsupr(extrctd_pid), TOF_PID) == 0))
 					  {
 						  printf("Before index list is fill  %d\n"+indexList);
-						  printf("count = %d\n"+ Count);
+						  printf("count = %d\n"+(uint16_t) Count);
 						  indexList |= (1 << Count);
 						  printf("After index list is : %d\n"+indexList);
-						  printf("Before count update = %d\n"+ Count);
+						  printf("Before count update = %d\n"+ (uint16_t)Count);
 						  Count++;
-						  printf("After count update = %d\n"+ Count);
+						  printf("After count update = %d\n"+ (uint16_t)Count);
 						  printf("After index list is : %d\n"+indexList);
 						  
 					  }
 
 				  }
 				  SysFreeString(var.bstrVal);
 			  }
@@ -230,17 +230,17 @@
 		 return false;
 	  }
 	  while (list)
 	  {
 		  printf("Before list =  %d\n",list);
 		  list &= (list - 1);
 		  printf("After list =  %d\n",list);
-		  printf("Before list =  %d\n",gDeviceCount);
+		  printf("Before list =  %d\n",*gDeviceCount);
 		  *gDeviceCount += 1;
-		  printf("After list =  %d\n",gDeviceCount);
+		  printf("After list =  %d\n",*gDeviceCount);
 	  }
 	  return true;
   }
   
 	bool getDeviceListInfo(uint32_t deviceCount,DeviceInfo* gDevicesList) 
 	{
 	  for (uint32_t index = 0; index < deviceCount; index++)
```

### Comparing `Econ_Windows-0.0.5/setup.py` & `Econ_Windows-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     for extension in ext_modules:
         extension.extra_compile_args = ['-std=c++11', '-fPIC']
         extension.extra_link_args = ['-std=c++11', '-fPIC']
 
 # setup
 setup(
     name='Econ_Windows',
-    version='0.0.5',
+    version='0.0.6',
     author='Sulthan Amanu',
     author_email='sulthan4380@example.com',
     description='Example project using pybind11',
     ext_modules=ext_modules,
     cmdclass={'build_ext': build_ext},
     zip_safe=False,
 )
```

