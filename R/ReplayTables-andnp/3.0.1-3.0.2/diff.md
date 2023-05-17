# Comparing `tmp/ReplayTables-andnp-3.0.1.tar.gz` & `tmp/ReplayTables-andnp-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReplayTables-andnp-3.0.1.tar", last modified: Wed May 17 17:09:10 2023, max compression
+gzip compressed data, was "ReplayTables-andnp-3.0.2.tar", last modified: Wed May 17 17:59:15 2023, max compression
```

## Comparing `ReplayTables-andnp-3.0.1.tar` & `ReplayTables-andnp-3.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0        0 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/README.md
--rw-r--r--   0        0        0     5167 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/Distributions.py
--rw-r--r--   0        0        0     2140 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/LagBuffer.py
--rw-r--r--   0        0        0     2392 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/PER.py
--rw-r--r--   0        0        0     2735 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/PrioritizedHeap.py
--rw-r--r--   0        0        0     3696 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/ReplayBuffer.py
--rw-r--r--   0        0        0     8237 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/Table.py
--rw-r--r--   0        0        0        0 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/__init__.py
--rw-r--r--   0        0        0     3418 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/_utils/MemoryWriter.py
--rw-r--r--   0        0        0     5811 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/_utils/MinMaxHeap.py
--rw-r--r--   0        0        0     1772 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/_utils/RandDict.py
--rw-r--r--   0        0        0     3822 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/_utils/SumTree.py
--rw-r--r--   0        0        0        0 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/_utils/__init__.py
--rw-r--r--   0        0        0     1356 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/_utils/jit.py
--rw-r--r--   0        0        0       58 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/ReplayTables/_utils/logger.py
--rw-r--r--   0        0        0      886 2023-05-17 17:09:07.537176 ReplayTables-andnp-3.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3076 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/tests/test_LagBuffer.py
--rw-r--r--   0        0        0     2449 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/tests/test_PER.py
--rw-r--r--   0        0        0     1385 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/tests/test_PrioritizedHeap.py
--rw-r--r--   0        0        0     2679 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/tests/test_ReplayBuffer.py
--rw-r--r--   0        0        0     1537 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/tests/test_Table.py
--rw-r--r--   0        0        0     5619 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/tests/test_View.py
--rw-r--r--   0        0        0        0 2023-05-17 17:08:26.316683 ReplayTables-andnp-3.0.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     1217 2023-05-17 17:08:26.320683 ReplayTables-andnp-3.0.1/tests/utils/test_MinMaxHeap.py
--rw-r--r--   0        0        0     2998 2023-05-17 17:08:26.320683 ReplayTables-andnp-3.0.1/tests/utils/test_SumTree.py
--rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-17 17:58:41.825039 ReplayTables-andnp-3.0.2/README.md
+-rw-r--r--   0        0        0     5167 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/Distributions.py
+-rw-r--r--   0        0        0     2140 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/LagBuffer.py
+-rw-r--r--   0        0        0     2392 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/PER.py
+-rw-r--r--   0        0        0     2976 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/PrioritizedHeap.py
+-rw-r--r--   0        0        0     3696 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/ReplayBuffer.py
+-rw-r--r--   0        0        0     8237 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/Table.py
+-rw-r--r--   0        0        0        0 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/__init__.py
+-rw-r--r--   0        0        0     3418 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/_utils/MemoryWriter.py
+-rw-r--r--   0        0        0     5811 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/_utils/MinMaxHeap.py
+-rw-r--r--   0        0        0     1772 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/_utils/RandDict.py
+-rw-r--r--   0        0        0     3822 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/_utils/SumTree.py
+-rw-r--r--   0        0        0        0 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/_utils/__init__.py
+-rw-r--r--   0        0        0     1356 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/_utils/jit.py
+-rw-r--r--   0        0        0       58 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/ReplayTables/_utils/logger.py
+-rw-r--r--   0        0        0      886 2023-05-17 17:59:12.777516 ReplayTables-andnp-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3076 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/test_LagBuffer.py
+-rw-r--r--   0        0        0     2449 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/test_PER.py
+-rw-r--r--   0        0        0     1384 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/test_PrioritizedHeap.py
+-rw-r--r--   0        0        0     2679 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/test_ReplayBuffer.py
+-rw-r--r--   0        0        0     1537 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/test_Table.py
+-rw-r--r--   0        0        0     5619 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/test_View.py
+-rw-r--r--   0        0        0        0 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1217 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/utils/test_MinMaxHeap.py
+-rw-r--r--   0        0        0     2998 2023-05-17 17:58:41.829038 ReplayTables-andnp-3.0.2/tests/utils/test_SumTree.py
+-rw-r--r--   0        0        0      284 1970-01-01 00:00:00.000000 ReplayTables-andnp-3.0.2/PKG-INFO
```

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/Distributions.py` & `ReplayTables-andnp-3.0.2/ReplayTables/Distributions.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/LagBuffer.py` & `ReplayTables-andnp-3.0.2/ReplayTables/LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/PER.py` & `ReplayTables-andnp-3.0.2/ReplayTables/PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/PrioritizedHeap.py` & `ReplayTables-andnp-3.0.2/ReplayTables/PrioritizedHeap.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,16 +17,23 @@
         self._c = config or PrioritizedHeapConfig()
         self._heap = MinMaxHeap[EID]()
 
     def size(self):
         return self._heap.size()
 
     def _add(self, transition: T):
-        eid = cast(EID, self._t)
-        self._t += 1
+        if hasattr(transition, '_eid'):
+            eid = getattr(transition, '_eid')
+            eid = cast(EID, eid)
+        else:
+            eid = cast(EID, self._t)
+            self._t += 1
+            try:
+                setattr(transition, '_eid', eid)
+            except Exception: ...
 
         self._storage[eid] = transition
         return eid
 
     def add(self, transition: T, /, **kwargs: Any):
         priority = kwargs['priority']
         if priority < self._c.threshold:
```

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/ReplayBuffer.py` & `ReplayTables-andnp-3.0.2/ReplayTables/ReplayBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/Table.py` & `ReplayTables-andnp-3.0.2/ReplayTables/Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/_utils/MemoryWriter.py` & `ReplayTables-andnp-3.0.2/ReplayTables/_utils/MemoryWriter.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/_utils/MinMaxHeap.py` & `ReplayTables-andnp-3.0.2/ReplayTables/_utils/MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/_utils/RandDict.py` & `ReplayTables-andnp-3.0.2/ReplayTables/_utils/RandDict.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/_utils/SumTree.py` & `ReplayTables-andnp-3.0.2/ReplayTables/_utils/SumTree.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/ReplayTables/_utils/jit.py` & `ReplayTables-andnp-3.0.2/ReplayTables/_utils/jit.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/pyproject.toml` & `ReplayTables-andnp-3.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "3.0.1"
+version = "3.0.2"
 tag_format = "$version"
 version_files = [
     "pyproject.toml",
 ]
 
 [tool.pdm]
 source = [
@@ -22,15 +22,15 @@
 ]
 
 [tool.mypy]
 mypy_path = "typings"
 
 [project]
 name = "ReplayTables-andnp"
