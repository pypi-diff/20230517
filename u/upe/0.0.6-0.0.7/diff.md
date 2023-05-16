# Comparing `tmp/upe-0.0.6.tar.gz` & `tmp/upe-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upe-0.0.6.tar", last modified: Tue May 16 22:05:08 2023, max compression
+gzip compressed data, was "upe-0.0.7.tar", last modified: Tue May 16 22:16:19 2023, max compression
```

## Comparing `upe-0.0.6.tar` & `upe-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 22:05:08.800576 upe-0.0.6/
--rw-rw-rw-   0        0        0      191 2023-05-16 22:05:08.800576 upe-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-16 22:05:08.774044 upe-0.0.6/libname/
--rw-rw-rw-   0        0        0       53 2023-05-16 22:02:41.000000 upe-0.0.6/libname/__init__.py
--rw-rw-rw-   0        0        0    55871 2023-05-16 22:01:49.000000 upe-0.0.6/libname/cdlab.py
--rw-rw-rw-   0        0        0    30036 2023-05-16 20:15:16.000000 upe-0.0.6/libname/nqueen.py
--rw-rw-rw-   0        0        0       42 2023-05-16 22:05:08.801578 upe-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      428 2023-05-16 22:04:01.000000 upe-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 22:05:08.799575 upe-0.0.6/upe.egg-info/
--rw-rw-rw-   0        0        0      191 2023-05-16 22:05:08.000000 upe-0.0.6/upe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      171 2023-05-16 22:05:08.000000 upe-0.0.6/upe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 22:05:08.000000 upe-0.0.6/upe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 22:05:08.000000 upe-0.0.6/upe.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 22:16:19.990922 upe-0.0.7/
+-rw-rw-rw-   0        0        0      191 2023-05-16 22:16:19.990922 upe-0.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-16 22:16:19.976740 upe-0.0.7/libname/
+-rw-rw-rw-   0        0        0       53 2023-05-16 22:02:41.000000 upe-0.0.7/libname/__init__.py
+-rw-rw-rw-   0        0        0    55734 2023-05-16 22:14:54.000000 upe-0.0.7/libname/cdlab.py
+-rw-rw-rw-   0        0        0    30036 2023-05-16 20:15:16.000000 upe-0.0.7/libname/nqueen.py
+-rw-rw-rw-   0        0        0       42 2023-05-16 22:16:19.990922 upe-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      428 2023-05-16 22:15:12.000000 upe-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 22:16:19.988921 upe-0.0.7/upe.egg-info/
+-rw-rw-rw-   0        0        0      191 2023-05-16 22:16:19.000000 upe-0.0.7/upe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      171 2023-05-16 22:16:19.000000 upe-0.0.7/upe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 22:16:19.000000 upe-0.0.7/upe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 22:16:19.000000 upe-0.0.7/upe.egg-info/top_level.txt
```

### Comparing `upe-0.0.6/libname/cdlab.py` & `upe-0.0.7/libname/cdlab.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,15 +588,15 @@
 for x in dfa_states_list:
     for i in x:
         if i in nfa_final_state:
             dfa_final_states.append(x)
             break
 
 print("\nFinal states of the DFA are : ", dfa_final_states)''')
-
+  
 
 
 def leftrec():
   print('''#include <iostream>
 #include <vector>
 #include <string>
 using namespace std;
@@ -1822,21 +1822,15 @@
 // E->T
 // Enter the no. of production of T:2
 // T->T*F
 // T->F
 // Enter the no. of production of F:2
 // F->(E)
 // F->i
-// LEADING(E) = (,*,+,i,
-// LEADING(T) = (,*,i,
-// LEADING(F) = (,i,
-
-// TRAILING(E) = ),*,+,i,
-// TRAILING(T) = ),*,i,
-// TRAILING(F) = ),i,''')
+''')
   
 
 
 def lr0():
   print('''#include <iostream>
 #include <string.h>
 
@@ -2499,8 +2493,9 @@
         if (x->right->label == '_')
             cout << x->right->data;
         else
             cout << x->right->label;
         cout << endl;
     }
     return 0;
-}''')
+}''')
+
```

### Comparing `upe-0.0.6/libname/nqueen.py` & `upe-0.0.7/libname/nqueen.py`

 * *Files identical despite different names*

