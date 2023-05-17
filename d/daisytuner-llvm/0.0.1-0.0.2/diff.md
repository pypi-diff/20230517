# Comparing `tmp/daisytuner_llvm-0.0.1-py3-none-any.whl.zip` & `tmp/daisytuner_llvm-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 17616 bytes, number of entries: 11
--rw-rw-r--  2.0 unx    11656 b- defN 23-May-17 08:20 daisy_clang/__init__.py
--rw-rw-r--  2.0 unx       51 b- defN 23-May-17 08:20 daisy_llvm_helpers/__init__.py
--rw-rw-r--  2.0 unx    11862 b- defN 23-May-17 08:20 daisy_llvm_helpers/llvm2sdfg.py
--rw-rw-r--  2.0 unx     3167 b- defN 23-May-17 08:20 daisy_llvm_helpers/scop2sdfg.py
--rw-rw-r--  2.0 unx    26937 b- defN 23-May-17 08:20 daisy_llvm_helpers/sdfg_generator.py
--rw-rw-r--  2.0 unx    17371 b- defN 23-May-17 08:20 daisy_llvm_helpers/sympy_utils.py
--rw-rw-r--  2.0 unx      474 b- defN 23-May-17 08:24 daisytuner_llvm-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-17 08:24 daisytuner_llvm-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       82 b- defN 23-May-17 08:24 daisytuner_llvm-0.0.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       31 b- defN 23-May-17 08:24 daisytuner_llvm-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      960 b- defN 23-May-17 08:24 daisytuner_llvm-0.0.1.dist-info/RECORD
-11 files, 72683 bytes uncompressed, 15974 bytes compressed:  78.0%
+Zip file size: 17618 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    11656 b- defN 23-May-17 09:18 daisy_clang/__init__.py
+-rw-r--r--  2.0 unx       51 b- defN 23-May-17 09:18 daisy_llvm_helpers/__init__.py
+-rw-r--r--  2.0 unx    11862 b- defN 23-May-17 09:18 daisy_llvm_helpers/llvm2sdfg.py
+-rw-r--r--  2.0 unx     3167 b- defN 23-May-17 09:18 daisy_llvm_helpers/scop2sdfg.py
+-rw-r--r--  2.0 unx    26937 b- defN 23-May-17 09:18 daisy_llvm_helpers/sdfg_generator.py
+-rw-r--r--  2.0 unx    17371 b- defN 23-May-17 09:18 daisy_llvm_helpers/sympy_utils.py
+-rw-r--r--  2.0 unx      476 b- defN 23-May-17 09:19 daisytuner_llvm-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-17 09:19 daisytuner_llvm-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       82 b- defN 23-May-17 09:19 daisytuner_llvm-0.0.2.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       31 b- defN 23-May-17 09:19 daisytuner_llvm-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      960 b- defN 23-May-17 09:19 daisytuner_llvm-0.0.2.dist-info/RECORD
+11 files, 72685 bytes uncompressed, 15976 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: daisy_llvm_helpers/sdfg_generator.py
 Comment: 
 
 Filename: daisy_llvm_helpers/sympy_utils.py
 Comment: 
 
-Filename: daisytuner_llvm-0.0.1.dist-info/METADATA
+Filename: daisytuner_llvm-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: daisytuner_llvm-0.0.1.dist-info/WHEEL
+Filename: daisytuner_llvm-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: daisytuner_llvm-0.0.1.dist-info/entry_points.txt
+Filename: daisytuner_llvm-0.0.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: daisytuner_llvm-0.0.1.dist-info/top_level.txt
+Filename: daisytuner_llvm-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: daisytuner_llvm-0.0.1.dist-info/RECORD
+Filename: daisytuner_llvm-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `daisytuner_llvm-0.0.1.dist-info/RECORD` & `daisytuner_llvm-0.0.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 daisy_clang/__init__.py,sha256=poeW6fh3Ujkp69YF6_uyv7uAlKLj4njFQnshPAdwPnc,11656
 daisy_llvm_helpers/__init__.py,sha256=W9CsyoXcq-_MW40hCSerRcc3HEGAWZ2chZekWNMPu-8,51
 daisy_llvm_helpers/llvm2sdfg.py,sha256=OPjhQQMfDTLIlEvKtjuotWyw6Bz3N7SHmMAtc-m9b3k,11862
 daisy_llvm_helpers/scop2sdfg.py,sha256=_Owyj0L9rXdRPLy9hWi39Li6AEDK4jzEKwKFIr1YXRI,3167
 daisy_llvm_helpers/sdfg_generator.py,sha256=nL-s2_bP0zrOUwY68NrLO5FrqoWU2E7bmMZi_Puktmg,26937
 daisy_llvm_helpers/sympy_utils.py,sha256=tOXOklhndEjUQ4b4o8DgXDYRSdJ8CC5wWIRQcgVDh1w,17371
-daisytuner_llvm-0.0.1.dist-info/METADATA,sha256=R7UxoTBsWX06ihGJihFaOgcMfOTiD3gxfDecBoye54U,474
-daisytuner_llvm-0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-daisytuner_llvm-0.0.1.dist-info/entry_points.txt,sha256=n7cEmtPMUWi9yoW6EBDRzS3BNgl6731DR9xMdkEYOfE,82
-daisytuner_llvm-0.0.1.dist-info/top_level.txt,sha256=-J9KP8Qj9dY-6iYAq7muAFGXTkNFvfQUAlDt33H73-o,31
-daisytuner_llvm-0.0.1.dist-info/RECORD,,
+daisytuner_llvm-0.0.2.dist-info/METADATA,sha256=Lndzv7mu_KR_sa5PtgaZNL3qstytyuDfhfgPYCDG3qo,476
+daisytuner_llvm-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+daisytuner_llvm-0.0.2.dist-info/entry_points.txt,sha256=n7cEmtPMUWi9yoW6EBDRzS3BNgl6731DR9xMdkEYOfE,82
+daisytuner_llvm-0.0.2.dist-info/top_level.txt,sha256=-J9KP8Qj9dY-6iYAq7muAFGXTkNFvfQUAlDt33H73-o,31
+daisytuner_llvm-0.0.2.dist-info/RECORD,,
```

