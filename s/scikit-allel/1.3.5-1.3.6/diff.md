# Comparing `tmp/scikit-allel-1.3.5.tar.gz` & `tmp/scikit-allel-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit-allel-1.3.5.tar", last modified: Fri May 14 10:51:40 2021, max compression
+gzip compressed data, was "scikit-allel-1.3.6.tar", last modified: Wed May 17 19:21:53 2023, max compression
```

## Comparing `scikit-allel-1.3.5.tar` & `scikit-allel-1.3.6.tar`

### file list

```diff
@@ -1,198 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.255323 scikit-allel-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.211322 scikit-allel-1.3.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.227322 scikit-allel-1.3.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1662 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)      812 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/.pep8speaks.yml
--rw-r--r--   0 runner    (1001) docker     (121)      464 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/.pyup.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      178 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2021-05-14 10:51:40.255323 scikit-allel-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      835 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.215323 scikit-allel-1.3.5/allel/
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14839 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.215323 scikit-allel-1.3.5/allel/chunked/
--rw-r--r--   0 runner    (1001) docker     (121)     2268 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/chunked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    31426 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/chunked/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     5918 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/chunked/storage_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (121)     4654 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/chunked/storage_zarr.py
--rw-r--r--   0 runner    (1001) docker     (121)     5363 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/chunked/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.215323 scikit-allel-1.3.5/allel/io/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/io/fasta.py
--rw-r--r--   0 runner    (1001) docker     (121)     7193 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/io/gff.py
--rw-r--r--   0 runner    (1001) docker     (121)     5057 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/io/util.py
--rw-r--r--   0 runner    (1001) docker     (121)    64997 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/io/vcf_read.py
--rw-r--r--   0 runner    (1001) docker     (121)     8677 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/io/vcf_write.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.215323 scikit-allel-1.3.5/allel/model/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33126 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/model/chunked.py
--rw-r--r--   0 runner    (1001) docker     (121)    38051 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/model/dask.py
--rw-r--r--   0 runner    (1001) docker     (121)     9659 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/model/generic.py
--rw-r--r--   0 runner    (1001) docker     (121)   143966 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/model/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (121)     6422 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/model/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.227322 scikit-allel-1.3.5/allel/opt/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   146388 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/opt/io_vcf_read.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    12146 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/opt/model.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    36356 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/opt/stats.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      601 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.219323 scikit-allel-1.3.5/allel/stats/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13375 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/admixture.py
--rw-r--r--   0 runner    (1001) docker     (121)     7922 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/decomposition.py
--rw-r--r--   0 runner    (1001) docker     (121)    11254 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/distance.py
--rw-r--r--   0 runner    (1001) docker     (121)    38740 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/diversity.py
--rw-r--r--   0 runner    (1001) docker     (121)    28050 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/fst.py
--rw-r--r--   0 runner    (1001) docker     (121)     4294 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/hw.py
--rw-r--r--   0 runner    (1001) docker     (121)     9253 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/ld.py
--rw-r--r--   0 runner    (1001) docker     (121)    17768 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/mendel.py
--rw-r--r--   0 runner    (1001) docker     (121)    10155 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (121)    10903 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/roh.py
--rw-r--r--   0 runner    (1001) docker     (121)    39470 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/selection.py
--rw-r--r--   0 runner    (1001) docker     (121)    21820 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/sf.py
--rw-r--r--   0 runner    (1001) docker     (121)    13865 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/stats/window.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.219323 scikit-allel-1.3.5/allel/test/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.223322 scikit-allel-1.3.5/allel/test/data/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2130 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/altlen.vcf
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/ann.vcf
--rw-r--r--   0 runner    (1001) docker     (121)      770 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/eff.vcf
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/empty.vcf
--rw-r--r--   0 runner    (1001) docker     (121)    31882 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/sample.gff
--rw-r--r--   0 runner    (1001) docker     (121)     4680 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/sample.sorted.gff.gz
--rw-r--r--   0 runner    (1001) docker     (121)      628 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/sample.sorted.gff.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (121)     1520 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/sample.utf8.vcf
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/sample.vcf
--rw-r--r--   0 runner    (1001) docker     (121)      954 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/sample.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/sample.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (121)      514 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test1.vcf
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test14.vcf
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test16.vcf
--rw-r--r--   0 runner    (1001) docker     (121)     2056 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test176.vcf
--rw-r--r--   0 runner    (1001) docker     (121)    33743 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test32.vcf
--rw-r--r--   0 runner    (1001) docker     (121)     2152 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test4.vcf
--rw-r--r--   0 runner    (1001) docker     (121)        4 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test48a.vcf
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test48b.vcf
--rw-r--r--   0 runner    (1001) docker     (121)      319 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test54.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (121)      104 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test54.vcf.gz.tbi
--rw-r--r--   0 runner    (1001) docker     (121)     1543 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/test63.vcf
--rw-r--r--   0 runner    (1001) docker     (121)     2052 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/data/unsorted.vcf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.223322 scikit-allel-1.3.5/allel/test/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1426 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/io/test_gff_read.py
--rw-r--r--   0 runner    (1001) docker     (121)   103629 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/io/test_vcf_read.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.223322 scikit-allel-1.3.5/allel/test/model/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.223322 scikit-allel-1.3.5/allel/test/model/ndarray/
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/model/ndarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13824 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/model/ndarray/test_arrays.py
--rw-r--r--   0 runner    (1001) docker     (121)     4091 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/model/ndarray/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2600 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/model/ndarray/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)    94675 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/model/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    20563 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/model/test_chunked.py
--rw-r--r--   0 runner    (1001) docker     (121)     9898 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/model/test_dask.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.223322 scikit-allel-1.3.5/allel/test/stats/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11001 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/stats/test_mendel.py
--rw-r--r--   0 runner    (1001) docker     (121)    18593 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/stats/test_selection.py
--rw-r--r--   0 runner    (1001) docker     (121)     2602 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/stats/test_sf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8225 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    32903 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (121)      903 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/test/tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    13851 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/allel/util.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-14 10:51:39.000000 scikit-allel-1.3.5/allel/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.231323 scikit-allel-1.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     6786 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.231323 scikit-allel-1.3.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/_static/EXISTS
--rw-r--r--   0 runner    (1001) docker     (121)     2998 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/_static/copybutton.js
--rw-r--r--   0 runner    (1001) docker     (121)     2635 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/chunked.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9899 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     4710 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      687 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/io.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.231323 scikit-allel-1.3.5/docs/model/
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/model/chunked.rst
--rw-r--r--   0 runner    (1001) docker     (121)      304 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/model/dask.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5717 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/model/ndarray.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/model/util.rst
--rw-r--r--   0 runner    (1001) docker     (121)      130 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/model.rst
--rw-r--r--   0 runner    (1001) docker     (121)    30336 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/release.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.231323 scikit-allel-1.3.5/docs/stats/
--rw-r--r--   0 runner    (1001) docker     (121)      345 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/admixture.rst
--rw-r--r--   0 runner    (1001) docker     (121)      170 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/decomposition.rst
--rw-r--r--   0 runner    (1001) docker     (121)      397 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/distance.rst
--rw-r--r--   0 runner    (1001) docker     (121)      605 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/diversity.rst
--rw-r--r--   0 runner    (1001) docker     (121)      595 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/fst.rst
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/hw.rst
--rw-r--r--   0 runner    (1001) docker     (121)      286 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/ld.rst
--rw-r--r--   0 runner    (1001) docker     (121)      315 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/mendel.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/misc.rst
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/preprocessing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/roh.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/selection.rst
--rw-r--r--   0 runner    (1001) docker     (121)      960 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/sf.rst
--rw-r--r--   0 runner    (1001) docker     (121)      277 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats/window.rst
--rw-r--r--   0 runner    (1001) docker     (121)      323 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/stats.rst
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/docs/util.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.231323 scikit-allel-1.3.5/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.247322 scikit-allel-1.3.5/notebooks/profiling/
--rw-r--r--   0 runner    (1001) docker     (121)   152634 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/chunked.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    20677 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/diversity_divergence.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    23343 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/fst.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   149312 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/gff3.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  1926480 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/ihs.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   835502 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/ihs_standardization.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   332449 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/io_vcf.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    67346 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/ld.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    24362 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/misc_plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    63637 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/model.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  1808311 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/nsl.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   157232 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/pairwise_distance.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   276425 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/sfs.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      101 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/spike.vcf.gz
--rw-r--r--   0 runner    (1001) docker     (121)    43587 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/tables.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   385913 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/tajima_d.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    28117 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/window_utils.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  2847744 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/xpehh.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  1088214 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/profiling/xpnsl.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   389876 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/repr_html.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.247322 scikit-allel-1.3.5/notebooks/sandbox/
--rw-r--r--   0 runner    (1001) docker     (121)    15792 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/sandbox/chunked_repr.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    49238 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/sandbox/dask_bcolz.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    11312 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/sandbox/dask_count_alleles_mask.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    29543 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/sandbox/dask_map_alleles.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    27728 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/sandbox/dask_profiling.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     6363 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/sandbox/dask_subset.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    14341 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/sandbox/issue_77.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   386118 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/sandbox/phase_by_transmission.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)  3271103 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/notebooks/sandbox/roh_mhmm.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.251323 scikit-allel-1.3.5/profiling/
--rw-r--r--   0 runner    (1001) docker     (121)      235 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/profiling/read_vcf.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)      273 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/release.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/requirements_dev_base.txt
--rw-r--r--   0 runner    (1001) docker     (121)      199 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/requirements_dev_optional.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/requirements_rtfd.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/requirements_test.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.255323 scikit-allel-1.3.5/scikit_allel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2030 2021-05-14 10:51:39.000000 scikit-allel-1.3.5/scikit_allel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6659 2021-05-14 10:51:40.000000 scikit-allel-1.3.5/scikit_allel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-14 10:51:39.000000 scikit-allel-1.3.5/scikit_allel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-14 10:51:39.000000 scikit-allel-1.3.5/scikit_allel.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-05-14 10:51:39.000000 scikit-allel-1.3.5/scikit_allel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-05-14 10:51:39.000000 scikit-allel-1.3.5/scikit_allel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-14 10:51:40.255323 scikit-allel-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-14 10:51:40.255323 scikit-allel-1.3.5/temp/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/temp/donotdelete.txt
--rw-r--r--   0 runner    (1001) docker     (121)      834 2021-05-14 10:51:33.000000 scikit-allel-1.3.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:53.013574 scikit-allel-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.965571 scikit-allel-1.3.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.981572 scikit-allel-1.3.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/.pep8speaks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/.pyup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-17 19:21:53.013574 scikit-allel-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.969571 scikit-allel-1.3.6/allel/
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14839 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.969571 scikit-allel-1.3.6/allel/chunked/
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/chunked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31426 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/chunked/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/chunked/storage_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/chunked/storage_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/chunked/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.973571 scikit-allel-1.3.6/allel/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/io/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/io/gff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/io/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64997 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/io/vcf_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8677 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/io/vcf_write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.973571 scikit-allel-1.3.6/allel/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33126 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/model/chunked.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38051 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/model/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/model/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143965 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/model/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/model/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.985572 scikit-allel-1.3.6/allel/opt/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146388 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/opt/io_vcf_read.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    12146 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/opt/model.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    36356 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/opt/stats.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.977572 scikit-allel-1.3.6/allel/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13375 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/admixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7922 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38740 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28050 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/fst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/hw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/ld.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17768 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/mendel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10155 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10948 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/roh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39470 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21820 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/sf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13865 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/stats/window.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.977572 scikit-allel-1.3.6/allel/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.981572 scikit-allel-1.3.6/allel/test/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/altlen.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/ann.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/eff.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/empty.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)    31882 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/sample.gff
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/sample.sorted.gff.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/sample.sorted.gff.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/sample.utf8.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/sample.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/sample.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/sample.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test1.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test14.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test16.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test176.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)    33743 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test32.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test4.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test48a.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test48b.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test54.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test54.vcf.gz.tbi
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/test63.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/data/unsorted.vcf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.981572 scikit-allel-1.3.6/allel/test/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/io/test_gff_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)   103629 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/io/test_vcf_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.981572 scikit-allel-1.3.6/allel/test/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.981572 scikit-allel-1.3.6/allel/test/model/ndarray/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/model/ndarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/model/ndarray/test_arrays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/model/ndarray/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/model/ndarray/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94675 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/model/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20563 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/model/test_chunked.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/model/test_dask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.981572 scikit-allel-1.3.6/allel/test/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/stats/test_mendel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18604 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/stats/test_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/stats/test_sf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/test/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13851 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/allel/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-17 19:21:52.000000 scikit-allel-1.3.6/allel/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.985572 scikit-allel-1.3.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.989572 scikit-allel-1.3.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/_static/EXISTS
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/_static/copybutton.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/chunked.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9899 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/io.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.989572 scikit-allel-1.3.6/docs/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/model/chunked.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/model/dask.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/model/ndarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/model/util.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30336 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/release.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.989572 scikit-allel-1.3.6/docs/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/admixture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/decomposition.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/distance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/diversity.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/fst.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/hw.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/ld.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/mendel.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/preprocessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/roh.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/selection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/sf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats/window.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/stats.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/docs/util.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:52.989572 scikit-allel-1.3.6/notebooks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:53.005573 scikit-allel-1.3.6/notebooks/profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)   152634 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/chunked.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    20677 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/diversity_divergence.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23343 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/fst.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   149312 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/gff3.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1926480 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/ihs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   835502 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/ihs_standardization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   332449 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/io_vcf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    67346 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/ld.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    24362 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/misc_plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    63637 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/model.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1808311 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/nsl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   157232 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/pairwise_distance.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   276425 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/sfs.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/spike.vcf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    43587 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/tables.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   385913 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/tajima_d.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    28117 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/window_utils.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  2847744 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/xpehh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1088214 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/profiling/xpnsl.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   389876 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/repr_html.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:53.009573 scikit-allel-1.3.6/notebooks/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/sandbox/chunked_repr.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    49238 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/sandbox/dask_bcolz.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11312 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/sandbox/dask_count_alleles_mask.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/sandbox/dask_map_alleles.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27728 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/sandbox/dask_profiling.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/sandbox/dask_subset.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14341 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/sandbox/issue_77.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   386118 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/sandbox/phase_by_transmission.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  3271103 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/notebooks/sandbox/roh_mhmm.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:53.013574 scikit-allel-1.3.6/profiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/profiling/read_vcf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/requirements_dev_base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/requirements_dev_optional.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/requirements_rtfd.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/requirements_test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:53.013574 scikit-allel-1.3.6/scikit_allel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-17 19:21:52.000000 scikit-allel-1.3.6/scikit_allel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-05-17 19:21:52.000000 scikit-allel-1.3.6/scikit_allel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:21:52.000000 scikit-allel-1.3.6/scikit_allel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 19:21:52.000000 scikit-allel-1.3.6/scikit_allel.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 19:21:52.000000 scikit-allel-1.3.6/scikit_allel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-17 19:21:52.000000 scikit-allel-1.3.6/scikit_allel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 19:21:53.013574 scikit-allel-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 19:21:53.013574 scikit-allel-1.3.6/temp/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/temp/donotdelete.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-17 19:21:48.000000 scikit-allel-1.3.6/tox.ini
```

### Comparing `scikit-allel-1.3.5/.github/workflows/deploy.yml` & `scikit-allel-1.3.6/.github/workflows/deploy.yml`

 * *Files 23% similar despite different names*

```diff
@@ -7,62 +7,62 @@
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        os: [ubuntu-20.04, windows-2019, macos-10.15]
+        os: [ubuntu-20.04, windows-2019, macos-11]
 
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         name: Install Python
         with:
           python-version: '3.8'
 
       - name: Build wheels
