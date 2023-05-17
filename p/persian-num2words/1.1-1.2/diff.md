# Comparing `tmp/persian_num2words-1.1.tar.gz` & `tmp/persian_num2words-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "persian_num2words-1.1.tar", last modified: Wed May 17 18:21:24 2023, max compression
+gzip compressed data, was "persian_num2words-1.2.tar", last modified: Wed May 17 18:34:05 2023, max compression
```

## Comparing `persian_num2words-1.1.tar` & `persian_num2words-1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.522441 persian_num2words-1.1/
--rw-r--r--   0 mostafa    (501) staff       (20)     1068 2023-05-14 12:03:58.000000 persian_num2words-1.1/LICENSE.txt
--rw-r--r--   0 mostafa    (501) staff       (20)     1844 2023-05-17 18:21:24.522486 persian_num2words-1.1/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)      163 2023-05-14 12:03:02.000000 persian_num2words-1.1/README.md
--rw-r--r--   0 mostafa    (501) staff       (20)       84 2023-05-14 12:00:11.000000 persian_num2words-1.1/pyproject.toml
--rw-r--r--   0 mostafa    (501) staff       (20)      734 2023-05-17 18:21:24.522716 persian_num2words-1.1/setup.cfg
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.520718 persian_num2words-1.1/src/
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.521485 persian_num2words-1.1/src/num2words/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.1/src/num2words/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)    12495 2023-05-14 13:32:45.000000 persian_num2words-1.1/src/num2words/num2words.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.522027 persian_num2words-1.1/src/persian_num2words.egg-info/
--rw-r--r--   0 mostafa    (501) staff       (20)     1844 2023-05-17 18:21:24.000000 persian_num2words-1.1/src/persian_num2words.egg-info/PKG-INFO
--rw-r--r--   0 mostafa    (501) staff       (20)      352 2023-05-17 18:21:24.000000 persian_num2words-1.1/src/persian_num2words.egg-info/SOURCES.txt
--rw-r--r--   0 mostafa    (501) staff       (20)        1 2023-05-17 18:21:24.000000 persian_num2words-1.1/src/persian_num2words.egg-info/dependency_links.txt
--rw-r--r--   0 mostafa    (501) staff       (20)       16 2023-05-17 18:21:24.000000 persian_num2words-1.1/src/persian_num2words.egg-info/top_level.txt
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.522216 persian_num2words-1.1/src/utils/
--rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.1/src/utils/__init__.py
--rw-r--r--   0 mostafa    (501) staff       (20)      156 2023-05-13 19:21:29.000000 persian_num2words-1.1/src/utils/small_function.py
-drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:21:24.522334 persian_num2words-1.1/tests/
--rw-r--r--   0 mostafa    (501) staff       (20)      228 2023-05-14 11:52:26.000000 persian_num2words-1.1/tests/test_num2word.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:34:05.921543 persian_num2words-1.2/
+-rw-r--r--   0 mostafa    (501) staff       (20)     1068 2023-05-14 12:03:58.000000 persian_num2words-1.2/LICENSE.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)     1844 2023-05-17 18:34:05.921584 persian_num2words-1.2/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)      163 2023-05-14 12:03:02.000000 persian_num2words-1.2/README.md
+-rw-r--r--   0 mostafa    (501) staff       (20)       84 2023-05-14 12:00:11.000000 persian_num2words-1.2/pyproject.toml
+-rw-r--r--   0 mostafa    (501) staff       (20)      734 2023-05-17 18:34:05.921808 persian_num2words-1.2/setup.cfg
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:34:05.919976 persian_num2words-1.2/src/
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:34:05.920650 persian_num2words-1.2/src/num2words/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.2/src/num2words/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)    12397 2023-05-17 18:25:56.000000 persian_num2words-1.2/src/num2words/num2words.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:34:05.921103 persian_num2words-1.2/src/persian_num2words.egg-info/
+-rw-r--r--   0 mostafa    (501) staff       (20)     1844 2023-05-17 18:34:05.000000 persian_num2words-1.2/src/persian_num2words.egg-info/PKG-INFO
+-rw-r--r--   0 mostafa    (501) staff       (20)      352 2023-05-17 18:34:05.000000 persian_num2words-1.2/src/persian_num2words.egg-info/SOURCES.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)        1 2023-05-17 18:34:05.000000 persian_num2words-1.2/src/persian_num2words.egg-info/dependency_links.txt
+-rw-r--r--   0 mostafa    (501) staff       (20)       16 2023-05-17 18:34:05.000000 persian_num2words-1.2/src/persian_num2words.egg-info/top_level.txt
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:34:05.921300 persian_num2words-1.2/src/utils/
+-rw-r--r--   0 mostafa    (501) staff       (20)        0 2023-05-14 11:40:42.000000 persian_num2words-1.2/src/utils/__init__.py
+-rw-r--r--   0 mostafa    (501) staff       (20)      156 2023-05-13 19:21:29.000000 persian_num2words-1.2/src/utils/small_function.py
+drwxr-xr-x   0 mostafa    (501) staff       (20)        0 2023-05-17 18:34:05.921422 persian_num2words-1.2/tests/
+-rw-r--r--   0 mostafa    (501) staff       (20)      228 2023-05-14 11:52:26.000000 persian_num2words-1.2/tests/test_num2word.py
```

### Comparing `persian_num2words-1.1/LICENSE.txt` & `persian_num2words-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `persian_num2words-1.1/PKG-INFO` & `persian_num2words-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian_num2words
-Version: 1.1
+Version: 1.2
 Summary: A Package to Convert Numbers to Words in Persian.
 Home-page: https://github.com/mosihere/persian_num2words
 Author: Mosihere
 Author-email: mosihere@gmail.com
 Project-URL: Bug Tracker, https://github.com/mosihere/persian_num2words/issues
 Project-URL: repository, https://github.com/mosihere/persian_num2words
 Classifier: Programming Language :: Python :: 3
```

