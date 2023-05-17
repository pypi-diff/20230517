# Comparing `tmp/apsw-3.8.9-r1.tar.gz` & `tmp/apsw-3.9.2-r1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apsw-3.8.9-r1.tar", last modified: Mon Oct 19 00:44:41 2015, max compression
+gzip compressed data, was "dist/apsw-3.9.2-r1.tar", last modified: Fri Jan  8 03:02:10 2016, max compression
```

## Comparing `apsw-3.8.9-r1.tar` & `apsw-3.9.2-r1.tar`

### file list

```diff
@@ -1,27 +1,76 @@
-drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2015-10-19 00:44:41.000000 apsw-3.8.9-r1/
--rw-r--r--   0 rstuart    (501) staff       (20)    14951 2015-10-19 00:42:16.000000 apsw-3.8.9-r1/checksums
--rw-r--r--   0 rstuart    (501) staff       (20)      663 2015-02-12 02:10:07.000000 apsw-3.8.9-r1/MANIFEST.in
--rw-r--r--   0 rstuart    (501) staff       (20)     4332 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/mingwsetup.bat
--rw-r--r--   0 rstuart    (501) staff       (20)      890 2015-10-19 00:44:41.000000 apsw-3.8.9-r1/PKG-INFO
--rw-r--r--   0 rstuart    (501) staff       (20)    33782 2015-02-12 02:10:26.000000 apsw-3.8.9-r1/setup.py
-drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2015-10-19 00:44:41.000000 apsw-3.8.9-r1/src/
--rw-r--r--   0 rstuart    (501) staff       (20)    51721 2015-10-19 00:42:16.000000 apsw-3.8.9-r1/src/apsw.c
--rw-r--r--   0 rstuart    (501) staff       (20)     8154 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/apswbuffer.c
--rw-r--r--   0 rstuart    (501) staff       (20)       32 2015-10-19 00:42:16.000000 apsw-3.8.9-r1/src/apswversion.h
--rw-r--r--   0 rstuart    (501) staff       (20)    12650 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/backup.c
--rw-r--r--   0 rstuart    (501) staff       (20)    22000 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/blob.c
--rw-r--r--   0 rstuart    (501) staff       (20)    96875 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/connection.c
--rw-r--r--   0 rstuart    (501) staff       (20)    43107 2015-10-19 00:42:16.000000 apsw-3.8.9-r1/src/cursor.c
--rw-r--r--   0 rstuart    (501) staff       (20)     9189 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/exceptions.c
--rw-r--r--   0 rstuart    (501) staff       (20)     9243 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/pyutil.c
--rw-r--r--   0 rstuart    (501) staff       (20)    22543 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/statementcache.c
--rw-r--r--   0 rstuart    (501) staff       (20)     1512 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/testextension.c
--rw-r--r--   0 rstuart    (501) staff       (20)     3774 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/traceback.c
--rw-r--r--   0 rstuart    (501) staff       (20)    11808 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/util.c
--rw-r--r--   0 rstuart    (501) staff       (20)    91852 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/vfs.c
--rw-r--r--   0 rstuart    (501) staff       (20)    47093 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/src/vtable.c
--rw-r--r--   0 rstuart    (501) staff       (20)   331286 2015-10-19 00:42:16.000000 apsw-3.8.9-r1/tests.py
-drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2015-10-19 00:44:41.000000 apsw-3.8.9-r1/tools/
--rwxr-xr-x   0 rstuart    (501) staff       (20)    13494 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/tools/apswtrace.py
--rw-r--r--   0 rstuart    (501) staff       (20)   120356 2015-02-12 02:10:07.000000 apsw-3.8.9-r1/tools/shell.py
--rw-r--r--   0 rstuart    (501) staff       (20)    19384 2014-07-07 12:13:23.000000 apsw-3.8.9-r1/tools/speedtest.py
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/
+-rw-r--r--   0 rstuart    (501) staff       (20)    17121 2016-01-08 02:02:59.000000 apsw-3.9.2-r1/checksums
+-rw-r--r--   0 rstuart    (501) staff       (20)      701 2016-01-08 02:52:36.000000 apsw-3.9.2-r1/MANIFEST.in
+-rw-r--r--   0 rstuart    (501) staff       (20)     4332 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/mingwsetup.bat
+-rw-r--r--   0 rstuart    (501) staff       (20)     1225 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/PKG-INFO
+-rw-r--r--   0 rstuart    (501) staff       (20)    34798 2016-01-08 02:58:58.000000 apsw-3.9.2-r1/setup.py
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/sqlite3/
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/sqlite3/.deps/
+-rw-r--r--   0 rstuart    (501) staff       (20)        8 2016-01-08 02:05:54.000000 apsw-3.9.2-r1/sqlite3/.deps/sqlite3-shell.Po
+-rw-r--r--   0 rstuart    (501) staff       (20)        8 2016-01-08 02:05:54.000000 apsw-3.9.2-r1/sqlite3/.deps/sqlite3-sqlite3.Po
+-rw-r--r--   0 rstuart    (501) staff       (20)        8 2016-01-08 02:05:54.000000 apsw-3.9.2-r1/sqlite3/.deps/sqlite3.Plo
+-rw-r--r--   0 rstuart    (501) staff       (20)   343598 2015-11-02 18:44:07.000000 apsw-3.9.2-r1/sqlite3/aclocal.m4
+-rwxr-xr-x   0 rstuart    (501) staff       (20)    44826 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/config.guess
+-rw-r--r--   0 rstuart    (501) staff       (20)    36535 2016-01-08 02:05:54.000000 apsw-3.9.2-r1/sqlite3/config.log
+-rwxr-xr-x   0 rstuart    (501) staff       (20)    58687 2016-01-08 02:05:54.000000 apsw-3.9.2-r1/sqlite3/config.status
+-rwxr-xr-x   0 rstuart    (501) staff       (20)    35454 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/config.sub
+-rwxr-xr-x   0 rstuart    (501) staff       (20)   441410 2015-11-02 18:44:08.000000 apsw-3.9.2-r1/sqlite3/configure
+-rw-r--r--   0 rstuart    (501) staff       (20)     4104 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/configure.ac
+-rwxr-xr-x   0 rstuart    (501) staff       (20)    20899 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/depcomp
+-rw-r--r--   0 rstuart    (501) staff       (20)    15744 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/INSTALL
+-rwxr-xr-x   0 rstuart    (501) staff       (20)    13998 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/install-sh
+-rwxr-xr-x   0 rstuart    (501) staff       (20)   293441 2016-01-08 02:05:54.000000 apsw-3.9.2-r1/sqlite3/libtool
+-rw-r--r--   0 rstuart    (501) staff       (20)   283477 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/ltmain.sh
+-rw-r--r--   0 rstuart    (501) staff       (20)    34416 2016-01-08 02:05:54.000000 apsw-3.9.2-r1/sqlite3/Makefile
+-rw-r--r--   0 rstuart    (501) staff       (20)      540 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/Makefile.am
+-rw-r--r--   0 rstuart    (501) staff       (20)    34647 2015-11-02 18:44:08.000000 apsw-3.9.2-r1/sqlite3/Makefile.in
+-rwxr-xr-x   0 rstuart    (501) staff       (20)    10346 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/missing
+-rw-r--r--   0 rstuart    (501) staff       (20)     1144 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/README
+-rw-r--r--   0 rstuart    (501) staff       (20)   152869 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/shell.c
+-rw-r--r--   0 rstuart    (501) staff       (20)     8928 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/sqlite3.1
+-rw-r--r--   0 rstuart    (501) staff       (20)  6461369 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/sqlite3.c
+-rw-r--r--   0 rstuart    (501) staff       (20)   405263 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/sqlite3.h
+-rw-r--r--   0 rstuart    (501) staff       (20)      262 2016-01-08 02:05:54.000000 apsw-3.9.2-r1/sqlite3/sqlite3.pc
+-rw-r--r--   0 rstuart    (501) staff       (20)      267 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/sqlite3.pc.in
+-rw-r--r--   0 rstuart    (501) staff       (20)      640 2016-01-08 02:05:54.000000 apsw-3.9.2-r1/sqlite3/sqlite3config.h
+-rw-r--r--   0 rstuart    (501) staff       (20)    28809 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/sqlite3ext.h
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/sqlite3/tea/
+-rw-r--r--   0 rstuart    (501) staff       (20)      147 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/aclocal.m4
+-rwxr-xr-x   0 rstuart    (501) staff       (20)   280822 2015-11-02 18:44:09.000000 apsw-3.9.2-r1/sqlite3/tea/configure
+-rw-r--r--   0 rstuart    (501) staff       (20)     8352 2015-11-02 18:44:08.000000 apsw-3.9.2-r1/sqlite3/tea/configure.ac
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/sqlite3/tea/doc/
+-rw-r--r--   0 rstuart    (501) staff       (20)      494 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/doc/sqlite3.n
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/sqlite3/tea/generic/
+-rw-r--r--   0 rstuart    (501) staff       (20)   121326 2015-11-02 18:44:08.000000 apsw-3.9.2-r1/sqlite3/tea/generic/tclsqlite3.c
+-rw-r--r--   0 rstuart    (501) staff       (20)      257 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/license.terms
+-rw-r--r--   0 rstuart    (501) staff       (20)    15902 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/Makefile.in
+-rw-r--r--   0 rstuart    (501) staff       (20)      167 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/pkgIndex.tcl.in
+-rw-r--r--   0 rstuart    (501) staff       (20)     1338 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/README
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/sqlite3/tea/tclconfig/
+-rw-r--r--   0 rstuart    (501) staff       (20)    13868 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/tclconfig/install-sh
+-rw-r--r--   0 rstuart    (501) staff       (20)   134055 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/tclconfig/tcl.m4
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/sqlite3/tea/win/
+-rw-r--r--   0 rstuart    (501) staff       (20)    13830 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/win/makefile.vc
+-rw-r--r--   0 rstuart    (501) staff       (20)    17329 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/win/nmakehlp.c
+-rw-r--r--   0 rstuart    (501) staff       (20)    18743 2015-11-02 18:44:06.000000 apsw-3.9.2-r1/sqlite3/tea/win/rules.vc
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/src/
+-rw-r--r--   0 rstuart    (501) staff       (20)    51840 2016-01-08 02:02:59.000000 apsw-3.9.2-r1/src/apsw.c
+-rw-r--r--   0 rstuart    (501) staff       (20)     8154 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/src/apswbuffer.c
+-rw-r--r--   0 rstuart    (501) staff       (20)       32 2016-01-08 02:02:59.000000 apsw-3.9.2-r1/src/apswversion.h
+-rw-r--r--   0 rstuart    (501) staff       (20)    12690 2016-01-08 02:02:59.000000 apsw-3.9.2-r1/src/backup.c
+-rw-r--r--   0 rstuart    (501) staff       (20)    22160 2016-01-08 02:02:59.000000 apsw-3.9.2-r1/src/blob.c
+-rw-r--r--   0 rstuart    (501) staff       (20)    97708 2016-01-08 02:02:59.000000 apsw-3.9.2-r1/src/connection.c
+-rw-r--r--   0 rstuart    (501) staff       (20)    43107 2016-01-08 02:02:59.000000 apsw-3.9.2-r1/src/cursor.c
+-rw-r--r--   0 rstuart    (501) staff       (20)     9189 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/src/exceptions.c
+-rw-r--r--   0 rstuart    (501) staff       (20)     9243 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/src/pyutil.c
+-rw-r--r--   0 rstuart    (501) staff       (20)    22543 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/src/statementcache.c
+-rw-r--r--   0 rstuart    (501) staff       (20)     1512 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/src/testextension.c
+-rw-r--r--   0 rstuart    (501) staff       (20)     3774 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/src/traceback.c
+-rw-r--r--   0 rstuart    (501) staff       (20)    11808 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/src/util.c
+-rw-r--r--   0 rstuart    (501) staff       (20)    91827 2016-01-08 02:02:59.000000 apsw-3.9.2-r1/src/vfs.c
+-rw-r--r--   0 rstuart    (501) staff       (20)    47093 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/src/vtable.c
+-rw-r--r--   0 rstuart    (501) staff       (20)   332396 2016-01-08 02:02:59.000000 apsw-3.9.2-r1/tests.py
+drwxr-xr-x   0 rstuart    (501) staff       (20)        0 2016-01-08 03:02:10.000000 apsw-3.9.2-r1/tools/
+-rwxr-xr-x   0 rstuart    (501) staff       (20)    13494 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/tools/apswtrace.py
+-rw-r--r--   0 rstuart    (501) staff       (20)   120356 2016-01-08 02:03:46.000000 apsw-3.9.2-r1/tools/shell.py
+-rw-r--r--   0 rstuart    (501) staff       (20)    19384 2014-07-07 12:13:23.000000 apsw-3.9.2-r1/tools/speedtest.py
```

### Comparing `apsw-3.8.9-r1/checksums` & `apsw-3.9.2-r1/checksums`

 * *Files 4% similar despite different names*

```diff
@@ -150,8 +150,27 @@
 https://sqlite.org/2015/sqlite-autoconf-3080802.tar.gz 2021091 1db237523419af7110e1d92c6b766e965f9322e4 3425fa580a56880f56bcb887dd26cc06
 
 https://sqlite.org/2015/sqlite-amalgamation-3080803.zip    1568475 fdac82a811fb62a6e326808f0010b2cd8e9055d2 97604645c615d81194541e1398687b61
 https://sqlite.org/2015/sqlite-autoconf-3080803.tar.gz 2021112 2fe3f6226a2a08a2e814b97cd53e36bb3c597112 51272e875879ee893e51070b07c33888
 
 https://sqlite.org/2015/sqlite-amalgamation-3080900.zip    1584545 f70e2841e4f26fe45849c2b9f5683bbe502d7523 02e9c3a6daa8b8587cf6bef828c2e33f
 https://sqlite.org/2015/sqlite-autoconf-3080900.tar.gz 2037200 db70dee268700b312cbaa5b3e5cf8454e1c8b7b9 6a18d4609852f4b63f812a1059df468f
