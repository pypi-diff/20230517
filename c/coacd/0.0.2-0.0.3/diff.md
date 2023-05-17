# Comparing `tmp/coacd-0.0.2-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/coacd-0.0.3-py3-none-win_amd64.whl.zip`

## zipinfo -v {}

 * *Differences in extra fields detected; using output from zipinfo -v*

```diff
@@ -1,249 +1,455 @@
 There is no zipfile comment.
 
 End-of-central-directory record:
 -------------------------------
 
-  Zip archive file size:                   1919454 (00000000001D49DEh)
-  Actual end-cent-dir record offset:       1919432 (00000000001D49C8h)
-  Expected end-cent-dir record offset:     1919432 (00000000001D49C8h)
+  Zip archive file size:                   5714247 (0000000000573147h)
+  Actual end-cent-dir record offset:       5714225 (0000000000573131h)
+  Expected end-cent-dir record offset:     5714225 (0000000000573131h)
   (based on the length of the central directory and its expected offset)
 
   This zipfile constitutes the sole disk of a single-part archive; its
-  central directory contains 8 entries.
-  The central directory is 622 (000000000000026Eh) bytes long,
+  central directory contains 12 entries.
+  The central directory is 1125 (0000000000000465h) bytes long,
   and its (expected) offset in bytes from the beginning of the zipfile
-  is 1918810 (00000000001D475Ah).
+  is 5713100 (0000000000572CCCh).
 
 
 Central directory entry #1:
 ---------------------------
 
-  coacd.cpython-39-x86_64-linux-gnu.so
+  coacd/
 
   offset of local header from start of archive:   0
                                                   (0000000000000000h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 22 19:29:24
-  32-bit CRC value (hex):                         e1cc2037
-  compressed size:                                1801595 bytes
-  uncompressed size:                              9444672 bytes
-  length of filename:                             36 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 May 16 21:05:26
+  file last modified on (UT extra field modtime): 2023 May 17 04:05:25 local
+  file last modified on (UT extra field modtime): 2023 May 17 04:05:25 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             6 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100755 octal):            -rwxr-xr-x
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #2:
 ---------------------------
 
-  coacd-0.0.2.dist-info/top_level.txt
+  coacd/lib_coacd.dll
 
-  offset of local header from start of archive:   1801661
-                                                  (00000000001B7DBDh) bytes
+  offset of local header from start of archive:   64
+                                                  (0000000000000040h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 22 19:29:24
-  32-bit CRC value (hex):                         0c8f9e69
-  compressed size:                                8 bytes
-  uncompressed size:                              6 bytes
-  length of filename:                             35 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 May 16 21:05:26
+  file last modified on (UT extra field modtime): 2023 May 17 04:05:25 local
+  file last modified on (UT extra field modtime): 2023 May 17 04:05:25 UTC
+  32-bit CRC value (hex):                         31093819
+  compressed size:                                5708094 bytes
+  uncompressed size:                              25298178 bytes
+  length of filename:                             19 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100644 octal):            -rw-r--r--
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
 
 Central directory entry #3:
 ---------------------------
 
-  coacd-0.0.2.dist-info/LICENSE
+  coacd/__init__.py
 
-  offset of local header from start of archive:   1801734
-                                                  (00000000001B7E06h) bytes
+  offset of local header from start of archive:   5708235
+                                                  (00000000005719CBh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 22 19:29:24
-  32-bit CRC value (hex):                         59bd864a
-  compressed size:                                635 bytes
-  uncompressed size:                              1080 bytes
-  length of filename:                             29 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 May 16 16:28:14
+  file last modified on (UT extra field modtime): 2023 May 16 23:28:14 local
+  file last modified on (UT extra field modtime): 2023 May 16 23:28:14 UTC
+  32-bit CRC value (hex):                         070a9f8e
+  compressed size:                                1168 bytes
+  uncompressed size:                              3831 bytes
+  length of filename:                             17 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100664 octal):            -rw-rw-r--
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
 
 Central directory entry #4:
 ---------------------------
 
-  coacd-0.0.2.dist-info/WHEEL
+  coacd-0.0.3.data/
 
-  offset of local header from start of archive:   1802428
-                                                  (00000000001B80BCh) bytes
+  offset of local header from start of archive:   5709478
+                                                  (0000000000571EA6h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
-  minimum software version required to extract:   2.0
-  compression method:                             deflated
-  compression sub-type (deflation):               normal
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 22 19:29:24
-  32-bit CRC value (hex):                         ef978a29
-  compressed size:                                107 bytes
-  uncompressed size:                              111 bytes
-  length of filename:                             27 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 May 16 20:53:00
+  file last modified on (UT extra field modtime): 2023 May 17 03:53:00 local
+  file last modified on (UT extra field modtime): 2023 May 17 03:53:00 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             17 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
   apparent file type:                             binary
-  Unix file attributes (100644 octal):            -rw-r--r--
-  MS-DOS file attributes (00 hex):                none
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
 
   There is no file comment.
 
 Central directory entry #5:
 ---------------------------
 
-  coacd-0.0.2.dist-info/METADATA
+  coacd-0.0.3.data/scripts/
 
-  offset of local header from start of archive:   1802592
-                                                  (00000000001B8160h) bytes
+  offset of local header from start of archive:   5709553
+                                                  (0000000000571EF1h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 16 20:53:00
+  file last modified on (UT extra field modtime): 2023 May 17 03:53:00 local
+  file last modified on (UT extra field modtime): 2023 May 17 03:53:00 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             25 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #6:
+---------------------------
+
+  coacd-0.0.3.data/scripts/coacd
+
+  offset of local header from start of archive:   5709636
+                                                  (0000000000571F44h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 22 19:29:24
-  32-bit CRC value (hex):                         e5ea768c
-  compressed size:                                463 bytes
-  uncompressed size:                              1123 bytes
+  file last modified on (DOS date/time):          2023 May 16 20:52:58
+  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 local
+  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 UTC
+  32-bit CRC value (hex):                         d4b77592
+  compressed size:                                1229 bytes
+  uncompressed size:                              3730 bytes
   length of filename:                             30 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100644 octal):            -rw-r--r--
+  apparent file type:                             text
+  Unix file attributes (100755 octal):            -rwxr-xr-x
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
 
-Central directory entry #6:
+Central directory entry #7:
+---------------------------
+
+  coacd-0.0.3.dist-info/
+
+  offset of local header from start of archive:   5710953
+                                                  (0000000000572469h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 16 21:24:08
+  file last modified on (UT extra field modtime): 2023 May 17 04:24:08 local
+  file last modified on (UT extra field modtime): 2023 May 17 04:24:08 UTC
+  32-bit CRC value (hex):                         00000000
+  compressed size:                                0 bytes
+  uncompressed size:                              0 bytes
+  length of filename:                             22 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             binary
+  Unix file attributes (040755 octal):            drwxr-xr-x
+  MS-DOS file attributes (10 hex):                dir 
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #8:
 ---------------------------
 
-  coacd-0.0.2.dist-info/RECORD
+  coacd-0.0.3.dist-info/RECORD
 
-  offset of local header from start of archive:   1803115
-                                                  (00000000001B836Bh) bytes
+  offset of local header from start of archive:   5711033
+                                                  (00000000005724B9h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 22 19:29:24
-  32-bit CRC value (hex):                         20324551
-  compressed size:                                442 bytes
-  uncompressed size:                              666 bytes
+  file last modified on (DOS date/time):          2023 May 16 21:12:50
+  file last modified on (UT extra field modtime): 2023 May 17 04:12:49 local
+  file last modified on (UT extra field modtime): 2023 May 17 04:12:49 UTC
+  32-bit CRC value (hex):                         d7a53d48
+  compressed size:                                414 bytes
+  uncompressed size:                              625 bytes
   length of filename:                             28 characters
-  length of extra field:                          0 bytes
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
+  apparent file type:                             text
   Unix file attributes (100664 octal):            -rw-rw-r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
 
-Central directory entry #7:
+Central directory entry #9:
 ---------------------------
 
-  coacd.libs/libz-574c8a6a.so.1.2.7
+  coacd-0.0.3.dist-info/METADATA
 
-  offset of local header from start of archive:   1803615
-                                                  (00000000001B855Fh) bytes
+  offset of local header from start of archive:   5711533
+                                                  (00000000005726ADh) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 22 19:29:24
-  32-bit CRC value (hex):                         227bc46a
-  compressed size:                                48630 bytes
-  uncompressed size:                              96272 bytes
-  length of filename:                             33 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 May 16 20:52:58
+  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 local
+  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 UTC
+  32-bit CRC value (hex):                         cc1de6e3
+  compressed size:                                475 bytes
+  uncompressed size:                              1195 bytes
+  length of filename:                             30 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100755 octal):            -rwxr-xr-x
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
 
-Central directory entry #8:
+Central directory entry #10:
 ---------------------------
 
-  coacd.libs/libgomp-a34b3233.so.1.0.0
+  coacd-0.0.3.dist-info/top_level.txt
 
-  offset of local header from start of archive:   1852308
-                                                  (00000000001C4394h) bytes
+  offset of local header from start of archive:   5712096
+                                                  (00000000005728E0h) bytes
   file system or operating system of origin:      Unix
-  version of encoding software:                   2.0
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 16 20:52:58
+  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 local
+  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 UTC
+  32-bit CRC value (hex):                         0c8f9e69
+  compressed size:                                6 bytes
+  uncompressed size:                              6 bytes
+  length of filename:                             35 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #11:
+---------------------------
+
+  coacd-0.0.3.dist-info/WHEEL
+
+  offset of local header from start of archive:   5712195
+                                                  (0000000000572943h) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
+  minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
+  minimum software version required to extract:   1.0
+  compression method:                             none (stored)
+  file security status:                           not encrypted
+  extended local header:                          no
+  file last modified on (DOS date/time):          2023 May 16 21:24:08
+  file last modified on (UT extra field modtime): 2023 May 17 04:24:08 local
+  file last modified on (UT extra field modtime): 2023 May 17 04:24:08 UTC
+  32-bit CRC value (hex):                         f70794a1
+  compressed size:                                98 bytes
+  uncompressed size:                              98 bytes
+  length of filename:                             27 characters
+  length of extra field:                          24 bytes
+  length of file comment:                         0 characters
+  disk number on which file begins:               disk 1
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
+  MS-DOS file attributes (00 hex):                none
+
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
+  There is no file comment.
+
+Central directory entry #12:
+---------------------------
+
+  coacd-0.0.3.dist-info/LICENSE
+
+  offset of local header from start of archive:   5712378
+                                                  (00000000005729FAh) bytes
+  file system or operating system of origin:      Unix
+  version of encoding software:                   3.0
   minimum file system compatibility required:     MS-DOS, OS/2 or NT FAT
   minimum software version required to extract:   2.0
   compression method:                             deflated
   compression sub-type (deflation):               normal
   file security status:                           not encrypted
   extended local header:                          no
-  file last modified on (DOS date/time):          2023 Mar 22 19:29:24
-  32-bit CRC value (hex):                         ff2cf05d
-  compressed size:                                66436 bytes
-  uncompressed size:                              168192 bytes
-  length of filename:                             36 characters
-  length of extra field:                          0 bytes
+  file last modified on (DOS date/time):          2023 May 16 20:52:58
+  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 local
+  file last modified on (UT extra field modtime): 2023 May 17 03:52:58 UTC
+  32-bit CRC value (hex):                         59bd864a
+  compressed size:                                635 bytes
+  uncompressed size:                              1080 bytes
+  length of filename:                             29 characters
+  length of extra field:                          24 bytes
   length of file comment:                         0 characters
   disk number on which file begins:               disk 1
-  apparent file type:                             binary
-  Unix file attributes (100755 octal):            -rwxr-xr-x
+  apparent file type:                             text
+  Unix file attributes (100644 octal):            -rw-r--r--
   MS-DOS file attributes (00 hex):                none
 
+  The central-directory extra field contains:
+  - A subfield with ID 0x5455 (universal time) and 5 data bytes.
+    The local extra field has UTC/GMT modification/access times.
+  - A subfield with ID 0x7875 (Unix UID/GID (any size)) and 11 data bytes:
+    01 04 e8 03 00 00 04 e8 03 00 00.
+
   There is no file comment.
```