-version = "3.0.1"
+version = "3.0.2"
 description = "A simple replay buffer implementation in python for sampling n-step trajectories"
 authors = [
     { name = "Andy Patterson", email = "andnpatterson@gmail.com" },
 ]
 dependencies = [
     "numba>=0.57",
     "numpy>=1.23.5",
```

### Comparing `ReplayTables-andnp-3.0.1/tests/test_LagBuffer.py` & `ReplayTables-andnp-3.0.2/tests/test_LagBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/tests/test_PER.py` & `ReplayTables-andnp-3.0.2/tests/test_PER.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/tests/test_PrioritizedHeap.py` & `ReplayTables-andnp-3.0.2/tests/test_PrioritizedHeap.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from ReplayTables.PrioritizedHeap import PrioritizedHeap
 
 class Data(NamedTuple):
     a: float | np.ndarray
     b: int | np.ndarray
 
-
 class TestPrioritizedHeap(unittest.TestCase):
     def test_simple_buffer(self):
         rng = np.random.default_rng(0)
 
         buffer = PrioritizedHeap(
             max_size=10,
             structure=Data,
```

### Comparing `ReplayTables-andnp-3.0.1/tests/test_ReplayBuffer.py` & `ReplayTables-andnp-3.0.2/tests/test_ReplayBuffer.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/tests/test_Table.py` & `ReplayTables-andnp-3.0.2/tests/test_Table.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/tests/test_View.py` & `ReplayTables-andnp-3.0.2/tests/test_View.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/tests/utils/test_MinMaxHeap.py` & `ReplayTables-andnp-3.0.2/tests/utils/test_MinMaxHeap.py`

 * *Files identical despite different names*

### Comparing `ReplayTables-andnp-3.0.1/tests/utils/test_SumTree.py` & `ReplayTables-andnp-3.0.2/tests/utils/test_SumTree.py`

 * *Files identical despite different names*