-^Chttps://sqlite.org/2015/sqlite-amalgamation-3080803.zip
+
+https://sqlite.org/2015/sqlite-amalgamation-3081002.zip    1596554 9ad3b477de04cc480fc0f7f1829c322c525f642d cb79cf3d8bab37072209d30cf4d11350
+https://sqlite.org/2015/sqlite-autoconf-3081002.tar.gz 2049387 c2f2c17d3dc4c4e179d35cc04e4420636d48a152 a18bfc015cd49a1e7a961b7b77bc3b37
+https://sqlite.org/2015/sqlite-amalgamation-3081001.zip    1596541 6e371df68010b9521a8d5e0795ef8a4acb6c3ef8 913478c71e1b179f87772aba9474f683
+https://sqlite.org/2015/sqlite-autoconf-3081001.tar.gz 2049377 86bfed5752783fb24c051f3efac5972ce11023f0 8bd9d7df3f67bc771f53c6dda42face2
+https://sqlite.org/2015/sqlite-amalgamation-3081000.zip    1596326 a0b064f09ce78e6e38453a7057eb05c4dbf25657 9e944369c6c477b76790abc45ced3843
+https://sqlite.org/2015/sqlite-autoconf-3081000.tar.gz 2049170 7e92b4f78d4648fb2a97a4dc721490cc08653a0b 04d0311ef70818e8d914c1dc383eddff
+
+https://sqlite.org/2015/sqlite-amalgamation-3081100.zip    1648834 bdd01fa7167b697f30ab76f42f4200bf58b75d98 1867eaa496c9e3dcd77c117fd05a9c5d
+https://sqlite.org/2015/sqlite-autoconf-3081100.tar.gz 2101901 da1322d883548bdb0f6312941b20ed497e3754fa 77b451925121028befbddbf45ea2bc49
+
+https://sqlite.org/2015/sqlite-amalgamation-3081101.zip    1648868 0dbb29c71c4385d1000c091f14475106784daceb 94907e831502e2080b76e281cfa24dde
+https://sqlite.org/2015/sqlite-autoconf-3081101.tar.gz 2101885 d0e22d7e361b6f50830a3cdeafe35311443f8f9a 298c8d6af7ca314f68de92bc7a356cbe
+
+https://sqlite.org/2015/sqlite-amalgamation-3090200.zip    1830895 2837b7f910a217aadc6e5862fcb8f6a3e365622b 0b1787d449b10fa9d7c0edeb15aa6f9f
+https://sqlite.org/2015/sqlite-autoconf-3090200.tar.gz 2284431 dae1ae5297fece9671ae0c434a7ecd0cda09c76a bc4eb5b3fc5cfcb6e059794306cac1ca
+https://sqlite.org/2015/sqlite-amalgamation-3090100.zip    1830615 3113a7656a25b21d6368af75592b57a7c9edf747 09aaf9e68d0ae44c0a001adc46d0ac26
+https://sqlite.org/2015/sqlite-autoconf-3090100.tar.gz 2284128 6b7d22c24c9695118a2706c8e026fb3c31780a30 74931054399a2d7acf35637efe8d6f45
+https://sqlite.org/2015/sqlite-amalgamation-3090000.zip    1830511 ac803cd1283b01b398beb565ebee774c7ca85515 93fe1d55ac14a9288661a8203b36470b
+https://sqlite.org/2015/sqlite-autoconf-3090000.tar.gz 2283997 6578aa8df05fd7777fbbc4fbf1912d981623f73b cd0f883b2ddfc29e8e1bbbbd8e85f555
```

### Comparing `apsw-3.8.9-r1/MANIFEST.in` & `apsw-3.9.2-r1/MANIFEST.in`

 * *Files 12% similar despite different names*

```diff
@@ -24,7 +24,10 @@
 include mingwsetup.bat
 include setup.py
 include tools/speedtest.py
 include tools/apswtrace.py
 # shell is not needed at runtime - we compile it into the C source
 include tools/shell.py
 include tests.py
