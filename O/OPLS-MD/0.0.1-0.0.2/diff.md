# Comparing `tmp/OPLS-MD-0.0.1.tar.gz` & `tmp/OPLS-MD-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OPLS-MD-0.0.1.tar", last modified: Wed Feb  8 12:19:34 2023, max compression
+gzip compressed data, was "OPLS-MD-0.0.2.tar", last modified: Wed May 17 11:44:56 2023, max compression
```

## Comparing `OPLS-MD-0.0.1.tar` & `OPLS-MD-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwx------   0 paajasan (1252311) hyad-all (3000000)        0 2023-02-08 12:19:34.624843 OPLS-MD-0.0.1/
-drwx------   0 paajasan (1252311) hyad-all (3000000)        0 2023-02-08 12:19:34.624843 OPLS-MD-0.0.1/OPLS_MD.egg-info/
--rw-------   0 paajasan (1252311) hyad-all (3000000)     2669 2023-02-08 12:19:34.000000 OPLS-MD-0.0.1/OPLS_MD.egg-info/PKG-INFO
--rw-------   0 paajasan (1252311) hyad-all (3000000)      218 2023-02-08 12:19:34.000000 OPLS-MD-0.0.1/OPLS_MD.egg-info/SOURCES.txt
--rw-------   0 paajasan (1252311) hyad-all (3000000)        1 2023-02-08 12:19:34.000000 OPLS-MD-0.0.1/OPLS_MD.egg-info/dependency_links.txt
--rw-------   0 paajasan (1252311) hyad-all (3000000)        8 2023-02-08 12:19:34.000000 OPLS-MD-0.0.1/OPLS_MD.egg-info/top_level.txt
--rw-------   0 paajasan (1252311) hyad-all (3000000)     2669 2023-02-08 12:19:34.624843 OPLS-MD-0.0.1/PKG-INFO
--rw-------   0 paajasan (1252311) hyad-all (3000000)     2274 2022-10-31 14:22:33.000000 OPLS-MD-0.0.1/README.md
--rw-------   0 paajasan (1252311) hyad-all (3000000)       88 2022-10-17 12:24:15.000000 OPLS-MD-0.0.1/pyproject.toml
--rw-------   0 paajasan (1252311) hyad-all (3000000)      534 2023-02-08 12:19:34.624843 OPLS-MD-0.0.1/setup.cfg
-drwx------   0 paajasan (1252311) hyad-all (3000000)        0 2023-02-08 12:19:34.624843 OPLS-MD-0.0.1/src/
--rw-------   0 paajasan (1252311) hyad-all (3000000)    42518 2023-02-08 12:02:25.000000 OPLS-MD-0.0.1/src/OPLS.py
--rw-------   0 paajasan (1252311) hyad-all (3000000)    11813 2023-02-08 12:02:25.000000 OPLS-MD-0.0.1/src/OPLS_MD.py
--rw-------   0 paajasan (1252311) hyad-all (3000000)       88 2023-02-08 12:02:25.000000 OPLS-MD-0.0.1/src/__init__.py
-drwx------   0 paajasan (1252311) hyad-all (3000000)        0 2023-02-08 12:19:34.624843 OPLS-MD-0.0.1/tests/
--rwx------   0 paajasan (1252311) hyad-all (3000000)     4842 2023-02-08 12:02:25.000000 OPLS-MD-0.0.1/tests/testing.py
+drwx------   0 paajasan (1252311) hyad-all (3000000)        0 2023-05-17 11:44:56.243329 OPLS-MD-0.0.2/
+-rw-------   0 paajasan (1252311) hyad-all (3000000)     1089 2023-02-08 12:37:16.000000 OPLS-MD-0.0.2/LICENSE
+drwx------   0 paajasan (1252311) hyad-all (3000000)        0 2023-05-17 11:44:56.243329 OPLS-MD-0.0.2/OPLS_MD.egg-info/
+-rw-------   0 paajasan (1252311) hyad-all (3000000)     5393 2023-05-17 11:44:56.000000 OPLS-MD-0.0.2/OPLS_MD.egg-info/PKG-INFO
+-rw-------   0 paajasan (1252311) hyad-all (3000000)      266 2023-05-17 11:44:56.000000 OPLS-MD-0.0.2/OPLS_MD.egg-info/SOURCES.txt
+-rw-------   0 paajasan (1252311) hyad-all (3000000)        1 2023-05-17 11:44:56.000000 OPLS-MD-0.0.2/OPLS_MD.egg-info/dependency_links.txt
+-rw-------   0 paajasan (1252311) hyad-all (3000000)        8 2023-05-17 11:44:56.000000 OPLS-MD-0.0.2/OPLS_MD.egg-info/top_level.txt
+-rw-------   0 paajasan (1252311) hyad-all (3000000)     5393 2023-05-17 11:44:56.243329 OPLS-MD-0.0.2/PKG-INFO
+-rw-------   0 paajasan (1252311) hyad-all (3000000)     4840 2023-02-08 13:26:52.000000 OPLS-MD-0.0.2/README.md
+-rw-------   0 paajasan (1252311) hyad-all (3000000)       88 2022-10-17 12:24:15.000000 OPLS-MD-0.0.2/pyproject.toml
+-rw-------   0 paajasan (1252311) hyad-all (3000000)      690 2023-05-17 11:44:56.247329 OPLS-MD-0.0.2/setup.cfg
+drwx------   0 paajasan (1252311) hyad-all (3000000)        0 2023-05-17 11:44:56.243329 OPLS-MD-0.0.2/src/
+-rw-------   0 paajasan (1252311) hyad-all (3000000)    21255 2023-05-17 11:43:11.000000 OPLS-MD-0.0.2/src/OPLS.py
+-rw-------   0 paajasan (1252311) hyad-all (3000000)    11938 2023-02-08 12:24:25.000000 OPLS-MD-0.0.2/src/OPLS_MD.py
+-rw-------   0 paajasan (1252311) hyad-all (3000000)     9267 2023-02-08 13:36:34.000000 OPLS-MD-0.0.2/src/OPLS_PLS.py
+-rw-------   0 paajasan (1252311) hyad-all (3000000)    11782 2023-02-08 12:24:25.000000 OPLS-MD-0.0.2/src/PLS.py
+-rw-------   0 paajasan (1252311) hyad-all (3000000)      148 2023-05-17 11:43:01.000000 OPLS-MD-0.0.2/src/__init__.py
+-rw-------   0 paajasan (1252311) hyad-all (3000000)     3581 2023-02-08 12:24:25.000000 OPLS-MD-0.0.2/src/utils.py
+drwx------   0 paajasan (1252311) hyad-all (3000000)        0 2023-05-17 11:44:56.243329 OPLS-MD-0.0.2/tests/
+-rwx------   0 paajasan (1252311) hyad-all (3000000)     5117 2023-02-08 12:24:25.000000 OPLS-MD-0.0.2/tests/testing.py
```

### Comparing `OPLS-MD-0.0.1/src/OPLS_MD.py` & `OPLS-MD-0.0.2/src/OPLS_MD.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 try:
     from MDAnalysis import Universe, AtomGroup
 except ImportError as e:
     Universe = None
     AtomGroup = None
 
