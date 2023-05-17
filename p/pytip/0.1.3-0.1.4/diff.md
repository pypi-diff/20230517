# Comparing `tmp/pytip-0.1.3-py2.py3-none-any.whl.zip` & `tmp/pytip-0.1.4-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 18007 bytes, number of entries: 17
--rw-rw-r--  2.0 unx      704 b- defN 23-May-08 03:40 pytip/__init__.py
+Zip file size: 18208 bytes, number of entries: 17
+-rw-rw-r--  2.0 unx      718 b- defN 23-May-10 01:34 pytip/__init__.py
 -rw-rw-r--  2.0 unx    42686 b- defN 23-Apr-16 06:56 pytip/data/browsers.json
 -rw-rw-r--  2.0 unx      389 b- defN 23-Apr-09 02:24 pytip/tools/__init__.py
--rw-rw-r--  2.0 unx     3268 b- defN 23-Apr-09 01:31 pytip/tools/item.py
+-rw-rw-r--  2.0 unx     3639 b- defN 23-May-17 03:48 pytip/tools/item.py
 -rw-rw-r--  2.0 unx      854 b- defN 23-Apr-09 01:59 pytip/tools/plot.py
 -rw-rw-r--  2.0 unx     1597 b- defN 23-Apr-09 10:43 pytip/tools/table.py
 -rw-rw-r--  2.0 unx      423 b- defN 23-Apr-16 02:29 pytip/utils/__init__.py
--rw-rw-r--  2.0 unx     3831 b- defN 23-Apr-16 07:13 pytip/utils/celery.py
--rw-rw-r--  2.0 unx     2268 b- defN 23-May-08 03:48 pytip/utils/checker.py
--rw-rw-r--  2.0 unx     1291 b- defN 23-Apr-17 02:26 pytip/utils/deco.py
+-rw-rw-r--  2.0 unx     3860 b- defN 23-May-17 02:15 pytip/utils/celery.py
+-rw-rw-r--  2.0 unx     2268 b- defN 23-May-17 02:15 pytip/utils/checker.py
+-rw-rw-r--  2.0 unx     1291 b- defN 23-May-17 02:15 pytip/utils/deco.py
 -rw-rw-r--  2.0 unx     2983 b- defN 23-Apr-16 07:13 pytip/utils/file.py
--rw-rw-r--  2.0 unx     1255 b- defN 23-May-08 03:35 pytip/utils/func.py
+-rw-rw-r--  2.0 unx     1255 b- defN 23-May-17 02:15 pytip/utils/func.py
 -rw-rw-r--  2.0 unx     1823 b- defN 23-Apr-16 08:49 pytip/utils/web.py
--rw-rw-r--  2.0 unx     1081 b- defN 23-May-08 04:13 pytip-0.1.3.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-08 04:13 pytip-0.1.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-May-08 04:13 pytip-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1291 b- defN 23-May-08 04:13 pytip-0.1.3.dist-info/RECORD
-17 files, 65860 bytes uncompressed, 15927 bytes compressed:  75.8%
+-rw-rw-r--  2.0 unx     1081 b- defN 23-May-17 03:49 pytip-0.1.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-17 03:49 pytip-0.1.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-17 03:49 pytip-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1291 b- defN 23-May-17 03:49 pytip-0.1.4.dist-info/RECORD
+17 files, 66274 bytes uncompressed, 16128 bytes compressed:  75.7%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: pytip/utils/func.py
 Comment: 
 
 Filename: pytip/utils/web.py
 Comment: 
 
-Filename: pytip-0.1.3.dist-info/METADATA
+Filename: pytip-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: pytip-0.1.3.dist-info/WHEEL
+Filename: pytip-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: pytip-0.1.3.dist-info/top_level.txt
+Filename: pytip-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: pytip-0.1.3.dist-info/RECORD
+Filename: pytip-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytip/__init__.py

```diff
@@ -13,10 +13,11 @@
 from .utils.file import (
     multiprocess_items, file_download, file_pickle, print_error
 )
 
 from .tools.plot import plt_ko
 from .tools.table import df_number_column
 from .tools.item import (
-    date_to_string, string_to_datetime, divide_chunks
+    date_to_string, string_to_datetime, divide_chunks,
+    password
 )
```

## pytip/tools/item.py