+
+# Sqlite
+recursive-include sqlite3 *
```

### Comparing `apsw-3.8.9-r1/mingwsetup.bat` & `apsw-3.9.2-r1/mingwsetup.bat`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/PKG-INFO` & `apsw-3.9.2-r1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 Metadata-Version: 1.1
 Name: apsw
-Version: 3.8.9-r1
+Version: 3.9.2-r1
 Summary: Another Python SQLite Wrapper
 Home-page: https://github.com/rogerbinns/apsw/
 Author: Roger Binns
 Author-email: rogerb@rogerbinns.com
 License: OSI Approved ::
 Description: A Python wrapper for the SQLite embedded relational database engine.
         In contrast to other wrappers such as pysqlite it focuses on being
         a minimal layer over SQLite attempting just to translate the
         complete SQLite API into Python.
+        
+        This packge is provided by a third party and NOT the original package
+        creater. It bundles sqlite 3 (via `python setup.py fetch --sqlite`) so
+        the packge can be cleanly installed. *PLEASE CAREFULLY REVIEW THE INSTALL
+        INSTRUCTIONS FOR APSW TO BE SURE THIS IS THE RIGHT SOLUTION FOR YOU!*
+        
 Keywords: database,sqlite
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
```

### Comparing `apsw-3.8.9-r1/setup.py` & `apsw-3.9.2-r1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,29 +229,44 @@
                 write("Unable to determine current SQLite version.  Use --version=VERSION", sys.stderr)
                 write("to set version - eg setup.py fetch --version=3.6.18", sys.stderr)
                 sys.exit(17)
             write("    Version is "+self.version)
         # now get each selected component
         downloaded=0
 