-from .OPLS import PLS, OPLS, OPLS_PLS
+from .OPLS import OPLS
+from .PLS import PLS
+from .OPLS_PLS import OPLS_PLS
 
 from typing import Union, Tuple
 
 
 class _MD_PLS_WRAPPER():
     """
     A wrapper class to wrap PLS object to accept MDAnalysis universes and atomg groups,
@@ -84,22 +86,24 @@
             return self._from_crd(super().inverse_transform(X))
         else:
             X_new, Y_new = super().inverse_transform(X, Y)
             return self._from_crd(X_new), Y_new
 
     def inverse_predict(self,
                         Y: np.ndarray,
+                        ndim: int = None,
                         copy=True):
-        return self._to_crd(super().inverse_predict(Y, copy))
+        return self._to_crd(super().inverse_predict(Y, ndim, copy))
 
     def predict(self,
                 crd: Union[np.ndarray, Universe, AtomGroup],
+                ndim: int = None,
                 copy=True):
         X = self._from_crd(crd)
-        return super().predict(X, copy)
+        return super().predict(X, ndim, copy)
 
 
 class _MD_OPLS_WRAPPER(_MD_PLS_WRAPPER):
     """
     A wrapper class to wrap OPLS object to accept MDAnalysis universes and atomg groups,
     as well as unflattened MD trajectories. Should NOT be instanciated as such, but through the OPLS_MD class.
     The final class needs to first inherit this class, and only then the class which is wrapped.
