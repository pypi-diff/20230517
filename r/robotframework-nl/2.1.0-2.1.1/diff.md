# Comparing `tmp/robotframework-nl-2.1.0.tar.gz` & `tmp/robotframework-nl-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-nl-2.1.0.tar", last modified: Fri Jan 13 16:42:04 2023, max compression
+gzip compressed data, was "robotframework-nl-2.1.1.tar", last modified: Wed May 17 13:57:45 2023, max compression
```

## Comparing `robotframework-nl-2.1.0.tar` & `robotframework-nl-2.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-13 16:42:04.278889 robotframework-nl-2.1.0/
--rw-rw-rw-   0        0        0     1548 2022-08-09 15:13:59.000000 robotframework-nl-2.1.0/LICENSE
--rw-rw-rw-   0        0        0     9699 2023-01-13 16:42:04.278889 robotframework-nl-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7351 2022-10-04 13:11:45.000000 robotframework-nl-2.1.0/README.md
--rw-rw-rw-   0        0        0      808 2023-01-13 16:40:22.000000 robotframework-nl-2.1.0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-01-13 16:42:04.264490 robotframework-nl-2.1.0/robotframework_nl.egg-info/
--rw-rw-rw-   0        0        0     9699 2023-01-13 16:42:04.000000 robotframework-nl-2.1.0/robotframework_nl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2023-01-13 16:42:04.000000 robotframework-nl-2.1.0/robotframework_nl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-13 16:42:04.000000 robotframework-nl-2.1.0/robotframework_nl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-01-13 16:42:04.000000 robotframework-nl-2.1.0/robotframework_nl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-01-13 16:42:04.000000 robotframework-nl-2.1.0/robotframework_nl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-13 16:42:04.276538 robotframework-nl-2.1.0/robotnl/
--rw-rw-rw-   0        0        0    10766 2022-08-09 15:13:59.000000 robotframework-nl-2.1.0/robotnl/CheckOperator.py
--rw-rw-rw-   0        0        0    16775 2023-01-13 16:40:22.000000 robotframework-nl-2.1.0/robotnl/RobotChecks.py
--rw-rw-rw-   0        0        0     1939 2022-10-04 13:11:45.000000 robotframework-nl-2.1.0/robotnl/__init__.py
--rw-rw-rw-   0        0        0     5166 2022-10-04 13:11:45.000000 robotframework-nl-2.1.0/robotnl/inline_keywords.py
--rw-rw-rw-   0        0        0       19 2023-01-13 16:40:22.000000 robotframework-nl-2.1.0/robotnl/version.py
--rw-rw-rw-   0        0        0       42 2023-01-13 16:42:04.278889 robotframework-nl-2.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-17 13:57:45.647747 robotframework-nl-2.1.1/
+-rw-rw-rw-   0        0        0     1548 2022-08-09 15:13:59.000000 robotframework-nl-2.1.1/LICENSE
+-rw-rw-rw-   0        0        0     9699 2023-05-17 13:57:45.646747 robotframework-nl-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7351 2022-10-04 13:11:45.000000 robotframework-nl-2.1.1/README.md
+-rw-rw-rw-   0        0        0      808 2023-05-17 13:53:27.000000 robotframework-nl-2.1.1/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-17 13:57:45.624585 robotframework-nl-2.1.1/robotframework_nl.egg-info/
+-rw-rw-rw-   0        0        0     9699 2023-05-17 13:57:45.000000 robotframework-nl-2.1.1/robotframework_nl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-05-17 13:57:45.000000 robotframework-nl-2.1.1/robotframework_nl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 13:57:45.000000 robotframework-nl-2.1.1/robotframework_nl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-17 13:57:45.000000 robotframework-nl-2.1.1/robotframework_nl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-17 13:57:45.000000 robotframework-nl-2.1.1/robotframework_nl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-17 13:57:45.646747 robotframework-nl-2.1.1/robotnl/
+-rw-rw-rw-   0        0        0    10766 2022-08-09 15:13:59.000000 robotframework-nl-2.1.1/robotnl/CheckOperator.py
+-rw-rw-rw-   0        0        0    16866 2023-05-17 13:53:27.000000 robotframework-nl-2.1.1/robotnl/RobotChecks.py
+-rw-rw-rw-   0        0        0     1939 2022-10-04 13:11:45.000000 robotframework-nl-2.1.1/robotnl/__init__.py
+-rw-rw-rw-   0        0        0     5166 2022-10-04 13:11:45.000000 robotframework-nl-2.1.1/robotnl/inline_keywords.py
+-rw-rw-rw-   0        0        0       19 2023-05-17 13:53:27.000000 robotframework-nl-2.1.1/robotnl/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-17 13:57:45.647747 robotframework-nl-2.1.1/setup.cfg
```

### Comparing `robotframework-nl-2.1.0/LICENSE` & `robotframework-nl-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-nl-2.1.0/PKG-INFO` & `robotframework-nl-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-nl
-Version: 2.1.0
+Version: 2.1.1
 Summary: robotnl is a proving ground to boost Robot framework closer to Natural Language.
 Author-email: Johan Foederer <github@famfoe.nl>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, J. Foederer
         All rights reserved.