-        if self.version!="fossil":
+        if not self.version.startswith("fossil"):
             v=[int(x) for x in self.version.split(".")]
             if len(v)<4:
                 v.append(0)
             self.webversion="%d%02d%02d%02d" % tuple(v)
 
         ## The amalgamation
         if self.sqlite:
-            if self.version=="fossil":
-                write("  Getting current trunk from fossil")
+            if self.version.startswith("fossil"):
+                write("  Getting code from fossil")
             else:
                 write("  Getting the SQLite amalgamation")
 
-            if self.version=="fossil":
-                AURL="https://sqlite.org/src/zip/sqlite3.zip?uuid=trunk"
+            if self.version.startswith("fossil"):
+                if self.version=="fossil":
+                    uuid="trunk"
+                else:
+                    showmsg=False
+                    if not self.version.startswith("fossil-"):
+                        showmsg=True
+                    else:
+                        uuid=self.version.split("-", 1)[1]
+                        if not uuid:
+                            showmsg=True
+                    if showmsg:
+                        write("Use fossil-HASH to identify a partifular commit", sys.stderr)
+                        write("eg  fossil-3a82c8e6", sys.stderr)
+                        sys.exit(18)
+
+                AURL="https://sqlite.org/src/zip/sqlite3.zip?uuid="+uuid
                 checksum=False
             else:
                 if sys.platform=="win32":
                     AURL="https://sqlite.org/sqlite-amalgamation-%s.zip" % (self.webversion,)
                 else:
                     AURL="https://sqlite.org/sqlite-autoconf-%s.tar.gz" % (self.webversion,)
                 checksum=True
@@ -285,15 +300,15 @@
                 if os.path.exists('sqlite3'):
                     for dirpath, dirnames, filenames in os.walk('sqlite3', topdown=False):
                         for file in filenames:
                             os.remove(os.path.join(dirpath, file))
                         for dir in dirnames:
                             os.rmdir(os.path.join(dirpath, dir))
                     os.rmdir('sqlite3')
-                if self.version=="fossil":
+                if self.version.startswith("fossil"):
                     zip=zipfile.ZipFile(data, "r")
                     for name in zip.namelist():
                         # extract
                         if name.endswith("/"):
                             os.mkdir(name)
                         else:
                             open(name, "wb").write(zip.read(name))
@@ -312,15 +327,15 @@
                     # the directory name has changed a bit with each release so try to work out what it is
                     if not configmember:
                         write("Unable to determine directory it extracted to.", dest=sys.stderr)
                         sys.exit(19)
                     dirname=configmember.name.split('/')[0]
                     os.rename(dirname, 'sqlite3')
                 os.chdir('sqlite3')
-                if self.version=="fossil":
+                if self.version.startswith("fossil"):
                     write("    Building amalgamation from fossil")
                     res=os.system("make TOP=. -f Makefile.linux-gcc sqlite3.c && cp src/sqlite3ext.h .")
                     defs=[]
                     if sqlite3config_h:
                         open("sqlite3config.h", "wb").write(sqlite3config_h)
                 else:
                     write("    Running configure to work out SQLite compilation flags")
@@ -601,15 +616,16 @@
                 # tries to catch misspelling the name of an extension.
                 # However the SQLITE_ENABLE prefix is also used by other
                 # options - see https://sqlite.org/compile.html but almost
                 # all of those have _ in them, so our abbreviated and
                 # hopefully future proof test
                 if "_" not in e.lower() and \
                        "memsys" not in e.lower() and \