```

### Comparing `OPLS-MD-0.0.1/tests/testing.py` & `OPLS-MD-0.0.2/tests/testing.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     pls_md = PLS_MD(n_components=5).fit(u, y_train)
     pls = PLS(n_components=5).fit(X_train, y_train)
     u.load_new(X_test.reshape((X_test.shape[0], u.atoms.n_atoms, 3)))
     assert np.all(np.abs(pls_md.transform(u)-pls.transform(X_test)) < 1e-6)
     assert np.abs(pls_md.score(u, y_test)-pls.score(X_test, y_test)) < 1e-10
 
 
-if (False):
+if (True):
     fig1, axes1 = plt.subplots(1, 2)
     fig2, axes2 = plt.subplots(1, 2)
 
     for center, scale in ((True, True), (True, False), (False, False)):
         print(f"center={center}, scale={scale}")
         ncomp = []
         opls = []
@@ -81,31 +81,41 @@
     pls_score = []
     for k in ncomp:
         print(k, end="\r")
         pls = PLS(n_components=k).fit(X_train, y_train)
         pls_score.append(pls.score(X_test, y_test))
 
     print("pls ", ["%.4f" % v for v in pls_score])
+    
+    ncomp = np.arange(maxk)+1
+    pls_score = []
+    pls = PLS(n_components=maxk).fit(X_train, y_train)
+    for k in ncomp:
+        print(k, end="\r")
+        pls_score.append(pls.score(X_test, y_test, ndim=k))
+
+    print("pls ", ["%.4f" % v for v in pls_score])
+
     opls_score = []
     for k in ncomp:
         print(k, end="\r")
         pls = OPLS(n_components=k).fit(X_train, y_train)
         opls_score.append(pls.score(X_test, y_test))
 
     print("opls", ["%.4f" % v for v in opls_score])
 
     opls_pls_score = {}
     ncomp_opls = np.arange(1, 7)
     for i in ncomp_opls:
         opls_pls_score[i] = []
+        opls = OPLS(n_components=i).fit(X_train, y_train)
+        pls = PLS(n_components=maxk).fit(opls.correct(X_train), y_train)
         for k in ncomp:
             print(i, k, end="\r")
-            opls = OPLS(n_components=i).fit(X_train, y_train)
-            pls = PLS(n_components=k).fit(opls.correct(X_train), y_train)
-            opls_pls_score[i].append(pls.score(opls.correct(X_test), y_test))
+            opls_pls_score[i].append(pls.score(opls.correct(X_test), y_test, ndim=k))
 
         print("%2d  " % i, ["%.4f" % v for v in opls_pls_score[i]])
 
     fig, ax = plt.subplots(1)
     ax.plot(ncomp, pls_score, label="PLS")
     ax.plot(ncomp, opls_score, label="OPLS")
     for i in opls_pls_score:
@@ -118,15 +128,15 @@
 
     fig, ax = plt.subplots(1)
     ax.plot(ncomp, pls_score, label="PLS")
     ax.plot(ncomp, opls_score, label="OPLS")
     for i in opls_pls_score:
         ax.plot(ncomp+i, opls_pls_score[i], "--", label=f"OPLS({i})-PLS")
 
-    ax.xlim(ncomp.min()-1, ncomp.max()+1)
+    ax.set_xlim(ncomp.min()-1, ncomp.max()+1)
     ax.legend()
     fig.set_size_inches(12, 8)
     fig.tight_layout()
     fig.savefig(pathlib.Path(__file__).parent / "scores2.png")
 
 jaas = 10
 print(0, jaas,
```

