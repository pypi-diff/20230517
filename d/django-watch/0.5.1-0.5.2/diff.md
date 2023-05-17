# Comparing `tmp/django_watch-0.5.1-py3-none-any.whl.zip` & `tmp/django_watch-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3976 bytes, number of entries: 7
+Zip file size: 3996 bytes, number of entries: 7
 -rwxr-xr-x  2.0 unx        0 b- defN 20-Jan-27 13:04 django_watch/__init__.py
--rw-rw-r--  2.0 unx     3154 b- defN 23-May-05 05:20 django_watch/middleware.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1900 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       13 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      572 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/RECORD
-7 files, 6825 bytes uncompressed, 2954 bytes compressed:  56.7%
+-rw-rw-r--  2.0 unx     3232 b- defN 23-May-17 14:11 django_watch/middleware.py
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-May-17 14:14 django_watch-0.5.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1900 b- defN 23-May-17 14:14 django_watch-0.5.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-17 14:14 django_watch-0.5.2.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       13 b- defN 23-May-17 14:14 django_watch-0.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      572 b- defN 23-May-17 14:14 django_watch-0.5.2.dist-info/RECORD
+7 files, 6903 bytes uncompressed, 2974 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: django_watch/__init__.py
 Comment: 
 
 Filename: django_watch/middleware.py
 Comment: 
 
-Filename: django_watch-0.5.1.dist-info/LICENSE
+Filename: django_watch-0.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: django_watch-0.5.1.dist-info/METADATA
+Filename: django_watch-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: django_watch-0.5.1.dist-info/WHEEL
+Filename: django_watch-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: django_watch-0.5.1.dist-info/top_level.txt
+Filename: django_watch-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: django_watch-0.5.1.dist-info/RECORD
+Filename: django_watch-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_watch/middleware.py

```diff
@@ -46,29 +46,29 @@
             process_stdout_end += f"{self.YELLOW} • STATUS {response.status_code} • Total time • {round((time.monotonic() - time_start), 2)}s{self.END}"        
             print(process_stdout_end)
         return response
 
     def process_view(self, request, func, args, kwargs):                 
         func = unwrap(func)   
         if hasattr(func, "__code__"):
-            process_stdout_start = f"\n| {self.GREEN}START {request.method} {func.__code__.co_filename} {self.END}| • {self.GREEN}{self.BOLD}{func.__name__}{self.END}{self.END} {self.GREEN}•{self.END} {self.GREEN}Line number {func.__code__.co_firstlineno}{self.END}"
-            request.process_stdout_end = f"\n| {self.YELLOW}{self.BOLD}END {request.method} {func.__code__.co_filename} {self.END}| • {self.YELLOW}{self.BOLD}{func.__name__}{self.END}{self.END}"
+            process_stdout_start = f"\n░░ {self.GREEN}START {request.method} {func.__code__.co_filename} {self.END}| • {self.GREEN}{self.BOLD}{func.__name__}{self.END}{self.END} {self.GREEN}•{self.END} {self.GREEN}Line number {func.__code__.co_firstlineno}{self.END}"
+            request.process_stdout_end = f"\n░░ {self.YELLOW}{self.BOLD}END {request.method} {func.__code__.co_filename} {self.END}| • {self.YELLOW}{self.BOLD}{func.__name__}{self.END}{self.END}"
             
             print(process_stdout_start)
             if args: 
-                print(f"| args: {args}"[:200])
+                print(f"░░░░ args: {args}"[:200])
             if kwargs: 
-                print(f"| kwargs: {kwargs}"[:200])
+                print(f"░░░░ kwargs: {kwargs}"[:200])
             if request.GET:
-                print(f"| request.GET: {request.GET}"[:200])                
+                print(f"░░░░ request.GET: {request.GET}"[:200])                
             if request.POST: 
-                print(f"| request.POST: {request.POST}"[:200])
+                print(f"░░░░ request.POST: {request.POST}"[:200])
                 
             try:
                 if not request.POST and request.body:
-                    print(f"| request.body: {request.body}"[:200])
+                    print(f"░░░░ request.body: {request.body}"[:200])
             except Exception as e:
                 pass
             
     def process_exception(self, request, exception):
-        print(f"{self.RED}{self.BOLD}| Exception{self.END}{self.END}")
-        print( "| TRACEBACK:\n{}".format( "".join(traceback.format_exception(type(exception), exception, exception.__traceback__))))
+        print(f"{self.RED}{self.BOLD}░ Exception{self.END}{self.END}")
+        print( "░░░░ TRACEBACK:\n{}".format( "".join(traceback.format_exception(type(exception), exception, exception.__traceback__))))
```

## Comparing `django_watch-0.5.1.dist-info/LICENSE` & `django_watch-0.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_watch-0.5.1.dist-info/METADATA` & `django_watch-0.5.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-watch
-Version: 0.5.1
+Version: 0.5.2
 Summary: Simple and useful django middleware for real-time logging.
 Home-page: https://github.com/Sobolev5/django-watch/
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