-                       e.lower() not in ("fts4", "fts3", "rtree", "icu", "iotrace", "stat2", "stat3", "stat4"):
+                       e.lower() not in ("fts4", "fts3", "rtree", "icu", "iotrace",
+                                         "stat2", "stat3", "stat4", "dbstat_vtab"):
                     write("Unknown enable "+e, sys.stderr)
                     raise ValueError("Bad enable "+e)
 
         # omits
         if self.omit:
             for e in self.omit.split(","):
                 e=e.strip()
@@ -829,15 +845,21 @@
 setup(name="apsw",
       version=version,
       description="Another Python SQLite Wrapper",
       long_description=\
 """A Python wrapper for the SQLite embedded relational database engine.
 In contrast to other wrappers such as pysqlite it focuses on being
 a minimal layer over SQLite attempting just to translate the
-complete SQLite API into Python.""",
+complete SQLite API into Python.
+
+This packge is provided by a third party and NOT the original package
+creater. It bundles sqlite 3 (via `python setup.py fetch --sqlite`) so
+the packge can be cleanly installed. *PLEASE CAREFULLY REVIEW THE INSTALL
+INSTRUCTIONS FOR APSW TO BE SURE THIS IS THE RIGHT SOLUTION FOR YOU!*
+""",
       author="Roger Binns",
       author_email="rogerb@rogerbinns.com",
       url="https://github.com/rogerbinns/apsw/",
       classifiers=[
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved",
```

### Comparing `apsw-3.8.9-r1/src/apsw.c` & `apsw-3.9.2-r1/src/apsw.c`

 * *Files 0% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 #endif
 
 #else
 /* SQLite 3 headers */
 #include "sqlite3.h"
 #endif
 
-#if SQLITE_VERSION_NUMBER < 3008009
-#error Your SQLite version is too old.  It must be at least 3.8.9
+#if SQLITE_VERSION_NUMBER < 3009000
+#error Your SQLite version is too old.  It must be at least 3.9
 #endif
 
 /* system headers */
 #include <assert.h>
 #include <stdarg.h>
 
 /* Get the version number */
@@ -528,32 +528,33 @@
   :param reset: If *True* then the highwater is set to the current value
   :returns: A tuple of current value and highwater value
 
   .. seealso::
 
     * :ref:`Status example <example-status>`
 
-  -* sqlite3_status
+  -* sqlite3_status64
 
 */
 static PyObject *
 status(APSW_ARGUNUSED PyObject *self, PyObject *args)
 {
-  int res, op, current=0, highwater=0, reset=0;
+  int res, op, reset=0;
+  sqlite3_int64 current=0, highwater=0;
 
   if(!PyArg_ParseTuple(args, "i|i:status(op, reset=False)", &op, &reset))
     return NULL;
 
-  res=sqlite3_status(op, &current, &highwater, reset);
+  res=sqlite3_status64(op, &current, &highwater, reset);
   SET_EXC(res, NULL);
 
   if(res!=SQLITE_OK)
     return NULL;
 
-  return Py_BuildValue("(ii)", current, highwater);
+  return Py_BuildValue("(LL)", current, highwater);
 }
 
 /** .. method:: vfsnames() -> list(string)
 
   Returns a list of the currently installed :ref:`vfs <vfs>`.  The first
   item in the list is the default vfs.
 */
@@ -1504,14 +1505,15 @@
       ADDINT(SQLITE_IOERR_GETTEMPPATH),
       ADDINT(SQLITE_WARNING_AUTOINDEX),
       ADDINT(SQLITE_CANTOPEN_CONVPATH),
       ADDINT(SQLITE_IOERR_CONVPATH),
       ADDINT(SQLITE_CONSTRAINT_ROWID),
       ADDINT(SQLITE_READONLY_DBMOVED),
       ADDINT(SQLITE_AUTH_USER),
+      ADDINT(SQLITE_IOERR_VNODE),
       END,
 
       /* error codes */
       DICT("mapping_result_codes"),
       ADDINT(SQLITE_OK),
       ADDINT(SQLITE_ERROR),
       ADDINT(SQLITE_INTERNAL),
@@ -1712,14 +1714,16 @@
       ADDINT(SQLITE_FCNTL_HAS_MOVED),
       ADDINT(SQLITE_FCNTL_SYNC),
       ADDINT(SQLITE_FCNTL_WIN32_SET_HANDLE),
       ADDINT(SQLITE_FCNTL_LAST_ERRNO),
       ADDINT(SQLITE_FCNTL_WAL_BLOCK),
       ADDINT(SQLITE_FCNTL_GET_LOCKPROXYFILE),
       ADDINT(SQLITE_FCNTL_SET_LOCKPROXYFILE),
+      ADDINT(SQLITE_FCNTL_RBU),
+      ADDINT(SQLITE_FCNTL_ZIPVFS),
       END,
 
       DICT("mapping_conflict_resolution_modes"),
       ADDINT(SQLITE_ROLLBACK),
       ADDINT(SQLITE_IGNORE),
       ADDINT(SQLITE_FAIL),
       ADDINT(SQLITE_ABORT),
```

### Comparing `apsw-3.8.9-r1/src/apswbuffer.c` & `apsw-3.9.2-r1/src/apswbuffer.c`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/src/backup.c` & `apsw-3.9.2-r1/src/backup.c`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,16 @@
   CHECK_USE(NULL);
   CHECK_BACKUP_CLOSED(NULL);
 
   if(args && !PyArg_ParseTuple(args, "|i:step(pages=All)", &pages))
     return NULL;
 
   PYSQLITE_BACKUP_CALL(res=sqlite3_backup_step(self->backup, pages));
+  if(PyErr_Occurred())
+    return NULL;
 
   if(res==SQLITE_DONE)
     {
       if(self->done!=Py_True)
         {
           Py_CLEAR(self->done);
           self->done=Py_True;
```

### Comparing `apsw-3.8.9-r1/src/blob.c` & `apsw-3.9.2-r1/src/blob.c`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,16 @@
 
   buffy=PyBytes_FromStringAndSize(NULL, length);
 
   if(!buffy) return NULL;
 
   thebuffer= PyBytes_AS_STRING(buffy);
   PYSQLITE_BLOB_CALL(res=sqlite3_blob_read(self->pBlob, thebuffer, length, self->curoffset));
+  if(PyErr_Occurred())
+    return NULL;
 
   if(res!=SQLITE_OK)
     {
       Py_DECREF(buffy);
       SET_EXC(res, self->connection->db);
       return NULL;
     }
@@ -426,14 +428,16 @@
   if(offset+lengthwanted>bufsize)
     return PyErr_Format(PyExc_ValueError, "Data would go beyond end of buffer");
 
   if(lengthwanted>bloblen-self->curoffset)
     return PyErr_Format(PyExc_ValueError, "More data requested than blob length");
 
   PYSQLITE_BLOB_CALL(res=sqlite3_blob_read(self->pBlob, (char*)buffer+offset, lengthwanted, self->curoffset));
+  if(PyErr_Occurred())
+    return NULL;
 
   if(res!=SQLITE_OK)
     {
       SET_EXC(res, self->connection->db);
       return NULL;
     }
   self->curoffset+=lengthwanted;
@@ -540,14 +544,16 @@
   if( ((int)(size+self->curoffset))<self->curoffset)
     return PyErr_Format(PyExc_ValueError, "Data is too large (integer wrap)");
 
   if( ((int)(size+self->curoffset))>sqlite3_blob_bytes(self->pBlob))
     return PyErr_Format(PyExc_ValueError, "Data would go beyond end of blob");
 
   PYSQLITE_BLOB_CALL(res=sqlite3_blob_write(self->pBlob, buffer, size, self->curoffset));
+  if(PyErr_Occurred())
+    return NULL;
 
   if(res!=SQLITE_OK)
     {
       SET_EXC(res, self->connection->db);
       return NULL;
     }
   else
@@ -675,14 +681,17 @@
     else
       return PyErr_Format(PyExc_TypeError, "blob reopen argument must be a number");
 
   /* no matter what happens we always reset current offset */
   self->curoffset=0;
 
   PYSQLITE_BLOB_CALL(res=sqlite3_blob_reopen(self->pBlob, rowid));
+  if(PyErr_Occurred())
+    return NULL;
+
   if(res!=SQLITE_OK)
     {
       SET_EXC(res, self->connection->db);
       return NULL;
     }
   Py_RETURN_NONE;
 }
@@ -756,8 +765,7 @@
     0,                         /* tp_mro */
     0,                         /* tp_cache */
     0,                         /* tp_subclasses */
     0,                         /* tp_weaklist */
     0                          /* tp_del */
     APSW_PYTYPE_VERSION
 };
-
```

### Comparing `apsw-3.8.9-r1/src/connection.c` & `apsw-3.9.2-r1/src/connection.c`

 * *Files 2% similar despite different names*

```diff
@@ -2222,21 +2222,27 @@
   gilstate=PyGILState_Ensure();
 
   Py_XDECREF((PyObject*)funcinfo);
 
   PyGILState_Release(gilstate);
 }
 
-/** .. method:: createscalarfunction(name, callable[, numargs=-1])
+/** .. method:: createscalarfunction(name, callable[, numargs=-1, deterministic=False])
 
   Registers a scalar function.  Scalar functions operate on one set of paramaters once.
 
   :param name: The string name of the function.  It should be less than 255 characters
   :param callable: The function that will be called
   :param numargs: How many arguments the function takes, with -1 meaning any number
+  :param deterministic: When True this means the function always
+           returns the same result for the same input arguments.
+           SQLite's query planner can perform additional optimisations
+           for deterministic functions.  For example a random()
+           function is not deterministic while one that returns the
+           length of a string is.
 
   .. note::
 
     You can register the same named function but with different
     *callable* and *numargs*.  For example::
 
       connection.createscalarfunction("toip", ipv4convert, 4)
@@ -2251,30 +2257,39 @@
      * :ref:`Example <scalar-example>`
      * :meth:`~Connection.createaggregatefunction`
 
   -* sqlite3_create_function_v2
 */
 
 static PyObject *
-Connection_createscalarfunction(Connection *self, PyObject *args)
+Connection_createscalarfunction(Connection *self, PyObject *args, PyObject *kwargs)
 {
+  static char *kwlist[]={"name", "callable", "numargs", "deterministic", NULL};
   int numargs=-1;
-  PyObject *callable;
+  PyObject *callable=NULL;
+  PyObject *odeterministic=NULL;
+  int deterministic=0;
   char *name=0;
   FunctionCBInfo *cbinfo;
   int res;
 
   CHECK_USE(NULL);
   CHECK_CLOSED(self,NULL);
 
-  if(!PyArg_ParseTuple(args, "esO|i:createscalarfunction(name,callback, numargs=-1)", STRENCODING, &name, &callable, &numargs))
+  if(!PyArg_ParseTupleAndKeywords(args, kwargs, "esO|iO!:createscalarfunction(name,callback, numargs=-1, deterministic=False)",
+                                  kwlist, STRENCODING, &name, &callable, &numargs, &PyBool_Type, &odeterministic))
     return NULL;
 
   assert(name);
   assert(callable);
+  if(odeterministic) {
+    res=PyObject_IsTrue(odeterministic);
+    if (res<0) return NULL;
+    deterministic=res;
+  }
 
   if(callable!=Py_None && !PyCallable_Check(callable))
     {
       PyMem_Free(name);
       PyErr_SetString(PyExc_TypeError, "parameter must be callable");
       return NULL;
     }
@@ -2292,15 +2307,15 @@
       Py_INCREF(callable);
     }
 
   PYSQLITE_CON_CALL(
                 res=sqlite3_create_function_v2(self->db,
 					       name,
 					       numargs,
-					       SQLITE_UTF8,
+					       SQLITE_UTF8|(deterministic?SQLITE_DETERMINISTIC:0),
 					       cbinfo,
 					       cbinfo?cbdispatch_func:NULL,
 					       NULL,
 					       NULL,
 					       apsw_free_func)
                 );
   if(res)
@@ -3318,15 +3333,15 @@
    "Create a new cursor" },
   {"close",  (PyCFunction)Connection_close, METH_VARARGS,
    "Closes the connection" },
   {"setbusytimeout", (PyCFunction)Connection_setbusytimeout, METH_VARARGS,
    "Sets the sqlite busy timeout in milliseconds.  Use zero to disable the timeout"},
   {"interrupt", (PyCFunction)Connection_interrupt, METH_NOARGS,
    "Causes any pending database operations to abort at the earliest opportunity"},
-  {"createscalarfunction", (PyCFunction)Connection_createscalarfunction, METH_VARARGS,
+  {"createscalarfunction", (PyCFunction)Connection_createscalarfunction, METH_VARARGS|METH_KEYWORDS,
    "Creates a scalar function"},
   {"createaggregatefunction", (PyCFunction)Connection_createaggregatefunction, METH_VARARGS,
    "Creates an aggregate function"},
   {"setbusyhandler", (PyCFunction)Connection_setbusyhandler, METH_O,
    "Sets the busy handler"},
   {"changes", (PyCFunction)Connection_changes, METH_NOARGS,
    "Returns the number of rows changed by last query"},
@@ -3450,8 +3465,7 @@
     0,                         /* tp_mro */
     0,                         /* tp_cache */
     0,                         /* tp_subclasses */
     0,                         /* tp_weaklist */
     0                          /* tp_del */
     APSW_PYTYPE_VERSION
 };
-
```

### Comparing `apsw-3.8.9-r1/src/cursor.c` & `apsw-3.9.2-r1/src/cursor.c`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/src/exceptions.c` & `apsw-3.9.2-r1/src/exceptions.c`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/src/pyutil.c` & `apsw-3.9.2-r1/src/pyutil.c`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/src/statementcache.c` & `apsw-3.9.2-r1/src/statementcache.c`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/src/testextension.c` & `apsw-3.9.2-r1/src/testextension.c`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/src/traceback.c` & `apsw-3.9.2-r1/src/traceback.c`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/src/util.c` & `apsw-3.9.2-r1/src/util.c`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/src/vfs.c` & `apsw-3.9.2-r1/src/vfs.c`

 * *Files 1% similar despite different names*

```diff
@@ -548,15 +548,15 @@
   /* If we are inheriting from another file object, and that file
      object supports version 2 io_methods (Shm* family of functions)
      then we need to allocate an io_methods dupe of our own and fill
      in their shm methods. */
   if(Py_TYPE(pyresult)==&APSWVFSFileType)
     {
       APSWVFSFile *f=(APSWVFSFile*)pyresult;
-      if(!f->base || !f->base->pMethods  || !f->base->pMethods==1 || !f->base->pMethods->xShmMap)
+      if(!f->base || !f->base->pMethods  || !f->base->pMethods->xShmMap)
 	goto version1;
       apswfile->pMethods=&apsw_io_methods_v2;
     }
   else
     {
     version1:
       apswfile->pMethods=&apsw_io_methods_v1;
```

### Comparing `apsw-3.8.9-r1/src/vtable.c` & `apsw-3.9.2-r1/src/vtable.c`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/tests.py` & `apsw-3.9.2-r1/tests.py`

 * *Files identical despite different names*

```diff
@@ -80,14 +80,17 @@
 try:
     import ctypes
     import _ctypes
 except:
     ctypes=None
     _ctypes=None
 
+# yay
+is64bit=ctypes and ctypes.sizeof(ctypes.c_size_t)>=8
+
 # Unicode string/bytes prefix
 if py3:
     UPREFIX=""
     BPREFIX="b"
 else:
     UPREFIX="u"
     BPREFIX=""
@@ -286,15 +289,15 @@
 
 # main test class/code
 class APSW(unittest.TestCase):
 
     connection_nargs={ # number of args for function.  those not listed take zero
         'createaggregatefunction': 2,
         'createcollation': 2,
-        'createscalarfunction': 2,
+        'createscalarfunction': 3,
         'collationneeded': 1,
         'setauthorizer': 1,
         'setbusyhandler': 1,
         'setbusytimeout': 1,
         'setcommithook': 1,
         'setprofile': 1,
         'setrollbackhook': 1,
@@ -1173,14 +1176,34 @@
         # register same named function taking different number of arguments
         for i in range(-1, 4):
             self.db.createscalarfunction("multi", lambda *args: len(args), i)
         gc.collect()
         for row in c.execute("select multi(), multi(1), multi(1,2), multi(1,2,3), multi(1,2,3,4), multi(1,2,3,4,5)"):
             self.assertEqual(row, (0, 1, 2, 3, 4, 5))
 
+        # deterministic flag
+
+        # check error handling
+        self.assertRaises(TypeError, self.db.createscalarfunction, "twelve", deterministic="324")
+        self.assertRaises(TypeError, self.db.createscalarfunction, "twelve", deterministic=324)
+
+        # check it has an effect
+        class Counter:  # on calling returns how many times this instance has been called
+            num_calls=0
+            def __call__(self):
+                self.num_calls+=1
+                return self.num_calls
+        self.db.createscalarfunction("deterministic", Counter(), deterministic=True)
+        self.db.createscalarfunction("nondeterministic", Counter(), deterministic=False)
+        self.db.createscalarfunction("unspecdeterministic", Counter())
+
+        self.assertEqual(c.execute("select deterministic()=deterministic()").fetchall()[0][0], 1)
+        self.assertEqual(c.execute("select nondeterministic()=nondeterministic()").fetchall()[0][0], 0)
+        self.assertEqual(c.execute("select unspecdeterministic()=unspecdeterministic()").fetchall()[0][0], 0)
+
 
     def testAggregateFunctions(self):
         "Verify aggregate functions"
         c=self.db.cursor()
         c.execute("create table foo(x,y,z)")
         # aggregate function
         class longest:
@@ -2863,15 +2886,15 @@
         db=apsw.Connection(":memory:")
         cur=db.cursor()
         db.close()
         cur.close()
 
     def testLargeObjects(self):
         "Verify handling of large strings/blobs (>2GB) [Python 2.5+, 64 bit platform]"
-        if not ctypes or ctypes.sizeof(ctypes.c_size_t)<8:
+        if not is64bit:
             return
         # For binary/blobs I use an anonymous area slightly larger than 2GB chunk of memory, but don't touch any of it
         import mmap
         f=mmap.mmap(-1, 2*1024*1024*1024+25000)
         c=self.db.cursor()
         c.execute("create table foo(theblob)")
         self.assertRaises(apsw.TooBigError,  c.execute, "insert into foo values(?)", (f,))
@@ -3430,15 +3453,15 @@
            # examining sqlite3.c).  If they acquire non-database
            # mutexes then that is ok.
 
            # In the case of sqlite3_result_*|declare_vtab, the mutex
            # is already held by enclosing sqlite3_step and the
            # methods will only be called from that same thread so it
            # isn't a problem.
-                        'skipcalls': re.compile("^sqlite3_(blob_bytes|column_count|bind_parameter_count|data_count|vfs_.+|changes|total_changes|get_autocommit|last_insert_rowid|complete|interrupt|limit|free|threadsafe|value_.+|libversion|enable_shared_cache|initialize|shutdown|config|memory_.+|soft_heap_limit(64)?|randomness|db_readonly|db_filename|release_memory|status|result_.+|user_data|mprintf|aggregate_context|declare_vtab|backup_remaining|backup_pagecount|sourceid|uri_.+)$"),
+                        'skipcalls': re.compile("^sqlite3_(blob_bytes|column_count|bind_parameter_count|data_count|vfs_.+|changes|total_changes|get_autocommit|last_insert_rowid|complete|interrupt|limit|free|threadsafe|value_.+|libversion|enable_shared_cache|initialize|shutdown|config|memory_.+|soft_heap_limit(64)?|randomness|db_readonly|db_filename|release_memory|status64|result_.+|user_data|mprintf|aggregate_context|declare_vtab|backup_remaining|backup_pagecount|sourceid|uri_.+)$"),
                         # also ignore this file
                         'skipfiles': re.compile(r"[/\\]apsw.c$"),
                         # error message
                         'desc': "sqlite3_ calls must wrap with PYSQLITE_CALL",
                         },
         'inuse':        {
                         'match': re.compile(r"(convert_column_to_pyobject|statementcache_prepare|statementcache_finalize|statementcache_next)\s*\("),
@@ -3666,15 +3689,15 @@
             self.assertRaises(TypeError, apsw.config, apsw.SQLITE_CONFIG_SINGLETHREAD, 2)
             self.assertRaises(TypeError, apsw.config, apsw.SQLITE_CONFIG_MEMSTATUS)
             apsw.config(apsw.SQLITE_CONFIG_MEMSTATUS, True)
             apsw.config(apsw.SQLITE_CONFIG_MEMSTATUS, False)
             self.assertRaises(TypeError, apsw.config, 89748937)
             x=long(0x7fffffff)
             self.assertRaises(OverflowError, apsw.config, x*x*x*x)
-            self.assert_(apsw.config(apsw.SQLITE_CONFIG_PCACHE_HDRSZ)>=0);
+            self.assertTrue(apsw.config(apsw.SQLITE_CONFIG_PCACHE_HDRSZ)>=0);
             apsw.config(apsw.SQLITE_CONFIG_PMASZ, -1)
         finally:
             # put back to normal
             apsw.config(apsw.SQLITE_CONFIG_SERIALIZED)
             apsw.config(apsw.SQLITE_CONFIG_MEMSTATUS, True)
             apsw.initialize()
 
@@ -5023,15 +5046,15 @@
             self.assertTrue(vfs2.xGetSystemCall("open")>0)
 
             ## xSetSystemCall
             fallback=apsw.VFS("fallback",  base="") # undo any damage we do
             try:
                 self.assertRaises(TypeError,  vfs.xSetSystemCall)
                 self.assertRaises(TypeError,  vfs.xSetSystemCall, 3, 4)
-                self.assertRaises(TypeError,  vfs.xSetSystemCall, "a\0b", 4)
+                self.assertRaises((TypeError, ValueError),  vfs.xSetSystemCall, "a\0b", 4)
                 self.assertRaises(TypeError,  vfs.xSetSystemCall, "none", 3.7)
                 realopen=vfs.xGetSystemCall("open")
                 self.assertEqual(False, vfs.xSetSystemCall("doesn't exist", 0))
                 self.assertEqual(True, vfs.xSetSystemCall("open", realopen+1))
                 self.assertEqual(realopen+1, vfs.xGetSystemCall("open"))
                 self.assertEqual(True, vfs.xSetSystemCall("open", realopen))
                 TestVFS.xSetSystemCall=TestVFS.xSetSystemCall1
```

### Comparing `apsw-3.8.9-r1/tools/apswtrace.py` & `apsw-3.9.2-r1/tools/apswtrace.py`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/tools/shell.py` & `apsw-3.9.2-r1/tools/shell.py`

 * *Files identical despite different names*

### Comparing `apsw-3.8.9-r1/tools/speedtest.py` & `apsw-3.9.2-r1/tools/speedtest.py`

 * *Files identical despite different names*