## zipnote {}

```diff
@@ -1,25 +1,37 @@
-Filename: coacd.cpython-39-x86_64-linux-gnu.so
+Filename: coacd/
 Comment: 
 
-Filename: coacd-0.0.2.dist-info/top_level.txt
+Filename: coacd/lib_coacd.dll
 Comment: 
 
-Filename: coacd-0.0.2.dist-info/LICENSE
+Filename: coacd/__init__.py
 Comment: 
 
-Filename: coacd-0.0.2.dist-info/WHEEL
+Filename: coacd-0.0.3.data/
 Comment: 
 
-Filename: coacd-0.0.2.dist-info/METADATA
+Filename: coacd-0.0.3.data/scripts/
 Comment: 
 
-Filename: coacd-0.0.2.dist-info/RECORD
+Filename: coacd-0.0.3.data/scripts/coacd
 Comment: 
 
-Filename: coacd.libs/libz-574c8a6a.so.1.2.7
+Filename: coacd-0.0.3.dist-info/
 Comment: 
 
-Filename: coacd.libs/libgomp-a34b3233.so.1.0.0
+Filename: coacd-0.0.3.dist-info/RECORD
+Comment: 
+
+Filename: coacd-0.0.3.dist-info/METADATA
+Comment: 
+
+Filename: coacd-0.0.3.dist-info/top_level.txt
+Comment: 
+
+Filename: coacd-0.0.3.dist-info/WHEEL
+Comment: 
+
+Filename: coacd-0.0.3.dist-info/LICENSE
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v1.0 to extract, compression method=store
```

## Comparing `coacd-0.0.2.dist-info/LICENSE` & `coacd-0.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `coacd-0.0.2.dist-info/METADATA` & `coacd-0.0.3.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coacd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Approximate Convex Decomposition for 3D Meshes with Collision-Aware Concavity and Tree Search
 Home-page: https://colin97.github.io/CoACD/
 Author-email: xiwei@ucsd.edu
 License: MIT
 Keywords: collision convex decomposition
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
@@ -16,13 +16,15 @@
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 License-File: LICENSE
+Requires-Dist: numpy
```