### Comparing `persian_num2words-1.1/setup.cfg` & `persian_num2words-1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = persian_num2words
-version = 1.1
+version = 1.2
 author = Mosihere
 author_email = mosihere@gmail.com
 description = A Package to Convert Numbers to Words in Persian.
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/mosihere/persian_num2words
 project_urls =
```

### Comparing `persian_num2words-1.1/src/num2words/num2words.py` & `persian_num2words-1.2/src/num2words/num2words.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import small_module.small_function
+import utils.small_function
 
 
 ones = {
     0: '',
     1: 'یک',
     2: 'دو',
     3: 'سه',
@@ -196,15 +196,15 @@
 
             return f'{hundreds_word} و {tens_word} و {ones_word}'
         
 
     elif number > 999 and number <= 9999:
 
         last_two_digits = int(str_number[2:])
-        if small_module.small_function.is_less_than_twenty(last_two_digits):
+        if utils.small_function.is_less_than_twenty(last_two_digits):
             tens_word = ten_to_nineteen[last_two_digits]
 
             find_thousands = int(str_number[0])
             find_hundreds = int(str_number[1])
 
             thousands_word = thousands[find_thousands]
             hundreds_word = hundreds[find_hundreds]
@@ -227,26 +227,26 @@
 
     elif number > 9999 and number <= 99999:
 
         first_two_digits = int(str_number[0:2])
         last_two_digits = int(str_number[3:])
 
 
-        if small_module.small_function.is_less_than_twenty(first_two_digits) and small_module.small_function.is_less_than_twenty(last_two_digits):
+        if utils.small_function.is_less_than_twenty(first_two_digits) and utils.small_function.is_less_than_twenty(last_two_digits):
             thousands_word = ten_to_nineteen[first_two_digits]
 
             find_hundreds = int(str_number[2])
             hundreds_word = hundreds[find_hundreds]
 
             tens_word = ten_to_nineteen[last_two_digits]
 
             return f'{thousands_word} هزار {hundreds_word} و {tens_word}'
     
 
-        elif small_module.small_function.is_less_than_twenty(first_two_digits) and not small_module.small_function.is_less_than_twenty(last_two_digits):
+        elif utils.small_function.is_less_than_twenty(first_two_digits) and not utils.small_function.is_less_than_twenty(last_two_digits):
 
             thousands_word = ten_to_nineteen[first_two_digits]
 
             find_hundreds = int(str_number[2])
             hundreds_word = hundreds[find_hundreds]
 
             find_tens = int(str_number[3])
@@ -254,15 +254,15 @@
 
             find_ones = int(str_number[4])
             ones_word = ones[find_ones]
 
             return f'{thousands_word} هزار {hundreds_word} {tens_word} {ones_word}' 
 
 
-        elif not small_module.small_function.is_less_than_twenty(first_two_digits) and small_module.small_function.is_less_than_twenty(last_two_digits):
+        elif not utils.small_function.is_less_than_twenty(first_two_digits) and utils.small_function.is_less_than_twenty(last_two_digits):
 
             find_ten_thousands = int(str_number[0])
             ten_thousands_word = twenties_and_others[find_ten_thousands]
 
             find_thousands = int(str_number[1])
             thousands_word = ones[find_thousands]
 
@@ -296,28 +296,28 @@
 
     elif number > 99999 and number <= 9999999:
 
         first_two_digits = int(str_number[1:3])
         last_two_digits = int(str_number[4:])
 
 
-        if small_module.small_function.is_less_than_twenty(first_two_digits) and small_module.small_function.s_less_than_twenty(last_two_digits):
+        if utils.small_function.is_less_than_twenty(first_two_digits) and utils.small_function.s_less_than_twenty(last_two_digits):
             find_hundred_thousands = int(str_number[0])
             hundred_thousands_word = hundreds[find_hundred_thousands]
             thousands_word = ten_to_nineteen[first_two_digits]
 
             find_hundreds = int(str_number[3])
             hundreds_word = hundreds[find_hundreds]
 
             tens_word = ten_to_nineteen[last_two_digits]
 
             return f'{hundred_thousands_word} و {thousands_word} هزار {hundreds_word} و {tens_word}'
     
 
-        elif small_module.small_function.is_less_than_twenty(first_two_digits) and not small_module.small_function.is_less_than_twenty(last_two_digits):
+        elif utils.small_function.is_less_than_twenty(first_two_digits) and not utils.small_function.is_less_than_twenty(last_two_digits):
 
             find_hundred_thousands = int(str_number[0])
             hundred_thousands_word = hundreds[find_hundred_thousands]
             thousands_word = ten_to_nineteen[first_two_digits]
 
 
             find_hundreds = int(str_number[3])
@@ -329,15 +329,15 @@
             find_ones = int(str_number[5])
             ones_word = ones[find_ones]
 
 
             return f' {hundred_thousands_word} {thousands_word} هزار {hundreds_word} {tens_word} {ones_word}' 
 
 
-        elif not small_module.small_function.is_less_than_twenty(first_two_digits) and small_module.small_function.is_less_than_twenty(last_two_digits):
+        elif not utils.small_function.is_less_than_twenty(first_two_digits) and utils.small_function.is_less_than_twenty(last_two_digits):
 
             find_hundred_thousands = int(str_number[0])
             hundred_thousands_word = hundreds[find_hundred_thousands]
 
             find_ten_thousands = int(str_number[1])
             ten_thousands_word = ten_to_nineteen[find_ten_thousands]
             print(ten_thousands_word)
```

### Comparing `persian_num2words-1.1/src/persian_num2words.egg-info/PKG-INFO` & `persian_num2words-1.2/src/persian_num2words.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: persian-num2words
-Version: 1.1
+Version: 1.2
 Summary: A Package to Convert Numbers to Words in Persian.
 Home-page: https://github.com/mosihere/persian_num2words
 Author: Mosihere
 Author-email: mosihere@gmail.com
 Project-URL: Bug Tracker, https://github.com/mosihere/persian_num2words/issues
 Project-URL: repository, https://github.com/mosihere/persian_num2words
 Classifier: Programming Language :: Python :: 3
```

