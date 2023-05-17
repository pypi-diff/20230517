# Comparing `tmp/pyintegralall-0.0.8.tar.gz` & `tmp/pyintegralall-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintegralall-0.0.8.tar", last modified: Thu Feb 23 10:20:17 2023, max compression
+gzip compressed data, was "pyintegralall-0.0.9.tar", last modified: Wed May 17 10:17:25 2023, max compression
```

## Comparing `pyintegralall-0.0.8.tar` & `pyintegralall-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 10:20:17.716858 pyintegralall-0.0.8/
--rw-r--r--   0 jean      (1000) users      (100)      894 2023-02-09 12:42:43.000000 pyintegralall-0.0.8/LICENSE.txt
--rw-r--r--   0 jean      (1000) users      (100)    10545 2023-02-23 10:20:17.716858 pyintegralall-0.0.8/PKG-INFO
--rwxrwxrwx   0 jean      (1000) users      (100)    10077 2023-02-23 10:16:50.000000 pyintegralall-0.0.8/README.md
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 10:20:17.716858 pyintegralall-0.0.8/pyintegralall.egg-info/
--rw-r--r--   0 jean      (1000) users      (100)    10545 2023-02-23 10:20:17.000000 pyintegralall-0.0.8/pyintegralall.egg-info/PKG-INFO
--rw-r--r--   0 jean      (1000) users      (100)      399 2023-02-23 10:20:17.000000 pyintegralall-0.0.8/pyintegralall.egg-info/SOURCES.txt
--rw-r--r--   0 jean      (1000) users      (100)        1 2023-02-23 10:20:17.000000 pyintegralall-0.0.8/pyintegralall.egg-info/dependency_links.txt
--rw-r--r--   0 jean      (1000) users      (100)       17 2023-02-23 10:20:17.000000 pyintegralall-0.0.8/pyintegralall.egg-info/requires.txt
--rw-r--r--   0 jean      (1000) users      (100)       14 2023-02-23 10:20:17.000000 pyintegralall-0.0.8/pyintegralall.egg-info/top_level.txt
--rw-r--r--   0 jean      (1000) users      (100)       38 2023-02-23 10:20:17.716858 pyintegralall-0.0.8/setup.cfg
--rw-r--r--   0 jean      (1000) users      (100)     1232 2023-02-23 10:19:05.000000 pyintegralall-0.0.8/setup.py
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 10:20:17.716858 pyintegralall-0.0.8/src/
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 10:20:17.716858 pyintegralall-0.0.8/src/fortran/
--rwxr-xr-x   0 jean      (1000) users      (100)     1473 2023-02-16 10:58:20.000000 pyintegralall-0.0.8/src/fortran/DataTypes.f90
--rw-r--r--   0 jean      (1000) users      (100)     7359 2023-02-12 19:36:00.000000 pyintegralall-0.0.8/src/fortran/GaussLegendreQuadrature.f90
--rw-r--r--   0 jean      (1000) users      (100)    43798 2023-02-17 10:40:16.000000 pyintegralall-0.0.8/src/fortran/IntegralALL.f90
--rwxr-xr-x   0 jean      (1000) users      (100)    11154 2023-02-12 17:59:45.000000 pyintegralall-0.0.8/src/fortran/LINinterpol.f90
-drwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-23 10:20:17.716858 pyintegralall-0.0.8/src/python/
--rw-r--r--   0 jean      (1000) users      (100)     1784 2023-02-09 12:42:44.000000 pyintegralall-0.0.8/src/python/PyIntegralALL.py
--rwxr-xr-x   0 jean      (1000) users      (100)        0 2023-02-09 12:42:44.000000 pyintegralall-0.0.8/src/python/__init__.py
--rw-r--r--   0 jean      (1000) users      (100)        6 2023-02-23 10:18:57.000000 pyintegralall-0.0.8/version.txt
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-17 10:17:25.537027 pyintegralall-0.0.9/
+-rw-r--r--   0 jeangomes   (501) staff       (20)      894 2023-05-16 15:25:46.000000 pyintegralall-0.0.9/LICENSE.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)    10709 2023-05-17 10:17:25.536829 pyintegralall-0.0.9/PKG-INFO
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    10155 2023-05-17 10:15:54.000000 pyintegralall-0.0.9/README.md
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-17 10:17:25.535773 pyintegralall-0.0.9/pyintegralall.egg-info/
+-rw-r--r--   0 jeangomes   (501) staff       (20)    10709 2023-05-17 10:17:25.000000 pyintegralall-0.0.9/pyintegralall.egg-info/PKG-INFO
+-rw-r--r--   0 jeangomes   (501) staff       (20)      399 2023-05-17 10:17:25.000000 pyintegralall-0.0.9/pyintegralall.egg-info/SOURCES.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)        1 2023-05-17 10:17:25.000000 pyintegralall-0.0.9/pyintegralall.egg-info/dependency_links.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)       17 2023-05-17 10:17:25.000000 pyintegralall-0.0.9/pyintegralall.egg-info/requires.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)       14 2023-05-17 10:17:25.000000 pyintegralall-0.0.9/pyintegralall.egg-info/top_level.txt
+-rw-r--r--   0 jeangomes   (501) staff       (20)       38 2023-05-17 10:17:25.537077 pyintegralall-0.0.9/setup.cfg
+-rw-r--r--   0 jeangomes   (501) staff       (20)     1350 2023-05-17 10:17:09.000000 pyintegralall-0.0.9/setup.py
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-17 10:17:25.534362 pyintegralall-0.0.9/src/
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-17 10:17:25.536371 pyintegralall-0.0.9/src/fortran/
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)     1473 2023-05-16 15:25:46.000000 pyintegralall-0.0.9/src/fortran/DataTypes.f90
+-rw-r--r--   0 jeangomes   (501) staff       (20)     7359 2023-05-16 15:25:46.000000 pyintegralall-0.0.9/src/fortran/GaussLegendreQuadrature.f90
+-rw-r--r--   0 jeangomes   (501) staff       (20)    43798 2023-05-16 15:25:46.000000 pyintegralall-0.0.9/src/fortran/IntegralALL.f90
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)    11154 2023-05-16 15:25:46.000000 pyintegralall-0.0.9/src/fortran/LINinterpol.f90
+drwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-17 10:17:25.536628 pyintegralall-0.0.9/src/python/
+-rw-r--r--   0 jeangomes   (501) staff       (20)     1784 2023-05-16 15:25:46.000000 pyintegralall-0.0.9/src/python/PyIntegralALL.py
+-rwxr-xr-x   0 jeangomes   (501) staff       (20)        0 2023-05-16 15:25:46.000000 pyintegralall-0.0.9/src/python/__init__.py
+-rw-r--r--   0 jeangomes   (501) staff       (20)        6 2023-05-16 15:29:55.000000 pyintegralall-0.0.9/version.txt
```

### Comparing `pyintegralall-0.0.8/LICENSE.txt` & `pyintegralall-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyintegralall-0.0.8/PKG-INFO` & `pyintegralall-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Metadata-Version: 2.1
 Name: pyintegralall