```diff
@@ -1,8 +1,10 @@
 import re
+import string
+import random
 import datetime
 import itertools
 
 
 REGEX_DATETIME = {
     '[\d]{4}-[\d]{2}-[\d]{2}.[A-Z]{2}[\d]{1,2}:[\d]{1,2}:[\d]{1,2}':
     '%Y-%m-%d.%p%I:%M:%S', # '2022-07-31.AM3:02:30'
@@ -21,15 +23,15 @@
         business_day:bool=False,
     ):
 
     r"""date 객체를 string 으로 자동변환
     _date        : 날짜객체
     only_number  : 날짜 구분자 없이 숫자로만 출력 
     datetime_obj : datetime 객체로 출력
-    business_day : 평일 날짜로 변환"""
+    business_day : 주말 -> 해당 주차 평일로 변환"""
 
     _return = None
     if date is None:
         _return = datetime.date.today().isoformat()
     elif type(date) == datetime.date:
         _return = date.isoformat()
     elif type(date) == datetime.datetime:
@@ -90,7 +92,14 @@
         for i in range(0, len(items), n): # looping till length l
             yield items[i:i + n]          # list should have
     
     elif type(items) == dict:
         for i in range(0, len(items), n):
             yield dict(itertools.islice(items.items(), i ,i+n))
 
+
+# 문자 난수생성 (비밀번호 생성기)
+def password(length:int=12) -> str:
+    r"""난수문자 생성기 (ex> 비밀번호)
+    length : 생성문자 길이"""
+    letters = string.ascii_letters + string.digits + "!#$%&*+-?@" # string.punctuation
+    return "".join([random.choice(letters)  for _ in range(length)])
```

## pytip/utils/celery.py

```diff
@@ -1,12 +1,12 @@
 import re
 import pandas
 from ..tools.item import string_to_datetime
 
-
+# Celery Log 파일 분석기
 class Celery:
 
     def __init__(self, file_path:str=None):
         self.file_path = file_path
         self.re_id = "\[[0-9A-z.]+\]"
         self.re_time = "^[0-9]{4}/[0-9]{1,2}/[0-9]{1,2} [0-9]{1,2}:[0-9]{1,2}:[0-9]{1,2}"
         self.re_celery_name = "\[celery\.[\w.]+\]"
```

## Comparing `pytip-0.1.3.dist-info/METADATA` & `pytip-0.1.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytip
-Version: 0.1.3
+Version: 0.1.4
 Home-page: https://github.com/YongBeomKim/pytip
 Author: momukji lab
 Author-email: ybkim@momukji.com
 License: MIT
 Keywords: pytip
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `pytip-0.1.3.dist-info/RECORD` & `pytip-0.1.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-pytip/__init__.py,sha256=AUkdQEMPxCJnJ_SXc5bAmj96UBQeiJZ_-Qn3W6_3Ruw,704
+pytip/__init__.py,sha256=j1C6VrbrG1sGnNR4jZ7d6YZjEF2UkaoLKg3JmNN3hcg,718
 pytip/data/browsers.json,sha256=fgvByElwtpg9QpigM0ss-Rpjnc_Uql4-3y0gJDB7dVI,42686
 pytip/tools/__init__.py,sha256=KKqbkgk5EkEh_2jwQdxUtXATP6peuk43t9zGBN0lQE8,389
-pytip/tools/item.py,sha256=JPF-meLFzP1iwam3jDqeQrPGGfY4fFFYd67jtIfX674,3268
+pytip/tools/item.py,sha256=-O0Q6QaifZdatGtfQaWeJ54K_6ADDzgNDY26A09Ihjo,3639
 pytip/tools/plot.py,sha256=2pmcMkz5HZ5fD5A5OgPr1_Cs2nTZP1DMcuqSyiSMCZk,854
 pytip/tools/table.py,sha256=ddAvODKP7SExPgeEBmeW4QCcZXkDi-aaM3saxqw6vDo,1597
 pytip/utils/__init__.py,sha256=ptGGMFwDewyV4fCaRR3BSwZIGAlug5Z_8xs-scpEDYk,423
-pytip/utils/celery.py,sha256=dEPGQtdQjixd6bL1vuCPkZjZA80-1l1yPSWnu4tpab0,3831
+pytip/utils/celery.py,sha256=rPXP3aAxIwkZBpjczcHELJegjMKbrmIUnpZulRdVcpE,3860
 pytip/utils/checker.py,sha256=VR08MkfhL_rhBll-92c1Xo28yaf4tWRfyBJUQlx2axU,2268
 pytip/utils/deco.py,sha256=BmidVhyoZbLKuziGamyA1TSOBGaU2xZy-ijUn6cAJ3g,1291
 pytip/utils/file.py,sha256=vFbfmPdM7-Fr-8SiJoQWeeu-4LTxCMjgYk4ftauMPBY,2983
 pytip/utils/func.py,sha256=fR_GQcYHMtYb0OC98zQ0i9AMVZqGgS3LJUoJZmjuWI0,1255
 pytip/utils/web.py,sha256=lyR6e7iyDIsSCPovTMmbSm8zu1AHEBEk35adIxYklZo,1823
-pytip-0.1.3.dist-info/METADATA,sha256=jy3M1bZg5H8Te02Q5TOHjtI8KNFSjs7r4rbGqaGJuiU,1081
-pytip-0.1.3.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-pytip-0.1.3.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
-pytip-0.1.3.dist-info/RECORD,,
+pytip-0.1.4.dist-info/METADATA,sha256=qlNME_KV-1OLcLyrluZl9P9QzMqHQYhVG8ObMbhjmmM,1081
+pytip-0.1.4.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+pytip-0.1.4.dist-info/top_level.txt,sha256=jF2tKdrfqmRq7kr--QAKzT5DpQOqrfwdSBO9WrauNHE,6
+pytip-0.1.4.dist-info/RECORD,,
```

