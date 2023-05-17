# Comparing `tmp/lttbc-0.2.1.tar.gz` & `tmp/lttbc-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lttbc-0.2.1.tar", last modified: Sat Apr  2 14:10:15 2022, max compression
+gzip compressed data, was "lttbc-0.2.2.tar", last modified: Wed May 17 10:58:45 2023, max compression
```

## Comparing `lttbc-0.2.1.tar` & `lttbc-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-04-02 14:10:15.478677 lttbc-0.2.1/
-drwxrwxrwx   0        0        0        0 2022-04-02 14:10:15.457658 lttbc-0.2.1/.github/
-drwxrwxrwx   0        0        0        0 2022-04-02 14:10:15.469669 lttbc-0.2.1/.github/workflows/
--rw-rw-rw-   0        0        0      839 2022-04-02 13:39:36.000000 lttbc-0.2.1/.github/workflows/python-app.yml
--rw-rw-rw-   0        0        0      403 2022-04-02 13:39:36.000000 lttbc-0.2.1/.gitignore
--rw-rw-rw-   0        0        0     1112 2022-04-02 13:39:36.000000 lttbc-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2649 2022-04-02 14:10:15.478677 lttbc-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2395 2022-04-02 13:39:36.000000 lttbc-0.2.1/README.md
--rw-rw-rw-   0        0        0     1655 2022-04-02 13:39:36.000000 lttbc-0.2.1/README.txt
-drwxrwxrwx   0        0        0        0 2022-04-02 14:10:15.472671 lttbc-0.2.1/images/
--rw-rw-rw-   0        0        0    91844 2022-04-02 13:39:36.000000 lttbc-0.2.1/images/demo.png
--rw-rw-rw-   0        0        0     6467 2022-04-02 13:39:36.000000 lttbc-0.2.1/lttbc.c
-drwxrwxrwx   0        0        0        0 2022-04-02 14:10:15.477676 lttbc-0.2.1/lttbc.egg-info/
--rw-rw-rw-   0        0        0     2649 2022-04-02 14:10:15.000000 lttbc-0.2.1/lttbc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2022-04-02 14:10:15.000000 lttbc-0.2.1/lttbc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-02 14:10:15.000000 lttbc-0.2.1/lttbc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2022-04-02 14:10:15.000000 lttbc-0.2.1/lttbc.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-04-02 14:10:15.000000 lttbc-0.2.1/lttbc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       13 2022-04-02 13:39:36.000000 lttbc-0.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-04-02 14:10:15.478677 lttbc-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1844 2022-04-02 13:39:36.000000 lttbc-0.2.1/setup.py
--rw-rw-rw-   0        0        0    11302 2022-04-02 13:39:36.000000 lttbc-0.2.1/test_downsample.py
--rw-rw-rw-   0        0        0      168 2022-04-02 13:39:36.000000 lttbc-0.2.1/tox.ini
+drwxrwxr-x   0 degon     (1001) degon     (1001)        0 2023-05-17 10:58:45.809356 lttbc-0.2.2/
+drwxrwxr-x   0 degon     (1001) degon     (1001)        0 2023-05-17 10:58:45.805356 lttbc-0.2.2/.github/
+drwxrwxr-x   0 degon     (1001) degon     (1001)        0 2023-05-17 10:58:45.805356 lttbc-0.2.2/.github/workflows/
+-rw-rw-r--   0 degon     (1001) degon     (1001)      805 2023-05-17 10:48:14.000000 lttbc-0.2.2/.github/workflows/python-app.yml
+-rw-rw-r--   0 degon     (1001) degon     (1001)      368 2023-05-17 10:48:14.000000 lttbc-0.2.2/.gitignore
+-rw-rw-r--   0 degon     (1001) degon     (1001)     1091 2023-05-17 10:48:14.000000 lttbc-0.2.2/LICENSE.txt
+-rw-rw-r--   0 degon     (1001) degon     (1001)     2587 2023-05-17 10:58:45.809356 lttbc-0.2.2/PKG-INFO
+-rw-rw-r--   0 degon     (1001) degon     (1001)     2335 2023-05-17 10:48:14.000000 lttbc-0.2.2/README.md
+-rw-rw-r--   0 degon     (1001) degon     (1001)     1609 2023-05-17 10:48:14.000000 lttbc-0.2.2/README.txt
+drwxrwxr-x   0 degon     (1001) degon     (1001)        0 2023-05-17 10:58:45.805356 lttbc-0.2.2/images/
+-rw-rw-r--   0 degon     (1001) degon     (1001)    91844 2023-05-17 10:48:14.000000 lttbc-0.2.2/images/demo.png
+-rw-rw-r--   0 degon     (1001) degon     (1001)     6276 2023-05-17 10:48:14.000000 lttbc-0.2.2/lttbc.c
+drwxrwxr-x   0 degon     (1001) degon     (1001)        0 2023-05-17 10:58:45.809356 lttbc-0.2.2/lttbc.egg-info/
+-rw-rw-r--   0 degon     (1001) degon     (1001)     2587 2023-05-17 10:58:45.000000 lttbc-0.2.2/lttbc.egg-info/PKG-INFO
+-rw-rw-r--   0 degon     (1001) degon     (1001)      295 2023-05-17 10:58:45.000000 lttbc-0.2.2/lttbc.egg-info/SOURCES.txt
+-rw-rw-r--   0 degon     (1001) degon     (1001)        1 2023-05-17 10:58:45.000000 lttbc-0.2.2/lttbc.egg-info/dependency_links.txt
+-rw-rw-r--   0 degon     (1001) degon     (1001)       12 2023-05-17 10:58:45.000000 lttbc-0.2.2/lttbc.egg-info/requires.txt
+-rw-rw-r--   0 degon     (1001) degon     (1001)       13 2023-05-17 10:58:45.000000 lttbc-0.2.2/lttbc.egg-info/top_level.txt
+-rw-rw-r--   0 degon     (1001) degon     (1001)     1226 2023-05-17 10:58:18.000000 lttbc-0.2.2/pyproject.toml
+-rw-rw-r--   0 degon     (1001) degon     (1001)       38 2023-05-17 10:58:45.809356 lttbc-0.2.2/setup.cfg
+-rw-rw-r--   0 degon     (1001) degon     (1001)      615 2023-05-17 10:51:42.000000 lttbc-0.2.2/setup.py
+-rw-rw-r--   0 degon     (1001) degon     (1001)    10978 2023-05-17 10:48:14.000000 lttbc-0.2.2/test_downsample.py
+-rw-rw-r--   0 degon     (1001) degon     (1001)      138 2023-05-17 10:57:51.000000 lttbc-0.2.2/tox.ini
```

### Comparing `lttbc-0.2.1/.github/workflows/python-app.yml` & `lttbc-0.2.2/.github/workflows/python-app.yml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-name: LTTBC Package
-
-on:
-  push:
-    branches: [ master ]
-  pull_request:
-    branches: [ master ]
-
-jobs:
-  build:
-
-    runs-on: ${{ matrix.os }}
-    strategy:
-      matrix:
-        os: [ubuntu-latest]
-        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10"]
-
-    steps:
-    - uses: actions/checkout@v2
-    - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
-      with:
-        python-version: ${{ matrix.python-version }}
-    - name: Install dependencies
-      run: |
-        python -m pip install --upgrade pip
-        python -m pip install flake8 pytest
-        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
-    - name: Build package
-      run: |
-        python -m pip install . -v
-    - name: Test with pytest
-      run: |
-        pytest
+name: LTTBC Package
+
+on:
+  push:
+    branches: [ master ]
+  pull_request:
+    branches: [ master ]
+
+jobs:
+  build:
+
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        os: [ubuntu-latest]
+        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10"]
+
+    steps:
+    - uses: actions/checkout@v2
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v2
+      with:
+        python-version: ${{ matrix.python-version }}
+    - name: Install dependencies
+      run: |
+        python -m pip install --upgrade pip
+        python -m pip install flake8 pytest
+        if [ -f requirements.txt ]; then pip install -r requirements.txt; fi
+    - name: Build package
+      run: |
+        python -m pip install . -v
+    - name: Test with pytest
+      run: |
+        pytest
```

### Comparing `lttbc-0.2.1/LICENSE.txt` & `lttbc-0.2.2/LICENSE.txt`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-The MIT License (MIT)
-
-Copyright (c) European XFEL, Dennis Göries
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+The MIT License (MIT)
+
+Copyright (c) European XFEL, Dennis Göries
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `lttbc-0.2.1/PKG-INFO` & `lttbc-0.2.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,69 @@
-Metadata-Version: 2.1
-Name: lttbc
-Version: 0.2.1
-Summary: Largest triangle three buckets module for Python written in C
-Home-page: https://github.com/dgoeries/lttbc/
-Author: European XFEL GmbH
-Author-email: dennis.goeries@xfel.eu
-Maintainer: Dennis Goeries
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# lttbc: Largest-Triangle-Three-Buckets (Python using a c implementation)
-This is a low-level implementation of the `Largest-Triangle-Three-Buckets` (LTTB) downsampling algorithm written in Python.
-
-The code has been translated from the work of Sveinn Steinarsson (https://github.com/sveinn-steinarsson/flot-downsample/).
-
-Known features and requirements:
-
-- The algorithm requires monotonically increasing x data (finite)
-- The algorithm requires finite y data (otherwise problems might occur)
-- x and y data have to be of same length (of course)
-- The algorithm returns arrays of **dtype** **double**
-
-## How to use on the field
-
-The module ``lttbc`` differs in the standard input from other largest triangle three buckets implementations.
-The ``downsample`` function takes an input for ``x`` and ``y`` in addition to the ``threshold``:
-
-    import lttbc
-    import numpy as np
-
-    ARRAY_SIZE = 10000
-    THRESHOLD = 1000
-
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
-
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-
-    # List data or a mixture is accepted as well ...
-    x = list(range(ARRAY_SIZE))
-    y = [np.random.uniform(0, 1000) for _ in range(ARRAY_SIZE)]
-
-    assert isinstance(x, list)
-    assert isinstance(y, list)
-
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-
-
+Metadata-Version: 2.1
+Name: lttbc
+Version: 0.2.2
+Summary: Largest triangle three buckets module for Python written in C
+Author-email: European XFEL GmbH <dennis.goeries@xfel.eu>
+Maintainer-email: Dennis Goeries <dennis.goeries@xfel.eu>
+License: MIT
+Project-URL: git, https://github.com/dgoeries/lttbc
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# lttbc: Largest-Triangle-Three-Buckets (Python using a c implementation)
+This is a low-level implementation of the `Largest-Triangle-Three-Buckets` (LTTB) downsampling algorithm written in Python.
+
+The code has been translated from the work of Sveinn Steinarsson (https://github.com/sveinn-steinarsson/flot-downsample/).
+
+Known features and requirements:
+
+- The algorithm requires monotonically increasing x data (finite)
+- The algorithm requires finite y data (otherwise problems might occur)
+- x and y data have to be of same length (of course)
+- The algorithm returns arrays of **dtype** **double**
+
+## How to use on the field
+
+The module ``lttbc`` differs in the standard input from other largest triangle three buckets implementations.
+The ``downsample`` function takes an input for ``x`` and ``y`` in addition to the ``threshold``:
+
+    import lttbc
+    import numpy as np
+
+    ARRAY_SIZE = 10000
+    THRESHOLD = 1000
+
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
+
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+
+    # List data or a mixture is accepted as well ...
+    x = list(range(ARRAY_SIZE))
+    y = [np.random.uniform(0, 1000) for _ in range(ARRAY_SIZE)]
+
+    assert isinstance(x, list)
+    assert isinstance(y, list)
+
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
```

### Comparing `lttbc-0.2.1/README.md` & `lttbc-0.2.2/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-# lttbc: Largest-Triangle-Three-Buckets (Python using a c implementation) [![PyPi](https://img.shields.io/pypi/v/lttbc?color=blue)](https://pypi.org/project/lttbc/) [![PyPI Downloads](https://img.shields.io/pypi/dm/lttbc.svg?label=PyPI%20downloads)](https://pypi.org/project/lttbc/) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/lttbc.svg?label=Conda%20downloads)](https://anaconda.org/conda-forge/lttbc)
-This is a low-level implementation of the `Largest-Triangle-Three-Buckets` (LTTB) downsampling algorithm written in Python.
-
-The code has been translated from the work of Sveinn Steinarsson (https://github.com/sveinn-steinarsson/flot-downsample/).
-
-## Demo and 'Known Issues'
-
-The examples show the efficiency of the downsampling algorithm with a data set
-set of ``5000`` data points down sampled to ``500`` and ``250`` points.
-
-![SampleView](images/demo.png)  
-
-Known features and requirements:
-
-- The algorithm requires monotonically increasing x data (finite)
-- The algorithm requires finite y data (otherwise problems might occur)
-- x and y data have to be of same length (of course)
-- The algorithm returns arrays of **dtype** **double**
-
-## Installing
-
-You can also install it [from PyPI](https://pypi.org/project/lttbc/)
-to use in other environments with Python 3.5 or later:
-
-    pip install lttbc
-
-## How to use on the field
-
-The module ``lttbc`` differs in the standard input from other largest triangle three buckets implementations.
-The ``downsample`` function takes an input for ``x`` and ``y`` in addition to the ``threshold``:
-
-    import lttbc
-    import numpy as np
-
-    ARRAY_SIZE = 10000
-    THRESHOLD = 1000
-
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
-
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-
-    # List data or a mixture is accepted as well ...
-    x = list(range(ARRAY_SIZE))
-    y = [np.random.uniform(0, 1000) for _ in range(ARRAY_SIZE)]
-
-    assert isinstance(x, list)
-    assert isinstance(y, list)
-
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
+# lttbc: Largest-Triangle-Three-Buckets (Python using a c implementation) [![PyPi](https://img.shields.io/pypi/v/lttbc?color=blue)](https://pypi.org/project/lttbc/) [![PyPI Downloads](https://img.shields.io/pypi/dm/lttbc.svg?label=PyPI%20downloads)](https://pypi.org/project/lttbc/) [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/lttbc.svg?label=Conda%20downloads)](https://anaconda.org/conda-forge/lttbc)
+This is a low-level implementation of the `Largest-Triangle-Three-Buckets` (LTTB) downsampling algorithm written in Python.
+
+The code has been translated from the work of Sveinn Steinarsson (https://github.com/sveinn-steinarsson/flot-downsample/).
+
+## Demo and 'Known Issues'
+
+The examples show the efficiency of the downsampling algorithm with a data set
+set of ``5000`` data points down sampled to ``500`` and ``250`` points.
+
+![SampleView](images/demo.png)  
+
+Known features and requirements:
+
+- The algorithm requires monotonically increasing x data (finite)
+- The algorithm requires finite y data (otherwise problems might occur)
+- x and y data have to be of same length (of course)
+- The algorithm returns arrays of **dtype** **double**
+
+## Installing
+
+You can also install it [from PyPI](https://pypi.org/project/lttbc/)
+to use in other environments with Python 3.5 or later:
+
+    pip install lttbc
+
+## How to use on the field
+
+The module ``lttbc`` differs in the standard input from other largest triangle three buckets implementations.
+The ``downsample`` function takes an input for ``x`` and ``y`` in addition to the ``threshold``:
+
+    import lttbc
+    import numpy as np
+
+    ARRAY_SIZE = 10000
+    THRESHOLD = 1000
+
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
+
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+
+    # List data or a mixture is accepted as well ...
+    x = list(range(ARRAY_SIZE))
+    y = [np.random.uniform(0, 1000) for _ in range(ARRAY_SIZE)]
+
+    assert isinstance(x, list)
+    assert isinstance(y, list)
+
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
```

### Comparing `lttbc-0.2.1/README.txt` & `lttbc-0.2.2/README.txt`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-# lttbc: Largest-Triangle-Three-Buckets (Python using a c implementation)
-This is a low-level implementation of the `Largest-Triangle-Three-Buckets` (LTTB) downsampling algorithm written in Python.
-
-The code has been translated from the work of Sveinn Steinarsson (https://github.com/sveinn-steinarsson/flot-downsample/).
-
-Known features and requirements:
-
-- The algorithm requires monotonically increasing x data (finite)
-- The algorithm requires finite y data (otherwise problems might occur)
-- x and y data have to be of same length (of course)
-- The algorithm returns arrays of **dtype** **double**
-
-## How to use on the field
-
-The module ``lttbc`` differs in the standard input from other largest triangle three buckets implementations.
-The ``downsample`` function takes an input for ``x`` and ``y`` in addition to the ``threshold``:
-
-    import lttbc
-    import numpy as np
-
-    ARRAY_SIZE = 10000
-    THRESHOLD = 1000
-
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
-
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-
-    # List data or a mixture is accepted as well ...
-    x = list(range(ARRAY_SIZE))
-    y = [np.random.uniform(0, 1000) for _ in range(ARRAY_SIZE)]
-
-    assert isinstance(x, list)
-    assert isinstance(y, list)
-
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
+# lttbc: Largest-Triangle-Three-Buckets (Python using a c implementation)
+This is a low-level implementation of the `Largest-Triangle-Three-Buckets` (LTTB) downsampling algorithm written in Python.
+
+The code has been translated from the work of Sveinn Steinarsson (https://github.com/sveinn-steinarsson/flot-downsample/).
+
+Known features and requirements:
+
+- The algorithm requires monotonically increasing x data (finite)
+- The algorithm requires finite y data (otherwise problems might occur)
+- x and y data have to be of same length (of course)
+- The algorithm returns arrays of **dtype** **double**
+
+## How to use on the field
+
+The module ``lttbc`` differs in the standard input from other largest triangle three buckets implementations.
+The ``downsample`` function takes an input for ``x`` and ``y`` in addition to the ``threshold``:
+
+    import lttbc
+    import numpy as np
+
+    ARRAY_SIZE = 10000
+    THRESHOLD = 1000
+
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
+
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+
+    # List data or a mixture is accepted as well ...
+    x = list(range(ARRAY_SIZE))
+    y = [np.random.uniform(0, 1000) for _ in range(ARRAY_SIZE)]
+
+    assert isinstance(x, list)
+    assert isinstance(y, list)
+
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
```

### Comparing `lttbc-0.2.1/images/demo.png` & `lttbc-0.2.2/images/demo.png`

 * *Files identical despite different names*

### Comparing `lttbc-0.2.1/lttbc.c` & `lttbc-0.2.2/lttbc.c`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
-#include <Python.h>
-#include <numpy/arrayobject.h>
-#include <numpy/npy_math.h>
-#include <math.h>
-
-
-static PyObject* downsample(PyObject *self, PyObject *args) {
-    int threshold;
-    PyObject *x_obj = NULL, *y_obj = NULL;
-    PyArrayObject *x_array = NULL, *y_array = NULL;
-
-    if (!PyArg_ParseTuple(args, "OOi", &x_obj, &y_obj, &threshold))
-        return NULL;
-
-    if ((!PyArray_Check(x_obj) && !PyList_Check(x_obj)) || (!PyArray_Check(y_obj) && !PyList_Check(y_obj))) {
-        PyErr_SetString(PyExc_TypeError, "Function requires x and y input to be of type list or ndarray ...");
-        goto fail;
-    }
-
-    // Interpret the input objects as numpy arrays, with reqs (contiguous, aligned, and writeable ...)
-    x_array = (PyArrayObject *)PyArray_FROM_OTF(x_obj, NPY_DOUBLE, NPY_ARRAY_IN_ARRAY);
-    y_array = (PyArrayObject *)PyArray_FROM_OTF(y_obj, NPY_DOUBLE, NPY_ARRAY_IN_ARRAY);
-    if (x_array == NULL || y_array == NULL) {
-        goto fail;
-    }
-
-    if (PyArray_NDIM(x_array) != 1 || PyArray_NDIM(y_array) != 1) {;
-        PyErr_SetString(PyExc_ValueError, "Both x and y must have a single dimension ...");
-        goto fail;
-    }
-
-    if (!PyArray_SAMESHAPE(x_array, y_array)) {
-        PyErr_SetString(PyExc_ValueError, "Input x and y must have the same shape ...");
-        goto fail;
-    }
-
-    // Declare data length and check if we actually have to downsample!
-    const Py_ssize_t data_length = (Py_ssize_t)PyArray_DIM(x_array, 0);
-    if (threshold >= data_length || threshold <= 0) {
-        // Nothing to do!
-        PyObject *value = Py_BuildValue("OO", x_array, y_array);
-        Py_DECREF(x_array);
-        Py_DECREF(y_array);
-        return value;
-    }
-
-    // Access the data in the NDArray!
-    double *x = (double*)PyArray_DATA(x_array);
-    double *y = (double*)PyArray_DATA(y_array);
-
-    // Create an empty output array with shape and dim for the output!
-    npy_intp dims[1];
-    dims[0] = threshold;
-    PyArrayObject *sampled_x = (PyArrayObject *)PyArray_Empty(1, dims,
-        PyArray_DescrFromType(NPY_DOUBLE), 0);
-    PyArrayObject *sampled_y = (PyArrayObject *)PyArray_Empty(1, dims,
-        PyArray_DescrFromType(NPY_DOUBLE), 0);
-    // Get a pointer to its data
-    double *sampled_x_data = (double*)PyArray_DATA(sampled_x);
-    double *sampled_y_data = (double*)PyArray_DATA(sampled_y);
-
-    // The main loop here!
-    Py_ssize_t sampled_index = 0;
-    const double every = (double)(data_length - 2) / (threshold - 2);
-
-    Py_ssize_t a = 0;
-    Py_ssize_t next_a = 0;
-
-    double max_area_point_x = 0.0;
-    double max_area_point_y = 0.0;
-
-    // Always add the first point!
-    if (npy_isfinite(x[a])) {
-        sampled_x_data[sampled_index] = x[a];
-    }
-    else {
-         sampled_x_data[sampled_index] = 0.0;
-    }
-    if (npy_isfinite(y[a])) {
-        sampled_y_data[sampled_index] = y[a];
-    }
-    else {
-         sampled_y_data[sampled_index] = 0.0;
-    }
-    sampled_index++;
-    Py_ssize_t i;
-    for (i = 0; i < threshold - 2; ++i) {
-        // Calculate point average for next bucket (containing c)
-        double avg_x = 0;
-        double avg_y = 0;
-        Py_ssize_t avg_range_start = (Py_ssize_t)(floor((i + 1)* every) + 1);
-        Py_ssize_t avg_range_end = (Py_ssize_t)(floor((i + 2) * every) + 1);
-        if (avg_range_end >= data_length){
-            avg_range_end = data_length;
-        }
-        Py_ssize_t avg_range_length = avg_range_end - avg_range_start;
-
-        for (;avg_range_start < avg_range_end; avg_range_start++){
-            avg_x += x[avg_range_start];
-            avg_y += y[avg_range_start];
-        }
-        avg_x /= avg_range_length;
-        avg_y /= avg_range_length;
-
-        // Get the range for this bucket
-        Py_ssize_t range_offs = (Py_ssize_t)(floor((i + 0) * every) + 1);
-        Py_ssize_t range_to = (Py_ssize_t)(floor((i + 1) * every) + 1);
-
-        // Point a
-        double point_a_x = x[a];
-        double point_a_y = y[a];
-
-        double max_area = -1.0;
-        for (; range_offs < range_to; range_offs++){
-            // Calculate triangle area over three buckets
-            double area = fabs((point_a_x - avg_x) * (y[range_offs] - point_a_y) - (point_a_x - x[range_offs]) * (avg_y - point_a_y)) * 0.5;
-            if (area > max_area){
-                max_area = area;
-                max_area_point_x = x[range_offs];
-                max_area_point_y = y[range_offs];
-                next_a = range_offs; // Next a is this b
-            }
-        }
-        // Pick this point from the bucket
-        sampled_x_data[sampled_index] = max_area_point_x;
-        sampled_y_data[sampled_index] = max_area_point_y;
-        sampled_index++;
-
-        // Current a becomes the next_a (chosen b)
-        a = next_a;
-    }
-
-    // Always add last! Check for finite values!
-    double last_a_x = x[data_length - 1];
-    double last_a_y = y[data_length - 1];
-    if (npy_isfinite(last_a_x)) {
-        sampled_x_data[sampled_index] = last_a_x;
-    }
-    else {
-         sampled_x_data[sampled_index] = 0.0;
-    }
-    if (npy_isfinite(last_a_y)) {
-        sampled_y_data[sampled_index] = last_a_y;
-    }
-    else {
-        sampled_y_data[sampled_index] = 0.0;
-    }
-
-    // Provide our return value
-    PyObject *value = Py_BuildValue("OO", sampled_x, sampled_y);
-
-    // And remove the references!
-    Py_DECREF(x_array);
-    Py_DECREF(y_array);
-    Py_XDECREF(sampled_x);
-    Py_XDECREF(sampled_y);
-
-    return value;
-
-fail:
-    Py_XDECREF(x_array);
-    Py_XDECREF(y_array);
-    return NULL;
-}
-
-// Method definition object
-static PyMethodDef lttbc_methods[] = {
-    {
-        "downsample", // The name of the method
-        downsample, // Function pointer to the method implementation
-        METH_VARARGS,
-        "Compute the largest triangle three buckets (LTTB) algorithm in a C extension."
-    },
-    {NULL, NULL, 0, NULL}
-};
-
-static struct PyModuleDef lttbc_module_definition = {
-    PyModuleDef_HEAD_INIT,
-    "lttbc",
-    "A Python module that computes the largest triangle three buckets algorithm (LTTB) using C code.",
-    -1,
-    lttbc_methods
-};
-
-// Module initialization
-PyMODINIT_FUNC PyInit_lttbc(void) {
-    Py_Initialize();
-    import_array();
-    return PyModule_Create(&lttbc_module_definition);
-}
+#define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
+#include <Python.h>
+#include <numpy/arrayobject.h>
+#include <numpy/npy_math.h>
+#include <math.h>
+
+
+static PyObject* downsample(PyObject *self, PyObject *args) {
+    int threshold;
+    PyObject *x_obj = NULL, *y_obj = NULL;
+    PyArrayObject *x_array = NULL, *y_array = NULL;
+
+    if (!PyArg_ParseTuple(args, "OOi", &x_obj, &y_obj, &threshold))
+        return NULL;
+
+    if ((!PyArray_Check(x_obj) && !PyList_Check(x_obj)) || (!PyArray_Check(y_obj) && !PyList_Check(y_obj))) {
+        PyErr_SetString(PyExc_TypeError, "Function requires x and y input to be of type list or ndarray ...");
+        goto fail;
+    }
+
+    // Interpret the input objects as numpy arrays, with reqs (contiguous, aligned, and writeable ...)
+    x_array = (PyArrayObject *)PyArray_FROM_OTF(x_obj, NPY_DOUBLE, NPY_ARRAY_IN_ARRAY);
+    y_array = (PyArrayObject *)PyArray_FROM_OTF(y_obj, NPY_DOUBLE, NPY_ARRAY_IN_ARRAY);
+    if (x_array == NULL || y_array == NULL) {
+        goto fail;
+    }
+
+    if (PyArray_NDIM(x_array) != 1 || PyArray_NDIM(y_array) != 1) {;
+        PyErr_SetString(PyExc_ValueError, "Both x and y must have a single dimension ...");
+        goto fail;
+    }
+
+    if (!PyArray_SAMESHAPE(x_array, y_array)) {
+        PyErr_SetString(PyExc_ValueError, "Input x and y must have the same shape ...");
+        goto fail;
+    }
+
+    // Declare data length and check if we actually have to downsample!
+    const Py_ssize_t data_length = (Py_ssize_t)PyArray_DIM(x_array, 0);
+    if (threshold >= data_length || threshold <= 0) {
+        // Nothing to do!
+        PyObject *value = Py_BuildValue("OO", x_array, y_array);
+        Py_DECREF(x_array);
+        Py_DECREF(y_array);
+        return value;
+    }
+
+    // Access the data in the NDArray!
+    double *x = (double*)PyArray_DATA(x_array);
+    double *y = (double*)PyArray_DATA(y_array);
+
+    // Create an empty output array with shape and dim for the output!
+    npy_intp dims[1];
+    dims[0] = threshold;
+    PyArrayObject *sampled_x = (PyArrayObject *)PyArray_Empty(1, dims,
+        PyArray_DescrFromType(NPY_DOUBLE), 0);
+    PyArrayObject *sampled_y = (PyArrayObject *)PyArray_Empty(1, dims,
+        PyArray_DescrFromType(NPY_DOUBLE), 0);
+    // Get a pointer to its data
+    double *sampled_x_data = (double*)PyArray_DATA(sampled_x);
+    double *sampled_y_data = (double*)PyArray_DATA(sampled_y);
+
+    // The main loop here!
+    Py_ssize_t sampled_index = 0;
+    const double every = (double)(data_length - 2) / (threshold - 2);
+
+    Py_ssize_t a = 0;
+    Py_ssize_t next_a = 0;
+
+    double max_area_point_x = 0.0;
+    double max_area_point_y = 0.0;
+
+    // Always add the first point!
+    if (npy_isfinite(x[a])) {
+        sampled_x_data[sampled_index] = x[a];
+    }
+    else {
+         sampled_x_data[sampled_index] = 0.0;
+    }
+    if (npy_isfinite(y[a])) {
+        sampled_y_data[sampled_index] = y[a];
+    }
+    else {
+         sampled_y_data[sampled_index] = 0.0;
+    }
+    sampled_index++;
+    Py_ssize_t i;
+    for (i = 0; i < threshold - 2; ++i) {
+        // Calculate point average for next bucket (containing c)
+        double avg_x = 0;
+        double avg_y = 0;
+        Py_ssize_t avg_range_start = (Py_ssize_t)(floor((i + 1)* every) + 1);
+        Py_ssize_t avg_range_end = (Py_ssize_t)(floor((i + 2) * every) + 1);
+        if (avg_range_end >= data_length){
+            avg_range_end = data_length;
+        }
+        Py_ssize_t avg_range_length = avg_range_end - avg_range_start;
+
+        for (;avg_range_start < avg_range_end; avg_range_start++){
+            avg_x += x[avg_range_start];
+            avg_y += y[avg_range_start];
+        }
+        avg_x /= avg_range_length;
+        avg_y /= avg_range_length;
+
+        // Get the range for this bucket
+        Py_ssize_t range_offs = (Py_ssize_t)(floor((i + 0) * every) + 1);
+        Py_ssize_t range_to = (Py_ssize_t)(floor((i + 1) * every) + 1);
+
+        // Point a
+        double point_a_x = x[a];
+        double point_a_y = y[a];
+
+        double max_area = -1.0;
+        for (; range_offs < range_to; range_offs++){
+            // Calculate triangle area over three buckets
+            double area = fabs((point_a_x - avg_x) * (y[range_offs] - point_a_y) - (point_a_x - x[range_offs]) * (avg_y - point_a_y)) * 0.5;
+            if (area > max_area){
+                max_area = area;
+                max_area_point_x = x[range_offs];
+                max_area_point_y = y[range_offs];
+                next_a = range_offs; // Next a is this b
+            }
+        }
+        // Pick this point from the bucket
+        sampled_x_data[sampled_index] = max_area_point_x;
+        sampled_y_data[sampled_index] = max_area_point_y;
+        sampled_index++;
+
+        // Current a becomes the next_a (chosen b)
+        a = next_a;
+    }
+
+    // Always add last! Check for finite values!
+    double last_a_x = x[data_length - 1];
+    double last_a_y = y[data_length - 1];
+    if (npy_isfinite(last_a_x)) {
+        sampled_x_data[sampled_index] = last_a_x;
+    }
+    else {
+         sampled_x_data[sampled_index] = 0.0;
+    }
+    if (npy_isfinite(last_a_y)) {
+        sampled_y_data[sampled_index] = last_a_y;
+    }
+    else {
+        sampled_y_data[sampled_index] = 0.0;
+    }
+
+    // Provide our return value
+    PyObject *value = Py_BuildValue("OO", sampled_x, sampled_y);
+
+    // And remove the references!
+    Py_DECREF(x_array);
+    Py_DECREF(y_array);
+    Py_XDECREF(sampled_x);
+    Py_XDECREF(sampled_y);
+
+    return value;
+
+fail:
+    Py_XDECREF(x_array);
+    Py_XDECREF(y_array);
+    return NULL;
+}
+
+// Method definition object
+static PyMethodDef lttbc_methods[] = {
+    {
+        "downsample", // The name of the method
+        downsample, // Function pointer to the method implementation
+        METH_VARARGS,
+        "Compute the largest triangle three buckets (LTTB) algorithm in a C extension."
+    },
+    {NULL, NULL, 0, NULL}
+};
+
+static struct PyModuleDef lttbc_module_definition = {
+    PyModuleDef_HEAD_INIT,
+    "lttbc",
+    "A Python module that computes the largest triangle three buckets algorithm (LTTB) using C code.",
+    -1,
+    lttbc_methods
+};
+
+// Module initialization
+PyMODINIT_FUNC PyInit_lttbc(void) {
+    Py_Initialize();
+    import_array();
+    return PyModule_Create(&lttbc_module_definition);
+}
```

### Comparing `lttbc-0.2.1/lttbc.egg-info/PKG-INFO` & `lttbc-0.2.2/lttbc.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,73 +1,69 @@
-Metadata-Version: 2.1
-Name: lttbc
-Version: 0.2.1
-Summary: Largest triangle three buckets module for Python written in C
-Home-page: https://github.com/dgoeries/lttbc/
-Author: European XFEL GmbH
-Author-email: dennis.goeries@xfel.eu
-Maintainer: Dennis Goeries
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
-# lttbc: Largest-Triangle-Three-Buckets (Python using a c implementation)
-This is a low-level implementation of the `Largest-Triangle-Three-Buckets` (LTTB) downsampling algorithm written in Python.
-
-The code has been translated from the work of Sveinn Steinarsson (https://github.com/sveinn-steinarsson/flot-downsample/).
-
-Known features and requirements:
-
-- The algorithm requires monotonically increasing x data (finite)
-- The algorithm requires finite y data (otherwise problems might occur)
-- x and y data have to be of same length (of course)
-- The algorithm returns arrays of **dtype** **double**
-
-## How to use on the field
-
-The module ``lttbc`` differs in the standard input from other largest triangle three buckets implementations.
-The ``downsample`` function takes an input for ``x`` and ``y`` in addition to the ``threshold``:
-
-    import lttbc
-    import numpy as np
-
-    ARRAY_SIZE = 10000
-    THRESHOLD = 1000
-
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
-
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-
-    # List data or a mixture is accepted as well ...
-    x = list(range(ARRAY_SIZE))
-    y = [np.random.uniform(0, 1000) for _ in range(ARRAY_SIZE)]
-
-    assert isinstance(x, list)
-    assert isinstance(y, list)
-
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-
-
+Metadata-Version: 2.1
+Name: lttbc
+Version: 0.2.2
+Summary: Largest triangle three buckets module for Python written in C
+Author-email: European XFEL GmbH <dennis.goeries@xfel.eu>
+Maintainer-email: Dennis Goeries <dennis.goeries@xfel.eu>
+License: MIT
+Project-URL: git, https://github.com/dgoeries/lttbc
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Scientific/Engineering :: Visualization
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# lttbc: Largest-Triangle-Three-Buckets (Python using a c implementation)
+This is a low-level implementation of the `Largest-Triangle-Three-Buckets` (LTTB) downsampling algorithm written in Python.
+
+The code has been translated from the work of Sveinn Steinarsson (https://github.com/sveinn-steinarsson/flot-downsample/).
+
+Known features and requirements:
+
+- The algorithm requires monotonically increasing x data (finite)
+- The algorithm requires finite y data (otherwise problems might occur)
+- x and y data have to be of same length (of course)
+- The algorithm returns arrays of **dtype** **double**
+
+## How to use on the field
+
+The module ``lttbc`` differs in the standard input from other largest triangle three buckets implementations.
+The ``downsample`` function takes an input for ``x`` and ``y`` in addition to the ``threshold``:
+
+    import lttbc
+    import numpy as np
+
+    ARRAY_SIZE = 10000
+    THRESHOLD = 1000
+
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
+
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+
+    # List data or a mixture is accepted as well ...
+    x = list(range(ARRAY_SIZE))
+    y = [np.random.uniform(0, 1000) for _ in range(ARRAY_SIZE)]
+
+    assert isinstance(x, list)
+    assert isinstance(y, list)
+
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
```

### Comparing `lttbc-0.2.1/test_downsample.py` & `lttbc-0.2.2/test_downsample.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,324 +1,324 @@
-import sys
-from time import perf_counter
-
-import numpy as np
-import pytest
-
-import lttbc
-
-ARRAY_SIZE = 1000
-THRESHOLD = 100
-LARGE_ARRAY = 1000000
-LARGE_THRESHOLD = 10000
-
-
-def test_input_wrong_x_y():
-    """Test the down sampling with wrong input types for x or/and y"""
-    x = 1
-    y = np.array([True] * ARRAY_SIZE, dtype=bool)
-    with pytest.raises(TypeError):
-        lttbc.downsample(x, y, THRESHOLD)
-
-    x = np.array([True] * ARRAY_SIZE, dtype=bool)
-    y = 4
-    with pytest.raises(TypeError):
-        lttbc.downsample(x, y, THRESHOLD)
-
-    x = "wrong"
-    y = np.array([True] * ARRAY_SIZE, dtype=bool)
-    with pytest.raises(TypeError):
-        lttbc.downsample(x, y, THRESHOLD)
-
-    x = np.array([True] * ARRAY_SIZE, dtype=bool)
-    y = "wrong"
-    with pytest.raises(TypeError):
-        lttbc.downsample(x, y, THRESHOLD)
-
-    x = 1
-    y = "wrong"
-    with pytest.raises(TypeError):
-        lttbc.downsample(x, y, THRESHOLD)
-
-
-def test_single_dimension_validation():
-    """Test that the downsample algorithm rejects arrays with multiple dims"""
-    x = np.array([[0., 0.], [1., 0.8], [0.9, 0.8], [0.9, 0.7], [0.9, 0.6],
-                  [0.8, 0.5], [0.8, 0.5], [0.7, 0.5], [0.1, 0.], [0., 0.]],
-                 dtype=np.double)
-    assert x.shape == (10, 2)
-    assert x.ndim == 2
-
-    y = np.array([True] * ARRAY_SIZE, dtype=bool)
-    with pytest.raises(ValueError):
-        lttbc.downsample(x, y, THRESHOLD)
-
-
-def test_negative_threshold():
-    """Test if a negative threshold provides problems"""
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, -THRESHOLD)
-    assert len(nx) == ARRAY_SIZE
-    assert len(ny) == ARRAY_SIZE
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-
-    np.testing.assert_array_almost_equal(ny, y)
-
-
-def test_threshold_larger():
-    """Test if a larger threshold provides problems"""
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    # Will return the arrays!
-    nx, ny = lttbc.downsample(x, y, ARRAY_SIZE + 1)
-    assert len(nx) == ARRAY_SIZE
-    assert len(ny) == ARRAY_SIZE
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-
-    # NOTE: Known feature, we return double arrays ...
-    np.testing.assert_array_almost_equal(nx, x)
-    np.testing.assert_array_almost_equal(ny, y)
-
-
-def test_input_list():
-    """Test the down sampling with lists types"""
-    x = list(range(ARRAY_SIZE))
-    y = [True] * ARRAY_SIZE
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-    test_array = np.array([1.0] * THRESHOLD, dtype=np.float64)
-    test_array_bool = np.array([1.0] * THRESHOLD, dtype=bool)
-    np.testing.assert_array_almost_equal(ny, test_array)
-    np.testing.assert_array_almost_equal(ny, test_array_bool)
-
-
-def test_input_list_array():
-    """Test the down sampling with mixed types"""
-    x = list(range(ARRAY_SIZE))
-    y = np.array([True] * ARRAY_SIZE, dtype=bool)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-    test_array = np.array([1.0] * THRESHOLD, dtype=np.float64)
-    test_array_bool = np.array([1.0] * THRESHOLD, dtype=bool)
-    np.testing.assert_array_almost_equal(ny, test_array)
-    np.testing.assert_array_almost_equal(ny, test_array_bool)
-
-
-def test_array_size():
-    """Test the input failure for different dimensions of arrays"""
-    x = np.arange(ARRAY_SIZE)
-    y = np.random.randint(1000, size=ARRAY_SIZE - 1, dtype=np.uint64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    with pytest.raises(ValueError):
-        assert lttbc.downsample(x, y, ARRAY_SIZE)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-
-
-def test_downsample_uint64():
-    """Test the base down sampling of the module"""
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-
-
-def test_downsample_bool():
-    """Test the down sampling with boolean types"""
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.array([True] * ARRAY_SIZE, dtype=bool)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-    test_array = np.array([1.0] * THRESHOLD, dtype=np.float64)
-    test_array_bool = np.array([1.0] * THRESHOLD, dtype=bool)
-    np.testing.assert_array_almost_equal(ny, test_array)
-    np.testing.assert_array_almost_equal(ny, test_array_bool)
-
-
-def test_inf():
-    """Test the down sampling with inf types"""
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.array([np.inf] * ARRAY_SIZE, dtype=np.float64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-    test_array = np.array([0.0] * THRESHOLD, dtype=np.float64)
-    np.testing.assert_array_almost_equal(ny, test_array)
-
-
-def test_nan():
-    """Test the down sampling with NaN types"""
-    x = np.arange(ARRAY_SIZE, dtype=np.int32)
-    y = np.array([np.nan] * ARRAY_SIZE, dtype=np.float64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, THRESHOLD)
-    assert len(nx) == THRESHOLD
-    assert len(ny) == THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-    test_array = np.array([0.0] * THRESHOLD, dtype=np.float64)
-    np.testing.assert_array_almost_equal(ny, test_array)
-
-
-def test_benchmark():
-    """Basic skeletton benchmark test for the down sample algorithm"""
-    x = np.arange(LARGE_ARRAY, dtype=np.int32)
-    y = np.arange(LARGE_ARRAY, dtype=np.float64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-
-    def sample():
-        nx, ny = lttbc.downsample(x, y, LARGE_THRESHOLD)
-        return nx, ny
-
-    t_start = perf_counter()
-    nx, ny = sample()
-    elapsed = perf_counter() - t_start
-
-    assert len(nx) == LARGE_THRESHOLD
-    assert len(ny) == LARGE_THRESHOLD
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-
-    assert elapsed < 0.1
-
-
-def test_array_mix_inf_nan():
-    """Test mix of problematic input 'inf' and 'nan'"""
-
-    x = np.arange(20, dtype=np.int32)
-    y = np.array([0.0, 1.0, 2.0, np.nan, 4.0, 5.0, 6.0, np.nan, np.inf,
-                  np.inf, 10.0, np.nan, 12.0, -np.inf, 14.0, 15.0, 16.0, 17.0,
-                  np.nan, 19.0], dtype=np.float64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, 10)
-    assert len(nx) == 10
-    assert len(ny) == 10
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-    test_array = np.array(
-        [0., 0., 4., 4., 4., 10., -np.inf, -np.inf, -np.inf, 19.],
-        dtype=np.float64)
-    np.testing.assert_array_almost_equal(ny, test_array)
-
-
-def test_single_nan():
-    """Test single 'nan' input for down sampling"""
-    x = np.arange(20, dtype=np.int32)
-    y = np.array([0.0, 1.0, 2.0, np.nan, 4.0, 5.0, 6.0, 7.0, 8.0,
-                  9.0, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, 16.0, 17.0,
-                  18.0, 19.0], dtype=np.float64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, 10)
-    assert len(nx) == 10
-    assert len(ny) == 10
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-    test_array = np.array(
-        [0., 0., 4., 5., 7., 10., 12., 14., 16., 19.],
-        dtype=np.float64)
-    np.testing.assert_array_almost_equal(ny, test_array)
-
-
-def test_single_inf():
-    """Test single 'inf' input for down sampling
-
-    XXX: Apparently infinite values provide a crappy result...
-    """
-    x = np.arange(20, dtype=np.int32)
-    y = np.array([0.0, 1.0, 2.0, np.inf, 4.0, 5.0, 6.0, 7.0, 8.0,
-                  9.0, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, 16.0, 17.0,
-                  18.0, 19.0], dtype=np.float64)
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    nx, ny = lttbc.downsample(x, y, 10)
-    assert len(nx) == 10
-    assert len(ny) == 10
-    assert nx.dtype == np.double
-    assert ny.dtype == np.double
-    assert sys.getrefcount(x) == 2
-    assert sys.getrefcount(y) == 2
-    assert sys.getrefcount(nx) == 2
-    assert sys.getrefcount(ny) == 2
-    test_array = np.array(
-        [0., 1., np.inf, np.inf, np.inf, np.inf, np.inf, np.inf, np.inf, 19.],
-        dtype=np.float64)
-    np.testing.assert_array_almost_equal(ny, test_array)
+import sys
+from time import perf_counter
+
+import numpy as np
+import pytest
+
+import lttbc
+
+ARRAY_SIZE = 1000
+THRESHOLD = 100
+LARGE_ARRAY = 1000000
+LARGE_THRESHOLD = 10000
+
+
+def test_input_wrong_x_y():
+    """Test the down sampling with wrong input types for x or/and y"""
+    x = 1
+    y = np.array([True] * ARRAY_SIZE, dtype=bool)
+    with pytest.raises(TypeError):
+        lttbc.downsample(x, y, THRESHOLD)
+
+    x = np.array([True] * ARRAY_SIZE, dtype=bool)
+    y = 4
+    with pytest.raises(TypeError):
+        lttbc.downsample(x, y, THRESHOLD)
+
+    x = "wrong"
+    y = np.array([True] * ARRAY_SIZE, dtype=bool)
+    with pytest.raises(TypeError):
+        lttbc.downsample(x, y, THRESHOLD)
+
+    x = np.array([True] * ARRAY_SIZE, dtype=bool)
+    y = "wrong"
+    with pytest.raises(TypeError):
+        lttbc.downsample(x, y, THRESHOLD)
+
+    x = 1
+    y = "wrong"
+    with pytest.raises(TypeError):
+        lttbc.downsample(x, y, THRESHOLD)
+
+
+def test_single_dimension_validation():
+    """Test that the downsample algorithm rejects arrays with multiple dims"""
+    x = np.array([[0., 0.], [1., 0.8], [0.9, 0.8], [0.9, 0.7], [0.9, 0.6],
+                  [0.8, 0.5], [0.8, 0.5], [0.7, 0.5], [0.1, 0.], [0., 0.]],
+                 dtype=np.double)
+    assert x.shape == (10, 2)
+    assert x.ndim == 2
+
+    y = np.array([True] * ARRAY_SIZE, dtype=bool)
+    with pytest.raises(ValueError):
+        lttbc.downsample(x, y, THRESHOLD)
+
+
+def test_negative_threshold():
+    """Test if a negative threshold provides problems"""
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, -THRESHOLD)
+    assert len(nx) == ARRAY_SIZE
+    assert len(ny) == ARRAY_SIZE
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+
+    np.testing.assert_array_almost_equal(ny, y)
+
+
+def test_threshold_larger():
+    """Test if a larger threshold provides problems"""
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    # Will return the arrays!
+    nx, ny = lttbc.downsample(x, y, ARRAY_SIZE + 1)
+    assert len(nx) == ARRAY_SIZE
+    assert len(ny) == ARRAY_SIZE
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+
+    # NOTE: Known feature, we return double arrays ...
+    np.testing.assert_array_almost_equal(nx, x)
+    np.testing.assert_array_almost_equal(ny, y)
+
+
+def test_input_list():
+    """Test the down sampling with lists types"""
+    x = list(range(ARRAY_SIZE))
+    y = [True] * ARRAY_SIZE
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+    test_array = np.array([1.0] * THRESHOLD, dtype=np.float64)
+    test_array_bool = np.array([1.0] * THRESHOLD, dtype=bool)
+    np.testing.assert_array_almost_equal(ny, test_array)
+    np.testing.assert_array_almost_equal(ny, test_array_bool)
+
+
+def test_input_list_array():
+    """Test the down sampling with mixed types"""
+    x = list(range(ARRAY_SIZE))
+    y = np.array([True] * ARRAY_SIZE, dtype=bool)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+    test_array = np.array([1.0] * THRESHOLD, dtype=np.float64)
+    test_array_bool = np.array([1.0] * THRESHOLD, dtype=bool)
+    np.testing.assert_array_almost_equal(ny, test_array)
+    np.testing.assert_array_almost_equal(ny, test_array_bool)
+
+
+def test_array_size():
+    """Test the input failure for different dimensions of arrays"""
+    x = np.arange(ARRAY_SIZE)
+    y = np.random.randint(1000, size=ARRAY_SIZE - 1, dtype=np.uint64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    with pytest.raises(ValueError):
+        assert lttbc.downsample(x, y, ARRAY_SIZE)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+
+
+def test_downsample_uint64():
+    """Test the base down sampling of the module"""
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.random.randint(1000, size=ARRAY_SIZE, dtype=np.uint64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+
+
+def test_downsample_bool():
+    """Test the down sampling with boolean types"""
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.array([True] * ARRAY_SIZE, dtype=bool)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+    test_array = np.array([1.0] * THRESHOLD, dtype=np.float64)
+    test_array_bool = np.array([1.0] * THRESHOLD, dtype=bool)
+    np.testing.assert_array_almost_equal(ny, test_array)
+    np.testing.assert_array_almost_equal(ny, test_array_bool)
+
+
+def test_inf():
+    """Test the down sampling with inf types"""
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.array([np.inf] * ARRAY_SIZE, dtype=np.float64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+    test_array = np.array([0.0] * THRESHOLD, dtype=np.float64)
+    np.testing.assert_array_almost_equal(ny, test_array)
+
+
+def test_nan():
+    """Test the down sampling with NaN types"""
+    x = np.arange(ARRAY_SIZE, dtype=np.int32)
+    y = np.array([np.nan] * ARRAY_SIZE, dtype=np.float64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, THRESHOLD)
+    assert len(nx) == THRESHOLD
+    assert len(ny) == THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+    test_array = np.array([0.0] * THRESHOLD, dtype=np.float64)
+    np.testing.assert_array_almost_equal(ny, test_array)
+
+
+def test_benchmark():
+    """Basic skeletton benchmark test for the down sample algorithm"""
+    x = np.arange(LARGE_ARRAY, dtype=np.int32)
+    y = np.arange(LARGE_ARRAY, dtype=np.float64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+
+    def sample():
+        nx, ny = lttbc.downsample(x, y, LARGE_THRESHOLD)
+        return nx, ny
+
+    t_start = perf_counter()
+    nx, ny = sample()
+    elapsed = perf_counter() - t_start
+
+    assert len(nx) == LARGE_THRESHOLD
+    assert len(ny) == LARGE_THRESHOLD
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+
+    assert elapsed < 0.1
+
+
+def test_array_mix_inf_nan():
+    """Test mix of problematic input 'inf' and 'nan'"""
+
+    x = np.arange(20, dtype=np.int32)
+    y = np.array([0.0, 1.0, 2.0, np.nan, 4.0, 5.0, 6.0, np.nan, np.inf,
+                  np.inf, 10.0, np.nan, 12.0, -np.inf, 14.0, 15.0, 16.0, 17.0,
+                  np.nan, 19.0], dtype=np.float64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, 10)
+    assert len(nx) == 10
+    assert len(ny) == 10
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+    test_array = np.array(
+        [0., 0., 4., 4., 4., 10., -np.inf, -np.inf, -np.inf, 19.],
+        dtype=np.float64)
+    np.testing.assert_array_almost_equal(ny, test_array)
+
+
+def test_single_nan():
+    """Test single 'nan' input for down sampling"""
+    x = np.arange(20, dtype=np.int32)
+    y = np.array([0.0, 1.0, 2.0, np.nan, 4.0, 5.0, 6.0, 7.0, 8.0,
+                  9.0, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, 16.0, 17.0,
+                  18.0, 19.0], dtype=np.float64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, 10)
+    assert len(nx) == 10
+    assert len(ny) == 10
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+    test_array = np.array(
+        [0., 0., 4., 5., 7., 10., 12., 14., 16., 19.],
+        dtype=np.float64)
+    np.testing.assert_array_almost_equal(ny, test_array)
+
+
+def test_single_inf():
+    """Test single 'inf' input for down sampling
+
+    XXX: Apparently infinite values provide a crappy result...
+    """
+    x = np.arange(20, dtype=np.int32)
+    y = np.array([0.0, 1.0, 2.0, np.inf, 4.0, 5.0, 6.0, 7.0, 8.0,
+                  9.0, 10.0, 11.0, 12.0, 13.0, 14.0, 15.0, 16.0, 17.0,
+                  18.0, 19.0], dtype=np.float64)
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    nx, ny = lttbc.downsample(x, y, 10)
+    assert len(nx) == 10
+    assert len(ny) == 10
+    assert nx.dtype == np.double
+    assert ny.dtype == np.double
+    assert sys.getrefcount(x) == 2
+    assert sys.getrefcount(y) == 2
+    assert sys.getrefcount(nx) == 2
+    assert sys.getrefcount(ny) == 2
+    test_array = np.array(
+        [0., 1., np.inf, np.inf, np.inf, np.inf, np.inf, np.inf, np.inf, 19.],
+        dtype=np.float64)
+    np.testing.assert_array_almost_equal(ny, test_array)
```