-Version: 0.0.8
-Summary: Numerical integration using several methods
-Home-page: https://github.com/neutrinomuon/IntegralALL
+Version: 0.0.9
+Summary: Integrate arrays, functions numerically using different methods in Python. Original Fortran 2003+ legacy routines date back to 2003-2004. Read the LICENSE.txt file.
+Home-page: https://github.com/neutrinomuon/pyintegralall
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Fortran
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-### IntegralALL
+### pyintegralall
 ####  A Fortran legacy package to easy integrate numerically
-email: antineutrinomuon@gmail.com, jean@astro.up.pt
+email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 © Copyright ®
 
 J.G. - Jean Gomes
 
 <hr>
 
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)<br>
 [![python3](https://img.shields.io/pypi/pyversions/pyintegralall)](https://img.shields.io/pypi/pyversions/pyintegralall)
 [![badgetlicense](https://anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)](https://anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)
 
 <hr>
 
 <div align="center">
-<img src='https://github.com/neutrinomuon/IntegralALL/blob/main/tutorials/Definite_Integral.png?raw=true' width="50%">
+<img src='https://github.com/neutrinomuon/pyintegralall/blob/main/tutorials/Definite_Integral.png?raw=true' width="50%">
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
 Integrate arrays, functions numerically using different
 methods. Original Fortran 2003+ routines date back to 2003-2004. Read the
-<a href='https://github.com/neutrinomuon/IntegralALL/blob/main/LICENSE.txt'>LICENSE.txt</a> file. Definite integrals are mathematical calculations that allow
+<a href='https://github.com/neutrinomuon/pyintegralall/blob/main/LICENSE.txt'>LICENSE.txt</a> file. Definite integrals are mathematical calculations that allow
 us to find the area under a curve between two defined points on the x-axis. In
 other words, they give us the total accumulated value of a function over an
 interval. Definite integrals are used in various fields, such as physics,
 engineering, and finance, to solve real-world problems, such as calculating
 the total distance travelled by a moving object or the total profit of a
 company over a certain period.
 
@@ -83,15 +81,15 @@
 </code>
 </pre>
 OBS.: Linux, OS-X ad Windows pre-compilations available in conda.
 
 You can also clone the repository and install by yourself in your machine:
 <pre>
 <code>
-git clone https://github.com/neutrinomuon/IntegralALL
+git clone https://github.com/neutrinomuon/pyintegralall
 python setup.py install
 </code>
 </pre>
 
 <hr>
 
 #### <b>METHODS</b>
@@ -122,15 +120,15 @@
 
 #### <b>STRUCTURE</b>
 
 The main structure of the directories and files are:
 
 <pre>
 <code>
-IntegralALL
+pyintegralall
 ├── pyintegralall
 │   ├── win-32
 │   │   └── pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 │   ├── linux-armv7l
 │   │   └── pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 │   ├── win-arm64
 │   │   └── pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
@@ -185,18 +183,18 @@
 │   ├── SOURCES.txt
 │   ├── top_level.txt
 │   └── requires.txt
 ├── LICENSE.txt
 ├── setup.py
 ├── tutorials
 │   ├── Definite_Integral.png
-│   ├── Example1 - IntegralALL.ipynb
+│   ├── Example1 - pyintegralall.ipynb
 │   ├── Definite_Integral.py
 │   └── .ipynb_checkpoints
-│       └── Example1 - IntegralALL-checkpoint.ipynb
+│       └── Example1 - pyintegralall-checkpoint.ipynb
 ├── src
 │   ├── python
 │   │   ├── __init__.py
 │   │   └── PyIntegralALL.py
 │   └── fortran
 │       ├── LINinterpol.cpython-39-darwin.so
 │       ├── GaussLegendreQuadrature.cpython-311-darwin.so
@@ -261,9 +259,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: pyintegralall Version: 0.0.8 Summary: Numerical
-integration using several methods Home-page: https://github.com/neutrinomuon/
-IntegralALL Author: Jean Gomes Author-email: antineutrinomuon@gmail.com
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Fortran Classifier: Operating System
-:: OS Independent Description-Content-Type: text/markdown License-File:
-LICENSE.txt ### IntegralALL #### A Fortran legacy package to easy integrate
-numerically email: antineutrinomuon@gmail.com, jean@astro.up.pt Â© Copyright Â®
-J.G. - Jean Gomes
+Metadata-Version: 2.1 Name: pyintegralall Version: 0.0.9 Summary: Integrate
+arrays, functions numerically using different methods in Python. Original
+Fortran 2003+ legacy routines date back to 2003-2004. Read the LICENSE.txt
+file. Home-page: https://github.com/neutrinomuon/pyintegralall Author: Jean
+Gomes Author-email: antineutrinomuon@gmail.com Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Fortran Classifier:
+Operating System :: OS Independent Description-Content-Type: text/markdown
+License-File: LICENSE.txt ### pyintegralall #### A Fortran legacy package to
+easy integrate numerically email: [antineutrinomuon@gmail.com](mailto:
+antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt) Â©
+Copyright Â® J.G. - Jean Gomes
 ===============================================================================
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)
 [![python3](https://img.shields.io/pypi/pyversions/pyintegralall)](https://
 img.shields.io/pypi/pyversions/pyintegralall) [![badgetlicense](https://
 anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)](https://
 anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)
 ===============================================================================
-       [https://github.com/neutrinomuon/IntegralALL/blob/main/tutorials/
+      [https://github.com/neutrinomuon/pyintegralall/blob/main/tutorials/
                         Definite_Integral.png?raw=true]
 ===============================================================================
 #### RESUME Integrate arrays, functions numerically using different methods.
 Original Fortran 2003+ routines date back to 2003-2004. Read the LICENSE.txt
 file. Definite integrals are mathematical calculations that allow us to find
 the area under a curve between two defined points on the x-axis. In other
 words, they give us the total accumulated value of a function over an interval.
@@ -51,15 +53,15 @@
 platforms.svg )](https://anaconda.org/neutrinomuon/pyintegralall/badges/
 platforms.svg)
 
 conda install -c neutrinomuon pyintegralall
 OBS.: Linux, OS-X ad Windows pre-compilations available in conda. You can also
 clone the repository and install by yourself in your machine:
 
-git clone https://github.com/neutrinomuon/IntegralALL
+git clone https://github.com/neutrinomuon/pyintegralall
 python setup.py install
 ===============================================================================
 #### METHODS The methods are given by Int_Type and may be summarized bellow:
 Int_Type Type Description
 0        R    Right rectangle Integral
 1        L    Left rectangle Integral
 2        T    Trapezoidal rule
@@ -71,15 +73,15 @@
 #### REFERENCES
    1. William H. Press, Saul A. Teukolsky, William T. Vetterling, and Brian P.
       Flannery. Numerical Recipes: The Art of Scientific Computing. William
       ISBN: 978-0521880688. Link: https://www.nr.com/
 ===============================================================================
 #### STRUCTURE The main structure of the directories and files are:
 
-IntegralALL
+pyintegralall
 âââ pyintegralall
 â   âââ win-32
 â   â   âââ pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 â   âââ linux-armv7l
 â   â   âââ pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 â   âââ win-arm64
 â   â   âââ pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
@@ -134,18 +136,18 @@
 â   âââ SOURCES.txt
 â   âââ top_level.txt
 â   âââ requires.txt
 âââ LICENSE.txt
 âââ setup.py
 âââ tutorials
 â   âââ Definite_Integral.png
-â   âââ Example1 - IntegralALL.ipynb
+â   âââ Example1 - pyintegralall.ipynb
 â   âââ Definite_Integral.py
 â   âââ .ipynb_checkpoints
-â       âââ Example1 - IntegralALL-checkpoint.ipynb
+â       âââ Example1 - pyintegralall-checkpoint.ipynb
 âââ src
 â   âââ python
 â   â   âââ __init__.py
 â   â   âââ PyIntegralALL.py
 â   âââ fortran
 â       âââ LINinterpol.cpython-39-darwin.so
 â       âââ GaussLegendreQuadrature.cpython-311-darwin.so
```

### Comparing `pyintegralall-0.0.8/README.md` & `pyintegralall-0.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-### IntegralALL
+### pyintegralall
 ####  A Fortran legacy package to easy integrate numerically
-email: antineutrinomuon@gmail.com, jean@astro.up.pt
+email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 © Copyright ®
 
 J.G. - Jean Gomes
 
 <hr>
 
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)<br>
 [![python3](https://img.shields.io/pypi/pyversions/pyintegralall)](https://img.shields.io/pypi/pyversions/pyintegralall)
 [![badgetlicense](https://anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)](https://anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)
 
 <hr>
 
 <div align="center">
-<img src='https://github.com/neutrinomuon/IntegralALL/blob/main/tutorials/Definite_Integral.png?raw=true' width="50%">
+<img src='https://github.com/neutrinomuon/pyintegralall/blob/main/tutorials/Definite_Integral.png?raw=true' width="50%">
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
 Integrate arrays, functions numerically using different
 methods. Original Fortran 2003+ routines date back to 2003-2004. Read the
-<a href='https://github.com/neutrinomuon/IntegralALL/blob/main/LICENSE.txt'>LICENSE.txt</a> file. Definite integrals are mathematical calculations that allow
+<a href='https://github.com/neutrinomuon/pyintegralall/blob/main/LICENSE.txt'>LICENSE.txt</a> file. Definite integrals are mathematical calculations that allow
 us to find the area under a curve between two defined points on the x-axis. In
 other words, they give us the total accumulated value of a function over an
 interval. Definite integrals are used in various fields, such as physics,
 engineering, and finance, to solve real-world problems, such as calculating
 the total distance travelled by a moving object or the total profit of a
 company over a certain period.
 
@@ -68,15 +68,15 @@
 </code>
 </pre>
 OBS.: Linux, OS-X ad Windows pre-compilations available in conda.
 
 You can also clone the repository and install by yourself in your machine:
 <pre>
 <code>
-git clone https://github.com/neutrinomuon/IntegralALL
+git clone https://github.com/neutrinomuon/pyintegralall
 python setup.py install
 </code>
 </pre>
 
 <hr>
 
 #### <b>METHODS</b>
@@ -107,15 +107,15 @@
 
 #### <b>STRUCTURE</b>
 
 The main structure of the directories and files are:
 
 <pre>
 <code>
-IntegralALL
+pyintegralall
 ├── pyintegralall
 │   ├── win-32
 │   │   └── pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 │   ├── linux-armv7l
 │   │   └── pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 │   ├── win-arm64
 │   │   └── pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
@@ -170,18 +170,18 @@
 │   ├── SOURCES.txt
 │   ├── top_level.txt
 │   └── requires.txt
 ├── LICENSE.txt
 ├── setup.py
 ├── tutorials
 │   ├── Definite_Integral.png
-│   ├── Example1 - IntegralALL.ipynb
+│   ├── Example1 - pyintegralall.ipynb
 │   ├── Definite_Integral.py
 │   └── .ipynb_checkpoints
-│       └── Example1 - IntegralALL-checkpoint.ipynb
+│       └── Example1 - pyintegralall-checkpoint.ipynb
 ├── src
 │   ├── python
 │   │   ├── __init__.py
 │   │   └── PyIntegralALL.py
 │   └── fortran
 │       ├── LINinterpol.cpython-39-darwin.so
 │       ├── GaussLegendreQuadrature.cpython-311-darwin.so
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-### IntegralALL #### A Fortran legacy package to easy integrate numerically
-email: antineutrinomuon@gmail.com, jean@astro.up.pt Â© Copyright Â® J.G. - Jean
-Gomes
+### pyintegralall #### A Fortran legacy package to easy integrate numerically
+email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com),
+[jean@astro.up.pt](mailto:jean@astro.up.pt) Â© Copyright Â® J.G. - Jean Gomes
 ===============================================================================
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)
 [![python3](https://img.shields.io/pypi/pyversions/pyintegralall)](https://
 img.shields.io/pypi/pyversions/pyintegralall) [![badgetlicense](https://
 anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)](https://
 anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)
 ===============================================================================
-       [https://github.com/neutrinomuon/IntegralALL/blob/main/tutorials/
+      [https://github.com/neutrinomuon/pyintegralall/blob/main/tutorials/
                         Definite_Integral.png?raw=true]
 ===============================================================================
 #### RESUME Integrate arrays, functions numerically using different methods.
 Original Fortran 2003+ routines date back to 2003-2004. Read the LICENSE.txt
 file. Definite integrals are mathematical calculations that allow us to find
 the area under a curve between two defined points on the x-axis. In other
 words, they give us the total accumulated value of a function over an interval.
@@ -45,15 +45,15 @@
 platforms.svg )](https://anaconda.org/neutrinomuon/pyintegralall/badges/
 platforms.svg)
 
 conda install -c neutrinomuon pyintegralall
 OBS.: Linux, OS-X ad Windows pre-compilations available in conda. You can also
 clone the repository and install by yourself in your machine:
 
-git clone https://github.com/neutrinomuon/IntegralALL
+git clone https://github.com/neutrinomuon/pyintegralall
 python setup.py install
 ===============================================================================
 #### METHODS The methods are given by Int_Type and may be summarized bellow:
 Int_Type Type Description
 0        R    Right rectangle Integral
 1        L    Left rectangle Integral
 2        T    Trapezoidal rule
@@ -65,15 +65,15 @@
 #### REFERENCES
    1. William H. Press, Saul A. Teukolsky, William T. Vetterling, and Brian P.
       Flannery. Numerical Recipes: The Art of Scientific Computing. William
       ISBN: 978-0521880688. Link: https://www.nr.com/
 ===============================================================================
 #### STRUCTURE The main structure of the directories and files are:
 
-IntegralALL
+pyintegralall
 âââ pyintegralall
 â   âââ win-32
 â   â   âââ pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 â   âââ linux-armv7l
 â   â   âââ pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 â   âââ win-arm64
 â   â   âââ pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
@@ -128,18 +128,18 @@
 â   âââ SOURCES.txt
 â   âââ top_level.txt
 â   âââ requires.txt
 âââ LICENSE.txt
 âââ setup.py
 âââ tutorials
 â   âââ Definite_Integral.png
-â   âââ Example1 - IntegralALL.ipynb
+â   âââ Example1 - pyintegralall.ipynb
 â   âââ Definite_Integral.py
 â   âââ .ipynb_checkpoints
-â       âââ Example1 - IntegralALL-checkpoint.ipynb
+â       âââ Example1 - pyintegralall-checkpoint.ipynb
 âââ src
 â   âââ python
 â   â   âââ __init__.py
 â   â   âââ PyIntegralALL.py
 â   âââ fortran
 â       âââ LINinterpol.cpython-39-darwin.so
 â       âââ GaussLegendreQuadrature.cpython-311-darwin.so
```

### Comparing `pyintegralall-0.0.8/pyintegralall.egg-info/PKG-INFO` & `pyintegralall-0.0.9/pyintegralall.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Metadata-Version: 2.1
 Name: pyintegralall
-Version: 0.0.8
-Summary: Numerical integration using several methods
-Home-page: https://github.com/neutrinomuon/IntegralALL
+Version: 0.0.9
+Summary: Integrate arrays, functions numerically using different methods in Python. Original Fortran 2003+ legacy routines date back to 2003-2004. Read the LICENSE.txt file.
+Home-page: https://github.com/neutrinomuon/pyintegralall
 Author: Jean Gomes
 Author-email: antineutrinomuon@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Fortran
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-### IntegralALL
+### pyintegralall
 ####  A Fortran legacy package to easy integrate numerically
-email: antineutrinomuon@gmail.com, jean@astro.up.pt
+email: [antineutrinomuon@gmail.com](mailto:antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt)
 
 © Copyright ®
 
 J.G. - Jean Gomes
 
 <hr>
 
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)<br>
 [![python3](https://img.shields.io/pypi/pyversions/pyintegralall)](https://img.shields.io/pypi/pyversions/pyintegralall)
 [![badgetlicense](https://anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)](https://anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)
 
 <hr>
 
 <div align="center">
-<img src='https://github.com/neutrinomuon/IntegralALL/blob/main/tutorials/Definite_Integral.png?raw=true' width="50%">
+<img src='https://github.com/neutrinomuon/pyintegralall/blob/main/tutorials/Definite_Integral.png?raw=true' width="50%">
 </div>
 
 <hr>
 
 #### <b>RESUME</b>
 
 Integrate arrays, functions numerically using different
 methods. Original Fortran 2003+ routines date back to 2003-2004. Read the
-<a href='https://github.com/neutrinomuon/IntegralALL/blob/main/LICENSE.txt'>LICENSE.txt</a> file. Definite integrals are mathematical calculations that allow
+<a href='https://github.com/neutrinomuon/pyintegralall/blob/main/LICENSE.txt'>LICENSE.txt</a> file. Definite integrals are mathematical calculations that allow
 us to find the area under a curve between two defined points on the x-axis. In
 other words, they give us the total accumulated value of a function over an
 interval. Definite integrals are used in various fields, such as physics,
 engineering, and finance, to solve real-world problems, such as calculating
 the total distance travelled by a moving object or the total profit of a
 company over a certain period.
 
@@ -83,15 +81,15 @@
 </code>
 </pre>
 OBS.: Linux, OS-X ad Windows pre-compilations available in conda.
 
 You can also clone the repository and install by yourself in your machine:
 <pre>
 <code>
-git clone https://github.com/neutrinomuon/IntegralALL
+git clone https://github.com/neutrinomuon/pyintegralall
 python setup.py install
 </code>
 </pre>
 
 <hr>
 
 #### <b>METHODS</b>
@@ -122,15 +120,15 @@
 
 #### <b>STRUCTURE</b>
 
 The main structure of the directories and files are:
 
 <pre>
 <code>
-IntegralALL
+pyintegralall
 ├── pyintegralall
 │   ├── win-32
 │   │   └── pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 │   ├── linux-armv7l
 │   │   └── pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 │   ├── win-arm64
 │   │   └── pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
@@ -185,18 +183,18 @@
 │   ├── SOURCES.txt
 │   ├── top_level.txt
 │   └── requires.txt
 ├── LICENSE.txt
 ├── setup.py
 ├── tutorials
 │   ├── Definite_Integral.png
-│   ├── Example1 - IntegralALL.ipynb
+│   ├── Example1 - pyintegralall.ipynb
 │   ├── Definite_Integral.py
 │   └── .ipynb_checkpoints
-│       └── Example1 - IntegralALL-checkpoint.ipynb
+│       └── Example1 - pyintegralall-checkpoint.ipynb
 ├── src
 │   ├── python
 │   │   ├── __init__.py
 │   │   └── PyIntegralALL.py
 │   └── fortran
 │       ├── LINinterpol.cpython-39-darwin.so
 │       ├── GaussLegendreQuadrature.cpython-311-darwin.so
@@ -261,9 +259,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,26 @@
-Metadata-Version: 2.1 Name: pyintegralall Version: 0.0.8 Summary: Numerical
-integration using several methods Home-page: https://github.com/neutrinomuon/
-IntegralALL Author: Jean Gomes Author-email: antineutrinomuon@gmail.com
-License: UNKNOWN Platform: UNKNOWN Classifier: Programming Language :: Python
-:: 3 Classifier: Programming Language :: Fortran Classifier: Operating System
-:: OS Independent Description-Content-Type: text/markdown License-File:
-LICENSE.txt ### IntegralALL #### A Fortran legacy package to easy integrate
-numerically email: antineutrinomuon@gmail.com, jean@astro.up.pt Â© Copyright Â®
-J.G. - Jean Gomes
+Metadata-Version: 2.1 Name: pyintegralall Version: 0.0.9 Summary: Integrate
+arrays, functions numerically using different methods in Python. Original
+Fortran 2003+ legacy routines date back to 2003-2004. Read the LICENSE.txt
+file. Home-page: https://github.com/neutrinomuon/pyintegralall Author: Jean
+Gomes Author-email: antineutrinomuon@gmail.com Classifier: Programming Language
+:: Python :: 3 Classifier: Programming Language :: Fortran Classifier:
+Operating System :: OS Independent Description-Content-Type: text/markdown
+License-File: LICENSE.txt ### pyintegralall #### A Fortran legacy package to
+easy integrate numerically email: [antineutrinomuon@gmail.com](mailto:
+antineutrinomuon@gmail.com), [jean@astro.up.pt](mailto:jean@astro.up.pt) Â©
+Copyright Â® J.G. - Jean Gomes
 ===============================================================================
 ![My Skills](https://skillicons.dev/icons?i=python,fortran,c,numpy&theme=light)
 [![python3](https://img.shields.io/pypi/pyversions/pyintegralall)](https://
 img.shields.io/pypi/pyversions/pyintegralall) [![badgetlicense](https://
 anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)](https://
 anaconda.org/neutrinomuon/pyintegralall/badges/license.svg)
 ===============================================================================
-       [https://github.com/neutrinomuon/IntegralALL/blob/main/tutorials/
+      [https://github.com/neutrinomuon/pyintegralall/blob/main/tutorials/
                         Definite_Integral.png?raw=true]
 ===============================================================================
 #### RESUME Integrate arrays, functions numerically using different methods.
 Original Fortran 2003+ routines date back to 2003-2004. Read the LICENSE.txt
 file. Definite integrals are mathematical calculations that allow us to find
 the area under a curve between two defined points on the x-axis. In other
 words, they give us the total accumulated value of a function over an interval.
@@ -51,15 +53,15 @@
 platforms.svg )](https://anaconda.org/neutrinomuon/pyintegralall/badges/
 platforms.svg)
 
 conda install -c neutrinomuon pyintegralall
 OBS.: Linux, OS-X ad Windows pre-compilations available in conda. You can also
 clone the repository and install by yourself in your machine:
 
-git clone https://github.com/neutrinomuon/IntegralALL
+git clone https://github.com/neutrinomuon/pyintegralall
 python setup.py install
 ===============================================================================
 #### METHODS The methods are given by Int_Type and may be summarized bellow:
 Int_Type Type Description
 0        R    Right rectangle Integral
 1        L    Left rectangle Integral
 2        T    Trapezoidal rule
@@ -71,15 +73,15 @@
 #### REFERENCES
    1. William H. Press, Saul A. Teukolsky, William T. Vetterling, and Brian P.
       Flannery. Numerical Recipes: The Art of Scientific Computing. William
       ISBN: 978-0521880688. Link: https://www.nr.com/
 ===============================================================================
 #### STRUCTURE The main structure of the directories and files are:
 
-IntegralALL
+pyintegralall
 âââ pyintegralall
 â   âââ win-32
 â   â   âââ pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 â   âââ linux-armv7l
 â   â   âââ pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
 â   âââ win-arm64
 â   â   âââ pyintegralall-0.0.5-py39hfeaa757_0.tar.bz2
@@ -134,18 +136,18 @@
 â   âââ SOURCES.txt
 â   âââ top_level.txt
 â   âââ requires.txt
 âââ LICENSE.txt
 âââ setup.py
 âââ tutorials
 â   âââ Definite_Integral.png
-â   âââ Example1 - IntegralALL.ipynb
+â   âââ Example1 - pyintegralall.ipynb
 â   âââ Definite_Integral.py
 â   âââ .ipynb_checkpoints
-â       âââ Example1 - IntegralALL-checkpoint.ipynb
+â       âââ Example1 - pyintegralall-checkpoint.ipynb
 âââ src
 â   âââ python
 â   â   âââ __init__.py
 â   â   âââ PyIntegralALL.py
 â   âââ fortran
 â       âââ LINinterpol.cpython-39-darwin.so
 â       âââ GaussLegendreQuadrature.cpython-311-darwin.so
```

### Comparing `pyintegralall-0.0.8/setup.py` & `pyintegralall-0.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,23 +5,23 @@
     long_description = fh.read()
 
 ext1 = Extension(  name='pyintegralall.flib',
                    sources=['src/fortran/DataTypes.f90','src/fortran/LINinterpol.f90','src/fortran/GaussLegendreQuadrature.f90','src/fortran/IntegralALL.f90'],
                  )
     
 setup( name='pyintegralall',
-       version='0.0.8',
+       version='0.0.9',
        ext_modules=[ ext1 ],
        extra_compile_args=['-O3'],
-       description='Numerical integration using several methods',
-       long_description=long_description,      # Long description read from the the readme file
+       description='Integrate arrays, functions numerically using different methods in Python. Original Fortran 2003+ legacy routines date back to 2003-2004. Read the LICENSE.txt file.',
+       long_description=long_description, # Long description read from the the readme file
        long_description_content_type="text/markdown",
        author='Jean Gomes',
        author_email='antineutrinomuon@gmail.com',
-       url='https://github.com/neutrinomuon/IntegralALL',
+       url='https://github.com/neutrinomuon/pyintegralall',
        install_requires=[ 'numpy','matplotlib' ],
        classifiers=[
            "Programming Language :: Python :: 3",
            "Programming Language :: Fortran",
            "Operating System :: OS Independent",
                    ],
        package_dir={"pyintegralall": "src/python"},
```

### Comparing `pyintegralall-0.0.8/src/fortran/DataTypes.f90` & `pyintegralall-0.0.9/src/fortran/DataTypes.f90`

 * *Files identical despite different names*

### Comparing `pyintegralall-0.0.8/src/fortran/GaussLegendreQuadrature.f90` & `pyintegralall-0.0.9/src/fortran/GaussLegendreQuadrature.f90`

 * *Files identical despite different names*

### Comparing `pyintegralall-0.0.8/src/fortran/IntegralALL.f90` & `pyintegralall-0.0.9/src/fortran/IntegralALL.f90`

 * *Files identical despite different names*

### Comparing `pyintegralall-0.0.8/src/fortran/LINinterpol.f90` & `pyintegralall-0.0.9/src/fortran/LINinterpol.f90`

 * *Files identical despite different names*

### Comparing `pyintegralall-0.0.8/src/python/PyIntegralALL.py` & `pyintegralall-0.0.9/src/python/PyIntegralALL.py`

 * *Files identical despite different names*