```

### Comparing `robotframework-nl-2.1.0/README.md` & `robotframework-nl-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-nl-2.1.0/pyproject.toml` & `robotframework-nl-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "robotframework-nl"
-version = "2.1.0"
+version = "2.1.1"
 description = "robotnl is a proving ground to boost Robot framework closer to Natural Language."
 readme = "README.md"
 authors = [{ name = "Johan Foederer", email = "github@famfoe.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3",
```

### Comparing `robotframework-nl-2.1.0/robotframework_nl.egg-info/PKG-INFO` & `robotframework-nl-2.1.1/robotframework_nl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-nl
-Version: 2.1.0
+Version: 2.1.1
 Summary: robotnl is a proving ground to boost Robot framework closer to Natural Language.
 Author-email: Johan Foederer <github@famfoe.nl>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, J. Foederer
         All rights reserved.
```

### Comparing `robotframework-nl-2.1.0/robotnl/CheckOperator.py` & `robotframework-nl-2.1.1/robotnl/CheckOperator.py`

 * *Files identical despite different names*

### Comparing `robotframework-nl-2.1.0/robotnl/RobotChecks.py` & `robotframework-nl-2.1.1/robotnl/RobotChecks.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,19 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import time
-from tkinter import messagebox, simpledialog, Tk
+try:
+    import tkinter
+    from tkinter import messagebox, simpledialog
+except ImportError:
+    tkinter = False
 
 from robot.libraries.BuiltIn import BuiltIn
 from robot.utils import timestr_to_secs, secs_to_timestr
 from .inline_keywords import is_keyword
 
 class CheckFailed(RuntimeError):
     ROBOT_CONTINUE_ON_FAILURE = True
@@ -43,20 +47,20 @@
 class RobotChecks:
     ROBOT_LIBRARY_SCOPE = "GLOBAL"
     def __init__(self):
         self.__gui = None
 
     @property
     def _gui(self):
-        if self.__gui is not None:
+        if self.__gui is not None or not tkinter:
             return self.__gui
         try:
             # Create and hide a Gui.
             # Enables the use for Tkiniter message boxes without displaying a main window
-            root = Tk()
+            root = tkinter.Tk()
             root.withdraw()
             self.__gui = True
         except:
             self.__gui = False
         return self.__gui
 
     def check_precondition(self, *args):
```

### Comparing `robotframework-nl-2.1.0/robotnl/__init__.py` & `robotframework-nl-2.1.1/robotnl/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-nl-2.1.0/robotnl/inline_keywords.py` & `robotframework-nl-2.1.1/robotnl/inline_keywords.py`

 * *Files identical despite different names*