-        uses: joerick/cibuildwheel@v1.11.0
+        uses: pypa/cibuildwheel@v2.12.3
         env:
-          # Only build on Python 3 (ready for 3.10 when it comes) and skip 32-bit builds
-          CIBW_BUILD: cp3*-*
-          CIBW_SKIP: "*-win32 *-manylinux_i686"
+          # Only build on Python 3 and skip 32-bit builds
+          CIBW_BUILD: "cp3*-*"
+          CIBW_SKIP: "cp36-* cp37-* *-win32 *linux_i686"
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         with:
           path: ./wheelhouse/*.whl
 
   build_sdist:
     name: Build source distribution
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
 
-      - uses: actions/setup-python@v2
+      - uses: actions/setup-python@v4
         name: Install Python
         with:
           python-version: '3.8'
 
       - name: Build sdist
         run: |
           python -m pip install -U setuptools setuptools_scm[toml]
           python setup.py sdist
 
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         with:
           path: dist/*.tar.gz
 
   upload_pypi:
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
     # upload to PyPI on every tag starting with 'v'
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@master
         with:
           user: __token__
```

### Comparing `scikit-allel-1.3.5/.github/workflows/test.yml` & `scikit-allel-1.3.6/.github/workflows/test.yml`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,17 @@
       fail-fast: false
       matrix:
         platform:
         - ubuntu-latest
         - windows-latest
         - macos-latest
         python-version:
-        - 3.7
-        - 3.8
+        - "3.8"
+        - "3.9"
+        - "3.10"
 
     steps:
 
     - uses: actions/checkout@v1
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
@@ -45,16 +46,16 @@
         flake8 allel --count --exit-zero --max-line-length=127 --statistics
 
     - name: Test
       run: |
         pytest -v allel
 
     - name: Test with doctest
-      if: matrix.platform == 'ubuntu-latest' && matrix.python-version == '3.8'
+      if: matrix.platform == 'ubuntu-latest' && matrix.python-version == '3.10'
       run: |
         pytest -v --cov=allel --doctest-modules allel
         coverage report -m
 
     - name: Build docs
-      if: matrix.platform == 'ubuntu-latest' && matrix.python-version == '3.8'
+      if: matrix.platform == 'ubuntu-latest' && matrix.python-version == '3.10'
       run: |
         cd docs && make html
```

### Comparing `scikit-allel-1.3.5/.gitignore` & `scikit-allel-1.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/LICENSE` & `scikit-allel-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/__init__.py` & `scikit-allel-1.3.6/allel/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/abc.py` & `scikit-allel-1.3.6/allel/abc.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/chunked/__init__.py` & `scikit-allel-1.3.6/allel/chunked/__init__.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/chunked/core.py` & `scikit-allel-1.3.6/allel/chunked/core.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/chunked/storage_hdf5.py` & `scikit-allel-1.3.6/allel/chunked/storage_hdf5.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/chunked/storage_zarr.py` & `scikit-allel-1.3.6/allel/chunked/storage_zarr.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/chunked/util.py` & `scikit-allel-1.3.6/allel/chunked/util.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/compat.py` & `scikit-allel-1.3.6/allel/compat.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/io/fasta.py` & `scikit-allel-1.3.6/allel/io/fasta.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/io/gff.py` & `scikit-allel-1.3.6/allel/io/gff.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/io/util.py` & `scikit-allel-1.3.6/allel/io/util.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/io/vcf_read.py` & `scikit-allel-1.3.6/allel/io/vcf_read.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/io/vcf_write.py` & `scikit-allel-1.3.6/allel/io/vcf_write.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/model/chunked.py` & `scikit-allel-1.3.6/allel/model/chunked.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/model/dask.py` & `scikit-allel-1.3.6/allel/model/dask.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/model/generic.py` & `scikit-allel-1.3.6/allel/model/generic.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/model/ndarray.py` & `scikit-allel-1.3.6/allel/model/ndarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -3697,15 +3697,15 @@
         start_indices = np.searchsorted(self, starts)
         stop_indices = np.searchsorted(self, stops, side='right')
 
         # find intervals overlapping at least one value
         loc_ranges = start_indices < stop_indices
 
         # find values within at least one interval
-        loc = np.zeros(self.shape, dtype=np.bool)
+        loc = np.zeros(self.shape, dtype=bool)
         for i, j in zip(start_indices[loc_ranges], stop_indices[loc_ranges]):
             loc[i:j] = True
 
         return loc, loc_ranges
 
     def locate_ranges(self, starts, stops, strict=True):
         """Locate items within the given ranges.
@@ -4467,15 +4467,15 @@
 
         >>> vt['DP']
         array([35, 12, 78, 22, 99])
 
     Access multiple columns::
 
         >>> vt[['DP', 'QD']]
-        <VariantTable shape=(5,) dtype=(numpy.record, {'names':['DP','QD'], ...
+        <VariantTable shape=(5,) dtype=(numpy.record, {'names': ['DP', 'QD'], ...
         [(35, 4.5) (12, 6.7) (78, 1.2) (22, 4.4) (99, 2.8)]
 
     Access a row::
 
         >>> vt[2]
         (b'chr2', 3, 78, 1.2, [5, 6])
```

### Comparing `scikit-allel-1.3.5/allel/model/util.py` & `scikit-allel-1.3.6/allel/model/util.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/opt/io_vcf_read.pyx` & `scikit-allel-1.3.6/allel/opt/io_vcf_read.pyx`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/opt/model.pyx` & `scikit-allel-1.3.6/allel/opt/model.pyx`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/opt/stats.pyx` & `scikit-allel-1.3.6/allel/opt/stats.pyx`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/plot.py` & `scikit-allel-1.3.6/allel/plot.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/admixture.py` & `scikit-allel-1.3.6/allel/stats/admixture.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/decomposition.py` & `scikit-allel-1.3.6/allel/stats/decomposition.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/distance.py` & `scikit-allel-1.3.6/allel/stats/distance.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/diversity.py` & `scikit-allel-1.3.6/allel/stats/diversity.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/fst.py` & `scikit-allel-1.3.6/allel/stats/fst.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/hw.py` & `scikit-allel-1.3.6/allel/stats/hw.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/ld.py` & `scikit-allel-1.3.6/allel/stats/ld.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/mendel.py` & `scikit-allel-1.3.6/allel/stats/mendel.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/misc.py` & `scikit-allel-1.3.6/allel/stats/misc.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/preprocessing.py` & `scikit-allel-1.3.6/allel/stats/preprocessing.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/roh.py` & `scikit-allel-1.3.6/allel/stats/roh.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,16 +90,16 @@
     else:
         p_accessible = is_accessible.mean()
         contig_size = is_accessible.size
 
     emission_mx = _mhmm_derive_emission_matrix(het_px, p_accessible)
 
     # initialize HMM
-    roh_hmm = hmm.MultinomialHMM(n_components=het_px.size)
-    roh_hmm.n_symbols_ = 3
+    # N.B., https://github.com/hmmlearn/hmmlearn/pull/429
+    roh_hmm = hmm.CategoricalHMM(n_components=het_px.size, n_features=3)
     roh_hmm.startprob_ = start_prob
     roh_hmm.transmat_ = transition_mx
     roh_hmm.emissionprob_ = emission_mx
 
     # locate heterozygous calls
     is_het = gv.is_het()
```

### Comparing `scikit-allel-1.3.5/allel/stats/selection.py` & `scikit-allel-1.3.6/allel/stats/selection.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/sf.py` & `scikit-allel-1.3.6/allel/stats/sf.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/stats/window.py` & `scikit-allel-1.3.6/allel/stats/window.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/altlen.vcf` & `scikit-allel-1.3.6/allel/test/data/altlen.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/ann.vcf` & `scikit-allel-1.3.6/allel/test/data/ann.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/eff.vcf` & `scikit-allel-1.3.6/allel/test/data/eff.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/empty.vcf` & `scikit-allel-1.3.6/allel/test/data/empty.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/sample.gff` & `scikit-allel-1.3.6/allel/test/data/sample.gff`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/sample.sorted.gff.gz` & `scikit-allel-1.3.6/allel/test/data/sample.sorted.gff.gz`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/sample.sorted.gff.gz.tbi` & `scikit-allel-1.3.6/allel/test/data/sample.sorted.gff.gz.tbi`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/sample.utf8.vcf` & `scikit-allel-1.3.6/allel/test/data/sample.utf8.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/sample.vcf` & `scikit-allel-1.3.6/allel/test/data/sample.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/sample.vcf.gz` & `scikit-allel-1.3.6/allel/test/data/sample.vcf.gz`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/test1.vcf` & `scikit-allel-1.3.6/allel/test/data/test1.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/test14.vcf` & `scikit-allel-1.3.6/allel/test/data/test14.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/test16.vcf` & `scikit-allel-1.3.6/allel/test/data/test16.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/test176.vcf` & `scikit-allel-1.3.6/allel/test/data/test176.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/test32.vcf` & `scikit-allel-1.3.6/allel/test/data/test32.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/test4.vcf` & `scikit-allel-1.3.6/allel/test/data/test4.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/test48b.vcf` & `scikit-allel-1.3.6/allel/test/data/test48b.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/test63.vcf` & `scikit-allel-1.3.6/allel/test/data/test63.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/data/unsorted.vcf` & `scikit-allel-1.3.6/allel/test/data/unsorted.vcf`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/io/test_gff_read.py` & `scikit-allel-1.3.6/allel/test/io/test_gff_read.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/io/test_vcf_read.py` & `scikit-allel-1.3.6/allel/test/io/test_vcf_read.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/model/ndarray/test_arrays.py` & `scikit-allel-1.3.6/allel/test/model/ndarray/test_arrays.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/model/ndarray/test_indexes.py` & `scikit-allel-1.3.6/allel/test/model/ndarray/test_indexes.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,24 +47,24 @@
         with pytest.raises(ValueError):
             SortedIndex(data)
 
         # valid data (unique)
         data = [1, 4, 5, 7, 12]
         idx = SortedIndex(data)
         aeq(data, idx)
-        assert np.int == idx.dtype
+        assert "i" == idx.dtype.kind
         assert 1 == idx.ndim
         assert 5 == len(idx)
         assert idx.is_unique
 
         # valid data (non-unique)
         data = [1, 4, 5, 5, 7, 12]
         idx = SortedIndex(data)
         aeq(data, idx)
-        assert np.int == idx.dtype
+        assert "i" == idx.dtype.kind
         assert 1 == idx.ndim
         assert 6 == len(idx)
         assert not idx.is_unique
 
         # valid data (typed)
         data = [1, 4, 5, 5, 7, 12]
         idx = SortedIndex(data, dtype='u4')
```

### Comparing `scikit-allel-1.3.5/allel/test/model/ndarray/test_tables.py` & `scikit-allel-1.3.6/allel/test/model/ndarray/test_tables.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/model/test_api.py` & `scikit-allel-1.3.6/allel/test/model/test_api.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/model/test_chunked.py` & `scikit-allel-1.3.6/allel/test/model/test_chunked.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/model/test_dask.py` & `scikit-allel-1.3.6/allel/test/model/test_dask.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/stats/test_mendel.py` & `scikit-allel-1.3.6/allel/test/stats/test_mendel.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/stats/test_selection.py` & `scikit-allel-1.3.6/allel/test/stats/test_selection.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,15 +558,15 @@
     expect = -np.log(5.5/1.5)
 
     for use_threads in True, False:
         for include_edges in True, False:
             score = xpehh(hap1, hap2, pos, include_edges=include_edges,
                           use_threads=use_threads)
             actual = score[9]
-            assert expect == actual
+            assert np.allclose(expect, actual)
 
 
 def test_nsl():
     n_variants = 1000
     n_haplotypes = 20
     h = np.random.randint(0, 2, size=(n_variants, n_haplotypes)).astype('i1')
```

### Comparing `scikit-allel-1.3.5/allel/test/stats/test_sf.py` & `scikit-allel-1.3.6/allel/test/stats/test_sf.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/test_api.py` & `scikit-allel-1.3.6/allel/test/test_api.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/test_stats.py` & `scikit-allel-1.3.6/allel/test/test_stats.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/test/tools.py` & `scikit-allel-1.3.6/allel/test/tools.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/allel/util.py` & `scikit-allel-1.3.6/allel/util.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/Makefile` & `scikit-allel-1.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/_static/copybutton.js` & `scikit-allel-1.3.6/docs/_static/copybutton.js`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/chunked.rst` & `scikit-allel-1.3.6/docs/chunked.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/conf.py` & `scikit-allel-1.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/index.rst` & `scikit-allel-1.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/io.rst` & `scikit-allel-1.3.6/docs/io.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/model/chunked.rst` & `scikit-allel-1.3.6/docs/model/chunked.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/model/ndarray.rst` & `scikit-allel-1.3.6/docs/model/ndarray.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/release.rst` & `scikit-allel-1.3.6/docs/release.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/stats/diversity.rst` & `scikit-allel-1.3.6/docs/stats/diversity.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/stats/fst.rst` & `scikit-allel-1.3.6/docs/stats/fst.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/stats/selection.rst` & `scikit-allel-1.3.6/docs/stats/selection.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/docs/stats/sf.rst` & `scikit-allel-1.3.6/docs/stats/sf.rst`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/chunked.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/chunked.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/diversity_divergence.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/diversity_divergence.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/fst.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/fst.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/gff3.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/gff3.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/ihs.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/ihs.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/ihs_standardization.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/ihs_standardization.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/io_vcf.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/io_vcf.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/ld.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/ld.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/misc_plotting.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/misc_plotting.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/model.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/model.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/nsl.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/nsl.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/pairwise_distance.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/pairwise_distance.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/sfs.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/sfs.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/tables.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/tables.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/tajima_d.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/tajima_d.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/window_utils.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/window_utils.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/xpehh.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/xpehh.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/profiling/xpnsl.ipynb` & `scikit-allel-1.3.6/notebooks/profiling/xpnsl.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/repr_html.ipynb` & `scikit-allel-1.3.6/notebooks/repr_html.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/sandbox/chunked_repr.ipynb` & `scikit-allel-1.3.6/notebooks/sandbox/chunked_repr.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/sandbox/dask_bcolz.ipynb` & `scikit-allel-1.3.6/notebooks/sandbox/dask_bcolz.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/sandbox/dask_count_alleles_mask.ipynb` & `scikit-allel-1.3.6/notebooks/sandbox/dask_count_alleles_mask.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/sandbox/dask_map_alleles.ipynb` & `scikit-allel-1.3.6/notebooks/sandbox/dask_map_alleles.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/sandbox/dask_profiling.ipynb` & `scikit-allel-1.3.6/notebooks/sandbox/dask_profiling.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/sandbox/dask_subset.ipynb` & `scikit-allel-1.3.6/notebooks/sandbox/dask_subset.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/sandbox/issue_77.ipynb` & `scikit-allel-1.3.6/notebooks/sandbox/issue_77.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/sandbox/phase_by_transmission.ipynb` & `scikit-allel-1.3.6/notebooks/sandbox/phase_by_transmission.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/notebooks/sandbox/roh_mhmm.ipynb` & `scikit-allel-1.3.6/notebooks/sandbox/roh_mhmm.ipynb`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/scikit_allel.egg-info/SOURCES.txt` & `scikit-allel-1.3.6/scikit_allel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikit-allel-1.3.5/setup.py` & `scikit-allel-1.3.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,16 +38,17 @@
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Scientific/Engineering',
     'Operating System :: Microsoft :: Windows',
     'Operating System :: POSIX',
     'Operating System :: Unix',
     'Operating System :: MacOS',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.6',
-    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
+    'Programming Language :: Python :: 3.9',
+    'Programming Language :: Python :: 3.10',
 ]
 
 
 # noinspection PyUnresolvedReferences
 def setup_extensions(metadata):
     try:
         print('[scikit-allel] setup extensions with cython')
```

### Comparing `scikit-allel-1.3.5/tox.ini` & `scikit-allel-1.3.6/tox.ini`

 * *Files identical despite different names*

