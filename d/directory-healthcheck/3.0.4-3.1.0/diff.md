# Comparing `tmp/directory_healthcheck-3.0.4-py3-none-any.whl.zip` & `tmp/directory_healthcheck-3.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5601 bytes, number of entries: 10
--rw-r--r--  2.0 unx       68 b- defN 23-Apr-06 09:48 directory_healthcheck/__init__.py
--rw-r--r--  2.0 unx      324 b- defN 23-Apr-06 09:48 directory_healthcheck/apps.py
--rw-r--r--  2.0 unx     2244 b- defN 23-Apr-06 09:48 directory_healthcheck/backends.py
--rw-r--r--  2.0 unx     1087 b- defN 23-Apr-06 09:48 directory_healthcheck/views.py
--rw-r--r--  2.0 unx      339 b- defN 23-Apr-06 09:48 directory_healthcheck/templates/directory_healthcheck/healthcheck.html
--rw-r--r--  2.0 unx     1091 b- defN 23-Apr-06 09:48 directory_healthcheck-3.0.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     4035 b- defN 23-Apr-06 09:48 directory_healthcheck-3.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-06 09:48 directory_healthcheck-3.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       22 b- defN 23-Apr-06 09:48 directory_healthcheck-3.0.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      932 b- defN 23-Apr-06 09:48 directory_healthcheck-3.0.4.dist-info/RECORD
-10 files, 10234 bytes uncompressed, 3971 bytes compressed:  61.2%
+Zip file size: 5609 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       68 b- defN 23-May-17 10:36 directory_healthcheck/__init__.py
+-rw-r--r--  2.0 unx      324 b- defN 23-May-17 10:36 directory_healthcheck/apps.py
+-rw-r--r--  2.0 unx     2244 b- defN 23-May-17 10:36 directory_healthcheck/backends.py
+-rw-r--r--  2.0 unx     1087 b- defN 23-May-17 10:36 directory_healthcheck/views.py
+-rw-r--r--  2.0 unx      339 b- defN 23-May-17 10:36 directory_healthcheck/templates/directory_healthcheck/healthcheck.html
+-rw-r--r--  2.0 unx     1091 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4074 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       22 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      932 b- defN 23-May-17 10:37 directory_healthcheck-3.1.0.dist-info/RECORD
+10 files, 10273 bytes uncompressed, 3979 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: directory_healthcheck/views.py
 Comment: 
 
 Filename: directory_healthcheck/templates/directory_healthcheck/healthcheck.html
 Comment: 
 
-Filename: directory_healthcheck-3.0.4.dist-info/LICENSE
+Filename: directory_healthcheck-3.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: directory_healthcheck-3.0.4.dist-info/METADATA
+Filename: directory_healthcheck-3.1.0.dist-info/METADATA
 Comment: 
 
-Filename: directory_healthcheck-3.0.4.dist-info/WHEEL
+Filename: directory_healthcheck-3.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: directory_healthcheck-3.0.4.dist-info/top_level.txt
+Filename: directory_healthcheck-3.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_healthcheck-3.0.4.dist-info/RECORD
+Filename: directory_healthcheck-3.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `directory_healthcheck-3.0.4.dist-info/LICENSE` & `directory_healthcheck-3.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_healthcheck-3.0.4.dist-info/METADATA` & `directory_healthcheck-3.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 Metadata-Version: 2.1
 Name: directory-healthcheck
-Version: 3.0.4
+Version: 3.1.0
 Summary: Library to streamline healthchecks for Directory apps.
 Home-page: https://github.com/uktrade/directory-healthcheck
 Author: Department for International Trade
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 1.11
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: django-health-check (==3.16.5)
-Requires-Dist: django (<=4.0.10,>=3.2.18)
+Requires-Dist: django-health-check (==3.17.0)
+Requires-Dist: django (<=4.1.9,>=3.2.18)
 Provides-Extra: test
 Requires-Dist: pytest (==3.10.0) ; extra == 'test'
 Requires-Dist: pytest-cov (==2.7.1) ; extra == 'test'
 Requires-Dist: pytest-django (==3.5.0) ; extra == 'test'
 Requires-Dist: flake8 (==5.0.4) ; extra == 'test'
 Requires-Dist: codecov (>=2.0.16) ; extra == 'test'
-Requires-Dist: twine (<2.0.0,>=1.11.0) ; extra == 'test'
+Requires-Dist: twine (<=4.0.2,>=1.11.0) ; extra == 'test'
 Requires-Dist: wheel (<1.0.0,>=0.31.0) ; extra == 'test'
 Requires-Dist: raven (==5.19.0) ; extra == 'test'
 Requires-Dist: setuptools (<66.1.0,>=59.6.0) ; extra == 'test'
 Requires-Dist: directory-sso-api-client ; extra == 'test'
 Requires-Dist: directory-api-client ; extra == 'test'
 Requires-Dist: directory-forms-api-client ; extra == 'test'
 Requires-Dist: directory-cms-client ; extra == 'test'
```

## Comparing `directory_healthcheck-3.0.4.dist-info/RECORD` & `directory_healthcheck-3.1.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 directory_healthcheck/__init__.py,sha256=MzxjIY-3JI1bs39tYXgNHjZdG8srfCVhLqfzp4nHh_U,68
 directory_healthcheck/apps.py,sha256=0YlRHNWpSolt1BeQ7kWG1IFauQ54GH-694hg26sQ4Bw,324
 directory_healthcheck/backends.py,sha256=-UOn5GJsRcuBAuqEWfPRnKpKIygqoDiEg68FvzIY0-Q,2244
 directory_healthcheck/views.py,sha256=GM69IDljqvY8S4IZntiXxL1u38NUjkmS72e-SGKlaHQ,1087
 directory_healthcheck/templates/directory_healthcheck/healthcheck.html,sha256=Na6eXAmCvfSUOG1IEEIUn4UbhkkUJpbKLlamkZQrRBg,339
-directory_healthcheck-3.0.4.dist-info/LICENSE,sha256=4QTWtORsQRx8DlWoAAEQHCse85Eas0SqCllvkojIO_M,1091
-directory_healthcheck-3.0.4.dist-info/METADATA,sha256=Glp7MRTWfdaGaCEwdGL4jndQFw48OrQR4q2lJQDWMZc,4035
-directory_healthcheck-3.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-directory_healthcheck-3.0.4.dist-info/top_level.txt,sha256=ulfdOAfZlBGuRGJ3NNjj_a-FxUHXi2-B3sJrTu_U9Y0,22
-directory_healthcheck-3.0.4.dist-info/RECORD,,
+directory_healthcheck-3.1.0.dist-info/LICENSE,sha256=4QTWtORsQRx8DlWoAAEQHCse85Eas0SqCllvkojIO_M,1091
+directory_healthcheck-3.1.0.dist-info/METADATA,sha256=PntYBJEQO-nm-ko79gHNxDNqk0LifGsDV1wjxKDWyxI,4074
+directory_healthcheck-3.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+directory_healthcheck-3.1.0.dist-info/top_level.txt,sha256=ulfdOAfZlBGuRGJ3NNjj_a-FxUHXi2-B3sJrTu_U9Y0,22
+directory_healthcheck-3.1.0.dist-info/RECORD,,
```

