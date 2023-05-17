# Comparing `tmp/dopplrSDK-1.2.0-py3-none-any.whl.zip` & `tmp/dopplrSDK-1.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3770 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat     4986 b- defN 23-May-17 16:29 dopplrSDK/__init__.py
--rw-rw-rw-  2.0 fat     1077 b- defN 23-May-17 16:41 dopplrSDK-1.2.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      347 b- defN 23-May-17 16:41 dopplrSDK-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 16:41 dopplrSDK-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       10 b- defN 23-May-17 16:41 dopplrSDK-1.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      477 b- defN 23-May-17 16:41 dopplrSDK-1.2.0.dist-info/RECORD
-6 files, 6989 bytes uncompressed, 2904 bytes compressed:  58.4%
+Zip file size: 3768 bytes, number of entries: 6
+-rw-rw-rw-  2.0 fat     4983 b- defN 23-May-17 16:50 dopplrSDK/__init__.py
+-rw-rw-rw-  2.0 fat     1077 b- defN 23-May-17 16:53 dopplrSDK-1.3.0.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      347 b- defN 23-May-17 16:53 dopplrSDK-1.3.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-17 16:53 dopplrSDK-1.3.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       10 b- defN 23-May-17 16:53 dopplrSDK-1.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      477 b- defN 23-May-17 16:53 dopplrSDK-1.3.0.dist-info/RECORD
+6 files, 6986 bytes uncompressed, 2902 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: dopplrSDK/__init__.py
 Comment: 
 
-Filename: dopplrSDK-1.2.0.dist-info/LICENSE.txt
+Filename: dopplrSDK-1.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dopplrSDK-1.2.0.dist-info/METADATA
+Filename: dopplrSDK-1.3.0.dist-info/METADATA
 Comment: 
 
-Filename: dopplrSDK-1.2.0.dist-info/WHEEL
+Filename: dopplrSDK-1.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: dopplrSDK-1.2.0.dist-info/top_level.txt
+Filename: dopplrSDK-1.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: dopplrSDK-1.2.0.dist-info/RECORD
+Filename: dopplrSDK-1.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dopplrSDK/__init__.py

```diff
@@ -60,15 +60,15 @@
                 Params={
                     'Bucket': ContainerName,
                     'Key': ConnectionString
                 },
                 ExpiresIn=3600  # URL expiration time in seconds (here it's set to 1 hour)
             )  
 
-        #print("insert1 ",url)
+        print("url : ",url)
         cnxn.close()
         #print("done")
     except Exception as error:
         if 'NoneType' in str(error):
             dopplrsource= 'File does not exists'
             print("Error : ", dopplrsource)
             sys.exit()
```

## Comparing `dopplrSDK-1.2.0.dist-info/LICENSE.txt` & `dopplrSDK-1.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

