# Comparing `tmp/grokspeechrec-0.0.1.tar.gz` & `tmp/grokspeechrec-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\grokspeechrec-0.0.1.tar", last modified: Wed May  3 20:09:33 2023, max compression
+gzip compressed data, was "D:\Drive_A\Python\pypidemo\dist\.tmp-nsb44e63\grokspeechrec-0.0.2.tar", last modified: Wed May 17 07:17:43 2023, max compression
```

## Comparing `grokspeechrec-0.0.1.tar` & `grokspeechrec-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 20:09:33.000000 grokspeechrec-0.0.1/
--rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 grokspeechrec-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1785 2023-05-03 20:09:33.000000 grokspeechrec-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2023-05-03 20:04:09.000000 grokspeechrec-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 20:09:33.000000 grokspeechrec-0.0.1/grokspeechrec.egg-info/
--rw-rw-rw-   0        0        0     1785 2023-05-03 20:09:31.000000 grokspeechrec-0.0.1/grokspeechrec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-05-03 20:09:31.000000 grokspeechrec-0.0.1/grokspeechrec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 20:09:31.000000 grokspeechrec-0.0.1/grokspeechrec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 20:09:31.000000 grokspeechrec-0.0.1/grokspeechrec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 20:09:31.000000 grokspeechrec-0.0.1/grokspeechrec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      583 2023-05-03 20:07:19.000000 grokspeechrec-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      134 2023-05-03 20:09:33.000000 grokspeechrec-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     2153 2023-05-03 20:06:46.000000 grokspeechrec-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:09:33.000000 grokspeechrec-0.0.1/src/
--rw-rw-rw-   0        0        0       24 2023-05-03 19:19:44.000000 grokspeechrec-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:09:33.000000 grokspeechrec-0.0.1/src/speechrec/
--rw-rw-rw-   0        0        0       43 2023-05-03 19:19:37.000000 grokspeechrec-0.0.1/src/speechrec/__init__.py
--rw-rw-rw-   0        0        0     1773 2023-05-03 18:43:10.000000 grokspeechrec-0.0.1/src/speechrec/app.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/
+-rw-rw-rw-   0        0        0     1077 2023-05-02 10:30:08.000000 grokspeechrec-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1794 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1136 2023-05-17 06:37:33.000000 grokspeechrec-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/grokspeechrec.egg-info/
+-rw-rw-rw-   0        0        0     1794 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/grokspeechrec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/grokspeechrec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/grokspeechrec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/grokspeechrec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/grokspeechrec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      592 2023-05-17 06:59:23.000000 grokspeechrec-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      134 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     2153 2023-05-17 06:37:20.000000 grokspeechrec-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/src/
+-rw-rw-rw-   0        0        0       24 2023-05-03 19:19:44.000000 grokspeechrec-0.0.2/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-17 07:17:43.000000 grokspeechrec-0.0.2/src/speechrec/
+-rw-rw-rw-   0        0        0       43 2023-05-17 06:18:40.000000 grokspeechrec-0.0.2/src/speechrec/__init__.py
+-rw-rw-rw-   0        0        0     1778 2023-05-17 06:37:50.000000 grokspeechrec-0.0.2/src/speechrec/app.py
```

### Comparing `grokspeechrec-0.0.1/LICENSE` & `grokspeechrec-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grokspeechrec-0.0.1/PKG-INFO` & `grokspeechrec-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grokspeechrec
-Version: 0.0.1
+Version: 0.0.2
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/grokspeechrec/
 Author: GROKLEARNING
 Author-email: GROKLEARNING <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/grokspeechrec
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/grokspeechrec/issues
@@ -32,15 +32,17 @@
 ```bash
 pip install --upgrade grokspeechrec
 ```
 
 ## Usage
 Once you have it installed, import the module and use it to pass Microphone Speech as shown below:
 
-    from grokspeechrec import speechrec
+```python
+from grokspeechrec import speechrec
 
-    rec = speechrec.app.Recognize()
-    output = rec.recognize(rec.model)
+rec = speechrec.app.Recognize()
+output = rec.recognize(rec.recognizer)
+```
 
 The `output` will contain the transcribed results.
```

### Comparing `grokspeechrec-0.0.1/README.md` & `grokspeechrec-0.0.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 ```bash
 pip install --upgrade grokspeechrec
 ```
 
 ## Usage
 Once you have it installed, import the module and use it to pass Microphone Speech as shown below:
 
-    from grokspeechrec import speechrec
+```python
+from grokspeechrec import speechrec
 
-    rec = speechrec.app.Recognize()
-    output = rec.recognize(rec.model)
+rec = speechrec.app.Recognize()
+output = rec.recognize(rec.recognizer)
+```
 
 The `output` will contain the transcribed results.
```

### Comparing `grokspeechrec-0.0.1/grokspeechrec.egg-info/PKG-INFO` & `grokspeechrec-0.0.2/grokspeechrec.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grokspeechrec
-Version: 0.0.1
+Version: 0.0.2
 Summary: TEST APP TMLC
 Home-page: https://github.com/visalakshi2001/grokspeechrec/
 Author: GROKLEARNING
 Author-email: GROKLEARNING <visalakshi2001@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/visalakshi2001/grokspeechrec
 Project-URL: Bug Tracker, https://github.com/visalakshi2001/grokspeechrec/issues
@@ -32,15 +32,17 @@
 ```bash
 pip install --upgrade grokspeechrec
 ```
 
 ## Usage
 Once you have it installed, import the module and use it to pass Microphone Speech as shown below:
 
-    from grokspeechrec import speechrec
+```python
+from grokspeechrec import speechrec
 
-    rec = speechrec.app.Recognize()
-    output = rec.recognize(rec.model)
+rec = speechrec.app.Recognize()
+output = rec.recognize(rec.recognizer)
+```
 
 The `output` will contain the transcribed results.
```

### Comparing `grokspeechrec-0.0.1/setup.py` & `grokspeechrec-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 with open("README.md", "rb") as fh:
     long_description = fh.read().decode("utf-8")
 
 setup(
     name='grokspeechrec',
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     author="GROKLEARNING",
     author_email='visalakshi2001@gmail.com',
     description = "TEST APP TMLC",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages= ["grokspeechrec", "grokspeechrec.speechrec"],
```

### Comparing `grokspeechrec-0.0.1/src/speechrec/app.py` & `grokspeechrec-0.0.2/src/speechrec/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         self.model = Model(os.path.join(MODEL_PTH, "vosk-model-en-us-daanzu-20200905-lgraph"))
         self.recognizer = KaldiRecognizer(self.model,16000)
 
     def __str__(self):
         return """Class to initiate speech recognizer"""
 
-    def model(self):
+    def recognizer(self):
         return self.recognizer
 
     @classmethod
     def recognize(self, recognizer_model):
         mic = pyaudio.PyAudio()
         stream = mic.open(rate=16000, channels=1, format=pyaudio.paInt16,input=True, frames_per_buffer=8192)
         stream.start_stream()
```

