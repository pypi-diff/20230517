# Comparing `tmp/Photini-2023.4.0.2.tar.gz` & `tmp/Photini-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Photini-2023.4.0.2.tar", last modified: Fri Apr 14 12:55:13 2023, max compression
+gzip compressed data, was "dist/Photini-2023.5.0.tar", last modified: Wed May 17 06:58:31 2023, max compression
```

## Comparing `Photini-2023.4.0.2.tar` & `Photini-2023.5.0.tar`

### file list

```diff
@@ -1,337 +1,77 @@
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/
--rw-r--r--   0 jim       (1026) users      (100)    15393 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/CHANGELOG.txt
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/LICENSE.txt
--rw-r--r--   0 jim       (1026) users      (100)      170 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/MANIFEST.in
--rw-r--r--   0 jim       (1026) users      (100)     8928 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/PKG-INFO
--rw-r--r--   0 jim       (1026) users      (100)     7814 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/README.rst
--rw-r--r--   0 jim       (1026) users      (100)       38 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/setup.cfg
--rw-r--r--   0 jim       (1026) users      (100)     4362 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/setup.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/Photini.egg-info/
--rw-r--r--   0 jim       (1026) users      (100)     8928 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/Photini.egg-info/PKG-INFO
--rw-r--r--   0 jim       (1026) users      (100)     9110 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/Photini.egg-info/SOURCES.txt
--rw-r--r--   0 jim       (1026) users      (100)        1 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/Photini.egg-info/dependency_links.txt
--rw-r--r--   0 jim       (1026) users      (100)      162 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/Photini.egg-info/entry_points.txt
--rw-r--r--   0 jim       (1026) users      (100)        1 2023-04-12 08:05:36.000000 Photini-2023.4.0.2/src/Photini.egg-info/not-zip-safe
--rw-r--r--   0 jim       (1026) users      (100)     1044 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/Photini.egg-info/requires.txt
--rw-r--r--   0 jim       (1026) users      (100)        8 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/Photini.egg-info/top_level.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/doc/
--rw-r--r--   0 jim       (1026) users      (100)    22962 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/DOC_LICENSE.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/doc/_static/
--rw-r--r--   0 jim       (1026) users      (100)      362 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/_static/theme_overrides.css
--rw-r--r--   0 jim       (1026) users      (100)     9019 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/conf.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/doc/images/
--rw-r--r--   0 jim       (1026) users      (100)    28931 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/photini_logo.png
--rw-r--r--   0 jim       (1026) users      (100)    15962 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_001.png
--rw-r--r--   0 jim       (1026) users      (100)    66348 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_002.png
--rw-r--r--   0 jim       (1026) users      (100)    65845 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_003.png
--rw-r--r--   0 jim       (1026) users      (100)    64733 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_004.png
--rw-r--r--   0 jim       (1026) users      (100)    65131 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_005.png
--rw-r--r--   0 jim       (1026) users      (100)    64148 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_006.png
--rw-r--r--   0 jim       (1026) users      (100)    67023 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_007.png
--rw-r--r--   0 jim       (1026) users      (100)    48212 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_008.png
--rw-r--r--   0 jim       (1026) users      (100)    71994 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_009.png
--rw-r--r--   0 jim       (1026) users      (100)    70012 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_020.png
--rw-r--r--   0 jim       (1026) users      (100)    69525 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_021.png
--rw-r--r--   0 jim       (1026) users      (100)    73576 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_022.png
--rw-r--r--   0 jim       (1026) users      (100)    65341 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_023.png
--rw-r--r--   0 jim       (1026) users      (100)    68287 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_024.png
--rw-r--r--   0 jim       (1026) users      (100)    65622 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_025.png
--rw-r--r--   0 jim       (1026) users      (100)    67340 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_026.png
--rw-r--r--   0 jim       (1026) users      (100)    72586 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_027.png
--rw-r--r--   0 jim       (1026) users      (100)    67154 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_028.png
--rw-r--r--   0 jim       (1026) users      (100)    73216 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_029.png
--rw-r--r--   0 jim       (1026) users      (100)    77326 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_030.png
--rw-r--r--   0 jim       (1026) users      (100)    76697 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_031.png
--rw-r--r--   0 jim       (1026) users      (100)    68783 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_032.png
--rw-r--r--   0 jim       (1026) users      (100)    70474 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_033.png
--rw-r--r--   0 jim       (1026) users      (100)    70537 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_034.png
--rw-r--r--   0 jim       (1026) users      (100)    77800 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_100.png
--rw-r--r--   0 jim       (1026) users      (100)    79011 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_101.png
--rw-r--r--   0 jim       (1026) users      (100)    79185 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_102.png
--rw-r--r--   0 jim       (1026) users      (100)    78789 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_103.png
--rw-r--r--   0 jim       (1026) users      (100)    62313 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_104.png
--rw-r--r--   0 jim       (1026) users      (100)    65935 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_105.png
--rw-r--r--   0 jim       (1026) users      (100)    67648 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_106.png
--rw-r--r--   0 jim       (1026) users      (100)    64890 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_107.png
--rw-r--r--   0 jim       (1026) users      (100)    42875 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_108.png
--rw-r--r--   0 jim       (1026) users      (100)    44739 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_109.png
--rw-r--r--   0 jim       (1026) users      (100)    44484 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_110.png
--rw-r--r--   0 jim       (1026) users      (100)    44818 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_111.png
--rw-r--r--   0 jim       (1026) users      (100)    46451 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_112.png
--rw-r--r--   0 jim       (1026) users      (100)    45716 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_113.png
--rw-r--r--   0 jim       (1026) users      (100)    43760 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_114.png
--rw-r--r--   0 jim       (1026) users      (100)    45329 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_115.png
--rw-r--r--   0 jim       (1026) users      (100)    47052 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_116.png
--rw-r--r--   0 jim       (1026) users      (100)    45324 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_117.png
--rw-r--r--   0 jim       (1026) users      (100)    98669 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_130.png
--rw-r--r--   0 jim       (1026) users      (100)    98212 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_131.png
--rw-r--r--   0 jim       (1026) users      (100)   100910 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_132.png
--rw-r--r--   0 jim       (1026) users      (100)    89696 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_133.png
--rw-r--r--   0 jim       (1026) users      (100)    80113 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_134.png
--rw-r--r--   0 jim       (1026) users      (100)    81620 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_135.png
--rw-r--r--   0 jim       (1026) users      (100)    79965 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_136.png
--rw-r--r--   0 jim       (1026) users      (100)    78982 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_137.png
--rw-r--r--   0 jim       (1026) users      (100)    89190 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_138.png
--rw-r--r--   0 jim       (1026) users      (100)    98494 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_139.png
--rw-r--r--   0 jim       (1026) users      (100)    58825 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_141.png
--rw-r--r--   0 jim       (1026) users      (100)    65771 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_142.png
--rw-r--r--   0 jim       (1026) users      (100)    61383 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_143.png
--rw-r--r--   0 jim       (1026) users      (100)    74612 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_144.png
--rw-r--r--   0 jim       (1026) users      (100)    72082 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_145.png
--rw-r--r--   0 jim       (1026) users      (100)    72823 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_146.png
--rw-r--r--   0 jim       (1026) users      (100)    60251 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_150.png
--rw-r--r--   0 jim       (1026) users      (100)    45446 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_151a.png
--rw-r--r--   0 jim       (1026) users      (100)    13244 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_151d.png
--rw-r--r--   0 jim       (1026) users      (100)    72503 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_152.png
--rw-r--r--   0 jim       (1026) users      (100)    65762 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_154.png
--rw-r--r--   0 jim       (1026) users      (100)    72249 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_155.png
--rw-r--r--   0 jim       (1026) users      (100)    80606 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_156.png
--rw-r--r--   0 jim       (1026) users      (100)    81976 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_157.png
--rw-r--r--   0 jim       (1026) users      (100)    72070 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_158.png
--rw-r--r--   0 jim       (1026) users      (100)    84127 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_159.png
--rw-r--r--   0 jim       (1026) users      (100)    54712 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_160.png
--rw-r--r--   0 jim       (1026) users      (100)    76525 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_161.png
--rw-r--r--   0 jim       (1026) users      (100)    54226 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_170.png
--rw-r--r--   0 jim       (1026) users      (100)    63855 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_171.png
--rw-r--r--   0 jim       (1026) users      (100)    69774 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_172.png
--rw-r--r--   0 jim       (1026) users      (100)    70791 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_173.png
--rw-r--r--   0 jim       (1026) users      (100)    66013 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_174.png
--rw-r--r--   0 jim       (1026) users      (100)    77354 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_175.png
--rw-r--r--   0 jim       (1026) users      (100)    20588 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_180.png
--rw-r--r--   0 jim       (1026) users      (100)    35446 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_181.png
--rw-r--r--   0 jim       (1026) users      (100)    40375 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_182.png
--rw-r--r--   0 jim       (1026) users      (100)    38151 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_183.png
--rw-r--r--   0 jim       (1026) users      (100)    43644 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_184.png
--rw-r--r--   0 jim       (1026) users      (100)    56298 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_185.png
--rw-r--r--   0 jim       (1026) users      (100)    69510 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_200.png
--rw-r--r--   0 jim       (1026) users      (100)    31477 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_201.png
--rw-r--r--   0 jim       (1026) users      (100)    39167 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_202.png
--rw-r--r--   0 jim       (1026) users      (100)    52117 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_203.png
--rw-r--r--   0 jim       (1026) users      (100)    76102 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_204.png
--rw-r--r--   0 jim       (1026) users      (100)   106593 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_220.png
--rw-r--r--   0 jim       (1026) users      (100)   115906 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_221.png
--rw-r--r--   0 jim       (1026) users      (100)   114123 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_222.png
--rw-r--r--   0 jim       (1026) users      (100)    86341 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_223.png
--rw-r--r--   0 jim       (1026) users      (100)    84648 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_224.png
--rw-r--r--   0 jim       (1026) users      (100)    87434 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_225.png
--rw-r--r--   0 jim       (1026) users      (100)    59154 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_230.png
--rw-r--r--   0 jim       (1026) users      (100)    66436 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_231.png
--rw-r--r--   0 jim       (1026) users      (100)    48689 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_232.png
--rw-r--r--   0 jim       (1026) users      (100)    41507 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_233.png
--rw-r--r--   0 jim       (1026) users      (100)    64402 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_234.png
--rw-r--r--   0 jim       (1026) users      (100)    61030 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_235.png
--rw-r--r--   0 jim       (1026) users      (100)    64905 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_236.png
--rw-r--r--   0 jim       (1026) users      (100)    73976 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_237.png
--rw-r--r--   0 jim       (1026) users      (100)    76099 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_238.png
--rw-r--r--   0 jim       (1026) users      (100)    76183 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_239.png
--rw-r--r--   0 jim       (1026) users      (100)    75744 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_240.png
--rw-r--r--   0 jim       (1026) users      (100)    83965 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_242.png
--rw-r--r--   0 jim       (1026) users      (100)    72956 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_250.png
--rw-r--r--   0 jim       (1026) users      (100)    76602 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_251.png
--rw-r--r--   0 jim       (1026) users      (100)    77132 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_252.png
--rw-r--r--   0 jim       (1026) users      (100)    18523 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_253.png
--rw-r--r--   0 jim       (1026) users      (100)    73131 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_254.png
--rw-r--r--   0 jim       (1026) users      (100)    68348 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_255.png
--rw-r--r--   0 jim       (1026) users      (100)    72388 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_256.png
--rw-r--r--   0 jim       (1026) users      (100)    73136 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_257.png
--rw-r--r--   0 jim       (1026) users      (100)    70116 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_258.png
--rw-r--r--   0 jim       (1026) users      (100)    79413 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_259.png
--rw-r--r--   0 jim       (1026) users      (100)    80423 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_260.png
--rw-r--r--   0 jim       (1026) users      (100)    64029 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_270.png
--rw-r--r--   0 jim       (1026) users      (100)   108239 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_271.png
--rw-r--r--   0 jim       (1026) users      (100)   112504 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_272.png
--rw-r--r--   0 jim       (1026) users      (100)   109408 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_273.png
--rw-r--r--   0 jim       (1026) users      (100)   110228 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_274.png
--rw-r--r--   0 jim       (1026) users      (100)   112780 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_275.png
--rw-r--r--   0 jim       (1026) users      (100)   107839 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_276.png
--rw-r--r--   0 jim       (1026) users      (100)   115642 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_277.png
--rw-r--r--   0 jim       (1026) users      (100)   117777 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_278.png
--rw-r--r--   0 jim       (1026) users      (100)   110698 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_279.png
--rw-r--r--   0 jim       (1026) users      (100)   110108 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_280.png
--rw-r--r--   0 jim       (1026) users      (100)    73241 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_36.png
--rw-r--r--   0 jim       (1026) users      (100)    22828 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/images/screenshot_37.png
--rw-r--r--   0 jim       (1026) users      (100)     1057 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/index.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/doc/manual/
--rw-r--r--   0 jim       (1026) users      (100)     3324 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/address.rst
--rw-r--r--   0 jim       (1026) users      (100)     9850 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/configuration.rst
--rw-r--r--   0 jim       (1026) users      (100)     7134 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/descriptive_metadata.rst
--rw-r--r--   0 jim       (1026) users      (100)     2314 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/extending.rst
--rw-r--r--   0 jim       (1026) users      (100)     4778 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/flickr.rst
--rw-r--r--   0 jim       (1026) users      (100)     2592 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/google_photos.rst
--rw-r--r--   0 jim       (1026) users      (100)     4697 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/image_selector.rst
--rw-r--r--   0 jim       (1026) users      (100)     4512 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/importer.rst
--rw-r--r--   0 jim       (1026) users      (100)      731 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/index.rst
--rw-r--r--   0 jim       (1026) users      (100)     4541 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/ipernity.rst
--rw-r--r--   0 jim       (1026) users      (100)     5345 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/map.rst
--rw-r--r--   0 jim       (1026) users      (100)     5212 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/ownership_metadata.rst
--rw-r--r--   0 jim       (1026) users      (100)     4528 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/pixelfed.rst
--rw-r--r--   0 jim       (1026) users      (100)     3165 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/regions.rst
--rw-r--r--   0 jim       (1026) users      (100)    11368 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/tags.rst
--rw-r--r--   0 jim       (1026) users      (100)     8028 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/technical_metadata.rst
--rw-r--r--   0 jim       (1026) users      (100)     1354 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/manual/video.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/doc/misc/
--rw-r--r--   0 jim       (1026) users      (100)      235 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/misc/changelog.rst
--rw-r--r--   0 jim       (1026) users      (100)      352 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/misc/doc_licence.rst
--rw-r--r--   0 jim       (1026) users      (100)      248 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/misc/index.rst
--rw-r--r--   0 jim       (1026) users      (100)      337 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/misc/licence.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/doc/other/
--rw-r--r--   0 jim       (1026) users      (100)    42560 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/other/installation.rst
--rw-r--r--   0 jim       (1026) users      (100)      609 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/other/introduction.rst
--rw-r--r--   0 jim       (1026) users      (100)    12643 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/other/localisation.rst
--rw-r--r--   0 jim       (1026) users      (100)      686 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/other/reading.rst
--rw-r--r--   0 jim       (1026) users      (100)     5239 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/other/workflow.rst
--rw-r--r--   0 jim       (1026) users      (100)       70 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/doc/requirements.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/
--rw-r--r--   0 jim       (1026) users      (100)     3134 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/lang/README.rst
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/ca/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/ca/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     2595 2023-04-14 12:54:40.000000 Photini-2023.4.0.2/src/lang/ca/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75951 2023-04-14 12:54:43.000000 Photini-2023.4.0.2/src/lang/ca/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1384 2023-04-14 12:54:46.000000 Photini-2023.4.0.2/src/lang/ca/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41764 2023-04-14 12:54:49.000000 Photini-2023.4.0.2/src/lang/ca/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    96826 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/ca/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/cs/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/cs/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     2728 2023-04-14 12:54:41.000000 Photini-2023.4.0.2/src/lang/cs/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75857 2023-04-14 12:54:44.000000 Photini-2023.4.0.2/src/lang/cs/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1708 2023-04-14 12:54:46.000000 Photini-2023.4.0.2/src/lang/cs/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    49939 2023-04-14 12:54:49.000000 Photini-2023.4.0.2/src/lang/cs/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    99461 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/cs/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/de/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/de/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1773 2023-04-14 12:54:42.000000 Photini-2023.4.0.2/src/lang/de/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    76335 2023-04-14 12:54:44.000000 Photini-2023.4.0.2/src/lang/de/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1302 2023-04-14 12:54:47.000000 Photini-2023.4.0.2/src/lang/de/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    42298 2023-04-14 12:54:49.000000 Photini-2023.4.0.2/src/lang/de/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    99572 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/de/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/en/
--rw-r--r--   0 jim       (1026) users      (100)    87978 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/en/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/es/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/es/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1814 2023-04-14 12:54:42.000000 Photini-2023.4.0.2/src/lang/es/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75982 2023-04-14 12:54:45.000000 Photini-2023.4.0.2/src/lang/es/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1171 2023-04-14 12:54:47.000000 Photini-2023.4.0.2/src/lang/es/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41696 2023-04-14 12:54:50.000000 Photini-2023.4.0.2/src/lang/es/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    96008 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/es/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/fr/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/fr/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1824 2023-04-14 12:54:42.000000 Photini-2023.4.0.2/src/lang/fr/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75661 2023-04-14 12:54:45.000000 Photini-2023.4.0.2/src/lang/fr/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1182 2023-04-14 12:54:48.000000 Photini-2023.4.0.2/src/lang/fr/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41713 2023-04-14 12:54:50.000000 Photini-2023.4.0.2/src/lang/fr/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)   100291 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/fr/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/it/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/it/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1648 2023-04-14 12:54:42.000000 Photini-2023.4.0.2/src/lang/it/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75543 2023-04-14 12:54:45.000000 Photini-2023.4.0.2/src/lang/it/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1171 2023-04-14 12:54:48.000000 Photini-2023.4.0.2/src/lang/it/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41530 2023-04-14 12:54:50.000000 Photini-2023.4.0.2/src/lang/it/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    95701 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/it/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/ko/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/ko/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     2765 2023-04-14 12:54:43.000000 Photini-2023.4.0.2/src/lang/ko/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)   141558 2023-04-14 12:54:45.000000 Photini-2023.4.0.2/src/lang/ko/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1662 2023-04-14 12:54:48.000000 Photini-2023.4.0.2/src/lang/ko/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    67188 2023-04-14 12:54:51.000000 Photini-2023.4.0.2/src/lang/ko/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    95625 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/ko/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/nb/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/nb/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1781 2023-04-14 12:54:43.000000 Photini-2023.4.0.2/src/lang/nb/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75596 2023-04-14 12:54:46.000000 Photini-2023.4.0.2/src/lang/nb/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1142 2023-04-14 12:54:48.000000 Photini-2023.4.0.2/src/lang/nb/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41669 2023-04-14 12:54:51.000000 Photini-2023.4.0.2/src/lang/nb/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    95337 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/nb/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/pl/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/pl/LC_MESSAGES/
--rw-r--r--   0 jim       (1026) users      (100)     1851 2023-04-14 12:54:43.000000 Photini-2023.4.0.2/src/lang/pl/LC_MESSAGES/index.po
--rw-r--r--   0 jim       (1026) users      (100)    75727 2023-04-14 12:54:46.000000 Photini-2023.4.0.2/src/lang/pl/LC_MESSAGES/manual.po
--rw-r--r--   0 jim       (1026) users      (100)     1277 2023-04-14 12:54:49.000000 Photini-2023.4.0.2/src/lang/pl/LC_MESSAGES/misc.po
--rw-r--r--   0 jim       (1026) users      (100)    41743 2023-04-14 12:54:51.000000 Photini-2023.4.0.2/src/lang/pl/LC_MESSAGES/other.po
--rw-r--r--   0 jim       (1026) users      (100)    95997 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/pl/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/templates/
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/templates/gettext/
--rw-r--r--   0 jim       (1026) users      (100)     1508 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/lang/templates/gettext/index.pot
--rw-r--r--   0 jim       (1026) users      (100)    72700 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/lang/templates/gettext/manual.pot
--rw-r--r--   0 jim       (1026) users      (100)     1055 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/lang/templates/gettext/misc.pot
--rw-r--r--   0 jim       (1026) users      (100)    40008 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/lang/templates/gettext/other.pot
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/lang/templates/qt/
--rw-r--r--   0 jim       (1026) users      (100)    96788 2023-04-14 12:55:01.000000 Photini-2023.4.0.2/src/lang/templates/qt/photini.ts
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/photini/
--rw-r--r--   0 jim       (1026) users      (100)      116 2023-04-14 12:54:24.000000 Photini-2023.4.0.2/src/photini/__init__.py
--rw-r--r--   0 jim       (1026) users      (100)      917 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/__main__.py
--rw-r--r--   0 jim       (1026) users      (100)    19879 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/address.py
--rw-r--r--   0 jim       (1026) users      (100)     4759 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/bingmap.py
--rw-r--r--   0 jim       (1026) users      (100)     5310 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/configstore.py
--rw-r--r--   0 jim       (1026) users      (100)     6890 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/cv.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/photini/data/
--rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/LICENSE.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/photini/data/bingmap/
--rw-r--r--   0 jim       (1026) users      (100)     7556 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/bingmap/script.js
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/photini/data/googlemap/
--rw-r--r--   0 jim       (1026) users      (100)     6239 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/googlemap/script.js
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/photini/data/icons/
--rw-r--r--   0 jim       (1026) users      (100)    14554 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/icons/photini_128.png
--rw-r--r--   0 jim       (1026) users      (100)     3262 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/icons/photini_48.png
--rw-r--r--   0 jim       (1026) users      (100)    86598 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/icons/photini_win.ico
--rw-r--r--   0 jim       (1026) users      (100)     2205 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/keys.txt
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/photini/data/lang/
--rw-r--r--   0 jim       (1026) users      (100)    22137 2023-04-14 12:55:06.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.ca.qm
--rw-r--r--   0 jim       (1026) users      (100)    40194 2023-04-14 12:55:05.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.cs.qm
--rw-r--r--   0 jim       (1026) users      (100)    44214 2023-04-14 12:55:04.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.de.qm
--rw-r--r--   0 jim       (1026) users      (100)    28726 2023-04-14 12:55:05.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.en.qm
--rw-r--r--   0 jim       (1026) users      (100)    10112 2023-04-14 12:55:05.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.es.qm
--rw-r--r--   0 jim       (1026) users      (100)    41878 2023-04-14 12:55:04.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.fr.qm
--rw-r--r--   0 jim       (1026) users      (100)      923 2023-04-14 12:55:05.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.it.qm
--rw-r--r--   0 jim       (1026) users      (100)     2072 2023-04-14 12:55:06.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.ko.qm
--rw-r--r--   0 jim       (1026) users      (100)    19489 2023-04-14 12:55:06.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.nb.qm
--rw-r--r--   0 jim       (1026) users      (100)    10060 2023-04-14 12:55:06.000000 Photini-2023.4.0.2/src/photini/data/lang/photini.pl.qm
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/photini/data/linux/
--rw-r--r--   0 jim       (1026) users      (100)      991 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/linux/photini.desktop
--rw-r--r--   0 jim       (1026) users      (100)      209 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/map_circle_blue.png
--rw-r--r--   0 jim       (1026) users      (100)      207 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/map_circle_red.png
--rw-r--r--   0 jim       (1026) users      (100)     1867 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/map_pin_grey.png
--rw-r--r--   0 jim       (1026) users      (100)     2016 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/map_pin_red.png
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/photini/data/mapboxmap/
--rw-r--r--   0 jim       (1026) users      (100)     5715 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/mapboxmap/script.js
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/src/photini/data/windows/
--rw-r--r--   0 jim       (1026) users      (100)     2638 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/data/windows/install_shortcuts.vbs
--rw-r--r--   0 jim       (1026) users      (100)    13464 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/descriptive.py
--rw-r--r--   0 jim       (1026) users      (100)    22760 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/editor.py
--rw-r--r--   0 jim       (1026) users      (100)     7893 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/editsettings.py
--rw-r--r--   0 jim       (1026) users      (100)    31789 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/exiv2.py
--rw-r--r--   0 jim       (1026) users      (100)     3287 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/ffmpeg.py
--rw-r--r--   0 jim       (1026) users      (100)    33292 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/flickr.py
--rw-r--r--   0 jim       (1026) users      (100)     4191 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/googlemap.py
--rw-r--r--   0 jim       (1026) users      (100)    13099 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/googlephotos.py
--rw-r--r--   0 jim       (1026) users      (100)     4382 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/gpximporter.py
--rw-r--r--   0 jim       (1026) users      (100)    40241 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/imagelist.py
--rw-r--r--   0 jim       (1026) users      (100)    27611 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/importer.py
--rw-r--r--   0 jim       (1026) users      (100)    27252 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/ipernity.py
--rw-r--r--   0 jim       (1026) users      (100)     4396 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/loggerwindow.py
--rw-r--r--   0 jim       (1026) users      (100)     4235 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/mapboxmap.py
--rw-r--r--   0 jim       (1026) users      (100)    36681 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/metadata.py
--rw-r--r--   0 jim       (1026) users      (100)    21920 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/ownership.py
--rw-r--r--   0 jim       (1026) users      (100)    25534 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/photinimap.py
--rw-r--r--   0 jim       (1026) users      (100)    37738 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/pixelfed.py
--rw-r--r--   0 jim       (1026) users      (100)    10550 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/pyqt.py
--rw-r--r--   0 jim       (1026) users      (100)    36607 2023-04-14 12:54:24.000000 Photini-2023.4.0.2/src/photini/regions.py
--rw-r--r--   0 jim       (1026) users      (100)     6711 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/scripts.py
--rw-r--r--   0 jim       (1026) users      (100)     3687 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/spelling.py
--rw-r--r--   0 jim       (1026) users      (100)    40105 2023-04-13 09:46:40.000000 Photini-2023.4.0.2/src/photini/technical.py
--rw-r--r--   0 jim       (1026) users      (100)    71730 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/types.py
--rw-r--r--   0 jim       (1026) users      (100)    47911 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/photini/uploader.py
--rw-r--r--   0 jim       (1026) users      (100)    34838 2023-04-13 09:46:40.000000 Photini-2023.4.0.2/src/photini/widgets.py
--rw-r--r--   0 jim       (1026) users      (100)     1097 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/src/run_photini.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/utils/
--rw-r--r--   0 jim       (1026) users      (100)     1257 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/build_docs.py
--rw-r--r--   0 jim       (1026) users      (100)     1511 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/build_lang.py
--rw-r--r--   0 jim       (1026) users      (100)     2723 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/download_cvs.py
--rw-r--r--   0 jim       (1026) users      (100)     8048 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/lang_update.py
--rw-r--r--   0 jim       (1026) users      (100)     2220 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/localise_desktop.py
-drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-04-14 12:55:13.000000 Photini-2023.4.0.2/utils/make_icons/
--rw-r--r--   0 jim       (1026) users      (100)      166 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/make_icons/circle.fig
--rw-r--r--   0 jim       (1026) users      (100)   178291 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/make_icons/icon_master.png
--rw-r--r--   0 jim       (1026) users      (100)     1279 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/make_icons/makefile
--rw-r--r--   0 jim       (1026) users      (100)     1539 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/tag_release.py
--rw-r--r--   0 jim       (1026) users      (100)     2846 2023-04-12 08:03:27.000000 Photini-2023.4.0.2/utils/update_version.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/
+-rw-r--r--   0 jim       (1026) users      (100)    15642 2023-05-17 06:57:34.000000 Photini-2023.5.0/CHANGELOG.txt
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.5.0/LICENSE.txt
+-rw-r--r--   0 jim       (1026) users      (100)      267 2023-05-17 06:57:34.000000 Photini-2023.5.0/MANIFEST.in
+-rw-r--r--   0 jim       (1026) users      (100)     8924 2023-05-17 06:58:31.000000 Photini-2023.5.0/PKG-INFO
+-rw-r--r--   0 jim       (1026) users      (100)     7814 2023-04-12 08:03:27.000000 Photini-2023.5.0/README.rst
+-rw-r--r--   0 jim       (1026) users      (100)     2093 2023-05-17 06:57:34.000000 Photini-2023.5.0/pyproject.toml
+-rw-r--r--   0 jim       (1026) users      (100)       38 2023-05-17 06:58:31.000000 Photini-2023.5.0/setup.cfg
+-rw-r--r--   0 jim       (1026) users      (100)     4698 2023-05-17 06:57:34.000000 Photini-2023.5.0/setup.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/Photini.egg-info/
+-rw-r--r--   0 jim       (1026) users      (100)     1707 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/Photini.egg-info/SOURCES.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/photini/
+-rw-r--r--   0 jim       (1026) users      (100)      114 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/__init__.py
+-rw-r--r--   0 jim       (1026) users      (100)      917 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/__main__.py
+-rw-r--r--   0 jim       (1026) users      (100)    19936 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/address.py
+-rw-r--r--   0 jim       (1026) users      (100)     4759 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/bingmap.py
+-rw-r--r--   0 jim       (1026) users      (100)     5310 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/configstore.py
+-rw-r--r--   0 jim       (1026) users      (100)     6890 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/cv.py
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/photini/data/
+-rw-r--r--   0 jim       (1026) users      (100)    35147 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/LICENSE.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/photini/data/bingmap/
+-rw-r--r--   0 jim       (1026) users      (100)     7556 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/bingmap/script.js
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/photini/data/googlemap/
+-rw-r--r--   0 jim       (1026) users      (100)     6239 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/googlemap/script.js
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/photini/data/icons/
+-rw-r--r--   0 jim       (1026) users      (100)    14554 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/icons/photini_128.png
+-rw-r--r--   0 jim       (1026) users      (100)     3262 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/icons/photini_48.png
+-rw-r--r--   0 jim       (1026) users      (100)    86598 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/icons/photini_win.ico
+-rw-r--r--   0 jim       (1026) users      (100)     2205 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/keys.txt
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/photini/data/lang/
+-rw-r--r--   0 jim       (1026) users      (100)    22137 2023-05-17 06:58:23.000000 Photini-2023.5.0/src/photini/data/lang/photini.ca.qm
+-rw-r--r--   0 jim       (1026) users      (100)    40194 2023-05-17 06:58:22.000000 Photini-2023.5.0/src/photini/data/lang/photini.cs.qm
+-rw-r--r--   0 jim       (1026) users      (100)    46568 2023-05-17 06:58:21.000000 Photini-2023.5.0/src/photini/data/lang/photini.de.qm
+-rw-r--r--   0 jim       (1026) users      (100)    29131 2023-05-17 06:58:22.000000 Photini-2023.5.0/src/photini/data/lang/photini.en.qm
+-rw-r--r--   0 jim       (1026) users      (100)    10112 2023-05-17 06:58:22.000000 Photini-2023.5.0/src/photini/data/lang/photini.es.qm
+-rw-r--r--   0 jim       (1026) users      (100)    41878 2023-05-17 06:58:21.000000 Photini-2023.5.0/src/photini/data/lang/photini.fr.qm
+-rw-r--r--   0 jim       (1026) users      (100)      923 2023-05-17 06:58:22.000000 Photini-2023.5.0/src/photini/data/lang/photini.it.qm
+-rw-r--r--   0 jim       (1026) users      (100)     2072 2023-05-17 06:58:23.000000 Photini-2023.5.0/src/photini/data/lang/photini.ko.qm
+-rw-r--r--   0 jim       (1026) users      (100)    19489 2023-05-17 06:58:24.000000 Photini-2023.5.0/src/photini/data/lang/photini.nb.qm
+-rw-r--r--   0 jim       (1026) users      (100)    10060 2023-05-17 06:58:23.000000 Photini-2023.5.0/src/photini/data/lang/photini.pl.qm
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/photini/data/linux/
+-rw-r--r--   0 jim       (1026) users      (100)      991 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/linux/photini.desktop
+-rw-r--r--   0 jim       (1026) users      (100)      209 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/map_circle_blue.png
+-rw-r--r--   0 jim       (1026) users      (100)      207 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/map_circle_red.png
+-rw-r--r--   0 jim       (1026) users      (100)     1867 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/map_pin_grey.png
+-rw-r--r--   0 jim       (1026) users      (100)     2016 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/map_pin_red.png
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/photini/data/mapboxmap/
+-rw-r--r--   0 jim       (1026) users      (100)     5715 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/mapboxmap/script.js
+drwxr-xr-x   0 jim       (1026) users      (100)        0 2023-05-17 06:58:31.000000 Photini-2023.5.0/src/photini/data/windows/
+-rw-r--r--   0 jim       (1026) users      (100)     2638 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/data/windows/install_shortcuts.vbs
+-rw-r--r--   0 jim       (1026) users      (100)    13464 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/descriptive.py
+-rw-r--r--   0 jim       (1026) users      (100)    22808 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/editor.py
+-rw-r--r--   0 jim       (1026) users      (100)     8435 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/editsettings.py
+-rw-r--r--   0 jim       (1026) users      (100)    32540 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/exiv2.py
+-rw-r--r--   0 jim       (1026) users      (100)     3287 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/ffmpeg.py
+-rw-r--r--   0 jim       (1026) users      (100)    33292 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/flickr.py
+-rw-r--r--   0 jim       (1026) users      (100)     4191 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/googlemap.py
+-rw-r--r--   0 jim       (1026) users      (100)    13099 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/googlephotos.py
+-rw-r--r--   0 jim       (1026) users      (100)     4382 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/gpximporter.py
+-rw-r--r--   0 jim       (1026) users      (100)    40241 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/imagelist.py
+-rw-r--r--   0 jim       (1026) users      (100)    27611 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/importer.py
+-rw-r--r--   0 jim       (1026) users      (100)    27252 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/ipernity.py
+-rw-r--r--   0 jim       (1026) users      (100)     4396 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/loggerwindow.py
+-rw-r--r--   0 jim       (1026) users      (100)     4235 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/mapboxmap.py
+-rw-r--r--   0 jim       (1026) users      (100)    36681 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/metadata.py
+-rw-r--r--   0 jim       (1026) users      (100)    21920 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/ownership.py
+-rw-r--r--   0 jim       (1026) users      (100)    25788 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/photinimap.py
+-rw-r--r--   0 jim       (1026) users      (100)    37738 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/pixelfed.py
+-rw-r--r--   0 jim       (1026) users      (100)    10550 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/pyqt.py
+-rw-r--r--   0 jim       (1026) users      (100)    36607 2023-04-14 12:54:24.000000 Photini-2023.5.0/src/photini/regions.py
+-rw-r--r--   0 jim       (1026) users      (100)     6875 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/scripts.py
+-rw-r--r--   0 jim       (1026) users      (100)     3687 2023-04-12 08:03:27.000000 Photini-2023.5.0/src/photini/spelling.py
+-rw-r--r--   0 jim       (1026) users      (100)    40998 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/technical.py
+-rw-r--r--   0 jim       (1026) users      (100)    72468 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/types.py
+-rw-r--r--   0 jim       (1026) users      (100)    47789 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/uploader.py
+-rw-r--r--   0 jim       (1026) users      (100)    35542 2023-05-17 06:57:34.000000 Photini-2023.5.0/src/photini/widgets.py
```

### Comparing `Photini-2023.4.0.2/CHANGELOG.txt` & `Photini-2023.5.0/CHANGELOG.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,20 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see
 <http://www.gnu.org/licenses/>.
 
+Changes in v2023.5.0:
+  1/ Latitude & longitude values no longer have comma separator.
+  2/ All numeric values are localised, e.g. to use decimal comma.
+  3/ Can ignore altitude when importing GPX data.
+  4/ Other minor improvements and bug fixes.
+
 Changes in v2023.4.0:
   1/ Add "image regions" tab.
   2/ Connect image regions to Flickr / Ipernity "notes".
   3/ Add GPS coordinates to location / address data.
   4/ Improved XMP metadata handling.
   5/ Other minor improvements and bug fixes.
```

### Comparing `Photini-2023.4.0.2/LICENSE.txt` & `Photini-2023.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/PKG-INFO` & `Photini-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: Photini
-Version: 2023.4.0.2
+Version: 2023.5.0
 Summary: Simple photo metadata editor
 Home-page: https://github.com/jim-easterbrook/Photini
 Author: Jim Easterbrook
 Author-email: jim@jim-easterbrook.me.uk
 License: GPLv3+
-Download-URL: https://github.com/jim-easterbrook/Photini/archive/2023.4.0.2.tar.gz
+Download-URL: https://github.com/jim-easterbrook/Photini/archive/2023.5.0.tar.gz
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `Photini-2023.4.0.2/README.rst` & `Photini-2023.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/setup.py` & `Photini-2023.5.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with this program.  If not, see
 #  <http://www.gnu.org/licenses/>.
 
 import os
 from setuptools import setup
+from setuptools import __version__ as setuptools_version
 
 
 # list dependency packages
 install_requires = ['appdirs', 'cachetools', 'chardet', 'exiv2', 'requests']
 extras_require = {
     'basic'    : ['PySide2'],
     'flickr'   : ['requests-oauthlib', 'requests-toolbelt', 'keyring'],
@@ -56,55 +57,59 @@
     package, sep, marker = package.partition(';')
     return '{} >= {}'.format(package, min_version[package]) + sep + marker
 
 for option in extras_require:
     extras_require[option] = [add_version(x) for x in extras_require[option]]
 install_requires = [add_version(x) for x in install_requires]
 
-# read current version info without importing package
-with open('src/photini/__init__.py') as f:
-    exec(f.read())
-
-with open('README.rst') as ldf:
-    long_description = ldf.read()
-url = 'https://github.com/jim-easterbrook/Photini'
-
 package_data = []
 for root, dirs, files in os.walk('src/photini/data/'):
     package_data += [
         os.path.join(root.replace('src/photini/', ''), x) for x in files]
+url = 'https://github.com/jim-easterbrook/Photini'
 
-setup(name = 'Photini',
-      version = __version__,
-      author = 'Jim Easterbrook',
-      author_email = 'jim@jim-easterbrook.me.uk',
-      url = url,
-      download_url = url + '/archive/' + __version__ + '.tar.gz',
-      description = 'Simple photo metadata editor',
-      long_description = long_description,
-      classifiers = [
-          'Development Status :: 5 - Production/Stable',
-          'Environment :: Win32 (MS Windows)',
-          'Environment :: X11 Applications :: Qt',
-          'Intended Audience :: End Users/Desktop',
-          'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-          'Operating System :: OS Independent',
-          'Programming Language :: Python :: 3',
-          'Topic :: Multimedia :: Graphics',
-          ],
-      license = 'GPLv3+',
-      packages = ['photini'],
-      package_dir = {'' : 'src'},
-      package_data = {'photini' : package_data},
-      entry_points = {
-          'console_scripts' : [
-              'photini-configure = photini.scripts:configure',
-              'photini-post-install = photini.scripts:post_install',
-              ],
-          'gui_scripts' : [
-              'photini = photini.editor:main',
+if tuple(map(int, setuptools_version.split('.'))) >= (61, 0):
+    # use metadata from pyproject.toml
+    setup()
+else:
+    # read current version info without importing package
+    with open('src/photini/__init__.py') as f:
+        exec(f.read())
+
+    with open('README.rst') as ldf:
+        long_description = ldf.read()
+
+    setup(name = 'Photini',
+          version = __version__,
+          author = 'Jim Easterbrook',
+          author_email = 'jim@jim-easterbrook.me.uk',
+          url = url,
+          download_url = url + '/archive/' + __version__ + '.tar.gz',
+          description = 'Simple photo metadata editor',
+          long_description = long_description,
+          classifiers = [
+              'Development Status :: 5 - Production/Stable',
+              'Environment :: Win32 (MS Windows)',
+              'Environment :: X11 Applications :: Qt',
+              'Intended Audience :: End Users/Desktop',
+              'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
+              'Operating System :: OS Independent',
+              'Programming Language :: Python :: 3',
+              'Topic :: Multimedia :: Graphics',
               ],
-          },
-      install_requires = install_requires,
-      extras_require = extras_require,
-      zip_safe = False,
-      )
+          license = 'GPLv3+',
+          packages = ['photini'],
+          package_dir = {'' : 'src'},
+          package_data = {'photini' : package_data},
+          entry_points = {
+              'console_scripts' : [
+                  'photini-configure = photini.scripts:configure',
+                  'photini-post-install = photini.scripts:post_install',
+                  ],
+              'gui_scripts' : [
+                  'photini = photini.editor:main',
+                  ],
+              },
+          install_requires = install_requires,
+          extras_require = extras_require,
+          zip_safe = False,
+          )
```

### Comparing `Photini-2023.4.0.2/src/photini/__main__.py` & `Photini-2023.5.0/src/photini/__main__.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/address.py` & `Photini-2023.5.0/src/photini/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,16 @@
             self.members[key] = SingleLineEdit(
                 'Iptc4xmpExt:' + key, length_check=ImageMetadata.max_bytes(key))
             self.members[key].setToolTip('<p>{}</p>'.format(tool_tip))
             self.members[key].new_value.connect(self.editing_finished)
         self.members['latlon'] = LatLongDisplay()
         self.members['latlon'].new_value.connect(self.editing_finished)
         self.members['alt'] = DoubleSpinBox('exif:GPSAltitude')
-        self.members['alt'].set_suffix(' m')
+        self.members['alt'].set_suffix(
+            translate('AddressTab', ' m', 'metres altitude'))
         self.members['alt'].setToolTip('<p>{}</p>'.format(
             translate('AddressTab', 'Altitude of the location in metres.')))
         self.members['alt'].new_value.connect(self.editing_finished)
         self.members['CountryCode'].setMaximumWidth(
             width_for_text(self.members['CountryCode'], 'W' * 4))
         for j, text in enumerate((translate('AddressTab', 'Name'),
                                   translate('AddressTab', 'Street'),
```

### Comparing `Photini-2023.4.0.2/src/photini/bingmap.py` & `Photini-2023.5.0/src/photini/bingmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/configstore.py` & `Photini-2023.5.0/src/photini/configstore.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/cv.py` & `Photini-2023.5.0/src/photini/cv.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/LICENSE.txt` & `Photini-2023.5.0/src/photini/data/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/bingmap/script.js` & `Photini-2023.5.0/src/photini/data/bingmap/script.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/googlemap/script.js` & `Photini-2023.5.0/src/photini/data/googlemap/script.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/icons/photini_128.png` & `Photini-2023.5.0/src/photini/data/icons/photini_128.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/icons/photini_48.png` & `Photini-2023.5.0/src/photini/data/icons/photini_48.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/icons/photini_win.ico` & `Photini-2023.5.0/src/photini/data/icons/photini_win.ico`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/keys.txt` & `Photini-2023.5.0/src/photini/data/keys.txt`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.ca.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.ca.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.cs.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.cs.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.de.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.de.qm`

 * *Files 3% similar despite different names*

```diff
@@ -1,2764 +1,2911 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0264 6542 0000 0ba0 0000 5a6c  .....deB......Zl
-00000020: 0000 74ed 0000 7388 0000 8b54 0000 73fe  ..t...s....T..s.
-00000030: 0000 8b7e 0004 a0b9 0000 00e5 0004 a0b9  ...~............
-00000040: 0000 6586 0004 bda9 0000 54aa 0004 d025  ..e.......T....%
-00000050: 0000 579c 0004 ec30 0000 5844 0005 4835  ..W....0..XD..H5
-00000060: 0000 089f 0005 4835 0000 72a5 0005 4835  ......H5..r...H5
-00000070: 0000 81b2 0005 8c04 0000 5b04 0005 97c5  ..........[.....
-00000080: 0000 2c44 0005 a200 0000 9b4a 0007 c4af  ..,D.......J....
-00000090: 0000 3a74 0012 2b0e 0000 5327 001c da4d  ..:t..+...S'...M
-000000a0: 0000 4b85 001c dbdd 0000 9664 0024 12d5  ..K........d.$..
-000000b0: 0000 38e5 002c f63e 0000 1695 002d 8634  ..8..,.>.....-.4
-000000c0: 0000 806e 0037 171b 0000 8018 003b f105  ...n.7.......;..
-000000d0: 0000 1c2a 0040 e4ce 0000 9f96 0043 4cae  ...*.@.......CL.
-000000e0: 0000 a0c3 0047 c4e3 0000 9873 004b 87d4  .....G.....s.K..
-000000f0: 0000 7c96 0056 aec2 0000 7e1b 0056 aec2  ..|..V....~..V..
-00000100: 0000 8909 0056 f6af 0000 2b1c 005a 81be  .....V....+..Z..
-00000110: 0000 8a93 005b 0b25 0000 2d47 005b 0b25  .....[.%..-G.[.%
-00000120: 0000 4b56 005b 0b25 0000 80c6 0060 1085  ..KV.[.%.....`..
-00000130: 0000 7ea1 0067 aad3 0000 57c6 0069 a403  ..~..g....W..i..
-00000140: 0000 35e8 0069 a403 0000 586e 006c c199  ..5..i....Xn.l..
-00000150: 0000 2742 0071 0769 0000 6018 0094 cf02  ..'B.q.i..`.....
-00000160: 0000 8a4d 00a2 1470 0000 8e75 00a3 85ee  ...M...p...u....
-00000170: 0000 0671 00b8 6470 0000 8d99 00bd d20e  ...q..dp........
-00000180: 0000 9229 00c0 dd34 0000 4610 00c6 1d14  ...)...4..F.....
-00000190: 0000 95c3 00c6 6470 0000 8e04 00d1 9ab5  ......dp........
-000001a0: 0000 97a8 00d7 0cb9 0000 3743 00f2 f2c8  ..........7C....
-000001b0: 0000 297b 0106 6074 0000 4d11 011d e755  ..){..`t..M....U
-000001c0: 0000 45c4 0126 bda5 0000 6666 0145 eb79  ..E..&....ff.E.y
-000001d0: 0000 324e 015e eb2f 0000 9e91 015f 0dad  ..2N.^./....._..
-000001e0: 0000 31ca 0163 c933 0000 2125 016a 032e  ..1..c.3..!%.j..
-000001f0: 0000 68a2 0173 8fc8 0000 9620 0180 6a59  ..h..s..... ..jY
-00000200: 0000 554f 018e d47e 0000 113b 018f 97f8  ..UO...~...;....
-00000210: 0000 87f2 01be 34b7 0000 8684 01c1 faa5  ......4.........
-00000220: 0000 2813 01c1 faa5 0000 8131 01c5 f5cd  ..(........1....
-00000230: 0000 9085 01ca 84a1 0000 7885 01d2 e96e  ..........x....n
-00000240: 0000 58b0 01d8 cd24 0000 3aaa 01e4 e113  ..X....$..:.....
-00000250: 0000 8ee2 01f7 4f45 0000 66c1 01fc 7925  ......OE..f...y%
-00000260: 0000 5407 01fd 69a5 0000 1da5 0201 ff63  ..T...i........c
-00000270: 0000 8349 0232 05d5 0000 4261 0249 c9ae  ...I.2....Ba.I..
-00000280: 0000 98e2 026d bc14 0000 9b8a 0277 2b35  .....m.......w+5
-00000290: 0000 39c5 0286 e00e 0000 118b 0296 5357  ..9...........SW
-000002a0: 0000 527d 0298 5c09 0000 62e0 02c8 9fa3  ..R}..\...b.....
-000002b0: 0000 2401 02cf fca5 0000 32fc 02d6 0815  ..$.......2.....
-000002c0: 0000 9afb 02f9 c4c5 0000 29d9 02f9 c4c5  ..........).....
-000002d0: 0000 49b1 02f9 c4c5 0000 7d47 0302 20f5  ..I.......}G.. .
-000002e0: 0000 4e34 0305 1aa9 0000 46ad 030c 9764  ..N4......F....d
-000002f0: 0000 5a5e 0354 44bd 0000 34ef 0359 7694  ..Z^.TD...4..Yv.
-00000300: 0000 94fe 035a 4e6e 0000 6e21 037d 2417  .....ZNn..n!.}$.
-00000310: 0000 8fa3 037d 9c24 0000 7e4c 037f eb99  .....}.$..~L....
-00000320: 0000 670f 0380 b55f 0000 9c2d 0391 ff0e  ..g...._...-....
-00000330: 0000 03c6 039a 6ece 0000 9456 03b0 bf25  ......n....V...%
-00000340: 0000 00b6 03b0 bf25 0000 77a8 03b4 664e  .......%..w...fN
-00000350: 0000 a089 03b5 83a3 0000 7c38 03e2 d39e  ..........|8....
-00000360: 0000 0ccb 03e6 8545 0000 74a8 03ef 1f79  .......E..t....y
-00000370: 0000 3450 03f1 1a05 0000 8754 03ff d948  ..4P.......T...H
-00000380: 0000 857a 0409 59a5 0000 7370 040e 9e79  ...z..Y...sp...y
-00000390: 0000 4a67 0442 4dfe 0000 775f 0457 019e  ..Jg.BM...w_.W..
-000003a0: 0000 0533 0459 8f63 0000 5b86 045f e8c9  ...3.Y.c..[.._..
-000003b0: 0000 1cc5 0460 e588 0000 54f6 0498 3c81  .....`....T...<.
-000003c0: 0000 84b3 04ab 7ea5 0000 4e7a 04c8 4039  ......~...Nz..@9
-000003d0: 0000 2892 04c8 4039 0000 47fe 04d2 fa22  ..(...@9..G...."
-000003e0: 0000 28c4 04d3 9ff4 0000 302d 04f5 7367  ..(.......0-..sg
-000003f0: 0000 2ab9 051a 65f5 0000 9736 0520 62a4  ..*...e....6. b.
-00000400: 0000 7649 0528 4ac0 0000 4dca 052d 4d3c  ..vI.(J...M..-M<
-00000410: 0000 2689 0530 af74 0000 80f5 0531 a702  ..&..0.t.....1..
-00000420: 0000 3f74 0535 96fe 0000 94c4 0537 8957  ..?t.5.......7.W
-00000430: 0000 23ad 053b 7b05 0000 2a77 053b 7b05  ..#..;{...*w.;{.
-00000440: 0000 4a23 053e 782d 0000 412e 0544 794d  ..J#.>x-..A..DyM
-00000450: 0000 40cf 055f 746e 0000 92d0 0565 06e3  ..@.._tn.....e..
-00000460: 0000 0ae8 0577 76ec 0000 85bb 057b 92f3  .....wv......{..
-00000470: 0000 2b78 057b 92f3 0000 7f6e 0588 b047  ..+x.{.....n...G
-00000480: 0000 1bef 058b e05e 0000 0905 058f dfb3  .......^........
-00000490: 0000 7479 059b 8898 0000 78d9 05a3 3419  ..ty......x...4.
-000004a0: 0000 768d 05a6 17ae 0000 7b92 05a6 c895  ..v.......{.....
-000004b0: 0000 3fd0 05a9 c6ae 0000 7561 05ab 8bc4  ..?.......ua....
-000004c0: 0000 0936 05ac 8de5 0000 2a0a 05af caf4  ...6......*.....
-000004d0: 0000 888c 05b9 6619 0000 1df0 05d3 4c4e  ......f.......LN
-000004e0: 0000 770b 05dd d675 0000 65b1 05e9 9749  ..w....u..e....I
-000004f0: 0000 7f0d 05fe 219e 0000 88c7 0618 f51e  ......!.........
-00000500: 0000 6ef5 0626 dcc9 0000 4002 0627 7c75  ..n..&....@..'|u
-00000510: 0000 4045 063b cf25 0000 3574 0647 6c6e  ..@E.;.%..5t.Gln
-00000520: 0000 3bda 064f 4f8e 0000 6c08 0653 24e5  ..;..OO...l..S$.
-00000530: 0000 7ac3 065a 7e13 0000 4675 0667 a1fe  ..z..Z~...Fu.g..
-00000540: 0000 7d7a 066a 3ba3 0000 21eb 067b 0603  ..}z.j;...!..{..
-00000550: 0000 595b 067c 1595 0000 3a39 068d 7d90  ..Y[.|....:9..}.
-00000560: 0000 77d7 068f 2045 0000 4358 0698 3c81  ..w... E..CX..<.
-00000570: 0000 0967 069d bc4e 0000 1420 06b7 eb69  ...g...N... ...i
-00000580: 0000 2dcb 06ba eeff 0000 9f0b 06c3 2be7  ..-...........+.
-00000590: 0000 5c13 06c9 55b9 0000 4979 06c9 b805  ..\...U...Iy....
-000005a0: 0000 839a 06ce 697e 0000 3d26 06d4 e879  ......i~..=&...y
-000005b0: 0000 3355 06e7 88c7 0000 5125 06ea 1312  ..3U......Q%....
-000005c0: 0000 3e82 06f1 acb5 0000 783b 0706 6093  ..>.......x;..`.
-000005d0: 0000 7513 071b d822 0000 97fe 0725 0ed3  ..u....".....%..
-000005e0: 0000 3cdf 072a 02b3 0000 3b32 072b 5bf1  ..<..*....;2.+[.
-000005f0: 0000 893b 073b 0713 0000 3dce 073e 8aae  ...;.;....=..>..
-00000600: 0000 30e1 0740 7b19 0000 3699 0745 d72e  ..0..@{...6..E..
-00000610: 0000 a03e 0747 58b5 0000 316b 0752 93ae  ...>.GX...1k.R..
-00000620: 0000 0140 0756 937c 0000 8ba8 0761 5de5  ...@.V.|.....a].
-00000630: 0000 1e58 0773 020e 0000 90e3 0778 9733  ...X.s.......x.3
-00000640: 0000 89a6 077c e91e 0000 3983 0783 2294  .....|....9...".
-00000650: 0000 2013 078c 0ba4 0000 1c84 0790 c8f5  .. .............
-00000660: 0000 2b47 0791 9109 0000 47ab 079d a354  ..+G......G....T
-00000670: 0000 9bdc 07a1 d6cb 0000 5aa2 07ab 8e03  ..........Z.....
-00000680: 0000 0000 07b4 0f05 0000 73da 07c3 bd54  ..........s....T
-00000690: 0000 8cbc 07e0 1a4f 0000 33c5 07f6 6e0f  .......O..3...n.
-000006a0: 0000 931f 0812 7098 0000 7908 0842 126e  ......p...y..B.n
-000006b0: 0000 598e 0843 f97e 0000 1872 0847 159e  ..Y..C.~...r.G..
-000006c0: 0000 8ff5 084e b2f5 0000 4dfc 089b d2f1  .....N....M.....
-000006d0: 0000 81dd 08a4 2089 0000 7b2b 08ad 8b6e  ...... ...{+...n
-000006e0: 0000 700e 08ae abbe 0000 0188 08bc 210e  ..p...........!.
-000006f0: 0000 0c86 08bd 8ce8 0000 418d 08f0 ac75  ..........A....u
-00000700: 0000 224d 08fb ecd3 0000 56db 08ff ed5f  .."M......V...._
-00000710: 0000 2e67 090d 6f19 0000 1aca 091d 05f0  ...g..o.........
-00000720: 0000 741a 0920 f035 0000 720a 0923 8a14  ..t.. .5..r..#..
-00000730: 0000 8f39 092a 03d5 0000 0037 092c eb99  ...9.*.....7.,..
-00000740: 0000 10ca 0941 e34c 0000 1f5f 0949 9184  .....A.L..._.I..
-00000750: 0000 79d6 0949 b384 0000 5f6f 094d 67fe  ..y..I...._o.Mg.
-00000760: 0000 2851 094d 67fe 0000 4738 094d 67fe  ..(Q.Mg...G8.Mg.
-00000770: 0000 7bf5 094d 67fe 0000 8170 095e 89d3  ..{..Mg....p.^..
-00000780: 0000 9a21 0968 7d7d 0000 2a3a 0968 7d7d  ...!.h}}..*:.h}}
-00000790: 0000 3128 0968 7d7d 0000 49e4 096d 01e5  ..1(.h}}..I..m..
-000007a0: 0000 08ca 096f 9788 0000 8797 0974 a647  .....o.......t.G
-000007b0: 0000 516b 097c 1775 0000 39fe 0987 b01e  ..Qk.|.u..9.....
-000007c0: 0000 7a7c 09ca a91e 0000 6d20 09ee 202e  ..z|......m .. .
-000007d0: 0000 153e 09f5 9023 0000 4c35 0a0d 74f2  ...>...#..L5..t.
-000007e0: 0000 09de 0a0d 74f2 0000 59ef 0a3b 8333  ......t...Y..;.3
-000007f0: 0000 078e 0a69 66c9 0000 38a4 0a6c 5bd9  .....if...8..l[.
-00000800: 0000 0112 0a6c 5bd9 0000 6606 0a73 2a51  .....l[...f..s*Q
-00000810: 0000 362c 0a7f ce9e 0000 9c96 0a89 b649  ..6,...........I
-00000820: 0000 2927 0a8b 8b22 0000 6632 0a8b d95e  ..)'..."..f2...^
-00000830: 0000 3806 0a99 6ff8 0000 8acf 0ac7 826e  ..8...o........n
-00000840: 0000 05b6 0ad6 d87e 0000 01d7 0ae9 b7f5  .......~........
-00000850: 0000 257d 0aea 9594 0000 22ad 0afb 86b9  ..%}......".....
-00000860: 0000 5239 0b0c 8953 0000 3096 0b16 9077  ..R9...S..0....w
-00000870: 0000 081a 0b31 6541 0000 0c1e 0b32 f535  .....1eA.....2.5
-00000880: 0000 4cb4 0b52 aea4 0000 41c6 0b55 9355  ..L..R....A..U.U
-00000890: 0000 96de 0b69 37c9 0000 63f5 0b6f 5c75  .....i7...c..o\u
-000008a0: 0000 870b 0b70 d229 0000 2d74 0b7b 2ca5  .....p.)..-t.{,.
-000008b0: 0000 1b65 0b81 700e 0000 6746 0b82 249e  ...e..p...gF..$.
-000008c0: 0000 04b5 0b8a 2614 0000 2c02 0ba0 757f  ......&...,...u.
-000008d0: 0000 9d39 0ba0 9785 0000 440a 0ba0 c9de  ...9......D.....
-000008e0: 0000 8a0d 0ba3 fc0c 0000 3eea 0ba4 08e7  ..........>.....
-000008f0: 0000 3f30 0bbf 620d 0000 0a4d 0bc0 05e4  ..?0..b....M....
-00000900: 0000 2cbc 0be4 0395 0000 884d 0bf0 453e  ..,........M..E>
-00000910: 0000 2093 0c13 2b8e 0000 3c2d 0c1a b9a5  .. ...+...<-....
-00000920: 0000 51db 0c25 7849 0000 608a 0c27 e76f  ..Q..%xI..`..'.o
-00000930: 0000 9df8 0c29 84a3 0000 3933 0c35 9b9e  .....)....93.5..
-00000940: 0000 64cb 0c4c 8c75 0000 7d0b 0c5d e1c2  ..d..L.u..}..]..
-00000950: 0000 246d 0c5e 6fb4 0000 408e 0c7d 7095  ..$m.^o...@..}p.
-00000960: 0000 2643 0c80 8aa3 0000 37b4 0c80 8aa3  ..&C......7.....
-00000970: 0000 5b36 0c93 93be 0000 5df2 0c94 ba43  ..[6......]....C
-00000980: 0000 0b83 0ca0 d5c3 0000 1fb5 0cbb 0173  ...............s
-00000990: 0000 5bd5 0cca 0285 0000 477b 0cce 648d  ..[.......G{..d.
-000009a0: 0000 9539 0cd8 f02d 0000 0998 0d04 cb1e  ...9...-........
-000009b0: 0000 3b86 0d0e 6da3 0000 1ba6 0d19 6c99  ..;...m.......l.
-000009c0: 0000 4888 0d34 07f1 0000 1f09 0d36 9b85  ..H..4.......6..
-000009d0: 0000 5fcd 0d86 3e6e 0000 5c55 0d8c 40ce  .._...>n..\U..@.
-000009e0: 0000 76c8 0d8f c4f3 0000 28f4 0d8f c4f3  ..v.......(.....
-000009f0: 0000 4944 0d96 5b13 0000 219f 0d96 f824  ..ID..[...!....$
-00000a00: 0000 22fb 0db0 6493 0000 4832 0dba 6f39  .."...d...H2..o9
-00000a10: 0000 61ec 0dc9 1a88 0000 25d0 0dd7 f89b  ..a.......%.....
-00000a20: 0000 5732 0e03 0de0 0000 2514 0e03 0de0  ..W2......%.....
-00000a30: 0000 4559 0e0b 4344 0000 8536 0e0c 2965  ..EY..CD...6..)e
-00000a40: 0000 44ce 0e14 c055 0000 567d 0e2c 0f2e  ..D....U..V}.,..
-00000a50: 0000 7dd3 0e31 45cf 0000 827a 0e39 c321  ..}..1E....z.9.!
-00000a60: 0000 5f09 0e6e 2258 0000 8441 0e6e 4858  .._..n"X...A.nHX
-00000a70: 0000 83cf 0e95 28b5 0000 1d11 0e97 bcb5  ......(.........
-00000a80: 0000 1d5d 0e9c a374 0000 8c3b 0e9e 60ae  ...]...t...;..`.
-00000a90: 0000 5007 0ea3 b08e 0000 02dd 0eaf 6fc3  ..P...........o.
-00000aa0: 0000 7266 0ebe c4c3 0000 7974 0ec1 ac3f  ..rf......yt...?
-00000ab0: 0000 4d7d 0ed2 6f37 0000 85fe 0ed2 862e  ..M}..o7........
-00000ac0: 0000 6a3c 0edb 53e1 0000 2bb0 0edb 53e1  ..j<..S...+...S.
-00000ad0: 0000 4ab9 0edd a743 0000 1eb7 0edf 208d  ..J....C...... .
-00000ae0: 0000 8d3d 0eeb 97ce 0000 6b04 0eed da75  ...=......k....u
-00000af0: 0000 84e6 0eee 44a4 0000 8bdb 0ef1 01de  ......D.........
-00000b00: 0000 5590 0ef6 09ee 0000 06fe 0f05 000c  ..U.............
-00000b10: 0000 2c72 0f16 93ca 0000 4bfb 0f31 815c  ..,r......K..1.\
-00000b20: 0000 42da 0f33 2495 0000 2e24 0f48 89e2  ..B..3$....$.H..
-00000b30: 0000 72ce 0f62 0773 0000 3e1d 0f64 7a39  ..r..b.s..>..dz9
-00000b40: 0000 7337 0f66 4e29 0000 7cc9 0f6f e836  ..s7.fN)..|..o.6
-00000b50: 0000 823b 0f82 a059 0000 7fa8 0f8f 1b8e  ...;...Y........
-00000b60: 0000 24c6 0f9a 906e 0000 4ee2 0f9d 6ca9  ..$....n..N...l.
-00000b70: 0000 26e8 0fa8 b309 0000 613f 0fa9 1015  ..&.......a?....
-00000b80: 0000 9a63 0fb1 d16f 0000 9aae 0fb6 b24e  ...c...o.......N
-00000b90: 0000 711d 0fd4 15de 0000 421c 0fd4 15de  ..q.......B.....
-00000ba0: 0000 7a37 0fe8 0889 0000 53bb 0fef 5405  ..z7......S...T.
-00000bb0: 0000 2d00 0fef 5405 0000 4b0d 6900 00a0  ..-...T...K.i...
-00000bc0: ee03 0000 0010 0026 0041 0064 0072 0065  .......&.A.d.r.e
-00000bd0: 0073 0073 0065 0800 0000 0006 0000 0008  .s.s.e..........
-00000be0: 2641 6464 7265 7373 0700 0000 0a41 6464  &Address.....Add
-00000bf0: 7265 7373 5461 6201 0300 0000 3e00 4100  ressTab.....>.A.
-00000c00: 6400 7200 6500 7300 7300 7300 7500 6300  d.r.e.s.s.s.u.c.
-00000c10: 6800 6500 2000 7000 6f00 7700 6500 7200  h.e. .p.o.w.e.r.
-00000c20: 6500 6400 2000 6200 7900 2000 4f00 7000  e.d. .b.y. .O.p.
-00000c30: 6500 6e00 4300 6100 6700 6508 0000 0000  e.n.C.a.g.e.....
-00000c40: 0600 0000 2241 6464 7265 7373 206c 6f6f  ...."Address loo
-00000c50: 6b75 7020 706f 7765 7265 6420 6279 204f  kup powered by O
-00000c60: 7065 6e43 6167 6507 0000 000a 4164 6472  penCage.....Addr
-00000c70: 6573 7354 6162 0103 0000 0008 0048 00f6  essTab.......H..
-00000c80: 0068 0065 0800 0000 0006 0000 0008 416c  .h.e..........Al
-00000c90: 7469 7475 6465 0700 0000 0a41 6464 7265  titude.....Addre
-00000ca0: 7373 5461 6201 0300 0000 0a00 5300 7400  ssTab.......S.t.
-00000cb0: 6100 6400 7408 0000 0000 0600 0000 0443  a.d.t..........C
-00000cc0: 6974 7907 0000 000a 4164 6472 6573 7354  ity.....AddressT
-00000cd0: 6162 0103 0000 0008 004c 0061 006e 0064  ab.......L.a.n.d
-00000ce0: 0800 0000 0006 0000 0007 436f 756e 7472  ..........Countr
-00000cf0: 7907 0000 000a 4164 6472 6573 7354 6162  y.....AddressTab
-00000d00: 0103 0000 001a 004f 0072 0074 0020 0065  .......O.r.t. .e
-00000d10: 006e 0074 0066 0065 0072 006e 0065 006e  .n.t.f.e.r.n.e.n
-00000d20: 0800 0000 0006 0000 000f 4465 6c65 7465  ..........Delete
-00000d30: 206c 6f63 6174 696f 6e07 0000 000a 4164   location.....Ad
-00000d40: 6472 6573 7354 6162 0103 0000 001e 004f  dressTab.......O
-00000d50: 0072 0074 0020 0064 0075 0070 006c 0069  .r.t. .d.u.p.l.i
-00000d60: 007a 0069 0065 0072 0065 006e 0800 0000  .z.i.e.r.e.n....
-00000d70: 0006 0000 0012 4475 706c 6963 6174 6520  ......Duplicate 
-00000d80: 6c6f 6361 7469 6f6e 0700 0000 0a41 6464  location.....Add
-00000d90: 7265 7373 5461 6201 0300 0000 aa00 4700  ressTab.......G.
-00000da0: 6500 6200 6500 6e00 2000 5300 6900 6500  e.b.e.n. .S.i.e.
-00000db0: 2000 6400 6500 6e00 2000 6100 7500 7300   .d.e.n. .a.u.s.
-00000dc0: 2000 3200 2000 6f00 6400 6500 7200 2000   .2. .o.d.e.r. .
-00000dd0: 3300 2000 4200 7500 6300 6800 7300 7400  3. .B.u.c.h.s.t.
-00000de0: 6100 6200 6500 6e00 2000 6200 6500 7300  a.b.e.n. .b.e.s.
-00000df0: 7400 6500 6800 6500 6e00 6400 6500 6e00  t.e.h.e.n.d.e.n.
-00000e00: 2000 4900 5300 4f00 2d00 3300 3100 3600   .I.S.O.-.3.1.6.
-00000e10: 3600 2d00 4c00 e400 6e00 6400 6500 7200  6.-.L...n.d.e.r.
-00000e20: 6300 6f00 6400 6500 2000 6400 6500 7300  c.o.d.e. .d.e.s.
-00000e30: 2000 4c00 6100 6e00 6400 6500 7300 2000   .L.a.n.d.e.s. .
-00000e40: 6500 6900 6e00 2e08 0000 0000 0600 0000  e.i.n...........
-00000e50: 3d45 6e74 6572 2074 6865 2032 206f 7220  =Enter the 2 or 
-00000e60: 3320 6c65 7474 6572 2049 534f 2033 3136  3 letter ISO 316
-00000e70: 3620 636f 756e 7472 7920 636f 6465 206f  6 country code o
-00000e80: 6620 7468 6520 636f 756e 7472 792e 0700  f the country...
-00000e90: 0000 0a41 6464 7265 7373 5461 6201 0300  ...AddressTab...
-00000ea0: 0000 8a00 4700 6500 6200 6500 6e00 2000  ....G.e.b.e.n. .
-00000eb0: 5300 6900 6500 2000 6400 6900 6500 2000  S.i.e. .d.i.e. .
-00000ec0: 4400 6500 7400 6100 6900 6c00 7300 2000  D.e.t.a.i.l.s. .
-00000ed0: 7a00 7500 2000 6400 6500 6d00 2000 4f00  z.u. .d.e.m. .O.
-00000ee0: 7200 7400 2000 6500 6900 6e00 2c00 2000  r.t. .e.i.n.,. .
-00000ef0: 6100 6e00 2000 6400 6500 6d00 2000 6400  a.n. .d.e.m. .d.
-00000f00: 6100 7300 2000 4200 6900 6c00 6400 2000  a.s. .B.i.l.d. .
-00000f10: 6500 7200 7300 7400 6500 6c00 6c00 7400  e.r.s.t.e.l.l.t.
-00000f20: 2000 7700 7500 7200 6400 6500 2e08 0000   .w.u.r.d.e.....
-00000f30: 0000 0600 0000 4045 6e74 6572 2074 6865  ......@Enter the
-00000f40: 2064 6574 6169 6c73 2061 626f 7574 2061   details about a
-00000f50: 206c 6f63 6174 696f 6e20 7768 6572 6520   location where 
-00000f60: 7468 6973 2069 6d61 6765 2077 6173 2063  this image was c
-00000f70: 7265 6174 6564 2e07 0000 000a 4164 6472  reated......Addr
-00000f80: 6573 7354 6162 0103 0000 0090 0047 0065  essTab.......G.e
-00000f90: 0062 0065 006e 0020 0053 0069 0065 0020  .b.e.n. .S.i.e. 
-00000fa0: 0064 0069 0065 0020 0044 0065 0074 0061  .d.i.e. .D.e.t.a
-00000fb0: 0069 006c 0073 0020 007a 0075 0020 0065  .i.l.s. .z.u. .e
-00000fc0: 0069 006e 0065 006d 0020 004f 0072 0074  .i.n.e.m. .O.r.t
-00000fd0: 0020 0065 0069 006e 002c 0020 0064 0065  . .e.i.n.,. .d.e
-00000fe0: 0072 0020 0069 006e 0020 0064 0069 0065  .r. .i.n. .d.i.e
-00000ff0: 0073 0065 006d 0020 0042 0069 006c 0064  .s.e.m. .B.i.l.d
-00001000: 0020 0067 0065 007a 0065 0069 0067 0074  . .g.e.z.e.i.g.t
-00001010: 0020 0077 0069 0072 0064 002e 0800 0000  . .w.i.r.d......
-00001020: 0006 0000 0040 456e 7465 7220 7468 6520  .....@Enter the 
-00001030: 6465 7461 696c 7320 6162 6f75 7420 6120  details about a 
-00001040: 6c6f 6361 7469 6f6e 2077 6869 6368 2069  location which i
-00001050: 7320 7368 6f77 6e20 696e 2074 6869 7320  s shown in this 
-00001060: 696d 6167 652e 0700 0000 0a41 6464 7265  image......Addre
-00001070: 7373 5461 6201 0300 0000 4400 4700 6500  ssTab.....D.G.e.
-00001080: 6200 6500 6e00 2000 5300 6900 6500 2000  b.e.n. .S.i.e. .
-00001090: 6400 6500 6e00 2000 4e00 6100 6d00 6500  d.e.n. .N.a.m.e.
-000010a0: 6e00 2000 6400 6500 7200 2000 5300 7400  n. .d.e.r. .S.t.
-000010b0: 6100 6400 7400 2000 6500 6900 6e00 2e08  a.d.t. .e.i.n...
-000010c0: 0000 0000 0600 0000 1b45 6e74 6572 2074  .........Enter t
-000010d0: 6865 206e 616d 6520 6f66 2074 6865 2063  he name of the c
-000010e0: 6974 792e 0700 0000 0a41 6464 7265 7373  ity......Address
-000010f0: 5461 6201 0300 0000 4600 4700 6500 6200  Tab.....F.G.e.b.
-00001100: 6500 6e00 2000 5300 6900 6500 2000 6400  e.n. .S.i.e. .d.
-00001110: 6500 6e00 2000 4e00 6100 6d00 6500 6e00  e.n. .N.a.m.e.n.
-00001120: 2000 6400 6500 7300 2000 4c00 6100 6e00   .d.e.s. .L.a.n.
-00001130: 6400 6500 7300 2000 6500 6900 6e00 2e08  d.e.s. .e.i.n...
-00001140: 0000 0000 0600 0000 1e45 6e74 6572 2074  .........Enter t
-00001150: 6865 206e 616d 6520 6f66 2074 6865 2063  he name of the c
-00001160: 6f75 6e74 7279 2e07 0000 000a 4164 6472  ountry......Addr
-00001170: 6573 7354 6162 0103 0000 0074 0047 0065  essTab.....t.G.e
-00001180: 0062 0065 006e 0020 0053 0069 0065 0020  .b.e.n. .S.i.e. 
-00001190: 0064 0065 006e 0020 004e 0061 006d 0065  .d.e.n. .N.a.m.e
-000011a0: 006e 0020 0064 0065 0072 0020 0050 0072  .n. .d.e.r. .P.r
-000011b0: 006f 0076 0069 006e 007a 0020 006f 0064  .o.v.i.n.z. .o.d
-000011c0: 0065 0072 0020 0064 0065 0073 0020 0042  .e.r. .d.e.s. .B
-000011d0: 0075 006e 0064 0065 0073 006c 0061 006e  .u.n.d.e.s.l.a.n
-000011e0: 0064 0065 0073 0020 0065 0069 006e 002e  .d.e.s. .e.i.n..
-000011f0: 0800 0000 0006 0000 0028 456e 7465 7220  .........(Enter 
-00001200: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-00001210: 7072 6f76 696e 6365 206f 7220 7374 6174  province or stat
-00001220: 652e 0700 0000 0a41 6464 7265 7373 5461  e......AddressTa
-00001230: 6201 0300 0000 4c00 4700 6500 6200 6500  b.....L.G.e.b.e.
-00001240: 6e00 2000 5300 6900 6500 2000 6400 6500  n. .S.i.e. .d.e.
-00001250: 6e00 2000 4e00 6100 6d00 6500 6e00 2000  n. .N.a.m.e.n. .
-00001260: 6400 6500 7300 2000 5500 6e00 7400 6500  d.e.s. .U.n.t.e.
-00001270: 7200 6f00 7200 7400 7300 2000 6500 6900  r.o.r.t.s. .e.i.
-00001280: 6e00 2e08 0000 0000 0600 0000 2245 6e74  n..........."Ent
-00001290: 6572 2074 6865 206e 616d 6520 6f66 2074  er the name of t
-000012a0: 6865 2073 7562 6c6f 6361 7469 6f6e 2e07  he sublocation..
-000012b0: 0000 000a 4164 6472 6573 7354 6162 0103  ....AddressTab..
-000012c0: 0000 004e 0047 0065 0062 0065 006e 0020  ...N.G.e.b.e.n. 
-000012d0: 0053 0069 0065 0020 0064 0065 006e 0020  .S.i.e. .d.e.n. 
-000012e0: 004e 0061 006d 0065 006e 0020 0064 0065  .N.a.m.e.n. .d.e
-000012f0: 0072 0020 0057 0065 006c 0074 0072 0065  .r. .W.e.l.t.r.e
-00001300: 0067 0069 006f 006e 0020 0065 0069 006e  .g.i.o.n. .e.i.n
-00001310: 002e 0800 0000 0006 0000 0023 456e 7465  ...........#Ente
-00001320: 7220 7468 6520 6e61 6d65 206f 6620 7468  r the name of th
-00001330: 6520 776f 726c 6420 7265 6769 6f6e 2e07  e world region..
-00001340: 0000 000a 4164 6472 6573 7354 6162 0103  ....AddressTab..
-00001350: 0000 0048 0047 0065 006f 0064 0061 0074  ...H.G.e.o.d.a.t
-00001360: 0061 0020 00a9 0020 004f 0070 0065 006e  .a. ... .O.p.e.n
-00001370: 0053 0074 0072 0065 0065 0074 004d 0061  .S.t.r.e.e.t.M.a
-00001380: 0070 0020 0063 006f 006e 0074 0072 0069  .p. .c.o.n.t.r.i
-00001390: 0062 0075 0074 006f 0072 0073 0800 0000  .b.u.t.o.r.s....
-000013a0: 0006 0000 0025 4765 6f64 6174 6120 c2a9  .....%Geodata ..
-000013b0: 204f 7065 6e53 7472 6565 744d 6170 2063   OpenStreetMap c
-000013c0: 6f6e 7472 6962 7574 6f72 7307 0000 000a  ontributors.....
-000013d0: 4164 6472 6573 7354 6162 0103 0000 004c  AddressTab.....L
-000013e0: 0041 0064 0072 0065 0073 0073 0065 0020  .A.d.r.e.s.s.e. 
-000013f0: 0061 0075 0073 0020 0042 0072 0065 0069  .a.u.s. .B.r.e.i
-00001400: 0074 0065 0020 0075 006e 0064 0020 004c  .t.e. .u.n.d. .L
-00001410: 00e4 006e 0067 0065 0020 0065 0072 006d  ...n.g.e. .e.r.m
-00001420: 0069 0074 0074 0065 006c 006e 0800 0000  .i.t.t.e.l.n....
-00001430: 0006 0000 001a 4765 7420 6164 6472 6573  ......Get addres
-00001440: 7320 6672 6f6d 206c 6174 2c20 6c6f 6e67  s from lat, long
-00001450: 0700 0000 0a41 6464 7265 7373 5461 6201  .....AddressTab.
-00001460: 0300 0000 0800 4e00 6100 6d00 6508 0000  ......N.a.m.e...
-00001470: 0000 0600 0000 044e 616d 6507 0000 000a  .......Name.....
-00001480: 4164 6472 6573 7354 6162 0103 0000 0014  AddressTab......
-00001490: 0042 0075 006e 0064 0065 0073 006c 0061  .B.u.n.d.e.s.l.a
-000014a0: 006e 0064 0800 0000 0006 0000 0008 5072  .n.d..........Pr
-000014b0: 6f76 696e 6365 0700 0000 0a41 6464 7265  ovince.....Addre
-000014c0: 7373 5461 6201 0300 0000 0c00 5200 6500  ssTab.......R.e.
-000014d0: 6700 6900 6f00 6e08 0000 0000 0600 0000  g.i.o.n.........
-000014e0: 0652 6567 696f 6e07 0000 000a 4164 6472  .Region.....Addr
-000014f0: 6573 7354 6162 0103 0000 000c 0053 0074  essTab.......S.t
-00001500: 0072 0061 00df 0065 0800 0000 0006 0000  .r.a...e........
-00001510: 0006 5374 7265 6574 0700 0000 0a41 6464  ..Street.....Add
-00001520: 7265 7373 5461 6201 0300 0000 0c00 4b00  ressTab.......K.
-00001530: 6100 6d00 6500 7200 6108 0000 0000 0600  a.m.e.r.a.......
-00001540: 0000 0663 616d 6572 6107 0000 000a 4164  ...camera.....Ad
-00001550: 6472 6573 7354 6162 0103 0000 001a 0042  dressTab.......B
-00001560: 0065 0074 0072 0065 0066 0066 0020 007b  .e.t.r.e.f.f. .{
-00001570: 0069 0064 0078 007d 0800 0000 0006 0000  .i.d.x.}........
-00001580: 000d 7375 626a 6563 7420 7b69 6478 7d07  ..subject {idx}.
-00001590: 0000 000a 4164 6472 6573 7354 6162 0103  ....AddressTab..
-000015a0: 0000 0036 0050 0068 006f 0074 0069 006e  ...6.P.h.o.t.i.n
-000015b0: 0069 002d 0046 006f 0074 006f 006d 0065  .i.-.F.o.t.o.m.e
-000015c0: 0074 0061 0064 0061 0074 0065 006e 0065  .t.a.d.a.t.e.n.e
-000015d0: 0064 0069 0074 006f 0072 0800 0000 0006  .d.i.t.o.r......
-000015e0: 0000 001d 5068 6f74 696e 6920 7068 6f74  ....Photini phot
-000015f0: 6f20 6d65 7461 6461 7461 2065 6469 746f  o metadata edito
-00001600: 7207 0000 0007 434c 4948 656c 7001 0300  r.....CLIHelp...
-00001610: 0000 5800 5600 6500 7200 7700 6500 6e00  ..X.V.e.r.w.e.n.
-00001620: 6400 7500 6e00 6700 3a00 2000 2500 7000  d.u.n.g.:. .%.p.
-00001630: 7200 6f00 6700 2000 5b00 6f00 7000 7400  r.o.g. .[.o.p.t.
-00001640: 6900 6f00 6e00 7300 5d00 2000 5b00 6600  i.o.n.s.]. .[.f.
-00001650: 6900 6c00 6500 5f00 6e00 6100 6d00 6500  i.l.e._.n.a.m.e.
-00001660: 2c00 2000 2e00 2e00 2e00 5d08 0000 0000  ,. .......].....
-00001670: 0600 0000 2755 7361 6765 3a20 2570 726f  ....'Usage: %pro
-00001680: 6720 5b6f 7074 696f 6e73 5d20 5b66 696c  g [options] [fil
-00001690: 655f 6e61 6d65 2c20 2e2e 2e5d 0700 0000  e_name, ...]....
-000016a0: 0743 4c49 4865 6c70 0103 0000 005c 0041  .CLIHelp.....\.A
-000016b0: 006e 007a 0061 0068 006c 0020 0064 0065  .n.z.a.h.l. .d.e
-000016c0: 0072 0020 0045 0069 006e 0074 0072 00e4  .r. .E.i.n.t.r..
-000016d0: 0067 0065 0020 0069 006d 0020 0046 0065  .g.e. .i.m. .F.e
-000016e0: 0068 006c 0065 0072 0070 0072 006f 0074  .h.l.e.r.p.r.o.t
-000016f0: 006f 006b 006f 006c 006c 0020 0065 0072  .o.k.o.l.l. .e.r
-00001700: 0068 00f6 0068 0065 006e 0800 0000 0006  .h...h.e.n......
-00001710: 0000 0023 696e 6372 6561 7365 206e 756d  ...#increase num
-00001720: 6265 7220 6f66 206c 6f67 6769 6e67 206d  ber of logging m
-00001730: 6573 7361 6765 7307 0000 0007 434c 4948  essages.....CLIH
-00001740: 656c 7001 0300 0000 5e00 4e00 6500 7500  elp.....^.N.e.u.
-00001750: 6500 2000 4600 7500 6e00 6b00 7400 6900  e. .F.u.n.k.t.i.
-00001760: 6f00 6e00 6500 6e00 2000 6f00 6400 6500  o.n.e.n. .o.d.e.
-00001770: 7200 2000 4100 5000 4900 2d00 5600 6500  r. .A.P.I.-.V.e.
-00001780: 7200 7300 6900 6f00 6e00 6500 6e00 2000  r.s.i.o.n.e.n. .
-00001790: 6100 7500 7300 7000 7200 6f00 6200 6900  a.u.s.p.r.o.b.i.
-000017a0: 6500 7200 6500 6e08 0000 0000 0600 0000  e.r.e.n.........
-000017b0: 2174 6573 7420 6e65 7720 6665 6174 7572  !test new featur
-000017c0: 6573 206f 7220 4150 4920 7665 7273 696f  es or API versio
-000017d0: 6e73 0700 0000 0743 4c49 4865 6c70 0103  ns.....CLIHelp..
-000017e0: 0000 0030 0042 0065 0073 0063 0068 0072  ...0.B.e.s.c.h.r
-000017f0: 0065 0069 0062 0065 006e 0026 0064 0065  .e.i.b.e.n.&.d.e
-00001800: 0020 004d 0065 0074 0061 0064 0061 0074  . .M.e.t.a.d.a.t
-00001810: 0065 006e 0800 0000 0006 0000 0015 2644  .e.n..........&D
-00001820: 6573 6372 6970 7469 7665 206d 6574 6164  escriptive metad
-00001830: 6174 6107 0000 000e 4465 7363 7269 7074  ata.....Descript
-00001840: 6976 6554 6162 0103 0000 0016 003c 0046  iveTab.......<.F
-00001850: 0061 0076 006f 0072 0069 0074 0065 006e  .a.v.o.r.i.t.e.n
-00001860: 003e 0800 0000 0006 0000 000c 3c66 6176  .>..........<fav
-00001870: 6f75 7269 7465 733e 0700 0000 0e44 6573  ourites>.....Des
-00001880: 6372 6970 7469 7665 5461 6201 0300 0002  criptiveTab.....
-00001890: ac00 4500 6900 6e00 6500 2000 6400 6500  ..E.i.n.e. .d.e.
-000018a0: 7400 6100 6900 6c00 6c00 6900 6500 7200  t.a.i.l.l.i.e.r.
-000018b0: 7400 6500 7200 6500 2000 7400 6500 7800  t.e.r.e. .t.e.x.
-000018c0: 7400 6c00 6900 6300 6800 6500 2000 4200  t.l.i.c.h.e. .B.
-000018d0: 6500 7300 6300 6800 7200 6500 6900 6200  e.s.c.h.r.e.i.b.
-000018e0: 7500 6e00 6700 2000 6400 6500 7300 2000  u.n.g. .d.e.s. .
-000018f0: 5a00 7700 6500 6300 6b00 7300 2000 7500  Z.w.e.c.k.s. .u.
-00001900: 6e00 6400 2000 6400 6500 7200 2000 4200  n.d. .d.e.r. .B.
-00001910: 6500 6400 6500 7500 7400 7500 6e00 6700  e.d.e.u.t.u.n.g.
-00001920: 2000 6500 6900 6e00 6500 7300 2000 4200   .e.i.n.e.s. .B.
-00001930: 6900 6c00 6400 6500 7300 2c00 2000 6400  i.l.d.e.s.,. .d.
-00001940: 6900 6500 2000 6400 6900 6500 2000 6400  i.e. .d.i.e. .d.
-00001950: 7500 7200 6300 6800 2000 6400 6900 6500  u.r.c.h. .d.i.e.
-00001960: 2000 4500 6900 6700 6500 6e00 7300 6300   .E.i.g.e.n.s.c.
-00001970: 6800 6100 6600 7400 2000 4100 6c00 7400  h.a.f.t. .A.l.t.
-00001980: 2d00 5400 6500 7800 7400 2000 2800 4200  -.T.e.x.t. .(.B.
-00001990: 6100 7200 7200 6900 6500 7200 6500 6600  a.r.r.i.e.r.e.f.
-000019a0: 7200 6500 6900 6800 6500 6900 7400 2900  r.e.i.h.e.i.t.).
-000019b0: 2000 6200 6500 7200 6500 6900 7400 6700   .b.e.r.e.i.t.g.
-000019c0: 6500 7300 7400 6500 6c00 6c00 7400 6500  e.s.t.e.l.l.t.e.
-000019d0: 6e00 2000 4900 6e00 6600 6f00 7200 6d00  n. .I.n.f.o.r.m.
-000019e0: 6100 7400 6900 6f00 6e00 6500 6e00 2000  a.t.i.o.n.e.n. .
-000019f0: 7700 6500 6900 7400 6500 7200 2000 6100  w.e.i.t.e.r. .a.
-00001a00: 7500 7300 6600 fc00 6800 7200 7400 2e00  u.s.f...h.r.t...
-00001a10: 2000 4400 6900 6500 7300 6500 2000 4500   .D.i.e.s.e. .E.
-00001a20: 6900 6700 6500 6e00 7300 6300 6800 6100  i.g.e.n.s.c.h.a.
-00001a30: 6600 7400 2000 6800 6100 7400 2000 6b00  f.t. .h.a.t. .k.
-00001a40: 6500 6900 6e00 6500 2000 5a00 6500 6900  e.i.n.e. .Z.e.i.
-00001a50: 6300 6800 6500 6e00 6200 6500 6700 7200  c.h.e.n.b.e.g.r.
-00001a60: 6500 6e00 7a00 7500 6e00 6700 2000 7500  e.n.z.u.n.g. .u.
-00001a70: 6e00 6400 2000 6900 7300 7400 2000 6e00  n.d. .i.s.t. .n.
-00001a80: 6900 6300 6800 7400 2000 6500 7200 6600  i.c.h.t. .e.r.f.
-00001a90: 6f00 7200 6400 6500 7200 6c00 6900 6300  o.r.d.e.r.l.i.c.
-00001aa0: 6800 2c00 2000 7700 6500 6e00 6e00 2000  h.,. .w.e.n.n. .
-00001ab0: 6400 6100 7300 2000 4600 6500 6c00 6400  d.a.s. .F.e.l.d.
-00001ac0: 2000 4100 6c00 7400 2d00 5400 6500 7800   .A.l.t.-.T.e.x.
-00001ad0: 7400 2000 2800 4200 6100 7200 7200 6900  t. .(.B.a.r.r.i.
-00001ae0: 6500 7200 6500 6600 7200 6500 6900 6800  e.r.e.f.r.e.i.h.
-00001af0: 6500 6900 7400 2900 2000 6400 6100 7300  e.i.t.). .d.a.s.
-00001b00: 2000 4200 6900 6c00 6400 2000 6100 7500   .B.i.l.d. .a.u.
-00001b10: 7300 7200 6500 6900 6300 6800 6500 6e00  s.r.e.i.c.h.e.n.
-00001b20: 6400 2000 6200 6500 7300 6300 6800 7200  d. .b.e.s.c.h.r.
-00001b30: 6500 6900 6200 7400 2e00 2e00 2e08 0000  e.i.b.t.........
-00001b40: 0000 0600 0001 3041 206d 6f72 6520 6465  ......0A more de
-00001b50: 7461 696c 6564 2074 6578 7475 616c 2064  tailed textual d
-00001b60: 6573 6372 6970 7469 6f6e 206f 6620 7468  escription of th
-00001b70: 6520 7075 7270 6f73 6520 616e 6420 6d65  e purpose and me
-00001b80: 616e 696e 6720 6f66 2061 6e20 696d 6167  aning of an imag
-00001b90: 6520 7468 6174 2065 6c61 626f 7261 7465  e that elaborate
-00001ba0: 7320 6f6e 2074 6865 2069 6e66 6f72 6d61  s on the informa
-00001bb0: 7469 6f6e 2070 726f 7669 6465 6420 6279  tion provided by
-00001bc0: 2074 6865 2041 6c74 2054 6578 7420 2841   the Alt Text (A
-00001bd0: 6363 6573 7369 6269 6c69 7479 2920 7072  ccessibility) pr
-00001be0: 6f70 6572 7479 2e20 5468 6973 2070 726f  operty. This pro
-00001bf0: 7065 7274 7920 646f 6573 206e 6f74 2068  perty does not h
-00001c00: 6176 6520 6120 6368 6172 6163 7465 7220  ave a character 
-00001c10: 6c69 6d69 7461 7469 6f6e 2061 6e64 2069  limitation and i
-00001c20: 7320 6e6f 7420 7265 7175 6972 6564 2069  s not required i
-00001c30: 6620 7468 6520 416c 7420 5465 7874 2028  f the Alt Text (
-00001c40: 4163 6365 7373 6962 696c 6974 7929 2066  Accessibility) f
-00001c50: 6965 6c64 2073 7566 6669 6369 656e 746c  ield sufficientl
-00001c60: 7920 6465 7363 7269 6265 7320 7468 6520  y describes the 
-00001c70: 696d 6167 652e 2e07 0000 000e 4465 7363  image.......Desc
-00001c80: 7269 7074 6976 6554 6162 0103 0000 0036  riptiveTab.....6
-00001c90: 0041 006c 0074 002d 0054 0065 0078 0074  .A.l.t.-.T.e.x.t
-00001ca0: 0020 0028 0042 0061 0072 0072 0069 0065  . .(.B.a.r.r.i.e
-00001cb0: 0072 0065 0066 0072 0065 0069 0068 0065  .r.e.f.r.e.i.h.e
-00001cc0: 0069 0074 0029 0800 0000 0006 0000 0018  .i.t.)..........
-00001cd0: 416c 7420 5465 7874 2028 4163 6365 7373  Alt Text (Access
-00001ce0: 6962 696c 6974 7929 0700 0000 0e44 6573  ibility).....Des
-00001cf0: 6372 6970 7469 7665 5461 6201 0300 0000  criptiveTab.....
-00001d00: 1800 4200 6500 7300 6300 6800 7200 6500  ..B.e.s.c.h.r.e.
-00001d10: 6900 6200 7500 6e00 6708 0000 0000 0600  i.b.u.n.g.......
-00001d20: 0000 1544 6573 6372 6970 7469 6f6e 202f  ...Description /
-00001d30: 2043 6170 7469 6f6e 0700 0000 0e44 6573   Caption.....Des
-00001d40: 6372 6970 7469 7665 5461 6201 0300 0001  criptiveTab.....
-00001d50: b000 4700 6500 6200 6500 6e00 2000 5300  ..G.e.b.e.n. .S.
-00001d60: 6900 6500 2000 6500 6900 6e00 6500 2020  i.e. .e.i.n.e.  
-00001d70: 1e00 4200 6900 6c00 6400 7500 6e00 7400  ..B.i.l.d.u.n.t.
-00001d80: 6500 7200 7300 6300 6800 7200 6900 6600  e.r.s.c.h.r.i.f.
-00001d90: 7420 1c00 2000 6500 6900 6e00 2c00 2000  t .. .e.i.n.,. .
-00001da0: 6400 6900 6500 2000 6400 6100 7300 2000  d.i.e. .d.a.s. .
-00001db0: 5700 6500 7200 2c00 2000 5700 6100 7300  W.e.r.,. .W.a.s.
-00001dc0: 2000 7500 6e00 6400 2000 5700 6100 7200   .u.n.d. .W.a.r.
-00001dd0: 7500 6d00 2000 6400 6500 7300 2000 4700  u.m. .d.e.s. .G.
-00001de0: 6500 7300 6300 6800 6500 6800 6500 6e00  e.s.c.h.e.h.e.n.
-00001df0: 7300 2000 6100 7500 6600 2000 6400 6900  s. .a.u.f. .d.i.
-00001e00: 6500 7300 6500 6d00 2000 4200 6900 6c00  e.s.e.m. .B.i.l.
-00001e10: 6400 2000 6200 6500 7300 6300 6800 7200  d. .b.e.s.c.h.r.
-00001e20: 6500 6900 6200 7400 2c00 2000 4400 6900  e.i.b.t.,. .D.i.
-00001e30: 6500 7300 2000 6b00 6100 6e00 6e00 2000  e.s. .k.a.n.n. .
-00001e40: 4e00 6100 6d00 6500 6e00 2000 7600 6f00  N.a.m.e.n. .v.o.
-00001e50: 6e00 2000 5000 6500 7200 7300 6f00 6e00  n. .P.e.r.s.o.n.
-00001e60: 6500 6e00 2000 7500 6e00 6400 2f00 6f00  e.n. .u.n.d./.o.
-00001e70: 6400 6500 7200 2000 6900 6800 7200 6500  d.e.r. .i.h.r.e.
-00001e80: 2000 5200 6f00 6c00 6c00 6500 2000 6900   .R.o.l.l.e. .i.
-00001e90: 6e00 2000 6400 6500 7200 2000 4800 6100  n. .d.e.r. .H.a.
-00001ea0: 6e00 6400 6c00 7500 6e00 6700 2c00 2000  n.d.l.u.n.g.,. .
-00001eb0: 6400 6900 6500 2000 6100 7500 6600 2000  d.i.e. .a.u.f. .
-00001ec0: 6400 6500 6d00 2000 4200 6900 6c00 6400  d.e.m. .B.i.l.d.
-00001ed0: 2000 7300 7400 6100 7400 7400 6600 6900   .s.t.a.t.t.f.i.
-00001ee0: 6e00 6400 6500 7400 2c00 2000 6200 6500  n.d.e.t.,. .b.e.
-00001ef0: 6900 6e00 6800 6100 6c00 7400 6500 6e00  i.n.h.a.l.t.e.n.
-00001f00: 2e08 0000 0000 0600 0000 c245 6e74 6572  ...........Enter
-00001f10: 2061 2022 6361 7074 696f 6e22 2064 6573   a "caption" des
-00001f20: 6372 6962 696e 6720 7468 6520 7768 6f2c  cribing the who,
-00001f30: 2077 6861 742c 2061 6e64 2077 6879 206f   what, and why o
-00001f40: 6620 7768 6174 2069 7320 6861 7070 656e  f what is happen
-00001f50: 696e 6720 696e 2074 6869 7320 696d 6167  ing in this imag
-00001f60: 652c 2074 6869 7320 6d69 6768 7420 696e  e, this might in
-00001f70: 636c 7564 6520 6e61 6d65 7320 6f66 2070  clude names of p
-00001f80: 656f 706c 652c 2061 6e64 2f6f 7220 7468  eople, and/or th
-00001f90: 6569 7220 726f 6c65 2069 6e20 7468 6520  eir role in the 
-00001fa0: 6163 7469 6f6e 2074 6861 7420 6973 2074  action that is t
-00001fb0: 616b 696e 6720 706c 6163 6520 7769 7468  aking place with
-00001fc0: 696e 2074 6865 2069 6d61 6765 2e07 0000  in the image....
-00001fd0: 000e 4465 7363 7269 7074 6976 6554 6162  ..DescriptiveTab
-00001fe0: 0103 0000 00b0 0047 0065 0062 0065 006e  .......G.e.b.e.n
-00001ff0: 0020 0053 0069 0065 0020 0065 0069 006e  . .S.i.e. .e.i.n
-00002000: 0065 0020 006b 0075 0072 007a 0065 0020  .e. .k.u.r.z.e. 
-00002010: 0076 0065 0072 00f6 0066 0066 0065 006e  .v.e.r...f.f.e.n
-00002020: 0074 006c 0069 0063 0068 0075 006e 0067  .t.l.i.c.h.u.n.g
-00002030: 0073 0066 00e4 0068 0069 0067 0065 0020  .s.f...h.i.g.e. 
-00002040: 005a 0075 0073 0061 006d 006d 0065 006e  .Z.u.s.a.m.m.e.n
-00002050: 0066 0061 0073 0073 0075 006e 0067 0020  .f.a.s.s.u.n.g. 
-00002060: 0064 0065 0073 0020 0049 006e 0068 0061  .d.e.s. .I.n.h.a
-00002070: 006c 0074 0073 0020 0064 0065 0073 0020  .l.t.s. .d.e.s. 
-00002080: 0042 0069 006c 0064 0065 0073 0020 0065  .B.i.l.d.e.s. .e
-00002090: 0069 006e 002e 0800 0000 0006 0000 004b  .i.n...........K
-000020a0: 456e 7465 7220 6120 6272 6965 6620 7075  Enter a brief pu
-000020b0: 626c 6973 6861 626c 6520 7379 6e6f 7073  blishable synops
-000020c0: 6973 206f 7220 7375 6d6d 6172 7920 6f66  is or summary of
-000020d0: 2074 6865 2063 6f6e 7465 6e74 7320 6f66   the contents of
-000020e0: 2074 6865 2069 6d61 6765 2e07 0000 000e   the image......
-000020f0: 4465 7363 7269 7074 6976 6554 6162 0103  DescriptiveTab..
-00002100: 0000 00de 0047 0065 0062 0065 006e 0020  .....G.e.b.e.n. 
-00002110: 0053 0069 0065 0020 0065 0069 006e 0065  .S.i.e. .e.i.n.e
-00002120: 006e 0020 006b 0075 0072 007a 0065 006e  .n. .k.u.r.z.e.n
-00002130: 002c 0020 0076 0065 0072 0062 0061 006c  .,. .v.e.r.b.a.l
-00002140: 0065 006e 0020 0075 006e 0064 0020 006d  .e.n. .u.n.d. .m
-00002150: 0065 006e 0073 0063 0068 0065 006e 006c  .e.n.s.c.h.e.n.l
-00002160: 0065 0073 0062 0061 0072 0065 006e 0020  .e.s.b.a.r.e.n. 
-00002170: 004e 0061 006d 0065 006e 0020 0066 00fc  .N.a.m.e.n. .f..
-00002180: 0072 0020 0064 0061 0073 0020 0042 0069  .r. .d.a.s. .B.i
-00002190: 006c 0064 0020 0065 0069 006e 002c 0020  .l.d. .e.i.n.,. 
-000021a0: 0064 0065 0072 0020 0061 0075 0063 0068  .d.e.r. .a.u.c.h
-000021b0: 0020 0064 0065 0072 0020 0044 0061 0074  . .d.e.r. .D.a.t
-000021c0: 0065 0069 006e 0061 006d 0065 0020 0073  .e.i.n.a.m.e. .s
-000021d0: 0065 0069 006e 0020 006b 0061 006e 006e  .e.i.n. .k.a.n.n
-000021e0: 002e 0800 0000 0006 0000 0056 456e 7465  ...........VEnte
-000021f0: 7220 6120 7368 6f72 7420 7665 7262 616c  r a short verbal
-00002200: 2061 6e64 2068 756d 616e 2072 6561 6461   and human reada
-00002210: 626c 6520 6e61 6d65 2066 6f72 2074 6865  ble name for the
-00002220: 2069 6d61 6765 2c20 7468 6973 206d 6179   image, this may
-00002230: 2062 6520 7468 6520 6669 6c65 206e 616d   be the file nam
-00002240: 652e 0700 0000 0e44 6573 6372 6970 7469  e......Descripti
-00002250: 7665 5461 6201 0300 0001 3800 4700 6500  veTab.....8.G.e.
-00002260: 6200 6500 6e00 2000 5300 6900 6500 2000  b.e.n. .S.i.e. .
-00002270: 6500 6900 6e00 6500 2000 6200 6500 6c00  e.i.n.e. .b.e.l.
-00002280: 6900 6500 6200 6900 6700 6500 2000 4100  i.e.b.i.g.e. .A.
-00002290: 6e00 7a00 6100 6800 6c00 2000 7600 6f00  n.z.a.h.l. .v.o.
-000022a0: 6e00 2000 5300 6300 6800 6c00 fc00 7300  n. .S.c.h.l...s.
-000022b0: 7300 6500 6c00 7700 f600 7200 7400 6500  s.e.l.w...r.t.e.
-000022c0: 7200 6e00 2c00 2000 4200 6500 6700 7200  r.n.,. .B.e.g.r.
-000022d0: 6900 6600 6600 6500 6e00 2000 6f00 6400  i.f.f.e.n. .o.d.
-000022e0: 6500 7200 2000 5000 6800 7200 6100 7300  e.r. .P.h.r.a.s.
-000022f0: 6500 6e00 2000 6500 6900 6e00 2c00 2000  e.n. .e.i.n.,. .
-00002300: 6400 6900 6500 2000 6400 6100 7300 2000  d.i.e. .d.a.s. .
-00002310: 5400 6800 6500 6d00 6100 2000 6400 6500  T.h.e.m.a. .d.e.
-00002320: 7300 2000 4200 6900 6c00 6400 6500 7300  s. .B.i.l.d.e.s.
-00002330: 2000 6100 7500 7300 6400 7200 fc00 6300   .a.u.s.d.r...c.
-00002340: 6b00 6500 6e00 2000 7300 6f00 6c00 6c00  k.e.n. .s.o.l.l.
-00002350: 6500 6e00 2e00 2000 5400 7200 6500 6e00  e.n... .T.r.e.n.
-00002360: 6e00 6500 6e00 2000 5300 6900 6500 2000  n.e.n. .S.i.e. .
-00002370: 7300 6900 6500 2000 6d00 6900 7400 2000  s.i.e. .m.i.t. .
-00002380: 3b00 2d00 5a00 6500 6900 6300 6800 6500  ;.-.Z.e.i.c.h.e.
-00002390: 6e00 2e08 0000 0000 0600 0000 8245 6e74  n............Ent
-000023a0: 6572 2061 6e79 206e 756d 6265 7220 6f66  er any number of
-000023b0: 206b 6579 776f 7264 732c 2074 6572 6d73   keywords, terms
-000023c0: 206f 7220 7068 7261 7365 7320 7573 6564   or phrases used
-000023d0: 2074 6f20 6578 7072 6573 7320 7468 6520   to express the 
-000023e0: 7375 626a 6563 7420 6d61 7474 6572 2069  subject matter i
-000023f0: 6e20 7468 6520 696d 6167 652e 2053 6570  n the image. Sep
-00002400: 6172 6174 6520 7468 656d 2077 6974 6820  arate them with 
-00002410: 223b 2220 6368 6172 6163 7465 7273 2e07  ";" characters..
-00002420: 0000 000e 4465 7363 7269 7074 6976 6554  ....DescriptiveT
-00002430: 6162 0103 0000 019a 0047 0065 0062 0065  ab.......G.e.b.e
-00002440: 006e 0020 0053 0069 0065 0020 0065 0069  .n. .S.i.e. .e.i
-00002450: 006e 0065 006e 0020 0054 0065 0078 0074  .n.e.n. .T.e.x.t
-00002460: 0020 0065 0069 006e 002c 0020 0064 0065  . .e.i.n.,. .d.e
-00002470: 0072 0020 0064 0061 0073 0020 0041 0075  .r. .d.a.s. .A.u
-00002480: 0073 0073 0065 0068 0065 006e 0020 0064  .s.s.e.h.e.n. .d
-00002490: 0065 0073 0020 0042 0069 006c 0064 0065  .e.s. .B.i.l.d.e
-000024a0: 0073 0020 0061 0075 0073 0020 0065 0069  .s. .a.u.s. .e.i
-000024b0: 006e 0065 0072 0020 0076 0069 0073 0075  .n.e.r. .v.i.s.u
-000024c0: 0065 006c 006c 0065 006e 0020 0050 0065  .e.l.l.e.n. .P.e
-000024d0: 0072 0073 0070 0065 006b 0074 0069 0076  .r.s.p.e.k.t.i.v
-000024e0: 0065 0020 0062 0065 0073 0063 0068 0072  .e. .b.e.s.c.h.r
-000024f0: 0065 0069 0062 0074 002c 0020 0075 006e  .e.i.b.t.,. .u.n
-00002500: 0064 0020 006b 006f 006e 007a 0065 006e  .d. .k.o.n.z.e.n
-00002510: 0074 0072 0069 0065 0072 0065 006e 0020  .t.r.i.e.r.e.n. 
-00002520: 0053 0069 0065 0020 0073 0069 0063 0068  .S.i.e. .s.i.c.h
-00002530: 0020 0064 0061 0062 0065 0069 0020 0061  . .d.a.b.e.i. .a
-00002540: 0075 0066 0020 0044 0065 0074 0061 0069  .u.f. .D.e.t.a.i
-00002550: 006c 0073 002c 0020 0064 0069 0065 0020  .l.s.,. .d.i.e. 
-00002560: 0066 00fc 0072 0020 0064 0065 006e 0020  .f...r. .d.e.n. 
-00002570: 005a 0077 0065 0063 006b 0020 0075 006e  .Z.w.e.c.k. .u.n
-00002580: 0064 0020 0064 0069 0065 0020 0042 0065  .d. .d.i.e. .B.e
-00002590: 0064 0065 0075 0074 0075 006e 0067 0020  .d.e.u.t.u.n.g. 
-000025a0: 0064 0065 0073 0020 0042 0069 006c 0064  .d.e.s. .B.i.l.d
-000025b0: 0065 0073 0020 0072 0065 006c 0065 0076  .e.s. .r.e.l.e.v
-000025c0: 0061 006e 0074 0020 0073 0069 006e 0064  .a.n.t. .s.i.n.d
-000025d0: 002e 0800 0000 0006 0000 009b 456e 7465  ............Ente
-000025e0: 7220 7465 7874 2064 6573 6372 6962 696e  r text describin
-000025f0: 6720 7468 6520 6170 7065 6172 616e 6365  g the appearance
-00002600: 206f 6620 7468 6520 696d 6167 6520 6672   of the image fr
-00002610: 6f6d 2061 2076 6973 7561 6c20 7065 7273  om a visual pers
-00002620: 7065 6374 6976 652c 2066 6f63 7573 696e  pective, focusin
-00002630: 6720 6f6e 2064 6574 6169 6c73 2074 6861  g on details tha
-00002640: 7420 6172 6520 7265 6c65 7661 6e74 2074  t are relevant t
-00002650: 6f20 7468 6520 7075 7270 6f73 6520 616e  o the purpose an
-00002660: 6420 6d65 616e 696e 6720 6f66 2074 6865  d meaning of the
-00002670: 2069 6d61 6765 2e07 0000 000e 4465 7363   image......Desc
-00002680: 7269 7074 6976 6554 6162 0103 0000 0054  riptiveTab.....T
-00002690: 0045 0072 0077 0065 0069 0074 0065 0072  .E.r.w.e.i.t.e.r
-000026a0: 0074 0065 0020 0042 0065 0073 0063 0068  .t.e. .B.e.s.c.h
-000026b0: 0072 0065 0069 0062 0075 006e 0067 0020  .r.e.i.b.u.n.g. 
-000026c0: 0028 0042 0061 0072 0072 0069 0065 0072  .(.B.a.r.r.i.e.r
-000026d0: 0065 0066 0072 0065 0069 0068 0065 0069  .e.f.r.e.i.h.e.i
-000026e0: 0074 0029 0800 0000 0006 0000 0024 4578  .t.).........$Ex
-000026f0: 7465 6e64 6564 2044 6573 6372 6970 7469  tended Descripti
-00002700: 6f6e 2028 4163 6365 7373 6962 696c 6974  on (Accessibilit
-00002710: 7929 0700 0000 0e44 6573 6372 6970 7469  y).....Descripti
-00002720: 7665 5461 6201 0300 0000 1600 dc00 6200  veTab.........b.
-00002730: 6500 7200 7300 6300 6800 7200 6900 6600  e.r.s.c.h.r.i.f.
-00002740: 7408 0000 0000 0600 0000 0848 6561 646c  t..........Headl
-00002750: 696e 6507 0000 000e 4465 7363 7269 7074  ine.....Descript
-00002760: 6976 6554 6162 0103 0000 001e 0053 0063  iveTab.......S.c
-00002770: 0068 006c 00fc 0073 0073 0065 006c 0077  .h.l...s.s.e.l.w
-00002780: 00f6 0072 0074 0065 0072 0800 0000 0006  ...r.t.e.r......
-00002790: 0000 0008 4b65 7977 6f72 6473 0700 0000  ....Keywords....
-000027a0: 0e44 6573 6372 6970 7469 7665 5461 6201  .DescriptiveTab.
-000027b0: 0300 0000 1200 4200 6500 7700 6500 7200  ......B.e.w.e.r.
-000027c0: 7400 7500 6e00 6708 0000 0000 0600 0000  t.u.n.g.........
-000027d0: 0652 6174 696e 6707 0000 000e 4465 7363  .Rating.....Desc
-000027e0: 7269 7074 6976 6554 6162 0103 0000 0024  riptiveTab.....$
-000027f0: 0054 0069 0074 0065 006c 0020 002f 0020  .T.i.t.e.l. ./. 
-00002800: 004f 0062 006a 0065 006b 0074 006e 0061  .O.b.j.e.k.t.n.a
-00002810: 006d 0065 0800 0000 0006 0000 0013 5469  .m.e..........Ti
-00002820: 746c 6520 2f20 4f62 6a65 6374 204e 616d  tle / Object Nam
-00002830: 6507 0000 000e 4465 7363 7269 7074 6976  e.....Descriptiv
-00002840: 6554 6162 0103 0000 0018 007a 0075 0072  eTab.......z.u.r
-00002850: 00fc 0063 006b 0077 0065 0069 0073 0065  ...c.k.w.e.i.s.e
-00002860: 006e 0800 0000 0006 0000 0006 7265 6a65  .n..........reje
-00002870: 6374 0700 0000 0e44 6573 6372 6970 7469  ct.....Descripti
-00002880: 7665 5461 6201 0300 0000 1c00 2800 7700  veTab.......(.w.
-00002890: 6500 6e00 6e00 2000 6d00 f600 6700 6c00  e.n.n. .m...g.l.
-000028a0: 6900 6300 6800 2908 0000 0000 0600 0000  i.c.h.).........
-000028b0: 0f28 7768 656e 2070 6f73 7369 626c 6529  .(when possible)
-000028c0: 0700 0000 0c45 6469 7453 6574 7469 6e67  .....EditSetting
-000028d0: 7301 0300 0000 1e00 4900 6d00 6d00 6500  s.......I.m.m.e.
-000028e0: 7200 2000 6500 7200 7300 7400 6500 6c00  r. .e.r.s.t.e.l.
-000028f0: 6c00 6500 6e08 0000 0000 0600 0000 0d41  l.e.n..........A
-00002900: 6c77 6179 7320 6372 6561 7465 0700 0000  lways create....
-00002910: 0c45 6469 7453 6574 7469 6e67 7301 0300  .EditSettings...
-00002920: 0000 1a00 4900 6d00 6d00 6500 7200 2000  ....I.m.m.e.r. .
-00002930: 6c00 f600 7300 6300 6800 6500 6e08 0000  l...s.c.h.e.n...
-00002940: 0000 0600 0000 0d41 6c77 6179 7320 6465  .......Always de
-00002950: 6c65 7465 0700 0000 0c45 6469 7453 6574  lete.....EditSet
-00002960: 7469 6e67 7301 0300 0000 1e00 4900 6d00  tings.......I.m.
-00002970: 6d00 6500 7200 2000 7300 6300 6800 7200  m.e.r. .s.c.h.r.
-00002980: 6500 6900 6200 6500 6e08 0000 0000 0600  e.i.b.e.n.......
-00002990: 0000 0c41 6c77 6179 7320 7772 6974 6507  ...Always write.
-000029a0: 0000 000c 4564 6974 5365 7474 696e 6773  ....EditSettings
-000029b0: 0103 0000 0034 0045 0072 0073 0074 0065  .....4.E.r.s.t.e
-000029c0: 006c 006c 0065 006e 002c 0020 0066 0061  .l.l.e.n.,. .f.a
-000029d0: 006c 006c 0073 0020 006e 006f 0074 0077  .l.l.s. .n.o.t.w
-000029e0: 0065 006e 0064 0069 0067 0800 0000 0006  .e.n.d.i.g......
-000029f0: 0000 0013 4372 6561 7465 2069 6620 6e65  ....Create if ne
-00002a00: 6365 7373 6172 7907 0000 000c 4564 6974  cessary.....Edit
-00002a10: 5365 7474 696e 6773 0103 0000 002a 004c  Settings.....*.L
-00002a20: 00f6 0073 0063 0068 0065 006e 002c 0020  ...s.c.h.e.n.,. 
-00002a30: 0077 0065 006e 006e 0020 006d 00f6 0067  .w.e.n.n. .m...g
-00002a40: 006c 0069 0063 0068 0800 0000 0006 0000  .l.i.c.h........
-00002a50: 0014 4465 6c65 7465 2077 6865 6e20 706f  ..Delete when po
-00002a60: 7373 6962 6c65 0700 0000 0c45 6469 7453  ssible.....EditS
-00002a70: 6574 7469 6e67 7301 0300 0000 2200 4400  ettings.....".D.
-00002a80: 6100 7400 6500 6900 2d00 5a00 6500 6900  a.t.e.i.-.Z.e.i.
-00002a90: 7400 7300 7400 6500 6d00 7000 6500 6c08  t.s.t.e.m.p.e.l.
-00002aa0: 0000 0000 0600 0000 0f46 696c 6520 7469  .........File ti
-00002ab0: 6d65 7374 616d 7073 0700 0000 0c45 6469  mestamps.....Edi
-00002ac0: 7453 6574 7469 6e67 7301 0300 0000 2400  tSettings.....$.
-00002ad0: 4900 5000 5400 4300 2d00 4900 4900 4d00  I.P.T.C.-.I.I.M.
-00002ae0: 2d00 4d00 6500 7400 6100 6400 6100 7400  -.M.e.t.a.d.a.t.
-00002af0: 6500 6e08 0000 0000 0600 0000 1149 5054  e.n..........IPT
-00002b00: 432d 4949 4d20 6d65 7461 6461 7461 0700  C-IIM metadata..
-00002b10: 0000 0c45 6469 7453 6574 7469 6e67 7301  ...EditSettings.
-00002b20: 0300 0000 2800 4f00 7200 6900 6700 6900  ....(.O.r.i.g.i.
-00002b30: 6e00 6100 6c00 2000 6200 6500 6900 6200  n.a.l. .b.e.i.b.
-00002b40: 6500 6800 6100 6c00 7400 6500 6e08 0000  e.h.a.l.t.e.n...
-00002b50: 0000 0600 0000 0d4b 6565 7020 6f72 6967  .......Keep orig
-00002b60: 696e 616c 0700 0000 0c45 6469 7453 6574  inal.....EditSet
-00002b70: 7469 6e67 7301 0300 0000 2c00 5000 6800  tings.....,.P.h.
-00002b80: 6f00 7400 6900 6e00 6900 3a00 2000 4500  o.t.i.n.i.:. .E.
-00002b90: 6900 6e00 7300 7400 6500 6c00 6c00 7500  i.n.s.t.e.l.l.u.
-00002ba0: 6e00 6700 6500 6e08 0000 0000 0600 0000  n.g.e.n.........
-00002bb0: 1150 686f 7469 6e69 3a20 7365 7474 696e  .Photini: settin
-00002bc0: 6773 0700 0000 0c45 6469 7453 6574 7469  gs.....EditSetti
-00002bd0: 6e67 7301 0300 0000 4600 4200 6500 6900  ngs.....F.B.e.i.
-00002be0: 6d00 2000 5300 7000 6500 6900 6300 6800  m. .S.p.e.i.c.h.
-00002bf0: 6500 7200 6e00 2000 6400 6500 7200 2000  e.r.n. .d.e.r. .
-00002c00: 4400 6100 7400 6500 6900 2000 6500 6900  D.a.t.e.i. .e.i.
-00002c10: 6e00 7300 7400 6500 6c00 6c00 6500 6e08  n.s.t.e.l.l.e.n.
-00002c20: 0000 0000 0600 0000 1953 6574 2074 6f20  .........Set to 
-00002c30: 7768 656e 2066 696c 6520 6973 2073 6176  when file is sav
-00002c40: 6564 0700 0000 0c45 6469 7453 6574 7469  ed.....EditSetti
-00002c50: 6e67 7301 0300 0000 5600 4500 6900 6e00  ngs.....V.E.i.n.
-00002c60: 7300 7400 6500 6c00 6c00 6500 6e00 2c00  s.t.e.l.l.e.n.,.
-00002c70: 2000 7700 6100 6e00 6e00 2000 6400 6100   .w.a.n.n. .d.a.
-00002c80: 7300 2000 4600 6f00 7400 6f00 2000 6100  s. .F.o.t.o. .a.
-00002c90: 7500 6600 6700 6500 6e00 6f00 6d00 6d00  u.f.g.e.n.o.m.m.
-00002ca0: 6500 6e00 2000 7700 7500 7200 6400 6508  e.n. .w.u.r.d.e.
-00002cb0: 0000 0000 0600 0000 1b53 6574 2074 6f20  .........Set to 
-00002cc0: 7768 656e 2070 686f 746f 2077 6173 2074  when photo was t
-00002cd0: 616b 656e 0700 0000 0c45 6469 7453 6574  aken.....EditSet
-00002ce0: 7469 6e67 7301 0300 0000 3e00 4900 5000  tings.....>.I.P.
-00002cf0: 5400 4300 2d00 4900 4900 4d00 2d00 4c00  T.C.-.I.I.M.-.L.
-00002d00: e400 6e00 6700 6500 6e00 6700 7200 6500  ..n.g.e.n.g.r.e.
-00002d10: 6e00 7a00 6500 6e00 2000 6100 6e00 7a00  n.z.e.n. .a.n.z.
-00002d20: 6500 6900 6700 6500 6e08 0000 0000 0600  e.i.g.e.n.......
-00002d30: 0000 1b53 686f 7720 4950 5443 2d49 494d  ...Show IPTC-IIM
-00002d40: 206c 656e 6774 6820 6c69 6d69 7473 0700   length limits..
-00002d50: 0000 0c45 6469 7453 6574 7469 6e67 7301  ...EditSettings.
-00002d60: 0300 0000 1e00 5300 6900 6400 6500 6300  ......S.i.d.e.c.
-00002d70: 6100 7200 2d00 4400 6100 7400 6500 6900  a.r.-.D.a.t.e.i.
-00002d80: 6500 6e08 0000 0000 0600 0000 0d53 6964  e.n..........Sid
-00002d90: 6563 6172 2066 696c 6573 0700 0000 0c45  ecar files.....E
-00002da0: 6469 7453 6574 7469 6e67 7301 0300 0000  ditSettings.....
-00002db0: 3200 5300 6300 6800 7200 6500 6900 6200  2.S.c.h.r.e.i.b.
-00002dc0: 6500 6e00 2c00 2000 7700 6500 6e00 6e00  e.n.,. .w.e.n.n.
-00002dd0: 2000 7600 6f00 7200 6800 6100 6e00 6400   .v.o.r.h.a.n.d.
-00002de0: 6500 6e08 0000 0000 0600 0000 0f57 7269  e.n..........Wri
-00002df0: 7465 2069 6620 6578 6973 7473 0700 0000  te if exists....
-00002e00: 0c45 6469 7453 6574 7469 6e67 7301 0300  .EditSettings...
-00002e10: 0000 2c00 4900 6e00 2000 4200 6900 6c00  ..,.I.n. .B.i.l.
-00002e20: 6400 6400 6100 7400 6500 6900 2000 7300  d.d.a.t.e.i. .s.
-00002e30: 6300 6800 7200 6500 6900 6200 6500 6e08  c.h.r.e.i.b.e.n.
-00002e40: 0000 0000 0600 0000 1357 7269 7465 2074  .........Write t
-00002e50: 6f20 696d 6167 6520 6669 6c65 0700 0000  o image file....
-00002e60: 0c45 6469 7453 6574 7469 6e67 7301 0300  .EditSettings...
-00002e70: 0000 2200 2600 4600 6c00 6900 6300 6b00  ..".&.F.l.i.c.k.
-00002e80: 7200 2000 6800 6f00 6300 6800 6c00 6100  r. .h.o.c.h.l.a.
-00002e90: 6400 6500 6e08 0000 0000 0600 0000 0e26  d.e.n..........&
-00002ea0: 466c 6963 6b72 2075 706c 6f61 6407 0000  Flickr upload...
-00002eb0: 0009 466c 6963 6b72 5461 6201 0300 0000  ..FlickrTab.....
-00002ec0: 6600 4100 6c00 6200 7500 6d00 2000 7700  f.A.l.b.u.m. .w.
-00002ed0: 6900 7200 6400 2000 6500 7200 7300 7400  i.r.d. .e.r.s.t.
-00002ee0: 6500 6c00 6c00 7400 2c00 2000 7700 6500  e.l.l.t.,. .w.e.
-00002ef0: 6e00 6e00 2000 4200 6900 6c00 6400 6500  n.n. .B.i.l.d.e.
-00002f00: 7200 2000 6800 6f00 6300 6800 6700 6500  r. .h.o.c.h.g.e.
-00002f10: 6c00 6100 6400 6500 6e00 2000 7700 7500  l.a.d.e.n. .w.u.
-00002f20: 7200 6400 6500 6e08 0000 0000 0600 0000  r.d.e.n.........
-00002f30: 2e41 6c62 756d 2077 696c 6c20 6265 2063  .Album will be c
-00002f40: 7265 6174 6564 2077 6865 6e20 7068 6f74  reated when phot
-00002f50: 6f73 2061 7265 2075 706c 6f61 6465 6407  os are uploaded.
-00002f60: 0000 0009 466c 6963 6b72 5461 6201 0300  ....FlickrTab...
-00002f70: 0000 2600 4b00 6f00 6d00 6d00 6500 6e00  ..&.K.o.m.m.e.n.
-00002f80: 7400 6100 7200 6500 2000 7a00 7500 6c00  t.a.r.e. .z.u.l.
-00002f90: 6100 7300 7300 6500 6e08 0000 0000 0600  a.s.s.e.n.......
-00002fa0: 0000 1041 6c6c 6f77 2063 6f6d 6d65 6e74  ...Allow comment
-00002fb0: 696e 6707 0000 0009 466c 6963 6b72 5461  ing.....FlickrTa
-00002fc0: 6201 0300 0000 3a00 4500 7400 6900 6b00  b.....:.E.t.i.k.
-00002fd0: 6500 7400 7400 6500 2000 7500 6e00 6400  e.t.t.e. .u.n.d.
-00002fe0: 2000 4e00 6f00 7400 6900 7a00 6500 6e00   .N.o.t.i.z.e.n.
-00002ff0: 2000 7a00 7500 6c00 6100 7300 7300 6500   .z.u.l.a.s.s.e.
-00003000: 6e08 0000 0000 0600 0000 1441 6c6c 6f77  n..........Allow
-00003010: 2074 6167 7320 616e 6420 6e6f 7465 7307   tags and notes.
-00003020: 0000 0009 466c 6963 6b72 5461 6201 0300  ....FlickrTab...
-00003030: 0000 2a00 4a00 6500 6400 6500 7300 2000  ..*.J.e.d.e.s. .
-00003040: 4600 6c00 6900 6300 6b00 7200 2d00 4d00  F.l.i.c.k.r.-.M.
-00003050: 6900 7400 6700 6c00 6900 6500 6408 0000  i.t.g.l.i.e.d...
-00003060: 0000 0600 0000 1141 6e79 2046 6c69 636b  .......Any Flick
-00003070: 7220 6d65 6d62 6572 0700 0000 0946 6c69  r member.....Fli
-00003080: 636b 7254 6162 0103 0000 0020 0041 0072  ckrTab..... .A.r
-00003090: 0074 002f 0049 006c 006c 0075 0073 0074  .t./.I.l.l.u.s.t
-000030a0: 0072 0061 0074 0069 006f 006e 0800 0000  .r.a.t.i.o.n....
-000030b0: 0006 0000 0010 4172 742f 496c 6c75 7374  ......Art/Illust
-000030c0: 7261 7469 6f6e 0700 0000 0946 6c69 636b  ration.....Flick
-000030d0: 7254 6162 0103 0000 0034 0041 006c 0062  rTab.....4.A.l.b
-000030e0: 0075 006d 006d 0069 0074 0067 006c 0069  .u.m.m.i.t.g.l.i
-000030f0: 0065 0064 0073 0063 0068 0061 0066 0074  .e.d.s.c.h.a.f.t
-00003100: 0020 00e4 006e 0064 0065 0072 006e 0800  . ...n.d.e.r.n..
-00003110: 0000 0006 0000 0017 4368 616e 6765 2061  ........Change a
-00003120: 6c62 756d 206d 656d 6265 7273 6869 7007  lbum membership.
-00003130: 0000 0009 466c 6963 6b72 5461 6201 0300  ....FlickrTab...
-00003140: 0000 2200 4900 6e00 6800 6100 6c00 7400  ..".I.n.h.a.l.t.
-00003150: 7300 7400 7900 7000 2000 e400 6e00 6400  s.t.y.p. ...n.d.
-00003160: 6500 7200 6e08 0000 0000 0600 0000 1343  e.r.n..........C
-00003170: 6861 6e67 6520 636f 6e74 656e 7420 7479  hange content ty
-00003180: 7065 0700 0000 0946 6c69 636b 7254 6162  pe.....FlickrTab
-00003190: 0103 0000 003e 0041 0075 0073 0062 006c  .....>.A.u.s.b.l
-000031a0: 0065 006e 0064 0065 006e 0020 0061 0075  .e.n.d.e.n. .a.u
-000031b0: 0073 0020 0064 0065 0072 0020 0053 0075  .s. .d.e.r. .S.u
-000031c0: 0063 0068 0065 0020 00e4 006e 0064 0065  .c.h.e. ...n.d.e
-000031d0: 0072 006e 0800 0000 0006 0000 0017 4368  .r.n..........Ch
-000031e0: 616e 6765 2068 6964 6520 6672 6f6d 2073  ange hide from s
-000031f0: 6561 7263 6807 0000 0009 466c 6963 6b72  earch.....Flickr
-00003200: 5461 6201 0300 0000 1a00 4c00 6900 7a00  Tab.......L.i.z.
-00003210: 6500 6e00 7a00 2000 e400 6e00 6400 6500  e.n.z. ...n.d.e.
-00003220: 7200 6e08 0000 0000 0600 0000 0e43 6861  r.n..........Cha
-00003230: 6e67 6520 6c69 6365 6e63 6507 0000 0009  nge licence.....
-00003240: 466c 6963 6b72 5461 6201 0300 0000 2e00  FlickrTab.......
-00003250: 5300 6900 6300 6800 6500 7200 6800 6500  S.i.c.h.e.r.h.e.
-00003260: 6900 7400 7300 7300 7400 7500 6600 6500  i.t.s.s.t.u.f.e.
-00003270: 2000 e400 6e00 6400 6500 7200 6e08 0000   ...n.d.e.r.n...
-00003280: 0000 0600 0000 1343 6861 6e67 6520 7361  .......Change sa
-00003290: 6665 7479 206c 6576 656c 0700 0000 0946  fety level.....F
-000032a0: 6c69 636b 7254 6162 0103 0000 0026 0053  lickrTab.....&.S
-000032b0: 0069 0063 0068 0074 0062 0061 0072 006b  .i.c.h.t.b.a.r.k
-000032c0: 0065 0069 0074 0020 00e4 006e 0064 0065  .e.i.t. ...n.d.e
-000032d0: 0072 006e 0800 0000 0006 0000 0016 4368  .r.n..........Ch
-000032e0: 616e 6765 2076 6965 7769 6e67 2070 7269  ange viewing pri
-000032f0: 7661 6379 0700 0000 0946 6c69 636b 7254  vacy.....FlickrT
-00003300: 6162 0103 0000 0080 00c4 006e 0064 0065  ab.........n.d.e
-00003310: 0072 006e 002c 0020 0077 0065 0072 0020  .r.n.,. .w.e.r. 
-00003320: 006b 006f 006d 006d 0065 006e 0074 0069  .k.o.m.m.e.n.t.i
-00003330: 0065 0072 0065 006e 0020 006f 0064 0065  .e.r.e.n. .o.d.e
-00003340: 0072 0020 0074 0061 0067 0067 0065 006e  .r. .t.a.g.g.e.n
-00003350: 0020 0064 0061 0072 0066 0020 0028 0075  . .d.a.r.f. .(.u
-00003360: 006e 0064 0020 0064 0069 0065 0020 0053  .n.d. .d.i.e. .S
-00003370: 0069 0063 0068 0074 0062 0061 0072 006b  .i.c.h.t.b.a.r.k
-00003380: 0065 0069 0074 0029 0800 0000 0006 0000  .e.i.t.)........
-00003390: 0033 4368 616e 6765 2077 686f 2063 616e  .3Change who can
-000033a0: 2063 6f6d 6d65 6e74 206f 7220 7461 6720   comment or tag 
-000033b0: 2861 6e64 2076 6965 7769 6e67 2070 7269  (and viewing pri
-000033c0: 7661 6379 2907 0000 0009 466c 6963 6b72  vacy).....Flickr
-000033d0: 5461 6201 0300 0000 1400 4900 6e00 6800  Tab.......I.n.h.
-000033e0: 6100 6c00 7400 7300 7400 7900 7008 0000  a.l.t.s.t.y.p...
-000033f0: 0000 0600 0000 0c43 6f6e 7465 6e74 2074  .......Content t
-00003400: 7970 6507 0000 0009 466c 6963 6b72 5461  ype.....FlickrTa
-00003410: 6201 0300 0000 1800 4200 6500 7300 6300  b.......B.e.s.c.
-00003420: 6800 7200 6500 6900 6200 7500 6e00 6708  h.r.e.i.b.u.n.g.
-00003430: 0000 0000 0600 0000 0b44 6573 6372 6970  .........Descrip
-00003440: 7469 6f6e 0700 0000 0946 6c69 636b 7254  tion.....FlickrT
-00003450: 6162 0103 0000 000e 0046 0061 006d 0069  ab.......F.a.m.i
-00003460: 006c 0069 0065 0800 0000 0006 0000 0006  .l.i.e..........
-00003470: 4661 6d69 6c79 0700 0000 0946 6c69 636b  Family.....Flick
-00003480: 7254 6162 0103 0000 000c 0046 006c 0069  rTab.......F.l.i
-00003490: 0063 006b 0072 0800 0000 0006 0000 0006  .c.k.r..........
-000034a0: 466c 6963 6b72 0700 0000 0946 6c69 636b  Flickr.....Flick
-000034b0: 7254 6162 0103 0000 000e 0046 0072 0065  rTab.......F.r.e
-000034c0: 0075 006e 0064 0065 0800 0000 0006 0000  .u.n.d.e........
-000034d0: 0007 4672 6965 6e64 7307 0000 0009 466c  ..Friends.....Fl
-000034e0: 6963 6b72 5461 6201 0300 0000 2600 4600  ickrTab.....&.F.
-000034f0: 7200 6500 7500 6e00 6400 6500 2000 7500  r.e.u.n.d.e. .u.
-00003500: 6e00 6400 2000 4600 6100 6d00 6900 6c00  n.d. .F.a.m.i.l.
-00003510: 6900 6508 0000 0000 0600 0000 1046 7269  i.e..........Fri
-00003520: 656e 6473 2026 2066 616d 696c 7907 0000  ends & family...
-00003530: 0009 466c 6963 6b72 5461 6201 0300 0000  ..FlickrTab.....
-00003540: 3000 4100 7500 7300 2000 6400 6500 7200  0.A.u.s. .d.e.r.
-00003550: 2000 5300 7500 6300 6800 6500 2000 6100   .S.u.c.h.e. .a.
-00003560: 7500 7300 6200 6c00 6500 6e00 6400 6500  u.s.b.l.e.n.d.e.
-00003570: 6e08 0000 0000 0600 0000 1048 6964 6520  n..........Hide 
-00003580: 6672 6f6d 2073 6561 7263 6807 0000 0009  from search.....
-00003590: 466c 6963 6b72 5461 6201 0300 0000 0c00  FlickrTab.......
-000035a0: 4c00 6900 7a00 6500 6e00 7a08 0000 0000  L.i.z.e.n.z.....
-000035b0: 0600 0000 074c 6963 656e 6365 0700 0000  .....Licence....
-000035c0: 0946 6c69 636b 7254 6162 0103 0000 000a  .FlickrTab......
-000035d0: 004d 00e4 00df 0069 0067 0800 0000 0006  .M.....i.g......
-000035e0: 0000 0008 4d6f 6465 7261 7465 0700 0000  ....Moderate....
-000035f0: 0946 6c69 636b 7254 6162 0103 0000 0016  .FlickrTab......
-00003600: 004e 0065 0075 0065 0073 0020 0041 006c  .N.e.u.e.s. .A.l
-00003610: 0062 0075 006d 0800 0000 0006 0000 0009  .b.u.m..........
-00003620: 4e65 7720 616c 6275 6d07 0000 0009 466c  New album.....Fl
-00003630: 6963 6b72 5461 6201 0300 0000 1c00 4e00  ickrTab.......N.
-00003640: 7500 7200 2000 6900 6300 6800 2000 7300  u.r. .i.c.h. .s.
-00003650: 6500 6c00 6200 7300 7408 0000 0000 0600  e.l.b.s.t.......
-00003660: 0000 084f 6e6c 7920 796f 7507 0000 0009  ...Only you.....
-00003670: 466c 6963 6b72 5461 6201 0300 0000 3400  FlickrTab.....4.
-00003680: 5000 6500 7200 7300 6f00 6e00 6500 6e00  P.e.r.s.o.n.e.n.
-00003690: 2c00 2000 6400 6500 6e00 6500 6e00 2000  ,. .d.e.n.e.n. .
-000036a0: 5300 6900 6500 2000 6600 6f00 6c00 6700  S.i.e. .f.o.l.g.
-000036b0: 6500 6e08 0000 0000 0600 0000 1150 656f  e.n..........Peo
-000036c0: 706c 6520 796f 7520 666f 6c6c 6f77 0700  ple you follow..
-000036d0: 0000 0946 6c69 636b 7254 6162 0103 0000  ...FlickrTab....
-000036e0: 0008 0046 006f 0074 006f 0800 0000 0006  ...F.o.t.o......
-000036f0: 0000 0005 5068 6f74 6f07 0000 0009 466c  ....Photo.....Fl
-00003700: 6963 6b72 5461 6201 0300 0000 0c00 5000  ickrTab.......P.
-00003710: 7200 6900 7600 6100 7408 0000 0000 0600  r.i.v.a.t.......
-00003720: 0000 0750 7269 7661 7465 0700 0000 0946  ...Private.....F
-00003730: 6c69 636b 7254 6162 0103 0000 0014 00d6  lickrTab........
-00003740: 0066 0066 0065 006e 0074 006c 0069 0063  .f.f.e.n.t.l.i.c
-00003750: 0068 0800 0000 0006 0000 0006 5075 626c  .h..........Publ
-00003760: 6963 0700 0000 0946 6c69 636b 7254 6162  ic.....FlickrTab
-00003770: 0103 0000 0024 004d 0065 0074 0061 0064  .....$.M.e.t.a.d
-00003780: 0061 0074 0065 006e 0020 0065 0072 0073  .a.t.e.n. .e.r.s
-00003790: 0065 0074 007a 0065 006e 0800 0000 0006  .e.t.z.e.n......
-000037a0: 0000 0010 5265 706c 6163 6520 6d65 7461  ....Replace meta
-000037b0: 6461 7461 0700 0000 0946 6c69 636b 7254  data.....FlickrT
-000037c0: 6162 0103 0000 001a 0045 0069 006e 0067  ab.......E.i.n.g
-000037d0: 0065 0073 0063 0068 0072 00e4 006e 006b  .e.s.c.h.r...n.k
-000037e0: 0074 0800 0000 0006 0000 000a 5265 7374  .t..........Rest
-000037f0: 7269 6374 6564 0700 0000 0946 6c69 636b  ricted.....Flick
-00003800: 7254 6162 0103 0000 000c 0053 0069 0063  rTab.......S.i.c
-00003810: 0068 0065 0072 0800 0000 0006 0000 0004  .h.e.r..........
-00003820: 5361 6665 0700 0000 0946 6c69 636b 7254  Safe.....FlickrT
-00003830: 6162 0103 0000 0020 0053 0069 0063 0068  ab..... .S.i.c.h
-00003840: 0065 0072 0068 0065 0069 0074 0073 0073  .e.r.h.e.i.t.s.s
-00003850: 0074 0075 0066 0065 0800 0000 0006 0000  .t.u.f.e........
-00003860: 000c 5361 6665 7479 206c 6576 656c 0700  ..Safety level..
-00003870: 0000 0946 6c69 636b 7254 6162 0103 0000  ...FlickrTab....
-00003880: 001c 0042 0069 006c 0064 0073 0063 0068  ...B.i.l.d.s.c.h
-00003890: 0069 0072 006d 0066 006f 0074 006f 0800  .i.r.m.f.o.t.o..
-000038a0: 0000 0006 0000 000a 5363 7265 656e 7368  ........Screensh
-000038b0: 6f74 0700 0000 0946 6c69 636b 7254 6162  ot.....FlickrTab
-000038c0: 0103 0000 001e 0053 0079 006e 0063 0068  .......S.y.n.c.h
-000038d0: 0072 006f 006e 0069 0073 0069 0065 0072  .r.o.n.i.s.i.e.r
-000038e0: 0065 006e 0800 0000 0006 0000 000b 5379  .e.n..........Sy
-000038f0: 6e63 6872 6f6e 6973 6507 0000 0009 466c  nchronise.....Fl
-00003900: 6963 6b72 5461 6201 0300 0000 0a00 5400  ickrTab.......T.
-00003910: 6900 7400 6500 6c08 0000 0000 0600 0000  i.t.e.l.........
-00003920: 0554 6974 6c65 0700 0000 0946 6c69 636b  .Title.....Flick
-00003930: 7254 6162 0103 0000 002a 0053 0069 0063  rTab.....*.S.i.c
-00003940: 0068 0074 0062 0061 0072 006b 0065 0069  .h.t.b.a.r.k.e.i
-00003950: 0074 0073 006f 0070 0074 0069 006f 006e  .t.s.o.p.t.i.o.n
-00003960: 0065 006e 0800 0000 0006 0000 000f 5669  .e.n..........Vi
-00003970: 6577 696e 6720 7072 6976 6163 7907 0000  ewing privacy...
-00003980: 0009 466c 6963 6b72 5461 6201 0300 0000  ..FlickrTab.....
-00003990: 2800 5600 6900 7200 7400 7500 6500 6c00  (.V.i.r.t.u.e.l.
-000039a0: 6c00 6500 2000 4600 6f00 7400 6f00 6700  l.e. .F.o.t.o.g.
-000039b0: 7200 6100 6600 6900 6508 0000 0000 0600  r.a.f.i.e.......
-000039c0: 0000 1356 6972 7475 616c 2050 686f 746f  ...Virtual Photo
-000039d0: 6772 6170 6879 0700 0000 0946 6c69 636b  graphy.....Flick
-000039e0: 7254 6162 0103 0000 0014 0041 006c 0062  rTab.......A.l.b
-000039f0: 0075 006d 0074 0069 0074 0065 006c 0800  .u.m.t.i.t.e.l..
-00003a00: 0000 0006 0000 000b 416c 6275 6d20 7469  ........Album ti
-00003a10: 746c 6507 0000 000f 476f 6f67 6c65 5068  tle.....GooglePh
-00003a20: 6f74 6f73 5461 6201 0300 0001 2200 4400  otosTab.....".D.
-00003a30: 6900 6500 2000 4400 6100 7400 6500 6900  i.e. .D.a.t.e.i.
-00003a40: 2020 1e00 7b00 6600 6900 6c00 6500 5f00    ..{.f.i.l.e._.
-00003a50: 6e00 6100 6d00 6500 7d20 1c00 2000 6900  n.a.m.e.} .. .i.
-00003a60: 7300 7400 2000 6700 7200 f600 df00 6500  s.t. .g.r.....e.
-00003a70: 7200 2000 6100 6c00 7300 2000 3200 3500  r. .a.l.s. .2.5.
-00003a80: a000 4d00 4200 2e00 2000 4800 6f00 6300  ..M.B... .H.o.c.
-00003a90: 6800 6c00 6100 6400 6500 6e00 2000 6d00  h.l.a.d.e.n. .m.
-00003aa0: 6900 7400 2000 5000 6800 6f00 7400 6900  i.t. .P.h.o.t.i.
-00003ab0: 6e00 6900 2000 7700 6900 7200 6400 2000  n.i. .w.i.r.d. .
-00003ac0: 6900 6e00 2000 6900 6800 7200 6500 6d00  i.n. .i.h.r.e.m.
-00003ad0: 2000 4700 6f00 6f00 6700 6c00 6500 2d00   .G.o.o.g.l.e.-.
-00003ae0: 4b00 6f00 6e00 7400 6f00 2000 6100 6c00  K.o.n.t.o. .a.l.
-00003af0: 7300 2000 6200 6500 6c00 6500 6700 7400  s. .b.e.l.e.g.t.
-00003b00: 6500 7200 2000 5300 7000 6500 6900 6300  e.r. .S.p.e.i.c.
-00003b10: 6800 6500 7200 2000 6700 6500 7a00 e400  h.e.r. .g.e.z...
-00003b20: 6800 6c00 7400 2e00 2000 5400 7200 6f00  h.l.t... .T.r.o.
-00003b30: 7400 7a00 6400 6500 6d00 2000 6800 6f00  t.z.d.e.m. .h.o.
-00003b40: 6300 6800 6c00 6100 6400 6500 6e00 3f08  c.h.l.a.d.e.n.?.
-00003b50: 0000 0000 0600 0000 8046 696c 6520 227b  .........File "{
-00003b60: 6669 6c65 5f6e 616d 657d 2220 6973 206f  file_name}" is o
-00003b70: 7665 7220 3235 c2a0 4d42 2e20 5265 6d65  ver 25..MB. Reme
-00003b80: 6d62 6572 2074 6861 7420 5068 6f74 696e  mber that Photin
-00003b90: 6920 7570 6c6f 6164 7320 636f 756e 7420  i uploads count 
-00003ba0: 746f 7761 7264 7320 7374 6f72 6167 6520  towards storage 
-00003bb0: 696e 2079 6f75 7220 476f 6f67 6c65 2041  in your Google A
-00003bc0: 6363 6f75 6e74 2e20 5570 6c6f 6164 2069  ccount. Upload i
-00003bd0: 7420 616e 7977 6179 3f07 0000 000f 476f  t anyway?.....Go
-00003be0: 6f67 6c65 5068 6f74 6f73 5461 6201 0300  oglePhotosTab...
-00003bf0: 0000 3000 4700 6f00 6f00 6700 6c00 6500  ..0.G.o.o.g.l.e.
-00003c00: 2000 2600 5000 6800 6f00 7400 6f00 7300   .&.P.h.o.t.o.s.
-00003c10: 2000 6800 6f00 6300 6800 6c00 6100 6400   .h.o.c.h.l.a.d.
-00003c20: 6500 6e08 0000 0000 0600 0000 1547 6f6f  e.n..........Goo
-00003c30: 676c 6520 2650 686f 746f 7320 7570 6c6f  gle &Photos uplo
-00003c40: 6164 0700 0000 0f47 6f6f 676c 6550 686f  ad.....GooglePho
-00003c50: 746f 7354 6162 0103 0000 001a 0047 006f  tosTab.......G.o
-00003c60: 006f 0067 006c 0065 0020 0050 0068 006f  .o.g.l.e. .P.h.o
-00003c70: 0074 006f 0073 0800 0000 0006 0000 000d  .t.o.s..........
-00003c80: 476f 6f67 6c65 2050 686f 746f 7307 0000  Google Photos...
-00003c90: 000f 476f 6f67 6c65 5068 6f74 6f73 5461  ..GooglePhotosTa
-00003ca0: 6201 0300 0000 1800 4700 7200 6f00 df00  b.......G.r.o...
-00003cb0: 6500 2000 4400 6100 7400 6500 6900 2e08  e. .D.a.t.e.i...
-00003cc0: 0000 0000 0600 0000 0b4c 6172 6765 2066  .........Large f
-00003cd0: 696c 652e 0700 0000 0f47 6f6f 676c 6550  ile......GoogleP
-00003ce0: 686f 746f 7354 6162 0103 0000 0016 004e  hotosTab.......N
-00003cf0: 0065 0075 0065 0073 0020 0041 006c 0062  .e.u.e.s. .A.l.b
-00003d00: 0075 006d 0800 0000 0006 0000 0009 4e65  .u.m..........Ne
-00003d10: 7720 616c 6275 6d07 0000 000f 476f 6f67  w album.....Goog
-00003d20: 6c65 5068 6f74 6f73 5461 6201 0300 0000  lePhotosTab.....
-00003d30: 2800 5000 6800 6f00 7400 6900 6e00 6900  (.P.h.o.t.i.n.i.
-00003d40: 3a00 2000 6700 7200 6f00 df00 6500 2000  :. .g.r.o...e. .
-00003d50: 4400 6100 7400 6500 6908 0000 0000 0600  D.a.t.e.i.......
-00003d60: 0000 1350 686f 7469 6e69 3a20 6c61 7267  ...Photini: larg
-00003d70: 6520 6669 6c65 0700 0000 0f47 6f6f 676c  e file.....Googl
-00003d80: 6550 686f 746f 7354 6162 0103 0000 003e  ePhotosTab.....>
-00003d90: 0042 0069 0074 0074 0065 0020 0065 0069  .B.i.t.t.e. .e.i
-00003da0: 006e 0065 006e 0020 0041 006c 0062 0075  .n.e.n. .A.l.b.u
-00003db0: 006d 0074 0069 0074 0065 006c 0020 0065  .m.t.i.t.e.l. .e
-00003dc0: 0069 006e 0067 0065 0062 0065 006e 0800  .i.n.g.e.b.e.n..
-00003dd0: 0000 0006 0000 0022 506c 6561 7365 2065  ......."Please e
-00003de0: 6e74 6572 2061 2074 6974 6c65 2066 6f72  nter a title for
-00003df0: 2074 6865 2061 6c62 756d 0700 0000 0f47   the album.....G
-00003e00: 6f6f 676c 6550 686f 746f 7354 6162 0103  ooglePhotosTab..
-00003e10: 0000 0062 0047 0050 0058 0020 0044 0061  ...b.G.P.X. .D.a
-00003e20: 0074 0065 0069 0065 006e 0020 0028 002a  .t.e.i.e.n. .(.*
-00003e30: 002e 0067 0070 0078 0020 002a 002e 0047  ...g.p.x. .*...G
-00003e40: 0050 0058 0020 002a 002e 0047 0070 0078  .P.X. .*...G.p.x
-00003e50: 0029 003b 003b 0041 006c 006c 0065 0020  .).;.;.A.l.l.e. 
-00003e60: 0044 0061 0074 0065 0069 0065 006e 0020  .D.a.t.e.i.e.n. 
-00003e70: 0028 002a 0029 0800 0000 0006 0000 002c  .(.*.).........,
-00003e80: 4750 5820 6669 6c65 7320 282a 2e67 7078  GPX files (*.gpx
-00003e90: 202a 2e47 5058 202a 2e47 7078 293b 3b41   *.GPX *.Gpx);;A
-00003ea0: 6c6c 2066 696c 6573 2028 2a29 0700 0000  ll files (*)....
-00003eb0: 0b47 7078 496d 706f 7274 6572 0103 0000  .GpxImporter....
-00003ec0: 002a 0047 0050 0058 002d 0044 0061 0074  .*.G.P.X.-.D.a.t
-00003ed0: 0065 0069 0020 0069 006d 0070 006f 0072  .e.i. .i.m.p.o.r
-00003ee0: 0074 0069 0065 0072 0065 006e 0800 0000  .t.i.e.r.e.n....
-00003ef0: 0006 0000 000f 496d 706f 7274 2047 5058  ......Import GPX
-00003f00: 2066 696c 6507 0000 000b 4770 7849 6d70   file.....GpxImp
-00003f10: 6f72 7465 7201 0300 0000 1e00 4400 6100  orter.......D.a.
-00003f20: 7400 6500 6900 2000 7300 6300 6800 6c00  t.e.i. .s.c.h.l.
-00003f30: 6900 6500 df00 6500 6e03 0000 0022 0044  i.e...e.n....".D
-00003f40: 0061 0074 0065 0069 0065 006e 0020 0073  .a.t.e.i.e.n. .s
-00003f50: 0063 0068 006c 0069 0065 00df 0065 006e  .c.h.l.i.e...e.n
-00003f60: 0800 0000 0006 0000 000d 436c 6f73 6520  ..........Close 
-00003f70: 6669 6c65 2873 2907 0000 0009 496d 6167  file(s).....Imag
-00003f80: 654c 6973 7401 0300 0000 4c00 4d00 f600  eList.....L.M...
-00003f90: 6300 6800 7400 6500 6e00 2000 5300 6900  c.h.t.e.n. .S.i.
-00003fa0: 6500 2000 4900 6800 7200 6500 2000 c400  e. .I.h.r.e. ...
-00003fb0: 6e00 6400 6500 7200 7500 6e00 6700 6500  n.d.e.r.u.n.g.e.
-00003fc0: 6e00 2000 7300 7000 6500 6900 6300 6800  n. .s.p.e.i.c.h.
-00003fd0: 6500 7200 6e00 3f08 0000 0000 0600 0000  e.r.n.?.........
-00003fe0: 2144 6f20 796f 7520 7761 6e74 2074 6f20  !Do you want to 
-00003ff0: 7361 7665 2079 6f75 7220 6368 616e 6765  save your change
-00004000: 733f 0700 0000 0949 6d61 6765 4c69 7374  s?.....ImageList
-00004010: 0103 0000 0058 0042 0069 006c 0064 0065  .....X.B.i.l.d.e
-00004020: 0072 0020 0028 007b 0030 007d 0029 003b  .r. .(.{.0.}.).;
-00004030: 003b 0056 0069 0064 0065 006f 0073 0020  .;.V.i.d.e.o.s. 
-00004040: 0028 007b 0031 007d 0029 003b 003b 0041  .(.{.1.}.).;.;.A
-00004050: 006c 006c 0065 0020 0044 0061 0074 0065  .l.l.e. .D.a.t.e
-00004060: 0069 0065 006e 0020 0028 002a 0029 0800  .i.e.n. .(.*.)..
-00004070: 0000 0006 0000 0029 496d 6167 6573 2028  .......)Images (
-00004080: 7b30 7d29 3b3b 5669 6465 6f73 2028 7b31  {0});;Videos ({1
-00004090: 7d29 3b3b 416c 6c20 6669 6c65 7320 282a  });;All files (*
-000040a0: 2907 0000 0009 496d 6167 654c 6973 7401  ).....ImageList.
-000040b0: 0300 0000 4600 4d00 6500 7400 6100 6400  ....F.M.e.t.a.d.
-000040c0: 6100 7400 6500 6e00 2d00 5500 6e00 7400  a.t.e.n.-.U.n.t.
-000040d0: 6500 7200 7300 6300 6800 6900 6500 6400  e.r.s.c.h.i.e.d.
-000040e0: 6500 3a00 2000 7b00 6600 6900 6c00 6500  e.:. .{.f.i.l.e.
-000040f0: 5f00 6e00 6100 6d00 6500 7d08 0000 0000  _.n.a.m.e.}.....
-00004100: 0600 0000 214d 6574 6164 6174 6120 6469  ....!Metadata di
-00004110: 6666 6572 656e 6365 733a 207b 6669 6c65  fferences: {file
-00004120: 5f6e 616d 657d 0700 0000 0949 6d61 6765  _name}.....Image
-00004130: 4c69 7374 0103 0000 0042 0056 006f 0072  List.....B.V.o.r
-00004140: 0073 0063 0068 0061 0075 0020 0069 006e  .s.c.h.a.u. .i.n
-00004150: 0020 0044 0061 0074 0065 0069 0020 006e  . .D.a.t.e.i. .n
-00004160: 0069 0063 0068 0074 0020 0076 006f 0072  .i.c.h.t. .v.o.r
-00004170: 0068 0061 006e 0064 0065 006e 0800 0000  .h.a.n.d.e.n....
-00004180: 0006 0000 0014 4e6f 2074 6875 6d62 6e61  ......No thumbna
-00004190: 696c 2069 6e20 6669 6c65 0700 0000 0949  il in file.....I
-000041a0: 6d61 6765 4c69 7374 0103 0000 001c 0044  mageList.......D
-000041b0: 0061 0074 0065 0069 0065 006e 0020 00f6  .a.t.e.i.e.n. ..
-000041c0: 0066 0066 006e 0065 006e 0800 0000 0006  .f.f.n.e.n......
-000041d0: 0000 000a 4f70 656e 2066 696c 6573 0700  ....Open files..
-000041e0: 0000 0949 6d61 6765 4c69 7374 0103 0000  ...ImageList....
-000041f0: 003a 0050 0068 006f 0074 0069 006e 0069  .:.P.h.o.t.i.n.i
-00004200: 003a 0020 0075 006e 0067 0065 0073 0070  .:. .u.n.g.e.s.p
-00004210: 0065 0069 0063 0068 0065 0072 0074 0065  .e.i.c.h.e.r.t.e
-00004220: 0020 0044 0061 0074 0065 006e 0800 0000  . .D.a.t.e.n....
-00004230: 0006 0000 0015 5068 6f74 696e 693a 2075  ......Photini: u
-00004240: 6e73 6176 6564 2064 6174 6107 0000 0009  nsaved data.....
-00004250: 496d 6167 654c 6973 7401 0300 0000 3600  ImageList.....6.
-00004260: 4d00 6900 6e00 6900 6100 7400 7500 7200  M.i.n.i.a.t.u.r.
-00004270: 6200 6900 6c00 6400 2000 6e00 6500 7500  b.i.l.d. .n.e.u.
-00004280: 2000 6700 6500 6e00 6500 7200 6900 6500   .g.e.n.e.r.i.e.
-00004290: 7200 6500 6e03 0000 003a 004d 0069 006e  r.e.n....:.M.i.n
-000042a0: 0069 0061 0074 0075 0072 0062 0069 006c  .i.a.t.u.r.b.i.l
-000042b0: 0064 0065 0072 0020 006e 0065 0075 0020  .d.e.r. .n.e.u. 
-000042c0: 0067 0065 006e 0065 0072 0069 0065 0072  .g.e.n.e.r.i.e.r
-000042d0: 0065 006e 0800 0000 0006 0000 0017 5265  .e.n..........Re
-000042e0: 6765 6e65 7261 7465 2074 6875 6d62 6e61  generate thumbna
-000042f0: 696c 2873 2907 0000 0009 496d 6167 654c  il(s).....ImageL
-00004300: 6973 7401 0300 0000 1e00 4400 6100 7400  ist.......D.a.t.
-00004310: 6500 6900 2000 6e00 6500 7500 2000 6c00  e.i. .n.e.u. .l.
-00004320: 6100 6400 6500 6e03 0000 0022 0044 0061  a.d.e.n....".D.a
-00004330: 0074 0065 0069 0065 006e 0020 006e 0065  .t.e.i.e.n. .n.e
-00004340: 0075 0020 006c 0061 0064 0065 006e 0800  .u. .l.a.d.e.n..
-00004350: 0000 0006 0000 000e 5265 6c6f 6164 2066  ........Reload f
-00004360: 696c 6528 7329 0700 0000 0949 6d61 6765  ile(s).....Image
-00004370: 4c69 7374 0103 0000 0028 00c4 006e 0064  List.....(...n.d
-00004380: 0065 0072 0075 006e 0067 0065 006e 0020  .e.r.u.n.g.e.n. 
-00004390: 0073 0070 0065 0069 0063 0068 0065 0072  .s.p.e.i.c.h.e.r
-000043a0: 006e 0800 0000 0006 0000 000c 5361 7665  .n..........Save
-000043b0: 2063 6861 6e67 6573 0700 0000 0949 6d61   changes.....Ima
-000043c0: 6765 4c69 7374 0103 0000 005e 0045 0069  geList.....^.E.i
-000043d0: 006e 0069 0067 0065 0020 0042 0069 006c  .n.i.g.e. .B.i.l
-000043e0: 0064 0065 0072 0020 0065 006e 0074 0068  .d.e.r. .e.n.t.h
-000043f0: 0061 006c 0074 0065 006e 0020 0075 006e  .a.l.t.e.n. .u.n
-00004400: 0067 0065 0073 0069 0063 0068 0065 0072  .g.e.s.i.c.h.e.r
-00004410: 0074 0065 0020 004d 0065 0074 0061 0064  .t.e. .M.e.t.a.d
-00004420: 0061 0074 0065 006e 002e 0800 0000 0006  .a.t.e.n........
-00004430: 0000 0022 536f 6d65 2069 6d61 6765 7320  ..."Some images 
-00004440: 6861 7665 2075 6e73 6176 6564 206d 6574  have unsaved met
-00004450: 6164 6174 612e 0700 0000 0949 6d61 6765  adata......Image
-00004460: 4c69 7374 0103 0000 001c 0053 006f 0072  List.......S.o.r
-00004470: 0074 0069 0065 0072 0065 006e 0020 006e  .t.i.e.r.e.n. .n
-00004480: 0061 0063 0068 0800 0000 0006 0000 0007  .a.c.h..........
-00004490: 536f 7274 2062 7907 0000 0009 496d 6167  Sort by.....Imag
-000044a0: 654c 6973 7401 0300 0000 2200 5600 6f00  eList.....".V.o.
-000044b0: 7200 7300 6300 6800 6100 7500 6200 6900  r.s.c.h.a.u.b.i.
-000044c0: 6c00 6400 6700 7200 f600 df00 6508 0000  l.d.g.r.....e...
-000044d0: 0000 0600 0000 0e54 6875 6d62 6e61 696c  .......Thumbnail
-000044e0: 2073 697a 6507 0000 0009 496d 6167 654c   size.....ImageL
-000044f0: 6973 7401 0300 0000 2600 c400 6e00 6400  ist.....&...n.d.
-00004500: 6500 7200 7500 6e00 6700 6500 6e00 2000  e.r.u.n.g.e.n. .
-00004510: 6100 6e00 7a00 6500 6900 6700 6500 6e08  a.n.z.e.i.g.e.n.
-00004520: 0000 0000 0600 0000 0c56 6965 7720 6368  .........View ch
-00004530: 616e 6765 7307 0000 0009 496d 6167 654c  anges.....ImageL
-00004540: 6973 7401 0300 0000 1a00 4100 7500 6600  ist.......A.u.f.
-00004550: 6e00 6100 6800 6d00 6500 6400 6100 7400  n.a.h.m.e.d.a.t.
-00004560: 7500 6d08 0000 0000 0600 0000 0a64 6174  u.m..........dat
-00004570: 6520 7461 6b65 6e07 0000 0009 496d 6167  e taken.....Imag
-00004580: 654c 6973 7401 0300 0000 1200 4400 6100  eList.......D.a.
-00004590: 7400 6500 6900 6e00 6100 6d00 6508 0000  t.e.i.n.a.m.e...
-000045a0: 0000 0600 0000 0966 696c 6520 6e61 6d65  .......file name
-000045b0: 0700 0000 0949 6d61 6765 4c69 7374 0103  .....ImageList..
-000045c0: 0000 0014 006e 0065 0075 0065 0072 0020  .....n.e.u.e.r. 
-000045d0: 0057 0065 0072 0074 0800 0000 0006 0000  .W.e.r.t........
-000045e0: 0009 6e65 7720 7661 6c75 6507 0000 0009  ..new value.....
-000045f0: 496d 6167 654c 6973 7401 0300 0000 1400  ImageList.......
-00004600: 6100 6c00 7400 6500 7200 2000 5700 6500  a.l.t.e.r. .W.e.
-00004610: 7200 7408 0000 0000 0600 0000 096f 6c64  r.t..........old
-00004620: 2076 616c 7565 0700 0000 0949 6d61 6765   value.....Image
-00004630: 4c69 7374 0103 0000 0014 0072 00fc 0063  List.......r...c
-00004640: 006b 0067 00e4 006e 0067 0069 0067 0800  .k.g...n.g.i.g..
-00004650: 0000 0006 0000 0004 756e 646f 0700 0000  ........undo....
-00004660: 0949 6d61 6765 4c69 7374 0103 0000 0026  .ImageList.....&
-00004670: 0025 006e 0020 0044 0061 0074 0065 0069  .%.n. .D.a.t.e.i
-00004680: 0020 0061 0075 0073 0067 0065 0077 00e4  . .a.u.s.g.e.w..
-00004690: 0068 006c 0074 0300 0000 2a00 2500 6e00  .h.l.t....*.%.n.
-000046a0: 2000 4400 6100 7400 6500 6900 6500 6e00   .D.a.t.e.i.e.n.
-000046b0: 2000 6100 7500 7300 6700 6500 7700 e400   .a.u.s.g.e.w...
-000046c0: 6800 6c00 7408 0000 0000 0600 0000 1325  h.l.t..........%
-000046d0: 6e20 6669 6c65 2873 2920 7365 6c65 6374  n file(s) select
-000046e0: 6564 0700 0000 0b49 6d70 6f72 7465 7254  ed.....ImporterT
-000046f0: 6162 0103 0000 0026 0042 0069 006c 0064  ab.....&.B.i.l.d
-00004700: 0065 0072 0020 0026 0049 006d 0070 006f  .e.r. .&.I.m.p.o
-00004710: 0072 0074 0069 0065 0072 0065 006e 0800  .r.t.i.e.r.e.n..
-00004720: 0000 0006 0000 000e 2649 6d70 6f72 7420  ........&Import 
-00004730: 7068 6f74 6f73 0700 0000 0b49 6d70 6f72  photos.....Impor
-00004740: 7465 7254 6162 0103 0000 0026 003c 004f  terTab.....&.<.O
-00004750: 0072 0064 006e 0065 0072 0020 0068 0069  .r.d.n.e.r. .h.i
-00004760: 006e 007a 0075 0066 00fc 0067 0065 006e  .n.z.u.f...g.e.n
-00004770: 003e 0800 0000 0006 0000 000e 3c61 6464  .>..........<add
-00004780: 2061 2066 6f6c 6465 723e 0700 0000 0b49   a folder>.....I
-00004790: 6d70 6f72 7465 7254 6162 0103 0000 0024  mporterTab.....$
-000047a0: 003c 0051 0075 0065 006c 006c 0065 0020  .<.Q.u.e.l.l.e. 
-000047b0: 0061 0075 0073 0077 00e4 0068 006c 0065  .a.u.s.w...h.l.e
-000047c0: 006e 003e 0800 0000 0006 0000 000f 3c73  .n.>..........<s
-000047d0: 656c 6563 7420 736f 7572 6365 3e07 0000  elect source>...
-000047e0: 000b 496d 706f 7274 6572 5461 6201 0300  ..ImporterTab...
-000047f0: 0000 6c00 5700 6500 6e00 6e00 2000 5300  ..l.W.e.n.n. .S.
-00004800: 6900 6500 2000 6a00 6500 7400 7a00 7400  i.e. .j.e.t.z.t.
-00004810: 2000 7300 6300 6800 6c00 6900 6500 df00   .s.c.h.l.i.e...
-00004820: 6500 6e00 2c00 2000 7700 6900 7200 6400  e.n.,. .w.i.r.d.
-00004830: 2000 6400 6500 7200 2000 4900 6d00 7000   .d.e.r. .I.m.p.
-00004840: 6f00 7200 7400 2000 6100 6200 6700 6500  o.r.t. .a.b.g.e.
-00004850: 6200 7200 6f00 6300 6800 6500 6e00 2e08  b.r.o.c.h.e.n...
-00004860: 0000 0000 0600 0000 2643 6c6f 7369 6e67  ........&Closing
-00004870: 206e 6f77 2077 696c 6c20 7465 726d 696e   now will termin
-00004880: 6174 6520 7468 6520 696d 706f 7274 2e07  ate the import..
+00000010: a700 0000 0264 6542 0000 0c38 0000 5a6c  .....deB...8..Zl
+00000020: 0000 7602 0000 7388 0000 9160 0000 73fe  ..v...s....`..s.
+00000030: 0000 918a 0004 a0b9 0000 0159 0004 a0b9  ...........Y....
+00000040: 0000 669b 0004 bda9 0000 55bf 0004 d025  ..f.......U....%
+00000050: 0000 58b1 0004 ec30 0000 5959 0005 4835  ..X....0..YY..H5
+00000060: 0000 09b4 0005 4835 0000 73ba 0005 4835  ......H5..s...H5
+00000070: 0000 84bf 0005 8c04 0000 5c19 0005 9625  ..........\....%
+00000080: 0000 8687 0005 97c5 0000 2d59 0005 a200  ..........-Y....
+00000090: 0000 a3e4 0007 c4af 0000 3b89 0012 2b0e  ..........;...+.
+000000a0: 0000 543c 001c da4d 0000 4c9a 001c dbdd  ..T<...M..L.....
+000000b0: 0000 9efe 0024 12d5 0000 39fa 002c f63e  .....$....9..,.>
+000000c0: 0000 17aa 002d 8634 0000 8183 0037 171b  .....-.4.....7..
+000000d0: 0000 812d 003b f105 0000 1d3f 0040 e4ce  ...-.;.....?.@..
+000000e0: 0000 a830 0043 4cae 0000 a95d 0047 c4e3  ...0.CL....].G..
+000000f0: 0000 a10d 004b 87d4 0000 7dab 0056 aec2  .....K....}..V..
+00000100: 0000 7f30 0056 aec2 0000 8ea3 0056 f6af  ...0.V.......V..
+00000110: 0000 2c31 005a 81be 0000 909f 005b 0b25  ..,1.Z.......[.%
+00000120: 0000 2e5c 005b 0b25 0000 4c6b 005b 0b25  ...\.[.%..Lk.[.%
+00000130: 0000 81db 0060 1085 0000 7fb6 0067 aad3  .....`.......g..
+00000140: 0000 58db 0069 a403 0000 36fd 0069 a403  ..X..i....6..i..
+00000150: 0000 5983 006c c199 0000 2857 0071 0769  ..Y..l....(W.q.i
+00000160: 0000 612d 0077 0ebc 0000 8714 0094 cf02  ..a-.w..........
+00000170: 0000 9059 00a2 1470 0000 9481 00a3 85ee  ...Y...p........
+00000180: 0000 0786 00b8 6470 0000 93a5 00bd d20e  ......dp........
+00000190: 0000 9ac3 00c0 dd34 0000 4725 00c6 1d14  .......4..G%....
+000001a0: 0000 9e5d 00c6 6470 0000 9410 00d1 9ab5  ...]..dp........
+000001b0: 0000 a042 00d7 0cb9 0000 3858 00f2 f2c8  ...B......8X....
+000001c0: 0000 2a90 0106 6074 0000 4e26 011d e755  ..*...`t..N&...U
+000001d0: 0000 46d9 0126 bda5 0000 677b 0145 eb79  ..F..&....g{.E.y
+000001e0: 0000 3363 015e eb2f 0000 a72b 015f 0dad  ..3c.^./...+._..
+000001f0: 0000 32df 0163 c933 0000 223a 016a 032e  ..2..c.3..":.j..
+00000200: 0000 69b7 0173 8fc8 0000 9eba 0180 6a59  ..i..s........jY
+00000210: 0000 5664 018e d47e 0000 1250 018f 97f8  ..Vd...~...P....
+00000220: 0000 8d8c 01be 34b7 0000 8c1e 01c1 faa5  ......4.........
+00000230: 0000 2928 01c1 faa5 0000 8246 01c5 f5cd  ..)(.......F....
+00000240: 0000 9691 01ca 84a1 0000 799a 01d2 e96e  ..........y....n
+00000250: 0000 59c5 01d8 cd24 0000 3bbf 01e4 e113  ..Y....$..;.....
+00000260: 0000 94ee 01f7 4f45 0000 67d6 01fc 7925  ......OE..g...y%
+00000270: 0000 551c 01fd 69a5 0000 1eba 0201 ff63  ..U...i........c
+00000280: 0000 88e3 0232 05d5 0000 4376 0249 c9ae  .....2....Cv.I..
+00000290: 0000 a17c 026d bc14 0000 a424 0277 2b35  ...|.m.....$.w+5
+000002a0: 0000 3ada 0286 e00e 0000 12a0 0296 5357  ..:...........SW
+000002b0: 0000 5392 0298 5c09 0000 63f5 02c8 9fa3  ..S...\...c.....
+000002c0: 0000 2516 02cf fca5 0000 3411 02d6 0815  ..%.......4.....
+000002d0: 0000 a395 02f9 c4c5 0000 2aee 02f9 c4c5  ..........*.....
+000002e0: 0000 4ac6 02f9 c4c5 0000 7e5c 0302 20f5  ..J.......~\.. .
+000002f0: 0000 4f49 0305 1aa9 0000 47c2 030c 9764  ..OI......G....d
+00000300: 0000 5b73 0354 44bd 0000 3604 0359 7694  ..[s.TD...6..Yv.
+00000310: 0000 9d98 035a 4e6e 0000 6f36 037d 2417  .....ZNn..o6.}$.
+00000320: 0000 95af 037d 9c24 0000 7f61 037f eb99  .....}.$...a....
+00000330: 0000 6824 0380 b55f 0000 a4c7 0391 ff0e  ..h$..._........
+00000340: 0000 04db 039a 6ece 0000 9cf0 03b0 bf25  ......n........%
+00000350: 0000 00b6 03b0 bf25 0000 78bd 03b4 664e  .......%..x...fN
+00000360: 0000 a923 03b5 83a3 0000 7d4d 03e2 d39e  ...#......}M....
+00000370: 0000 0de0 03e6 8545 0000 75bd 03ef 1f79  .......E..u....y
+00000380: 0000 3565 03f1 1a05 0000 8cee 03ff d948  ..5e...........H
+00000390: 0000 8b14 0409 59a5 0000 7485 040e 9e79  ......Y...t....y
+000003a0: 0000 4b7c 0442 4dfe 0000 7874 044c 1eee  ..K|.BM...xt.L..
+000003b0: 0000 9979 0457 019e 0000 0648 0459 8f63  ...y.W.....H.Y.c
+000003c0: 0000 5c9b 045f e8c9 0000 1dda 0460 e588  ..\.._.......`..
+000003d0: 0000 560b 0498 3c81 0000 8a4d 04ab 7ea5  ..V...<....M..~.
+000003e0: 0000 4f8f 04c8 4039 0000 29a7 04c8 4039  ..O...@9..)...@9
+000003f0: 0000 4913 04d0 e082 0000 8fe7 04d2 fa22  ..I............"
+00000400: 0000 29d9 04d3 9ff4 0000 3142 04f5 7367  ..).......1B..sg
+00000410: 0000 2bce 0515 8cbe 0000 8638 051a 65f5  ..+........8..e.
+00000420: 0000 9fd0 0520 62a4 0000 775e 0528 4ac0  ..... b...w^.(J.
+00000430: 0000 4edf 052d 4d3c 0000 279e 0530 af74  ..N..-M<..'..0.t
+00000440: 0000 820a 0531 a702 0000 4089 0535 96fe  .....1....@..5..
+00000450: 0000 9d5e 0537 8957 0000 24c2 053b 7b05  ...^.7.W..$..;{.
+00000460: 0000 2b8c 053b 7b05 0000 4b38 053e 782d  ..+..;{...K8.>x-
+00000470: 0000 4243 0544 794d 0000 41e4 055f 746e  ..BC.DyM..A.._tn
+00000480: 0000 9b6a 0565 06e3 0000 0bfd 0577 76ec  ...j.e.......wv.
+00000490: 0000 8b55 057b 92f3 0000 2c8d 057b 92f3  ...U.{....,..{..
+000004a0: 0000 8083 0588 b047 0000 1d04 058b e05e  .......G.......^
+000004b0: 0000 0a1a 058f dfb3 0000 758e 059b 8898  ..........u.....
+000004c0: 0000 79ee 05a3 3419 0000 77a2 05a6 17ae  ..y...4...w.....
+000004d0: 0000 7ca7 05a6 c895 0000 40e5 05a9 c6ae  ..|.......@.....
+000004e0: 0000 7676 05ab 8bc4 0000 0a4b 05ac 8de5  ..vv.......K....
+000004f0: 0000 2b1f 05af caf4 0000 8e26 05b9 6619  ..+........&..f.
+00000500: 0000 1f05 05d3 4c4e 0000 7820 05dd d675  ......LN..x ...u
+00000510: 0000 66c6 05e9 9749 0000 8022 05fe 219e  ..f....I..."..!.
+00000520: 0000 8e61 0602 a46e 0000 835b 0618 f51e  ...a...n...[....
+00000530: 0000 700a 0626 dcc9 0000 4117 0627 7c75  ..p..&....A..'|u
+00000540: 0000 415a 063b cf25 0000 3689 0647 6c6e  ..AZ.;.%..6..Gln
+00000550: 0000 3cef 064f 4f8e 0000 6d1d 0653 24e5  ..<..OO...m..S$.
+00000560: 0000 7bd8 065a 7e13 0000 478a 0667 a1fe  ..{..Z~...G..g..
+00000570: 0000 7e8f 066a 3ba3 0000 2300 067b 0603  ..~..j;...#..{..
+00000580: 0000 5a70 067c 1595 0000 3b4e 068d 7d90  ..Zp.|....;N..}.
+00000590: 0000 78ec 068f 2045 0000 446d 0698 3c81  ..x... E..Dm..<.
+000005a0: 0000 0a7c 069d bc4e 0000 1535 06a5 c6b5  ...|...N...5....
+000005b0: 0000 84ea 06b7 eb69 0000 2ee0 06ba eeff  .......i........
+000005c0: 0000 a7a5 06c3 2be7 0000 5d28 06c9 55b9  ......+...](..U.
+000005d0: 0000 4a8e 06c9 b805 0000 8934 06ce 697e  ..J........4..i~
+000005e0: 0000 3e3b 06d4 e879 0000 346a 06e7 88c7  ..>;...y..4j....
+000005f0: 0000 523a 06ea 1312 0000 3f97 06f1 acb5  ..R:......?.....
+00000600: 0000 7950 0706 6093 0000 7628 0717 352e  ..yP..`...v(..5.
+00000610: 0000 8567 071b d822 0000 a098 0725 0ed3  ...g...".....%..
+00000620: 0000 3df4 072a 02b3 0000 3c47 072b 5bf1  ..=..*....<G.+[.
+00000630: 0000 8ed5 073b 0713 0000 3ee3 073e 8aae  .....;....>..>..
+00000640: 0000 31f6 0740 7b19 0000 37ae 0745 d72e  ..1..@{...7..E..
+00000650: 0000 a8d8 0747 58b5 0000 3280 0752 93ae  .....GX...2..R..
+00000660: 0000 01b4 0756 937c 0000 91b4 0761 5de5  .....V.|.....a].
+00000670: 0000 1f6d 0773 020e 0000 9833 0778 9733  ...m.s.....3.x.3
+00000680: 0000 8f40 077c e91e 0000 3a98 0783 2294  ...@.|....:...".
+00000690: 0000 2128 078c 0ba4 0000 1d99 0790 c8f5  ..!(............
+000006a0: 0000 2c5c 0791 9109 0000 48c0 079d a354  ..,\......H....T
+000006b0: 0000 a476 07a1 d6cb 0000 5bb7 07ab 8e03  ...v......[.....
+000006c0: 0000 0000 07b4 0f05 0000 74ef 07c3 bd54  ..........t....T
+000006d0: 0000 92c8 07c9 d658 0000 85f3 07e0 1a4f  .......X.......O
+000006e0: 0000 34da 07ee 2434 0000 86b4 07f6 6e0f  ..4...$4......n.
+000006f0: 0000 9bb9 0812 7098 0000 7a1d 0842 126e  ......p...z..B.n
+00000700: 0000 5aa3 0843 f97e 0000 1987 0847 159e  ..Z..C.~.....G..
+00000710: 0000 9601 084e b2f5 0000 4f11 0876 6c3e  .....N....O..vl>
+00000720: 0000 024b 089b d2f1 0000 8777 08a4 2089  ...K.......w.. .
+00000730: 0000 7c40 08ad 8b6e 0000 7123 08ae abbe  ..|@...n..q#....
+00000740: 0000 01fc 08bc 210e 0000 0d9b 08bd 8ce8  ......!.........
+00000750: 0000 42a2 08f0 ac75 0000 2362 08fb ecd3  ..B....u..#b....
+00000760: 0000 57f0 08ff ed5f 0000 2f7c 090d 6f19  ..W...._../|..o.
+00000770: 0000 1bdf 091d 05f0 0000 752f 0920 f035  ..........u/. .5
+00000780: 0000 731f 0923 8a14 0000 9545 092a 03d5  ..s..#.....E.*..
+00000790: 0000 0037 092c eb99 0000 11df 0941 e34c  ...7.,.......A.L
+000007a0: 0000 2074 0949 9184 0000 7aeb 0949 b384  .. t.I....z..I..
+000007b0: 0000 6084 094d 67fe 0000 2966 094d 67fe  ..`..Mg...)f.Mg.
+000007c0: 0000 484d 094d 67fe 0000 7d0a 094d 67fe  ..HM.Mg...}..Mg.
+000007d0: 0000 8319 095e 89d3 0000 a2bb 0968 7d7d  .....^.......h}}
+000007e0: 0000 2b4f 0968 7d7d 0000 323d 0968 7d7d  ..+O.h}}..2=.h}}
+000007f0: 0000 4af9 096d 01e5 0000 09df 096f 9788  ..J..m.......o..
+00000800: 0000 8d31 0974 a647 0000 5280 0977 0c94  ...1.t.G..R..w..
+00000810: 0000 8529 097c 1775 0000 3b13 0987 b01e  ...).|.u..;.....
+00000820: 0000 7b91 09ca a91e 0000 6e35 09ee 202e  ..{.......n5.. .
+00000830: 0000 1653 09f5 9023 0000 4d4a 0a0d 74f2  ...S...#..MJ..t.
+00000840: 0000 0af3 0a0d 74f2 0000 5b04 0a3b 8333  ......t...[..;.3
+00000850: 0000 08a3 0a69 66c9 0000 39b9 0a6c 5bd9  .....if...9..l[.
+00000860: 0000 0186 0a6c 5bd9 0000 671b 0a73 2a51  .....l[...g..s*Q
+00000870: 0000 3741 0a7f ce9e 0000 a530 0a89 b649  ..7A.......0...I
+00000880: 0000 2a3c 0a8b 8b22 0000 6747 0a8b d95e  ..*<..."..gG...^
+00000890: 0000 391b 0a99 6ff8 0000 90db 0ac7 826e  ..9...o........n
+000008a0: 0000 06cb 0ad6 d87e 0000 02ec 0ae9 b7f5  .......~........
+000008b0: 0000 2692 0aea 9594 0000 23c2 0afb 86b9  ..&.......#.....
+000008c0: 0000 534e 0b0c 8953 0000 31ab 0b16 9077  ..SN...S..1....w
+000008d0: 0000 092f 0b1c 6fee 0000 00e5 0b31 6541  .../..o......1eA
+000008e0: 0000 0d33 0b32 f535 0000 4dc9 0b52 aea4  ...3.2.5..M..R..
+000008f0: 0000 42db 0b55 9355 0000 9f78 0b69 37c9  ..B..U.U...x.i7.
+00000900: 0000 650a 0b6f 5c75 0000 8ca5 0b70 d229  ..e..o\u.....p.)
+00000910: 0000 2e89 0b7b 2ca5 0000 1c7a 0b81 700e  .....{,....z..p.
+00000920: 0000 685b 0b82 249e 0000 05ca 0b8a 2614  ..h[..$.......&.
+00000930: 0000 2d17 0ba0 757f 0000 a5d3 0ba0 9785  ..-...u.........
+00000940: 0000 451f 0ba0 c9de 0000 8fa7 0ba3 fc0c  ..E.............
+00000950: 0000 3fff 0ba4 08e7 0000 4045 0bbf 620d  ..?.......@E..b.
+00000960: 0000 0b62 0bc0 05e4 0000 2dd1 0bc0 93e3  ...b......-.....
+00000970: 0000 8478 0be4 0395 0000 8de7 0bf0 453e  ...x..........E>
+00000980: 0000 21a8 0c13 2b8e 0000 3d42 0c1a b9a5  ..!...+...=B....
+00000990: 0000 52f0 0c25 7849 0000 619f 0c27 e76f  ..R..%xI..a..'.o
+000009a0: 0000 a692 0c28 b745 0000 8742 0c29 84a3  .....(.E...B.)..
+000009b0: 0000 3a48 0c35 9b9e 0000 65e0 0c4c 8c75  ..:H.5....e..L.u
+000009c0: 0000 7e20 0c5d e1c2 0000 2582 0c5e 6fb4  ..~ .]....%..^o.
+000009d0: 0000 41a3 0c7d 7095 0000 2758 0c80 8aa3  ..A..}p...'X....
+000009e0: 0000 38c9 0c80 8aa3 0000 5c4b 0c93 93be  ..8.......\K....
+000009f0: 0000 5f07 0c94 ba43 0000 0c98 0ca0 d5c3  .._....C........
+00000a00: 0000 20ca 0cbb 0173 0000 5cea 0cca 0285  .. ....s..\.....
+00000a10: 0000 4890 0cce 648d 0000 9dd3 0cd8 f02d  ..H...d........-
+00000a20: 0000 0aad 0d04 cb1e 0000 3c9b 0d0e 50f8  ..........<...P.
+00000a30: 0000 82cd 0d0e 6da3 0000 1cbb 0d19 6c99  ......m.......l.
+00000a40: 0000 499d 0d34 07f1 0000 201e 0d36 9b85  ..I..4.... ..6..
+00000a50: 0000 60e2 0d49 166e 0000 8285 0d86 3e6e  ..`..I.n......>n
+00000a60: 0000 5d6a 0d8c 40ce 0000 77dd 0d8f c4f3  ..]j..@...w.....
+00000a70: 0000 2a09 0d8f c4f3 0000 4a59 0d96 5b13  ..*.......JY..[.
+00000a80: 0000 22b4 0d96 f824 0000 2410 0db0 6493  .."....$..$...d.
+00000a90: 0000 4947 0dba 6f39 0000 6301 0dc9 1a88  ..IG..o9..c.....
+00000aa0: 0000 26e5 0dd7 f89b 0000 5847 0e03 0de0  ..&.......XG....
+00000ab0: 0000 2629 0e03 0de0 0000 466e 0e0b 4344  ..&)......Fn..CD
+00000ac0: 0000 8ad0 0e0c 2965 0000 45e3 0e14 c055  ......)e..E....U
+00000ad0: 0000 5792 0e2c 0f2e 0000 7ee8 0e31 45cf  ..W..,....~..1E.
+00000ae0: 0000 8814 0e39 c321 0000 601e 0e6e 2258  .....9.!..`..n"X
+00000af0: 0000 89db 0e6e 4858 0000 8969 0e6f 36c5  .....nHX...i.o6.
+00000b00: 0000 85ab 0e95 28b5 0000 1e26 0e97 bcb5  ......(....&....
+00000b10: 0000 1e72 0e9c a374 0000 9247 0e9e 60ae  ...r...t...G..`.
+00000b20: 0000 511c 0ea3 b08e 0000 03f2 0eaf 6fc3  ..Q...........o.
+00000b30: 0000 737b 0ebe c4c3 0000 7a89 0ec1 ac3f  ..s{......z....?
+00000b40: 0000 4e92 0ed2 6f37 0000 8b98 0ed2 862e  ..N...o7........
+00000b50: 0000 6b51 0edb 53e1 0000 2cc5 0edb 53e1  ..kQ..S...,...S.
+00000b60: 0000 4bce 0edd a743 0000 1fcc 0edf 208d  ..K....C...... .
+00000b70: 0000 9349 0eeb 97ce 0000 6c19 0eed da75  ...I......l....u
+00000b80: 0000 8a80 0eee 44a4 0000 91e7 0ef1 01de  ......D.........
+00000b90: 0000 56a5 0ef6 09ee 0000 0813 0f05 000c  ..V.............
+00000ba0: 0000 2d87 0f16 93ca 0000 4d10 0f31 815c  ..-.......M..1.\
+00000bb0: 0000 43ef 0f33 2495 0000 2f39 0f48 89e2  ..C..3$.../9.H..
+00000bc0: 0000 73e3 0f59 715e 0000 96ef 0f62 0773  ..s..Yq^.....b.s
+00000bd0: 0000 3f32 0f64 7a39 0000 744c 0f66 4e29  ..?2.dz9..tL.fN)
+00000be0: 0000 7dde 0f6f e836 0000 87d5 0f82 a059  ..}..o.6.......Y
+00000bf0: 0000 80bd 0f8f 1b8e 0000 25db 0f9a 906e  ..........%....n
+00000c00: 0000 4ff7 0f9d 6ca9 0000 27fd 0fa8 b309  ..O...l...'.....
+00000c10: 0000 6254 0fa9 1015 0000 a2fd 0fb1 d16f  ..bT...........o
+00000c20: 0000 a348 0fb6 b24e 0000 7232 0fd4 15de  ...H...N..r2....
+00000c30: 0000 4331 0fd4 15de 0000 7b4c 0fe8 0889  ..C1......{L....
+00000c40: 0000 54d0 0fef 5405 0000 2e15 0fef 5405  ..T...T.......T.
+00000c50: 0000 4c22 6900 00a9 8803 0000 0010 0026  ..L"i..........&
+00000c60: 0041 0064 0072 0065 0073 0073 0065 0800  .A.d.r.e.s.s.e..
+00000c70: 0000 0006 0000 0008 2641 6464 7265 7373  ........&Address
+00000c80: 0700 0000 0a41 6464 7265 7373 5461 6201  .....AddressTab.
+00000c90: 0300 0000 3e00 4100 6400 7200 6500 7300  ....>.A.d.r.e.s.
+00000ca0: 7300 7300 7500 6300 6800 6500 2000 7000  s.s.u.c.h.e. .p.
+00000cb0: 6f00 7700 6500 7200 6500 6400 2000 6200  o.w.e.r.e.d. .b.
+00000cc0: 7900 2000 4f00 7000 6500 6e00 4300 6100  y. .O.p.e.n.C.a.
+00000cd0: 6700 6508 0000 0000 0600 0000 2241 6464  g.e........."Add
+00000ce0: 7265 7373 206c 6f6f 6b75 7020 706f 7765  ress lookup powe
+00000cf0: 7265 6420 6279 204f 7065 6e43 6167 6507  red by OpenCage.
+00000d00: 0000 000a 4164 6472 6573 7354 6162 0103  ....AddressTab..
+00000d10: 0000 0008 0048 00f6 0068 0065 0800 0000  .....H...h.e....
+00000d20: 0006 0000 0008 416c 7469 7475 6465 0700  ......Altitude..
+00000d30: 0000 0a41 6464 7265 7373 5461 6201 0300  ...AddressTab...
+00000d40: 0000 3200 4800 f600 6800 6500 2000 6400  ..2.H...h.e. .d.
+00000d50: 6500 7300 2000 4f00 7200 7400 6500 7300  e.s. .O.r.t.e.s.
+00000d60: 2000 6900 6e00 2000 4d00 6500 7400 6500   .i.n. .M.e.t.e.
+00000d70: 7200 6e00 2e08 0000 0000 0600 0000 2341  r.n...........#A
+00000d80: 6c74 6974 7564 6520 6f66 2074 6865 206c  ltitude of the l
+00000d90: 6f63 6174 696f 6e20 696e 206d 6574 7265  ocation in metre
+00000da0: 732e 0700 0000 0a41 6464 7265 7373 5461  s......AddressTa
+00000db0: 6201 0300 0000 0a00 5300 7400 6100 6400  b.......S.t.a.d.
+00000dc0: 7408 0000 0000 0600 0000 0443 6974 7907  t..........City.
+00000dd0: 0000 000a 4164 6472 6573 7354 6162 0103  ....AddressTab..
+00000de0: 0000 0008 004c 0061 006e 0064 0800 0000  .....L.a.n.d....
+00000df0: 0006 0000 0007 436f 756e 7472 7907 0000  ......Country...
+00000e00: 000a 4164 6472 6573 7354 6162 0103 0000  ..AddressTab....
+00000e10: 001a 004f 0072 0074 0020 0065 006e 0074  ...O.r.t. .e.n.t
+00000e20: 0066 0065 0072 006e 0065 006e 0800 0000  .f.e.r.n.e.n....
+00000e30: 0006 0000 000f 4465 6c65 7465 206c 6f63  ......Delete loc
+00000e40: 6174 696f 6e07 0000 000a 4164 6472 6573  ation.....Addres
+00000e50: 7354 6162 0103 0000 001e 004f 0072 0074  sTab.......O.r.t
+00000e60: 0020 0064 0075 0070 006c 0069 007a 0069  . .d.u.p.l.i.z.i
+00000e70: 0065 0072 0065 006e 0800 0000 0006 0000  .e.r.e.n........
+00000e80: 0012 4475 706c 6963 6174 6520 6c6f 6361  ..Duplicate loca
+00000e90: 7469 6f6e 0700 0000 0a41 6464 7265 7373  tion.....Address
+00000ea0: 5461 6201 0300 0000 6000 4700 6500 6200  Tab.....`.G.e.b.
+00000eb0: 6500 6e00 2000 5300 6900 6500 2000 6400  e.n. .S.i.e. .d.
+00000ec0: 6500 6e00 2000 7600 6f00 6c00 6c00 7300  e.n. .v.o.l.l.s.
+00000ed0: 7400 e400 6e00 6400 6900 6700 6500 6e00  t...n.d.i.g.e.n.
+00000ee0: 2000 4e00 6100 6d00 6500 6e00 2000 6400   .N.a.m.e.n. .d.
+00000ef0: 6500 7300 2000 4f00 7200 7400 6500 7300  e.s. .O.r.t.e.s.
+00000f00: 2000 6500 6900 6e00 2e08 0000 0000 0600   .e.i.n.........
+00000f10: 0000 2245 6e74 6572 2061 2066 756c 6c20  .."Enter a full 
+00000f20: 6e61 6d65 206f 6620 7468 6520 6c6f 6361  name of the loca
+00000f30: 7469 6f6e 2e07 0000 000a 4164 6472 6573  tion......Addres
+00000f40: 7354 6162 0103 0000 00aa 0047 0065 0062  sTab.......G.e.b
+00000f50: 0065 006e 0020 0053 0069 0065 0020 0064  .e.n. .S.i.e. .d
+00000f60: 0065 006e 0020 0061 0075 0073 0020 0032  .e.n. .a.u.s. .2
+00000f70: 0020 006f 0064 0065 0072 0020 0033 0020  . .o.d.e.r. .3. 
+00000f80: 0042 0075 0063 0068 0073 0074 0061 0062  .B.u.c.h.s.t.a.b
+00000f90: 0065 006e 0020 0062 0065 0073 0074 0065  .e.n. .b.e.s.t.e
+00000fa0: 0068 0065 006e 0064 0065 006e 0020 0049  .h.e.n.d.e.n. .I
+00000fb0: 0053 004f 002d 0033 0031 0036 0036 002d  .S.O.-.3.1.6.6.-
+00000fc0: 004c 00e4 006e 0064 0065 0072 0063 006f  .L...n.d.e.r.c.o
+00000fd0: 0064 0065 0020 0064 0065 0073 0020 004c  .d.e. .d.e.s. .L
+00000fe0: 0061 006e 0064 0065 0073 0020 0065 0069  .a.n.d.e.s. .e.i
+00000ff0: 006e 002e 0800 0000 0006 0000 003d 456e  .n...........=En
+00001000: 7465 7220 7468 6520 3220 6f72 2033 206c  ter the 2 or 3 l
+00001010: 6574 7465 7220 4953 4f20 3331 3636 2063  etter ISO 3166 c
+00001020: 6f75 6e74 7279 2063 6f64 6520 6f66 2074  ountry code of t
+00001030: 6865 2063 6f75 6e74 7279 2e07 0000 000a  he country......
+00001040: 4164 6472 6573 7354 6162 0103 0000 008a  AddressTab......
+00001050: 0047 0065 0062 0065 006e 0020 0053 0069  .G.e.b.e.n. .S.i
+00001060: 0065 0020 0064 0069 0065 0020 0044 0065  .e. .d.i.e. .D.e
+00001070: 0074 0061 0069 006c 0073 0020 007a 0075  .t.a.i.l.s. .z.u
+00001080: 0020 0064 0065 006d 0020 004f 0072 0074  . .d.e.m. .O.r.t
+00001090: 0020 0065 0069 006e 002c 0020 0061 006e  . .e.i.n.,. .a.n
+000010a0: 0020 0064 0065 006d 0020 0064 0061 0073  . .d.e.m. .d.a.s
+000010b0: 0020 0042 0069 006c 0064 0020 0065 0072  . .B.i.l.d. .e.r
+000010c0: 0073 0074 0065 006c 006c 0074 0020 0077  .s.t.e.l.l.t. .w
+000010d0: 0075 0072 0064 0065 002e 0800 0000 0006  .u.r.d.e........
+000010e0: 0000 0040 456e 7465 7220 7468 6520 6465  ...@Enter the de
+000010f0: 7461 696c 7320 6162 6f75 7420 6120 6c6f  tails about a lo
+00001100: 6361 7469 6f6e 2077 6865 7265 2074 6869  cation where thi
+00001110: 7320 696d 6167 6520 7761 7320 6372 6561  s image was crea
+00001120: 7465 642e 0700 0000 0a41 6464 7265 7373  ted......Address
+00001130: 5461 6201 0300 0000 9000 4700 6500 6200  Tab.......G.e.b.
+00001140: 6500 6e00 2000 5300 6900 6500 2000 6400  e.n. .S.i.e. .d.
+00001150: 6900 6500 2000 4400 6500 7400 6100 6900  i.e. .D.e.t.a.i.
+00001160: 6c00 7300 2000 7a00 7500 2000 6500 6900  l.s. .z.u. .e.i.
+00001170: 6e00 6500 6d00 2000 4f00 7200 7400 2000  n.e.m. .O.r.t. .
+00001180: 6500 6900 6e00 2c00 2000 6400 6500 7200  e.i.n.,. .d.e.r.
+00001190: 2000 6900 6e00 2000 6400 6900 6500 7300   .i.n. .d.i.e.s.
+000011a0: 6500 6d00 2000 4200 6900 6c00 6400 2000  e.m. .B.i.l.d. .
+000011b0: 6700 6500 7a00 6500 6900 6700 7400 2000  g.e.z.e.i.g.t. .
+000011c0: 7700 6900 7200 6400 2e08 0000 0000 0600  w.i.r.d.........
+000011d0: 0000 4045 6e74 6572 2074 6865 2064 6574  ..@Enter the det
+000011e0: 6169 6c73 2061 626f 7574 2061 206c 6f63  ails about a loc
+000011f0: 6174 696f 6e20 7768 6963 6820 6973 2073  ation which is s
+00001200: 686f 776e 2069 6e20 7468 6973 2069 6d61  hown in this ima
+00001210: 6765 2e07 0000 000a 4164 6472 6573 7354  ge......AddressT
+00001220: 6162 0103 0000 0044 0047 0065 0062 0065  ab.....D.G.e.b.e
+00001230: 006e 0020 0053 0069 0065 0020 0064 0065  .n. .S.i.e. .d.e
+00001240: 006e 0020 004e 0061 006d 0065 006e 0020  .n. .N.a.m.e.n. 
+00001250: 0064 0065 0072 0020 0053 0074 0061 0064  .d.e.r. .S.t.a.d
+00001260: 0074 0020 0065 0069 006e 002e 0800 0000  .t. .e.i.n......
+00001270: 0006 0000 001b 456e 7465 7220 7468 6520  ......Enter the 
+00001280: 6e61 6d65 206f 6620 7468 6520 6369 7479  name of the city
+00001290: 2e07 0000 000a 4164 6472 6573 7354 6162  ......AddressTab
+000012a0: 0103 0000 0046 0047 0065 0062 0065 006e  .....F.G.e.b.e.n
+000012b0: 0020 0053 0069 0065 0020 0064 0065 006e  . .S.i.e. .d.e.n
+000012c0: 0020 004e 0061 006d 0065 006e 0020 0064  . .N.a.m.e.n. .d
+000012d0: 0065 0073 0020 004c 0061 006e 0064 0065  .e.s. .L.a.n.d.e
+000012e0: 0073 0020 0065 0069 006e 002e 0800 0000  .s. .e.i.n......
+000012f0: 0006 0000 001e 456e 7465 7220 7468 6520  ......Enter the 
+00001300: 6e61 6d65 206f 6620 7468 6520 636f 756e  name of the coun
+00001310: 7472 792e 0700 0000 0a41 6464 7265 7373  try......Address
+00001320: 5461 6201 0300 0000 7400 4700 6500 6200  Tab.....t.G.e.b.
+00001330: 6500 6e00 2000 5300 6900 6500 2000 6400  e.n. .S.i.e. .d.
+00001340: 6500 6e00 2000 4e00 6100 6d00 6500 6e00  e.n. .N.a.m.e.n.
+00001350: 2000 6400 6500 7200 2000 5000 7200 6f00   .d.e.r. .P.r.o.
+00001360: 7600 6900 6e00 7a00 2000 6f00 6400 6500  v.i.n.z. .o.d.e.
+00001370: 7200 2000 6400 6500 7300 2000 4200 7500  r. .d.e.s. .B.u.
+00001380: 6e00 6400 6500 7300 6c00 6100 6e00 6400  n.d.e.s.l.a.n.d.
+00001390: 6500 7300 2000 6500 6900 6e00 2e08 0000  e.s. .e.i.n.....
+000013a0: 0000 0600 0000 2845 6e74 6572 2074 6865  ......(Enter the
+000013b0: 206e 616d 6520 6f66 2074 6865 2070 726f   name of the pro
+000013c0: 7669 6e63 6520 6f72 2073 7461 7465 2e07  vince or state..
+000013d0: 0000 000a 4164 6472 6573 7354 6162 0103  ....AddressTab..
+000013e0: 0000 004c 0047 0065 0062 0065 006e 0020  ...L.G.e.b.e.n. 
+000013f0: 0053 0069 0065 0020 0064 0065 006e 0020  .S.i.e. .d.e.n. 
+00001400: 004e 0061 006d 0065 006e 0020 0064 0065  .N.a.m.e.n. .d.e
+00001410: 0073 0020 0055 006e 0074 0065 0072 006f  .s. .U.n.t.e.r.o
+00001420: 0072 0074 0073 0020 0065 0069 006e 002e  .r.t.s. .e.i.n..
+00001430: 0800 0000 0006 0000 0022 456e 7465 7220  ........."Enter 
+00001440: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
+00001450: 7375 626c 6f63 6174 696f 6e2e 0700 0000  sublocation.....
+00001460: 0a41 6464 7265 7373 5461 6201 0300 0000  .AddressTab.....
+00001470: 4e00 4700 6500 6200 6500 6e00 2000 5300  N.G.e.b.e.n. .S.
+00001480: 6900 6500 2000 6400 6500 6e00 2000 4e00  i.e. .d.e.n. .N.
+00001490: 6100 6d00 6500 6e00 2000 6400 6500 7200  a.m.e.n. .d.e.r.
+000014a0: 2000 5700 6500 6c00 7400 7200 6500 6700   .W.e.l.t.r.e.g.
+000014b0: 6900 6f00 6e00 2000 6500 6900 6e00 2e08  i.o.n. .e.i.n...
+000014c0: 0000 0000 0600 0000 2345 6e74 6572 2074  ........#Enter t
+000014d0: 6865 206e 616d 6520 6f66 2074 6865 2077  he name of the w
+000014e0: 6f72 6c64 2072 6567 696f 6e2e 0700 0000  orld region.....
+000014f0: 0a41 6464 7265 7373 5461 6201 0300 0000  .AddressTab.....
+00001500: 4800 4700 6500 6f00 6400 6100 7400 6100  H.G.e.o.d.a.t.a.
+00001510: 2000 a900 2000 4f00 7000 6500 6e00 5300   ... .O.p.e.n.S.
+00001520: 7400 7200 6500 6500 7400 4d00 6100 7000  t.r.e.e.t.M.a.p.
+00001530: 2000 6300 6f00 6e00 7400 7200 6900 6200   .c.o.n.t.r.i.b.
+00001540: 7500 7400 6f00 7200 7308 0000 0000 0600  u.t.o.r.s.......
+00001550: 0000 2547 656f 6461 7461 20c2 a920 4f70  ..%Geodata .. Op
+00001560: 656e 5374 7265 6574 4d61 7020 636f 6e74  enStreetMap cont
+00001570: 7269 6275 746f 7273 0700 0000 0a41 6464  ributors.....Add
+00001580: 7265 7373 5461 6201 0300 0000 4c00 4100  ressTab.....L.A.
+00001590: 6400 7200 6500 7300 7300 6500 2000 6100  d.r.e.s.s.e. .a.
+000015a0: 7500 7300 2000 4200 7200 6500 6900 7400  u.s. .B.r.e.i.t.
+000015b0: 6500 2000 7500 6e00 6400 2000 4c00 e400  e. .u.n.d. .L...
+000015c0: 6e00 6700 6500 2000 6500 7200 6d00 6900  n.g.e. .e.r.m.i.
+000015d0: 7400 7400 6500 6c00 6e08 0000 0000 0600  t.t.e.l.n.......
+000015e0: 0000 1a47 6574 2061 6464 7265 7373 2066  ...Get address f
+000015f0: 726f 6d20 6c61 742c 206c 6f6e 6707 0000  rom lat, long...
+00001600: 000a 4164 6472 6573 7354 6162 0103 0000  ..AddressTab....
+00001610: 0008 004e 0061 006d 0065 0800 0000 0006  ...N.a.m.e......
+00001620: 0000 0004 4e61 6d65 0700 0000 0a41 6464  ....Name.....Add
+00001630: 7265 7373 5461 6201 0300 0000 1400 4200  ressTab.......B.
+00001640: 7500 6e00 6400 6500 7300 6c00 6100 6e00  u.n.d.e.s.l.a.n.
+00001650: 6408 0000 0000 0600 0000 0850 726f 7669  d..........Provi
+00001660: 6e63 6507 0000 000a 4164 6472 6573 7354  nce.....AddressT
+00001670: 6162 0103 0000 000c 0052 0065 0067 0069  ab.......R.e.g.i
+00001680: 006f 006e 0800 0000 0006 0000 0006 5265  .o.n..........Re
+00001690: 6769 6f6e 0700 0000 0a41 6464 7265 7373  gion.....Address
+000016a0: 5461 6201 0300 0000 0c00 5300 7400 7200  Tab.......S.t.r.
+000016b0: 6100 df00 6508 0000 0000 0600 0000 0653  a...e..........S
+000016c0: 7472 6565 7407 0000 000a 4164 6472 6573  treet.....Addres
+000016d0: 7354 6162 0103 0000 000c 004b 0061 006d  sTab.......K.a.m
+000016e0: 0065 0072 0061 0800 0000 0006 0000 0006  .e.r.a..........
+000016f0: 6361 6d65 7261 0700 0000 0a41 6464 7265  camera.....Addre
+00001700: 7373 5461 6201 0300 0000 1a00 4200 6500  ssTab.......B.e.
+00001710: 7400 7200 6500 6600 6600 2000 7b00 6900  t.r.e.f.f. .{.i.
+00001720: 6400 7800 7d08 0000 0000 0600 0000 0d73  d.x.}..........s
+00001730: 7562 6a65 6374 207b 6964 787d 0700 0000  ubject {idx}....
+00001740: 0a41 6464 7265 7373 5461 6201 0300 0000  .AddressTab.....
+00001750: 3600 5000 6800 6f00 7400 6900 6e00 6900  6.P.h.o.t.i.n.i.
+00001760: 2d00 4600 6f00 7400 6f00 6d00 6500 7400  -.F.o.t.o.m.e.t.
+00001770: 6100 6400 6100 7400 6500 6e00 6500 6400  a.d.a.t.e.n.e.d.
+00001780: 6900 7400 6f00 7208 0000 0000 0600 0000  i.t.o.r.........
+00001790: 1d50 686f 7469 6e69 2070 686f 746f 206d  .Photini photo m
+000017a0: 6574 6164 6174 6120 6564 6974 6f72 0700  etadata editor..
+000017b0: 0000 0743 4c49 4865 6c70 0103 0000 0058  ...CLIHelp.....X
+000017c0: 0056 0065 0072 0077 0065 006e 0064 0075  .V.e.r.w.e.n.d.u
+000017d0: 006e 0067 003a 0020 0025 0070 0072 006f  .n.g.:. .%.p.r.o
+000017e0: 0067 0020 005b 006f 0070 0074 0069 006f  .g. .[.o.p.t.i.o
+000017f0: 006e 0073 005d 0020 005b 0066 0069 006c  .n.s.]. .[.f.i.l
+00001800: 0065 005f 006e 0061 006d 0065 002c 0020  .e._.n.a.m.e.,. 
+00001810: 002e 002e 002e 005d 0800 0000 0006 0000  .......]........
+00001820: 0027 5573 6167 653a 2025 7072 6f67 205b  .'Usage: %prog [
+00001830: 6f70 7469 6f6e 735d 205b 6669 6c65 5f6e  options] [file_n
+00001840: 616d 652c 202e 2e2e 5d07 0000 0007 434c  ame, ...].....CL
+00001850: 4948 656c 7001 0300 0000 5c00 4100 6e00  IHelp.....\.A.n.
+00001860: 7a00 6100 6800 6c00 2000 6400 6500 7200  z.a.h.l. .d.e.r.
+00001870: 2000 4500 6900 6e00 7400 7200 e400 6700   .E.i.n.t.r...g.
+00001880: 6500 2000 6900 6d00 2000 4600 6500 6800  e. .i.m. .F.e.h.
+00001890: 6c00 6500 7200 7000 7200 6f00 7400 6f00  l.e.r.p.r.o.t.o.
+000018a0: 6b00 6f00 6c00 6c00 2000 6500 7200 6800  k.o.l.l. .e.r.h.
+000018b0: f600 6800 6500 6e08 0000 0000 0600 0000  ..h.e.n.........
+000018c0: 2369 6e63 7265 6173 6520 6e75 6d62 6572  #increase number
+000018d0: 206f 6620 6c6f 6767 696e 6720 6d65 7373   of logging mess
+000018e0: 6167 6573 0700 0000 0743 4c49 4865 6c70  ages.....CLIHelp
+000018f0: 0103 0000 005e 004e 0065 0075 0065 0020  .....^.N.e.u.e. 
+00001900: 0046 0075 006e 006b 0074 0069 006f 006e  .F.u.n.k.t.i.o.n
+00001910: 0065 006e 0020 006f 0064 0065 0072 0020  .e.n. .o.d.e.r. 
+00001920: 0041 0050 0049 002d 0056 0065 0072 0073  .A.P.I.-.V.e.r.s
+00001930: 0069 006f 006e 0065 006e 0020 0061 0075  .i.o.n.e.n. .a.u
+00001940: 0073 0070 0072 006f 0062 0069 0065 0072  .s.p.r.o.b.i.e.r
+00001950: 0065 006e 0800 0000 0006 0000 0021 7465  .e.n.........!te
+00001960: 7374 206e 6577 2066 6561 7475 7265 7320  st new features 
+00001970: 6f72 2041 5049 2076 6572 7369 6f6e 7307  or API versions.
+00001980: 0000 0007 434c 4948 656c 7001 0300 0000  ....CLIHelp.....
+00001990: 3000 4200 6500 7300 6300 6800 7200 6500  0.B.e.s.c.h.r.e.
+000019a0: 6900 6200 6500 6e00 2600 6400 6500 2000  i.b.e.n.&.d.e. .
+000019b0: 4d00 6500 7400 6100 6400 6100 7400 6500  M.e.t.a.d.a.t.e.
+000019c0: 6e08 0000 0000 0600 0000 1526 4465 7363  n..........&Desc
+000019d0: 7269 7074 6976 6520 6d65 7461 6461 7461  riptive metadata
+000019e0: 0700 0000 0e44 6573 6372 6970 7469 7665  .....Descriptive
+000019f0: 5461 6201 0300 0000 1600 3c00 4600 6100  Tab.......<.F.a.
+00001a00: 7600 6f00 7200 6900 7400 6500 6e00 3e08  v.o.r.i.t.e.n.>.
+00001a10: 0000 0000 0600 0000 0c3c 6661 766f 7572  .........<favour
+00001a20: 6974 6573 3e07 0000 000e 4465 7363 7269  ites>.....Descri
+00001a30: 7074 6976 6554 6162 0103 0000 02ac 0045  ptiveTab.......E
+00001a40: 0069 006e 0065 0020 0064 0065 0074 0061  .i.n.e. .d.e.t.a
+00001a50: 0069 006c 006c 0069 0065 0072 0074 0065  .i.l.l.i.e.r.t.e
+00001a60: 0072 0065 0020 0074 0065 0078 0074 006c  .r.e. .t.e.x.t.l
+00001a70: 0069 0063 0068 0065 0020 0042 0065 0073  .i.c.h.e. .B.e.s
+00001a80: 0063 0068 0072 0065 0069 0062 0075 006e  .c.h.r.e.i.b.u.n
+00001a90: 0067 0020 0064 0065 0073 0020 005a 0077  .g. .d.e.s. .Z.w
+00001aa0: 0065 0063 006b 0073 0020 0075 006e 0064  .e.c.k.s. .u.n.d
+00001ab0: 0020 0064 0065 0072 0020 0042 0065 0064  . .d.e.r. .B.e.d
+00001ac0: 0065 0075 0074 0075 006e 0067 0020 0065  .e.u.t.u.n.g. .e
+00001ad0: 0069 006e 0065 0073 0020 0042 0069 006c  .i.n.e.s. .B.i.l
+00001ae0: 0064 0065 0073 002c 0020 0064 0069 0065  .d.e.s.,. .d.i.e
+00001af0: 0020 0064 0069 0065 0020 0064 0075 0072  . .d.i.e. .d.u.r
+00001b00: 0063 0068 0020 0064 0069 0065 0020 0045  .c.h. .d.i.e. .E
+00001b10: 0069 0067 0065 006e 0073 0063 0068 0061  .i.g.e.n.s.c.h.a
+00001b20: 0066 0074 0020 0041 006c 0074 002d 0054  .f.t. .A.l.t.-.T
+00001b30: 0065 0078 0074 0020 0028 0042 0061 0072  .e.x.t. .(.B.a.r
+00001b40: 0072 0069 0065 0072 0065 0066 0072 0065  .r.i.e.r.e.f.r.e
+00001b50: 0069 0068 0065 0069 0074 0029 0020 0062  .i.h.e.i.t.). .b
+00001b60: 0065 0072 0065 0069 0074 0067 0065 0073  .e.r.e.i.t.g.e.s
+00001b70: 0074 0065 006c 006c 0074 0065 006e 0020  .t.e.l.l.t.e.n. 
+00001b80: 0049 006e 0066 006f 0072 006d 0061 0074  .I.n.f.o.r.m.a.t
+00001b90: 0069 006f 006e 0065 006e 0020 0077 0065  .i.o.n.e.n. .w.e
+00001ba0: 0069 0074 0065 0072 0020 0061 0075 0073  .i.t.e.r. .a.u.s
+00001bb0: 0066 00fc 0068 0072 0074 002e 0020 0044  .f...h.r.t... .D
+00001bc0: 0069 0065 0073 0065 0020 0045 0069 0067  .i.e.s.e. .E.i.g
+00001bd0: 0065 006e 0073 0063 0068 0061 0066 0074  .e.n.s.c.h.a.f.t
+00001be0: 0020 0068 0061 0074 0020 006b 0065 0069  . .h.a.t. .k.e.i
+00001bf0: 006e 0065 0020 005a 0065 0069 0063 0068  .n.e. .Z.e.i.c.h
+00001c00: 0065 006e 0062 0065 0067 0072 0065 006e  .e.n.b.e.g.r.e.n
+00001c10: 007a 0075 006e 0067 0020 0075 006e 0064  .z.u.n.g. .u.n.d
+00001c20: 0020 0069 0073 0074 0020 006e 0069 0063  . .i.s.t. .n.i.c
+00001c30: 0068 0074 0020 0065 0072 0066 006f 0072  .h.t. .e.r.f.o.r
+00001c40: 0064 0065 0072 006c 0069 0063 0068 002c  .d.e.r.l.i.c.h.,
+00001c50: 0020 0077 0065 006e 006e 0020 0064 0061  . .w.e.n.n. .d.a
+00001c60: 0073 0020 0046 0065 006c 0064 0020 0041  .s. .F.e.l.d. .A
+00001c70: 006c 0074 002d 0054 0065 0078 0074 0020  .l.t.-.T.e.x.t. 
+00001c80: 0028 0042 0061 0072 0072 0069 0065 0072  .(.B.a.r.r.i.e.r
+00001c90: 0065 0066 0072 0065 0069 0068 0065 0069  .e.f.r.e.i.h.e.i
+00001ca0: 0074 0029 0020 0064 0061 0073 0020 0042  .t.). .d.a.s. .B
+00001cb0: 0069 006c 0064 0020 0061 0075 0073 0072  .i.l.d. .a.u.s.r
+00001cc0: 0065 0069 0063 0068 0065 006e 0064 0020  .e.i.c.h.e.n.d. 
+00001cd0: 0062 0065 0073 0063 0068 0072 0065 0069  .b.e.s.c.h.r.e.i
+00001ce0: 0062 0074 002e 002e 002e 0800 0000 0006  .b.t............
+00001cf0: 0000 0130 4120 6d6f 7265 2064 6574 6169  ...0A more detai
+00001d00: 6c65 6420 7465 7874 7561 6c20 6465 7363  led textual desc
+00001d10: 7269 7074 696f 6e20 6f66 2074 6865 2070  ription of the p
+00001d20: 7572 706f 7365 2061 6e64 206d 6561 6e69  urpose and meani
+00001d30: 6e67 206f 6620 616e 2069 6d61 6765 2074  ng of an image t
+00001d40: 6861 7420 656c 6162 6f72 6174 6573 206f  hat elaborates o
+00001d50: 6e20 7468 6520 696e 666f 726d 6174 696f  n the informatio
+00001d60: 6e20 7072 6f76 6964 6564 2062 7920 7468  n provided by th
+00001d70: 6520 416c 7420 5465 7874 2028 4163 6365  e Alt Text (Acce
+00001d80: 7373 6962 696c 6974 7929 2070 726f 7065  ssibility) prope
+00001d90: 7274 792e 2054 6869 7320 7072 6f70 6572  rty. This proper
+00001da0: 7479 2064 6f65 7320 6e6f 7420 6861 7665  ty does not have
+00001db0: 2061 2063 6861 7261 6374 6572 206c 696d   a character lim
+00001dc0: 6974 6174 696f 6e20 616e 6420 6973 206e  itation and is n
+00001dd0: 6f74 2072 6571 7569 7265 6420 6966 2074  ot required if t
+00001de0: 6865 2041 6c74 2054 6578 7420 2841 6363  he Alt Text (Acc
+00001df0: 6573 7369 6269 6c69 7479 2920 6669 656c  essibility) fiel
+00001e00: 6420 7375 6666 6963 6965 6e74 6c79 2064  d sufficiently d
+00001e10: 6573 6372 6962 6573 2074 6865 2069 6d61  escribes the ima
+00001e20: 6765 2e2e 0700 0000 0e44 6573 6372 6970  ge.......Descrip
+00001e30: 7469 7665 5461 6201 0300 0000 3600 4100  tiveTab.....6.A.
+00001e40: 6c00 7400 2d00 5400 6500 7800 7400 2000  l.t.-.T.e.x.t. .
+00001e50: 2800 4200 6100 7200 7200 6900 6500 7200  (.B.a.r.r.i.e.r.
+00001e60: 6500 6600 7200 6500 6900 6800 6500 6900  e.f.r.e.i.h.e.i.
+00001e70: 7400 2908 0000 0000 0600 0000 1841 6c74  t.)..........Alt
+00001e80: 2054 6578 7420 2841 6363 6573 7369 6269   Text (Accessibi
+00001e90: 6c69 7479 2907 0000 000e 4465 7363 7269  lity).....Descri
+00001ea0: 7074 6976 6554 6162 0103 0000 0018 0042  ptiveTab.......B
+00001eb0: 0065 0073 0063 0068 0072 0065 0069 0062  .e.s.c.h.r.e.i.b
+00001ec0: 0075 006e 0067 0800 0000 0006 0000 0015  .u.n.g..........
+00001ed0: 4465 7363 7269 7074 696f 6e20 2f20 4361  Description / Ca
+00001ee0: 7074 696f 6e07 0000 000e 4465 7363 7269  ption.....Descri
+00001ef0: 7074 6976 6554 6162 0103 0000 01b0 0047  ptiveTab.......G
+00001f00: 0065 0062 0065 006e 0020 0053 0069 0065  .e.b.e.n. .S.i.e
+00001f10: 0020 0065 0069 006e 0065 0020 201e 0042  . .e.i.n.e.  ..B
+00001f20: 0069 006c 0064 0075 006e 0074 0065 0072  .i.l.d.u.n.t.e.r
+00001f30: 0073 0063 0068 0072 0069 0066 0074 201c  .s.c.h.r.i.f.t .
+00001f40: 0020 0065 0069 006e 002c 0020 0064 0069  . .e.i.n.,. .d.i
+00001f50: 0065 0020 0064 0061 0073 0020 0057 0065  .e. .d.a.s. .W.e
+00001f60: 0072 002c 0020 0057 0061 0073 0020 0075  .r.,. .W.a.s. .u
+00001f70: 006e 0064 0020 0057 0061 0072 0075 006d  .n.d. .W.a.r.u.m
+00001f80: 0020 0064 0065 0073 0020 0047 0065 0073  . .d.e.s. .G.e.s
+00001f90: 0063 0068 0065 0068 0065 006e 0073 0020  .c.h.e.h.e.n.s. 
+00001fa0: 0061 0075 0066 0020 0064 0069 0065 0073  .a.u.f. .d.i.e.s
+00001fb0: 0065 006d 0020 0042 0069 006c 0064 0020  .e.m. .B.i.l.d. 
+00001fc0: 0062 0065 0073 0063 0068 0072 0065 0069  .b.e.s.c.h.r.e.i
+00001fd0: 0062 0074 002c 0020 0044 0069 0065 0073  .b.t.,. .D.i.e.s
+00001fe0: 0020 006b 0061 006e 006e 0020 004e 0061  . .k.a.n.n. .N.a
+00001ff0: 006d 0065 006e 0020 0076 006f 006e 0020  .m.e.n. .v.o.n. 
+00002000: 0050 0065 0072 0073 006f 006e 0065 006e  .P.e.r.s.o.n.e.n
+00002010: 0020 0075 006e 0064 002f 006f 0064 0065  . .u.n.d./.o.d.e
+00002020: 0072 0020 0069 0068 0072 0065 0020 0052  .r. .i.h.r.e. .R
+00002030: 006f 006c 006c 0065 0020 0069 006e 0020  .o.l.l.e. .i.n. 
+00002040: 0064 0065 0072 0020 0048 0061 006e 0064  .d.e.r. .H.a.n.d
+00002050: 006c 0075 006e 0067 002c 0020 0064 0069  .l.u.n.g.,. .d.i
+00002060: 0065 0020 0061 0075 0066 0020 0064 0065  .e. .a.u.f. .d.e
+00002070: 006d 0020 0042 0069 006c 0064 0020 0073  .m. .B.i.l.d. .s
+00002080: 0074 0061 0074 0074 0066 0069 006e 0064  .t.a.t.t.f.i.n.d
+00002090: 0065 0074 002c 0020 0062 0065 0069 006e  .e.t.,. .b.e.i.n
+000020a0: 0068 0061 006c 0074 0065 006e 002e 0800  .h.a.l.t.e.n....
+000020b0: 0000 0006 0000 00c2 456e 7465 7220 6120  ........Enter a 
+000020c0: 2263 6170 7469 6f6e 2220 6465 7363 7269  "caption" descri
+000020d0: 6269 6e67 2074 6865 2077 686f 2c20 7768  bing the who, wh
+000020e0: 6174 2c20 616e 6420 7768 7920 6f66 2077  at, and why of w
+000020f0: 6861 7420 6973 2068 6170 7065 6e69 6e67  hat is happening
+00002100: 2069 6e20 7468 6973 2069 6d61 6765 2c20   in this image, 
+00002110: 7468 6973 206d 6967 6874 2069 6e63 6c75  this might inclu
+00002120: 6465 206e 616d 6573 206f 6620 7065 6f70  de names of peop
+00002130: 6c65 2c20 616e 642f 6f72 2074 6865 6972  le, and/or their
+00002140: 2072 6f6c 6520 696e 2074 6865 2061 6374   role in the act
+00002150: 696f 6e20 7468 6174 2069 7320 7461 6b69  ion that is taki
+00002160: 6e67 2070 6c61 6365 2077 6974 6869 6e20  ng place within 
+00002170: 7468 6520 696d 6167 652e 0700 0000 0e44  the image......D
+00002180: 6573 6372 6970 7469 7665 5461 6201 0300  escriptiveTab...
+00002190: 0000 b000 4700 6500 6200 6500 6e00 2000  ....G.e.b.e.n. .
+000021a0: 5300 6900 6500 2000 6500 6900 6e00 6500  S.i.e. .e.i.n.e.
+000021b0: 2000 6b00 7500 7200 7a00 6500 2000 7600   .k.u.r.z.e. .v.
+000021c0: 6500 7200 f600 6600 6600 6500 6e00 7400  e.r...f.f.e.n.t.
+000021d0: 6c00 6900 6300 6800 7500 6e00 6700 7300  l.i.c.h.u.n.g.s.
+000021e0: 6600 e400 6800 6900 6700 6500 2000 5a00  f...h.i.g.e. .Z.
+000021f0: 7500 7300 6100 6d00 6d00 6500 6e00 6600  u.s.a.m.m.e.n.f.
+00002200: 6100 7300 7300 7500 6e00 6700 2000 6400  a.s.s.u.n.g. .d.
+00002210: 6500 7300 2000 4900 6e00 6800 6100 6c00  e.s. .I.n.h.a.l.
+00002220: 7400 7300 2000 6400 6500 7300 2000 4200  t.s. .d.e.s. .B.
+00002230: 6900 6c00 6400 6500 7300 2000 6500 6900  i.l.d.e.s. .e.i.
+00002240: 6e00 2e08 0000 0000 0600 0000 4b45 6e74  n...........KEnt
+00002250: 6572 2061 2062 7269 6566 2070 7562 6c69  er a brief publi
+00002260: 7368 6162 6c65 2073 796e 6f70 7369 7320  shable synopsis 
+00002270: 6f72 2073 756d 6d61 7279 206f 6620 7468  or summary of th
+00002280: 6520 636f 6e74 656e 7473 206f 6620 7468  e contents of th
+00002290: 6520 696d 6167 652e 0700 0000 0e44 6573  e image......Des
+000022a0: 6372 6970 7469 7665 5461 6201 0300 0000  criptiveTab.....
+000022b0: de00 4700 6500 6200 6500 6e00 2000 5300  ..G.e.b.e.n. .S.
+000022c0: 6900 6500 2000 6500 6900 6e00 6500 6e00  i.e. .e.i.n.e.n.
+000022d0: 2000 6b00 7500 7200 7a00 6500 6e00 2c00   .k.u.r.z.e.n.,.
+000022e0: 2000 7600 6500 7200 6200 6100 6c00 6500   .v.e.r.b.a.l.e.
+000022f0: 6e00 2000 7500 6e00 6400 2000 6d00 6500  n. .u.n.d. .m.e.
+00002300: 6e00 7300 6300 6800 6500 6e00 6c00 6500  n.s.c.h.e.n.l.e.
+00002310: 7300 6200 6100 7200 6500 6e00 2000 4e00  s.b.a.r.e.n. .N.
+00002320: 6100 6d00 6500 6e00 2000 6600 fc00 7200  a.m.e.n. .f...r.
+00002330: 2000 6400 6100 7300 2000 4200 6900 6c00   .d.a.s. .B.i.l.
+00002340: 6400 2000 6500 6900 6e00 2c00 2000 6400  d. .e.i.n.,. .d.
+00002350: 6500 7200 2000 6100 7500 6300 6800 2000  e.r. .a.u.c.h. .
+00002360: 6400 6500 7200 2000 4400 6100 7400 6500  d.e.r. .D.a.t.e.
+00002370: 6900 6e00 6100 6d00 6500 2000 7300 6500  i.n.a.m.e. .s.e.
+00002380: 6900 6e00 2000 6b00 6100 6e00 6e00 2e08  i.n. .k.a.n.n...
+00002390: 0000 0000 0600 0000 5645 6e74 6572 2061  ........VEnter a
+000023a0: 2073 686f 7274 2076 6572 6261 6c20 616e   short verbal an
+000023b0: 6420 6875 6d61 6e20 7265 6164 6162 6c65  d human readable
+000023c0: 206e 616d 6520 666f 7220 7468 6520 696d   name for the im
+000023d0: 6167 652c 2074 6869 7320 6d61 7920 6265  age, this may be
+000023e0: 2074 6865 2066 696c 6520 6e61 6d65 2e07   the file name..
+000023f0: 0000 000e 4465 7363 7269 7074 6976 6554  ....DescriptiveT
+00002400: 6162 0103 0000 0138 0047 0065 0062 0065  ab.....8.G.e.b.e
+00002410: 006e 0020 0053 0069 0065 0020 0065 0069  .n. .S.i.e. .e.i
+00002420: 006e 0065 0020 0062 0065 006c 0069 0065  .n.e. .b.e.l.i.e
+00002430: 0062 0069 0067 0065 0020 0041 006e 007a  .b.i.g.e. .A.n.z
+00002440: 0061 0068 006c 0020 0076 006f 006e 0020  .a.h.l. .v.o.n. 
+00002450: 0053 0063 0068 006c 00fc 0073 0073 0065  .S.c.h.l...s.s.e
+00002460: 006c 0077 00f6 0072 0074 0065 0072 006e  .l.w...r.t.e.r.n
+00002470: 002c 0020 0042 0065 0067 0072 0069 0066  .,. .B.e.g.r.i.f
+00002480: 0066 0065 006e 0020 006f 0064 0065 0072  .f.e.n. .o.d.e.r
+00002490: 0020 0050 0068 0072 0061 0073 0065 006e  . .P.h.r.a.s.e.n
+000024a0: 0020 0065 0069 006e 002c 0020 0064 0069  . .e.i.n.,. .d.i
+000024b0: 0065 0020 0064 0061 0073 0020 0054 0068  .e. .d.a.s. .T.h
+000024c0: 0065 006d 0061 0020 0064 0065 0073 0020  .e.m.a. .d.e.s. 
+000024d0: 0042 0069 006c 0064 0065 0073 0020 0061  .B.i.l.d.e.s. .a
+000024e0: 0075 0073 0064 0072 00fc 0063 006b 0065  .u.s.d.r...c.k.e
+000024f0: 006e 0020 0073 006f 006c 006c 0065 006e  .n. .s.o.l.l.e.n
+00002500: 002e 0020 0054 0072 0065 006e 006e 0065  ... .T.r.e.n.n.e
+00002510: 006e 0020 0053 0069 0065 0020 0073 0069  .n. .S.i.e. .s.i
+00002520: 0065 0020 006d 0069 0074 0020 003b 002d  .e. .m.i.t. .;.-
+00002530: 005a 0065 0069 0063 0068 0065 006e 002e  .Z.e.i.c.h.e.n..
+00002540: 0800 0000 0006 0000 0082 456e 7465 7220  ..........Enter 
+00002550: 616e 7920 6e75 6d62 6572 206f 6620 6b65  any number of ke
+00002560: 7977 6f72 6473 2c20 7465 726d 7320 6f72  ywords, terms or
+00002570: 2070 6872 6173 6573 2075 7365 6420 746f   phrases used to
+00002580: 2065 7870 7265 7373 2074 6865 2073 7562   express the sub
+00002590: 6a65 6374 206d 6174 7465 7220 696e 2074  ject matter in t
+000025a0: 6865 2069 6d61 6765 2e20 5365 7061 7261  he image. Separa
+000025b0: 7465 2074 6865 6d20 7769 7468 2022 3b22  te them with ";"
+000025c0: 2063 6861 7261 6374 6572 732e 0700 0000   characters.....
+000025d0: 0e44 6573 6372 6970 7469 7665 5461 6201  .DescriptiveTab.
+000025e0: 0300 0001 9a00 4700 6500 6200 6500 6e00  ......G.e.b.e.n.
+000025f0: 2000 5300 6900 6500 2000 6500 6900 6e00   .S.i.e. .e.i.n.
+00002600: 6500 6e00 2000 5400 6500 7800 7400 2000  e.n. .T.e.x.t. .
+00002610: 6500 6900 6e00 2c00 2000 6400 6500 7200  e.i.n.,. .d.e.r.
+00002620: 2000 6400 6100 7300 2000 4100 7500 7300   .d.a.s. .A.u.s.
+00002630: 7300 6500 6800 6500 6e00 2000 6400 6500  s.e.h.e.n. .d.e.
+00002640: 7300 2000 4200 6900 6c00 6400 6500 7300  s. .B.i.l.d.e.s.
+00002650: 2000 6100 7500 7300 2000 6500 6900 6e00   .a.u.s. .e.i.n.
+00002660: 6500 7200 2000 7600 6900 7300 7500 6500  e.r. .v.i.s.u.e.
+00002670: 6c00 6c00 6500 6e00 2000 5000 6500 7200  l.l.e.n. .P.e.r.
+00002680: 7300 7000 6500 6b00 7400 6900 7600 6500  s.p.e.k.t.i.v.e.
+00002690: 2000 6200 6500 7300 6300 6800 7200 6500   .b.e.s.c.h.r.e.
+000026a0: 6900 6200 7400 2c00 2000 7500 6e00 6400  i.b.t.,. .u.n.d.
+000026b0: 2000 6b00 6f00 6e00 7a00 6500 6e00 7400   .k.o.n.z.e.n.t.
+000026c0: 7200 6900 6500 7200 6500 6e00 2000 5300  r.i.e.r.e.n. .S.
+000026d0: 6900 6500 2000 7300 6900 6300 6800 2000  i.e. .s.i.c.h. .
+000026e0: 6400 6100 6200 6500 6900 2000 6100 7500  d.a.b.e.i. .a.u.
+000026f0: 6600 2000 4400 6500 7400 6100 6900 6c00  f. .D.e.t.a.i.l.
+00002700: 7300 2c00 2000 6400 6900 6500 2000 6600  s.,. .d.i.e. .f.
+00002710: fc00 7200 2000 6400 6500 6e00 2000 5a00  ..r. .d.e.n. .Z.
+00002720: 7700 6500 6300 6b00 2000 7500 6e00 6400  w.e.c.k. .u.n.d.
+00002730: 2000 6400 6900 6500 2000 4200 6500 6400   .d.i.e. .B.e.d.
+00002740: 6500 7500 7400 7500 6e00 6700 2000 6400  e.u.t.u.n.g. .d.
+00002750: 6500 7300 2000 4200 6900 6c00 6400 6500  e.s. .B.i.l.d.e.
+00002760: 7300 2000 7200 6500 6c00 6500 7600 6100  s. .r.e.l.e.v.a.
+00002770: 6e00 7400 2000 7300 6900 6e00 6400 2e08  n.t. .s.i.n.d...
+00002780: 0000 0000 0600 0000 9b45 6e74 6572 2074  .........Enter t
+00002790: 6578 7420 6465 7363 7269 6269 6e67 2074  ext describing t
+000027a0: 6865 2061 7070 6561 7261 6e63 6520 6f66  he appearance of
+000027b0: 2074 6865 2069 6d61 6765 2066 726f 6d20   the image from 
+000027c0: 6120 7669 7375 616c 2070 6572 7370 6563  a visual perspec
+000027d0: 7469 7665 2c20 666f 6375 7369 6e67 206f  tive, focusing o
+000027e0: 6e20 6465 7461 696c 7320 7468 6174 2061  n details that a
+000027f0: 7265 2072 656c 6576 616e 7420 746f 2074  re relevant to t
+00002800: 6865 2070 7572 706f 7365 2061 6e64 206d  he purpose and m
+00002810: 6561 6e69 6e67 206f 6620 7468 6520 696d  eaning of the im
+00002820: 6167 652e 0700 0000 0e44 6573 6372 6970  age......Descrip
+00002830: 7469 7665 5461 6201 0300 0000 5400 4500  tiveTab.....T.E.
+00002840: 7200 7700 6500 6900 7400 6500 7200 7400  r.w.e.i.t.e.r.t.
+00002850: 6500 2000 4200 6500 7300 6300 6800 7200  e. .B.e.s.c.h.r.
+00002860: 6500 6900 6200 7500 6e00 6700 2000 2800  e.i.b.u.n.g. .(.
+00002870: 4200 6100 7200 7200 6900 6500 7200 6500  B.a.r.r.i.e.r.e.
+00002880: 6600 7200 6500 6900 6800 6500 6900 7400  f.r.e.i.h.e.i.t.
+00002890: 2908 0000 0000 0600 0000 2445 7874 656e  ).........$Exten
+000028a0: 6465 6420 4465 7363 7269 7074 696f 6e20  ded Description 
+000028b0: 2841 6363 6573 7369 6269 6c69 7479 2907  (Accessibility).
+000028c0: 0000 000e 4465 7363 7269 7074 6976 6554  ....DescriptiveT
+000028d0: 6162 0103 0000 0016 00dc 0062 0065 0072  ab.........b.e.r
+000028e0: 0073 0063 0068 0072 0069 0066 0074 0800  .s.c.h.r.i.f.t..
+000028f0: 0000 0006 0000 0008 4865 6164 6c69 6e65  ........Headline
+00002900: 0700 0000 0e44 6573 6372 6970 7469 7665  .....Descriptive
+00002910: 5461 6201 0300 0000 1e00 5300 6300 6800  Tab.......S.c.h.
+00002920: 6c00 fc00 7300 7300 6500 6c00 7700 f600  l...s.s.e.l.w...
+00002930: 7200 7400 6500 7208 0000 0000 0600 0000  r.t.e.r.........
+00002940: 084b 6579 776f 7264 7307 0000 000e 4465  .Keywords.....De
+00002950: 7363 7269 7074 6976 6554 6162 0103 0000  scriptiveTab....
+00002960: 0012 0042 0065 0077 0065 0072 0074 0075  ...B.e.w.e.r.t.u
+00002970: 006e 0067 0800 0000 0006 0000 0006 5261  .n.g..........Ra
+00002980: 7469 6e67 0700 0000 0e44 6573 6372 6970  ting.....Descrip
+00002990: 7469 7665 5461 6201 0300 0000 2400 5400  tiveTab.....$.T.
+000029a0: 6900 7400 6500 6c00 2000 2f00 2000 4f00  i.t.e.l. ./. .O.
+000029b0: 6200 6a00 6500 6b00 7400 6e00 6100 6d00  b.j.e.k.t.n.a.m.
+000029c0: 6508 0000 0000 0600 0000 1354 6974 6c65  e..........Title
+000029d0: 202f 204f 626a 6563 7420 4e61 6d65 0700   / Object Name..
+000029e0: 0000 0e44 6573 6372 6970 7469 7665 5461  ...DescriptiveTa
+000029f0: 6201 0300 0000 1800 7a00 7500 7200 fc00  b.......z.u.r...
+00002a00: 6300 6b00 7700 6500 6900 7300 6500 6e08  c.k.w.e.i.s.e.n.
+00002a10: 0000 0000 0600 0000 0672 656a 6563 7407  .........reject.
+00002a20: 0000 000e 4465 7363 7269 7074 6976 6554  ....DescriptiveT
+00002a30: 6162 0103 0000 001c 0028 0077 0065 006e  ab.......(.w.e.n
+00002a40: 006e 0020 006d 00f6 0067 006c 0069 0063  .n. .m...g.l.i.c
+00002a50: 0068 0029 0800 0000 0006 0000 000f 2877  .h.)..........(w
+00002a60: 6865 6e20 706f 7373 6962 6c65 2907 0000  hen possible)...
+00002a70: 000c 4564 6974 5365 7474 696e 6773 0103  ..EditSettings..
+00002a80: 0000 001e 0049 006d 006d 0065 0072 0020  .....I.m.m.e.r. 
+00002a90: 0065 0072 0073 0074 0065 006c 006c 0065  .e.r.s.t.e.l.l.e
+00002aa0: 006e 0800 0000 0006 0000 000d 416c 7761  .n..........Alwa
+00002ab0: 7973 2063 7265 6174 6507 0000 000c 4564  ys create.....Ed
+00002ac0: 6974 5365 7474 696e 6773 0103 0000 001a  itSettings......
+00002ad0: 0049 006d 006d 0065 0072 0020 006c 00f6  .I.m.m.e.r. .l..
+00002ae0: 0073 0063 0068 0065 006e 0800 0000 0006  .s.c.h.e.n......
+00002af0: 0000 000d 416c 7761 7973 2064 656c 6574  ....Always delet
+00002b00: 6507 0000 000c 4564 6974 5365 7474 696e  e.....EditSettin
+00002b10: 6773 0103 0000 001e 0049 006d 006d 0065  gs.......I.m.m.e
+00002b20: 0072 0020 0073 0063 0068 0072 0065 0069  .r. .s.c.h.r.e.i
+00002b30: 0062 0065 006e 0800 0000 0006 0000 000c  .b.e.n..........
+00002b40: 416c 7761 7973 2077 7269 7465 0700 0000  Always write....
+00002b50: 0c45 6469 7453 6574 7469 6e67 7301 0300  .EditSettings...
+00002b60: 0000 3400 4500 7200 7300 7400 6500 6c00  ..4.E.r.s.t.e.l.
+00002b70: 6c00 6500 6e00 2c00 2000 6600 6100 6c00  l.e.n.,. .f.a.l.
+00002b80: 6c00 7300 2000 6e00 6f00 7400 7700 6500  l.s. .n.o.t.w.e.
+00002b90: 6e00 6400 6900 6708 0000 0000 0600 0000  n.d.i.g.........
+00002ba0: 1343 7265 6174 6520 6966 206e 6563 6573  .Create if neces
+00002bb0: 7361 7279 0700 0000 0c45 6469 7453 6574  sary.....EditSet
+00002bc0: 7469 6e67 7301 0300 0000 2a00 4c00 f600  tings.....*.L...
+00002bd0: 7300 6300 6800 6500 6e00 2c00 2000 7700  s.c.h.e.n.,. .w.
+00002be0: 6500 6e00 6e00 2000 6d00 f600 6700 6c00  e.n.n. .m...g.l.
+00002bf0: 6900 6300 6808 0000 0000 0600 0000 1444  i.c.h..........D
+00002c00: 656c 6574 6520 7768 656e 2070 6f73 7369  elete when possi
+00002c10: 626c 6507 0000 000c 4564 6974 5365 7474  ble.....EditSett
+00002c20: 696e 6773 0103 0000 0022 0044 0061 0074  ings.....".D.a.t
+00002c30: 0065 0069 002d 005a 0065 0069 0074 0073  .e.i.-.Z.e.i.t.s
+00002c40: 0074 0065 006d 0070 0065 006c 0800 0000  .t.e.m.p.e.l....
+00002c50: 0006 0000 000f 4669 6c65 2074 696d 6573  ......File times
+00002c60: 7461 6d70 7307 0000 000c 4564 6974 5365  tamps.....EditSe
+00002c70: 7474 696e 6773 0103 0000 0024 0049 0050  ttings.....$.I.P
+00002c80: 0054 0043 002d 0049 0049 004d 002d 004d  .T.C.-.I.I.M.-.M
+00002c90: 0065 0074 0061 0064 0061 0074 0065 006e  .e.t.a.d.a.t.e.n
+00002ca0: 0800 0000 0006 0000 0011 4950 5443 2d49  ..........IPTC-I
+00002cb0: 494d 206d 6574 6164 6174 6107 0000 000c  IM metadata.....
+00002cc0: 4564 6974 5365 7474 696e 6773 0103 0000  EditSettings....
+00002cd0: 0028 004f 0072 0069 0067 0069 006e 0061  .(.O.r.i.g.i.n.a
+00002ce0: 006c 0020 0062 0065 0069 0062 0065 0068  .l. .b.e.i.b.e.h
+00002cf0: 0061 006c 0074 0065 006e 0800 0000 0006  .a.l.t.e.n......
+00002d00: 0000 000d 4b65 6570 206f 7269 6769 6e61  ....Keep origina
+00002d10: 6c07 0000 000c 4564 6974 5365 7474 696e  l.....EditSettin
+00002d20: 6773 0103 0000 002c 0050 0068 006f 0074  gs.....,.P.h.o.t
+00002d30: 0069 006e 0069 003a 0020 0045 0069 006e  .i.n.i.:. .E.i.n
+00002d40: 0073 0074 0065 006c 006c 0075 006e 0067  .s.t.e.l.l.u.n.g
+00002d50: 0065 006e 0800 0000 0006 0000 0011 5068  .e.n..........Ph
+00002d60: 6f74 696e 693a 2073 6574 7469 6e67 7307  otini: settings.
+00002d70: 0000 000c 4564 6974 5365 7474 696e 6773  ....EditSettings
+00002d80: 0103 0000 0046 0042 0065 0069 006d 0020  .....F.B.e.i.m. 
+00002d90: 0053 0070 0065 0069 0063 0068 0065 0072  .S.p.e.i.c.h.e.r
+00002da0: 006e 0020 0064 0065 0072 0020 0044 0061  .n. .d.e.r. .D.a
+00002db0: 0074 0065 0069 0020 0065 0069 006e 0073  .t.e.i. .e.i.n.s
+00002dc0: 0074 0065 006c 006c 0065 006e 0800 0000  .t.e.l.l.e.n....
+00002dd0: 0006 0000 0019 5365 7420 746f 2077 6865  ......Set to whe
+00002de0: 6e20 6669 6c65 2069 7320 7361 7665 6407  n file is saved.
+00002df0: 0000 000c 4564 6974 5365 7474 696e 6773  ....EditSettings
+00002e00: 0103 0000 0056 0045 0069 006e 0073 0074  .....V.E.i.n.s.t
+00002e10: 0065 006c 006c 0065 006e 002c 0020 0077  .e.l.l.e.n.,. .w
+00002e20: 0061 006e 006e 0020 0064 0061 0073 0020  .a.n.n. .d.a.s. 
+00002e30: 0046 006f 0074 006f 0020 0061 0075 0066  .F.o.t.o. .a.u.f
+00002e40: 0067 0065 006e 006f 006d 006d 0065 006e  .g.e.n.o.m.m.e.n
+00002e50: 0020 0077 0075 0072 0064 0065 0800 0000  . .w.u.r.d.e....
+00002e60: 0006 0000 001b 5365 7420 746f 2077 6865  ......Set to whe
+00002e70: 6e20 7068 6f74 6f20 7761 7320 7461 6b65  n photo was take
+00002e80: 6e07 0000 000c 4564 6974 5365 7474 696e  n.....EditSettin
+00002e90: 6773 0103 0000 003e 0049 0050 0054 0043  gs.....>.I.P.T.C
+00002ea0: 002d 0049 0049 004d 002d 004c 00e4 006e  .-.I.I.M.-.L...n
+00002eb0: 0067 0065 006e 0067 0072 0065 006e 007a  .g.e.n.g.r.e.n.z
+00002ec0: 0065 006e 0020 0061 006e 007a 0065 0069  .e.n. .a.n.z.e.i
+00002ed0: 0067 0065 006e 0800 0000 0006 0000 001b  .g.e.n..........
+00002ee0: 5368 6f77 2049 5054 432d 4949 4d20 6c65  Show IPTC-IIM le
+00002ef0: 6e67 7468 206c 696d 6974 7307 0000 000c  ngth limits.....
+00002f00: 4564 6974 5365 7474 696e 6773 0103 0000  EditSettings....
+00002f10: 001e 0053 0069 0064 0065 0063 0061 0072  ...S.i.d.e.c.a.r
+00002f20: 002d 0044 0061 0074 0065 0069 0065 006e  .-.D.a.t.e.i.e.n
+00002f30: 0800 0000 0006 0000 000d 5369 6465 6361  ..........Sideca
+00002f40: 7220 6669 6c65 7307 0000 000c 4564 6974  r files.....Edit
+00002f50: 5365 7474 696e 6773 0103 0000 0032 0053  Settings.....2.S
+00002f60: 0063 0068 0072 0065 0069 0062 0065 006e  .c.h.r.e.i.b.e.n
+00002f70: 002c 0020 0077 0065 006e 006e 0020 0076  .,. .w.e.n.n. .v
+00002f80: 006f 0072 0068 0061 006e 0064 0065 006e  .o.r.h.a.n.d.e.n
+00002f90: 0800 0000 0006 0000 000f 5772 6974 6520  ..........Write 
+00002fa0: 6966 2065 7869 7374 7307 0000 000c 4564  if exists.....Ed
+00002fb0: 6974 5365 7474 696e 6773 0103 0000 002c  itSettings.....,
+00002fc0: 0049 006e 0020 0042 0069 006c 0064 0064  .I.n. .B.i.l.d.d
+00002fd0: 0061 0074 0065 0069 0020 0073 0063 0068  .a.t.e.i. .s.c.h
+00002fe0: 0072 0065 0069 0062 0065 006e 0800 0000  .r.e.i.b.e.n....
+00002ff0: 0006 0000 0013 5772 6974 6520 746f 2069  ......Write to i
+00003000: 6d61 6765 2066 696c 6507 0000 000c 4564  mage file.....Ed
+00003010: 6974 5365 7474 696e 6773 0103 0000 0022  itSettings....."
+00003020: 0026 0046 006c 0069 0063 006b 0072 0020  .&.F.l.i.c.k.r. 
+00003030: 0068 006f 0063 0068 006c 0061 0064 0065  .h.o.c.h.l.a.d.e
+00003040: 006e 0800 0000 0006 0000 000e 2646 6c69  .n..........&Fli
+00003050: 636b 7220 7570 6c6f 6164 0700 0000 0946  ckr upload.....F
+00003060: 6c69 636b 7254 6162 0103 0000 0066 0041  lickrTab.....f.A
+00003070: 006c 0062 0075 006d 0020 0077 0069 0072  .l.b.u.m. .w.i.r
+00003080: 0064 0020 0065 0072 0073 0074 0065 006c  .d. .e.r.s.t.e.l
+00003090: 006c 0074 002c 0020 0077 0065 006e 006e  .l.t.,. .w.e.n.n
+000030a0: 0020 0042 0069 006c 0064 0065 0072 0020  . .B.i.l.d.e.r. 
+000030b0: 0068 006f 0063 0068 0067 0065 006c 0061  .h.o.c.h.g.e.l.a
+000030c0: 0064 0065 006e 0020 0077 0075 0072 0064  .d.e.n. .w.u.r.d
+000030d0: 0065 006e 0800 0000 0006 0000 002e 416c  .e.n..........Al
+000030e0: 6275 6d20 7769 6c6c 2062 6520 6372 6561  bum will be crea
+000030f0: 7465 6420 7768 656e 2070 686f 746f 7320  ted when photos 
+00003100: 6172 6520 7570 6c6f 6164 6564 0700 0000  are uploaded....
+00003110: 0946 6c69 636b 7254 6162 0103 0000 0026  .FlickrTab.....&
+00003120: 004b 006f 006d 006d 0065 006e 0074 0061  .K.o.m.m.e.n.t.a
+00003130: 0072 0065 0020 007a 0075 006c 0061 0073  .r.e. .z.u.l.a.s
+00003140: 0073 0065 006e 0800 0000 0006 0000 0010  .s.e.n..........
+00003150: 416c 6c6f 7720 636f 6d6d 656e 7469 6e67  Allow commenting
+00003160: 0700 0000 0946 6c69 636b 7254 6162 0103  .....FlickrTab..
+00003170: 0000 003a 0045 0074 0069 006b 0065 0074  ...:.E.t.i.k.e.t
+00003180: 0074 0065 0020 0075 006e 0064 0020 004e  .t.e. .u.n.d. .N
+00003190: 006f 0074 0069 007a 0065 006e 0020 007a  .o.t.i.z.e.n. .z
+000031a0: 0075 006c 0061 0073 0073 0065 006e 0800  .u.l.a.s.s.e.n..
+000031b0: 0000 0006 0000 0014 416c 6c6f 7720 7461  ........Allow ta
+000031c0: 6773 2061 6e64 206e 6f74 6573 0700 0000  gs and notes....
+000031d0: 0946 6c69 636b 7254 6162 0103 0000 002a  .FlickrTab.....*
+000031e0: 004a 0065 0064 0065 0073 0020 0046 006c  .J.e.d.e.s. .F.l
+000031f0: 0069 0063 006b 0072 002d 004d 0069 0074  .i.c.k.r.-.M.i.t
+00003200: 0067 006c 0069 0065 0064 0800 0000 0006  .g.l.i.e.d......
+00003210: 0000 0011 416e 7920 466c 6963 6b72 206d  ....Any Flickr m
+00003220: 656d 6265 7207 0000 0009 466c 6963 6b72  ember.....Flickr
+00003230: 5461 6201 0300 0000 2000 4100 7200 7400  Tab..... .A.r.t.
+00003240: 2f00 4900 6c00 6c00 7500 7300 7400 7200  /.I.l.l.u.s.t.r.
+00003250: 6100 7400 6900 6f00 6e08 0000 0000 0600  a.t.i.o.n.......
+00003260: 0000 1041 7274 2f49 6c6c 7573 7472 6174  ...Art/Illustrat
+00003270: 696f 6e07 0000 0009 466c 6963 6b72 5461  ion.....FlickrTa
+00003280: 6201 0300 0000 3400 4100 6c00 6200 7500  b.....4.A.l.b.u.
+00003290: 6d00 6d00 6900 7400 6700 6c00 6900 6500  m.m.i.t.g.l.i.e.
+000032a0: 6400 7300 6300 6800 6100 6600 7400 2000  d.s.c.h.a.f.t. .
+000032b0: e400 6e00 6400 6500 7200 6e08 0000 0000  ..n.d.e.r.n.....
+000032c0: 0600 0000 1743 6861 6e67 6520 616c 6275  .....Change albu
+000032d0: 6d20 6d65 6d62 6572 7368 6970 0700 0000  m membership....
+000032e0: 0946 6c69 636b 7254 6162 0103 0000 0022  .FlickrTab....."
+000032f0: 0049 006e 0068 0061 006c 0074 0073 0074  .I.n.h.a.l.t.s.t
+00003300: 0079 0070 0020 00e4 006e 0064 0065 0072  .y.p. ...n.d.e.r
+00003310: 006e 0800 0000 0006 0000 0013 4368 616e  .n..........Chan
+00003320: 6765 2063 6f6e 7465 6e74 2074 7970 6507  ge content type.
+00003330: 0000 0009 466c 6963 6b72 5461 6201 0300  ....FlickrTab...
+00003340: 0000 3e00 4100 7500 7300 6200 6c00 6500  ..>.A.u.s.b.l.e.
+00003350: 6e00 6400 6500 6e00 2000 6100 7500 7300  n.d.e.n. .a.u.s.
+00003360: 2000 6400 6500 7200 2000 5300 7500 6300   .d.e.r. .S.u.c.
+00003370: 6800 6500 2000 e400 6e00 6400 6500 7200  h.e. ...n.d.e.r.
+00003380: 6e08 0000 0000 0600 0000 1743 6861 6e67  n..........Chang
+00003390: 6520 6869 6465 2066 726f 6d20 7365 6172  e hide from sear
+000033a0: 6368 0700 0000 0946 6c69 636b 7254 6162  ch.....FlickrTab
+000033b0: 0103 0000 001a 004c 0069 007a 0065 006e  .......L.i.z.e.n
+000033c0: 007a 0020 00e4 006e 0064 0065 0072 006e  .z. ...n.d.e.r.n
+000033d0: 0800 0000 0006 0000 000e 4368 616e 6765  ..........Change
+000033e0: 206c 6963 656e 6365 0700 0000 0946 6c69   licence.....Fli
+000033f0: 636b 7254 6162 0103 0000 002e 0053 0069  ckrTab.......S.i
+00003400: 0063 0068 0065 0072 0068 0065 0069 0074  .c.h.e.r.h.e.i.t
+00003410: 0073 0073 0074 0075 0066 0065 0020 00e4  .s.s.t.u.f.e. ..
+00003420: 006e 0064 0065 0072 006e 0800 0000 0006  .n.d.e.r.n......
+00003430: 0000 0013 4368 616e 6765 2073 6166 6574  ....Change safet
+00003440: 7920 6c65 7665 6c07 0000 0009 466c 6963  y level.....Flic
+00003450: 6b72 5461 6201 0300 0000 2600 5300 6900  krTab.....&.S.i.
+00003460: 6300 6800 7400 6200 6100 7200 6b00 6500  c.h.t.b.a.r.k.e.
+00003470: 6900 7400 2000 e400 6e00 6400 6500 7200  i.t. ...n.d.e.r.
+00003480: 6e08 0000 0000 0600 0000 1643 6861 6e67  n..........Chang
+00003490: 6520 7669 6577 696e 6720 7072 6976 6163  e viewing privac
+000034a0: 7907 0000 0009 466c 6963 6b72 5461 6201  y.....FlickrTab.
+000034b0: 0300 0000 8000 c400 6e00 6400 6500 7200  ........n.d.e.r.
+000034c0: 6e00 2c00 2000 7700 6500 7200 2000 6b00  n.,. .w.e.r. .k.
+000034d0: 6f00 6d00 6d00 6500 6e00 7400 6900 6500  o.m.m.e.n.t.i.e.
+000034e0: 7200 6500 6e00 2000 6f00 6400 6500 7200  r.e.n. .o.d.e.r.
+000034f0: 2000 7400 6100 6700 6700 6500 6e00 2000   .t.a.g.g.e.n. .
+00003500: 6400 6100 7200 6600 2000 2800 7500 6e00  d.a.r.f. .(.u.n.
+00003510: 6400 2000 6400 6900 6500 2000 5300 6900  d. .d.i.e. .S.i.
+00003520: 6300 6800 7400 6200 6100 7200 6b00 6500  c.h.t.b.a.r.k.e.
+00003530: 6900 7400 2908 0000 0000 0600 0000 3343  i.t.).........3C
+00003540: 6861 6e67 6520 7768 6f20 6361 6e20 636f  hange who can co
+00003550: 6d6d 656e 7420 6f72 2074 6167 2028 616e  mment or tag (an
+00003560: 6420 7669 6577 696e 6720 7072 6976 6163  d viewing privac
+00003570: 7929 0700 0000 0946 6c69 636b 7254 6162  y).....FlickrTab
+00003580: 0103 0000 0014 0049 006e 0068 0061 006c  .......I.n.h.a.l
+00003590: 0074 0073 0074 0079 0070 0800 0000 0006  .t.s.t.y.p......
+000035a0: 0000 000c 436f 6e74 656e 7420 7479 7065  ....Content type
+000035b0: 0700 0000 0946 6c69 636b 7254 6162 0103  .....FlickrTab..
+000035c0: 0000 0018 0042 0065 0073 0063 0068 0072  .....B.e.s.c.h.r
+000035d0: 0065 0069 0062 0075 006e 0067 0800 0000  .e.i.b.u.n.g....
+000035e0: 0006 0000 000b 4465 7363 7269 7074 696f  ......Descriptio
+000035f0: 6e07 0000 0009 466c 6963 6b72 5461 6201  n.....FlickrTab.
+00003600: 0300 0000 0e00 4600 6100 6d00 6900 6c00  ......F.a.m.i.l.
+00003610: 6900 6508 0000 0000 0600 0000 0646 616d  i.e..........Fam
+00003620: 696c 7907 0000 0009 466c 6963 6b72 5461  ily.....FlickrTa
+00003630: 6201 0300 0000 0c00 4600 6c00 6900 6300  b.......F.l.i.c.
+00003640: 6b00 7208 0000 0000 0600 0000 0646 6c69  k.r..........Fli
+00003650: 636b 7207 0000 0009 466c 6963 6b72 5461  ckr.....FlickrTa
+00003660: 6201 0300 0000 0e00 4600 7200 6500 7500  b.......F.r.e.u.
+00003670: 6e00 6400 6508 0000 0000 0600 0000 0746  n.d.e..........F
+00003680: 7269 656e 6473 0700 0000 0946 6c69 636b  riends.....Flick
+00003690: 7254 6162 0103 0000 0026 0046 0072 0065  rTab.....&.F.r.e
+000036a0: 0075 006e 0064 0065 0020 0075 006e 0064  .u.n.d.e. .u.n.d
+000036b0: 0020 0046 0061 006d 0069 006c 0069 0065  . .F.a.m.i.l.i.e
+000036c0: 0800 0000 0006 0000 0010 4672 6965 6e64  ..........Friend
+000036d0: 7320 2620 6661 6d69 6c79 0700 0000 0946  s & family.....F
+000036e0: 6c69 636b 7254 6162 0103 0000 0030 0041  lickrTab.....0.A
+000036f0: 0075 0073 0020 0064 0065 0072 0020 0053  .u.s. .d.e.r. .S
+00003700: 0075 0063 0068 0065 0020 0061 0075 0073  .u.c.h.e. .a.u.s
+00003710: 0062 006c 0065 006e 0064 0065 006e 0800  .b.l.e.n.d.e.n..
+00003720: 0000 0006 0000 0010 4869 6465 2066 726f  ........Hide fro
+00003730: 6d20 7365 6172 6368 0700 0000 0946 6c69  m search.....Fli
+00003740: 636b 7254 6162 0103 0000 000c 004c 0069  ckrTab.......L.i
+00003750: 007a 0065 006e 007a 0800 0000 0006 0000  .z.e.n.z........
+00003760: 0007 4c69 6365 6e63 6507 0000 0009 466c  ..Licence.....Fl
+00003770: 6963 6b72 5461 6201 0300 0000 0a00 4d00  ickrTab.......M.
+00003780: e400 df00 6900 6708 0000 0000 0600 0000  ....i.g.........
+00003790: 084d 6f64 6572 6174 6507 0000 0009 466c  .Moderate.....Fl
+000037a0: 6963 6b72 5461 6201 0300 0000 1600 4e00  ickrTab.......N.
+000037b0: 6500 7500 6500 7300 2000 4100 6c00 6200  e.u.e.s. .A.l.b.
+000037c0: 7500 6d08 0000 0000 0600 0000 094e 6577  u.m..........New
+000037d0: 2061 6c62 756d 0700 0000 0946 6c69 636b   album.....Flick
+000037e0: 7254 6162 0103 0000 001c 004e 0075 0072  rTab.......N.u.r
+000037f0: 0020 0069 0063 0068 0020 0073 0065 006c  . .i.c.h. .s.e.l
+00003800: 0062 0073 0074 0800 0000 0006 0000 0008  .b.s.t..........
+00003810: 4f6e 6c79 2079 6f75 0700 0000 0946 6c69  Only you.....Fli
+00003820: 636b 7254 6162 0103 0000 0034 0050 0065  ckrTab.....4.P.e
+00003830: 0072 0073 006f 006e 0065 006e 002c 0020  .r.s.o.n.e.n.,. 
+00003840: 0064 0065 006e 0065 006e 0020 0053 0069  .d.e.n.e.n. .S.i
+00003850: 0065 0020 0066 006f 006c 0067 0065 006e  .e. .f.o.l.g.e.n
+00003860: 0800 0000 0006 0000 0011 5065 6f70 6c65  ..........People
+00003870: 2079 6f75 2066 6f6c 6c6f 7707 0000 0009   you follow.....
+00003880: 466c 6963 6b72 5461 6201 0300 0000 0800  FlickrTab.......
+00003890: 4600 6f00 7400 6f08 0000 0000 0600 0000  F.o.t.o.........
+000038a0: 0550 686f 746f 0700 0000 0946 6c69 636b  .Photo.....Flick
+000038b0: 7254 6162 0103 0000 000c 0050 0072 0069  rTab.......P.r.i
+000038c0: 0076 0061 0074 0800 0000 0006 0000 0007  .v.a.t..........
+000038d0: 5072 6976 6174 6507 0000 0009 466c 6963  Private.....Flic
+000038e0: 6b72 5461 6201 0300 0000 1400 d600 6600  krTab.........f.
+000038f0: 6600 6500 6e00 7400 6c00 6900 6300 6808  f.e.n.t.l.i.c.h.
+00003900: 0000 0000 0600 0000 0650 7562 6c69 6307  .........Public.
+00003910: 0000 0009 466c 6963 6b72 5461 6201 0300  ....FlickrTab...
+00003920: 0000 2400 4d00 6500 7400 6100 6400 6100  ..$.M.e.t.a.d.a.
+00003930: 7400 6500 6e00 2000 6500 7200 7300 6500  t.e.n. .e.r.s.e.
+00003940: 7400 7a00 6500 6e08 0000 0000 0600 0000  t.z.e.n.........
+00003950: 1052 6570 6c61 6365 206d 6574 6164 6174  .Replace metadat
+00003960: 6107 0000 0009 466c 6963 6b72 5461 6201  a.....FlickrTab.
+00003970: 0300 0000 1a00 4500 6900 6e00 6700 6500  ......E.i.n.g.e.
+00003980: 7300 6300 6800 7200 e400 6e00 6b00 7408  s.c.h.r...n.k.t.
+00003990: 0000 0000 0600 0000 0a52 6573 7472 6963  .........Restric
+000039a0: 7465 6407 0000 0009 466c 6963 6b72 5461  ted.....FlickrTa
+000039b0: 6201 0300 0000 0c00 5300 6900 6300 6800  b.......S.i.c.h.
+000039c0: 6500 7208 0000 0000 0600 0000 0453 6166  e.r..........Saf
+000039d0: 6507 0000 0009 466c 6963 6b72 5461 6201  e.....FlickrTab.
+000039e0: 0300 0000 2000 5300 6900 6300 6800 6500  .... .S.i.c.h.e.
+000039f0: 7200 6800 6500 6900 7400 7300 7300 7400  r.h.e.i.t.s.s.t.
+00003a00: 7500 6600 6508 0000 0000 0600 0000 0c53  u.f.e..........S
+00003a10: 6166 6574 7920 6c65 7665 6c07 0000 0009  afety level.....
+00003a20: 466c 6963 6b72 5461 6201 0300 0000 1c00  FlickrTab.......
+00003a30: 4200 6900 6c00 6400 7300 6300 6800 6900  B.i.l.d.s.c.h.i.
+00003a40: 7200 6d00 6600 6f00 7400 6f08 0000 0000  r.m.f.o.t.o.....
+00003a50: 0600 0000 0a53 6372 6565 6e73 686f 7407  .....Screenshot.
+00003a60: 0000 0009 466c 6963 6b72 5461 6201 0300  ....FlickrTab...
+00003a70: 0000 1e00 5300 7900 6e00 6300 6800 7200  ....S.y.n.c.h.r.
+00003a80: 6f00 6e00 6900 7300 6900 6500 7200 6500  o.n.i.s.i.e.r.e.
+00003a90: 6e08 0000 0000 0600 0000 0b53 796e 6368  n..........Synch
+00003aa0: 726f 6e69 7365 0700 0000 0946 6c69 636b  ronise.....Flick
+00003ab0: 7254 6162 0103 0000 000a 0054 0069 0074  rTab.......T.i.t
+00003ac0: 0065 006c 0800 0000 0006 0000 0005 5469  .e.l..........Ti
+00003ad0: 746c 6507 0000 0009 466c 6963 6b72 5461  tle.....FlickrTa
+00003ae0: 6201 0300 0000 2a00 5300 6900 6300 6800  b.....*.S.i.c.h.
+00003af0: 7400 6200 6100 7200 6b00 6500 6900 7400  t.b.a.r.k.e.i.t.
+00003b00: 7300 6f00 7000 7400 6900 6f00 6e00 6500  s.o.p.t.i.o.n.e.
+00003b10: 6e08 0000 0000 0600 0000 0f56 6965 7769  n..........Viewi
+00003b20: 6e67 2070 7269 7661 6379 0700 0000 0946  ng privacy.....F
+00003b30: 6c69 636b 7254 6162 0103 0000 0028 0056  lickrTab.....(.V
+00003b40: 0069 0072 0074 0075 0065 006c 006c 0065  .i.r.t.u.e.l.l.e
+00003b50: 0020 0046 006f 0074 006f 0067 0072 0061  . .F.o.t.o.g.r.a
+00003b60: 0066 0069 0065 0800 0000 0006 0000 0013  .f.i.e..........
+00003b70: 5669 7274 7561 6c20 5068 6f74 6f67 7261  Virtual Photogra
+00003b80: 7068 7907 0000 0009 466c 6963 6b72 5461  phy.....FlickrTa
+00003b90: 6201 0300 0000 1400 4100 6c00 6200 7500  b.......A.l.b.u.
+00003ba0: 6d00 7400 6900 7400 6500 6c08 0000 0000  m.t.i.t.e.l.....
+00003bb0: 0600 0000 0b41 6c62 756d 2074 6974 6c65  .....Album title
+00003bc0: 0700 0000 0f47 6f6f 676c 6550 686f 746f  .....GooglePhoto
+00003bd0: 7354 6162 0103 0000 0122 0044 0069 0065  sTab.....".D.i.e
+00003be0: 0020 0044 0061 0074 0065 0069 0020 201e  . .D.a.t.e.i.  .
+00003bf0: 007b 0066 0069 006c 0065 005f 006e 0061  .{.f.i.l.e._.n.a
+00003c00: 006d 0065 007d 201c 0020 0069 0073 0074  .m.e.} .. .i.s.t
+00003c10: 0020 0067 0072 00f6 00df 0065 0072 0020  . .g.r.....e.r. 
+00003c20: 0061 006c 0073 0020 0032 0035 00a0 004d  .a.l.s. .2.5...M
+00003c30: 0042 002e 0020 0048 006f 0063 0068 006c  .B... .H.o.c.h.l
+00003c40: 0061 0064 0065 006e 0020 006d 0069 0074  .a.d.e.n. .m.i.t
+00003c50: 0020 0050 0068 006f 0074 0069 006e 0069  . .P.h.o.t.i.n.i
+00003c60: 0020 0077 0069 0072 0064 0020 0069 006e  . .w.i.r.d. .i.n
+00003c70: 0020 0069 0068 0072 0065 006d 0020 0047  . .i.h.r.e.m. .G
+00003c80: 006f 006f 0067 006c 0065 002d 004b 006f  .o.o.g.l.e.-.K.o
+00003c90: 006e 0074 006f 0020 0061 006c 0073 0020  .n.t.o. .a.l.s. 
+00003ca0: 0062 0065 006c 0065 0067 0074 0065 0072  .b.e.l.e.g.t.e.r
+00003cb0: 0020 0053 0070 0065 0069 0063 0068 0065  . .S.p.e.i.c.h.e
+00003cc0: 0072 0020 0067 0065 007a 00e4 0068 006c  .r. .g.e.z...h.l
+00003cd0: 0074 002e 0020 0054 0072 006f 0074 007a  .t... .T.r.o.t.z
+00003ce0: 0064 0065 006d 0020 0068 006f 0063 0068  .d.e.m. .h.o.c.h
+00003cf0: 006c 0061 0064 0065 006e 003f 0800 0000  .l.a.d.e.n.?....
+00003d00: 0006 0000 0080 4669 6c65 2022 7b66 696c  ......File "{fil
+00003d10: 655f 6e61 6d65 7d22 2069 7320 6f76 6572  e_name}" is over
+00003d20: 2032 35c2 a04d 422e 2052 656d 656d 6265   25..MB. Remembe
+00003d30: 7220 7468 6174 2050 686f 7469 6e69 2075  r that Photini u
+00003d40: 706c 6f61 6473 2063 6f75 6e74 2074 6f77  ploads count tow
+00003d50: 6172 6473 2073 746f 7261 6765 2069 6e20  ards storage in 
+00003d60: 796f 7572 2047 6f6f 676c 6520 4163 636f  your Google Acco
+00003d70: 756e 742e 2055 706c 6f61 6420 6974 2061  unt. Upload it a
+00003d80: 6e79 7761 793f 0700 0000 0f47 6f6f 676c  nyway?.....Googl
+00003d90: 6550 686f 746f 7354 6162 0103 0000 0030  ePhotosTab.....0
+00003da0: 0047 006f 006f 0067 006c 0065 0020 0026  .G.o.o.g.l.e. .&
+00003db0: 0050 0068 006f 0074 006f 0073 0020 0068  .P.h.o.t.o.s. .h
+00003dc0: 006f 0063 0068 006c 0061 0064 0065 006e  .o.c.h.l.a.d.e.n
+00003dd0: 0800 0000 0006 0000 0015 476f 6f67 6c65  ..........Google
+00003de0: 2026 5068 6f74 6f73 2075 706c 6f61 6407   &Photos upload.
+00003df0: 0000 000f 476f 6f67 6c65 5068 6f74 6f73  ....GooglePhotos
+00003e00: 5461 6201 0300 0000 1a00 4700 6f00 6f00  Tab.......G.o.o.
+00003e10: 6700 6c00 6500 2000 5000 6800 6f00 7400  g.l.e. .P.h.o.t.
+00003e20: 6f00 7308 0000 0000 0600 0000 0d47 6f6f  o.s..........Goo
+00003e30: 676c 6520 5068 6f74 6f73 0700 0000 0f47  gle Photos.....G
+00003e40: 6f6f 676c 6550 686f 746f 7354 6162 0103  ooglePhotosTab..
+00003e50: 0000 0018 0047 0072 006f 00df 0065 0020  .....G.r.o...e. 
+00003e60: 0044 0061 0074 0065 0069 002e 0800 0000  .D.a.t.e.i......
+00003e70: 0006 0000 000b 4c61 7267 6520 6669 6c65  ......Large file
+00003e80: 2e07 0000 000f 476f 6f67 6c65 5068 6f74  ......GooglePhot
+00003e90: 6f73 5461 6201 0300 0000 1600 4e00 6500  osTab.......N.e.
+00003ea0: 7500 6500 7300 2000 4100 6c00 6200 7500  u.e.s. .A.l.b.u.
+00003eb0: 6d08 0000 0000 0600 0000 094e 6577 2061  m..........New a
+00003ec0: 6c62 756d 0700 0000 0f47 6f6f 676c 6550  lbum.....GoogleP
+00003ed0: 686f 746f 7354 6162 0103 0000 0028 0050  hotosTab.....(.P
+00003ee0: 0068 006f 0074 0069 006e 0069 003a 0020  .h.o.t.i.n.i.:. 
+00003ef0: 0067 0072 006f 00df 0065 0020 0044 0061  .g.r.o...e. .D.a
+00003f00: 0074 0065 0069 0800 0000 0006 0000 0013  .t.e.i..........
+00003f10: 5068 6f74 696e 693a 206c 6172 6765 2066  Photini: large f
+00003f20: 696c 6507 0000 000f 476f 6f67 6c65 5068  ile.....GooglePh
+00003f30: 6f74 6f73 5461 6201 0300 0000 3e00 4200  otosTab.....>.B.
+00003f40: 6900 7400 7400 6500 2000 6500 6900 6e00  i.t.t.e. .e.i.n.
+00003f50: 6500 6e00 2000 4100 6c00 6200 7500 6d00  e.n. .A.l.b.u.m.
+00003f60: 7400 6900 7400 6500 6c00 2000 6500 6900  t.i.t.e.l. .e.i.
+00003f70: 6e00 6700 6500 6200 6500 6e08 0000 0000  n.g.e.b.e.n.....
+00003f80: 0600 0000 2250 6c65 6173 6520 656e 7465  ...."Please ente
+00003f90: 7220 6120 7469 746c 6520 666f 7220 7468  r a title for th
+00003fa0: 6520 616c 6275 6d07 0000 000f 476f 6f67  e album.....Goog
+00003fb0: 6c65 5068 6f74 6f73 5461 6201 0300 0000  lePhotosTab.....
+00003fc0: 6200 4700 5000 5800 2000 4400 6100 7400  b.G.P.X. .D.a.t.
+00003fd0: 6500 6900 6500 6e00 2000 2800 2a00 2e00  e.i.e.n. .(.*...
+00003fe0: 6700 7000 7800 2000 2a00 2e00 4700 5000  g.p.x. .*...G.P.
+00003ff0: 5800 2000 2a00 2e00 4700 7000 7800 2900  X. .*...G.p.x.).
+00004000: 3b00 3b00 4100 6c00 6c00 6500 2000 4400  ;.;.A.l.l.e. .D.
+00004010: 6100 7400 6500 6900 6500 6e00 2000 2800  a.t.e.i.e.n. .(.
+00004020: 2a00 2908 0000 0000 0600 0000 2c47 5058  *.).........,GPX
+00004030: 2066 696c 6573 2028 2a2e 6770 7820 2a2e   files (*.gpx *.
+00004040: 4750 5820 2a2e 4770 7829 3b3b 416c 6c20  GPX *.Gpx);;All 
+00004050: 6669 6c65 7320 282a 2907 0000 000b 4770  files (*).....Gp
+00004060: 7849 6d70 6f72 7465 7201 0300 0000 2a00  xImporter.....*.
+00004070: 4700 5000 5800 2d00 4400 6100 7400 6500  G.P.X.-.D.a.t.e.
+00004080: 6900 2000 6900 6d00 7000 6f00 7200 7400  i. .i.m.p.o.r.t.
+00004090: 6900 6500 7200 6500 6e08 0000 0000 0600  i.e.r.e.n.......
+000040a0: 0000 0f49 6d70 6f72 7420 4750 5820 6669  ...Import GPX fi
+000040b0: 6c65 0700 0000 0b47 7078 496d 706f 7274  le.....GpxImport
+000040c0: 6572 0103 0000 001e 0044 0061 0074 0065  er.......D.a.t.e
+000040d0: 0069 0020 0073 0063 0068 006c 0069 0065  .i. .s.c.h.l.i.e
+000040e0: 00df 0065 006e 0300 0000 2200 4400 6100  ...e.n....".D.a.
+000040f0: 7400 6500 6900 6500 6e00 2000 7300 6300  t.e.i.e.n. .s.c.
+00004100: 6800 6c00 6900 6500 df00 6500 6e08 0000  h.l.i.e...e.n...
+00004110: 0000 0600 0000 0d43 6c6f 7365 2066 696c  .......Close fil
+00004120: 6528 7329 0700 0000 0949 6d61 6765 4c69  e(s).....ImageLi
+00004130: 7374 0103 0000 004c 004d 00f6 0063 0068  st.....L.M...c.h
+00004140: 0074 0065 006e 0020 0053 0069 0065 0020  .t.e.n. .S.i.e. 
+00004150: 0049 0068 0072 0065 0020 00c4 006e 0064  .I.h.r.e. ...n.d
+00004160: 0065 0072 0075 006e 0067 0065 006e 0020  .e.r.u.n.g.e.n. 
+00004170: 0073 0070 0065 0069 0063 0068 0065 0072  .s.p.e.i.c.h.e.r
+00004180: 006e 003f 0800 0000 0006 0000 0021 446f  .n.?.........!Do
+00004190: 2079 6f75 2077 616e 7420 746f 2073 6176   you want to sav
+000041a0: 6520 796f 7572 2063 6861 6e67 6573 3f07  e your changes?.
+000041b0: 0000 0009 496d 6167 654c 6973 7401 0300  ....ImageList...
+000041c0: 0000 5800 4200 6900 6c00 6400 6500 7200  ..X.B.i.l.d.e.r.
+000041d0: 2000 2800 7b00 3000 7d00 2900 3b00 3b00   .(.{.0.}.).;.;.
+000041e0: 5600 6900 6400 6500 6f00 7300 2000 2800  V.i.d.e.o.s. .(.
+000041f0: 7b00 3100 7d00 2900 3b00 3b00 4100 6c00  {.1.}.).;.;.A.l.
+00004200: 6c00 6500 2000 4400 6100 7400 6500 6900  l.e. .D.a.t.e.i.
+00004210: 6500 6e00 2000 2800 2a00 2908 0000 0000  e.n. .(.*.).....
+00004220: 0600 0000 2949 6d61 6765 7320 287b 307d  ....)Images ({0}
+00004230: 293b 3b56 6964 656f 7320 287b 317d 293b  );;Videos ({1});
+00004240: 3b41 6c6c 2066 696c 6573 2028 2a29 0700  ;All files (*)..
+00004250: 0000 0949 6d61 6765 4c69 7374 0103 0000  ...ImageList....
+00004260: 0046 004d 0065 0074 0061 0064 0061 0074  .F.M.e.t.a.d.a.t
+00004270: 0065 006e 002d 0055 006e 0074 0065 0072  .e.n.-.U.n.t.e.r
+00004280: 0073 0063 0068 0069 0065 0064 0065 003a  .s.c.h.i.e.d.e.:
+00004290: 0020 007b 0066 0069 006c 0065 005f 006e  . .{.f.i.l.e._.n
+000042a0: 0061 006d 0065 007d 0800 0000 0006 0000  .a.m.e.}........
+000042b0: 0021 4d65 7461 6461 7461 2064 6966 6665  .!Metadata diffe
+000042c0: 7265 6e63 6573 3a20 7b66 696c 655f 6e61  rences: {file_na
+000042d0: 6d65 7d07 0000 0009 496d 6167 654c 6973  me}.....ImageLis
+000042e0: 7401 0300 0000 4200 5600 6f00 7200 7300  t.....B.V.o.r.s.
+000042f0: 6300 6800 6100 7500 2000 6900 6e00 2000  c.h.a.u. .i.n. .
+00004300: 4400 6100 7400 6500 6900 2000 6e00 6900  D.a.t.e.i. .n.i.
+00004310: 6300 6800 7400 2000 7600 6f00 7200 6800  c.h.t. .v.o.r.h.
+00004320: 6100 6e00 6400 6500 6e08 0000 0000 0600  a.n.d.e.n.......
+00004330: 0000 144e 6f20 7468 756d 626e 6169 6c20  ...No thumbnail 
+00004340: 696e 2066 696c 6507 0000 0009 496d 6167  in file.....Imag
+00004350: 654c 6973 7401 0300 0000 1c00 4400 6100  eList.......D.a.
+00004360: 7400 6500 6900 6500 6e00 2000 f600 6600  t.e.i.e.n. ...f.
+00004370: 6600 6e00 6500 6e08 0000 0000 0600 0000  f.n.e.n.........
+00004380: 0a4f 7065 6e20 6669 6c65 7307 0000 0009  .Open files.....
+00004390: 496d 6167 654c 6973 7401 0300 0000 3a00  ImageList.....:.
+000043a0: 5000 6800 6f00 7400 6900 6e00 6900 3a00  P.h.o.t.i.n.i.:.
+000043b0: 2000 7500 6e00 6700 6500 7300 7000 6500   .u.n.g.e.s.p.e.
+000043c0: 6900 6300 6800 6500 7200 7400 6500 2000  i.c.h.e.r.t.e. .
+000043d0: 4400 6100 7400 6500 6e08 0000 0000 0600  D.a.t.e.n.......
+000043e0: 0000 1550 686f 7469 6e69 3a20 756e 7361  ...Photini: unsa
+000043f0: 7665 6420 6461 7461 0700 0000 0949 6d61  ved data.....Ima
+00004400: 6765 4c69 7374 0103 0000 0036 004d 0069  geList.....6.M.i
+00004410: 006e 0069 0061 0074 0075 0072 0062 0069  .n.i.a.t.u.r.b.i
+00004420: 006c 0064 0020 006e 0065 0075 0020 0067  .l.d. .n.e.u. .g
+00004430: 0065 006e 0065 0072 0069 0065 0072 0065  .e.n.e.r.i.e.r.e
+00004440: 006e 0300 0000 3a00 4d00 6900 6e00 6900  .n....:.M.i.n.i.
+00004450: 6100 7400 7500 7200 6200 6900 6c00 6400  a.t.u.r.b.i.l.d.
+00004460: 6500 7200 2000 6e00 6500 7500 2000 6700  e.r. .n.e.u. .g.
+00004470: 6500 6e00 6500 7200 6900 6500 7200 6500  e.n.e.r.i.e.r.e.
+00004480: 6e08 0000 0000 0600 0000 1752 6567 656e  n..........Regen
+00004490: 6572 6174 6520 7468 756d 626e 6169 6c28  erate thumbnail(
+000044a0: 7329 0700 0000 0949 6d61 6765 4c69 7374  s).....ImageList
+000044b0: 0103 0000 001e 0044 0061 0074 0065 0069  .......D.a.t.e.i
+000044c0: 0020 006e 0065 0075 0020 006c 0061 0064  . .n.e.u. .l.a.d
+000044d0: 0065 006e 0300 0000 2200 4400 6100 7400  .e.n....".D.a.t.
+000044e0: 6500 6900 6500 6e00 2000 6e00 6500 7500  e.i.e.n. .n.e.u.
+000044f0: 2000 6c00 6100 6400 6500 6e08 0000 0000   .l.a.d.e.n.....
+00004500: 0600 0000 0e52 656c 6f61 6420 6669 6c65  .....Reload file
+00004510: 2873 2907 0000 0009 496d 6167 654c 6973  (s).....ImageLis
+00004520: 7401 0300 0000 2800 c400 6e00 6400 6500  t.....(...n.d.e.
+00004530: 7200 7500 6e00 6700 6500 6e00 2000 7300  r.u.n.g.e.n. .s.
+00004540: 7000 6500 6900 6300 6800 6500 7200 6e08  p.e.i.c.h.e.r.n.
+00004550: 0000 0000 0600 0000 0c53 6176 6520 6368  .........Save ch
+00004560: 616e 6765 7307 0000 0009 496d 6167 654c  anges.....ImageL
+00004570: 6973 7401 0300 0000 5e00 4500 6900 6e00  ist.....^.E.i.n.
+00004580: 6900 6700 6500 2000 4200 6900 6c00 6400  i.g.e. .B.i.l.d.
+00004590: 6500 7200 2000 6500 6e00 7400 6800 6100  e.r. .e.n.t.h.a.
+000045a0: 6c00 7400 6500 6e00 2000 7500 6e00 6700  l.t.e.n. .u.n.g.
+000045b0: 6500 7300 6900 6300 6800 6500 7200 7400  e.s.i.c.h.e.r.t.
+000045c0: 6500 2000 4d00 6500 7400 6100 6400 6100  e. .M.e.t.a.d.a.
+000045d0: 7400 6500 6e00 2e08 0000 0000 0600 0000  t.e.n...........
+000045e0: 2253 6f6d 6520 696d 6167 6573 2068 6176  "Some images hav
+000045f0: 6520 756e 7361 7665 6420 6d65 7461 6461  e unsaved metada
+00004600: 7461 2e07 0000 0009 496d 6167 654c 6973  ta......ImageLis
+00004610: 7401 0300 0000 1c00 5300 6f00 7200 7400  t.......S.o.r.t.
+00004620: 6900 6500 7200 6500 6e00 2000 6e00 6100  i.e.r.e.n. .n.a.
+00004630: 6300 6808 0000 0000 0600 0000 0753 6f72  c.h..........Sor
+00004640: 7420 6279 0700 0000 0949 6d61 6765 4c69  t by.....ImageLi
+00004650: 7374 0103 0000 0022 0056 006f 0072 0073  st.....".V.o.r.s
+00004660: 0063 0068 0061 0075 0062 0069 006c 0064  .c.h.a.u.b.i.l.d
+00004670: 0067 0072 00f6 00df 0065 0800 0000 0006  .g.r.....e......
+00004680: 0000 000e 5468 756d 626e 6169 6c20 7369  ....Thumbnail si
+00004690: 7a65 0700 0000 0949 6d61 6765 4c69 7374  ze.....ImageList
+000046a0: 0103 0000 0026 00c4 006e 0064 0065 0072  .....&...n.d.e.r
+000046b0: 0075 006e 0067 0065 006e 0020 0061 006e  .u.n.g.e.n. .a.n
+000046c0: 007a 0065 0069 0067 0065 006e 0800 0000  .z.e.i.g.e.n....
+000046d0: 0006 0000 000c 5669 6577 2063 6861 6e67  ......View chang
+000046e0: 6573 0700 0000 0949 6d61 6765 4c69 7374  es.....ImageList
+000046f0: 0103 0000 001a 0041 0075 0066 006e 0061  .......A.u.f.n.a
+00004700: 0068 006d 0065 0064 0061 0074 0075 006d  .h.m.e.d.a.t.u.m
+00004710: 0800 0000 0006 0000 000a 6461 7465 2074  ..........date t
+00004720: 616b 656e 0700 0000 0949 6d61 6765 4c69  aken.....ImageLi
+00004730: 7374 0103 0000 0012 0044 0061 0074 0065  st.......D.a.t.e
+00004740: 0069 006e 0061 006d 0065 0800 0000 0006  .i.n.a.m.e......
+00004750: 0000 0009 6669 6c65 206e 616d 6507 0000  ....file name...
+00004760: 0009 496d 6167 654c 6973 7401 0300 0000  ..ImageList.....
+00004770: 1400 6e00 6500 7500 6500 7200 2000 5700  ..n.e.u.e.r. .W.
+00004780: 6500 7200 7408 0000 0000 0600 0000 096e  e.r.t..........n
+00004790: 6577 2076 616c 7565 0700 0000 0949 6d61  ew value.....Ima
+000047a0: 6765 4c69 7374 0103 0000 0014 0061 006c  geList.......a.l
+000047b0: 0074 0065 0072 0020 0057 0065 0072 0074  .t.e.r. .W.e.r.t
+000047c0: 0800 0000 0006 0000 0009 6f6c 6420 7661  ..........old va
+000047d0: 6c75 6507 0000 0009 496d 6167 654c 6973  lue.....ImageLis
+000047e0: 7401 0300 0000 1400 7200 fc00 6300 6b00  t.......r...c.k.
+000047f0: 6700 e400 6e00 6700 6900 6708 0000 0000  g...n.g.i.g.....
+00004800: 0600 0000 0475 6e64 6f07 0000 0009 496d  .....undo.....Im
+00004810: 6167 654c 6973 7401 0300 0000 2600 2500  ageList.....&.%.
+00004820: 6e00 2000 4400 6100 7400 6500 6900 2000  n. .D.a.t.e.i. .
+00004830: 6100 7500 7300 6700 6500 7700 e400 6800  a.u.s.g.e.w...h.
+00004840: 6c00 7403 0000 002a 0025 006e 0020 0044  l.t....*.%.n. .D
+00004850: 0061 0074 0065 0069 0065 006e 0020 0061  .a.t.e.i.e.n. .a
+00004860: 0075 0073 0067 0065 0077 00e4 0068 006c  .u.s.g.e.w...h.l
+00004870: 0074 0800 0000 0006 0000 0013 256e 2066  .t..........%n f
+00004880: 696c 6528 7329 2073 656c 6563 7465 6407  ile(s) selected.
 00004890: 0000 000b 496d 706f 7274 6572 5461 6201  ....ImporterTab.
-000048a0: 0300 0000 1c00 4600 6f00 7400 6f00 7300  ......F.o.t.o.s.
-000048b0: 2000 6b00 6f00 7000 6900 6500 7200 6500   .k.o.p.i.e.r.e.
-000048c0: 6e08 0000 0000 0600 0000 0b43 6f70 7920  n..........Copy 
-000048d0: 7068 6f74 6f73 0700 0000 0b49 6d70 6f72  photos.....Impor
-000048e0: 7465 7254 6162 0103 0000 0066 0049 006d  terTab.....f.I.m
-000048f0: 0070 006f 0072 0074 0069 0065 0072 0065  .p.o.r.t.i.e.r.e
-00004900: 006e 0020 0076 006f 006e 0020 0046 006f  .n. .v.o.n. .F.o
-00004910: 0074 006f 0073 0020 0069 0073 0074 0020  .t.o.s. .i.s.t. 
-00004920: 006e 006f 0063 0068 0020 006e 0069 0063  .n.o.c.h. .n.i.c
-00004930: 0068 0074 0020 0061 0062 0067 0065 0073  .h.t. .a.b.g.e.s
-00004940: 0063 0068 006c 006f 0073 0073 0065 006e  .c.h.l.o.s.s.e.n
-00004950: 002e 0800 0000 0006 0000 0022 496d 706f  ..........."Impo
-00004960: 7274 696e 6720 7068 6f74 6f73 2068 6173  rting photos has
-00004970: 206e 6f74 2066 696e 6973 6865 642e 0700   not finished...
-00004980: 0000 0b49 6d70 6f72 7465 7254 6162 0103  ...ImporterTab..
-00004990: 0000 0024 0050 0068 006f 0074 006f 0073  ...$.P.h.o.t.o.s
-000049a0: 0020 0076 0065 0072 0073 0063 0068 0069  . .v.e.r.s.c.h.i
-000049b0: 0065 0062 0065 006e 0800 0000 0006 0000  .e.b.e.n........
-000049c0: 000b 4d6f 7665 2070 686f 746f 7307 0000  ..Move photos...
-000049d0: 000b 496d 706f 7274 6572 5461 6201 0300  ..ImporterTab...
-000049e0: 0000 2a00 5000 6800 6f00 7400 6900 6e00  ..*.P.h.o.t.i.n.
-000049f0: 6900 3a00 2000 4900 6d00 7000 6f00 7200  i.:. .I.m.p.o.r.
-00004a00: 7400 2000 6c00 e400 7500 6600 7408 0000  t. .l...u.f.t...
-00004a10: 0000 0600 0000 1b50 686f 7469 6e69 3a20  .......Photini: 
-00004a20: 696d 706f 7274 2069 6e20 7072 6f67 7265  import in progre
-00004a30: 7373 0700 0000 0b49 6d70 6f72 7465 7254  ss.....ImporterT
-00004a40: 6162 0103 0000 0032 0022 007b 0073 006f  ab.....2.".{.s.o
-00004a50: 0075 0072 0063 0065 005f 006e 0061 006d  .u.r.c.e._.n.a.m
-00004a60: 0065 007d 0022 0020 0065 006e 0074 0066  .e.}.". .e.n.t.f
-00004a70: 0065 0072 006e 0065 006e 0800 0000 0006  .e.r.n.e.n......
-00004a80: 0000 0016 5265 6d6f 7665 2022 7b73 6f75  ....Remove "{sou
-00004a90: 7263 655f 6e61 6d65 7d22 0700 0000 0b49  rce_name}".....I
-00004aa0: 6d70 6f72 7465 7254 6162 0103 0000 001c  mporterTab......
-00004ab0: 0041 006c 006c 0065 0020 0061 0075 0073  .A.l.l.e. .a.u.s
-00004ac0: 0077 00e4 0068 006c 0065 006e 0800 0000  .w...h.l.e.n....
-00004ad0: 0006 0000 000a 5365 6c65 6374 2061 6c6c  ......Select all
-00004ae0: 0700 0000 0b49 6d70 6f72 7465 7254 6162  .....ImporterTab
-00004af0: 0103 0000 001a 004e 0065 0075 0020 0061  .......N.e.u. .a
-00004b00: 0075 0073 0077 00e4 0068 006c 0065 006e  .u.s.w...h.l.e.n
-00004b10: 0800 0000 0006 0000 000a 5365 6c65 6374  ..........Select
-00004b20: 206e 6577 0700 0000 0b49 6d70 6f72 7465   new.....Importe
-00004b30: 7254 6162 0103 0000 002a 0051 0075 0065  rTab.....*.Q.u.e
-00004b40: 006c 006c 006f 0072 0064 006e 0065 0072  .l.l.o.r.d.n.e.r
-00004b50: 0020 0061 0075 0073 0077 00e4 0068 006c  . .a.u.s.w...h.l
-00004b60: 0065 006e 0800 0000 0006 0000 0012 5365  .e.n..........Se
-00004b70: 6c65 6374 2072 6f6f 7420 666f 6c64 6572  lect root folder
-00004b80: 0700 0000 0b49 6d70 6f72 7465 7254 6162  .....ImporterTab
-00004b90: 0103 0000 000c 0051 0075 0065 006c 006c  .......Q.u.e.l.l
-00004ba0: 0065 0800 0000 0006 0000 0006 536f 7572  .e..........Sour
-00004bb0: 6365 0700 0000 0b49 6d70 6f72 7465 7254  ce.....ImporterT
-00004bc0: 6162 0103 0000 001a 0053 0074 006f 0070  ab.......S.t.o.p
-00004bd0: 0020 004b 006f 0070 0069 0065 0072 0065  . .K.o.p.i.e.r.e
-00004be0: 006e 0800 0000 0006 0000 0009 5374 6f70  .n..........Stop
-00004bf0: 2063 6f70 7907 0000 000b 496d 706f 7274   copy.....Import
-00004c00: 6572 5461 6201 0300 0000 2000 5300 7400  erTab..... .S.t.
-00004c10: 6f00 7000 2000 5600 6500 7200 7300 6300  o.p. .V.e.r.s.c.
-00004c20: 6800 6900 6500 6200 6500 6e08 0000 0000  h.i.e.b.e.n.....
-00004c30: 0600 0000 0953 746f 7020 6d6f 7665 0700  .....Stop move..
-00004c40: 0000 0b49 6d70 6f72 7465 7254 6162 0103  ...ImporterTab..
-00004c50: 0000 0014 005a 0069 0065 006c 0066 006f  .....Z.i.e.l.f.o
-00004c60: 0072 006d 0061 0074 0800 0000 0006 0000  .r.m.a.t........
-00004c70: 000d 5461 7267 6574 2066 6f72 6d61 7407  ..Target format.
-00004c80: 0000 000b 496d 706f 7274 6572 5461 6201  ....ImporterTab.
-00004c90: 0300 0000 2a00 4b00 6100 6d00 6500 7200  ....*.K.a.m.e.r.
-00004ca0: 6100 3a00 2000 7b00 6300 6100 6d00 6500  a.:. .{.c.a.m.e.
-00004cb0: 7200 6100 5f00 6e00 6100 6d00 6500 7d08  r.a._.n.a.m.e.}.
-00004cc0: 0000 0000 0600 0000 1563 616d 6572 613a  .........camera:
-00004cd0: 207b 6361 6d65 7261 5f6e 616d 657d 0700   {camera_name}..
-00004ce0: 0000 0b49 6d70 6f72 7465 7254 6162 0103  ...ImporterTab..
-00004cf0: 0000 002a 004f 0072 0064 006e 0065 0072  ...*.O.r.d.n.e.r
-00004d00: 003a 0020 007b 0066 006f 006c 0064 0065  .:. .{.f.o.l.d.e
-00004d10: 0072 005f 006e 0061 006d 0065 007d 0800  .r._.n.a.m.e.}..
-00004d20: 0000 0006 0000 0015 666f 6c64 6572 3a20  ........folder: 
-00004d30: 7b66 6f6c 6465 725f 6e61 6d65 7d07 0000  {folder_name}...
-00004d40: 000b 496d 706f 7274 6572 5461 6201 0300  ..ImporterTab...
-00004d50: 0000 1200 4e00 6500 7500 2000 6c00 6100  ....N.e.u. .l.a.
-00004d60: 6400 6500 6e08 0000 0000 0600 0000 0772  d.e.n..........r
-00004d70: 6566 7265 7368 0700 0000 0b49 6d70 6f72  efresh.....Impor
-00004d80: 7465 7254 6162 0103 0000 0026 0026 0049  terTab.....&.&.I
-00004d90: 0070 0065 0072 006e 0069 0074 0079 002d  .p.e.r.n.i.t.y.-
-00004da0: 0048 006f 0063 0068 006c 0061 0064 0065  .H.o.c.h.l.a.d.e
-00004db0: 006e 0800 0000 0006 0000 0010 2649 7065  .n..........&Ipe
-00004dc0: 726e 6974 7920 7570 6c6f 6164 0700 0000  rnity upload....
-00004dd0: 0b49 7065 726e 6974 7954 6162 0103 0000  .IpernityTab....
-00004de0: 001a 004e 0061 006d 0065 006e 0073 006e  ...N.a.m.e.n.s.n
-00004df0: 0065 006e 006e 0075 006e 0067 0800 0000  .e.n.n.u.n.g....
-00004e00: 0006 0000 000b 4174 7472 6962 7574 696f  ......Attributio
-00004e10: 6e07 0000 000b 4970 6572 6e69 7479 5461  n.....IpernityTa
-00004e20: 6201 0300 0000 3e00 4e00 6100 6d00 6500  b.....>.N.a.m.e.
-00004e30: 6e00 7300 6e00 6500 6e00 6e00 7500 6e00  n.s.n.e.n.n.u.n.
-00004e40: 6700 2000 2b00 2000 6b00 6500 6900 6e00  g. .+. .k.e.i.n.
-00004e50: 6500 2000 4100 6200 6c00 6500 6900 7400  e. .A.b.l.e.i.t.
-00004e60: 7500 6e00 6708 0000 0000 0600 0000 1b41  u.n.g..........A
-00004e70: 7474 7269 6275 7469 6f6e 202b 206e 6f20  ttribution + no 
-00004e80: 6465 7269 7661 7469 7665 0700 0000 0b49  derivative.....I
-00004e90: 7065 726e 6974 7954 6162 0103 0000 0042  pernityTab.....B
-00004ea0: 004e 0061 006d 0065 006e 0073 006e 0065  .N.a.m.e.n.s.n.e
-00004eb0: 006e 006e 0075 006e 0067 0020 002b 0020  .n.n.u.n.g. .+. 
-00004ec0: 006e 0069 0063 0068 0074 0020 006b 006f  .n.i.c.h.t. .k.o
-00004ed0: 006d 006d 0065 0072 007a 0069 0065 006c  .m.m.e.r.z.i.e.l
-00004ee0: 006c 0800 0000 0006 0000 001c 4174 7472  .l..........Attr
-00004ef0: 6962 7574 696f 6e20 2b20 6e6f 6e20 636f  ibution + non co
-00004f00: 6d6d 6572 6369 616c 0700 0000 0b49 7065  mmercial.....Ipe
-00004f10: 726e 6974 7954 6162 0103 0000 0066 004e  rnityTab.....f.N
-00004f20: 0061 006d 0065 006e 0073 006e 0065 006e  .a.m.e.n.s.n.e.n
-00004f30: 006e 0075 006e 0067 0020 002b 0020 006e  .n.u.n.g. .+. .n
-00004f40: 0069 0063 0068 0074 0020 006b 006f 006d  .i.c.h.t. .k.o.m
-00004f50: 006d 0065 0072 007a 0069 0065 006c 006c  .m.e.r.z.i.e.l.l
-00004f60: 0020 002b 0020 006b 0065 0069 006e 0065  . .+. .k.e.i.n.e
-00004f70: 0020 0041 0062 006c 0065 0069 0074 0075  . .A.b.l.e.i.t.u
-00004f80: 006e 0067 0800 0000 0006 0000 002c 4174  .n.g.........,At
-00004f90: 7472 6962 7574 696f 6e20 2b20 6e6f 6e20  tribution + non 
-00004fa0: 636f 6d6d 6572 6369 616c 202b 206e 6f20  commercial + no 
-00004fb0: 6465 7269 7661 7469 7665 0700 0000 0b49  derivative.....I
-00004fc0: 7065 726e 6974 7954 6162 0103 0000 007a  pernityTab.....z
-00004fd0: 004e 0061 006d 0065 006e 0073 006e 0065  .N.a.m.e.n.s.n.e
-00004fe0: 006e 006e 0075 006e 0067 0020 002b 0020  .n.n.u.n.g. .+. 
-00004ff0: 006e 0069 0063 0068 0074 0020 006b 006f  .n.i.c.h.t. .k.o
-00005000: 006d 006d 0065 0072 007a 0069 0065 006c  .m.m.e.r.z.i.e.l
-00005010: 006c 0020 002b 0020 0067 006c 0065 0069  .l. .+. .g.l.e.i
-00005020: 0063 0068 0062 0065 0072 0065 0063 0068  .c.h.b.e.r.e.c.h
-00005030: 0074 0069 0067 0074 0065 0020 004e 0075  .t.i.g.t.e. .N.u
-00005040: 0074 007a 0075 006e 0067 0800 0000 0006  .t.z.u.n.g......
-00005050: 0000 002a 4174 7472 6962 7574 696f 6e20  ...*Attribution 
-00005060: 2b20 6e6f 6e20 636f 6d6d 6572 6369 616c  + non commercial
-00005070: 202b 2073 6861 7265 2061 6c69 6b65 0700   + share alike..
-00005080: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
-00005090: 0000 0052 004e 0061 006d 0065 006e 0073  ...R.N.a.m.e.n.s
-000050a0: 006e 0065 006e 006e 0075 006e 0067 0020  .n.e.n.n.u.n.g. 
-000050b0: 002b 0020 0067 006c 0065 0069 0063 0068  .+. .g.l.e.i.c.h
-000050c0: 0062 0065 0072 0065 0063 0068 0074 0069  .b.e.r.e.c.h.t.i
-000050d0: 0067 0074 0065 0020 004e 0075 0074 007a  .g.t.e. .N.u.t.z
-000050e0: 0075 006e 0067 0800 0000 0006 0000 0019  .u.n.g..........
-000050f0: 4174 7472 6962 7574 696f 6e20 2b20 7368  Attribution + sh
-00005100: 6172 6520 616c 696b 6507 0000 000b 4970  are alike.....Ip
-00005110: 6572 6e69 7479 5461 6201 0300 0000 3400  ernityTab.....4.
-00005120: 4100 6c00 6200 7500 6d00 6d00 6900 7400  A.l.b.u.m.m.i.t.
-00005130: 6700 6c00 6900 6500 6400 7300 6300 6800  g.l.i.e.d.s.c.h.
-00005140: 6100 6600 7400 2000 e400 6e00 6400 6500  a.f.t. ...n.d.e.
-00005150: 7200 6e08 0000 0000 0600 0000 1743 6861  r.n..........Cha
-00005160: 6e67 6520 616c 6275 6d20 6d65 6d62 6572  nge album member
-00005170: 7368 6970 0700 0000 0b49 7065 726e 6974  ship.....Ipernit
-00005180: 7954 6162 0103 0000 001a 004c 0069 007a  yTab.......L.i.z
-00005190: 0065 006e 007a 0020 00e4 006e 0064 0065  .e.n.z. ...n.d.e
-000051a0: 0072 006e 0800 0000 0006 0000 0012 4368  .r.n..........Ch
-000051b0: 616e 6765 2074 6865 206c 6963 656e 6365  ange the licence
-000051c0: 0700 0000 0b49 7065 726e 6974 7954 6162  .....IpernityTab
-000051d0: 0103 0000 0030 00c4 006e 0064 0065 0072  .....0...n.d.e.r
-000051e0: 006e 0020 0077 0065 0072 0020 0065 0073  .n. .w.e.r. .e.s
-000051f0: 0020 0073 0065 0068 0065 006e 0020 006b  . .s.e.h.e.n. .k
-00005200: 0061 006e 006e 0800 0000 0006 0000 0015  .a.n.n..........
-00005210: 4368 616e 6765 2077 686f 2063 616e 2073  Change who can s
-00005220: 6565 2069 7407 0000 000b 4970 6572 6e69  ee it.....Iperni
-00005230: 7479 5461 6201 0300 0000 1000 4b00 6f00  tyTab.......K.o.
-00005240: 6e00 7400 6100 6b00 7400 6508 0000 0000  n.t.a.k.t.e.....
-00005250: 0600 0000 0843 6f6e 7461 6374 7307 0000  .....Contacts...
-00005260: 000b 4970 6572 6e69 7479 5461 6201 0300  ..IpernityTab...
-00005270: 0000 4c00 5500 7200 6800 6500 6200 6500  ..L.U.r.h.e.b.e.
-00005280: 7200 7200 6500 6300 6800 7400 2000 2800  r.r.e.c.h.t. .(.
-00005290: 6100 6c00 6c00 6500 2000 5200 6500 6300  a.l.l.e. .R.e.c.
-000052a0: 6800 7400 6500 2000 7600 6f00 7200 6200  h.t.e. .v.o.r.b.
-000052b0: 6500 6800 6100 6c00 7400 6500 6e00 2908  e.h.a.l.t.e.n.).
-000052c0: 0000 0000 0600 0000 1f43 6f70 7972 6967  .........Copyrig
-000052d0: 6874 2028 616c 6c20 7269 6768 7473 2072  ht (all rights r
-000052e0: 6573 6572 7665 6429 0700 0000 0b49 7065  eserved).....Ipe
-000052f0: 726e 6974 7954 6162 0103 0000 0018 0042  rnityTab.......B
-00005300: 0065 0073 0063 0068 0072 0065 0069 0062  .e.s.c.h.r.e.i.b
-00005310: 0075 006e 0067 0800 0000 0006 0000 000b  .u.n.g..........
-00005320: 4465 7363 7269 7074 696f 6e07 0000 000b  Description.....
-00005330: 4970 6572 6e69 7479 5461 6201 0300 0000  IpernityTab.....
-00005340: 0800 4100 6c00 6c00 6508 0000 0000 0600  ..A.l.l.e.......
-00005350: 0000 0845 7665 7279 6f6e 6507 0000 000b  ...Everyone.....
-00005360: 4970 6572 6e69 7479 5461 6201 0300 0000  IpernityTab.....
-00005370: 2200 4100 6c00 6c00 6500 2000 2800 f600  ".A.l.l.e. .(...
-00005380: 6600 6600 6500 6e00 7400 6c00 6900 6300  f.f.e.n.t.l.i.c.
-00005390: 6800 2908 0000 0000 0600 0000 1145 7665  h.)..........Eve
-000053a0: 7279 6f6e 6520 2870 7562 6c69 6329 0700  ryone (public)..
-000053b0: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
-000053c0: 0000 000e 0046 0061 006d 0069 006c 0069  .....F.a.m.i.l.i
-000053d0: 0065 0800 0000 0006 0000 0006 4661 6d69  .e..........Fami
-000053e0: 6c79 0700 0000 0b49 7065 726e 6974 7954  ly.....IpernityT
-000053f0: 6162 0103 0000 0026 0046 0061 006d 0069  ab.....&.F.a.m.i
-00005400: 006c 0069 0065 0020 0075 006e 0064 0020  .l.i.e. .u.n.d. 
-00005410: 0046 0072 0065 0075 006e 0064 0065 0800  .F.r.e.u.n.d.e..
-00005420: 0000 0006 0000 0010 4661 6d69 6c79 2026  ........Family &
-00005430: 2066 7269 656e 6473 0700 0000 0b49 7065   friends.....Ipe
-00005440: 726e 6974 7954 6162 0103 0000 0070 0046  rnityTab.....p.F
-00005450: 0072 0065 0069 0065 0020 0056 0065 0072  .r.e.i.e. .V.e.r
-00005460: 0077 0065 006e 0064 0075 006e 0067 0020  .w.e.n.d.u.n.g. 
-00005470: 0028 0055 0072 0068 0065 0062 0065 0072  .(.U.r.h.e.b.e.r
-00005480: 0072 0065 0063 0068 0074 0020 0061 0062  .r.e.c.h.t. .a.b
-00005490: 0067 0065 0074 0072 0065 0074 0065 006e  .g.e.t.r.e.t.e.n
-000054a0: 002c 0020 006b 0065 0069 006e 0065 0020  .,. .k.e.i.n.e. 
-000054b0: 004c 0069 007a 0065 006e 007a 0029 0800  .L.i.z.e.n.z.)..
-000054c0: 0000 0006 0000 002c 4672 6565 2075 7365  .......,Free use
-000054d0: 2028 636f 7079 7269 6768 7420 7375 7272   (copyright surr
-000054e0: 656e 6465 7265 642c 206e 6f20 6c69 6365  endered, no lice
-000054f0: 6e63 6529 0700 0000 0b49 7065 726e 6974  nce).....Ipernit
-00005500: 7954 6162 0103 0000 000e 0046 0072 0065  yTab.......F.r.e
-00005510: 0075 006e 0064 0065 0800 0000 0006 0000  .u.n.d.e........
-00005520: 0007 4672 6965 6e64 7307 0000 000b 4970  ..Friends.....Ip
-00005530: 6572 6e69 7479 5461 6201 0300 0000 1000  ernityTab.......
-00005540: 4900 7000 6500 7200 6e00 6900 7400 7908  I.p.e.r.n.i.t.y.
-00005550: 0000 0000 0600 0000 0849 7065 726e 6974  .........Ipernit
-00005560: 7907 0000 000b 4970 6572 6e69 7479 5461  y.....IpernityTa
-00005570: 6201 0300 0000 0c00 4c00 6900 7a00 6500  b.......L.i.z.e.
-00005580: 6e00 7a08 0000 0000 0600 0000 074c 6963  n.z..........Lic
-00005590: 656e 6365 0700 0000 0b49 7065 726e 6974  ence.....Ipernit
-000055a0: 7954 6162 0103 0000 0016 004e 0065 0075  yTab.......N.e.u
-000055b0: 0065 0073 0020 0041 006c 0062 0075 006d  .e.s. .A.l.b.u.m
-000055c0: 0800 0000 0006 0000 0009 4e65 7720 616c  ..........New al
-000055d0: 6275 6d07 0000 000b 4970 6572 6e69 7479  bum.....Ipernity
-000055e0: 5461 6201 0300 0000 1c00 4e00 7500 7200  Tab.......N.u.r.
-000055f0: 2000 6900 6300 6800 2000 7300 6500 6c00   .i.c.h. .s.e.l.
-00005600: 6200 7300 7408 0000 0000 0600 0000 084f  b.s.t..........O
-00005610: 6e6c 7920 796f 7507 0000 000b 4970 6572  nly you.....Iper
-00005620: 6e69 7479 5461 6201 0300 0000 2000 4e00  nityTab..... .N.
-00005630: 7500 7200 2000 5300 6900 6500 2000 2800  u.r. .S.i.e. .(.
-00005640: 7000 7200 6900 7600 6100 7400 2908 0000  p.r.i.v.a.t.)...
-00005650: 0000 0600 0000 124f 6e6c 7920 796f 7520  .......Only you 
-00005660: 2870 7269 7661 7465 2907 0000 000b 4970  (private).....Ip
-00005670: 6572 6e69 7479 5461 6201 0300 0000 2400  ernityTab.....$.
-00005680: 4d00 6500 7400 6100 6400 6100 7400 6500  M.e.t.a.d.a.t.e.
-00005690: 6e00 2000 6500 7200 7300 6500 7400 7a00  n. .e.r.s.e.t.z.
-000056a0: 6500 6e08 0000 0000 0600 0000 1052 6570  e.n..........Rep
-000056b0: 6c61 6365 206d 6574 6164 6174 6107 0000  lace metadata...
-000056c0: 000b 4970 6572 6e69 7479 5461 6201 0300  ..IpernityTab...
-000056d0: 0000 1e00 5300 7900 6e00 6300 6800 7200  ....S.y.n.c.h.r.
-000056e0: 6f00 6e00 6900 7300 6900 6500 7200 6500  o.n.i.s.i.e.r.e.
-000056f0: 6e08 0000 0000 0600 0000 0b53 796e 6368  n..........Synch
-00005700: 726f 6e69 7365 0700 0000 0b49 7065 726e  ronise.....Ipern
-00005710: 6974 7954 6162 0103 0000 000a 0054 0069  ityTab.......T.i
-00005720: 0074 0065 006c 0800 0000 0006 0000 0005  .t.e.l..........
-00005730: 5469 746c 6507 0000 000b 4970 6572 6e69  Title.....Iperni
-00005740: 7479 5461 6201 0300 0000 3e00 5700 6500  tyTab.....>.W.e.
-00005750: 7200 2000 6400 6100 7200 6600 2000 6400  r. .d.a.r.f. .d.
-00005760: 6100 7300 2000 4100 6c00 6200 7500 6d00  a.s. .A.l.b.u.m.
-00005770: 2000 6b00 6f00 6d00 6d00 6500 6e00 7400   .k.o.m.m.e.n.t.
-00005780: 6900 6500 7200 6500 6e08 0000 0000 0600  i.e.r.e.n.......
-00005790: 0000 1857 686f 2063 616e 2063 6f6d 6d65  ...Who can comme
-000057a0: 6e74 206f 6e20 616c 6275 6d07 0000 000b  nt on album.....
-000057b0: 4970 6572 6e69 7479 5461 6201 0300 0000  IpernityTab.....
-000057c0: 1200 5700 6500 7200 2000 6b00 6100 6e00  ..W.e.r. .k.a.n.
-000057d0: 6e00 3a08 0000 0000 0600 0000 0857 686f  n.:..........Who
-000057e0: 2063 616e 3a07 0000 000b 4970 6572 6e69   can:.....Iperni
-000057f0: 7479 5461 6201 0300 0000 4c00 5300 6300  tyTab.....L.S.c.
-00005800: 6800 6c00 fc00 7300 7300 6500 6c00 7700  h.l...s.s.e.l.w.
-00005810: f600 7200 7400 6500 7200 2000 7500 6e00  ..r.t.e.r. .u.n.
-00005820: 6400 2000 4e00 6f00 7400 6900 7a00 6500  d. .N.o.t.i.z.e.
-00005830: 6e00 2000 6800 6900 6e00 7a00 7500 6600  n. .h.i.n.z.u.f.
-00005840: fc00 6700 6500 6e08 0000 0000 0600 0000  ..g.e.n.........
-00005850: 1361 6464 206b 6579 776f 7264 732c 206e  .add keywords, n
-00005860: 6f74 6573 0700 0000 0b49 7065 726e 6974  otes.....Ipernit
-00005870: 7954 6162 0103 0000 002e 004d 0065 006e  yTab.......M.e.n
-00005880: 0073 0063 0068 0065 006e 0020 0069 0064  .s.c.h.e.n. .i.d
-00005890: 0065 006e 0074 0069 0066 0069 007a 0069  .e.n.t.i.f.i.z.i
-000058a0: 0065 0072 0065 006e 0800 0000 0006 0000  .e.r.e.n........
-000058b0: 000f 6964 656e 7469 6679 2070 656f 706c  ..identify peopl
-000058c0: 6507 0000 000b 4970 6572 6e69 7479 5461  e.....IpernityTa
-000058d0: 6201 0300 0000 3e00 6500 6900 6e00 6500  b.....>.e.i.n.e.
-000058e0: 6e00 2000 4b00 6f00 6d00 6d00 6500 6e00  n. .K.o.m.m.e.n.
-000058f0: 7400 6100 7200 2000 7600 6500 7200 f600  t.a.r. .v.e.r...
-00005900: 6600 6600 6500 6e00 7400 6c00 6900 6300  f.f.e.n.t.l.i.c.
-00005910: 6800 6500 6e08 0000 0000 0600 0000 0e70  h.e.n..........p
-00005920: 6f73 7420 6120 636f 6d6d 656e 7407 0000  ost a comment...
-00005930: 000b 4970 6572 6e69 7479 5461 6201 0300  ..IpernityTab...
-00005940: 0000 2000 4400 6100 7300 2000 4600 6f00  .. .D.a.s. .F.o.
-00005950: 7400 6f00 2000 6100 6e00 7300 6500 6800  t.o. .a.n.s.e.h.
-00005960: 6500 6e08 0000 0000 0600 0000 0d73 6565  e.n..........see
-00005970: 2074 6865 2070 686f 746f 0700 0000 0b49   the photo.....I
-00005980: 7065 726e 6974 7954 6162 0103 0000 000a  pernityTab......
-00005990: 0053 0070 0072 003a 0020 0800 0000 0006  .S.p.r.:. ......
-000059a0: 0000 0006 4c61 6e67 3a20 0700 0000 0d4c  ....Lang: .....L
-000059b0: 616e 6741 6c74 5769 6467 6574 0103 0000  angAltWidget....
-000059c0: 000e 0053 0070 0072 0061 0063 0068 0065  ...S.p.r.a.c.h.e
-000059d0: 0800 0000 0006 0000 0008 4c61 6e67 7561  ..........Langua
-000059e0: 6765 0700 0000 0d4c 616e 6741 6c74 5769  ge.....LangAltWi
-000059f0: 6467 6574 0103 0000 0018 004e 0065 0075  dget.......N.e.u
-00005a00: 0065 0020 0053 0070 0072 0061 0063 0068  .e. .S.p.r.a.c.h
-00005a10: 0065 0800 0000 0006 0000 000c 4e65 7720  .e..........New 
-00005a20: 6c61 6e67 7561 6765 0700 0000 0d4c 616e  language.....Lan
-00005a30: 6741 6c74 5769 6467 6574 0103 0000 0032  gAltWidget.....2
-00005a40: 0053 0074 0061 006e 0064 0061 0072 0064  .S.t.a.n.d.a.r.d
-00005a50: 0073 0070 0072 0061 0063 0068 0065 0020  .s.p.r.a.c.h.e. 
-00005a60: 0066 0065 0073 0074 006c 0065 0067 0065  .f.e.s.t.l.e.g.e
-00005a70: 006e 0800 0000 0006 0000 0014 5365 7420  .n..........Set 
-00005a80: 6465 6661 756c 7420 6c61 6e67 7561 6765  default language
-00005a90: 0700 0000 0d4c 616e 6741 6c74 5769 6467  .....LangAltWidg
-00005aa0: 6574 0103 0000 00b8 0049 006e 0020 0077  et.......I.n. .w
-00005ab0: 0065 006c 0063 0068 0065 0072 0020 0053  .e.l.c.h.e.r. .S
-00005ac0: 0070 0072 0061 0063 0068 0065 0020 0069  .p.r.a.c.h.e. .i
-00005ad0: 0073 0074 0020 0064 0065 0072 0020 0061  .s.t. .d.e.r. .a
-00005ae0: 006b 0074 0075 0065 006c 006c 0065 0020  .k.t.u.e.l.l.e. 
-00005af0: 0054 0065 0078 0074 003f 0020 0042 0069  .T.e.x.t.?. .B.i
-00005b00: 0074 0074 0065 0020 0067 0065 0062 0065  .t.t.e. .g.e.b.e
-00005b10: 006e 0020 0053 0069 0065 0020 0065 0069  .n. .S.i.e. .e.i
-00005b20: 006e 0020 0052 0046 0043 0033 0030 0036  .n. .R.F.C.3.0.6
-00005b30: 0036 002d 0053 0070 0072 0061 0063 0068  .6.-.S.p.r.a.c.h
-00005b40: 006b 0065 006e 006e 007a 0065 0069 0063  .k.e.n.n.z.e.i.c
-00005b50: 0068 0065 006e 0020 0065 0069 006e 002e  .h.e.n. .e.i.n..
-00005b60: 0800 0000 0006 0000 004b 5768 6174 206c  .........KWhat l
-00005b70: 616e 6775 6167 6520 6973 2074 6865 2063  anguage is the c
-00005b80: 7572 7265 6e74 2074 6578 7420 696e 3f20  urrent text in? 
-00005b90: 506c 6561 7365 2065 6e74 6572 2061 6e20  Please enter an 
-00005ba0: 5246 4333 3036 3620 6c61 6e67 7561 6765  RFC3066 language
-00005bb0: 2074 6167 2e07 0000 000d 4c61 6e67 416c   tag......LangAl
-00005bc0: 7457 6964 6765 7401 0300 0000 b200 5700  tWidget.......W.
-00005bd0: 6500 6c00 6300 6800 6500 2000 5300 7000  e.l.c.h.e. .S.p.
-00005be0: 7200 6100 6300 6800 6500 2000 6d00 f600  r.a.c.h.e. .m...
-00005bf0: 6300 6800 7400 6500 6e00 2000 5300 6900  c.h.t.e.n. .S.i.
-00005c00: 6500 2000 6800 6900 6e00 7a00 7500 6600  e. .h.i.n.z.u.f.
-00005c10: fc00 6700 6500 6e00 3f00 2000 4200 6900  ..g.e.n.?. .B.i.
-00005c20: 7400 7400 6500 2000 6700 6500 6200 6500  t.t.e. .g.e.b.e.
-00005c30: 6e00 2000 5300 6900 6500 2000 6500 6900  n. .S.i.e. .e.i.
-00005c40: 6e00 2000 5200 4600 4300 3300 3000 3600  n. .R.F.C.3.0.6.
-00005c50: 3600 2d00 5300 7000 7200 6100 6300 6800  6.-.S.p.r.a.c.h.
-00005c60: 6b00 6500 6e00 6e00 7a00 6500 6900 6300  k.e.n.n.z.e.i.c.
-00005c70: 6800 6500 6e00 2000 6500 6900 6e00 2e08  h.e.n. .e.i.n...
-00005c80: 0000 0000 0600 0000 4a57 6861 7420 6c61  ........JWhat la
-00005c90: 6e67 7561 6765 2077 6f75 6c64 2079 6f75  nguage would you
-00005ca0: 206c 696b 6520 746f 2061 6464 3f20 506c   like to add? Pl
-00005cb0: 6561 7365 2065 6e74 6572 2061 6e20 5246  ease enter an RF
-00005cc0: 4333 3036 3620 6c61 6e67 7561 6765 2074  C3066 language t
-00005cd0: 6167 2e07 0000 000d 4c61 6e67 416c 7457  ag......LangAltW
-00005ce0: 6964 6765 7401 0300 0000 1a00 4200 7200  idget.......B.r.
-00005cf0: 6500 6900 7400 6500 2c00 2000 4c00 e400  e.i.t.e.,. .L...
-00005d00: 6e00 6700 6508 0000 0000 0600 0000 094c  n.g.e..........L
-00005d10: 6174 2c20 6c6f 6e67 0700 0000 0e4c 6174  at, long.....Lat
-00005d20: 4c6f 6e67 4469 7370 6c61 7901 0300 0000  LongDisplay.....
-00005d30: 3a00 5000 6800 6f00 7400 6900 6e00 6900  :.P.h.o.t.i.n.i.
-00005d40: 2d00 4600 6500 6800 6c00 6500 7200 7000  -.F.e.h.l.e.r.p.
-00005d50: 7200 6f00 7400 6f00 6b00 6f00 6c00 6c00  r.o.t.o.k.o.l.l.
-00005d60: 6900 6500 7200 7500 6e00 6708 0000 0000  i.e.r.u.n.g.....
-00005d70: 0600 0000 1550 686f 7469 6e69 2065 7272  .....Photini err
-00005d80: 6f72 206c 6f67 6769 6e67 0700 0000 0c4c  or logging.....L
-00005d90: 6f67 6765 7257 696e 646f 7701 0300 0000  oggerWindow.....
-00005da0: 3000 5000 7200 6f00 7400 6f00 6b00 6f00  0.P.r.o.t.o.k.o.
-00005db0: 6c00 6c00 6400 6100 7400 6500 6900 2000  l.l.d.a.t.e.i. .
-00005dc0: 7300 7000 6500 6900 6300 6800 6500 7200  s.p.e.i.c.h.e.r.
-00005dd0: 6e08 0000 0000 0600 0000 0d53 6176 6520  n..........Save 
-00005de0: 6c6f 6720 6669 6c65 0700 0000 0c4c 6f67  log file.....Log
-00005df0: 6765 7257 696e 646f 7701 0300 0000 1a00  gerWindow.......
-00005e00: 4b00 6100 7200 7400 6500 2000 2800 2600  K.a.r.t.e. .(.&.
-00005e10: 4200 6900 6e00 6700 2908 0000 0000 0600  B.i.n.g.).......
-00005e20: 0000 0b4d 6170 2028 2642 696e 6729 0700  ...Map (&Bing)..
-00005e30: 0000 0a4d 6170 5461 6242 696e 6701 0300  ...MapTabBing...
-00005e40: 0000 6000 5300 7500 6300 6800 6500 2000  ..`.S.u.c.h.e. .
-00005e50: 7500 6e00 6400 2000 4e00 6100 6300 6800  u.n.d. .N.a.c.h.
-00005e60: 7300 6300 6800 6c00 6100 6700 6500 6e00  s.c.h.l.a.g.e.n.
-00005e70: 2000 6400 6500 7200 2000 4800 f600 6800   .d.e.r. .H...h.
-00005e80: 6500 2000 7000 7200 6f00 7600 6900 6400  e. .p.r.o.v.i.d.
-00005e90: 6500 6400 2000 6200 7900 2000 4200 6900  e.d. .b.y. .B.i.
-00005ea0: 6e00 6708 0000 0000 0600 0000 2b53 6561  n.g.........+Sea
-00005eb0: 7263 6820 616e 6420 616c 7469 7475 6465  rch and altitude
-00005ec0: 206c 6f6f 6b75 7020 7072 6f76 6964 6564   lookup provided
-00005ed0: 2062 7920 4269 6e67 0700 0000 0a4d 6170   by Bing.....Map
-00005ee0: 5461 6242 696e 6701 0300 0000 5400 5300  TabBing.....T.S.
-00005ef0: 6500 7200 7600 6500 7200 2000 fc00 6200  e.r.v.e.r. ...b.
-00005f00: 6500 7200 6c00 6100 7300 7400 6500 7400  e.r.l.a.s.t.e.t.
-00005f10: 2c00 2000 6200 6900 7400 7400 6500 2000  ,. .b.i.t.t.e. .
-00005f20: 6e00 6f00 6300 6800 6d00 6100 6c00 2000  n.o.c.h.m.a.l. .
-00005f30: 7000 7200 6f00 6200 6900 6500 7200 6500  p.r.o.b.i.e.r.e.
-00005f40: 6e08 0000 0000 0600 0000 2153 6572 7665  n.........!Serve
-00005f50: 7220 6f76 6572 6c6f 6164 2c20 706c 6561  r overload, plea
-00005f60: 7365 2074 7279 2061 6761 696e 0700 0000  se try again....
-00005f70: 0a4d 6170 5461 6242 696e 6701 0300 0000  .MapTabBing.....
-00005f80: 1e00 4b00 6100 7200 7400 6500 2000 2800  ..K.a.r.t.e. .(.
-00005f90: 2600 4700 6f00 6f00 6700 6c00 6500 2908  &.G.o.o.g.l.e.).
-00005fa0: 0000 0000 0600 0000 0d4d 6170 2028 2647  .........Map (&G
-00005fb0: 6f6f 676c 6529 0700 0000 0c4d 6170 5461  oogle).....MapTa
-00005fc0: 6247 6f6f 676c 6501 0300 0000 5600 5300  bGoogle.....V.S.
-00005fd0: 7500 6300 6800 6500 2000 7500 6e00 6400  u.c.h.e. .u.n.d.
-00005fe0: 2000 4800 f600 6800 6500 6e00 6500 7200   .H...h.e.n.e.r.
-00005ff0: 6d00 6900 7400 7400 6c00 7500 6e00 6700  m.i.t.t.l.u.n.g.
-00006000: 2000 7000 6f00 7700 6500 7200 6500 6400   .p.o.w.e.r.e.d.
-00006010: 2000 6200 7900 2000 4700 6f00 6f00 6700   .b.y. .G.o.o.g.
-00006020: 6c00 6508 0000 0000 0600 0000 2c53 6561  l.e.........,Sea
-00006030: 7263 6820 616e 6420 616c 7469 7475 6465  rch and altitude
-00006040: 206c 6f6f 6b75 7020 706f 7765 7265 6420   lookup powered 
-00006050: 6279 2047 6f6f 676c 6507 0000 000c 4d61  by Google.....Ma
-00006060: 7054 6162 476f 6f67 6c65 0103 0000 001e  pTabGoogle......
-00006070: 004b 0061 0072 0074 0065 0020 0028 0026  .K.a.r.t.e. .(.&
-00006080: 004d 0061 0070 0062 006f 0078 0029 0800  .M.a.p.b.o.x.)..
-00006090: 0000 0006 0000 000d 4d61 7020 2826 4d61  ........Map (&Ma
-000060a0: 7062 6f78 2907 0000 000c 4d61 7054 6162  pbox).....MapTab
-000060b0: 4d61 7062 6f78 0103 0000 0020 0053 0075  Mapbox..... .S.u
-000060c0: 0063 0068 0065 0020 006d 0069 0074 0020  .c.h.e. .m.i.t. 
-000060d0: 004d 0061 0070 0062 006f 0078 0800 0000  .M.a.p.b.o.x....
-000060e0: 0006 0000 0018 5365 6172 6368 2070 6f77  ......Search pow
-000060f0: 6572 6564 2062 7920 4d61 7062 6f78 0700  ered by Mapbox..
-00006100: 0000 0c4d 6170 5461 624d 6170 626f 7801  ...MapTabMapbox.
-00006110: 0300 0000 1800 dc00 6200 6500 7200 2000  ........b.e.r. .
-00006120: 5000 6800 6f00 7400 6900 6e00 6908 0000  P.h.o.t.i.n.i...
-00006130: 0000 0600 0000 0d41 626f 7574 2050 686f  .......About Pho
-00006140: 7469 6e69 0700 0000 074d 656e 7542 6172  tini.....MenuBar
-00006150: 0103 0000 0080 0045 0069 006e 0020 0065  .......E.i.n. .e
-00006160: 0069 006e 0066 0061 0063 0068 0020 007a  .i.n.f.a.c.h. .z
-00006170: 0075 0020 0062 0065 0064 0069 0065 006e  .u. .b.e.d.i.e.n
-00006180: 0065 006e 0064 0065 0072 0020 004d 0065  .e.n.d.e.r. .M.e
-00006190: 0074 0061 0064 0061 0074 0065 006e 002d  .t.a.d.a.t.e.n.-
-000061a0: 0045 0064 0069 0074 006f 0072 0020 0066  .E.d.i.t.o.r. .f
-000061b0: 00fc 0072 0020 0064 0069 0067 0069 0074  ...r. .d.i.g.i.t
-000061c0: 0061 006c 0065 0020 0042 0069 006c 0064  .a.l.e. .B.i.l.d
-000061d0: 0065 0072 002e 0800 0000 0006 0000 0051  .e.r...........Q
-000061e0: 416e 2065 6173 7920 746f 2075 7365 2064  An easy to use d
-000061f0: 6967 6974 616c 2070 686f 746f 6772 6170  igital photograp
-00006200: 6820 6d65 7461 6461 7461 2028 4578 6966  h metadata (Exif
-00006210: 2c20 4950 5443 2c20 584d 5029 2065 6469  , IPTC, XMP) edi
-00006220: 7469 6e67 2061 7070 6c69 6361 7469 6f6e  ting application
-00006230: 2e07 0000 0007 4d65 6e75 4261 7201 0300  ......MenuBar...
-00006240: 0000 3200 4100 7500 6600 2000 4100 6b00  ..2.A.u.f. .A.k.
-00006250: 7400 7500 6100 6c00 6900 7300 6900 6500  t.u.a.l.i.s.i.e.
-00006260: 7200 7500 6e00 6700 2000 7000 7200 fc00  r.u.n.g. .p.r...
-00006270: 6600 6500 6e08 0000 0000 0600 0000 1043  f.e.n..........C
-00006280: 6865 636b 2066 6f72 2075 7064 6174 6507  heck for update.
-00006290: 0000 0007 4d65 6e75 4261 7201 0300 0000  ....MenuBar.....
-000062a0: 2c00 4100 6c00 6c00 6500 2000 4400 6100  ,.A.l.l.e. .D.a.
-000062b0: 7400 6500 6900 6500 6e00 2000 7300 6300  t.e.i.e.n. .s.c.
-000062c0: 6800 6c00 6900 6500 df00 6500 6e08 0000  h.l.i.e...e.n...
-000062d0: 0000 0600 0000 0f43 6c6f 7365 2061 6c6c  .......Close all
-000062e0: 2066 696c 6573 0700 0000 074d 656e 7542   files.....MenuB
-000062f0: 6172 0103 0000 003c 0052 0065 0063 0068  ar.....<.R.e.c.h
-00006300: 0074 0073 0063 0068 0072 0065 0069 0062  .t.s.c.h.r.e.i.b
-00006310: 0070 0072 00fc 0066 0075 006e 0067 0020  .p.r...f.u.n.g. 
-00006320: 0061 006b 0074 0069 0076 0069 0065 0072  .a.k.t.i.v.i.e.r
-00006330: 0065 006e 0800 0000 0006 0000 0012 456e  .e.n..........En
-00006340: 6162 6c65 2073 7065 6c6c 2063 6865 636b  able spell check
-00006350: 0700 0000 074d 656e 7542 6172 0103 0000  .....MenuBar....
-00006360: 000a 0044 0061 0074 0065 0069 0800 0000  ...D.a.t.e.i....
-00006370: 0006 0000 0004 4669 6c65 0700 0000 074d  ......File.....M
-00006380: 656e 7542 6172 0103 0000 004c 0046 0065  enuBar.....L.F.e
-00006390: 0068 006c 0065 006e 0064 0065 0020 004d  .h.l.e.n.d.e. .M
-000063a0: 0069 006e 0069 0061 0074 0075 0072 0061  .i.n.i.a.t.u.r.a
-000063b0: 006e 0073 0069 0063 0068 0074 0065 006e  .n.s.i.c.h.t.e.n
-000063c0: 0020 006b 006f 0072 0072 0069 0067 0069  . .k.o.r.r.i.g.i
-000063d0: 0065 0072 0065 006e 0800 0000 0006 0000  .e.r.e.n........
-000063e0: 0016 4669 7820 6d69 7373 696e 6720 7468  ..Fix missing th
-000063f0: 756d 626e 6169 6c73 0700 0000 074d 656e  umbnails.....Men
-00006400: 7542 6172 0103 0000 000a 0048 0069 006c  uBar.......H.i.l
-00006410: 0066 0065 0800 0000 0006 0000 0004 4865  .f.e..........He
-00006420: 6c70 0700 0000 074d 656e 7542 6172 0103  lp.....MenuBar..
-00006430: 0000 001c 0044 0061 0074 0065 0069 0065  .....D.a.t.e.i.e
-00006440: 006e 0020 00f6 0066 0066 006e 0065 006e  .n. ...f.f.n.e.n
-00006450: 0800 0000 0006 0000 000a 4f70 656e 2066  ..........Open f
-00006460: 696c 6573 0700 0000 074d 656e 7542 6172  iles.....MenuBar
-00006470: 0103 0000 0066 0044 0065 0072 0020 0071  .....f.D.e.r. .q
-00006480: 0075 0065 006c 006c 006f 0066 0066 0065  .u.e.l.l.o.f.f.e
-00006490: 006e 0065 0020 0051 0075 0065 006c 006c  .n.e. .Q.u.e.l.l
-000064a0: 0063 006f 0064 0065 0020 0069 0073 0074  .c.o.d.e. .i.s.t
-000064b0: 0020 0076 0069 0061 0020 007b 0075 0072  . .v.i.a. .{.u.r
-000064c0: 006c 007d 0020 0065 0072 0068 00e4 006c  .l.}. .e.r.h...l
-000064d0: 0074 006c 0069 0063 0068 002e 0800 0000  .t.l.i.c.h......
-000064e0: 0006 0000 0029 4f70 656e 2073 6f75 7263  .....)Open sourc
-000064f0: 6520 7061 636b 6167 6520 6176 6169 6c61  e package availa
-00006500: 626c 6520 6672 6f6d 207b 7572 6c7d 2e07  ble from {url}..
-00006510: 0000 0007 4d65 6e75 4261 7201 0300 0000  ....MenuBar.....
-00006520: 1000 4f00 7000 7400 6900 6f00 6e00 6500  ..O.p.t.i.o.n.e.
-00006530: 6e08 0000 0000 0600 0000 074f 7074 696f  n..........Optio
-00006540: 6e73 0700 0000 074d 656e 7542 6172 0103  ns.....MenuBar..
-00006550: 0000 0030 0044 006f 006b 0075 006d 0065  ...0.D.o.k.u.m.e
-00006560: 006e 0074 0061 0074 0069 006f 006e 0020  .n.t.a.t.i.o.n. 
-00006570: 007a 0075 0020 0050 0068 006f 0074 0069  .z.u. .P.h.o.t.i
-00006580: 006e 0069 0800 0000 0006 0000 0015 5068  .n.i..........Ph
-00006590: 6f74 696e 6920 646f 6375 6d65 6e74 6174  otini documentat
-000065a0: 696f 6e07 0000 0007 4d65 6e75 4261 7201  ion.....MenuBar.
-000065b0: 0300 0000 3600 5000 6800 6f00 7400 6900  ....6.P.h.o.t.i.
-000065c0: 6e00 6900 2d00 4600 6f00 7400 6f00 6d00  n.i.-.F.o.t.o.m.
-000065d0: 6500 7400 6100 6400 6100 7400 6500 6e00  e.t.a.d.a.t.e.n.
-000065e0: 6500 6400 6900 7400 6f00 7208 0000 0000  e.d.i.t.o.r.....
-000065f0: 0600 0000 1d50 686f 7469 6e69 2070 686f  .....Photini pho
-00006600: 746f 206d 6574 6164 6174 6120 6564 6974  to metadata edit
-00006610: 6f72 0700 0000 074d 656e 7542 6172 0103  or.....MenuBar..
-00006620: 0000 001a 0050 0068 006f 0074 0069 006e  .....P.h.o.t.i.n
-00006630: 0069 003a 0020 00fc 0062 0065 0072 0800  .i.:. ...b.e.r..
-00006640: 0000 0006 0000 000e 5068 6f74 696e 693a  ........Photini:
-00006650: 2061 626f 7574 0700 0000 074d 656e 7542   about.....MenuB
-00006660: 6172 0103 0000 0030 0050 0068 006f 0074  ar.....0.P.h.o.t
-00006670: 0069 006e 0069 003a 0020 0056 0065 0072  .i.n.i.:. .V.e.r
-00006680: 0073 0069 006f 006e 0073 0070 0072 00fc  .s.i.o.n.s.p.r..
-00006690: 0066 0075 006e 0067 0800 0000 0006 0000  .f.u.n.g........
-000066a0: 0016 5068 6f74 696e 693a 2076 6572 7369  ..Photini: versi
-000066b0: 6f6e 2063 6865 636b 0700 0000 074d 656e  on check.....Men
-000066c0: 7542 6172 0103 0000 0012 0053 0063 0068  uBar.......S.c.h
-000066d0: 006c 0069 0065 00df 0065 006e 0800 0000  .l.i.e...e.n....
-000066e0: 0006 0000 0004 5175 6974 0700 0000 074d  ......Quit.....M
-000066f0: 656e 7542 6172 0103 0000 0028 00c4 006e  enuBar.....(...n
-00006700: 0064 0065 0072 0075 006e 0067 0065 006e  .d.e.r.u.n.g.e.n
-00006710: 0020 0073 0070 0065 0069 0063 0068 0065  . .s.p.e.i.c.h.e
-00006720: 0072 006e 0800 0000 0006 0000 000c 5361  .r.n..........Sa
-00006730: 7665 2063 6861 6e67 6573 0700 0000 074d  ve changes.....M
-00006740: 656e 7542 6172 0103 0000 0024 0041 0075  enuBar.....$.A.u
-00006750: 0073 0067 0065 0077 00e4 0068 006c 0074  .s.g.e.w...h.l.t
-00006760: 0065 0020 0042 0069 006c 0064 0065 0072  .e. .B.i.l.d.e.r
-00006770: 0800 0000 0006 0000 000f 5365 6c65 6374  ..........Select
-00006780: 6564 2069 6d61 6765 7307 0000 0007 4d65  ed images.....Me
-00006790: 6e75 4261 7201 0300 0000 1a00 4500 6900  nuBar.......E.i.
-000067a0: 6e00 7300 7400 6500 6c00 6c00 7500 6e00  n.s.t.e.l.l.u.n.
-000067b0: 6700 6500 6e08 0000 0000 0600 0000 0853  g.e.n..........S
-000067c0: 6574 7469 6e67 7307 0000 0007 4d65 6e75  ettings.....Menu
-000067d0: 4261 7201 0300 0000 1e00 5200 6500 6300  Bar.......R.e.c.
-000067e0: 6800 7400 7300 6300 6800 7200 6500 6900  h.t.s.c.h.r.e.i.
-000067f0: 6200 7500 6e00 6708 0000 0000 0600 0000  b.u.n.g.........
-00006800: 0853 7065 6c6c 696e 6707 0000 0007 4d65  .Spelling.....Me
-00006810: 6e75 4261 7201 0300 0001 1c00 4400 6900  nuBar.......D.i.
-00006820: 6500 7300 6500 7300 2000 5000 7200 6f00  e.s.e.s. .P.r.o.
-00006830: 6700 7200 6100 6d00 6d00 2000 7700 7500  g.r.a.m.m. .w.u.
-00006840: 7200 6400 6500 2000 7500 6e00 7400 6500  r.d.e. .u.n.t.e.
-00006850: 7200 2000 6400 6500 7200 2000 4700 4e00  r. .d.e.r. .G.N.
-00006860: 5500 2000 4700 6500 6e00 6500 7200 6100  U. .G.e.n.e.r.a.
-00006870: 6c00 2000 5000 7500 6200 6c00 6900 6300  l. .P.u.b.l.i.c.
-00006880: 2000 4c00 6900 6300 6500 6e00 7300 6500   .L.i.c.e.n.s.e.
-00006890: 2000 7600 6500 7200 f600 6600 6600 6500   .v.e.r...f.f.e.
-000068a0: 6e00 7400 6c00 6900 6300 6800 7400 2e00  n.t.l.i.c.h.t...
-000068b0: 2000 4600 fc00 7200 2000 7700 6500 6900   .F...r. .w.e.i.
-000068c0: 7400 6500 7200 6500 2000 4900 6e00 6600  t.e.r.e. .I.n.f.
-000068d0: 6f00 7200 6d00 6100 7400 6900 6f00 6e00  o.r.m.a.t.i.o.n.
-000068e0: 6500 6e00 2000 6100 7500 6600 2000 6400  e.n. .a.u.f. .d.
-000068f0: 6900 6500 2000 5300 6300 6800 6100 6c00  i.e. .S.c.h.a.l.
-00006900: 7400 6600 6c00 e400 6300 6800 6500 2020  t.f.l...c.h.e.  
-00006910: 1e00 7b00 6400 6500 7400 6100 6900 6c00  ..{.d.e.t.a.i.l.
-00006920: 7300 7d20 1c00 2000 6b00 6c00 6900 6300  s.} .. .k.l.i.c.
-00006930: 6b00 6500 6e00 2e08 0000 0000 0600 0000  k.e.n...........
-00006940: 6554 6869 7320 7072 6f67 7261 6d20 6973  eThis program is
-00006950: 2072 656c 6561 7365 6420 7769 7468 2061   released with a
-00006960: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
-00006970: 6c69 6320 4c69 6365 6e73 652e 2046 6f72  lic License. For
-00006980: 2064 6574 6169 6c73 2063 6c69 636b 2074   details click t
-00006990: 6865 2022 7b64 6574 6169 6c73 7d22 2062  he "{details}" b
-000069a0: 7574 746f 6e2e 0700 0000 074d 656e 7542  utton......MenuB
-000069b0: 6172 0103 0000 00a6 0053 0069 0065 0020  ar.......S.i.e. 
-000069c0: 0076 0065 0072 0077 0065 006e 0064 0065  .v.e.r.w.e.n.d.e
-000069d0: 006e 0020 0064 0065 0072 007a 0065 0069  .n. .d.e.r.z.e.i
-000069e0: 0074 0020 0050 0068 006f 0074 0069 006e  .t. .P.h.o.t.i.n
-000069f0: 0069 0020 0056 0065 0072 0073 0069 006f  .i. .V.e.r.s.i.o
-00006a00: 006e 0020 007b 0076 0065 0072 0073 0069  .n. .{.v.e.r.s.i
-00006a10: 006f 006e 007d 002e 0020 0044 0069 0065  .o.n.}... .D.i.e
-00006a20: 0020 006e 0065 0075 0065 0073 0074 0065  . .n.e.u.e.s.t.e
-00006a30: 0020 0056 0065 0072 0073 0069 006f 006e  . .V.e.r.s.i.o.n
-00006a40: 0020 0069 0073 0074 0020 007b 0072 0065  . .i.s.t. .{.r.e
-00006a50: 006c 0065 0061 0073 0065 007d 002e 0800  .l.e.a.s.e.}....
-00006a60: 0000 0006 0000 0055 596f 7520 6172 6520  .......UYou are 
-00006a70: 6375 7272 656e 746c 7920 7275 6e6e 696e  currently runnin
-00006a80: 6720 5068 6f74 696e 6920 7665 7273 696f  g Photini versio
-00006a90: 6e20 7b76 6572 7369 6f6e 7d2e 2054 6865  n {version}. The
-00006aa0: 206c 6174 6573 7420 7265 6c65 6173 6520   latest release 
-00006ab0: 6973 207b 7265 6c65 6173 657d 2e07 0000  is {release}....
-00006ac0: 0007 4d65 6e75 4261 7201 0300 0000 3600  ..MenuBar.....6.
-00006ad0: 2600 4500 6900 6700 6500 6e00 7400 fc00  &.E.i.g.e.n.t...
-00006ae0: 6d00 6500 7200 7300 6300 6800 6100 6600  m.e.r.s.c.h.a.f.
-00006af0: 7400 2d00 4d00 6500 7400 6100 6400 6100  t.-.M.e.t.a.d.a.
-00006b00: 7400 6500 6e08 0000 0000 0600 0000 1326  t.e.n..........&
-00006b10: 4f77 6e65 7273 6869 7020 6d65 7461 6461  Ownership metada
-00006b20: 7461 0700 0000 084f 776e 6572 5461 6201  ta.....OwnerTab.
-00006b30: 0300 0000 2e00 4100 6c00 6c00 6500 2000  ......A.l.l.e. .
-00006b40: 5200 6500 6300 6800 7400 6500 2000 7600  R.e.c.h.t.e. .v.
-00006b50: 6f00 7200 6200 6500 6800 6100 6c00 7400  o.r.b.e.h.a.l.t.
-00006b60: 6500 6e08 0000 0000 0600 0000 1341 6c6c  e.n..........All
-00006b70: 2072 6967 6874 7320 7265 7365 7276 6564   rights reserved
-00006b80: 0700 0000 084f 776e 6572 5461 6201 0300  .....OwnerTab...
-00006b90: 0000 2000 5600 6f00 7200 6c00 6100 6700  .. .V.o.r.l.a.g.
-00006ba0: 6500 2000 6100 6e00 7700 6500 6e00 6400  e. .a.n.w.e.n.d.
-00006bb0: 6500 6e08 0000 0000 0600 0000 0e41 7070  e.n..........App
-00006bc0: 6c79 2074 656d 706c 6174 6507 0000 0008  ly template.....
-00006bd0: 4f77 6e65 7254 6162 0103 0000 003a 004e  OwnerTab.....:.N
-00006be0: 0061 006d 0065 006e 0073 006e 0065 006e  .a.m.e.n.s.n.e.n
-00006bf0: 006e 0075 006e 0067 0020 0034 002e 0030  .n.u.n.g. .4...0
-00006c00: 0020 0028 0043 0043 0020 0042 0059 0020  . .(.C.C. .B.Y. 
-00006c10: 0034 002e 0030 0029 0800 0000 0006 0000  .4...0.)........
-00006c20: 001b 4174 7472 6962 7574 696f 6e20 342e  ..Attribution 4.
-00006c30: 3020 2843 4320 4259 2034 2e30 2907 0000  0 (CC BY 4.0)...
-00006c40: 0008 4f77 6e65 7254 6162 0103 0000 006c  ..OwnerTab.....l
-00006c50: 004e 0061 006d 0065 006e 0073 006e 0065  .N.a.m.e.n.s.n.e
-00006c60: 006e 006e 0075 006e 0067 0020 002d 0020  .n.n.u.n.g. .-. 
-00006c70: 004b 0065 0069 006e 0065 0020 0042 0065  .K.e.i.n.e. .B.e
-00006c80: 0061 0072 0062 0065 0069 0074 0075 006e  .a.r.b.e.i.t.u.n
-00006c90: 0067 0065 006e 0020 0034 002e 0030 0020  .g.e.n. .4...0. 
-00006ca0: 0028 0043 0043 0020 0042 0059 002d 004e  .(.C.C. .B.Y.-.N
-00006cb0: 0044 0020 0034 002e 0030 0029 0800 0000  .D. .4...0.)....
-00006cc0: 0006 0000 002c 4174 7472 6962 7574 696f  .....,Attributio
-00006cd0: 6e2d 4e6f 4465 7269 7661 7469 7665 7320  n-NoDerivatives 
-00006ce0: 342e 3020 2843 4320 4259 2d4e 4420 342e  4.0 (CC BY-ND 4.
-00006cf0: 3029 0700 0000 084f 776e 6572 5461 6201  0).....OwnerTab.
-00006d00: 0300 0000 6400 4e00 6100 6d00 6500 6e00  ....d.N.a.m.e.n.
-00006d10: 7300 6e00 6500 6e00 6e00 7500 6e00 6700  s.n.e.n.n.u.n.g.
-00006d20: 2d00 4e00 6900 6300 6800 7400 2000 6b00  -.N.i.c.h.t. .k.
-00006d30: 6f00 6d00 6d00 6500 7200 7a00 6900 6500  o.m.m.e.r.z.i.e.
-00006d40: 6c00 6c00 2000 3400 2e00 3000 2000 2800  l.l. .4...0. .(.
-00006d50: 4300 4300 2000 4200 5900 2d00 4e00 4300  C.C. .B.Y.-.N.C.
-00006d60: 2000 3400 2e00 3000 2908 0000 0000 0600   .4...0.).......
-00006d70: 0000 2c41 7474 7269 6275 7469 6f6e 2d4e  ..,Attribution-N
-00006d80: 6f6e 436f 6d6d 6572 6369 616c 2034 2e30  onCommercial 4.0
-00006d90: 2028 4343 2042 592d 4e43 2034 2e30 2907   (CC BY-NC 4.0).
-00006da0: 0000 0008 4f77 6e65 7254 6162 0103 0000  ....OwnerTab....
-00006db0: 009a 004e 0061 006d 0065 006e 0073 006e  ...N.a.m.e.n.s.n
-00006dc0: 0065 006e 006e 0075 006e 0067 0020 002d  .e.n.n.u.n.g. .-
-00006dd0: 0020 004e 0069 0063 0068 0074 0020 006b  . .N.i.c.h.t. .k
-00006de0: 006f 006d 006d 0065 0072 007a 0069 0065  .o.m.m.e.r.z.i.e
-00006df0: 006c 006c 0020 002d 0020 004b 0065 0069  .l.l. .-. .K.e.i
-00006e00: 006e 0065 0020 0042 0065 0061 0072 0062  .n.e. .B.e.a.r.b
-00006e10: 0065 0069 0074 0075 006e 0067 0065 006e  .e.i.t.u.n.g.e.n
-00006e20: 0020 0034 002e 0030 0020 0028 0043 0043  . .4...0. .(.C.C
-00006e30: 0020 0042 0059 002d 004e 0043 002d 004e  . .B.Y.-.N.C.-.N
-00006e40: 0044 0020 0034 002e 0030 0029 0800 0000  .D. .4...0.)....
-00006e50: 0006 0000 003d 4174 7472 6962 7574 696f  .....=Attributio
-00006e60: 6e2d 4e6f 6e43 6f6d 6d65 7263 6961 6c2d  n-NonCommercial-
-00006e70: 4e6f 4465 7269 7661 7469 7665 7320 342e  NoDerivatives 4.
-00006e80: 3020 2843 4320 4259 2d4e 432d 4e44 2034  0 (CC BY-NC-ND 4
-00006e90: 2e30 2907 0000 0008 4f77 6e65 7254 6162  .0).....OwnerTab
-00006ea0: 0103 0000 00be 004e 0061 006d 0065 006e  .......N.a.m.e.n
-00006eb0: 0073 006e 0065 006e 006e 0075 006e 0067  .s.n.e.n.n.u.n.g
-00006ec0: 0020 002d 0020 004e 0069 0063 0068 0074  . .-. .N.i.c.h.t
-00006ed0: 002d 006b 006f 006d 006d 0065 0072 007a  .-.k.o.m.m.e.r.z
-00006ee0: 0069 0065 006c 006c 0020 002d 0020 0057  .i.e.l.l. .-. .W
-00006ef0: 0065 0069 0074 0065 0072 0067 0061 0062  .e.i.t.e.r.g.a.b
-00006f00: 0065 0020 0075 006e 0074 0065 0072 0020  .e. .u.n.t.e.r. 
-00006f10: 0067 006c 0065 0069 0063 0068 0065 006e  .g.l.e.i.c.h.e.n
-00006f20: 0020 0042 0065 0064 0069 006e 0067 0075  . .B.e.d.i.n.g.u
-00006f30: 006e 0067 0065 006e 0020 0034 002e 0030  .n.g.e.n. .4...0
-00006f40: 0020 0028 0043 0043 0020 0042 0059 002d  . .(.C.C. .B.Y.-
-00006f50: 004e 0043 002d 0053 0041 0020 0034 002e  .N.C.-.S.A. .4..
-00006f60: 0030 0029 0800 0000 0006 0000 003a 4174  .0.).........:At
-00006f70: 7472 6962 7574 696f 6e2d 4e6f 6e43 6f6d  tribution-NonCom
-00006f80: 6d65 7263 6961 6c2d 5368 6172 6541 6c69  mercial-ShareAli
-00006f90: 6b65 2034 2e30 2028 4343 2042 592d 4e43  ke 4.0 (CC BY-NC
-00006fa0: 2d53 4120 342e 3029 0700 0000 084f 776e  -SA 4.0).....Own
-00006fb0: 6572 5461 6201 0300 0000 9000 4e00 6100  erTab.......N.a.
-00006fc0: 6d00 6500 6e00 7300 6e00 6500 6e00 6e00  m.e.n.s.n.e.n.n.
-00006fd0: 7500 6e00 6700 2000 2d00 2000 5700 6500  u.n.g. .-. .W.e.
-00006fe0: 6900 7400 6500 7200 6700 6100 6200 6500  i.t.e.r.g.a.b.e.
-00006ff0: 2000 7500 6e00 7400 6500 7200 2000 6700   .u.n.t.e.r. .g.
-00007000: 6c00 6500 6900 6300 6800 6500 6e00 2000  l.e.i.c.h.e.n. .
-00007010: 4200 6500 6400 6900 6e00 6700 7500 6e00  B.e.d.i.n.g.u.n.
-00007020: 6700 6500 6e00 2000 3400 2e00 3000 2000  g.e.n. .4...0. .
-00007030: 2800 4300 4300 2000 4200 5900 2d00 5300  (.C.C. .B.Y.-.S.
-00007040: 4100 2000 3400 2e00 3000 2908 0000 0000  A. .4...0.).....
-00007050: 0600 0000 2941 7474 7269 6275 7469 6f6e  ....)Attribution
-00007060: 2d53 6861 7265 416c 696b 6520 342e 3020  -ShareAlike 4.0 
-00007070: 2843 4320 4259 2d53 4120 342e 3029 0700  (CC BY-SA 4.0)..
-00007080: 0000 084f 776e 6572 5461 6201 0300 0000  ...OwnerTab.....
-00007090: 6a00 4300 4300 3000 2000 3100 2e00 3000  j.C.C.0. .1...0.
-000070a0: 2000 5500 6e00 6900 7600 6500 7200 7300   .U.n.i.v.e.r.s.
-000070b0: 6500 6c00 6c00 2000 2800 4300 4300 3000  e.l.l. .(.C.C.0.
-000070c0: 2000 3100 2e00 3000 2900 2000 5000 7500   .1...0.). .P.u.
-000070d0: 6200 6c00 6900 6300 2000 4400 6f00 6d00  b.l.i.c. .D.o.m.
-000070e0: 6100 6900 6e00 2000 4400 6500 6400 6900  a.i.n. .D.e.d.i.
-000070f0: 6300 6100 7400 6900 6f00 6e08 0000 0000  c.a.t.i.o.n.....
-00007100: 0600 0000 3443 4330 2031 2e30 2055 6e69  ....4CC0 1.0 Uni
-00007110: 7665 7273 616c 2028 4343 3020 312e 3029  versal (CC0 1.0)
-00007120: 2050 7562 6c69 6320 446f 6d61 696e 2044   Public Domain D
-00007130: 6564 6963 6174 696f 6e07 0000 0008 4f77  edication.....Ow
-00007140: 6e65 7254 6162 0103 0000 000a 0053 0074  nerTab.......S.t
-00007150: 0061 0064 0074 0800 0000 0006 0000 0004  .a.d.t..........
-00007160: 4369 7479 0700 0000 084f 776e 6572 5461  City.....OwnerTa
-00007170: 6201 0300 0000 2800 5500 7200 6800 6500  b.....(.U.r.h.e.
-00007180: 6200 6500 7200 7200 6500 6300 6800 7400  b.e.r.r.e.c.h.t.
-00007190: 7300 6800 6900 6e00 7700 6500 6900 7308  s.h.i.n.w.e.i.s.
-000071a0: 0000 0000 0600 0000 1043 6f70 7972 6967  .........Copyrig
-000071b0: 6874 204e 6f74 6963 6507 0000 0008 4f77  ht Notice.....Ow
-000071c0: 6e65 7254 6162 0103 0000 0008 004c 0061  nerTab.......L.a
-000071d0: 006e 0064 0800 0000 0006 0000 0007 436f  .n.d..........Co
-000071e0: 756e 7472 7907 0000 0008 4f77 6e65 7254  untry.....OwnerT
-000071f0: 6162 0103 0000 0010 0046 006f 0074 006f  ab.......F.o.t.o
-00007200: 0067 0072 0061 0066 0800 0000 0006 0000  .g.r.a.f........
-00007210: 0007 4372 6561 746f 7207 0000 0008 4f77  ..Creator.....Ow
-00007220: 6e65 7254 6162 0103 0000 002c 004e 0065  nerTab.....,.N.e
-00007230: 0075 0065 0020 004c 0069 007a 0065 006e  .u.e. .L.i.z.e.n
-00007240: 007a 0020 0064 0065 0066 0069 006e 0069  .z. .d.e.f.i.n.i
-00007250: 0065 0072 0065 006e 0800 0000 0006 0000  .e.r.e.n........
-00007260: 0012 4465 6669 6e65 206e 6577 206c 6963  ..Define new lic
-00007270: 656e 6365 0700 0000 084f 776e 6572 5461  ence.....OwnerTa
-00007280: 6201 0300 0000 2400 5600 6f00 7200 6c00  b.....$.V.o.r.l.
-00007290: 6100 6700 6500 2000 6200 6500 6100 7200  a.g.e. .b.e.a.r.
-000072a0: 6200 6500 6900 7400 6500 6e08 0000 0000  b.e.i.t.e.n.....
-000072b0: 0600 0000 0d45 6469 7420 7465 6d70 6c61  .....Edit templa
-000072c0: 7465 0700 0000 084f 776e 6572 5461 6201  te.....OwnerTab.
-000072d0: 0300 0000 1200 4500 2d00 4d00 6100 6900  ......E.-.M.a.i.
-000072e0: 6c00 2800 7300 2908 0000 0000 0600 0000  l.(.s.).........
-000072f0: 0845 6d61 696c 2873 2907 0000 0008 4f77  .Email(s).....Ow
-00007300: 6e65 7254 6162 0103 0000 00e0 0047 0065  nerTab.......G.e
-00007310: 0062 0065 006e 0020 0053 0069 0065 0020  .b.e.n. .S.i.e. 
-00007320: 0065 0069 006e 0065 006e 0020 0048 0069  .e.i.n.e.n. .H.i
-00007330: 006e 0077 0065 0069 0073 0020 0061 0075  .n.w.e.i.s. .a.u
-00007340: 0066 0020 0064 0065 006e 0020 0061 006b  .f. .d.e.n. .a.k
-00007350: 0074 0075 0065 006c 006c 0065 006e 0020  .t.u.e.l.l.e.n. 
-00007360: 0049 006e 0068 0061 0062 0065 0072 0020  .I.n.h.a.b.e.r. 
-00007370: 0064 0065 0073 0020 0055 0072 0068 0065  .d.e.s. .U.r.h.e
-00007380: 0062 0065 0072 0072 0065 0063 0068 0074  .b.e.r.r.e.c.h.t
-00007390: 0073 0020 0066 00fc 0072 0020 0064 0069  .s. .f...r. .d.i
-000073a0: 0065 0073 0065 0073 0020 0042 0069 006c  .e.s.e.s. .B.i.l
-000073b0: 0064 0020 0065 0069 006e 002c 0020 007a  .d. .e.i.n.,. .z
-000073c0: 002e 0020 0042 002e 0020 0022 00a9 0032  ... .B... ."...2
-000073d0: 0030 0030 0038 0020 004a 0061 006e 0065  .0.0.8. .J.a.n.e
-000073e0: 0020 0044 006f 0065 0022 002e 0800 0000  . .D.o.e."......
-000073f0: 0006 0000 005f 456e 7465 7220 6120 6e6f  ....._Enter a no
-00007400: 7469 6365 206f 6e20 7468 6520 6375 7272  tice on the curr
-00007410: 656e 7420 6f77 6e65 7220 6f66 2074 6865  ent owner of the
-00007420: 2063 6f70 7972 6967 6874 2066 6f72 2074   copyright for t
-00007430: 6869 7320 696d 6167 652c 2073 7563 6820  his image, such 
-00007440: 6173 2022 c2a9 3230 3038 204a 616e 6520  as "..2008 Jane 
-00007450: 446f 6522 2e07 0000 0008 4f77 6e65 7254  Doe"......OwnerT
-00007460: 6162 0103 0000 0118 0047 0065 0062 0065  ab.......G.e.b.e
-00007470: 006e 0020 0053 0069 0065 0020 0049 006e  .n. .S.i.e. .I.n
-00007480: 0066 006f 0072 006d 0061 0074 0069 006f  .f.o.r.m.a.t.i.o
-00007490: 006e 0065 006e 0020 00fc 0062 0065 0072  .n.e.n. ...b.e.r
-000074a0: 0020 0045 006d 0062 0061 0072 0067 006f  . .E.m.b.a.r.g.o
-000074b0: 0073 0020 006f 0064 0065 0072 0020 0061  .s. .o.d.e.r. .a
-000074c0: 006e 0064 0065 0072 0065 0020 0045 0069  .n.d.e.r.e. .E.i
-000074d0: 006e 0073 0063 0068 0072 00e4 006e 006b  .n.s.c.h.r...n.k
-000074e0: 0075 006e 0067 0065 006e 0020 0065 0069  .u.n.g.e.n. .e.i
-000074f0: 006e 002c 0020 0064 0069 0065 0020 006e  .n.,. .d.i.e. .n
-00007500: 0069 0063 0068 0074 0020 0064 0075 0072  .i.c.h.t. .d.u.r
-00007510: 0063 0068 0020 0064 0061 0073 0020 0046  .c.h. .d.a.s. .F
-00007520: 0065 006c 0064 0020 0052 0065 0063 0068  .e.l.d. .R.e.c.h
-00007530: 0074 0065 0076 0065 0072 0077 0065 006e  .t.e.v.e.r.w.e.n
-00007540: 0064 0075 006e 0067 0073 0062 0065 0064  .d.u.n.g.s.b.e.d
-00007550: 0069 006e 0067 0075 006e 0067 0065 006e  .i.n.g.u.n.g.e.n
-00007560: 0020 0061 0062 0067 0065 0064 0065 0063  . .a.b.g.e.d.e.c
-00007570: 006b 0074 0020 0073 0069 006e 0064 002e  .k.t. .s.i.n.d..
-00007580: 0800 0000 0006 0000 0065 456e 7465 7220  .........eEnter 
-00007590: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
-000075a0: 7420 656d 6261 7267 6f65 732c 206f 7220  t embargoes, or 
-000075b0: 6f74 6865 7220 7265 7374 7269 6374 696f  other restrictio
-000075c0: 6e73 206e 6f74 2063 6f76 6572 6564 2062  ns not covered b
-000075d0: 7920 7468 6520 5269 6768 7473 2055 7361  y the Rights Usa
-000075e0: 6765 2054 6572 6d73 2066 6965 6c64 2e07  ge Terms field..
-000075f0: 0000 0008 4f77 6e65 7254 6162 0103 0000  ....OwnerTab....
-00007600: 0072 0047 0065 0062 0065 006e 0020 0053  .r.G.e.b.e.n. .S
-00007610: 0069 0065 0020 0041 006e 0077 0065 0069  .i.e. .A.n.w.e.i
-00007620: 0073 0075 006e 0067 0065 006e 0020 007a  .s.u.n.g.e.n. .z
-00007630: 0075 0072 0020 006c 0065 0067 0061 006c  .u.r. .l.e.g.a.l
-00007640: 0065 006e 0020 004e 0075 0074 007a 0075  .e.n. .N.u.t.z.u
-00007650: 006e 0067 0020 0064 0065 0073 0020 0042  .n.g. .d.e.s. .B
-00007660: 0069 006c 0064 0065 0073 0020 0065 0069  .i.l.d.e.s. .e.i
-00007670: 006e 002e 0800 0000 0006 0000 0039 456e  .n...........9En
-00007680: 7465 7220 696e 7374 7275 6374 696f 6e73  ter instructions
-00007690: 206f 6e20 686f 7720 7468 6973 2069 6d61   on how this ima
-000076a0: 6765 2063 616e 206c 6567 616c 6c79 2062  ge can legally b
-000076b0: 6520 7573 6564 2e07 0000 0008 4f77 6e65  e used......Owne
-000076c0: 7254 6162 0103 0000 00a2 0047 0065 0062  rTab.......G.e.b
-000076d0: 0065 006e 0020 0053 0069 0065 0020 0064  .e.n. .S.i.e. .d
-000076e0: 0069 0065 0020 0053 0074 0061 0064 0074  .i.e. .S.t.a.d.t
-000076f0: 0020 0066 00fc 0072 0020 0064 0069 0065  . .f...r. .d.i.e
-00007700: 0020 0041 0064 0072 0065 0073 0073 0065  . .A.d.r.e.s.s.e
-00007710: 0020 0064 0065 0072 0020 0050 0065 0072  . .d.e.r. .P.e.r
-00007720: 0073 006f 006e 0020 0065 0069 006e 002c  .s.o.n. .e.i.n.,
-00007730: 0020 0064 0069 0065 0020 0064 0069 0065  . .d.i.e. .d.i.e
-00007740: 0073 0065 0073 0020 0042 0069 006c 0064  .s.e.s. .B.i.l.d
-00007750: 0020 0065 0072 0073 0074 0065 006c 006c  . .e.r.s.t.e.l.l
-00007760: 0074 0020 0068 0061 0074 002e 0800 0000  .t. .h.a.t......
-00007770: 0006 0000 0045 456e 7465 7220 7468 6520  .....EEnter the 
-00007780: 6369 7479 2066 6f72 2074 6865 2061 6464  city for the add
-00007790: 7265 7373 206f 6620 7468 6520 7065 7273  ress of the pers
-000077a0: 6f6e 2074 6861 7420 6372 6561 7465 6420  on that created 
-000077b0: 7468 6973 2069 6d61 6765 2e07 0000 0008  this image......
-000077c0: 4f77 6e65 7254 6162 0103 0000 00ae 0047  OwnerTab.......G
-000077d0: 0065 0062 0065 006e 0020 0053 0069 0065  .e.b.e.n. .S.i.e
-000077e0: 0020 0064 0065 006e 0020 004c 00e4 006e  . .d.e.n. .L...n
-000077f0: 0064 0065 0072 006e 0061 006d 0065 006e  .d.e.r.n.a.m.e.n
-00007800: 0020 0066 00fc 0072 0020 0064 0069 0065  . .f...r. .d.i.e
-00007810: 0020 0041 0064 0072 0065 0073 0073 0065  . .A.d.r.e.s.s.e
-00007820: 0020 0064 0065 0072 0020 0050 0065 0072  . .d.e.r. .P.e.r
-00007830: 0073 006f 006e 0020 0065 0069 006e 002c  .s.o.n. .e.i.n.,
-00007840: 0020 0064 0069 0065 0020 0064 0069 0065  . .d.i.e. .d.i.e
-00007850: 0073 0065 0073 0020 0042 0069 006c 0064  .s.e.s. .B.i.l.d
-00007860: 0020 0065 0072 0073 0074 0065 006c 006c  . .e.r.s.t.e.l.l
-00007870: 0074 0020 0068 0061 0074 002e 0800 0000  .t. .h.a.t......
-00007880: 0006 0000 004d 456e 7465 7220 7468 6520  .....MEnter the 
-00007890: 636f 756e 7472 7920 6e61 6d65 2066 6f72  country name for
-000078a0: 2074 6865 2061 6464 7265 7373 206f 6620   the address of 
-000078b0: 7468 6520 7065 7273 6f6e 2074 6861 7420  the person that 
-000078c0: 6372 6561 7465 6420 7468 6973 2069 6d61  created this ima
-000078d0: 6765 2e07 0000 0008 4f77 6e65 7254 6162  ge......OwnerTab
-000078e0: 0103 0000 00a6 0047 0065 0062 0065 006e  .......G.e.b.e.n
-000078f0: 0020 0053 0069 0065 0020 0064 0069 0065  . .S.i.e. .d.i.e
-00007900: 0020 0042 0065 0072 0075 0066 0073 0062  . .B.e.r.u.f.s.b
-00007910: 0065 007a 0065 0069 0063 0068 006e 0075  .e.z.e.i.c.h.n.u
-00007920: 006e 0067 0020 0064 0065 0072 0020 0050  .n.g. .d.e.r. .P
-00007930: 0065 0072 0073 006f 006e 0020 0065 0069  .e.r.s.o.n. .e.i
-00007940: 006e 002c 0020 0064 0069 0065 0020 0069  .n.,. .d.i.e. .i
-00007950: 006d 0020 0046 0065 006c 0064 0020 0055  .m. .F.e.l.d. .U
-00007960: 0072 0068 0065 0062 0065 0072 0020 0061  .r.h.e.b.e.r. .a
-00007970: 0075 0066 0067 0065 0066 00fc 0068 0072  .u.f.g.e.f...h.r
-00007980: 0074 0020 0069 0073 0074 002e 0800 0000  .t. .i.s.t......
-00007990: 0006 0000 003e 456e 7465 7220 7468 6520  .....>Enter the 
-000079a0: 6a6f 6220 7469 746c 6520 6f66 2074 6865  job title of the
-000079b0: 2070 6572 736f 6e20 6c69 7374 6564 2069   person listed i
-000079c0: 6e20 7468 6520 4372 6561 746f 7220 6669  n the Creator fi
-000079d0: 656c 642e 0700 0000 084f 776e 6572 5461  eld......OwnerTa
-000079e0: 6201 0300 0000 8200 4700 6500 6200 6500  b.......G.e.b.e.
-000079f0: 6e00 2000 5300 6900 6500 2000 6400 6500  n. .S.i.e. .d.e.
-00007a00: 6e00 2000 4e00 6100 6d00 6500 6e00 2000  n. .N.a.m.e.n. .
-00007a10: 6400 6500 7200 2000 5000 6500 7200 7300  d.e.r. .P.e.r.s.
-00007a20: 6f00 6e00 2000 6500 6900 6e00 2c00 2000  o.n. .e.i.n.,. .
-00007a30: 6400 6900 6500 2000 6400 6900 6500 7300  d.i.e. .d.i.e.s.
-00007a40: 6500 7300 2000 4200 6900 6c00 6400 2000  e.s. .B.i.l.d. .
-00007a50: 6500 7200 7300 7400 6500 6c00 6c00 7400  e.r.s.t.e.l.l.t.
-00007a60: 2000 6800 6100 7400 2e08 0000 0000 0600   .h.a.t.........
-00007a70: 0000 3545 6e74 6572 2074 6865 206e 616d  ..5Enter the nam
-00007a80: 6520 6f66 2074 6865 2070 6572 736f 6e20  e of the person 
-00007a90: 7468 6174 2063 7265 6174 6564 2074 6869  that created thi
-00007aa0: 7320 696d 6167 652e 0700 0000 084f 776e  s image......Own
-00007ab0: 6572 5461 6201 0300 0000 b000 4700 6500  erTab.......G.e.
-00007ac0: 6200 6500 6e00 2000 5300 6900 6500 2000  b.e.n. .S.i.e. .
-00007ad0: 6400 6900 6500 2000 5000 6f00 7300 7400  d.i.e. .P.o.s.t.
-00007ae0: 6c00 6500 6900 7400 7a00 6100 6800 6c00  l.e.i.t.z.a.h.l.
-00007af0: 2000 6600 fc00 7200 2000 6400 6900 6500   .f...r. .d.i.e.
-00007b00: 2000 4100 6400 7200 6500 7300 7300 6500   .A.d.r.e.s.s.e.
-00007b10: 2000 6400 6500 7200 2000 5000 6500 7200   .d.e.r. .P.e.r.
-00007b20: 7300 6f00 6e00 2000 6500 6900 6e00 2c00  s.o.n. .e.i.n.,.
-00007b30: 2000 6400 6900 6500 2000 6400 6900 6500   .d.i.e. .d.i.e.
-00007b40: 7300 6500 7300 2000 4200 6900 6c00 6400  s.e.s. .B.i.l.d.
-00007b50: 2000 6500 7200 7300 7400 6500 6c00 6c00   .e.r.s.t.e.l.l.
-00007b60: 7400 2000 6800 6100 7400 2e08 0000 0000  t. .h.a.t.......
-00007b70: 0600 0000 4c45 6e74 6572 2074 6865 2070  ....LEnter the p
-00007b80: 6f73 7461 6c20 636f 6465 2066 6f72 2074  ostal code for t
-00007b90: 6865 2061 6464 7265 7373 206f 6620 7468  he address of th
-00007ba0: 6520 7065 7273 6f6e 2074 6861 7420 6372  e person that cr
-00007bb0: 6561 7465 6420 7468 6973 2069 6d61 6765  eated this image
-00007bc0: 2e07 0000 0008 4f77 6e65 7254 6162 0103  ......OwnerTab..
-00007bd0: 0000 00ac 0047 0065 0062 0065 006e 0020  .....G.e.b.e.n. 
-00007be0: 0053 0069 0065 0020 0064 0061 0073 0020  .S.i.e. .d.a.s. 
-00007bf0: 0042 0075 006e 0064 0065 0073 006c 0061  .B.u.n.d.e.s.l.a
-00007c00: 006e 0064 0020 0066 00fc 0072 0020 0064  .n.d. .f...r. .d
-00007c10: 0069 0065 0020 0041 0064 0072 0065 0073  .i.e. .A.d.r.e.s
-00007c20: 0073 0065 0020 0064 0065 0072 0020 0050  .s.e. .d.e.r. .P
-00007c30: 0065 0072 0073 006f 006e 0020 0065 0069  .e.r.s.o.n. .e.i
-00007c40: 006e 002c 0020 0064 0069 0065 0020 0064  .n.,. .d.i.e. .d
-00007c50: 0069 0065 0073 0065 0073 0020 0042 0069  .i.e.s.e.s. .B.i
-00007c60: 006c 0064 0020 0065 0072 0073 0074 0065  .l.d. .e.r.s.t.e
-00007c70: 006c 006c 0074 0020 0068 0061 0074 002e  .l.l.t. .h.a.t..
-00007c80: 0800 0000 0006 0000 0046 456e 7465 7220  .........FEnter 
-00007c90: 7468 6520 7374 6174 6520 666f 7220 7468  the state for th
-00007ca0: 6520 6164 6472 6573 7320 6f66 2074 6865  e address of the
-00007cb0: 2070 6572 736f 6e20 7468 6174 2063 7265   person that cre
-00007cc0: 6174 6564 2074 6869 7320 696d 6167 652e  ated this image.
-00007cd0: 0700 0000 084f 776e 6572 5461 6201 0300  .....OwnerTab...
-00007ce0: 0000 9600 4700 6500 6200 6500 6e00 2000  ....G.e.b.e.n. .
-00007cf0: 5300 6900 6500 2000 6500 6900 6e00 2c00  S.i.e. .e.i.n.,.
-00007d00: 2000 7700 6500 7200 2000 6200 6500 6900   .w.e.r. .b.e.i.
-00007d10: 2000 6400 6500 7200 2000 5600 6500 7200   .d.e.r. .V.e.r.
-00007d20: f600 6600 6600 6500 6e00 7400 6c00 6900  ..f.f.e.n.t.l.i.
-00007d30: 6300 6800 7500 6e00 6700 2000 6400 6500  c.h.u.n.g. .d.e.
-00007d40: 7300 2000 4200 6900 6c00 6400 6500 7300  s. .B.i.l.d.e.s.
-00007d50: 2000 6700 6500 6e00 6100 6e00 6e00 7400   .g.e.n.a.n.n.t.
-00007d60: 2000 7700 6500 7200 6400 6500 6e00 2000   .w.e.r.d.e.n. .
-00007d70: 7300 6f00 6c00 6c00 2e08 0000 0000 0600  s.o.l.l.........
-00007d80: 0000 3a45 6e74 6572 2077 686f 2073 686f  ..:Enter who sho
-00007d90: 756c 6420 6265 2063 7265 6469 7465 6420  uld be credited 
-00007da0: 7768 656e 2074 6869 7320 696d 6167 6520  when this image 
-00007db0: 6973 2070 7562 6c69 7368 6564 2e07 0000  is published....
-00007dc0: 0008 4f77 6e65 7254 6162 0103 0000 002c  ..OwnerTab.....,
-00007dd0: 0056 006f 0072 006c 0061 0067 0065 0020  .V.o.r.l.a.g.e. 
-00007de0: 0069 006e 0069 0074 0069 0061 006c 0069  .i.n.i.t.i.a.l.i
-00007df0: 0073 0069 0065 0072 0065 006e 0800 0000  .s.i.e.r.e.n....
-00007e00: 0006 0000 0013 496e 6974 6961 6c69 7365  ......Initialise
-00007e10: 2074 656d 706c 6174 6507 0000 0008 4f77   template.....Ow
-00007e20: 6e65 7254 6162 0103 0000 0016 0041 006e  nerTab.......A.n
-00007e30: 0077 0065 0069 0073 0075 006e 0067 0065  .w.e.i.s.u.n.g.e
-00007e40: 006e 0800 0000 0006 0000 000c 496e 7374  .n..........Inst
-00007e50: 7275 6374 696f 6e73 0700 0000 084f 776e  ructions.....Own
-00007e60: 6572 5461 6201 0300 0000 0800 4e00 6100  erTab.......N.a.
-00007e70: 6d00 6508 0000 0000 0600 0000 044e 616d  m.e..........Nam
-00007e80: 6507 0000 0008 4f77 6e65 7254 6162 0103  e.....OwnerTab..
-00007e90: 0000 0034 004c 0069 006e 006b 0020 007a  ...4.L.i.n.k. .z
-00007ea0: 0075 0020 201e 007b 006c 0069 0063 0065  .u.  ..{.l.i.c.e
-00007eb0: 006e 0063 0065 007d 201c 0020 00f6 0066  .n.c.e.} .. ...f
-00007ec0: 0066 006e 0065 006e 0800 0000 0006 0000  .f.n.e.n........
-00007ed0: 0018 4f70 656e 206c 696e 6b20 746f 2022  ..Open link to "
-00007ee0: 7b6c 6963 656e 6365 7d22 0700 0000 084f  {licence}".....O
-00007ef0: 776e 6572 5461 6201 0300 0000 1400 5400  wnerTab.......T.
-00007f00: 6500 6c00 6500 6600 6f00 6e00 2800 6500  e.l.e.f.o.n.(.e.
-00007f10: 2908 0000 0000 0600 0000 0850 686f 6e65  )..........Phone
-00007f20: 2873 2907 0000 0008 4f77 6e65 7254 6162  (s).....OwnerTab
-00007f30: 0103 0000 0032 0050 0068 006f 0074 0069  .....2.P.h.o.t.i
-00007f40: 006e 0069 003a 0020 0045 0069 0067 0065  .n.i.:. .E.i.g.e
-00007f50: 006e 0074 0075 006d 0073 0076 006f 0072  .n.t.u.m.s.v.o.r
-00007f60: 006c 0061 0067 0065 0800 0000 0006 0000  .l.a.g.e........
-00007f70: 001b 5068 6f74 696e 693a 206f 776e 6572  ..Photini: owner
-00007f80: 7368 6970 2074 656d 706c 6174 6507 0000  ship template...
-00007f90: 0008 4f77 6e65 7254 6162 0103 0000 0018  ..OwnerTab......
-00007fa0: 0050 006f 0073 0074 006c 0065 0069 0074  .P.o.s.t.l.e.i.t
-00007fb0: 007a 0061 0068 006c 0800 0000 0006 0000  .z.a.h.l........
-00007fc0: 000b 506f 7374 616c 2043 6f64 6507 0000  ..Postal Code...
-00007fd0: 0008 4f77 6e65 7254 6162 0103 0000 002c  ..OwnerTab.....,
-00007fe0: 0050 0075 0062 006c 0069 0063 0020 0044  .P.u.b.l.i.c. .D
-00007ff0: 006f 006d 0061 0069 006e 0020 004d 0061  .o.m.a.i.n. .M.a
-00008000: 0072 006b 0020 0031 002e 0030 0800 0000  .r.k. .1...0....
-00008010: 0006 0000 0016 5075 626c 6963 2044 6f6d  ......Public Dom
-00008020: 6169 6e20 4d61 726b 2031 2e30 0700 0000  ain Mark 1.0....
-00008030: 084f 776e 6572 5461 6201 0300 0000 0c00  .OwnerTab.......
-00008040: 5200 6500 6300 6800 7400 6508 0000 0000  R.e.c.h.t.e.....
-00008050: 0600 0000 0652 6967 6874 7307 0000 0008  .....Rights.....
-00008060: 4f77 6e65 7254 6162 0103 0000 001a 0053  OwnerTab.......S
-00008070: 0074 0061 0061 0074 002f 0050 0072 006f  .t.a.a.t./.P.r.o
-00008080: 0076 0069 006e 007a 0800 0000 0006 0000  .v.i.n.z........
-00008090: 000e 5374 6174 652f 5072 6f76 696e 6365  ..State/Province
-000080a0: 0700 0000 084f 776e 6572 5461 6201 0300  .....OwnerTab...
-000080b0: 0000 0600 5500 5200 4c08 0000 0000 0600  ....U.R.L.......
-000080c0: 0000 0355 524c 0700 0000 084f 776e 6572  ...URL.....Owner
-000080d0: 5461 6201 0300 0000 2600 4e00 7500 7400  Tab.....&.N.u.t.
-000080e0: 7a00 7500 6e00 6700 7300 6200 6500 6400  z.u.n.g.s.b.e.d.
-000080f0: 6900 6e00 6700 7500 6e00 6700 6500 6e08  i.n.g.u.n.g.e.n.
-00008100: 0000 0000 0600 0000 0b55 7361 6765 2054  .........Usage T
-00008110: 6572 6d73 0700 0000 084f 776e 6572 5461  erms.....OwnerTa
-00008120: 6201 0300 0000 9800 5600 6500 7200 7700  b.......V.e.r.w.
-00008130: 6500 6e00 6400 6500 6e00 2000 5300 6900  e.n.d.e.n. .S.i.
-00008140: 6500 2000 2500 5900 2c00 2000 7500 6d00  e. .%.Y.,. .u.m.
-00008150: 2000 6400 6100 7300 2000 4a00 6100 6800   .d.a.s. .J.a.h.
-00008160: 7200 2000 6500 6900 6e00 7a00 7500 6600  r. .e.i.n.z.u.f.
-00008170: fc00 6700 6500 6e00 2c00 2000 6900 6e00  ..g.e.n.,. .i.n.
-00008180: 2000 6400 6500 6d00 2000 6400 6100 7300   .d.e.m. .d.a.s.
-00008190: 2000 4600 6f00 7400 6f00 2000 6100 7500   .F.o.t.o. .a.u.
-000081a0: 6600 6700 6500 6e00 6f00 6d00 6d00 6500  f.g.e.n.o.m.m.e.
-000081b0: 6e00 2000 7700 7500 7200 6400 6500 2e08  n. .w.u.r.d.e...
-000081c0: 0000 0000 0600 0000 3355 7365 2025 5920  ........3Use %Y 
-000081d0: 746f 2069 6e73 6572 7420 7468 6520 7965  to insert the ye
-000081e0: 6172 2074 6865 2070 686f 746f 6772 6170  ar the photograp
-000081f0: 6820 7761 7320 7461 6b65 6e2e 0700 0000  h was taken.....
-00008200: 084f 776e 6572 5461 6201 0300 0000 1a00  .OwnerTab.......
-00008210: 5700 6500 6200 2d00 4500 7200 6b00 6c00  W.e.b.-.E.r.k.l.
-00008220: e400 7200 7500 6e00 6708 0000 0000 0600  ..r.u.n.g.......
-00008230: 0000 0d57 6562 2053 7461 7465 6d65 6e74  ...Web Statement
-00008240: 0700 0000 084f 776e 6572 5461 6201 0300  .....OwnerTab...
-00008250: 0000 1400 5700 6500 6200 2d00 5500 5200  ....W.e.b.-.U.R.
-00008260: 4c00 2800 7300 2908 0000 0000 0600 0000  L.(.s.).........
-00008270: 0a57 6562 2055 524c 2873 2907 0000 0008  .Web URL(s).....
-00008280: 4f77 6e65 7254 6162 0103 0000 0018 003c  OwnerTab.......<
-00008290: 004e 0065 0075 0065 0020 0053 0075 0063  .N.e.u.e. .S.u.c
-000082a0: 0068 0065 003e 0800 0000 0006 0000 000c  .h.e.>..........
-000082b0: 3c6e 6577 2073 6561 7263 683e 0700 0000  <new search>....
-000082c0: 0a50 686f 7469 6e69 4d61 7001 0300 0000  .PhotiniMap.....
-000082d0: 2600 3c00 5300 7500 6300 6800 6500 2000  &.<.S.u.c.h.e. .
-000082e0: 7700 6900 6500 6400 6500 7200 6800 6f00  w.i.e.d.e.r.h.o.
-000082f0: 6c00 6500 6e00 3e08 0000 0000 0600 0000  l.e.n.>.........
-00008300: 0f3c 7265 7065 6174 2073 6561 7263 683e  .<repeat search>
-00008310: 0700 0000 0a50 686f 7469 6e69 4d61 7001  .....PhotiniMap.
-00008320: 0300 0000 1c00 3c00 7700 6900 6400 6500  ......<.w.i.d.e.
-00008330: 6e00 2000 7300 6500 6100 7200 6300 6800  n. .s.e.a.r.c.h.
-00008340: 3e08 0000 0000 0600 0000 0e3c 7769 6465  >..........<wide
-00008350: 6e20 7365 6172 6368 3e07 0000 000a 5068  n search>.....Ph
-00008360: 6f74 696e 694d 6170 0103 0000 0008 0048  otiniMap.......H
-00008370: 00f6 0068 0065 0800 0000 0006 0000 0008  ...h.e..........
-00008380: 416c 7469 7475 6465 0700 0000 0a50 686f  Altitude.....Pho
-00008390: 7469 6e69 4d61 7001 0300 0000 3000 4800  tiniMap.....0.H.
-000083a0: f600 6800 6500 2000 6100 7500 7300 2000  ..h.e. .a.u.s. .
-000083b0: 4b00 6100 7200 7400 6500 2000 6500 7200  K.a.r.t.e. .e.r.
-000083c0: 6d00 6900 7400 7400 6500 6c00 6e08 0000  m.i.t.t.e.l.n...
-000083d0: 0000 0600 0000 1547 6574 2061 6c74 6974  .......Get altit
-000083e0: 7564 6520 6672 6f6d 206d 6170 0700 0000  ude from map....
-000083f0: 0a50 686f 7469 6e69 4d61 7001 0300 0000  .PhotiniMap.....
-00008400: 1e00 4700 5000 5800 2d00 4400 6100 7400  ..G.P.X.-.D.a.t.
-00008410: 6500 6900 2000 6c00 6100 6400 6500 6e08  e.i. .l.a.d.e.n.
-00008420: 0000 0000 0600 0000 0d4c 6f61 6420 4750  .........Load GP
-00008430: 5820 6669 6c65 0700 0000 0a50 686f 7469  X file.....Photi
-00008440: 6e69 4d61 7001 0300 0000 2600 4700 5000  niMap.....&.G.P.
-00008450: 5800 2d00 4400 6100 7400 6500 6e00 2000  X.-.D.a.t.e.n. .
-00008460: 6500 6e00 7400 6600 6500 7200 6e00 6500  e.n.t.f.e.r.n.e.
-00008470: 6e08 0000 0000 0600 0000 0f52 656d 6f76  n..........Remov
-00008480: 6520 4750 5820 6461 7461 0700 0000 0a50  e GPX data.....P
-00008490: 686f 7469 6e69 4d61 7001 0300 0000 0a00  hotiniMap.......
-000084a0: 5300 7500 6300 6800 6508 0000 0000 0600  S.u.c.h.e.......
-000084b0: 0000 0653 6561 7263 6807 0000 000a 5068  ...Search.....Ph
-000084c0: 6f74 696e 694d 6170 0103 0000 003a 004b  otiniMap.....:.K
-000084d0: 006f 006f 0072 0064 0069 006e 0061 0074  .o.o.r.d.i.n.a.t
-000084e0: 0065 006e 0020 0061 0075 0073 0020 0047  .e.n. .a.u.s. .G
-000084f0: 0050 0058 0020 0066 0065 0073 0074 006c  .P.X. .f.e.s.t.l
-00008500: 0065 0067 0065 006e 0800 0000 0006 0000  .e.g.e.n........
-00008510: 0013 5365 7420 636f 6f72 6473 2066 726f  ..Set coords fro
-00008520: 6d20 4750 5807 0000 000a 5068 6f74 696e  m GPX.....Photin
-00008530: 694d 6170 0103 0000 0030 005a 0075 0020  iMap.....0.Z.u. 
-00008540: 0053 0061 006d 006d 006c 0075 006e 0067  .S.a.m.m.l.u.n.g
-00008550: 0065 006e 0020 0068 0069 006e 007a 0075  .e.n. .h.i.n.z.u
-00008560: 0066 00fc 0067 0065 006e 0800 0000 0006  .f...g.e.n......
-00008570: 0000 0012 4164 6420 746f 2063 6f6c 6c65  ....Add to colle
-00008580: 6374 696f 6e73 0700 0000 0b50 6978 656c  ctions.....Pixel
-00008590: 6665 6454 6162 0103 0000 002e 0041 006c  fedTab.......A.l
-000085a0: 006c 0065 0020 0052 0065 0063 0068 0074  .l.e. .R.e.c.h.t
-000085b0: 0065 0020 0056 006f 0072 0062 0065 0068  .e. .V.o.r.b.e.h
-000085c0: 0061 006c 0074 0065 006e 0800 0000 0006  .a.l.t.e.n......
-000085d0: 0000 0013 416c 6c20 5269 6768 7473 2052  ....All Rights R
-000085e0: 6573 6572 7665 6407 0000 000b 5069 7865  eserved.....Pixe
-000085f0: 6c66 6564 5461 6201 0300 0000 1a00 4e00  lfedTab.......N.
-00008600: 6100 6d00 6500 6e00 7300 6e00 6500 6e00  a.m.e.n.s.n.e.n.
-00008610: 6e00 7500 6e00 6708 0000 0000 0600 0000  n.u.n.g.........
-00008620: 0b41 7474 7269 6275 7469 6f6e 0700 0000  .Attribution....
-00008630: 0b50 6978 656c 6665 6454 6162 0103 0000  .PixelfedTab....
-00008640: 0020 0042 0069 006c 0064 0075 006e 0074  . .B.i.l.d.u.n.t
-00008650: 0065 0072 0073 0063 0068 0072 0069 0066  .e.r.s.c.h.r.i.f
-00008660: 0074 0800 0000 0006 0000 0007 4361 7074  .t..........Capt
-00008670: 696f 6e07 0000 000b 5069 7865 6c66 6564  ion.....Pixelfed
-00008680: 5461 6201 0300 0000 3600 5700 e400 6800  Tab.....6.W...h.
-00008690: 6c00 6500 6e00 2000 5300 6900 6500 2000  l.e.n. .S.i.e. .
-000086a0: 6500 6900 6e00 6500 2000 4900 6e00 7300  e.i.n.e. .I.n.s.
-000086b0: 7400 6100 6e00 7a00 2000 6100 7500 7308  t.a.n.z. .a.u.s.
-000086c0: 0000 0000 0600 0000 1243 686f 6f73 6520  .........Choose 
-000086d0: 616e 2069 6e73 7461 6e63 6507 0000 000b  an instance.....
-000086e0: 5069 7865 6c66 6564 5461 6201 0300 0000  PixelfedTab.....
-000086f0: 3200 5300 6900 6300 6800 7400 6200 6100  2.S.i.c.h.t.b.a.
-00008700: 7200 6b00 6500 6900 7400 2000 6400 6500  r.k.e.i.t. .d.e.
-00008710: 7200 2000 5300 6100 6d00 6d00 6c00 7500  r. .S.a.m.m.l.u.
-00008720: 6e00 6708 0000 0000 0600 0000 1543 6f6c  n.g..........Col
-00008730: 6c65 6374 696f 6e20 7669 7369 6269 6c69  lection visibili
-00008740: 7479 0700 0000 0b50 6978 656c 6665 6454  ty.....PixelfedT
-00008750: 6162 0103 0000 002e 004e 0065 0075 0065  ab.......N.e.u.e
-00008760: 0020 0053 0061 006d 006d 006c 0075 006e  . .S.a.m.m.l.u.n
-00008770: 0067 0020 0065 0072 0073 0074 0065 006c  .g. .e.r.s.t.e.l
-00008780: 006c 0065 006e 0800 0000 0006 0000 0015  .l.e.n..........
-00008790: 4372 6561 7465 206e 6577 2063 6f6c 6c65  Create new colle
-000087a0: 6374 696f 6e07 0000 000b 5069 7865 6c66  ction.....Pixelf
-000087b0: 6564 5461 6201 0300 0000 1800 4200 6500  edTab.......B.e.
-000087c0: 7300 6300 6800 7200 6500 6900 6200 7500  s.c.h.r.e.i.b.u.
-000087d0: 6e00 6708 0000 0000 0600 0000 0b44 6573  n.g..........Des
-000087e0: 6372 6970 7469 6f6e 0700 0000 0b50 6978  cription.....Pix
-000087f0: 656c 6665 6454 6162 0103 0000 002e 004b  elfedTab.......K
-00008800: 006f 006d 006d 0065 006e 0074 0061 0072  .o.m.m.e.n.t.a.r
-00008810: 0065 0020 0064 0065 0061 006b 0074 0069  .e. .d.e.a.k.t.i
-00008820: 0076 0069 0065 0072 0065 006e 0800 0000  .v.i.e.r.e.n....
-00008830: 0006 0000 0010 4469 7361 626c 6520 636f  ......Disable co
-00008840: 6d6d 656e 7473 0700 0000 0b50 6978 656c  mments.....Pixel
-00008850: 6665 6454 6162 0103 0000 000e 0045 006e  fedTab.......E.n
-00008860: 0074 0077 0075 0072 0066 0800 0000 0006  .t.w.u.r.f......
-00008870: 0000 0005 4472 6166 7407 0000 000b 5069  ....Draft.....Pi
-00008880: 7865 6c66 6564 5461 6201 0300 0000 1400  xelfedTab.......
-00008890: 4e00 7500 7200 2000 4600 6f00 6c00 6700  N.u.r. .F.o.l.g.
-000088a0: 6500 7208 0000 0000 0600 0000 0e46 6f6c  e.r..........Fol
-000088b0: 6c6f 7765 7273 206f 6e6c 7907 0000 000b  lowers only.....
-000088c0: 5069 7865 6c66 6564 5461 6201 0300 0000  PixelfedTab.....
-000088d0: 1400 4700 6500 6e00 6500 7200 6900 6500  ..G.e.n.e.r.i.e.
-000088e0: 7200 6500 6e08 0000 0000 0600 0000 0847  r.e.n..........G
-000088f0: 656e 6572 6174 6507 0000 000b 5069 7865  enerate.....Pixe
-00008900: 6c66 6564 5461 6201 0300 0000 0c00 4c00  lfedTab.......L.
-00008910: 6900 7a00 6500 6e00 7a08 0000 0000 0600  i.z.e.n.z.......
-00008920: 0000 074c 6963 656e 6365 0700 0000 0b50  ...Licence.....P
-00008930: 6978 656c 6665 6454 6162 0103 0000 0028  ixelfedTab.....(
-00008940: 0046 0065 0068 006c 0065 006e 0064 0065  .F.e.h.l.e.n.d.e
-00008950: 0072 0020 0061 006c 0074 002e 0020 0054  .r. .a.l.t... .T
-00008960: 0065 0078 0074 002e 0800 0000 0006 0000  .e.x.t..........
-00008970: 0011 4d69 7373 696e 6720 616c 7420 7465  ..Missing alt te
-00008980: 7874 2e07 0000 000b 5069 7865 6c66 6564  xt......Pixelfed
-00008990: 5461 6201 0300 0000 1a00 4e00 6500 7500  Tab.......N.e.u.
-000089a0: 6500 2000 5300 6100 6d00 6d00 6c00 7500  e. .S.a.m.m.l.u.
-000089b0: 6e00 6708 0000 0000 0600 0000 0e4e 6577  n.g..........New
-000089c0: 2063 6f6c 6c65 6374 696f 6e07 0000 000b   collection.....
-000089d0: 5069 7865 6c66 6564 5461 6201 0300 0000  PixelfedTab.....
-000089e0: 0c00 4100 6e00 6400 6500 7200 6508 0000  ..A.n.d.e.r.e...
-000089f0: 0000 0600 0000 054f 7468 6572 0700 0000  .......Other....
-00008a00: 0b50 6978 656c 6665 6454 6162 0103 0000  .PixelfedTab....
-00008a10: 0024 0050 0068 006f 0074 0069 006e 0069  .$.P.h.o.t.i.n.i
-00008a20: 003a 0020 0061 006c 0074 002e 0020 0054  .:. .a.l.t... .T
-00008a30: 0065 0078 0074 0800 0000 0006 0000 0011  .e.x.t..........
-00008a40: 5068 6f74 696e 693a 2061 6c74 2074 6578  Photini: alt tex
-00008a50: 7407 0000 000b 5069 7865 6c66 6564 5461  t.....PixelfedTa
-00008a60: 6201 0300 0000 3400 5000 6800 6f00 7400  b.....4.P.h.o.t.
-00008a70: 6900 6e00 6900 3a00 2000 4900 6e00 7300  i.n.i.:. .I.n.s.
-00008a80: 7400 6100 6e00 7a00 2000 6100 7500 7300  t.a.n.z. .a.u.s.
-00008a90: 7700 e400 6800 6c00 6500 6e08 0000 0000  w...h.l.e.n.....
-00008aa0: 0600 0000 1850 686f 7469 6e69 3a20 6368  .....Photini: ch
-00008ab0: 6f6f 7365 2069 6e73 7461 6e63 6507 0000  oose instance...
-00008ac0: 000b 5069 7865 6c66 6564 5461 6201 0300  ..PixelfedTab...
-00008ad0: 0000 3200 5300 6900 6300 6800 7400 6200  ..2.S.i.c.h.t.b.
-00008ae0: 6100 7200 6b00 6500 6900 7400 2000 6400  a.r.k.e.i.t. .d.
-00008af0: 6500 7300 2000 4200 6500 6900 7400 7200  e.s. .B.e.i.t.r.
-00008b00: 6100 6700 7308 0000 0000 0600 0000 0f50  a.g.s..........P
-00008b10: 6f73 7420 7669 7369 6269 6c69 7479 0700  ost visibility..
-00008b20: 0000 0b50 6978 656c 6665 6454 6162 0103  ...PixelfedTab..
-00008b30: 0000 0014 00d6 0066 0066 0065 006e 0074  .......f.f.e.n.t
-00008b40: 006c 0069 0063 0068 0800 0000 0006 0000  .l.i.c.h........
-00008b50: 0006 5075 626c 6963 0700 0000 0b50 6978  ..Public.....Pix
-00008b60: 656c 6665 6454 6162 0103 0000 0032 0047  elfedTab.....2.G
-00008b70: 0065 006d 0065 0069 006e 0066 0072 0065  .e.m.e.i.n.f.r.e
-00008b80: 0069 0065 0020 0057 0069 0064 006d 0075  .i.e. .W.i.d.m.u
-00008b90: 006e 0067 0020 0028 0043 0043 0030 0029  .n.g. .(.C.C.0.)
-00008ba0: 0800 0000 0006 0000 001e 5075 626c 6963  ..........Public
-00008bb0: 2044 6f6d 6169 6e20 4465 6469 6361 7469   Domain Dedicati
-00008bc0: 6f6e 2028 4343 3029 0700 0000 0b50 6978  on (CC0).....Pix
-00008bd0: 656c 6665 6454 6162 0103 0000 0024 0047  elfedTab.....$.G
-00008be0: 0065 006d 0065 0069 006e 0066 0072 0065  .e.m.e.i.n.f.r.e
-00008bf0: 0069 0065 0020 0041 0072 0062 0065 0069  .i.e. .A.r.b.e.i
-00008c00: 0074 0800 0000 0006 0000 0012 5075 626c  .t..........Publ
-00008c10: 6963 2044 6f6d 6169 6e20 576f 726b 0700  ic Domain Work..
-00008c20: 0000 0b50 6978 656c 6665 6454 6162 0103  ...PixelfedTab..
-00008c30: 0000 002a 0056 0065 0072 0074 0072 0061  ...*.V.e.r.t.r.a
-00008c40: 0075 006c 0069 0063 0068 0065 0072 0020  .u.l.i.c.h.e.r. 
-00008c50: 0042 0065 0069 0074 0072 0061 0067 0800  .B.e.i.t.r.a.g..
-00008c60: 0000 0006 0000 000e 5365 6e73 6974 6976  ........Sensitiv
-00008c70: 6520 706f 7374 0700 0000 0b50 6978 656c  e post.....Pixel
-00008c80: 6665 6454 6162 0103 0000 000a 0054 0069  fedTab.......T.i
-00008c90: 0074 0065 006c 0800 0000 0006 0000 0005  .t.e.l..........
-00008ca0: 5469 746c 6507 0000 000b 5069 7865 6c66  Title.....Pixelf
-00008cb0: 6564 5461 6201 0300 0000 1400 5500 6e00  edTab.......U.n.
-00008cc0: 6700 6500 6c00 6900 7300 7400 6500 7408  g.e.l.i.s.t.e.t.
-00008cd0: 0000 0000 0600 0000 0855 6e6c 6973 7465  .........Unliste
-00008ce0: 6407 0000 000b 5069 7865 6c66 6564 5461  d.....PixelfedTa
-00008cf0: 6201 0300 0000 1400 4900 6e00 6800 6100  b.......I.n.h.a.
-00008d00: 6c00 7400 7300 7400 7900 7008 0000 0000  l.t.s.t.y.p.....
-00008d10: 0600 0000 0c43 6f6e 7465 6e74 2074 7970  .....Content typ
-00008d20: 6507 0000 000a 5265 6769 6f6e 7354 6162  e.....RegionsTab
-00008d30: 0103 0000 0018 0042 0065 0073 0063 0068  .......B.e.s.c.h
-00008d40: 0072 0065 0069 0062 0075 006e 0067 0800  .r.e.i.b.u.n.g..
-00008d50: 0000 0006 0000 000b 4465 7363 7269 7074  ........Descript
-00008d60: 696f 6e07 0000 000a 5265 6769 6f6e 7354  ion.....RegionsT
-00008d70: 6162 0103 0000 0008 004e 0061 006d 0065  ab.......N.a.m.e
-00008d80: 0800 0000 0006 0000 0004 4e61 6d65 0700  ..........Name..
-00008d90: 0000 0a52 6567 696f 6e73 5461 6201 0300  ...RegionsTab...
-00008da0: 0000 2a00 2600 5400 6500 6300 6800 6e00  ..*.&.T.e.c.h.n.
-00008db0: 6900 7300 6300 6800 6500 2000 4d00 6500  i.s.c.h.e. .M.e.
-00008dc0: 7400 6100 6400 6100 7400 6500 6e08 0000  t.a.d.a.t.e.n...
-00008dd0: 0000 0600 0000 1326 5465 6368 6e69 6361  .......&Technica
-00008de0: 6c20 6d65 7461 6461 7461 0700 0000 0c54  l metadata.....T
-00008df0: 6563 686e 6963 616c 5461 6201 0300 0000  echnicalTab.....
-00008e00: 1400 3300 3500 6d00 6d00 2000 6500 7100  ..3.5.m.m. .e.q.
-00008e10: 7500 6900 7608 0000 0000 0600 0000 0a33  u.i.v..........3
-00008e20: 356d 6d20 6571 7569 7607 0000 000c 5465  5mm equiv.....Te
-00008e30: 6368 6e69 6361 6c54 6162 0103 0000 0066  chnicalTab.....f
-00008e40: 0042 006c 0065 006e 0064 0065 0020 0075  .B.l.e.n.d.e. .u
-00008e50: 006e 0064 0020 0042 0072 0065 006e 006e  .n.d. .B.r.e.n.n
-00008e60: 0077 0065 0069 0074 0065 0020 0061 0075  .w.e.i.t.e. .a.u
-00008e70: 0073 0020 004f 0062 006a 0065 006b 0074  .s. .O.b.j.e.k.t
-00008e80: 0069 0076 0064 0061 0074 0065 006e 0020  .i.v.d.a.t.e.n. 
-00008e90: 00fc 0062 0065 0072 006e 0065 0068 006d  ...b.e.r.n.e.h.m
-00008ea0: 0065 006e 003f 0800 0000 0006 0000 0048  .e.n.?.........H
-00008eb0: 4164 6a75 7374 2069 6d61 6765 2061 7065  Adjust image ape
-00008ec0: 7274 7572 6520 616e 6420 666f 6361 6c20  rture and focal 
-00008ed0: 6c65 6e67 7468 2074 6f20 6167 7265 6520  length to agree 
-00008ee0: 7769 7468 206c 656e 7320 7370 6563 6966  with lens specif
-00008ef0: 6963 6174 696f 6e3f 0700 0000 0c54 6563  ication?.....Tec
-00008f00: 686e 6963 616c 5461 6201 0300 0000 2400  hnicalTab.....$.
-00008f10: 5500 6800 7200 7a00 6500 6900 7400 6500  U.h.r.z.e.i.t.e.
-00008f20: 6e00 2000 6100 6e00 7000 6100 7300 7300  n. .a.n.p.a.s.s.
-00008f30: 6500 6e08 0000 0000 0600 0000 0c41 646a  e.n..........Adj
-00008f40: 7573 7420 7469 6d65 7307 0000 000c 5465  ust times.....Te
-00008f50: 6368 6e69 6361 6c54 6162 0103 0000 000c  chnicalTab......
-00008f60: 0042 006c 0065 006e 0064 0065 0800 0000  .B.l.e.n.d.e....
-00008f70: 0006 0000 0008 4170 6572 7475 7265 0700  ......Aperture..
-00008f80: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
-00008f90: 0300 0000 3400 4200 6c00 6500 6e00 6400  ....4.B.l.e.n.d.
-00008fa0: 6500 2000 6200 6500 6900 2000 6d00 6100  e. .b.e.i. .m.a.
-00008fb0: 7800 2e00 2000 4200 7200 6500 6e00 6e00  x... .B.r.e.n.n.
-00008fc0: 7700 6500 6900 7400 6508 0000 0000 0600  w.e.i.t.e.......
-00008fd0: 0000 1d41 7065 7274 7572 6520 6174 206d  ...Aperture at m
-00008fe0: 6178 2e20 666f 6361 6c20 6c65 6e67 7468  ax. focal length
-00008ff0: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
-00009000: 6201 0300 0000 3400 4200 6c00 6500 6e00  b.....4.B.l.e.n.
-00009010: 6400 6500 2000 6200 6500 6900 2000 6d00  d.e. .b.e.i. .m.
-00009020: 6900 6e00 2e00 2000 4200 7200 6500 6e00  i.n... .B.r.e.n.
-00009030: 6e00 7700 6500 6900 7400 6508 0000 0000  n.w.e.i.t.e.....
-00009040: 0600 0000 1d41 7065 7274 7572 6520 6174  .....Aperture at
-00009050: 206d 696e 2e20 666f 6361 6c20 6c65 6e67   min. focal leng
-00009060: 7468 0700 0000 0c54 6563 686e 6963 616c  th.....Technical
-00009070: 5461 6201 0300 0000 0c00 4b00 6100 6d00  Tab.......K.a.m.
-00009080: 6500 7200 6108 0000 0000 0600 0000 0643  e.r.a..........C
-00009090: 616d 6572 6107 0000 000c 5465 6368 6e69  amera.....Techni
-000090a0: 6361 6c54 6162 0103 0000 0022 0044 0061  calTab.....".D.a
-000090b0: 0074 0075 006d 0020 0075 006e 0064 0020  .t.u.m. .u.n.d. 
-000090c0: 0055 0068 0072 007a 0065 0069 0074 0800  .U.h.r.z.e.i.t..
-000090d0: 0000 0006 0000 000d 4461 7465 2061 6e64  ........Date and
-000090e0: 2074 696d 6507 0000 000c 5465 6368 6e69   time.....Techni
-000090f0: 6361 6c54 6162 0103 0000 001a 0044 0069  calTab.......D.i
-00009100: 0067 0069 0074 0061 006c 0069 0073 0069  .g.i.t.a.l.i.s.i
-00009110: 0065 0072 0074 0800 0000 0006 0000 0009  .e.r.t..........
-00009120: 4469 6769 7469 7365 6407 0000 000c 5465  Digitised.....Te
-00009130: 6368 6e69 6361 6c54 6162 0103 0000 0014  chnicalTab......
-00009140: 0042 0072 0065 006e 006e 0077 0065 0069  .B.r.e.n.n.w.e.i
-00009150: 0074 0065 0800 0000 0006 0000 000c 466f  .t.e..........Fo
-00009160: 6361 6c20 6c65 6e67 7468 0700 0000 0c54  cal length.....T
-00009170: 6563 686e 6963 616c 5461 6201 0300 0000  echnicalTab.....
-00009180: 1800 4c00 6900 6e00 7300 6500 6e00 6d00  ..L.i.n.s.e.n.m.
-00009190: 6f00 6400 6500 6c00 6c08 0000 0000 0600  o.d.e.l.l.......
-000091a0: 0000 0a4c 656e 7320 6d6f 6465 6c07 0000  ...Lens model...
-000091b0: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
-000091c0: 0000 0046 0044 0069 0067 0069 0074 0061  ...F.D.i.g.i.t.a
-000091d0: 006c 0069 0073 0069 0065 0072 0074 0020  .l.i.s.i.e.r.t. 
-000091e0: 0075 006e 0064 0020 0056 0065 0072 00e4  .u.n.d. .V.e.r..
-000091f0: 006e 0064 0065 0072 0074 0020 006b 006f  .n.d.e.r.t. .k.o
-00009200: 0070 0070 0065 006c 006e 0800 0000 0006  .p.p.e.l.n......
-00009210: 0000 001f 4c69 6e6b 2027 6469 6769 7469  ....Link 'digiti
-00009220: 7365 6427 2061 6e64 2027 6d6f 6469 6669  sed' and 'modifi
-00009230: 6564 2707 0000 000c 5465 6368 6e69 6361  ed'.....Technica
-00009240: 6c54 6162 0103 0000 004a 0041 0075 0066  lTab.....J.A.u.f
-00009250: 0067 0065 006e 006f 006d 006d 0065 006e  .g.e.n.o.m.m.e.n
-00009260: 0020 0075 006e 0064 0020 0044 0069 0067  . .u.n.d. .D.i.g
-00009270: 0069 0074 0061 006c 0069 0073 0069 0065  .i.t.a.l.i.s.i.e
-00009280: 0072 0074 0020 006b 006f 0070 0070 0065  .r.t. .k.o.p.p.e
-00009290: 006c 006e 0800 0000 0006 0000 001c 4c69  .l.n..........Li
-000092a0: 6e6b 2027 7461 6b65 6e27 2061 6e64 2027  nk 'taken' and '
-000092b0: 6469 6769 7469 7365 6427 0700 0000 0c54  digitised'.....T
-000092c0: 6563 686e 6963 616c 5461 6201 0300 0000  echnicalTab.....
-000092d0: 1c00 4800 6500 7200 7300 7400 6500 6c00  ..H.e.r.s.t.e.l.
-000092e0: 6c00 6500 7200 6e00 6100 6d00 6508 0000  l.e.r.n.a.m.e...
-000092f0: 0000 0600 0000 0c4d 616b 6572 2773 206e  .......Maker's n
-00009300: 616d 6507 0000 000c 5465 6368 6e69 6361  ame.....Technica
-00009310: 6c54 6162 0103 0000 0016 004d 0061 0078  lTab.......M.a.x
-00009320: 002e 0020 0042 006c 0065 006e 0064 0065  ... .B.l.e.n.d.e
-00009330: 0800 0000 0006 0000 000c 4d61 7820 6170  ..........Max ap
-00009340: 6572 7475 7265 0700 0000 0c54 6563 686e  erture.....Techn
-00009350: 6963 616c 5461 6201 0300 0000 2600 4d00  icalTab.....&.M.
-00009360: 6100 7800 6900 6d00 6100 6c00 6500 2000  a.x.i.m.a.l.e. .
-00009370: 4200 7200 6500 6e00 6e00 7700 6500 6900  B.r.e.n.n.w.e.i.
-00009380: 7400 6508 0000 0000 0600 0000 144d 6178  t.e..........Max
-00009390: 696d 756d 2066 6f63 616c 206c 656e 6774  imum focal lengt
-000093a0: 6807 0000 000c 5465 6368 6e69 6361 6c54  h.....TechnicalT
-000093b0: 6162 0103 0000 0026 004d 0069 006e 0069  ab.....&.M.i.n.i
-000093c0: 006d 0061 006c 0065 0020 0042 0072 0065  .m.a.l.e. .B.r.e
-000093d0: 006e 006e 0077 0065 0069 0074 0065 0800  .n.n.w.e.i.t.e..
-000093e0: 0000 0006 0000 0014 4d69 6e69 6d75 6d20  ........Minimum 
-000093f0: 666f 6361 6c20 6c65 6e67 7468 0700 0000  focal length....
-00009400: 0c54 6563 686e 6963 616c 5461 6201 0300  .TechnicalTab...
-00009410: 0000 1400 4d00 6f00 6400 6500 6c00 6c00  ....M.o.d.e.l.l.
-00009420: 6e00 6100 6d00 6508 0000 0000 0600 0000  n.a.m.e.........
-00009430: 0a4d 6f64 656c 206e 616d 6507 0000 000c  .Model name.....
-00009440: 5465 6368 6e69 6361 6c54 6162 0103 0000  TechnicalTab....
-00009450: 0012 0056 0065 0072 00e4 006e 0064 0065  ...V.e.r...n.d.e
-00009460: 0072 0074 0800 0000 0006 0000 0008 4d6f  .r.t..........Mo
-00009470: 6469 6669 6564 0700 0000 0c54 6563 686e  dified.....Techn
-00009480: 6963 616c 5461 6201 0300 0000 1600 4100  icalTab.......A.
-00009490: 7500 7300 7200 6900 6300 6800 7400 7500  u.s.r.i.c.h.t.u.
-000094a0: 6e00 6708 0000 0000 0600 0000 0b4f 7269  n.g..........Ori
-000094b0: 656e 7461 7469 6f6e 0700 0000 0c54 6563  entation.....Tec
-000094c0: 686e 6963 616c 5461 6201 0300 0000 0c00  hnicalTab.......
-000094d0: 4100 6e00 6400 6500 7200 6508 0000 0000  A.n.d.e.r.e.....
-000094e0: 0600 0000 054f 7468 6572 0700 0000 0c54  .....Other.....T
-000094f0: 6563 686e 6963 616c 5461 6201 0300 0000  echnicalTab.....
-00009500: 3400 5000 6800 6f00 7400 6900 6e00 6900  4.P.h.o.t.i.n.i.
-00009510: 3a00 2000 4b00 6100 6d00 6500 7200 6100  :. .K.a.m.e.r.a.
-00009520: 2000 6400 6500 6600 6900 6e00 6900 6500   .d.e.f.i.n.i.e.
-00009530: 7200 6500 6e08 0000 0000 0600 0000 1650  r.e.n..........P
-00009540: 686f 7469 6e69 3a20 6465 6669 6e65 2063  hotini: define c
-00009550: 616d 6572 6107 0000 000c 5465 6368 6e69  amera.....Techni
-00009560: 6361 6c54 6162 0103 0000 0032 0050 0068  calTab.....2.P.h
-00009570: 006f 0074 0069 006e 0069 003a 0020 004c  .o.t.i.n.i.:. .L
-00009580: 0069 006e 0073 0065 0020 0064 0065 0066  .i.n.s.e. .d.e.f
-00009590: 0069 006e 0069 0065 0072 0065 006e 0800  .i.n.i.e.r.e.n..
-000095a0: 0000 0006 0000 0014 5068 6f74 696e 693a  ........Photini:
-000095b0: 2064 6566 696e 6520 6c65 6e73 0700 0000   define lens....
-000095c0: 0c54 6563 686e 6963 616c 5461 6201 0300  .TechnicalTab...
-000095d0: 0000 1600 4700 6500 6e00 6100 7500 6900  ....G.e.n.a.u.i.
-000095e0: 6700 6b00 6500 6900 7408 0000 0000 0600  g.k.e.i.t.......
-000095f0: 0000 0950 7265 6369 7369 6f6e 0700 0000  ...Precision....
-00009600: 0c54 6563 686e 6963 616c 5461 6201 0300  .TechnicalTab...
-00009610: 0000 1800 5300 6500 7200 6900 6500 6e00  ....S.e.r.i.e.n.
-00009620: 6e00 7500 6d00 6d00 6500 7208 0000 0000  n.u.m.m.e.r.....
-00009630: 0600 0000 0d53 6572 6961 6c20 6e75 6d62  .....Serial numb
-00009640: 6572 0700 0000 0c54 6563 686e 6963 616c  er.....Technical
-00009650: 5461 6201 0300 0000 1600 4100 7500 6600  Tab.......A.u.f.
-00009660: 6700 6500 6e00 6f00 6d00 6d00 6500 6e08  g.e.n.o.m.m.e.n.
-00009670: 0000 0000 0600 0000 0554 616b 656e 0700  .........Taken..
-00009680: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
-00009690: 0300 0000 4600 4200 6c00 6500 6e00 6400  ....F.B.l.e.n.d.
-000096a0: 6500 2000 7500 6e00 6400 2000 4200 7200  e. .u.n.d. .B.r.
-000096b0: 6500 6e00 6e00 7700 6500 6900 7400 6500  e.n.n.w.e.i.t.e.
-000096c0: 2000 6100 6b00 7400 7500 6100 6c00 6900   .a.k.t.u.a.l.i.
-000096d0: 7300 6900 6500 7200 6500 6e08 0000 0000  s.i.e.r.e.n.....
-000096e0: 0600 0000 1e55 7064 6174 6520 6170 6572  .....Update aper
-000096f0: 7475 7265 2026 2066 6f63 616c 206c 656e  ture & focal len
-00009700: 6774 6807 0000 000c 5465 6368 6e69 6361  gth.....Technica
-00009710: 6c54 6162 0103 0000 0006 006d 0061 0078  lTab.......m.a.x
-00009720: 0800 0000 0006 0000 0003 6d61 7807 0000  ..........max...
-00009730: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
-00009740: 0000 0006 006d 0069 006e 0800 0000 0006  .....m.i.n......
-00009750: 0000 0003 6d69 6e07 0000 000c 5465 6368  ....min.....Tech
-00009760: 6e69 6361 6c54 6162 0103 0000 000c 006e  nicalTab.......n
-00009770: 006f 0072 006d 0061 006c 0800 0000 0006  .o.r.m.a.l......
-00009780: 0000 0006 6e6f 726d 616c 0700 0000 0c54  ....normal.....T
-00009790: 6563 686e 6963 616c 5461 6201 0300 0000  echnicalTab.....
-000097a0: 2a00 6c00 6900 6e00 6b00 7300 2d00 7200  *.l.i.n.k.s.-.r.
-000097b0: 6500 6300 6800 7400 7300 2000 7300 7000  e.c.h.t.s. .s.p.
-000097c0: 6900 6500 6700 6500 6c00 6e08 0000 0000  i.e.g.e.l.n.....
-000097d0: 0600 0000 1572 6566 6c65 6374 206c 6566  .....reflect lef
-000097e0: 7420 746f 2072 6967 6874 0700 0000 0c54  t to right.....T
-000097f0: 6563 686e 6963 616c 5461 6201 0300 0000  echnicalTab.....
-00009800: 4000 6c00 6900 6e00 6b00 7300 2000 6f00  @.l.i.n.k.s. .o.
-00009810: 6200 6500 6e00 2d00 7200 6500 6300 6800  b.e.n.-.r.e.c.h.
-00009820: 7400 7300 2000 7500 6e00 7400 6500 6e00  t.s. .u.n.t.e.n.
-00009830: 2000 7300 7000 6900 6500 6700 6500 6c00   .s.p.i.e.g.e.l.
-00009840: 6e08 0000 0000 0600 0000 2072 6566 6c65  n......... refle
-00009850: 6374 2074 6f70 206c 6566 7420 746f 2062  ct top left to b
-00009860: 6f74 746f 6d20 7269 6768 7407 0000 000c  ottom right.....
-00009870: 5465 6368 6e69 6361 6c54 6162 0103 0000  TechnicalTab....
-00009880: 0040 0072 0065 0063 0068 0074 0073 0020  .@.r.e.c.h.t.s. 
-00009890: 006f 0062 0065 006e 002d 006c 0069 006e  .o.b.e.n.-.l.i.n
-000098a0: 006b 0073 0020 0075 006e 0074 0065 006e  .k.s. .u.n.t.e.n
-000098b0: 0020 0073 0070 0069 0065 0067 0065 006c  . .s.p.i.e.g.e.l
-000098c0: 006e 0800 0000 0006 0000 0020 7265 666c  .n......... refl
-000098d0: 6563 7420 746f 7020 7269 6768 7420 746f  ect top right to
-000098e0: 2062 6f74 746f 6d20 6c65 6674 0700 0000   bottom left....
+000048a0: 0300 0000 2600 4200 6900 6c00 6400 6500  ....&.B.i.l.d.e.
+000048b0: 7200 2000 2600 4900 6d00 7000 6f00 7200  r. .&.I.m.p.o.r.
+000048c0: 7400 6900 6500 7200 6500 6e08 0000 0000  t.i.e.r.e.n.....
+000048d0: 0600 0000 0e26 496d 706f 7274 2070 686f  .....&Import pho
+000048e0: 746f 7307 0000 000b 496d 706f 7274 6572  tos.....Importer
+000048f0: 5461 6201 0300 0000 2600 3c00 4f00 7200  Tab.....&.<.O.r.
+00004900: 6400 6e00 6500 7200 2000 6800 6900 6e00  d.n.e.r. .h.i.n.
+00004910: 7a00 7500 6600 fc00 6700 6500 6e00 3e08  z.u.f...g.e.n.>.
+00004920: 0000 0000 0600 0000 0e3c 6164 6420 6120  .........<add a 
+00004930: 666f 6c64 6572 3e07 0000 000b 496d 706f  folder>.....Impo
+00004940: 7274 6572 5461 6201 0300 0000 2400 3c00  rterTab.....$.<.
+00004950: 5100 7500 6500 6c00 6c00 6500 2000 6100  Q.u.e.l.l.e. .a.
+00004960: 7500 7300 7700 e400 6800 6c00 6500 6e00  u.s.w...h.l.e.n.
+00004970: 3e08 0000 0000 0600 0000 0f3c 7365 6c65  >..........<sele
+00004980: 6374 2073 6f75 7263 653e 0700 0000 0b49  ct source>.....I
+00004990: 6d70 6f72 7465 7254 6162 0103 0000 006c  mporterTab.....l
+000049a0: 0057 0065 006e 006e 0020 0053 0069 0065  .W.e.n.n. .S.i.e
+000049b0: 0020 006a 0065 0074 007a 0074 0020 0073  . .j.e.t.z.t. .s
+000049c0: 0063 0068 006c 0069 0065 00df 0065 006e  .c.h.l.i.e...e.n
+000049d0: 002c 0020 0077 0069 0072 0064 0020 0064  .,. .w.i.r.d. .d
+000049e0: 0065 0072 0020 0049 006d 0070 006f 0072  .e.r. .I.m.p.o.r
+000049f0: 0074 0020 0061 0062 0067 0065 0062 0072  .t. .a.b.g.e.b.r
+00004a00: 006f 0063 0068 0065 006e 002e 0800 0000  .o.c.h.e.n......
+00004a10: 0006 0000 0026 436c 6f73 696e 6720 6e6f  .....&Closing no
+00004a20: 7720 7769 6c6c 2074 6572 6d69 6e61 7465  w will terminate
+00004a30: 2074 6865 2069 6d70 6f72 742e 0700 0000   the import.....
+00004a40: 0b49 6d70 6f72 7465 7254 6162 0103 0000  .ImporterTab....
+00004a50: 001c 0046 006f 0074 006f 0073 0020 006b  ...F.o.t.o.s. .k
+00004a60: 006f 0070 0069 0065 0072 0065 006e 0800  .o.p.i.e.r.e.n..
+00004a70: 0000 0006 0000 000b 436f 7079 2070 686f  ........Copy pho
+00004a80: 746f 7307 0000 000b 496d 706f 7274 6572  tos.....Importer
+00004a90: 5461 6201 0300 0000 6600 4900 6d00 7000  Tab.....f.I.m.p.
+00004aa0: 6f00 7200 7400 6900 6500 7200 6500 6e00  o.r.t.i.e.r.e.n.
+00004ab0: 2000 7600 6f00 6e00 2000 4600 6f00 7400   .v.o.n. .F.o.t.
+00004ac0: 6f00 7300 2000 6900 7300 7400 2000 6e00  o.s. .i.s.t. .n.
+00004ad0: 6f00 6300 6800 2000 6e00 6900 6300 6800  o.c.h. .n.i.c.h.
+00004ae0: 7400 2000 6100 6200 6700 6500 7300 6300  t. .a.b.g.e.s.c.
+00004af0: 6800 6c00 6f00 7300 7300 6500 6e00 2e08  h.l.o.s.s.e.n...
+00004b00: 0000 0000 0600 0000 2249 6d70 6f72 7469  ........"Importi
+00004b10: 6e67 2070 686f 746f 7320 6861 7320 6e6f  ng photos has no
+00004b20: 7420 6669 6e69 7368 6564 2e07 0000 000b  t finished......
+00004b30: 496d 706f 7274 6572 5461 6201 0300 0000  ImporterTab.....
+00004b40: 2400 5000 6800 6f00 7400 6f00 7300 2000  $.P.h.o.t.o.s. .
+00004b50: 7600 6500 7200 7300 6300 6800 6900 6500  v.e.r.s.c.h.i.e.
+00004b60: 6200 6500 6e08 0000 0000 0600 0000 0b4d  b.e.n..........M
+00004b70: 6f76 6520 7068 6f74 6f73 0700 0000 0b49  ove photos.....I
+00004b80: 6d70 6f72 7465 7254 6162 0103 0000 002a  mporterTab.....*
+00004b90: 0050 0068 006f 0074 0069 006e 0069 003a  .P.h.o.t.i.n.i.:
+00004ba0: 0020 0049 006d 0070 006f 0072 0074 0020  . .I.m.p.o.r.t. 
+00004bb0: 006c 00e4 0075 0066 0074 0800 0000 0006  .l...u.f.t......
+00004bc0: 0000 001b 5068 6f74 696e 693a 2069 6d70  ....Photini: imp
+00004bd0: 6f72 7420 696e 2070 726f 6772 6573 7307  ort in progress.
+00004be0: 0000 000b 496d 706f 7274 6572 5461 6201  ....ImporterTab.
+00004bf0: 0300 0000 3200 2200 7b00 7300 6f00 7500  ....2.".{.s.o.u.
+00004c00: 7200 6300 6500 5f00 6e00 6100 6d00 6500  r.c.e._.n.a.m.e.
+00004c10: 7d00 2200 2000 6500 6e00 7400 6600 6500  }.". .e.n.t.f.e.
+00004c20: 7200 6e00 6500 6e08 0000 0000 0600 0000  r.n.e.n.........
+00004c30: 1652 656d 6f76 6520 227b 736f 7572 6365  .Remove "{source
+00004c40: 5f6e 616d 657d 2207 0000 000b 496d 706f  _name}".....Impo
+00004c50: 7274 6572 5461 6201 0300 0000 1c00 4100  rterTab.......A.
+00004c60: 6c00 6c00 6500 2000 6100 7500 7300 7700  l.l.e. .a.u.s.w.
+00004c70: e400 6800 6c00 6500 6e08 0000 0000 0600  ..h.l.e.n.......
+00004c80: 0000 0a53 656c 6563 7420 616c 6c07 0000  ...Select all...
+00004c90: 000b 496d 706f 7274 6572 5461 6201 0300  ..ImporterTab...
+00004ca0: 0000 1a00 4e00 6500 7500 2000 6100 7500  ....N.e.u. .a.u.
+00004cb0: 7300 7700 e400 6800 6c00 6500 6e08 0000  s.w...h.l.e.n...
+00004cc0: 0000 0600 0000 0a53 656c 6563 7420 6e65  .......Select ne
+00004cd0: 7707 0000 000b 496d 706f 7274 6572 5461  w.....ImporterTa
+00004ce0: 6201 0300 0000 2a00 5100 7500 6500 6c00  b.....*.Q.u.e.l.
+00004cf0: 6c00 6f00 7200 6400 6e00 6500 7200 2000  l.o.r.d.n.e.r. .
+00004d00: 6100 7500 7300 7700 e400 6800 6c00 6500  a.u.s.w...h.l.e.
+00004d10: 6e08 0000 0000 0600 0000 1253 656c 6563  n..........Selec
+00004d20: 7420 726f 6f74 2066 6f6c 6465 7207 0000  t root folder...
+00004d30: 000b 496d 706f 7274 6572 5461 6201 0300  ..ImporterTab...
+00004d40: 0000 0c00 5100 7500 6500 6c00 6c00 6508  ....Q.u.e.l.l.e.
+00004d50: 0000 0000 0600 0000 0653 6f75 7263 6507  .........Source.
+00004d60: 0000 000b 496d 706f 7274 6572 5461 6201  ....ImporterTab.
+00004d70: 0300 0000 1a00 5300 7400 6f00 7000 2000  ......S.t.o.p. .
+00004d80: 4b00 6f00 7000 6900 6500 7200 6500 6e08  K.o.p.i.e.r.e.n.
+00004d90: 0000 0000 0600 0000 0953 746f 7020 636f  .........Stop co
+00004da0: 7079 0700 0000 0b49 6d70 6f72 7465 7254  py.....ImporterT
+00004db0: 6162 0103 0000 0020 0053 0074 006f 0070  ab..... .S.t.o.p
+00004dc0: 0020 0056 0065 0072 0073 0063 0068 0069  . .V.e.r.s.c.h.i
+00004dd0: 0065 0062 0065 006e 0800 0000 0006 0000  .e.b.e.n........
+00004de0: 0009 5374 6f70 206d 6f76 6507 0000 000b  ..Stop move.....
+00004df0: 496d 706f 7274 6572 5461 6201 0300 0000  ImporterTab.....
+00004e00: 1400 5a00 6900 6500 6c00 6600 6f00 7200  ..Z.i.e.l.f.o.r.
+00004e10: 6d00 6100 7408 0000 0000 0600 0000 0d54  m.a.t..........T
+00004e20: 6172 6765 7420 666f 726d 6174 0700 0000  arget format....
+00004e30: 0b49 6d70 6f72 7465 7254 6162 0103 0000  .ImporterTab....
+00004e40: 002a 004b 0061 006d 0065 0072 0061 003a  .*.K.a.m.e.r.a.:
+00004e50: 0020 007b 0063 0061 006d 0065 0072 0061  . .{.c.a.m.e.r.a
+00004e60: 005f 006e 0061 006d 0065 007d 0800 0000  ._.n.a.m.e.}....
+00004e70: 0006 0000 0015 6361 6d65 7261 3a20 7b63  ......camera: {c
+00004e80: 616d 6572 615f 6e61 6d65 7d07 0000 000b  amera_name}.....
+00004e90: 496d 706f 7274 6572 5461 6201 0300 0000  ImporterTab.....
+00004ea0: 2a00 4f00 7200 6400 6e00 6500 7200 3a00  *.O.r.d.n.e.r.:.
+00004eb0: 2000 7b00 6600 6f00 6c00 6400 6500 7200   .{.f.o.l.d.e.r.
+00004ec0: 5f00 6e00 6100 6d00 6500 7d08 0000 0000  _.n.a.m.e.}.....
+00004ed0: 0600 0000 1566 6f6c 6465 723a 207b 666f  .....folder: {fo
+00004ee0: 6c64 6572 5f6e 616d 657d 0700 0000 0b49  lder_name}.....I
+00004ef0: 6d70 6f72 7465 7254 6162 0103 0000 0012  mporterTab......
+00004f00: 004e 0065 0075 0020 006c 0061 0064 0065  .N.e.u. .l.a.d.e
+00004f10: 006e 0800 0000 0006 0000 0007 7265 6672  .n..........refr
+00004f20: 6573 6807 0000 000b 496d 706f 7274 6572  esh.....Importer
+00004f30: 5461 6201 0300 0000 2600 2600 4900 7000  Tab.....&.&.I.p.
+00004f40: 6500 7200 6e00 6900 7400 7900 2d00 4800  e.r.n.i.t.y.-.H.
+00004f50: 6f00 6300 6800 6c00 6100 6400 6500 6e08  o.c.h.l.a.d.e.n.
+00004f60: 0000 0000 0600 0000 1026 4970 6572 6e69  .........&Iperni
+00004f70: 7479 2075 706c 6f61 6407 0000 000b 4970  ty upload.....Ip
+00004f80: 6572 6e69 7479 5461 6201 0300 0000 1a00  ernityTab.......
+00004f90: 4e00 6100 6d00 6500 6e00 7300 6e00 6500  N.a.m.e.n.s.n.e.
+00004fa0: 6e00 6e00 7500 6e00 6708 0000 0000 0600  n.n.u.n.g.......
+00004fb0: 0000 0b41 7474 7269 6275 7469 6f6e 0700  ...Attribution..
+00004fc0: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
+00004fd0: 0000 003e 004e 0061 006d 0065 006e 0073  ...>.N.a.m.e.n.s
+00004fe0: 006e 0065 006e 006e 0075 006e 0067 0020  .n.e.n.n.u.n.g. 
+00004ff0: 002b 0020 006b 0065 0069 006e 0065 0020  .+. .k.e.i.n.e. 
+00005000: 0041 0062 006c 0065 0069 0074 0075 006e  .A.b.l.e.i.t.u.n
+00005010: 0067 0800 0000 0006 0000 001b 4174 7472  .g..........Attr
+00005020: 6962 7574 696f 6e20 2b20 6e6f 2064 6572  ibution + no der
+00005030: 6976 6174 6976 6507 0000 000b 4970 6572  ivative.....Iper
+00005040: 6e69 7479 5461 6201 0300 0000 4200 4e00  nityTab.....B.N.
+00005050: 6100 6d00 6500 6e00 7300 6e00 6500 6e00  a.m.e.n.s.n.e.n.
+00005060: 6e00 7500 6e00 6700 2000 2b00 2000 6e00  n.u.n.g. .+. .n.
+00005070: 6900 6300 6800 7400 2000 6b00 6f00 6d00  i.c.h.t. .k.o.m.
+00005080: 6d00 6500 7200 7a00 6900 6500 6c00 6c08  m.e.r.z.i.e.l.l.
+00005090: 0000 0000 0600 0000 1c41 7474 7269 6275  .........Attribu
+000050a0: 7469 6f6e 202b 206e 6f6e 2063 6f6d 6d65  tion + non comme
+000050b0: 7263 6961 6c07 0000 000b 4970 6572 6e69  rcial.....Iperni
+000050c0: 7479 5461 6201 0300 0000 6600 4e00 6100  tyTab.....f.N.a.
+000050d0: 6d00 6500 6e00 7300 6e00 6500 6e00 6e00  m.e.n.s.n.e.n.n.
+000050e0: 7500 6e00 6700 2000 2b00 2000 6e00 6900  u.n.g. .+. .n.i.
+000050f0: 6300 6800 7400 2000 6b00 6f00 6d00 6d00  c.h.t. .k.o.m.m.
+00005100: 6500 7200 7a00 6900 6500 6c00 6c00 2000  e.r.z.i.e.l.l. .
+00005110: 2b00 2000 6b00 6500 6900 6e00 6500 2000  +. .k.e.i.n.e. .
+00005120: 4100 6200 6c00 6500 6900 7400 7500 6e00  A.b.l.e.i.t.u.n.
+00005130: 6708 0000 0000 0600 0000 2c41 7474 7269  g.........,Attri
+00005140: 6275 7469 6f6e 202b 206e 6f6e 2063 6f6d  bution + non com
+00005150: 6d65 7263 6961 6c20 2b20 6e6f 2064 6572  mercial + no der
+00005160: 6976 6174 6976 6507 0000 000b 4970 6572  ivative.....Iper
+00005170: 6e69 7479 5461 6201 0300 0000 7a00 4e00  nityTab.....z.N.
+00005180: 6100 6d00 6500 6e00 7300 6e00 6500 6e00  a.m.e.n.s.n.e.n.
+00005190: 6e00 7500 6e00 6700 2000 2b00 2000 6e00  n.u.n.g. .+. .n.
+000051a0: 6900 6300 6800 7400 2000 6b00 6f00 6d00  i.c.h.t. .k.o.m.
+000051b0: 6d00 6500 7200 7a00 6900 6500 6c00 6c00  m.e.r.z.i.e.l.l.
+000051c0: 2000 2b00 2000 6700 6c00 6500 6900 6300   .+. .g.l.e.i.c.
+000051d0: 6800 6200 6500 7200 6500 6300 6800 7400  h.b.e.r.e.c.h.t.
+000051e0: 6900 6700 7400 6500 2000 4e00 7500 7400  i.g.t.e. .N.u.t.
+000051f0: 7a00 7500 6e00 6708 0000 0000 0600 0000  z.u.n.g.........
+00005200: 2a41 7474 7269 6275 7469 6f6e 202b 206e  *Attribution + n
+00005210: 6f6e 2063 6f6d 6d65 7263 6961 6c20 2b20  on commercial + 
+00005220: 7368 6172 6520 616c 696b 6507 0000 000b  share alike.....
+00005230: 4970 6572 6e69 7479 5461 6201 0300 0000  IpernityTab.....
+00005240: 5200 4e00 6100 6d00 6500 6e00 7300 6e00  R.N.a.m.e.n.s.n.
+00005250: 6500 6e00 6e00 7500 6e00 6700 2000 2b00  e.n.n.u.n.g. .+.
+00005260: 2000 6700 6c00 6500 6900 6300 6800 6200   .g.l.e.i.c.h.b.
+00005270: 6500 7200 6500 6300 6800 7400 6900 6700  e.r.e.c.h.t.i.g.
+00005280: 7400 6500 2000 4e00 7500 7400 7a00 7500  t.e. .N.u.t.z.u.
+00005290: 6e00 6708 0000 0000 0600 0000 1941 7474  n.g..........Att
+000052a0: 7269 6275 7469 6f6e 202b 2073 6861 7265  ribution + share
+000052b0: 2061 6c69 6b65 0700 0000 0b49 7065 726e   alike.....Ipern
+000052c0: 6974 7954 6162 0103 0000 0034 0041 006c  ityTab.....4.A.l
+000052d0: 0062 0075 006d 006d 0069 0074 0067 006c  .b.u.m.m.i.t.g.l
+000052e0: 0069 0065 0064 0073 0063 0068 0061 0066  .i.e.d.s.c.h.a.f
+000052f0: 0074 0020 00e4 006e 0064 0065 0072 006e  .t. ...n.d.e.r.n
+00005300: 0800 0000 0006 0000 0017 4368 616e 6765  ..........Change
+00005310: 2061 6c62 756d 206d 656d 6265 7273 6869   album membershi
+00005320: 7007 0000 000b 4970 6572 6e69 7479 5461  p.....IpernityTa
+00005330: 6201 0300 0000 1a00 4c00 6900 7a00 6500  b.......L.i.z.e.
+00005340: 6e00 7a00 2000 e400 6e00 6400 6500 7200  n.z. ...n.d.e.r.
+00005350: 6e08 0000 0000 0600 0000 1243 6861 6e67  n..........Chang
+00005360: 6520 7468 6520 6c69 6365 6e63 6507 0000  e the licence...
+00005370: 000b 4970 6572 6e69 7479 5461 6201 0300  ..IpernityTab...
+00005380: 0000 3000 c400 6e00 6400 6500 7200 6e00  ..0...n.d.e.r.n.
+00005390: 2000 7700 6500 7200 2000 6500 7300 2000   .w.e.r. .e.s. .
+000053a0: 7300 6500 6800 6500 6e00 2000 6b00 6100  s.e.h.e.n. .k.a.
+000053b0: 6e00 6e08 0000 0000 0600 0000 1543 6861  n.n..........Cha
+000053c0: 6e67 6520 7768 6f20 6361 6e20 7365 6520  nge who can see 
+000053d0: 6974 0700 0000 0b49 7065 726e 6974 7954  it.....IpernityT
+000053e0: 6162 0103 0000 0010 004b 006f 006e 0074  ab.......K.o.n.t
+000053f0: 0061 006b 0074 0065 0800 0000 0006 0000  .a.k.t.e........
+00005400: 0008 436f 6e74 6163 7473 0700 0000 0b49  ..Contacts.....I
+00005410: 7065 726e 6974 7954 6162 0103 0000 004c  pernityTab.....L
+00005420: 0055 0072 0068 0065 0062 0065 0072 0072  .U.r.h.e.b.e.r.r
+00005430: 0065 0063 0068 0074 0020 0028 0061 006c  .e.c.h.t. .(.a.l
+00005440: 006c 0065 0020 0052 0065 0063 0068 0074  .l.e. .R.e.c.h.t
+00005450: 0065 0020 0076 006f 0072 0062 0065 0068  .e. .v.o.r.b.e.h
+00005460: 0061 006c 0074 0065 006e 0029 0800 0000  .a.l.t.e.n.)....
+00005470: 0006 0000 001f 436f 7079 7269 6768 7420  ......Copyright 
+00005480: 2861 6c6c 2072 6967 6874 7320 7265 7365  (all rights rese
+00005490: 7276 6564 2907 0000 000b 4970 6572 6e69  rved).....Iperni
+000054a0: 7479 5461 6201 0300 0000 1800 4200 6500  tyTab.......B.e.
+000054b0: 7300 6300 6800 7200 6500 6900 6200 7500  s.c.h.r.e.i.b.u.
+000054c0: 6e00 6708 0000 0000 0600 0000 0b44 6573  n.g..........Des
+000054d0: 6372 6970 7469 6f6e 0700 0000 0b49 7065  cription.....Ipe
+000054e0: 726e 6974 7954 6162 0103 0000 0008 0041  rnityTab.......A
+000054f0: 006c 006c 0065 0800 0000 0006 0000 0008  .l.l.e..........
+00005500: 4576 6572 796f 6e65 0700 0000 0b49 7065  Everyone.....Ipe
+00005510: 726e 6974 7954 6162 0103 0000 0022 0041  rnityTab.....".A
+00005520: 006c 006c 0065 0020 0028 00f6 0066 0066  .l.l.e. .(...f.f
+00005530: 0065 006e 0074 006c 0069 0063 0068 0029  .e.n.t.l.i.c.h.)
+00005540: 0800 0000 0006 0000 0011 4576 6572 796f  ..........Everyo
+00005550: 6e65 2028 7075 626c 6963 2907 0000 000b  ne (public).....
+00005560: 4970 6572 6e69 7479 5461 6201 0300 0000  IpernityTab.....
+00005570: 0e00 4600 6100 6d00 6900 6c00 6900 6508  ..F.a.m.i.l.i.e.
+00005580: 0000 0000 0600 0000 0646 616d 696c 7907  .........Family.
+00005590: 0000 000b 4970 6572 6e69 7479 5461 6201  ....IpernityTab.
+000055a0: 0300 0000 2600 4600 6100 6d00 6900 6c00  ....&.F.a.m.i.l.
+000055b0: 6900 6500 2000 7500 6e00 6400 2000 4600  i.e. .u.n.d. .F.
+000055c0: 7200 6500 7500 6e00 6400 6508 0000 0000  r.e.u.n.d.e.....
+000055d0: 0600 0000 1046 616d 696c 7920 2620 6672  .....Family & fr
+000055e0: 6965 6e64 7307 0000 000b 4970 6572 6e69  iends.....Iperni
+000055f0: 7479 5461 6201 0300 0000 7000 4600 7200  tyTab.....p.F.r.
+00005600: 6500 6900 6500 2000 5600 6500 7200 7700  e.i.e. .V.e.r.w.
+00005610: 6500 6e00 6400 7500 6e00 6700 2000 2800  e.n.d.u.n.g. .(.
+00005620: 5500 7200 6800 6500 6200 6500 7200 7200  U.r.h.e.b.e.r.r.
+00005630: 6500 6300 6800 7400 2000 6100 6200 6700  e.c.h.t. .a.b.g.
+00005640: 6500 7400 7200 6500 7400 6500 6e00 2c00  e.t.r.e.t.e.n.,.
+00005650: 2000 6b00 6500 6900 6e00 6500 2000 4c00   .k.e.i.n.e. .L.
+00005660: 6900 7a00 6500 6e00 7a00 2908 0000 0000  i.z.e.n.z.).....
+00005670: 0600 0000 2c46 7265 6520 7573 6520 2863  ....,Free use (c
+00005680: 6f70 7972 6967 6874 2073 7572 7265 6e64  opyright surrend
+00005690: 6572 6564 2c20 6e6f 206c 6963 656e 6365  ered, no licence
+000056a0: 2907 0000 000b 4970 6572 6e69 7479 5461  ).....IpernityTa
+000056b0: 6201 0300 0000 0e00 4600 7200 6500 7500  b.......F.r.e.u.
+000056c0: 6e00 6400 6508 0000 0000 0600 0000 0746  n.d.e..........F
+000056d0: 7269 656e 6473 0700 0000 0b49 7065 726e  riends.....Ipern
+000056e0: 6974 7954 6162 0103 0000 0010 0049 0070  ityTab.......I.p
+000056f0: 0065 0072 006e 0069 0074 0079 0800 0000  .e.r.n.i.t.y....
+00005700: 0006 0000 0008 4970 6572 6e69 7479 0700  ......Ipernity..
+00005710: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
+00005720: 0000 000c 004c 0069 007a 0065 006e 007a  .....L.i.z.e.n.z
+00005730: 0800 0000 0006 0000 0007 4c69 6365 6e63  ..........Licenc
+00005740: 6507 0000 000b 4970 6572 6e69 7479 5461  e.....IpernityTa
+00005750: 6201 0300 0000 1600 4e00 6500 7500 6500  b.......N.e.u.e.
+00005760: 7300 2000 4100 6c00 6200 7500 6d08 0000  s. .A.l.b.u.m...
+00005770: 0000 0600 0000 094e 6577 2061 6c62 756d  .......New album
+00005780: 0700 0000 0b49 7065 726e 6974 7954 6162  .....IpernityTab
+00005790: 0103 0000 001c 004e 0075 0072 0020 0069  .......N.u.r. .i
+000057a0: 0063 0068 0020 0073 0065 006c 0062 0073  .c.h. .s.e.l.b.s
+000057b0: 0074 0800 0000 0006 0000 0008 4f6e 6c79  .t..........Only
+000057c0: 2079 6f75 0700 0000 0b49 7065 726e 6974   you.....Ipernit
+000057d0: 7954 6162 0103 0000 0020 004e 0075 0072  yTab..... .N.u.r
+000057e0: 0020 0053 0069 0065 0020 0028 0070 0072  . .S.i.e. .(.p.r
+000057f0: 0069 0076 0061 0074 0029 0800 0000 0006  .i.v.a.t.)......
+00005800: 0000 0012 4f6e 6c79 2079 6f75 2028 7072  ....Only you (pr
+00005810: 6976 6174 6529 0700 0000 0b49 7065 726e  ivate).....Ipern
+00005820: 6974 7954 6162 0103 0000 0024 004d 0065  ityTab.....$.M.e
+00005830: 0074 0061 0064 0061 0074 0065 006e 0020  .t.a.d.a.t.e.n. 
+00005840: 0065 0072 0073 0065 0074 007a 0065 006e  .e.r.s.e.t.z.e.n
+00005850: 0800 0000 0006 0000 0010 5265 706c 6163  ..........Replac
+00005860: 6520 6d65 7461 6461 7461 0700 0000 0b49  e metadata.....I
+00005870: 7065 726e 6974 7954 6162 0103 0000 001e  pernityTab......
+00005880: 0053 0079 006e 0063 0068 0072 006f 006e  .S.y.n.c.h.r.o.n
+00005890: 0069 0073 0069 0065 0072 0065 006e 0800  .i.s.i.e.r.e.n..
+000058a0: 0000 0006 0000 000b 5379 6e63 6872 6f6e  ........Synchron
+000058b0: 6973 6507 0000 000b 4970 6572 6e69 7479  ise.....Ipernity
+000058c0: 5461 6201 0300 0000 0a00 5400 6900 7400  Tab.......T.i.t.
+000058d0: 6500 6c08 0000 0000 0600 0000 0554 6974  e.l..........Tit
+000058e0: 6c65 0700 0000 0b49 7065 726e 6974 7954  le.....IpernityT
+000058f0: 6162 0103 0000 003e 0057 0065 0072 0020  ab.....>.W.e.r. 
+00005900: 0064 0061 0072 0066 0020 0064 0061 0073  .d.a.r.f. .d.a.s
+00005910: 0020 0041 006c 0062 0075 006d 0020 006b  . .A.l.b.u.m. .k
+00005920: 006f 006d 006d 0065 006e 0074 0069 0065  .o.m.m.e.n.t.i.e
+00005930: 0072 0065 006e 0800 0000 0006 0000 0018  .r.e.n..........
+00005940: 5768 6f20 6361 6e20 636f 6d6d 656e 7420  Who can comment 
+00005950: 6f6e 2061 6c62 756d 0700 0000 0b49 7065  on album.....Ipe
+00005960: 726e 6974 7954 6162 0103 0000 0012 0057  rnityTab.......W
+00005970: 0065 0072 0020 006b 0061 006e 006e 003a  .e.r. .k.a.n.n.:
+00005980: 0800 0000 0006 0000 0008 5768 6f20 6361  ..........Who ca
+00005990: 6e3a 0700 0000 0b49 7065 726e 6974 7954  n:.....IpernityT
+000059a0: 6162 0103 0000 004c 0053 0063 0068 006c  ab.....L.S.c.h.l
+000059b0: 00fc 0073 0073 0065 006c 0077 00f6 0072  ...s.s.e.l.w...r
+000059c0: 0074 0065 0072 0020 0075 006e 0064 0020  .t.e.r. .u.n.d. 
+000059d0: 004e 006f 0074 0069 007a 0065 006e 0020  .N.o.t.i.z.e.n. 
+000059e0: 0068 0069 006e 007a 0075 0066 00fc 0067  .h.i.n.z.u.f...g
+000059f0: 0065 006e 0800 0000 0006 0000 0013 6164  .e.n..........ad
+00005a00: 6420 6b65 7977 6f72 6473 2c20 6e6f 7465  d keywords, note
+00005a10: 7307 0000 000b 4970 6572 6e69 7479 5461  s.....IpernityTa
+00005a20: 6201 0300 0000 2e00 4d00 6500 6e00 7300  b.......M.e.n.s.
+00005a30: 6300 6800 6500 6e00 2000 6900 6400 6500  c.h.e.n. .i.d.e.
+00005a40: 6e00 7400 6900 6600 6900 7a00 6900 6500  n.t.i.f.i.z.i.e.
+00005a50: 7200 6500 6e08 0000 0000 0600 0000 0f69  r.e.n..........i
+00005a60: 6465 6e74 6966 7920 7065 6f70 6c65 0700  dentify people..
+00005a70: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
+00005a80: 0000 003e 0065 0069 006e 0065 006e 0020  ...>.e.i.n.e.n. 
+00005a90: 004b 006f 006d 006d 0065 006e 0074 0061  .K.o.m.m.e.n.t.a
+00005aa0: 0072 0020 0076 0065 0072 00f6 0066 0066  .r. .v.e.r...f.f
+00005ab0: 0065 006e 0074 006c 0069 0063 0068 0065  .e.n.t.l.i.c.h.e
+00005ac0: 006e 0800 0000 0006 0000 000e 706f 7374  .n..........post
+00005ad0: 2061 2063 6f6d 6d65 6e74 0700 0000 0b49   a comment.....I
+00005ae0: 7065 726e 6974 7954 6162 0103 0000 0020  pernityTab..... 
+00005af0: 0044 0061 0073 0020 0046 006f 0074 006f  .D.a.s. .F.o.t.o
+00005b00: 0020 0061 006e 0073 0065 0068 0065 006e  . .a.n.s.e.h.e.n
+00005b10: 0800 0000 0006 0000 000d 7365 6520 7468  ..........see th
+00005b20: 6520 7068 6f74 6f07 0000 000b 4970 6572  e photo.....Iper
+00005b30: 6e69 7479 5461 6201 0300 0000 0a00 5300  nityTab.......S.
+00005b40: 7000 7200 3a00 2008 0000 0000 0600 0000  p.r.:. .........
+00005b50: 064c 616e 673a 2007 0000 000d 4c61 6e67  .Lang: .....Lang
+00005b60: 416c 7457 6964 6765 7401 0300 0000 0e00  AltWidget.......
+00005b70: 5300 7000 7200 6100 6300 6800 6508 0000  S.p.r.a.c.h.e...
+00005b80: 0000 0600 0000 084c 616e 6775 6167 6507  .......Language.
+00005b90: 0000 000d 4c61 6e67 416c 7457 6964 6765  ....LangAltWidge
+00005ba0: 7401 0300 0000 1800 4e00 6500 7500 6500  t.......N.e.u.e.
+00005bb0: 2000 5300 7000 7200 6100 6300 6800 6508   .S.p.r.a.c.h.e.
+00005bc0: 0000 0000 0600 0000 0c4e 6577 206c 616e  .........New lan
+00005bd0: 6775 6167 6507 0000 000d 4c61 6e67 416c  guage.....LangAl
+00005be0: 7457 6964 6765 7401 0300 0000 3200 5300  tWidget.....2.S.
+00005bf0: 7400 6100 6e00 6400 6100 7200 6400 7300  t.a.n.d.a.r.d.s.
+00005c00: 7000 7200 6100 6300 6800 6500 2000 6600  p.r.a.c.h.e. .f.
+00005c10: 6500 7300 7400 6c00 6500 6700 6500 6e08  e.s.t.l.e.g.e.n.
+00005c20: 0000 0000 0600 0000 1453 6574 2064 6566  .........Set def
+00005c30: 6175 6c74 206c 616e 6775 6167 6507 0000  ault language...
+00005c40: 000d 4c61 6e67 416c 7457 6964 6765 7401  ..LangAltWidget.
+00005c50: 0300 0000 b800 4900 6e00 2000 7700 6500  ......I.n. .w.e.
+00005c60: 6c00 6300 6800 6500 7200 2000 5300 7000  l.c.h.e.r. .S.p.
+00005c70: 7200 6100 6300 6800 6500 2000 6900 7300  r.a.c.h.e. .i.s.
+00005c80: 7400 2000 6400 6500 7200 2000 6100 6b00  t. .d.e.r. .a.k.
+00005c90: 7400 7500 6500 6c00 6c00 6500 2000 5400  t.u.e.l.l.e. .T.
+00005ca0: 6500 7800 7400 3f00 2000 4200 6900 7400  e.x.t.?. .B.i.t.
+00005cb0: 7400 6500 2000 6700 6500 6200 6500 6e00  t.e. .g.e.b.e.n.
+00005cc0: 2000 5300 6900 6500 2000 6500 6900 6e00   .S.i.e. .e.i.n.
+00005cd0: 2000 5200 4600 4300 3300 3000 3600 3600   .R.F.C.3.0.6.6.
+00005ce0: 2d00 5300 7000 7200 6100 6300 6800 6b00  -.S.p.r.a.c.h.k.
+00005cf0: 6500 6e00 6e00 7a00 6500 6900 6300 6800  e.n.n.z.e.i.c.h.
+00005d00: 6500 6e00 2000 6500 6900 6e00 2e08 0000  e.n. .e.i.n.....
+00005d10: 0000 0600 0000 4b57 6861 7420 6c61 6e67  ......KWhat lang
+00005d20: 7561 6765 2069 7320 7468 6520 6375 7272  uage is the curr
+00005d30: 656e 7420 7465 7874 2069 6e3f 2050 6c65  ent text in? Ple
+00005d40: 6173 6520 656e 7465 7220 616e 2052 4643  ase enter an RFC
+00005d50: 3330 3636 206c 616e 6775 6167 6520 7461  3066 language ta
+00005d60: 672e 0700 0000 0d4c 616e 6741 6c74 5769  g......LangAltWi
+00005d70: 6467 6574 0103 0000 00b2 0057 0065 006c  dget.......W.e.l
+00005d80: 0063 0068 0065 0020 0053 0070 0072 0061  .c.h.e. .S.p.r.a
+00005d90: 0063 0068 0065 0020 006d 00f6 0063 0068  .c.h.e. .m...c.h
+00005da0: 0074 0065 006e 0020 0053 0069 0065 0020  .t.e.n. .S.i.e. 
+00005db0: 0068 0069 006e 007a 0075 0066 00fc 0067  .h.i.n.z.u.f...g
+00005dc0: 0065 006e 003f 0020 0042 0069 0074 0074  .e.n.?. .B.i.t.t
+00005dd0: 0065 0020 0067 0065 0062 0065 006e 0020  .e. .g.e.b.e.n. 
+00005de0: 0053 0069 0065 0020 0065 0069 006e 0020  .S.i.e. .e.i.n. 
+00005df0: 0052 0046 0043 0033 0030 0036 0036 002d  .R.F.C.3.0.6.6.-
+00005e00: 0053 0070 0072 0061 0063 0068 006b 0065  .S.p.r.a.c.h.k.e
+00005e10: 006e 006e 007a 0065 0069 0063 0068 0065  .n.n.z.e.i.c.h.e
+00005e20: 006e 0020 0065 0069 006e 002e 0800 0000  .n. .e.i.n......
+00005e30: 0006 0000 004a 5768 6174 206c 616e 6775  .....JWhat langu
+00005e40: 6167 6520 776f 756c 6420 796f 7520 6c69  age would you li
+00005e50: 6b65 2074 6f20 6164 643f 2050 6c65 6173  ke to add? Pleas
+00005e60: 6520 656e 7465 7220 616e 2052 4643 3330  e enter an RFC30
+00005e70: 3636 206c 616e 6775 6167 6520 7461 672e  66 language tag.
+00005e80: 0700 0000 0d4c 616e 6741 6c74 5769 6467  .....LangAltWidg
+00005e90: 6574 0103 0000 001a 0042 0072 0065 0069  et.......B.r.e.i
+00005ea0: 0074 0065 002c 0020 004c 00e4 006e 0067  .t.e.,. .L...n.g
+00005eb0: 0065 0800 0000 0006 0000 0009 4c61 742c  .e..........Lat,
+00005ec0: 206c 6f6e 6707 0000 000e 4c61 744c 6f6e   long.....LatLon
+00005ed0: 6744 6973 706c 6179 0103 0000 003a 0050  gDisplay.....:.P
+00005ee0: 0068 006f 0074 0069 006e 0069 002d 0046  .h.o.t.i.n.i.-.F
+00005ef0: 0065 0068 006c 0065 0072 0070 0072 006f  .e.h.l.e.r.p.r.o
+00005f00: 0074 006f 006b 006f 006c 006c 0069 0065  .t.o.k.o.l.l.i.e
+00005f10: 0072 0075 006e 0067 0800 0000 0006 0000  .r.u.n.g........
+00005f20: 0015 5068 6f74 696e 6920 6572 726f 7220  ..Photini error 
+00005f30: 6c6f 6767 696e 6707 0000 000c 4c6f 6767  logging.....Logg
+00005f40: 6572 5769 6e64 6f77 0103 0000 0030 0050  erWindow.....0.P
+00005f50: 0072 006f 0074 006f 006b 006f 006c 006c  .r.o.t.o.k.o.l.l
+00005f60: 0064 0061 0074 0065 0069 0020 0073 0070  .d.a.t.e.i. .s.p
+00005f70: 0065 0069 0063 0068 0065 0072 006e 0800  .e.i.c.h.e.r.n..
+00005f80: 0000 0006 0000 000d 5361 7665 206c 6f67  ........Save log
+00005f90: 2066 696c 6507 0000 000c 4c6f 6767 6572   file.....Logger
+00005fa0: 5769 6e64 6f77 0103 0000 001a 004b 0061  Window.......K.a
+00005fb0: 0072 0074 0065 0020 0028 0026 0042 0069  .r.t.e. .(.&.B.i
+00005fc0: 006e 0067 0029 0800 0000 0006 0000 000b  .n.g.)..........
+00005fd0: 4d61 7020 2826 4269 6e67 2907 0000 000a  Map (&Bing).....
+00005fe0: 4d61 7054 6162 4269 6e67 0103 0000 0060  MapTabBing.....`
+00005ff0: 0053 0075 0063 0068 0065 0020 0075 006e  .S.u.c.h.e. .u.n
+00006000: 0064 0020 004e 0061 0063 0068 0073 0063  .d. .N.a.c.h.s.c
+00006010: 0068 006c 0061 0067 0065 006e 0020 0064  .h.l.a.g.e.n. .d
+00006020: 0065 0072 0020 0048 00f6 0068 0065 0020  .e.r. .H...h.e. 
+00006030: 0070 0072 006f 0076 0069 0064 0065 0064  .p.r.o.v.i.d.e.d
+00006040: 0020 0062 0079 0020 0042 0069 006e 0067  . .b.y. .B.i.n.g
+00006050: 0800 0000 0006 0000 002b 5365 6172 6368  .........+Search
+00006060: 2061 6e64 2061 6c74 6974 7564 6520 6c6f   and altitude lo
+00006070: 6f6b 7570 2070 726f 7669 6465 6420 6279  okup provided by
+00006080: 2042 696e 6707 0000 000a 4d61 7054 6162   Bing.....MapTab
+00006090: 4269 6e67 0103 0000 0054 0053 0065 0072  Bing.....T.S.e.r
+000060a0: 0076 0065 0072 0020 00fc 0062 0065 0072  .v.e.r. ...b.e.r
+000060b0: 006c 0061 0073 0074 0065 0074 002c 0020  .l.a.s.t.e.t.,. 
+000060c0: 0062 0069 0074 0074 0065 0020 006e 006f  .b.i.t.t.e. .n.o
+000060d0: 0063 0068 006d 0061 006c 0020 0070 0072  .c.h.m.a.l. .p.r
+000060e0: 006f 0062 0069 0065 0072 0065 006e 0800  .o.b.i.e.r.e.n..
+000060f0: 0000 0006 0000 0021 5365 7276 6572 206f  .......!Server o
+00006100: 7665 726c 6f61 642c 2070 6c65 6173 6520  verload, please 
+00006110: 7472 7920 6167 6169 6e07 0000 000a 4d61  try again.....Ma
+00006120: 7054 6162 4269 6e67 0103 0000 001e 004b  pTabBing.......K
+00006130: 0061 0072 0074 0065 0020 0028 0026 0047  .a.r.t.e. .(.&.G
+00006140: 006f 006f 0067 006c 0065 0029 0800 0000  .o.o.g.l.e.)....
+00006150: 0006 0000 000d 4d61 7020 2826 476f 6f67  ......Map (&Goog
+00006160: 6c65 2907 0000 000c 4d61 7054 6162 476f  le).....MapTabGo
+00006170: 6f67 6c65 0103 0000 0056 0053 0075 0063  ogle.....V.S.u.c
+00006180: 0068 0065 0020 0075 006e 0064 0020 0048  .h.e. .u.n.d. .H
+00006190: 00f6 0068 0065 006e 0065 0072 006d 0069  ...h.e.n.e.r.m.i
+000061a0: 0074 0074 006c 0075 006e 0067 0020 0070  .t.t.l.u.n.g. .p
+000061b0: 006f 0077 0065 0072 0065 0064 0020 0062  .o.w.e.r.e.d. .b
+000061c0: 0079 0020 0047 006f 006f 0067 006c 0065  .y. .G.o.o.g.l.e
+000061d0: 0800 0000 0006 0000 002c 5365 6172 6368  .........,Search
+000061e0: 2061 6e64 2061 6c74 6974 7564 6520 6c6f   and altitude lo
+000061f0: 6f6b 7570 2070 6f77 6572 6564 2062 7920  okup powered by 
+00006200: 476f 6f67 6c65 0700 0000 0c4d 6170 5461  Google.....MapTa
+00006210: 6247 6f6f 676c 6501 0300 0000 1e00 4b00  bGoogle.......K.
+00006220: 6100 7200 7400 6500 2000 2800 2600 4d00  a.r.t.e. .(.&.M.
+00006230: 6100 7000 6200 6f00 7800 2908 0000 0000  a.p.b.o.x.).....
+00006240: 0600 0000 0d4d 6170 2028 264d 6170 626f  .....Map (&Mapbo
+00006250: 7829 0700 0000 0c4d 6170 5461 624d 6170  x).....MapTabMap
+00006260: 626f 7801 0300 0000 2000 5300 7500 6300  box..... .S.u.c.
+00006270: 6800 6500 2000 6d00 6900 7400 2000 4d00  h.e. .m.i.t. .M.
+00006280: 6100 7000 6200 6f00 7808 0000 0000 0600  a.p.b.o.x.......
+00006290: 0000 1853 6561 7263 6820 706f 7765 7265  ...Search powere
+000062a0: 6420 6279 204d 6170 626f 7807 0000 000c  d by Mapbox.....
+000062b0: 4d61 7054 6162 4d61 7062 6f78 0103 0000  MapTabMapbox....
+000062c0: 0018 00dc 0062 0065 0072 0020 0050 0068  .....b.e.r. .P.h
+000062d0: 006f 0074 0069 006e 0069 0800 0000 0006  .o.t.i.n.i......
+000062e0: 0000 000d 4162 6f75 7420 5068 6f74 696e  ....About Photin
+000062f0: 6907 0000 0007 4d65 6e75 4261 7201 0300  i.....MenuBar...
+00006300: 0000 8000 4500 6900 6e00 2000 6500 6900  ....E.i.n. .e.i.
+00006310: 6e00 6600 6100 6300 6800 2000 7a00 7500  n.f.a.c.h. .z.u.
+00006320: 2000 6200 6500 6400 6900 6500 6e00 6500   .b.e.d.i.e.n.e.
+00006330: 6e00 6400 6500 7200 2000 4d00 6500 7400  n.d.e.r. .M.e.t.
+00006340: 6100 6400 6100 7400 6500 6e00 2d00 4500  a.d.a.t.e.n.-.E.
+00006350: 6400 6900 7400 6f00 7200 2000 6600 fc00  d.i.t.o.r. .f...
+00006360: 7200 2000 6400 6900 6700 6900 7400 6100  r. .d.i.g.i.t.a.
+00006370: 6c00 6500 2000 4200 6900 6c00 6400 6500  l.e. .B.i.l.d.e.
+00006380: 7200 2e08 0000 0000 0600 0000 5141 6e20  r...........QAn 
+00006390: 6561 7379 2074 6f20 7573 6520 6469 6769  easy to use digi
+000063a0: 7461 6c20 7068 6f74 6f67 7261 7068 206d  tal photograph m
+000063b0: 6574 6164 6174 6120 2845 7869 662c 2049  etadata (Exif, I
+000063c0: 5054 432c 2058 4d50 2920 6564 6974 696e  PTC, XMP) editin
+000063d0: 6720 6170 706c 6963 6174 696f 6e2e 0700  g application...
+000063e0: 0000 074d 656e 7542 6172 0103 0000 0032  ...MenuBar.....2
+000063f0: 0041 0075 0066 0020 0041 006b 0074 0075  .A.u.f. .A.k.t.u
+00006400: 0061 006c 0069 0073 0069 0065 0072 0075  .a.l.i.s.i.e.r.u
+00006410: 006e 0067 0020 0070 0072 00fc 0066 0065  .n.g. .p.r...f.e
+00006420: 006e 0800 0000 0006 0000 0010 4368 6563  .n..........Chec
+00006430: 6b20 666f 7220 7570 6461 7465 0700 0000  k for update....
+00006440: 074d 656e 7542 6172 0103 0000 002c 0041  .MenuBar.....,.A
+00006450: 006c 006c 0065 0020 0044 0061 0074 0065  .l.l.e. .D.a.t.e
+00006460: 0069 0065 006e 0020 0073 0063 0068 006c  .i.e.n. .s.c.h.l
+00006470: 0069 0065 00df 0065 006e 0800 0000 0006  .i.e...e.n......
+00006480: 0000 000f 436c 6f73 6520 616c 6c20 6669  ....Close all fi
+00006490: 6c65 7307 0000 0007 4d65 6e75 4261 7201  les.....MenuBar.
+000064a0: 0300 0000 3c00 5200 6500 6300 6800 7400  ....<.R.e.c.h.t.
+000064b0: 7300 6300 6800 7200 6500 6900 6200 7000  s.c.h.r.e.i.b.p.
+000064c0: 7200 fc00 6600 7500 6e00 6700 2000 6100  r...f.u.n.g. .a.
+000064d0: 6b00 7400 6900 7600 6900 6500 7200 6500  k.t.i.v.i.e.r.e.
+000064e0: 6e08 0000 0000 0600 0000 1245 6e61 626c  n..........Enabl
+000064f0: 6520 7370 656c 6c20 6368 6563 6b07 0000  e spell check...
+00006500: 0007 4d65 6e75 4261 7201 0300 0000 0a00  ..MenuBar.......
+00006510: 4400 6100 7400 6500 6908 0000 0000 0600  D.a.t.e.i.......
+00006520: 0000 0446 696c 6507 0000 0007 4d65 6e75  ...File.....Menu
+00006530: 4261 7201 0300 0000 4c00 4600 6500 6800  Bar.....L.F.e.h.
+00006540: 6c00 6500 6e00 6400 6500 2000 4d00 6900  l.e.n.d.e. .M.i.
+00006550: 6e00 6900 6100 7400 7500 7200 6100 6e00  n.i.a.t.u.r.a.n.
+00006560: 7300 6900 6300 6800 7400 6500 6e00 2000  s.i.c.h.t.e.n. .
+00006570: 6b00 6f00 7200 7200 6900 6700 6900 6500  k.o.r.r.i.g.i.e.
+00006580: 7200 6500 6e08 0000 0000 0600 0000 1646  r.e.n..........F
+00006590: 6978 206d 6973 7369 6e67 2074 6875 6d62  ix missing thumb
+000065a0: 6e61 696c 7307 0000 0007 4d65 6e75 4261  nails.....MenuBa
+000065b0: 7201 0300 0000 0a00 4800 6900 6c00 6600  r.......H.i.l.f.
+000065c0: 6508 0000 0000 0600 0000 0448 656c 7007  e..........Help.
+000065d0: 0000 0007 4d65 6e75 4261 7201 0300 0000  ....MenuBar.....
+000065e0: 1c00 4400 6100 7400 6500 6900 6500 6e00  ..D.a.t.e.i.e.n.
+000065f0: 2000 f600 6600 6600 6e00 6500 6e08 0000   ...f.f.n.e.n...
+00006600: 0000 0600 0000 0a4f 7065 6e20 6669 6c65  .......Open file
+00006610: 7307 0000 0007 4d65 6e75 4261 7201 0300  s.....MenuBar...
+00006620: 0000 6600 4400 6500 7200 2000 7100 7500  ..f.D.e.r. .q.u.
+00006630: 6500 6c00 6c00 6f00 6600 6600 6500 6e00  e.l.l.o.f.f.e.n.
+00006640: 6500 2000 5100 7500 6500 6c00 6c00 6300  e. .Q.u.e.l.l.c.
+00006650: 6f00 6400 6500 2000 6900 7300 7400 2000  o.d.e. .i.s.t. .
+00006660: 7600 6900 6100 2000 7b00 7500 7200 6c00  v.i.a. .{.u.r.l.
+00006670: 7d00 2000 6500 7200 6800 e400 6c00 7400  }. .e.r.h...l.t.
+00006680: 6c00 6900 6300 6800 2e08 0000 0000 0600  l.i.c.h.........
+00006690: 0000 294f 7065 6e20 736f 7572 6365 2070  ..)Open source p
+000066a0: 6163 6b61 6765 2061 7661 696c 6162 6c65  ackage available
+000066b0: 2066 726f 6d20 7b75 726c 7d2e 0700 0000   from {url}.....
+000066c0: 074d 656e 7542 6172 0103 0000 0010 004f  .MenuBar.......O
+000066d0: 0070 0074 0069 006f 006e 0065 006e 0800  .p.t.i.o.n.e.n..
+000066e0: 0000 0006 0000 0007 4f70 7469 6f6e 7307  ........Options.
+000066f0: 0000 0007 4d65 6e75 4261 7201 0300 0000  ....MenuBar.....
+00006700: 3000 4400 6f00 6b00 7500 6d00 6500 6e00  0.D.o.k.u.m.e.n.
+00006710: 7400 6100 7400 6900 6f00 6e00 2000 7a00  t.a.t.i.o.n. .z.
+00006720: 7500 2000 5000 6800 6f00 7400 6900 6e00  u. .P.h.o.t.i.n.
+00006730: 6908 0000 0000 0600 0000 1550 686f 7469  i..........Photi
+00006740: 6e69 2064 6f63 756d 656e 7461 7469 6f6e  ni documentation
+00006750: 0700 0000 074d 656e 7542 6172 0103 0000  .....MenuBar....
+00006760: 0036 0050 0068 006f 0074 0069 006e 0069  .6.P.h.o.t.i.n.i
+00006770: 002d 0046 006f 0074 006f 006d 0065 0074  .-.F.o.t.o.m.e.t
+00006780: 0061 0064 0061 0074 0065 006e 0065 0064  .a.d.a.t.e.n.e.d
+00006790: 0069 0074 006f 0072 0800 0000 0006 0000  .i.t.o.r........
+000067a0: 001d 5068 6f74 696e 6920 7068 6f74 6f20  ..Photini photo 
+000067b0: 6d65 7461 6461 7461 2065 6469 746f 7207  metadata editor.
+000067c0: 0000 0007 4d65 6e75 4261 7201 0300 0000  ....MenuBar.....
+000067d0: 1a00 5000 6800 6f00 7400 6900 6e00 6900  ..P.h.o.t.i.n.i.
+000067e0: 3a00 2000 fc00 6200 6500 7208 0000 0000  :. ...b.e.r.....
+000067f0: 0600 0000 0e50 686f 7469 6e69 3a20 6162  .....Photini: ab
+00006800: 6f75 7407 0000 0007 4d65 6e75 4261 7201  out.....MenuBar.
+00006810: 0300 0000 3000 5000 6800 6f00 7400 6900  ....0.P.h.o.t.i.
+00006820: 6e00 6900 3a00 2000 5600 6500 7200 7300  n.i.:. .V.e.r.s.
+00006830: 6900 6f00 6e00 7300 7000 7200 fc00 6600  i.o.n.s.p.r...f.
+00006840: 7500 6e00 6708 0000 0000 0600 0000 1650  u.n.g..........P
+00006850: 686f 7469 6e69 3a20 7665 7273 696f 6e20  hotini: version 
+00006860: 6368 6563 6b07 0000 0007 4d65 6e75 4261  check.....MenuBa
+00006870: 7201 0300 0000 1200 5300 6300 6800 6c00  r.......S.c.h.l.
+00006880: 6900 6500 df00 6500 6e08 0000 0000 0600  i.e...e.n.......
+00006890: 0000 0451 7569 7407 0000 0007 4d65 6e75  ...Quit.....Menu
+000068a0: 4261 7201 0300 0000 2800 c400 6e00 6400  Bar.....(...n.d.
+000068b0: 6500 7200 7500 6e00 6700 6500 6e00 2000  e.r.u.n.g.e.n. .
+000068c0: 7300 7000 6500 6900 6300 6800 6500 7200  s.p.e.i.c.h.e.r.
+000068d0: 6e08 0000 0000 0600 0000 0c53 6176 6520  n..........Save 
+000068e0: 6368 616e 6765 7307 0000 0007 4d65 6e75  changes.....Menu
+000068f0: 4261 7201 0300 0000 2400 4100 7500 7300  Bar.....$.A.u.s.
+00006900: 6700 6500 7700 e400 6800 6c00 7400 6500  g.e.w...h.l.t.e.
+00006910: 2000 4200 6900 6c00 6400 6500 7208 0000   .B.i.l.d.e.r...
+00006920: 0000 0600 0000 0f53 656c 6563 7465 6420  .......Selected 
+00006930: 696d 6167 6573 0700 0000 074d 656e 7542  images.....MenuB
+00006940: 6172 0103 0000 001a 0045 0069 006e 0073  ar.......E.i.n.s
+00006950: 0074 0065 006c 006c 0075 006e 0067 0065  .t.e.l.l.u.n.g.e
+00006960: 006e 0800 0000 0006 0000 0008 5365 7474  .n..........Sett
+00006970: 696e 6773 0700 0000 074d 656e 7542 6172  ings.....MenuBar
+00006980: 0103 0000 001e 0052 0065 0063 0068 0074  .......R.e.c.h.t
+00006990: 0073 0063 0068 0072 0065 0069 0062 0075  .s.c.h.r.e.i.b.u
+000069a0: 006e 0067 0800 0000 0006 0000 0008 5370  .n.g..........Sp
+000069b0: 656c 6c69 6e67 0700 0000 074d 656e 7542  elling.....MenuB
+000069c0: 6172 0103 0000 011c 0044 0069 0065 0073  ar.......D.i.e.s
+000069d0: 0065 0073 0020 0050 0072 006f 0067 0072  .e.s. .P.r.o.g.r
+000069e0: 0061 006d 006d 0020 0077 0075 0072 0064  .a.m.m. .w.u.r.d
+000069f0: 0065 0020 0075 006e 0074 0065 0072 0020  .e. .u.n.t.e.r. 
+00006a00: 0064 0065 0072 0020 0047 004e 0055 0020  .d.e.r. .G.N.U. 
+00006a10: 0047 0065 006e 0065 0072 0061 006c 0020  .G.e.n.e.r.a.l. 
+00006a20: 0050 0075 0062 006c 0069 0063 0020 004c  .P.u.b.l.i.c. .L
+00006a30: 0069 0063 0065 006e 0073 0065 0020 0076  .i.c.e.n.s.e. .v
+00006a40: 0065 0072 00f6 0066 0066 0065 006e 0074  .e.r...f.f.e.n.t
+00006a50: 006c 0069 0063 0068 0074 002e 0020 0046  .l.i.c.h.t... .F
+00006a60: 00fc 0072 0020 0077 0065 0069 0074 0065  ...r. .w.e.i.t.e
+00006a70: 0072 0065 0020 0049 006e 0066 006f 0072  .r.e. .I.n.f.o.r
+00006a80: 006d 0061 0074 0069 006f 006e 0065 006e  .m.a.t.i.o.n.e.n
+00006a90: 0020 0061 0075 0066 0020 0064 0069 0065  . .a.u.f. .d.i.e
+00006aa0: 0020 0053 0063 0068 0061 006c 0074 0066  . .S.c.h.a.l.t.f
+00006ab0: 006c 00e4 0063 0068 0065 0020 201e 007b  .l...c.h.e.  ..{
+00006ac0: 0064 0065 0074 0061 0069 006c 0073 007d  .d.e.t.a.i.l.s.}
+00006ad0: 201c 0020 006b 006c 0069 0063 006b 0065   .. .k.l.i.c.k.e
+00006ae0: 006e 002e 0800 0000 0006 0000 0065 5468  .n...........eTh
+00006af0: 6973 2070 726f 6772 616d 2069 7320 7265  is program is re
+00006b00: 6c65 6173 6564 2077 6974 6820 6120 474e  leased with a GN
+00006b10: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
+00006b20: 204c 6963 656e 7365 2e20 466f 7220 6465   License. For de
+00006b30: 7461 696c 7320 636c 6963 6b20 7468 6520  tails click the 
+00006b40: 227b 6465 7461 696c 737d 2220 6275 7474  "{details}" butt
+00006b50: 6f6e 2e07 0000 0007 4d65 6e75 4261 7201  on......MenuBar.
+00006b60: 0300 0000 a600 5300 6900 6500 2000 7600  ......S.i.e. .v.
+00006b70: 6500 7200 7700 6500 6e00 6400 6500 6e00  e.r.w.e.n.d.e.n.
+00006b80: 2000 6400 6500 7200 7a00 6500 6900 7400   .d.e.r.z.e.i.t.
+00006b90: 2000 5000 6800 6f00 7400 6900 6e00 6900   .P.h.o.t.i.n.i.
+00006ba0: 2000 5600 6500 7200 7300 6900 6f00 6e00   .V.e.r.s.i.o.n.
+00006bb0: 2000 7b00 7600 6500 7200 7300 6900 6f00   .{.v.e.r.s.i.o.
+00006bc0: 6e00 7d00 2e00 2000 4400 6900 6500 2000  n.}... .D.i.e. .
+00006bd0: 6e00 6500 7500 6500 7300 7400 6500 2000  n.e.u.e.s.t.e. .
+00006be0: 5600 6500 7200 7300 6900 6f00 6e00 2000  V.e.r.s.i.o.n. .
+00006bf0: 6900 7300 7400 2000 7b00 7200 6500 6c00  i.s.t. .{.r.e.l.
+00006c00: 6500 6100 7300 6500 7d00 2e08 0000 0000  e.a.s.e.}.......
+00006c10: 0600 0000 5559 6f75 2061 7265 2063 7572  ....UYou are cur
+00006c20: 7265 6e74 6c79 2072 756e 6e69 6e67 2050  rently running P
+00006c30: 686f 7469 6e69 2076 6572 7369 6f6e 207b  hotini version {
+00006c40: 7665 7273 696f 6e7d 2e20 5468 6520 6c61  version}. The la
+00006c50: 7465 7374 2072 656c 6561 7365 2069 7320  test release is 
+00006c60: 7b72 656c 6561 7365 7d2e 0700 0000 074d  {release}......M
+00006c70: 656e 7542 6172 0103 0000 0036 0026 0045  enuBar.....6.&.E
+00006c80: 0069 0067 0065 006e 0074 00fc 006d 0065  .i.g.e.n.t...m.e
+00006c90: 0072 0073 0063 0068 0061 0066 0074 002d  .r.s.c.h.a.f.t.-
+00006ca0: 004d 0065 0074 0061 0064 0061 0074 0065  .M.e.t.a.d.a.t.e
+00006cb0: 006e 0800 0000 0006 0000 0013 264f 776e  .n..........&Own
+00006cc0: 6572 7368 6970 206d 6574 6164 6174 6107  ership metadata.
+00006cd0: 0000 0008 4f77 6e65 7254 6162 0103 0000  ....OwnerTab....
+00006ce0: 002e 0041 006c 006c 0065 0020 0052 0065  ...A.l.l.e. .R.e
+00006cf0: 0063 0068 0074 0065 0020 0076 006f 0072  .c.h.t.e. .v.o.r
+00006d00: 0062 0065 0068 0061 006c 0074 0065 006e  .b.e.h.a.l.t.e.n
+00006d10: 0800 0000 0006 0000 0013 416c 6c20 7269  ..........All ri
+00006d20: 6768 7473 2072 6573 6572 7665 6407 0000  ghts reserved...
+00006d30: 0008 4f77 6e65 7254 6162 0103 0000 0020  ..OwnerTab..... 
+00006d40: 0056 006f 0072 006c 0061 0067 0065 0020  .V.o.r.l.a.g.e. 
+00006d50: 0061 006e 0077 0065 006e 0064 0065 006e  .a.n.w.e.n.d.e.n
+00006d60: 0800 0000 0006 0000 000e 4170 706c 7920  ..........Apply 
+00006d70: 7465 6d70 6c61 7465 0700 0000 084f 776e  template.....Own
+00006d80: 6572 5461 6201 0300 0000 3a00 4e00 6100  erTab.....:.N.a.
+00006d90: 6d00 6500 6e00 7300 6e00 6500 6e00 6e00  m.e.n.s.n.e.n.n.
+00006da0: 7500 6e00 6700 2000 3400 2e00 3000 2000  u.n.g. .4...0. .
+00006db0: 2800 4300 4300 2000 4200 5900 2000 3400  (.C.C. .B.Y. .4.
+00006dc0: 2e00 3000 2908 0000 0000 0600 0000 1b41  ..0.)..........A
+00006dd0: 7474 7269 6275 7469 6f6e 2034 2e30 2028  ttribution 4.0 (
+00006de0: 4343 2042 5920 342e 3029 0700 0000 084f  CC BY 4.0).....O
+00006df0: 776e 6572 5461 6201 0300 0000 6c00 4e00  wnerTab.....l.N.
+00006e00: 6100 6d00 6500 6e00 7300 6e00 6500 6e00  a.m.e.n.s.n.e.n.
+00006e10: 6e00 7500 6e00 6700 2000 2d00 2000 4b00  n.u.n.g. .-. .K.
+00006e20: 6500 6900 6e00 6500 2000 4200 6500 6100  e.i.n.e. .B.e.a.
+00006e30: 7200 6200 6500 6900 7400 7500 6e00 6700  r.b.e.i.t.u.n.g.
+00006e40: 6500 6e00 2000 3400 2e00 3000 2000 2800  e.n. .4...0. .(.
+00006e50: 4300 4300 2000 4200 5900 2d00 4e00 4400  C.C. .B.Y.-.N.D.
+00006e60: 2000 3400 2e00 3000 2908 0000 0000 0600   .4...0.).......
+00006e70: 0000 2c41 7474 7269 6275 7469 6f6e 2d4e  ..,Attribution-N
+00006e80: 6f44 6572 6976 6174 6976 6573 2034 2e30  oDerivatives 4.0
+00006e90: 2028 4343 2042 592d 4e44 2034 2e30 2907   (CC BY-ND 4.0).
+00006ea0: 0000 0008 4f77 6e65 7254 6162 0103 0000  ....OwnerTab....
+00006eb0: 0064 004e 0061 006d 0065 006e 0073 006e  .d.N.a.m.e.n.s.n
+00006ec0: 0065 006e 006e 0075 006e 0067 002d 004e  .e.n.n.u.n.g.-.N
+00006ed0: 0069 0063 0068 0074 0020 006b 006f 006d  .i.c.h.t. .k.o.m
+00006ee0: 006d 0065 0072 007a 0069 0065 006c 006c  .m.e.r.z.i.e.l.l
+00006ef0: 0020 0034 002e 0030 0020 0028 0043 0043  . .4...0. .(.C.C
+00006f00: 0020 0042 0059 002d 004e 0043 0020 0034  . .B.Y.-.N.C. .4
+00006f10: 002e 0030 0029 0800 0000 0006 0000 002c  ...0.).........,
+00006f20: 4174 7472 6962 7574 696f 6e2d 4e6f 6e43  Attribution-NonC
+00006f30: 6f6d 6d65 7263 6961 6c20 342e 3020 2843  ommercial 4.0 (C
+00006f40: 4320 4259 2d4e 4320 342e 3029 0700 0000  C BY-NC 4.0)....
+00006f50: 084f 776e 6572 5461 6201 0300 0000 9a00  .OwnerTab.......
+00006f60: 4e00 6100 6d00 6500 6e00 7300 6e00 6500  N.a.m.e.n.s.n.e.
+00006f70: 6e00 6e00 7500 6e00 6700 2000 2d00 2000  n.n.u.n.g. .-. .
+00006f80: 4e00 6900 6300 6800 7400 2000 6b00 6f00  N.i.c.h.t. .k.o.
+00006f90: 6d00 6d00 6500 7200 7a00 6900 6500 6c00  m.m.e.r.z.i.e.l.
+00006fa0: 6c00 2000 2d00 2000 4b00 6500 6900 6e00  l. .-. .K.e.i.n.
+00006fb0: 6500 2000 4200 6500 6100 7200 6200 6500  e. .B.e.a.r.b.e.
+00006fc0: 6900 7400 7500 6e00 6700 6500 6e00 2000  i.t.u.n.g.e.n. .
+00006fd0: 3400 2e00 3000 2000 2800 4300 4300 2000  4...0. .(.C.C. .
+00006fe0: 4200 5900 2d00 4e00 4300 2d00 4e00 4400  B.Y.-.N.C.-.N.D.
+00006ff0: 2000 3400 2e00 3000 2908 0000 0000 0600   .4...0.).......
+00007000: 0000 3d41 7474 7269 6275 7469 6f6e 2d4e  ..=Attribution-N
+00007010: 6f6e 436f 6d6d 6572 6369 616c 2d4e 6f44  onCommercial-NoD
+00007020: 6572 6976 6174 6976 6573 2034 2e30 2028  erivatives 4.0 (
+00007030: 4343 2042 592d 4e43 2d4e 4420 342e 3029  CC BY-NC-ND 4.0)
+00007040: 0700 0000 084f 776e 6572 5461 6201 0300  .....OwnerTab...
+00007050: 0000 be00 4e00 6100 6d00 6500 6e00 7300  ....N.a.m.e.n.s.
+00007060: 6e00 6500 6e00 6e00 7500 6e00 6700 2000  n.e.n.n.u.n.g. .
+00007070: 2d00 2000 4e00 6900 6300 6800 7400 2d00  -. .N.i.c.h.t.-.
+00007080: 6b00 6f00 6d00 6d00 6500 7200 7a00 6900  k.o.m.m.e.r.z.i.
+00007090: 6500 6c00 6c00 2000 2d00 2000 5700 6500  e.l.l. .-. .W.e.
+000070a0: 6900 7400 6500 7200 6700 6100 6200 6500  i.t.e.r.g.a.b.e.
+000070b0: 2000 7500 6e00 7400 6500 7200 2000 6700   .u.n.t.e.r. .g.
+000070c0: 6c00 6500 6900 6300 6800 6500 6e00 2000  l.e.i.c.h.e.n. .
+000070d0: 4200 6500 6400 6900 6e00 6700 7500 6e00  B.e.d.i.n.g.u.n.
+000070e0: 6700 6500 6e00 2000 3400 2e00 3000 2000  g.e.n. .4...0. .
+000070f0: 2800 4300 4300 2000 4200 5900 2d00 4e00  (.C.C. .B.Y.-.N.
+00007100: 4300 2d00 5300 4100 2000 3400 2e00 3000  C.-.S.A. .4...0.
+00007110: 2908 0000 0000 0600 0000 3a41 7474 7269  ).........:Attri
+00007120: 6275 7469 6f6e 2d4e 6f6e 436f 6d6d 6572  bution-NonCommer
+00007130: 6369 616c 2d53 6861 7265 416c 696b 6520  cial-ShareAlike 
+00007140: 342e 3020 2843 4320 4259 2d4e 432d 5341  4.0 (CC BY-NC-SA
+00007150: 2034 2e30 2907 0000 0008 4f77 6e65 7254   4.0).....OwnerT
+00007160: 6162 0103 0000 0090 004e 0061 006d 0065  ab.......N.a.m.e
+00007170: 006e 0073 006e 0065 006e 006e 0075 006e  .n.s.n.e.n.n.u.n
+00007180: 0067 0020 002d 0020 0057 0065 0069 0074  .g. .-. .W.e.i.t
+00007190: 0065 0072 0067 0061 0062 0065 0020 0075  .e.r.g.a.b.e. .u
+000071a0: 006e 0074 0065 0072 0020 0067 006c 0065  .n.t.e.r. .g.l.e
+000071b0: 0069 0063 0068 0065 006e 0020 0042 0065  .i.c.h.e.n. .B.e
+000071c0: 0064 0069 006e 0067 0075 006e 0067 0065  .d.i.n.g.u.n.g.e
+000071d0: 006e 0020 0034 002e 0030 0020 0028 0043  .n. .4...0. .(.C
+000071e0: 0043 0020 0042 0059 002d 0053 0041 0020  .C. .B.Y.-.S.A. 
+000071f0: 0034 002e 0030 0029 0800 0000 0006 0000  .4...0.)........
+00007200: 0029 4174 7472 6962 7574 696f 6e2d 5368  .)Attribution-Sh
+00007210: 6172 6541 6c69 6b65 2034 2e30 2028 4343  areAlike 4.0 (CC
+00007220: 2042 592d 5341 2034 2e30 2907 0000 0008   BY-SA 4.0).....
+00007230: 4f77 6e65 7254 6162 0103 0000 006a 0043  OwnerTab.....j.C
+00007240: 0043 0030 0020 0031 002e 0030 0020 0055  .C.0. .1...0. .U
+00007250: 006e 0069 0076 0065 0072 0073 0065 006c  .n.i.v.e.r.s.e.l
+00007260: 006c 0020 0028 0043 0043 0030 0020 0031  .l. .(.C.C.0. .1
+00007270: 002e 0030 0029 0020 0050 0075 0062 006c  ...0.). .P.u.b.l
+00007280: 0069 0063 0020 0044 006f 006d 0061 0069  .i.c. .D.o.m.a.i
+00007290: 006e 0020 0044 0065 0064 0069 0063 0061  .n. .D.e.d.i.c.a
+000072a0: 0074 0069 006f 006e 0800 0000 0006 0000  .t.i.o.n........
+000072b0: 0034 4343 3020 312e 3020 556e 6976 6572  .4CC0 1.0 Univer
+000072c0: 7361 6c20 2843 4330 2031 2e30 2920 5075  sal (CC0 1.0) Pu
+000072d0: 626c 6963 2044 6f6d 6169 6e20 4465 6469  blic Domain Dedi
+000072e0: 6361 7469 6f6e 0700 0000 084f 776e 6572  cation.....Owner
+000072f0: 5461 6201 0300 0000 0a00 5300 7400 6100  Tab.......S.t.a.
+00007300: 6400 7408 0000 0000 0600 0000 0443 6974  d.t..........Cit
+00007310: 7907 0000 0008 4f77 6e65 7254 6162 0103  y.....OwnerTab..
+00007320: 0000 0028 0055 0072 0068 0065 0062 0065  ...(.U.r.h.e.b.e
+00007330: 0072 0072 0065 0063 0068 0074 0073 0068  .r.r.e.c.h.t.s.h
+00007340: 0069 006e 0077 0065 0069 0073 0800 0000  .i.n.w.e.i.s....
+00007350: 0006 0000 0010 436f 7079 7269 6768 7420  ......Copyright 
+00007360: 4e6f 7469 6365 0700 0000 084f 776e 6572  Notice.....Owner
+00007370: 5461 6201 0300 0000 0800 4c00 6100 6e00  Tab.......L.a.n.
+00007380: 6408 0000 0000 0600 0000 0743 6f75 6e74  d..........Count
+00007390: 7279 0700 0000 084f 776e 6572 5461 6201  ry.....OwnerTab.
+000073a0: 0300 0000 1000 4600 6f00 7400 6f00 6700  ......F.o.t.o.g.
+000073b0: 7200 6100 6608 0000 0000 0600 0000 0743  r.a.f..........C
+000073c0: 7265 6174 6f72 0700 0000 084f 776e 6572  reator.....Owner
+000073d0: 5461 6201 0300 0000 2c00 4e00 6500 7500  Tab.....,.N.e.u.
+000073e0: 6500 2000 4c00 6900 7a00 6500 6e00 7a00  e. .L.i.z.e.n.z.
+000073f0: 2000 6400 6500 6600 6900 6e00 6900 6500   .d.e.f.i.n.i.e.
+00007400: 7200 6500 6e08 0000 0000 0600 0000 1244  r.e.n..........D
+00007410: 6566 696e 6520 6e65 7720 6c69 6365 6e63  efine new licenc
+00007420: 6507 0000 0008 4f77 6e65 7254 6162 0103  e.....OwnerTab..
+00007430: 0000 0024 0056 006f 0072 006c 0061 0067  ...$.V.o.r.l.a.g
+00007440: 0065 0020 0062 0065 0061 0072 0062 0065  .e. .b.e.a.r.b.e
+00007450: 0069 0074 0065 006e 0800 0000 0006 0000  .i.t.e.n........
+00007460: 000d 4564 6974 2074 656d 706c 6174 6507  ..Edit template.
+00007470: 0000 0008 4f77 6e65 7254 6162 0103 0000  ....OwnerTab....
+00007480: 0012 0045 002d 004d 0061 0069 006c 0028  ...E.-.M.a.i.l.(
+00007490: 0073 0029 0800 0000 0006 0000 0008 456d  .s.)..........Em
+000074a0: 6169 6c28 7329 0700 0000 084f 776e 6572  ail(s).....Owner
+000074b0: 5461 6201 0300 0000 e000 4700 6500 6200  Tab.......G.e.b.
+000074c0: 6500 6e00 2000 5300 6900 6500 2000 6500  e.n. .S.i.e. .e.
+000074d0: 6900 6e00 6500 6e00 2000 4800 6900 6e00  i.n.e.n. .H.i.n.
+000074e0: 7700 6500 6900 7300 2000 6100 7500 6600  w.e.i.s. .a.u.f.
+000074f0: 2000 6400 6500 6e00 2000 6100 6b00 7400   .d.e.n. .a.k.t.
+00007500: 7500 6500 6c00 6c00 6500 6e00 2000 4900  u.e.l.l.e.n. .I.
+00007510: 6e00 6800 6100 6200 6500 7200 2000 6400  n.h.a.b.e.r. .d.
+00007520: 6500 7300 2000 5500 7200 6800 6500 6200  e.s. .U.r.h.e.b.
+00007530: 6500 7200 7200 6500 6300 6800 7400 7300  e.r.r.e.c.h.t.s.
+00007540: 2000 6600 fc00 7200 2000 6400 6900 6500   .f...r. .d.i.e.
+00007550: 7300 6500 7300 2000 4200 6900 6c00 6400  s.e.s. .B.i.l.d.
+00007560: 2000 6500 6900 6e00 2c00 2000 7a00 2e00   .e.i.n.,. .z...
+00007570: 2000 4200 2e00 2000 2200 a900 3200 3000   .B... ."...2.0.
+00007580: 3000 3800 2000 4a00 6100 6e00 6500 2000  0.8. .J.a.n.e. .
+00007590: 4400 6f00 6500 2200 2e08 0000 0000 0600  D.o.e.".........
+000075a0: 0000 5f45 6e74 6572 2061 206e 6f74 6963  .._Enter a notic
+000075b0: 6520 6f6e 2074 6865 2063 7572 7265 6e74  e on the current
+000075c0: 206f 776e 6572 206f 6620 7468 6520 636f   owner of the co
+000075d0: 7079 7269 6768 7420 666f 7220 7468 6973  pyright for this
+000075e0: 2069 6d61 6765 2c20 7375 6368 2061 7320   image, such as 
+000075f0: 22c2 a932 3030 3820 4a61 6e65 2044 6f65  "..2008 Jane Doe
+00007600: 222e 0700 0000 084f 776e 6572 5461 6201  "......OwnerTab.
+00007610: 0300 0001 1800 4700 6500 6200 6500 6e00  ......G.e.b.e.n.
+00007620: 2000 5300 6900 6500 2000 4900 6e00 6600   .S.i.e. .I.n.f.
+00007630: 6f00 7200 6d00 6100 7400 6900 6f00 6e00  o.r.m.a.t.i.o.n.
+00007640: 6500 6e00 2000 fc00 6200 6500 7200 2000  e.n. ...b.e.r. .
+00007650: 4500 6d00 6200 6100 7200 6700 6f00 7300  E.m.b.a.r.g.o.s.
+00007660: 2000 6f00 6400 6500 7200 2000 6100 6e00   .o.d.e.r. .a.n.
+00007670: 6400 6500 7200 6500 2000 4500 6900 6e00  d.e.r.e. .E.i.n.
+00007680: 7300 6300 6800 7200 e400 6e00 6b00 7500  s.c.h.r...n.k.u.
+00007690: 6e00 6700 6500 6e00 2000 6500 6900 6e00  n.g.e.n. .e.i.n.
+000076a0: 2c00 2000 6400 6900 6500 2000 6e00 6900  ,. .d.i.e. .n.i.
+000076b0: 6300 6800 7400 2000 6400 7500 7200 6300  c.h.t. .d.u.r.c.
+000076c0: 6800 2000 6400 6100 7300 2000 4600 6500  h. .d.a.s. .F.e.
+000076d0: 6c00 6400 2000 5200 6500 6300 6800 7400  l.d. .R.e.c.h.t.
+000076e0: 6500 7600 6500 7200 7700 6500 6e00 6400  e.v.e.r.w.e.n.d.
+000076f0: 7500 6e00 6700 7300 6200 6500 6400 6900  u.n.g.s.b.e.d.i.
+00007700: 6e00 6700 7500 6e00 6700 6500 6e00 2000  n.g.u.n.g.e.n. .
+00007710: 6100 6200 6700 6500 6400 6500 6300 6b00  a.b.g.e.d.e.c.k.
+00007720: 7400 2000 7300 6900 6e00 6400 2e08 0000  t. .s.i.n.d.....
+00007730: 0000 0600 0000 6545 6e74 6572 2069 6e66  ......eEnter inf
+00007740: 6f72 6d61 7469 6f6e 2061 626f 7574 2065  ormation about e
+00007750: 6d62 6172 676f 6573 2c20 6f72 206f 7468  mbargoes, or oth
+00007760: 6572 2072 6573 7472 6963 7469 6f6e 7320  er restrictions 
+00007770: 6e6f 7420 636f 7665 7265 6420 6279 2074  not covered by t
+00007780: 6865 2052 6967 6874 7320 5573 6167 6520  he Rights Usage 
+00007790: 5465 726d 7320 6669 656c 642e 0700 0000  Terms field.....
+000077a0: 084f 776e 6572 5461 6201 0300 0000 7200  .OwnerTab.....r.
+000077b0: 4700 6500 6200 6500 6e00 2000 5300 6900  G.e.b.e.n. .S.i.
+000077c0: 6500 2000 4100 6e00 7700 6500 6900 7300  e. .A.n.w.e.i.s.
+000077d0: 7500 6e00 6700 6500 6e00 2000 7a00 7500  u.n.g.e.n. .z.u.
+000077e0: 7200 2000 6c00 6500 6700 6100 6c00 6500  r. .l.e.g.a.l.e.
+000077f0: 6e00 2000 4e00 7500 7400 7a00 7500 6e00  n. .N.u.t.z.u.n.
+00007800: 6700 2000 6400 6500 7300 2000 4200 6900  g. .d.e.s. .B.i.
+00007810: 6c00 6400 6500 7300 2000 6500 6900 6e00  l.d.e.s. .e.i.n.
+00007820: 2e08 0000 0000 0600 0000 3945 6e74 6572  ..........9Enter
+00007830: 2069 6e73 7472 7563 7469 6f6e 7320 6f6e   instructions on
+00007840: 2068 6f77 2074 6869 7320 696d 6167 6520   how this image 
+00007850: 6361 6e20 6c65 6761 6c6c 7920 6265 2075  can legally be u
+00007860: 7365 642e 0700 0000 084f 776e 6572 5461  sed......OwnerTa
+00007870: 6201 0300 0000 a200 4700 6500 6200 6500  b.......G.e.b.e.
+00007880: 6e00 2000 5300 6900 6500 2000 6400 6900  n. .S.i.e. .d.i.
+00007890: 6500 2000 5300 7400 6100 6400 7400 2000  e. .S.t.a.d.t. .
+000078a0: 6600 fc00 7200 2000 6400 6900 6500 2000  f...r. .d.i.e. .
+000078b0: 4100 6400 7200 6500 7300 7300 6500 2000  A.d.r.e.s.s.e. .
+000078c0: 6400 6500 7200 2000 5000 6500 7200 7300  d.e.r. .P.e.r.s.
+000078d0: 6f00 6e00 2000 6500 6900 6e00 2c00 2000  o.n. .e.i.n.,. .
+000078e0: 6400 6900 6500 2000 6400 6900 6500 7300  d.i.e. .d.i.e.s.
+000078f0: 6500 7300 2000 4200 6900 6c00 6400 2000  e.s. .B.i.l.d. .
+00007900: 6500 7200 7300 7400 6500 6c00 6c00 7400  e.r.s.t.e.l.l.t.
+00007910: 2000 6800 6100 7400 2e08 0000 0000 0600   .h.a.t.........
+00007920: 0000 4545 6e74 6572 2074 6865 2063 6974  ..EEnter the cit
+00007930: 7920 666f 7220 7468 6520 6164 6472 6573  y for the addres
+00007940: 7320 6f66 2074 6865 2070 6572 736f 6e20  s of the person 
+00007950: 7468 6174 2063 7265 6174 6564 2074 6869  that created thi
+00007960: 7320 696d 6167 652e 0700 0000 084f 776e  s image......Own
+00007970: 6572 5461 6201 0300 0000 ae00 4700 6500  erTab.......G.e.
+00007980: 6200 6500 6e00 2000 5300 6900 6500 2000  b.e.n. .S.i.e. .
+00007990: 6400 6500 6e00 2000 4c00 e400 6e00 6400  d.e.n. .L...n.d.
+000079a0: 6500 7200 6e00 6100 6d00 6500 6e00 2000  e.r.n.a.m.e.n. .
+000079b0: 6600 fc00 7200 2000 6400 6900 6500 2000  f...r. .d.i.e. .
+000079c0: 4100 6400 7200 6500 7300 7300 6500 2000  A.d.r.e.s.s.e. .
+000079d0: 6400 6500 7200 2000 5000 6500 7200 7300  d.e.r. .P.e.r.s.
+000079e0: 6f00 6e00 2000 6500 6900 6e00 2c00 2000  o.n. .e.i.n.,. .
+000079f0: 6400 6900 6500 2000 6400 6900 6500 7300  d.i.e. .d.i.e.s.
+00007a00: 6500 7300 2000 4200 6900 6c00 6400 2000  e.s. .B.i.l.d. .
+00007a10: 6500 7200 7300 7400 6500 6c00 6c00 7400  e.r.s.t.e.l.l.t.
+00007a20: 2000 6800 6100 7400 2e08 0000 0000 0600   .h.a.t.........
+00007a30: 0000 4d45 6e74 6572 2074 6865 2063 6f75  ..MEnter the cou
+00007a40: 6e74 7279 206e 616d 6520 666f 7220 7468  ntry name for th
+00007a50: 6520 6164 6472 6573 7320 6f66 2074 6865  e address of the
+00007a60: 2070 6572 736f 6e20 7468 6174 2063 7265   person that cre
+00007a70: 6174 6564 2074 6869 7320 696d 6167 652e  ated this image.
+00007a80: 0700 0000 084f 776e 6572 5461 6201 0300  .....OwnerTab...
+00007a90: 0000 a600 4700 6500 6200 6500 6e00 2000  ....G.e.b.e.n. .
+00007aa0: 5300 6900 6500 2000 6400 6900 6500 2000  S.i.e. .d.i.e. .
+00007ab0: 4200 6500 7200 7500 6600 7300 6200 6500  B.e.r.u.f.s.b.e.
+00007ac0: 7a00 6500 6900 6300 6800 6e00 7500 6e00  z.e.i.c.h.n.u.n.
+00007ad0: 6700 2000 6400 6500 7200 2000 5000 6500  g. .d.e.r. .P.e.
+00007ae0: 7200 7300 6f00 6e00 2000 6500 6900 6e00  r.s.o.n. .e.i.n.
+00007af0: 2c00 2000 6400 6900 6500 2000 6900 6d00  ,. .d.i.e. .i.m.
+00007b00: 2000 4600 6500 6c00 6400 2000 5500 7200   .F.e.l.d. .U.r.
+00007b10: 6800 6500 6200 6500 7200 2000 6100 7500  h.e.b.e.r. .a.u.
+00007b20: 6600 6700 6500 6600 fc00 6800 7200 7400  f.g.e.f...h.r.t.
+00007b30: 2000 6900 7300 7400 2e08 0000 0000 0600   .i.s.t.........
+00007b40: 0000 3e45 6e74 6572 2074 6865 206a 6f62  ..>Enter the job
+00007b50: 2074 6974 6c65 206f 6620 7468 6520 7065   title of the pe
+00007b60: 7273 6f6e 206c 6973 7465 6420 696e 2074  rson listed in t
+00007b70: 6865 2043 7265 6174 6f72 2066 6965 6c64  he Creator field
+00007b80: 2e07 0000 0008 4f77 6e65 7254 6162 0103  ......OwnerTab..
+00007b90: 0000 0082 0047 0065 0062 0065 006e 0020  .....G.e.b.e.n. 
+00007ba0: 0053 0069 0065 0020 0064 0065 006e 0020  .S.i.e. .d.e.n. 
+00007bb0: 004e 0061 006d 0065 006e 0020 0064 0065  .N.a.m.e.n. .d.e
+00007bc0: 0072 0020 0050 0065 0072 0073 006f 006e  .r. .P.e.r.s.o.n
+00007bd0: 0020 0065 0069 006e 002c 0020 0064 0069  . .e.i.n.,. .d.i
+00007be0: 0065 0020 0064 0069 0065 0073 0065 0073  .e. .d.i.e.s.e.s
+00007bf0: 0020 0042 0069 006c 0064 0020 0065 0072  . .B.i.l.d. .e.r
+00007c00: 0073 0074 0065 006c 006c 0074 0020 0068  .s.t.e.l.l.t. .h
+00007c10: 0061 0074 002e 0800 0000 0006 0000 0035  .a.t...........5
+00007c20: 456e 7465 7220 7468 6520 6e61 6d65 206f  Enter the name o
+00007c30: 6620 7468 6520 7065 7273 6f6e 2074 6861  f the person tha
+00007c40: 7420 6372 6561 7465 6420 7468 6973 2069  t created this i
+00007c50: 6d61 6765 2e07 0000 0008 4f77 6e65 7254  mage......OwnerT
+00007c60: 6162 0103 0000 00b0 0047 0065 0062 0065  ab.......G.e.b.e
+00007c70: 006e 0020 0053 0069 0065 0020 0064 0069  .n. .S.i.e. .d.i
+00007c80: 0065 0020 0050 006f 0073 0074 006c 0065  .e. .P.o.s.t.l.e
+00007c90: 0069 0074 007a 0061 0068 006c 0020 0066  .i.t.z.a.h.l. .f
+00007ca0: 00fc 0072 0020 0064 0069 0065 0020 0041  ...r. .d.i.e. .A
+00007cb0: 0064 0072 0065 0073 0073 0065 0020 0064  .d.r.e.s.s.e. .d
+00007cc0: 0065 0072 0020 0050 0065 0072 0073 006f  .e.r. .P.e.r.s.o
+00007cd0: 006e 0020 0065 0069 006e 002c 0020 0064  .n. .e.i.n.,. .d
+00007ce0: 0069 0065 0020 0064 0069 0065 0073 0065  .i.e. .d.i.e.s.e
+00007cf0: 0073 0020 0042 0069 006c 0064 0020 0065  .s. .B.i.l.d. .e
+00007d00: 0072 0073 0074 0065 006c 006c 0074 0020  .r.s.t.e.l.l.t. 
+00007d10: 0068 0061 0074 002e 0800 0000 0006 0000  .h.a.t..........
+00007d20: 004c 456e 7465 7220 7468 6520 706f 7374  .LEnter the post
+00007d30: 616c 2063 6f64 6520 666f 7220 7468 6520  al code for the 
+00007d40: 6164 6472 6573 7320 6f66 2074 6865 2070  address of the p
+00007d50: 6572 736f 6e20 7468 6174 2063 7265 6174  erson that creat
+00007d60: 6564 2074 6869 7320 696d 6167 652e 0700  ed this image...
+00007d70: 0000 084f 776e 6572 5461 6201 0300 0000  ...OwnerTab.....
+00007d80: ac00 4700 6500 6200 6500 6e00 2000 5300  ..G.e.b.e.n. .S.
+00007d90: 6900 6500 2000 6400 6100 7300 2000 4200  i.e. .d.a.s. .B.
+00007da0: 7500 6e00 6400 6500 7300 6c00 6100 6e00  u.n.d.e.s.l.a.n.
+00007db0: 6400 2000 6600 fc00 7200 2000 6400 6900  d. .f...r. .d.i.
+00007dc0: 6500 2000 4100 6400 7200 6500 7300 7300  e. .A.d.r.e.s.s.
+00007dd0: 6500 2000 6400 6500 7200 2000 5000 6500  e. .d.e.r. .P.e.
+00007de0: 7200 7300 6f00 6e00 2000 6500 6900 6e00  r.s.o.n. .e.i.n.
+00007df0: 2c00 2000 6400 6900 6500 2000 6400 6900  ,. .d.i.e. .d.i.
+00007e00: 6500 7300 6500 7300 2000 4200 6900 6c00  e.s.e.s. .B.i.l.
+00007e10: 6400 2000 6500 7200 7300 7400 6500 6c00  d. .e.r.s.t.e.l.
+00007e20: 6c00 7400 2000 6800 6100 7400 2e08 0000  l.t. .h.a.t.....
+00007e30: 0000 0600 0000 4645 6e74 6572 2074 6865  ......FEnter the
+00007e40: 2073 7461 7465 2066 6f72 2074 6865 2061   state for the a
+00007e50: 6464 7265 7373 206f 6620 7468 6520 7065  ddress of the pe
+00007e60: 7273 6f6e 2074 6861 7420 6372 6561 7465  rson that create
+00007e70: 6420 7468 6973 2069 6d61 6765 2e07 0000  d this image....
+00007e80: 0008 4f77 6e65 7254 6162 0103 0000 0096  ..OwnerTab......
+00007e90: 0047 0065 0062 0065 006e 0020 0053 0069  .G.e.b.e.n. .S.i
+00007ea0: 0065 0020 0065 0069 006e 002c 0020 0077  .e. .e.i.n.,. .w
+00007eb0: 0065 0072 0020 0062 0065 0069 0020 0064  .e.r. .b.e.i. .d
+00007ec0: 0065 0072 0020 0056 0065 0072 00f6 0066  .e.r. .V.e.r...f
+00007ed0: 0066 0065 006e 0074 006c 0069 0063 0068  .f.e.n.t.l.i.c.h
+00007ee0: 0075 006e 0067 0020 0064 0065 0073 0020  .u.n.g. .d.e.s. 
+00007ef0: 0042 0069 006c 0064 0065 0073 0020 0067  .B.i.l.d.e.s. .g
+00007f00: 0065 006e 0061 006e 006e 0074 0020 0077  .e.n.a.n.n.t. .w
+00007f10: 0065 0072 0064 0065 006e 0020 0073 006f  .e.r.d.e.n. .s.o
+00007f20: 006c 006c 002e 0800 0000 0006 0000 003a  .l.l...........:
+00007f30: 456e 7465 7220 7768 6f20 7368 6f75 6c64  Enter who should
+00007f40: 2062 6520 6372 6564 6974 6564 2077 6865   be credited whe
+00007f50: 6e20 7468 6973 2069 6d61 6765 2069 7320  n this image is 
+00007f60: 7075 626c 6973 6865 642e 0700 0000 084f  published......O
+00007f70: 776e 6572 5461 6201 0300 0000 2c00 5600  wnerTab.....,.V.
+00007f80: 6f00 7200 6c00 6100 6700 6500 2000 6900  o.r.l.a.g.e. .i.
+00007f90: 6e00 6900 7400 6900 6100 6c00 6900 7300  n.i.t.i.a.l.i.s.
+00007fa0: 6900 6500 7200 6500 6e08 0000 0000 0600  i.e.r.e.n.......
+00007fb0: 0000 1349 6e69 7469 616c 6973 6520 7465  ...Initialise te
+00007fc0: 6d70 6c61 7465 0700 0000 084f 776e 6572  mplate.....Owner
+00007fd0: 5461 6201 0300 0000 1600 4100 6e00 7700  Tab.......A.n.w.
+00007fe0: 6500 6900 7300 7500 6e00 6700 6500 6e08  e.i.s.u.n.g.e.n.
+00007ff0: 0000 0000 0600 0000 0c49 6e73 7472 7563  .........Instruc
+00008000: 7469 6f6e 7307 0000 0008 4f77 6e65 7254  tions.....OwnerT
+00008010: 6162 0103 0000 0008 004e 0061 006d 0065  ab.......N.a.m.e
+00008020: 0800 0000 0006 0000 0004 4e61 6d65 0700  ..........Name..
+00008030: 0000 084f 776e 6572 5461 6201 0300 0000  ...OwnerTab.....
+00008040: 3400 4c00 6900 6e00 6b00 2000 7a00 7500  4.L.i.n.k. .z.u.
+00008050: 2020 1e00 7b00 6c00 6900 6300 6500 6e00    ..{.l.i.c.e.n.
+00008060: 6300 6500 7d20 1c00 2000 f600 6600 6600  c.e.} .. ...f.f.
+00008070: 6e00 6500 6e08 0000 0000 0600 0000 184f  n.e.n..........O
+00008080: 7065 6e20 6c69 6e6b 2074 6f20 227b 6c69  pen link to "{li
+00008090: 6365 6e63 657d 2207 0000 0008 4f77 6e65  cence}".....Owne
+000080a0: 7254 6162 0103 0000 0014 0054 0065 006c  rTab.......T.e.l
+000080b0: 0065 0066 006f 006e 0028 0065 0029 0800  .e.f.o.n.(.e.)..
+000080c0: 0000 0006 0000 0008 5068 6f6e 6528 7329  ........Phone(s)
+000080d0: 0700 0000 084f 776e 6572 5461 6201 0300  .....OwnerTab...
+000080e0: 0000 3200 5000 6800 6f00 7400 6900 6e00  ..2.P.h.o.t.i.n.
+000080f0: 6900 3a00 2000 4500 6900 6700 6500 6e00  i.:. .E.i.g.e.n.
+00008100: 7400 7500 6d00 7300 7600 6f00 7200 6c00  t.u.m.s.v.o.r.l.
+00008110: 6100 6700 6508 0000 0000 0600 0000 1b50  a.g.e..........P
+00008120: 686f 7469 6e69 3a20 6f77 6e65 7273 6869  hotini: ownershi
+00008130: 7020 7465 6d70 6c61 7465 0700 0000 084f  p template.....O
+00008140: 776e 6572 5461 6201 0300 0000 1800 5000  wnerTab.......P.
+00008150: 6f00 7300 7400 6c00 6500 6900 7400 7a00  o.s.t.l.e.i.t.z.
+00008160: 6100 6800 6c08 0000 0000 0600 0000 0b50  a.h.l..........P
+00008170: 6f73 7461 6c20 436f 6465 0700 0000 084f  ostal Code.....O
+00008180: 776e 6572 5461 6201 0300 0000 2c00 5000  wnerTab.....,.P.
+00008190: 7500 6200 6c00 6900 6300 2000 4400 6f00  u.b.l.i.c. .D.o.
+000081a0: 6d00 6100 6900 6e00 2000 4d00 6100 7200  m.a.i.n. .M.a.r.
+000081b0: 6b00 2000 3100 2e00 3008 0000 0000 0600  k. .1...0.......
+000081c0: 0000 1650 7562 6c69 6320 446f 6d61 696e  ...Public Domain
+000081d0: 204d 6172 6b20 312e 3007 0000 0008 4f77   Mark 1.0.....Ow
+000081e0: 6e65 7254 6162 0103 0000 000c 0052 0065  nerTab.......R.e
+000081f0: 0063 0068 0074 0065 0800 0000 0006 0000  .c.h.t.e........
+00008200: 0006 5269 6768 7473 0700 0000 084f 776e  ..Rights.....Own
+00008210: 6572 5461 6201 0300 0000 1a00 5300 7400  erTab.......S.t.
+00008220: 6100 6100 7400 2f00 5000 7200 6f00 7600  a.a.t./.P.r.o.v.
+00008230: 6900 6e00 7a08 0000 0000 0600 0000 0e53  i.n.z..........S
+00008240: 7461 7465 2f50 726f 7669 6e63 6507 0000  tate/Province...
+00008250: 0008 4f77 6e65 7254 6162 0103 0000 0006  ..OwnerTab......
+00008260: 0055 0052 004c 0800 0000 0006 0000 0003  .U.R.L..........
+00008270: 5552 4c07 0000 0008 4f77 6e65 7254 6162  URL.....OwnerTab
+00008280: 0103 0000 0026 004e 0075 0074 007a 0075  .....&.N.u.t.z.u
+00008290: 006e 0067 0073 0062 0065 0064 0069 006e  .n.g.s.b.e.d.i.n
+000082a0: 0067 0075 006e 0067 0065 006e 0800 0000  .g.u.n.g.e.n....
+000082b0: 0006 0000 000b 5573 6167 6520 5465 726d  ......Usage Term
+000082c0: 7307 0000 0008 4f77 6e65 7254 6162 0103  s.....OwnerTab..
+000082d0: 0000 0098 0056 0065 0072 0077 0065 006e  .....V.e.r.w.e.n
+000082e0: 0064 0065 006e 0020 0053 0069 0065 0020  .d.e.n. .S.i.e. 
+000082f0: 0025 0059 002c 0020 0075 006d 0020 0064  .%.Y.,. .u.m. .d
+00008300: 0061 0073 0020 004a 0061 0068 0072 0020  .a.s. .J.a.h.r. 
+00008310: 0065 0069 006e 007a 0075 0066 00fc 0067  .e.i.n.z.u.f...g
+00008320: 0065 006e 002c 0020 0069 006e 0020 0064  .e.n.,. .i.n. .d
+00008330: 0065 006d 0020 0064 0061 0073 0020 0046  .e.m. .d.a.s. .F
+00008340: 006f 0074 006f 0020 0061 0075 0066 0067  .o.t.o. .a.u.f.g
+00008350: 0065 006e 006f 006d 006d 0065 006e 0020  .e.n.o.m.m.e.n. 
+00008360: 0077 0075 0072 0064 0065 002e 0800 0000  .w.u.r.d.e......
+00008370: 0006 0000 0033 5573 6520 2559 2074 6f20  .....3Use %Y to 
+00008380: 696e 7365 7274 2074 6865 2079 6561 7220  insert the year 
+00008390: 7468 6520 7068 6f74 6f67 7261 7068 2077  the photograph w
+000083a0: 6173 2074 616b 656e 2e07 0000 0008 4f77  as taken......Ow
+000083b0: 6e65 7254 6162 0103 0000 001a 0057 0065  nerTab.......W.e
+000083c0: 0062 002d 0045 0072 006b 006c 00e4 0072  .b.-.E.r.k.l...r
+000083d0: 0075 006e 0067 0800 0000 0006 0000 000d  .u.n.g..........
+000083e0: 5765 6220 5374 6174 656d 656e 7407 0000  Web Statement...
+000083f0: 0008 4f77 6e65 7254 6162 0103 0000 0014  ..OwnerTab......
+00008400: 0057 0065 0062 002d 0055 0052 004c 0028  .W.e.b.-.U.R.L.(
+00008410: 0073 0029 0800 0000 0006 0000 000a 5765  .s.)..........We
+00008420: 6220 5552 4c28 7329 0700 0000 084f 776e  b URL(s).....Own
+00008430: 6572 5461 6201 0300 0000 1800 3c00 4e00  erTab.......<.N.
+00008440: 6500 7500 6500 2000 5300 7500 6300 6800  e.u.e. .S.u.c.h.
+00008450: 6500 3e08 0000 0000 0600 0000 0c3c 6e65  e.>..........<ne
+00008460: 7720 7365 6172 6368 3e07 0000 000a 5068  w search>.....Ph
+00008470: 6f74 696e 694d 6170 0103 0000 0026 003c  otiniMap.....&.<
+00008480: 0053 0075 0063 0068 0065 0020 0077 0069  .S.u.c.h.e. .w.i
+00008490: 0065 0064 0065 0072 0068 006f 006c 0065  .e.d.e.r.h.o.l.e
+000084a0: 006e 003e 0800 0000 0006 0000 000f 3c72  .n.>..........<r
+000084b0: 6570 6561 7420 7365 6172 6368 3e07 0000  epeat search>...
+000084c0: 000a 5068 6f74 696e 694d 6170 0103 0000  ..PhotiniMap....
+000084d0: 001c 003c 0077 0069 0064 0065 006e 0020  ...<.w.i.d.e.n. 
+000084e0: 0073 0065 0061 0072 0063 0068 003e 0800  .s.e.a.r.c.h.>..
+000084f0: 0000 0006 0000 000e 3c77 6964 656e 2073  ........<widen s
+00008500: 6561 7263 683e 0700 0000 0a50 686f 7469  earch>.....Photi
+00008510: 6e69 4d61 7001 0300 0000 0800 4800 f600  niMap.......H...
+00008520: 6800 6508 0000 0000 0600 0000 0841 6c74  h.e..........Alt
+00008530: 6974 7564 6507 0000 000a 5068 6f74 696e  itude.....Photin
+00008540: 694d 6170 0103 0000 0030 0048 00f6 0068  iMap.....0.H...h
+00008550: 0065 0020 0061 0075 0073 0020 004b 0061  .e. .a.u.s. .K.a
+00008560: 0072 0074 0065 0020 0065 0072 006d 0069  .r.t.e. .e.r.m.i
+00008570: 0074 0074 0065 006c 006e 0800 0000 0006  .t.t.e.l.n......
+00008580: 0000 0015 4765 7420 616c 7469 7475 6465  ....Get altitude
+00008590: 2066 726f 6d20 6d61 7007 0000 000a 5068   from map.....Ph
+000085a0: 6f74 696e 694d 6170 0103 0000 001e 0047  otiniMap.......G
+000085b0: 0050 0058 002d 0044 0061 0074 0065 0069  .P.X.-.D.a.t.e.i
+000085c0: 0020 006c 0061 0064 0065 006e 0800 0000  . .l.a.d.e.n....
+000085d0: 0006 0000 000d 4c6f 6164 2047 5058 2066  ......Load GPX f
+000085e0: 696c 6507 0000 000a 5068 6f74 696e 694d  ile.....PhotiniM
+000085f0: 6170 0103 0000 0026 0047 0050 0058 002d  ap.....&.G.P.X.-
+00008600: 0044 0061 0074 0065 006e 0020 0065 006e  .D.a.t.e.n. .e.n
+00008610: 0074 0066 0065 0072 006e 0065 006e 0800  .t.f.e.r.n.e.n..
+00008620: 0000 0006 0000 000f 5265 6d6f 7665 2047  ........Remove G
+00008630: 5058 2064 6174 6107 0000 000a 5068 6f74  PX data.....Phot
+00008640: 696e 694d 6170 0103 0000 000a 0053 0075  iniMap.......S.u
+00008650: 0063 0068 0065 0800 0000 0006 0000 0006  .c.h.e..........
+00008660: 5365 6172 6368 0700 0000 0a50 686f 7469  Search.....Photi
+00008670: 6e69 4d61 7001 0300 0000 3a00 4b00 6f00  niMap.....:.K.o.
+00008680: 6f00 7200 6400 6900 6e00 6100 7400 6500  o.r.d.i.n.a.t.e.
+00008690: 6e00 2000 6100 7500 7300 2000 4700 5000  n. .a.u.s. .G.P.
+000086a0: 5800 2000 6600 6500 7300 7400 6c00 6500  X. .f.e.s.t.l.e.
+000086b0: 6700 6500 6e08 0000 0000 0600 0000 1353  g.e.n..........S
+000086c0: 6574 2063 6f6f 7264 7320 6672 6f6d 2047  et coords from G
+000086d0: 5058 0700 0000 0a50 686f 7469 6e69 4d61  PX.....PhotiniMa
+000086e0: 7001 0300 0000 3000 5a00 7500 2000 5300  p.....0.Z.u. .S.
+000086f0: 6100 6d00 6d00 6c00 7500 6e00 6700 6500  a.m.m.l.u.n.g.e.
+00008700: 6e00 2000 6800 6900 6e00 7a00 7500 6600  n. .h.i.n.z.u.f.
+00008710: fc00 6700 6500 6e08 0000 0000 0600 0000  ..g.e.n.........
+00008720: 1241 6464 2074 6f20 636f 6c6c 6563 7469  .Add to collecti
+00008730: 6f6e 7307 0000 000b 5069 7865 6c66 6564  ons.....Pixelfed
+00008740: 5461 6201 0300 0000 2e00 4100 6c00 6c00  Tab.......A.l.l.
+00008750: 6500 2000 5200 6500 6300 6800 7400 6500  e. .R.e.c.h.t.e.
+00008760: 2000 5600 6f00 7200 6200 6500 6800 6100   .V.o.r.b.e.h.a.
+00008770: 6c00 7400 6500 6e08 0000 0000 0600 0000  l.t.e.n.........
+00008780: 1341 6c6c 2052 6967 6874 7320 5265 7365  .All Rights Rese
+00008790: 7276 6564 0700 0000 0b50 6978 656c 6665  rved.....Pixelfe
+000087a0: 6454 6162 0103 0000 001a 004e 0061 006d  dTab.......N.a.m
+000087b0: 0065 006e 0073 006e 0065 006e 006e 0075  .e.n.s.n.e.n.n.u
+000087c0: 006e 0067 0800 0000 0006 0000 000b 4174  .n.g..........At
+000087d0: 7472 6962 7574 696f 6e07 0000 000b 5069  tribution.....Pi
+000087e0: 7865 6c66 6564 5461 6201 0300 0000 2000  xelfedTab..... .
+000087f0: 4200 6900 6c00 6400 7500 6e00 7400 6500  B.i.l.d.u.n.t.e.
+00008800: 7200 7300 6300 6800 7200 6900 6600 7408  r.s.c.h.r.i.f.t.
+00008810: 0000 0000 0600 0000 0743 6170 7469 6f6e  .........Caption
+00008820: 0700 0000 0b50 6978 656c 6665 6454 6162  .....PixelfedTab
+00008830: 0103 0000 0036 0057 00e4 0068 006c 0065  .....6.W...h.l.e
+00008840: 006e 0020 0053 0069 0065 0020 0065 0069  .n. .S.i.e. .e.i
+00008850: 006e 0065 0020 0049 006e 0073 0074 0061  .n.e. .I.n.s.t.a
+00008860: 006e 007a 0020 0061 0075 0073 0800 0000  .n.z. .a.u.s....
+00008870: 0006 0000 0012 4368 6f6f 7365 2061 6e20  ......Choose an 
+00008880: 696e 7374 616e 6365 0700 0000 0b50 6978  instance.....Pix
+00008890: 656c 6665 6454 6162 0103 0000 0032 0053  elfedTab.....2.S
+000088a0: 0069 0063 0068 0074 0062 0061 0072 006b  .i.c.h.t.b.a.r.k
+000088b0: 0065 0069 0074 0020 0064 0065 0072 0020  .e.i.t. .d.e.r. 
+000088c0: 0053 0061 006d 006d 006c 0075 006e 0067  .S.a.m.m.l.u.n.g
+000088d0: 0800 0000 0006 0000 0015 436f 6c6c 6563  ..........Collec
+000088e0: 7469 6f6e 2076 6973 6962 696c 6974 7907  tion visibility.
+000088f0: 0000 000b 5069 7865 6c66 6564 5461 6201  ....PixelfedTab.
+00008900: 0300 0000 2e00 4e00 6500 7500 6500 2000  ......N.e.u.e. .
+00008910: 5300 6100 6d00 6d00 6c00 7500 6e00 6700  S.a.m.m.l.u.n.g.
+00008920: 2000 6500 7200 7300 7400 6500 6c00 6c00   .e.r.s.t.e.l.l.
+00008930: 6500 6e08 0000 0000 0600 0000 1543 7265  e.n..........Cre
+00008940: 6174 6520 6e65 7720 636f 6c6c 6563 7469  ate new collecti
+00008950: 6f6e 0700 0000 0b50 6978 656c 6665 6454  on.....PixelfedT
+00008960: 6162 0103 0000 0018 0042 0065 0073 0063  ab.......B.e.s.c
+00008970: 0068 0072 0065 0069 0062 0075 006e 0067  .h.r.e.i.b.u.n.g
+00008980: 0800 0000 0006 0000 000b 4465 7363 7269  ..........Descri
+00008990: 7074 696f 6e07 0000 000b 5069 7865 6c66  ption.....Pixelf
+000089a0: 6564 5461 6201 0300 0000 2e00 4b00 6f00  edTab.......K.o.
+000089b0: 6d00 6d00 6500 6e00 7400 6100 7200 6500  m.m.e.n.t.a.r.e.
+000089c0: 2000 6400 6500 6100 6b00 7400 6900 7600   .d.e.a.k.t.i.v.
+000089d0: 6900 6500 7200 6500 6e08 0000 0000 0600  i.e.r.e.n.......
+000089e0: 0000 1044 6973 6162 6c65 2063 6f6d 6d65  ...Disable comme
+000089f0: 6e74 7307 0000 000b 5069 7865 6c66 6564  nts.....Pixelfed
+00008a00: 5461 6201 0300 0000 0e00 4500 6e00 7400  Tab.......E.n.t.
+00008a10: 7700 7500 7200 6608 0000 0000 0600 0000  w.u.r.f.........
+00008a20: 0544 7261 6674 0700 0000 0b50 6978 656c  .Draft.....Pixel
+00008a30: 6665 6454 6162 0103 0000 0014 004e 0075  fedTab.......N.u
+00008a40: 0072 0020 0046 006f 006c 0067 0065 0072  .r. .F.o.l.g.e.r
+00008a50: 0800 0000 0006 0000 000e 466f 6c6c 6f77  ..........Follow
+00008a60: 6572 7320 6f6e 6c79 0700 0000 0b50 6978  ers only.....Pix
+00008a70: 656c 6665 6454 6162 0103 0000 0014 0047  elfedTab.......G
+00008a80: 0065 006e 0065 0072 0069 0065 0072 0065  .e.n.e.r.i.e.r.e
+00008a90: 006e 0800 0000 0006 0000 0008 4765 6e65  .n..........Gene
+00008aa0: 7261 7465 0700 0000 0b50 6978 656c 6665  rate.....Pixelfe
+00008ab0: 6454 6162 0103 0000 000c 004c 0069 007a  dTab.......L.i.z
+00008ac0: 0065 006e 007a 0800 0000 0006 0000 0007  .e.n.z..........
+00008ad0: 4c69 6365 6e63 6507 0000 000b 5069 7865  Licence.....Pixe
+00008ae0: 6c66 6564 5461 6201 0300 0000 2800 4600  lfedTab.....(.F.
+00008af0: 6500 6800 6c00 6500 6e00 6400 6500 7200  e.h.l.e.n.d.e.r.
+00008b00: 2000 6100 6c00 7400 2e00 2000 5400 6500   .a.l.t... .T.e.
+00008b10: 7800 7400 2e08 0000 0000 0600 0000 114d  x.t............M
+00008b20: 6973 7369 6e67 2061 6c74 2074 6578 742e  issing alt text.
+00008b30: 0700 0000 0b50 6978 656c 6665 6454 6162  .....PixelfedTab
+00008b40: 0103 0000 001a 004e 0065 0075 0065 0020  .......N.e.u.e. 
+00008b50: 0053 0061 006d 006d 006c 0075 006e 0067  .S.a.m.m.l.u.n.g
+00008b60: 0800 0000 0006 0000 000e 4e65 7720 636f  ..........New co
+00008b70: 6c6c 6563 7469 6f6e 0700 0000 0b50 6978  llection.....Pix
+00008b80: 656c 6665 6454 6162 0103 0000 000c 0041  elfedTab.......A
+00008b90: 006e 0064 0065 0072 0065 0800 0000 0006  .n.d.e.r.e......
+00008ba0: 0000 0005 4f74 6865 7207 0000 000b 5069  ....Other.....Pi
+00008bb0: 7865 6c66 6564 5461 6201 0300 0000 2400  xelfedTab.....$.
+00008bc0: 5000 6800 6f00 7400 6900 6e00 6900 3a00  P.h.o.t.i.n.i.:.
+00008bd0: 2000 6100 6c00 7400 2e00 2000 5400 6500   .a.l.t... .T.e.
+00008be0: 7800 7408 0000 0000 0600 0000 1150 686f  x.t..........Pho
+00008bf0: 7469 6e69 3a20 616c 7420 7465 7874 0700  tini: alt text..
+00008c00: 0000 0b50 6978 656c 6665 6454 6162 0103  ...PixelfedTab..
+00008c10: 0000 0034 0050 0068 006f 0074 0069 006e  ...4.P.h.o.t.i.n
+00008c20: 0069 003a 0020 0049 006e 0073 0074 0061  .i.:. .I.n.s.t.a
+00008c30: 006e 007a 0020 0061 0075 0073 0077 00e4  .n.z. .a.u.s.w..
+00008c40: 0068 006c 0065 006e 0800 0000 0006 0000  .h.l.e.n........
+00008c50: 0018 5068 6f74 696e 693a 2063 686f 6f73  ..Photini: choos
+00008c60: 6520 696e 7374 616e 6365 0700 0000 0b50  e instance.....P
+00008c70: 6978 656c 6665 6454 6162 0103 0000 0032  ixelfedTab.....2
+00008c80: 0053 0069 0063 0068 0074 0062 0061 0072  .S.i.c.h.t.b.a.r
+00008c90: 006b 0065 0069 0074 0020 0064 0065 0073  .k.e.i.t. .d.e.s
+00008ca0: 0020 0042 0065 0069 0074 0072 0061 0067  . .B.e.i.t.r.a.g
+00008cb0: 0073 0800 0000 0006 0000 000f 506f 7374  .s..........Post
+00008cc0: 2076 6973 6962 696c 6974 7907 0000 000b   visibility.....
+00008cd0: 5069 7865 6c66 6564 5461 6201 0300 0000  PixelfedTab.....
+00008ce0: 1400 d600 6600 6600 6500 6e00 7400 6c00  ....f.f.e.n.t.l.
+00008cf0: 6900 6300 6808 0000 0000 0600 0000 0650  i.c.h..........P
+00008d00: 7562 6c69 6307 0000 000b 5069 7865 6c66  ublic.....Pixelf
+00008d10: 6564 5461 6201 0300 0000 3200 4700 6500  edTab.....2.G.e.
+00008d20: 6d00 6500 6900 6e00 6600 7200 6500 6900  m.e.i.n.f.r.e.i.
+00008d30: 6500 2000 5700 6900 6400 6d00 7500 6e00  e. .W.i.d.m.u.n.
+00008d40: 6700 2000 2800 4300 4300 3000 2908 0000  g. .(.C.C.0.)...
+00008d50: 0000 0600 0000 1e50 7562 6c69 6320 446f  .......Public Do
+00008d60: 6d61 696e 2044 6564 6963 6174 696f 6e20  main Dedication 
+00008d70: 2843 4330 2907 0000 000b 5069 7865 6c66  (CC0).....Pixelf
+00008d80: 6564 5461 6201 0300 0000 2400 4700 6500  edTab.....$.G.e.
+00008d90: 6d00 6500 6900 6e00 6600 7200 6500 6900  m.e.i.n.f.r.e.i.
+00008da0: 6500 2000 4100 7200 6200 6500 6900 7408  e. .A.r.b.e.i.t.
+00008db0: 0000 0000 0600 0000 1250 7562 6c69 6320  .........Public 
+00008dc0: 446f 6d61 696e 2057 6f72 6b07 0000 000b  Domain Work.....
+00008dd0: 5069 7865 6c66 6564 5461 6201 0300 0000  PixelfedTab.....
+00008de0: 2a00 5600 6500 7200 7400 7200 6100 7500  *.V.e.r.t.r.a.u.
+00008df0: 6c00 6900 6300 6800 6500 7200 2000 4200  l.i.c.h.e.r. .B.
+00008e00: 6500 6900 7400 7200 6100 6708 0000 0000  e.i.t.r.a.g.....
+00008e10: 0600 0000 0e53 656e 7369 7469 7665 2070  .....Sensitive p
+00008e20: 6f73 7407 0000 000b 5069 7865 6c66 6564  ost.....Pixelfed
+00008e30: 5461 6201 0300 0000 0a00 5400 6900 7400  Tab.......T.i.t.
+00008e40: 6500 6c08 0000 0000 0600 0000 0554 6974  e.l..........Tit
+00008e50: 6c65 0700 0000 0b50 6978 656c 6665 6454  le.....PixelfedT
+00008e60: 6162 0103 0000 0014 0055 006e 0067 0065  ab.......U.n.g.e
+00008e70: 006c 0069 0073 0074 0065 0074 0800 0000  .l.i.s.t.e.t....
+00008e80: 0006 0000 0008 556e 6c69 7374 6564 0700  ......Unlisted..
+00008e90: 0000 0b50 6978 656c 6665 6454 6162 0103  ...PixelfedTab..
+00008ea0: 0000 0014 0049 006e 0068 0061 006c 0074  .....I.n.h.a.l.t
+00008eb0: 0073 0074 0079 0070 0800 0000 0006 0000  .s.t.y.p........
+00008ec0: 000c 436f 6e74 656e 7420 7479 7065 0700  ..Content type..
+00008ed0: 0000 0a52 6567 696f 6e73 5461 6201 0300  ...RegionsTab...
+00008ee0: 0000 1c00 5200 6500 6700 6900 6f00 6e00  ....R.e.g.i.o.n.
+00008ef0: 2000 6c00 f600 7300 6300 6800 6500 6e08   .l...s.c.h.e.n.
+00008f00: 0000 0000 0600 0000 0d44 656c 6574 6520  .........Delete 
+00008f10: 7265 6769 6f6e 0700 0000 0a52 6567 696f  region.....Regio
+00008f20: 6e73 5461 6201 0300 0000 2000 4500 6300  nsTab..... .E.c.
+00008f30: 6b00 7000 7500 6e00 6b00 7400 2000 6c00  k.p.u.n.k.t. .l.
+00008f40: f600 7300 6300 6800 6500 6e08 0000 0000  ..s.c.h.e.n.....
+00008f50: 0600 0000 0d44 656c 6574 6520 7665 7274  .....Delete vert
+00008f60: 6578 0700 0000 0a52 6567 696f 6e73 5461  ex.....RegionsTa
+00008f70: 6201 0300 0000 1800 4200 6500 7300 6300  b.......B.e.s.c.
+00008f80: 6800 7200 6500 6900 6200 7500 6e00 6708  h.r.e.i.b.u.n.g.
+00008f90: 0000 0000 0600 0000 0b44 6573 6372 6970  .........Descrip
+00008fa0: 7469 6f6e 0700 0000 0a52 6567 696f 6e73  tion.....Regions
+00008fb0: 5461 6201 0300 0000 ac00 4600 7200 6500  Tab.......F.r.e.
+00008fc0: 6900 7400 6500 7800 7400 2d00 4e00 6100  i.t.e.x.t.-.N.a.
+00008fd0: 6d00 6500 2000 6400 6500 7200 2000 5200  m.e. .d.e.r. .R.
+00008fe0: 6500 6700 6900 6f00 6e00 2e00 2000 5300  e.g.i.o.n... .S.
+00008ff0: 6f00 6c00 6c00 7400 6500 2000 7500 6e00  o.l.l.t.e. .u.n.
+00009000: 7400 6500 7200 2000 6100 6c00 6c00 6500  t.e.r. .a.l.l.e.
+00009010: 6e00 2000 5200 6500 6700 6900 6f00 6e00  n. .R.e.g.i.o.n.
+00009020: 7300 6e00 6100 6d00 6500 6e00 2000 6500  s.n.a.m.e.n. .e.
+00009030: 6900 6e00 6500 7300 2000 4200 6900 6c00  i.n.e.s. .B.i.l.
+00009040: 6400 6500 7300 2000 6500 6900 6e00 6400  d.e.s. .e.i.n.d.
+00009050: 6500 7500 7400 6900 6700 2000 7300 6500  e.u.t.i.g. .s.e.
+00009060: 6900 6e00 2e08 0000 0000 0600 0000 5246  i.n...........RF
+00009070: 7265 652d 7465 7874 206e 616d 6520 6f66  ree-text name of
+00009080: 2074 6865 2072 6567 696f 6e2e 2053 686f   the region. Sho
+00009090: 756c 6420 6265 2075 6e69 7175 6520 616d  uld be unique am
+000090a0: 6f6e 6720 616c 6c20 5265 6769 6f6e 204e  ong all Region N
+000090b0: 616d 6573 206f 6620 616e 2069 6d61 6765  ames of an image
+000090c0: 2e07 0000 000a 5265 6769 6f6e 7354 6162  ......RegionsTab
+000090d0: 0103 0000 001a 0042 0069 006c 0064 0026  .......B.i.l.d.&
+000090e0: 0072 0065 0067 0069 006f 006e 0065 006e  .r.e.g.i.o.n.e.n
+000090f0: 0800 0000 0006 0000 000e 496d 6167 6520  ..........Image 
+00009100: 2652 6567 696f 6e73 0700 0000 0a52 6567  &Regions.....Reg
+00009110: 696f 6e73 5461 6201 0300 0000 0800 4e00  ionsTab.......N.
+00009120: 6100 6d00 6508 0000 0000 0600 0000 044e  a.m.e..........N
+00009130: 616d 6507 0000 000a 5265 6769 6f6e 7354  ame.....RegionsT
+00009140: 6162 0103 0000 0016 004e 0065 0075 0065  ab.......N.e.u.e
+00009150: 0072 0020 004b 0072 0065 0069 0073 0800  .r. .K.r.e.i.s..
+00009160: 0000 0006 0000 000a 4e65 7720 6369 7263  ........New circ
+00009170: 6c65 0700 0000 0a52 6567 696f 6e73 5461  le.....RegionsTa
+00009180: 6201 0300 0000 1600 4e00 6500 7500 6500  b.......N.e.u.e.
+00009190: 7200 2000 5000 7500 6e00 6b00 7408 0000  r. .P.u.n.k.t...
+000091a0: 0000 0600 0000 094e 6577 2070 6f69 6e74  .......New point
+000091b0: 0700 0000 0a52 6567 696f 6e73 5461 6201  .....RegionsTab.
+000091c0: 0300 0000 1a00 4e00 6500 7500 6500 7300  ......N.e.u.e.s.
+000091d0: 2000 5000 6f00 6c00 7900 6700 6f00 6e08   .P.o.l.y.g.o.n.
+000091e0: 0000 0000 0600 0000 0b4e 6577 2070 6f6c  .........New pol
+000091f0: 7967 6f6e 0700 0000 0a52 6567 696f 6e73  ygon.....Regions
+00009200: 5461 6201 0300 0000 1c00 4e00 6500 7500  Tab.......N.e.u.
+00009210: 6500 7300 2000 5200 6500 6300 6800 7400  e.s. .R.e.c.h.t.
+00009220: 6500 6300 6b08 0000 0000 0600 0000 0d4e  e.c.k..........N
+00009230: 6577 2072 6563 7461 6e67 6c65 0700 0000  ew rectangle....
+00009240: 0a52 6567 696f 6e73 5461 6201 0300 0000  .RegionsTab.....
+00009250: 1c00 4e00 6500 7500 6500 7200 2000 4500  ..N.e.u.e.r. .E.
+00009260: 6300 6b00 7000 7500 6e00 6b00 7408 0000  c.k.p.u.n.k.t...
+00009270: 0000 0600 0000 0a4e 6577 2076 6572 7465  .......New verte
+00009280: 7807 0000 000a 5265 6769 6f6e 7354 6162  x.....RegionsTab
+00009290: 0103 0000 0024 0041 0062 0067 0065 0062  .....$.A.b.g.e.b
+000092a0: 0069 006c 0064 0065 0074 0065 0020 0050  .i.l.d.e.t.e. .P
+000092b0: 0065 0072 0073 006f 006e 0800 0000 0006  .e.r.s.o.n......
+000092c0: 0000 000c 5065 7273 6f6e 2073 686f 776e  ....Person shown
+000092d0: 0700 0000 0a52 6567 696f 6e73 5461 6201  .....RegionsTab.
+000092e0: 0300 0000 0a00 5200 6f00 6c00 6c00 6508  ......R.o.l.l.e.
+000092f0: 0000 0000 0600 0000 0452 6f6c 6507 0000  .........Role...
+00009300: 000a 5265 6769 6f6e 7354 6162 0103 0000  ..RegionsTab....
+00009310: 002a 0055 006e 006c 0065 0073 0062 0061  .*.U.n.l.e.s.b.a
+00009320: 0072 0065 0073 0020 0042 0069 006c 0064  .r.e.s. .B.i.l.d
+00009330: 0066 006f 0072 006d 0061 0074 0800 0000  .f.o.r.m.a.t....
+00009340: 0006 0000 0017 556e 7265 6164 6162 6c65  ......Unreadable
+00009350: 2069 6d61 6765 2066 6f72 6d61 7407 0000   image format...
+00009360: 000a 5265 6769 6f6e 7354 6162 0103 0000  ..RegionsTab....
+00009370: 000a 0050 0069 0078 0065 006c 0800 0000  ...P.i.x.e.l....
+00009380: 0006 0000 0005 7069 7865 6c07 0000 000a  ......pixel.....
+00009390: 5265 6769 6f6e 7354 6162 0103 0000 000e  RegionsTab......
+000093a0: 0072 0065 006c 0061 0074 0069 0076 0800  .r.e.l.a.t.i.v..
+000093b0: 0000 0006 0000 0008 7265 6c61 7469 7665  ........relative
+000093c0: 0700 0000 0a52 6567 696f 6e73 5461 6201  .....RegionsTab.
+000093d0: 0300 0000 2a00 2600 5400 6500 6300 6800  ....*.&.T.e.c.h.
+000093e0: 6e00 6900 7300 6300 6800 6500 2000 4d00  n.i.s.c.h.e. .M.
+000093f0: 6500 7400 6100 6400 6100 7400 6500 6e08  e.t.a.d.a.t.e.n.
+00009400: 0000 0000 0600 0000 1326 5465 6368 6e69  .........&Techni
+00009410: 6361 6c20 6d65 7461 6461 7461 0700 0000  cal metadata....
+00009420: 0c54 6563 686e 6963 616c 5461 6201 0300  .TechnicalTab...
+00009430: 0000 1400 3300 3500 6d00 6d00 2000 6500  ....3.5.m.m. .e.
+00009440: 7100 7500 6900 7608 0000 0000 0600 0000  q.u.i.v.........
+00009450: 0a33 356d 6d20 6571 7569 7607 0000 000c  .35mm equiv.....
+00009460: 5465 6368 6e69 6361 6c54 6162 0103 0000  TechnicalTab....
+00009470: 0066 0042 006c 0065 006e 0064 0065 0020  .f.B.l.e.n.d.e. 
+00009480: 0075 006e 0064 0020 0042 0072 0065 006e  .u.n.d. .B.r.e.n
+00009490: 006e 0077 0065 0069 0074 0065 0020 0061  .n.w.e.i.t.e. .a
+000094a0: 0075 0073 0020 004f 0062 006a 0065 006b  .u.s. .O.b.j.e.k
+000094b0: 0074 0069 0076 0064 0061 0074 0065 006e  .t.i.v.d.a.t.e.n
+000094c0: 0020 00fc 0062 0065 0072 006e 0065 0068  . ...b.e.r.n.e.h
+000094d0: 006d 0065 006e 003f 0800 0000 0006 0000  .m.e.n.?........
+000094e0: 0048 4164 6a75 7374 2069 6d61 6765 2061  .HAdjust image a
+000094f0: 7065 7274 7572 6520 616e 6420 666f 6361  perture and foca
+00009500: 6c20 6c65 6e67 7468 2074 6f20 6167 7265  l length to agre
+00009510: 6520 7769 7468 206c 656e 7320 7370 6563  e with lens spec
+00009520: 6966 6963 6174 696f 6e3f 0700 0000 0c54  ification?.....T
+00009530: 6563 686e 6963 616c 5461 6201 0300 0000  echnicalTab.....
+00009540: 2400 5500 6800 7200 7a00 6500 6900 7400  $.U.h.r.z.e.i.t.
+00009550: 6500 6e00 2000 6100 6e00 7000 6100 7300  e.n. .a.n.p.a.s.
+00009560: 7300 6500 6e08 0000 0000 0600 0000 0c41  s.e.n..........A
+00009570: 646a 7573 7420 7469 6d65 7307 0000 000c  djust times.....
+00009580: 5465 6368 6e69 6361 6c54 6162 0103 0000  TechnicalTab....
+00009590: 000c 0042 006c 0065 006e 0064 0065 0800  ...B.l.e.n.d.e..
+000095a0: 0000 0006 0000 0008 4170 6572 7475 7265  ........Aperture
+000095b0: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
+000095c0: 6201 0300 0000 3400 4200 6c00 6500 6e00  b.....4.B.l.e.n.
+000095d0: 6400 6500 2000 6200 6500 6900 2000 6d00  d.e. .b.e.i. .m.
+000095e0: 6100 7800 2e00 2000 4200 7200 6500 6e00  a.x... .B.r.e.n.
+000095f0: 6e00 7700 6500 6900 7400 6508 0000 0000  n.w.e.i.t.e.....
+00009600: 0600 0000 1d41 7065 7274 7572 6520 6174  .....Aperture at
+00009610: 206d 6178 2e20 666f 6361 6c20 6c65 6e67   max. focal leng
+00009620: 7468 0700 0000 0c54 6563 686e 6963 616c  th.....Technical
+00009630: 5461 6201 0300 0000 3400 4200 6c00 6500  Tab.....4.B.l.e.
+00009640: 6e00 6400 6500 2000 6200 6500 6900 2000  n.d.e. .b.e.i. .
+00009650: 6d00 6900 6e00 2e00 2000 4200 7200 6500  m.i.n... .B.r.e.
+00009660: 6e00 6e00 7700 6500 6900 7400 6508 0000  n.n.w.e.i.t.e...
+00009670: 0000 0600 0000 1d41 7065 7274 7572 6520  .......Aperture 
+00009680: 6174 206d 696e 2e20 666f 6361 6c20 6c65  at min. focal le
+00009690: 6e67 7468 0700 0000 0c54 6563 686e 6963  ngth.....Technic
+000096a0: 616c 5461 6201 0300 0000 0c00 4b00 6100  alTab.......K.a.
+000096b0: 6d00 6500 7200 6108 0000 0000 0600 0000  m.e.r.a.........
+000096c0: 0643 616d 6572 6107 0000 000c 5465 6368  .Camera.....Tech
+000096d0: 6e69 6361 6c54 6162 0103 0000 0022 0044  nicalTab.....".D
+000096e0: 0061 0074 0075 006d 0020 0075 006e 0064  .a.t.u.m. .u.n.d
+000096f0: 0020 0055 0068 0072 007a 0065 0069 0074  . .U.h.r.z.e.i.t
+00009700: 0800 0000 0006 0000 000d 4461 7465 2061  ..........Date a
+00009710: 6e64 2074 696d 6507 0000 000c 5465 6368  nd time.....Tech
+00009720: 6e69 6361 6c54 6162 0103 0000 001a 0044  nicalTab.......D
+00009730: 0069 0067 0069 0074 0061 006c 0069 0073  .i.g.i.t.a.l.i.s
+00009740: 0069 0065 0072 0074 0800 0000 0006 0000  .i.e.r.t........
+00009750: 0009 4469 6769 7469 7365 6407 0000 000c  ..Digitised.....
+00009760: 5465 6368 6e69 6361 6c54 6162 0103 0000  TechnicalTab....
+00009770: 0014 0042 0072 0065 006e 006e 0077 0065  ...B.r.e.n.n.w.e
+00009780: 0069 0074 0065 0800 0000 0006 0000 000c  .i.t.e..........
+00009790: 466f 6361 6c20 6c65 6e67 7468 0700 0000  Focal length....
+000097a0: 0c54 6563 686e 6963 616c 5461 6201 0300  .TechnicalTab...
+000097b0: 0000 1800 4c00 6900 6e00 7300 6500 6e00  ....L.i.n.s.e.n.
+000097c0: 6d00 6f00 6400 6500 6c00 6c08 0000 0000  m.o.d.e.l.l.....
+000097d0: 0600 0000 0a4c 656e 7320 6d6f 6465 6c07  .....Lens model.
+000097e0: 0000 000c 5465 6368 6e69 6361 6c54 6162  ....TechnicalTab
+000097f0: 0103 0000 0046 0044 0069 0067 0069 0074  .....F.D.i.g.i.t
+00009800: 0061 006c 0069 0073 0069 0065 0072 0074  .a.l.i.s.i.e.r.t
+00009810: 0020 0075 006e 0064 0020 0056 0065 0072  . .u.n.d. .V.e.r
+00009820: 00e4 006e 0064 0065 0072 0074 0020 006b  ...n.d.e.r.t. .k
+00009830: 006f 0070 0070 0065 006c 006e 0800 0000  .o.p.p.e.l.n....
+00009840: 0006 0000 001f 4c69 6e6b 2027 6469 6769  ......Link 'digi
+00009850: 7469 7365 6427 2061 6e64 2027 6d6f 6469  tised' and 'modi
+00009860: 6669 6564 2707 0000 000c 5465 6368 6e69  fied'.....Techni
+00009870: 6361 6c54 6162 0103 0000 004a 0041 0075  calTab.....J.A.u
+00009880: 0066 0067 0065 006e 006f 006d 006d 0065  .f.g.e.n.o.m.m.e
+00009890: 006e 0020 0075 006e 0064 0020 0044 0069  .n. .u.n.d. .D.i
+000098a0: 0067 0069 0074 0061 006c 0069 0073 0069  .g.i.t.a.l.i.s.i
+000098b0: 0065 0072 0074 0020 006b 006f 0070 0070  .e.r.t. .k.o.p.p
+000098c0: 0065 006c 006e 0800 0000 0006 0000 001c  .e.l.n..........
+000098d0: 4c69 6e6b 2027 7461 6b65 6e27 2061 6e64  Link 'taken' and
+000098e0: 2027 6469 6769 7469 7365 6427 0700 0000   'digitised'....
 000098f0: 0c54 6563 686e 6963 616c 5461 6201 0300  .TechnicalTab...
-00009900: 0000 2600 6f00 6200 6500 6e00 2d00 7500  ..&.o.b.e.n.-.u.
-00009910: 6e00 7400 6500 6e00 2000 7300 7000 6900  n.t.e.n. .s.p.i.
-00009920: 6500 6700 6500 6c00 6e08 0000 0000 0600  e.g.e.l.n.......
-00009930: 0000 1572 6566 6c65 6374 2074 6f70 2074  ...reflect top t
-00009940: 6f20 626f 7474 6f6d 0700 0000 0c54 6563  o bottom.....Tec
-00009950: 686e 6963 616c 5461 6201 0300 0000 3e00  hnicalTab.....>.
-00009960: 3900 3000 2000 4700 7200 6100 6400 2000  9.0. .G.r.a.d. .
-00009970: 6900 6d00 2000 5500 6800 7200 7a00 6500  i.m. .U.h.r.z.e.
-00009980: 6900 6700 6500 7200 7300 6900 6e00 6e00  i.g.e.r.s.i.n.n.
-00009990: 2000 6400 7200 6500 6800 6500 6e08 0000   .d.r.e.h.e.n...
-000099a0: 0000 0600 0000 0c72 6f74 6174 6520 2b39  .......rotate +9
-000099b0: 30c2 b007 0000 000c 5465 6368 6e69 6361  0.......Technica
-000099c0: 6c54 6162 0103 0000 0044 0039 0030 0020  lTab.....D.9.0. 
-000099d0: 0047 0072 0061 0064 0020 0067 0065 0067  .G.r.a.d. .g.e.g
-000099e0: 0065 006e 0020 0055 0068 0072 007a 0065  .e.n. .U.h.r.z.e
-000099f0: 0069 0067 0065 0072 0073 0069 006e 006e  .i.g.e.r.s.i.n.n
-00009a00: 0020 0064 0072 0065 0068 0065 006e 0800  . .d.r.e.h.e.n..
-00009a10: 0000 0006 0000 000c 726f 7461 7465 202d  ........rotate -
-00009a20: 3930 c2b0 0700 0000 0c54 6563 686e 6963  90.......Technic
-00009a30: 616c 5461 6201 0300 0000 4000 3100 3800  alTab.....@.1.8.
-00009a40: 3000 2000 4700 7200 6100 6400 2000 6900  0. .G.r.a.d. .i.
-00009a50: 6d00 2000 5500 6800 7200 7a00 6500 6900  m. .U.h.r.z.e.i.
-00009a60: 6700 6500 7200 7300 6900 6e00 6e00 2000  g.e.r.s.i.n.n. .
-00009a70: 6400 7200 6500 6800 6500 6e08 0000 0000  d.r.e.h.e.n.....
-00009a80: 0600 0000 0c72 6f74 6174 6520 3138 30c2  .....rotate 180.
-00009a90: b007 0000 000c 5465 6368 6e69 6361 6c54  ......TechnicalT
-00009aa0: 6162 0103 0000 0026 005a 0075 0020 0041  ab.....&.Z.u. .A
-00009ab0: 006c 0062 0065 006e 0020 0068 0069 006e  .l.b.e.n. .h.i.n
-00009ac0: 007a 0075 0066 00fc 0067 0065 006e 0800  .z.u.f...g.e.n..
-00009ad0: 0000 0006 0000 000d 4164 6420 746f 2061  ........Add to a
-00009ae0: 6c62 756d 7307 0000 000f 5570 6c6f 6164  lbums.....Upload
-00009af0: 6572 5461 6273 416c 6c01 0300 0000 3000  erTabsAll.....0.
-00009b00: 4700 6500 6e00 6500 6800 6d00 6900 6700  G.e.n.e.h.m.i.g.
-00009b10: 7500 6e00 6700 2000 6500 7200 6600 6f00  u.n.g. .e.r.f.o.
-00009b20: 7200 6400 6500 7200 6c00 6900 6300 6808  r.d.e.r.l.i.c.h.
-00009b30: 0000 0000 0600 0000 1641 7574 686f 7269  .........Authori
-00009b40: 7361 7469 6f6e 2072 6571 7569 7265 6407  sation required.
-00009b50: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
-00009b60: 416c 6c01 0300 0000 2200 4600 6500 6e00  All.....".F.e.n.
-00009b70: 7300 7400 6500 7200 2000 7300 6300 6800  s.t.e.r. .s.c.h.
-00009b80: 6c00 6900 6500 df00 6500 6e08 0000 0000  l.i.e...e.n.....
-00009b90: 0600 0000 0c43 6c6f 7365 2077 696e 646f  .....Close windo
-00009ba0: 7707 0000 000f 5570 6c6f 6164 6572 5461  w.....UploaderTa
-00009bb0: 6273 416c 6c01 0300 0000 4600 4200 6500  bsAll.....F.B.e.
-00009bc0: 6500 6e00 6400 6500 6e00 2000 7700 6900  e.n.d.e.n. .w.i.
-00009bd0: 7200 6400 2000 6400 6100 7300 2000 4800  r.d. .d.a.s. .H.
-00009be0: 6f00 6300 6800 6c00 6100 6400 6500 6e00  o.c.h.l.a.d.e.n.
-00009bf0: 2000 7300 7400 6f00 7000 7000 6500 6e00   .s.t.o.p.p.e.n.
-00009c00: 2e08 0000 0000 0600 0000 2643 6c6f 7369  ..........&Closi
-00009c10: 6e67 206e 6f77 2077 696c 6c20 7465 726d  ng now will term
-00009c20: 696e 6174 6520 7468 6520 7570 6c6f 6164  inate the upload
-00009c30: 2e07 0000 000f 5570 6c6f 6164 6572 5461  ......UploaderTa
-00009c40: 6273 416c 6c01 0300 0000 2a00 4e00 6500  bsAll.....*.N.e.
-00009c50: 7500 6500 7300 2000 4100 6c00 6200 7500  u.e.s. .A.l.b.u.
-00009c60: 6d00 2000 6500 7200 7300 7400 6500 6c00  m. .e.r.s.t.e.l.
-00009c70: 6c00 6500 6e08 0000 0000 0600 0000 1043  l.e.n..........C
-00009c80: 7265 6174 6520 6e65 7720 616c 6275 6d07  reate new album.
-00009c90: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
-00009ca0: 416c 6c01 0300 0000 ca00 4400 6100 7400  All.......D.a.t.
-00009cb0: 6500 6900 2020 1e00 7b00 6600 6900 6c00  e.i.  ..{.f.i.l.
-00009cc0: 6500 5f00 6e00 6100 6d00 6500 7d20 1c00  e._.n.a.m.e.} ..
-00009cd0: 2000 6800 6100 7400 2000 7b00 7300 6900   .h.a.t. .{.s.i.
-00009ce0: 7a00 6500 7d00 2000 5000 6900 7800 6500  z.e.}. .P.i.x.e.
-00009cf0: 6c00 2000 7500 6e00 6400 2000 fc00 6200  l. .u.n.d. ...b.
-00009d00: 6500 7200 7300 6300 6800 7200 6500 6900  e.r.s.c.h.r.e.i.
-00009d10: 7400 6500 7400 2000 6400 6900 6500 2000  t.e.t. .d.i.e. .
-00009d20: 4700 7200 6500 6e00 7a00 6500 2000 7600  G.r.e.n.z.e. .v.
-00009d30: 6f00 6e00 2000 7b00 6d00 6100 7800 5f00  o.n. .{.m.a.x._.
-00009d40: 7300 6900 7a00 6500 7d00 2000 5000 6900  s.i.z.e.}. .P.i.
-00009d50: 7800 6500 6c00 2000 7600 6f00 6e00 2000  x.e.l. .v.o.n. .
-00009d60: 7b00 7300 6500 7200 7600 6900 6300 6500  {.s.e.r.v.i.c.e.
-00009d70: 7d00 2e08 0000 0000 0600 0000 5846 696c  }...........XFil
-00009d80: 6520 227b 6669 6c65 5f6e 616d 657d 2220  e "{file_name}" 
-00009d90: 6861 7320 7b73 697a 657d 2070 6978 656c  has {size} pixel
-00009da0: 7320 616e 6420 6578 6365 6564 7320 7b73  s and exceeds {s
-00009db0: 6572 7669 6365 7d27 7320 6c69 6d69 7420  ervice}'s limit 
-00009dc0: 6f66 207b 6d61 785f 7369 7a65 7d20 7069  of {max_size} pi
-00009dd0: 7865 6c73 2e07 0000 000f 5570 6c6f 6164  xels......Upload
-00009de0: 6572 5461 6273 416c 6c01 0300 0000 6200  erTabsAll.....b.
-00009df0: 4800 6f00 6300 6800 6c00 6100 6400 6500  H.o.c.h.l.a.d.e.
-00009e00: 6e00 2000 6400 6500 7200 2000 4400 6100  n. .d.e.r. .D.a.
-00009e10: 7400 6500 6900 2020 1e00 7b00 6600 6900  t.e.i.  ..{.f.i.
-00009e20: 6c00 6500 5f00 6e00 6100 6d00 6500 7d20  l.e._.n.a.m.e.} 
-00009e30: 1c00 2000 6600 6500 6800 6c00 6700 6500  .. .f.e.h.l.g.e.
-00009e40: 7300 6300 6800 6c00 6100 6700 6500 6e00  s.c.h.l.a.g.e.n.
-00009e50: 2e08 0000 0000 0600 0000 2146 696c 6520  ..........!File 
-00009e60: 227b 6669 6c65 5f6e 616d 657d 2220 7570  "{file_name}" up
-00009e70: 6c6f 6164 2066 6169 6c65 642e 0700 0000  load failed.....
-00009e80: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
-00009e90: 0103 0000 001c 0044 0061 0074 0065 0069  .......D.a.t.e.i
-00009ea0: 0020 007a 0075 0020 0067 0072 006f 00df  . .z.u. .g.r.o..
-00009eb0: 002e 0800 0000 0006 0000 000f 4669 6c65  ............File
-00009ec0: 2074 6f6f 206c 6172 6765 2e07 0000 000f   too large......
-00009ed0: 5570 6c6f 6164 6572 5461 6273 416c 6c01  UploaderTabsAll.
-00009ee0: 0300 0000 ba00 4400 6100 7400 6500 6900  ......D.a.t.e.i.
-00009ef0: 2000 7b00 6600 6900 6c00 6500 5f00 6e00   .{.f.i.l.e._.n.
-00009f00: 6100 6d00 6500 7d00 2000 7700 7500 7200  a.m.e.}. .w.u.r.
-00009f10: 6400 6500 2000 6200 6500 7200 6500 6900  d.e. .b.e.r.e.i.
-00009f20: 7400 7300 2000 6100 7500 6600 2000 7b00  t.s. .a.u.f. .{.
-00009f30: 7300 6500 7200 7600 6900 6300 6500 7d00  s.e.r.v.i.c.e.}.
-00009f40: 2000 6800 6f00 6300 6800 6700 6500 6c00   .h.o.c.h.g.e.l.
-00009f50: 6100 6400 6500 6e00 2e00 2000 5700 6900  a.d.e.n... .W.i.
-00009f60: 6500 2000 6d00 f600 6300 6800 7400 6500  e. .m...c.h.t.e.
-00009f70: 6e00 2000 5300 6900 6500 2000 7300 6900  n. .S.i.e. .s.i.
-00009f80: 6500 2000 6100 6b00 7400 7500 6100 6c00  e. .a.k.t.u.a.l.
-00009f90: 6900 7300 6900 6500 7200 6500 6e00 3f08  i.s.i.e.r.e.n.?.
-00009fa0: 0000 0000 0600 0000 5946 696c 6520 7b66  ........YFile {f
-00009fb0: 696c 655f 6e61 6d65 7d20 6861 7320 616c  ile_name} has al
-00009fc0: 7265 6164 7920 6265 656e 2075 706c 6f61  ready been uploa
-00009fd0: 6465 6420 746f 207b 7365 7276 6963 657d  ded to {service}
-00009fe0: 2e20 486f 7720 776f 756c 6420 796f 7520  . How would you 
-00009ff0: 6c69 6b65 2074 6f20 7570 6461 7465 2069  like to update i
-0000a000: 743f 0700 0000 0f55 706c 6f61 6465 7254  t?.....UploaderT
-0000a010: 6162 7341 6c6c 0103 0000 0032 0049 006e  absAll.....2.I.n
-0000a020: 006b 006f 006d 0070 0061 0074 0069 0062  .k.o.m.p.a.t.i.b
-0000a030: 006c 0065 0073 0020 0042 0069 006c 0064  .l.e.s. .B.i.l.d
-0000a040: 0066 006f 0072 006d 0061 0074 002e 0800  .f.o.r.m.a.t....
-0000a050: 0000 0006 0000 0018 496e 636f 6d70 6174  ........Incompat
-0000a060: 6962 6c65 2069 6d61 6765 2074 7970 652e  ible image type.
-0000a070: 0700 0000 0f55 706c 6f61 6465 7254 6162  .....UploaderTab
-0000a080: 7341 6c6c 0103 0000 0010 0041 006e 006d  sAll.......A.n.m
-0000a090: 0065 006c 0064 0065 006e 0800 0000 0006  .e.l.d.e.n......
-0000a0a0: 0000 0006 4c6f 6720 696e 0700 0000 0f55  ....Log in.....U
-0000a0b0: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
-0000a0c0: 0000 0010 0041 0062 006d 0065 006c 0064  .....A.b.m.e.l.d
-0000a0d0: 0065 006e 0800 0000 0006 0000 0007 4c6f  .e.n..........Lo
-0000a0e0: 6720 6f75 7407 0000 000f 5570 6c6f 6164  g out.....Upload
-0000a0f0: 6572 5461 6273 416c 6c01 0300 0000 4600  erTabsAll.....F.
-0000a100: 4100 6e00 6700 6500 6d00 6500 6c00 6400  A.n.g.e.m.e.l.d.
-0000a110: 6500 7400 2000 6100 6c00 7300 2000 7b00  e.t. .a.l.s. .{.
-0000a120: 7500 7300 6500 7200 7d00 2000 6100 7500  u.s.e.r.}. .a.u.
-0000a130: 6600 2000 7b00 7300 6500 7200 7600 6900  f. .{.s.e.r.v.i.
-0000a140: 6300 6500 7d08 0000 0000 0600 0000 204c  c.e.}......... L
-0000a150: 6f67 6765 6420 696e 2061 7320 7b75 7365  ogged in as {use
-0000a160: 727d 206f 6e20 7b73 6572 7669 6365 7d07  r} on {service}.
-0000a170: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
-0000a180: 416c 6c01 0300 0000 2a00 4b00 6500 6900  All.....*.K.e.i.
-0000a190: 6e00 2000 4200 6900 6c00 6400 2000 6800  n. .B.i.l.d. .h.
-0000a1a0: 6f00 6300 6800 6700 6500 6c00 6100 6400  o.c.h.g.e.l.a.d.
-0000a1b0: 6500 6e08 0000 0000 0600 0000 0f4e 6f20  e.n..........No 
-0000a1c0: 696d 6167 6520 7570 6c6f 6164 0700 0000  image upload....
-0000a1d0: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
-0000a1e0: 0103 0000 0018 004b 0065 0069 006e 0020  .......K.e.i.n. 
-0000a1f0: 0054 0072 0065 0066 0066 0065 0072 0800  .T.r.e.f.f.e.r..
-0000a200: 0000 0006 0000 0008 4e6f 206d 6174 6368  ........No match
-0000a210: 0700 0000 0f55 706c 6f61 6465 7254 6162  .....UploaderTab
-0000a220: 7341 6c6c 0103 0000 003c 004e 0069 0063  sAll.....<.N.i.c
-0000a230: 0068 0074 0020 0061 006e 0067 0065 006d  .h.t. .a.n.g.e.m
-0000a240: 0065 006c 0064 0065 0074 0020 0062 0065  .e.l.d.e.t. .b.e
-0000a250: 0069 0020 007b 0073 0065 0072 0076 0069  .i. .{.s.e.r.v.i
-0000a260: 0063 0065 007d 0800 0000 0006 0000 001a  .c.e.}..........
-0000a270: 4e6f 7420 6c6f 6767 6564 2069 6e20 746f  Not logged in to
-0000a280: 207b 7365 7276 6963 657d 0700 0000 0f55   {service}.....U
-0000a290: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
-0000a2a0: 0000 0022 0050 0068 006f 0074 0069 006e  ...".P.h.o.t.i.n
-0000a2b0: 0069 003a 0020 007a 0075 006c 0061 0073  .i.:. .z.u.l.a.s
-0000a2c0: 0073 0065 006e 0800 0000 0006 0000 0012  .s.e.n..........
-0000a2d0: 5068 6f74 696e 693a 2061 7574 686f 7269  Photini: authori
-0000a2e0: 7365 0700 0000 0f55 706c 6f61 6465 7254  se.....UploaderT
-0000a2f0: 6162 7341 6c6c 0103 0000 0034 0050 0068  absAll.....4.P.h
-0000a300: 006f 0074 0069 006e 0069 003a 0020 0069  .o.t.i.n.i.:. .i
-0000a310: 006e 006b 006f 006d 0070 0061 0074 0069  .n.k.o.m.p.a.t.i
-0000a320: 0062 006c 0065 0072 0020 0054 0079 0070  .b.l.e.r. .T.y.p
-0000a330: 0800 0000 0006 0000 001a 5068 6f74 696e  ..........Photin
-0000a340: 693a 2069 6e63 6f6d 7061 7469 626c 6520  i: incompatible 
-0000a350: 7479 7065 0700 0000 0f55 706c 6f61 6465  type.....Uploade
-0000a360: 7254 6162 7341 6c6c 0103 0000 0020 0050  rTabsAll..... .P
-0000a370: 0068 006f 0074 0069 006e 0069 003a 0020  .h.o.t.i.n.i.:. 
-0000a380: 007a 0075 0020 0067 0072 006f 00df 0800  .z.u. .g.r.o....
-0000a390: 0000 0006 0000 0012 5068 6f74 696e 693a  ........Photini:
-0000a3a0: 2074 6f6f 206c 6172 6765 0700 0000 0f55   too large.....U
-0000a3b0: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
-0000a3c0: 0000 003c 0050 0068 006f 0074 0069 006e  ...<.P.h.o.t.i.n
-0000a3d0: 0069 003a 0020 0046 0065 0068 006c 0065  .i.:. .F.e.h.l.e
-0000a3e0: 0072 0020 0062 0065 0069 006d 0020 0048  .r. .b.e.i.m. .H
-0000a3f0: 006f 0063 0068 006c 0061 0064 0065 006e  .o.c.h.l.a.d.e.n
-0000a400: 0800 0000 0006 0000 0015 5068 6f74 696e  ..........Photin
-0000a410: 693a 2075 706c 6f61 6420 6572 726f 7207  i: upload error.
-0000a420: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
-0000a430: 416c 6c01 0300 0000 3000 5000 6800 6f00  All.....0.P.h.o.
-0000a440: 7400 6900 6e00 6900 3a00 2000 4800 6f00  t.i.n.i.:. .H.o.
-0000a450: 6300 6800 6c00 6100 6400 6500 6e00 2000  c.h.l.a.d.e.n. .
-0000a460: 6c00 e400 7500 6600 7408 0000 0000 0600  l...u.f.t.......
-0000a470: 0000 1b50 686f 7469 6e69 3a20 7570 6c6f  ...Photini: uplo
-0000a480: 6164 2069 6e20 7072 6f67 7265 7373 0700  ad in progress..
-0000a490: 0000 0f55 706c 6f61 6465 7254 6162 7341  ...UploaderTabsA
-0000a4a0: 6c6c 0103 0000 00ce 0042 0069 0074 0074  ll.......B.i.t.t
-0000a4b0: 0065 0020 0076 0065 0072 0077 0065 006e  .e. .v.e.r.w.e.n
-0000a4c0: 0064 0065 006e 0020 0053 0069 0065 0020  .d.e.n. .S.i.e. 
-0000a4d0: 0049 0068 0072 0065 006e 0020 0057 0065  .I.h.r.e.n. .W.e
-0000a4e0: 0062 0062 0072 006f 0077 0073 0065 0072  .b.b.r.o.w.s.e.r
-0000a4f0: 002c 0020 0075 006d 0020 0050 0068 006f  .,. .u.m. .P.h.o
-0000a500: 0074 0069 006e 0069 0020 007a 0075 0020  .t.i.n.i. .z.u. 
-0000a510: 0061 0075 0074 006f 0072 0069 0073 0069  .a.u.t.o.r.i.s.i
-0000a520: 0065 0072 0065 006e 002c 0020 0075 006e  .e.r.e.n.,. .u.n
-0000a530: 0064 0020 0073 0063 0068 006c 0069 0065  .d. .s.c.h.l.i.e
-0000a540: 00df 0065 006e 0020 0053 0069 0065 0020  ...e.n. .S.i.e. 
-0000a550: 0064 0061 006e 006e 0020 0064 0069 0065  .d.a.n.n. .d.i.e
-0000a560: 0073 0065 006e 0020 0044 0069 0061 006c  .s.e.n. .D.i.a.l
-0000a570: 006f 0067 002e 0800 0000 0006 0000 004d  .o.g...........M
-0000a580: 506c 6561 7365 2075 7365 2079 6f75 7220  Please use your 
-0000a590: 7765 6220 6272 6f77 7365 7220 746f 2061  web browser to a
-0000a5a0: 7574 686f 7269 7365 2050 686f 7469 6e69  uthorise Photini
-0000a5b0: 2c20 616e 6420 7468 656e 2063 6c6f 7365  , and then close
-0000a5c0: 2074 6869 7320 6469 616c 6f67 2e07 0000   this dialog....
-0000a5d0: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
-0000a5e0: 6c01 0300 0000 1600 4600 6f00 7200 7400  l.......F.o.r.t.
-0000a5f0: 7300 6300 6800 7200 6900 7400 7408 0000  s.c.h.r.i.t.t...
-0000a600: 0000 0600 0000 0850 726f 6772 6573 7307  .......Progress.
-0000a610: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
-0000a620: 416c 6c01 0300 0000 1a00 4200 6900 6c00  All.......B.i.l.
-0000a630: 6400 2000 6500 7200 7300 6500 7400 7a00  d. .e.r.s.e.t.z.
-0000a640: 6500 6e08 0000 0000 0600 0000 0d52 6570  e.n..........Rep
-0000a650: 6c61 6365 2069 6d61 6765 0700 0000 0f55  lace image.....U
-0000a660: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
-0000a670: 0000 001c 0050 0068 006f 0074 006f 0020  .....P.h.o.t.o. 
-0000a680: 0065 0072 0073 0065 0074 007a 0065 006e  .e.r.s.e.t.z.e.n
-0000a690: 0800 0000 0006 0000 000d 5265 706c 6163  ..........Replac
-0000a6a0: 6520 7068 6f74 6f07 0000 000f 5570 6c6f  e photo.....Uplo
-0000a6b0: 6164 6572 5461 6273 416c 6c01 0300 0000  aderTabsAll.....
-0000a6c0: 1c00 4200 6900 6c00 6400 2000 6100 7500  ..B.i.l.d. .a.u.
-0000a6d0: 7300 7700 e400 6800 6c00 6500 6e08 0000  s.w...h.l.e.n...
-0000a6e0: 0000 0600 0000 0f53 656c 6563 7420 616e  .......Select an
-0000a6f0: 2069 6d61 6765 0700 0000 0f55 706c 6f61   image.....Uploa
-0000a700: 6465 7254 6162 7341 6c6c 0103 0000 0018  derTabsAll......
-0000a710: 00dc 0062 0065 0072 0073 0070 0072 0069  ...b.e.r.s.p.r.i
-0000a720: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
-0000a730: 0004 536b 6970 0700 0000 0f55 706c 6f61  ..Skip.....Uploa
-0000a740: 6465 7254 6162 7341 6c6c 0103 0000 0022  derTabsAll....."
-0000a750: 0048 006f 0063 0068 006c 0061 0064 0065  .H.o.c.h.l.a.d.e
-0000a760: 006e 0020 0073 0074 0061 0072 0074 0065  .n. .s.t.a.r.t.e
-0000a770: 006e 0800 0000 0006 0000 000c 5374 6172  .n..........Star
-0000a780: 7420 7570 6c6f 6164 0700 0000 0f55 706c  t upload.....Upl
-0000a790: 6f61 6465 7254 6162 7341 6c6c 0103 0000  oaderTabsAll....
-0000a7a0: 0022 0048 006f 0063 0068 006c 0061 0064  .".H.o.c.h.l.a.d
-0000a7b0: 0065 006e 0020 0073 0074 006f 0070 0070  .e.n. .s.t.o.p.p
-0000a7c0: 0065 006e 0800 0000 0006 0000 000b 5374  .e.n..........St
-0000a7d0: 6f70 2075 706c 6f61 6407 0000 000f 5570  op upload.....Up
-0000a7e0: 6c6f 6164 6572 5461 6273 416c 6c01 0300  loaderTabsAll...
-0000a7f0: 0000 3200 4100 6c00 7300 2000 6e00 6500  ..2.A.l.s. .n.e.
-0000a800: 7500 6500 7300 2000 5000 6800 6f00 7400  u.e.s. .P.h.o.t.
-0000a810: 6f00 2000 6800 6f00 6300 6800 6c00 6100  o. .h.o.c.h.l.a.
-0000a820: 6400 6500 6e08 0000 0000 0600 0000 1355  d.e.n..........U
-0000a830: 706c 6f61 6420 6173 206e 6577 2070 686f  pload as new pho
-0000a840: 746f 0700 0000 0f55 706c 6f61 6465 7254  to.....UploaderT
-0000a850: 6162 7341 6c6c 0103 0000 005a 0048 006f  absAll.....Z.H.o
-0000a860: 0063 0068 006c 0061 0064 0065 006e 0020  .c.h.l.a.d.e.n. 
-0000a870: 006e 0061 0063 0068 0020 007b 0073 0065  .n.a.c.h. .{.s.e
-0000a880: 0072 0076 0069 0063 0065 007d 0020 0077  .r.v.i.c.e.}. .w
-0000a890: 0075 0072 0064 0065 0020 006e 0069 0063  .u.r.d.e. .n.i.c
-0000a8a0: 0068 0074 0020 0062 0065 0065 006e 0064  .h.t. .b.e.e.n.d
-0000a8b0: 0065 0074 002e 0800 0000 0006 0000 0025  .e.t...........%
-0000a8c0: 5570 6c6f 6164 2074 6f20 7b73 6572 7669  Upload to {servi
-0000a8d0: 6365 7d20 6861 7320 6e6f 7420 6669 6e69  ce} has not fini
-0000a8e0: 7368 6564 2e07 0000 000f 5570 6c6f 6164  shed......Upload
-0000a8f0: 6572 5461 6273 416c 6c01 0300 0000 6800  erTabsAll.....h.
-0000a900: 5700 6500 6c00 6300 6800 6500 2000 4200  W.e.l.c.h.e. .B.
-0000a910: 6900 6c00 6400 6400 6100 7400 6500 6900  i.l.d.d.a.t.e.i.
-0000a920: 2000 7000 6100 7300 7300 7400 2000 7a00   .p.a.s.s.t. .z.
-0000a930: 7500 2000 6400 6900 6500 7300 6500 6d00  u. .d.i.e.s.e.m.
-0000a940: 2000 4200 6900 6c00 6400 2000 6100 7500   .B.i.l.d. .a.u.
-0000a950: 6600 2000 7b00 7300 6500 7200 7600 6900  f. .{.s.e.r.v.i.
-0000a960: 6300 6500 7d00 3f08 0000 0000 0600 0000  c.e.}.?.........
-0000a970: 3357 6869 6368 2069 6d61 6765 2066 696c  3Which image fil
-0000a980: 6520 6d61 7463 6865 7320 7468 6973 2070  e matches this p
-0000a990: 6963 7475 7265 206f 6e20 7b73 6572 7669  icture on {servi
-0000a9a0: 6365 7d3f 0700 0000 0f55 706c 6f61 6465  ce}?.....Uploade
-0000a9b0: 7254 6162 7341 6c6c 0103 0000 0050 004d  rTabsAll.....P.M
-0000a9c0: 00f6 0063 0068 0074 0065 006e 0020 0053  ...c.h.t.e.n. .S
-0000a9d0: 0069 0065 0020 0065 0073 0020 0069 006e  .i.e. .e.s. .i.n
-0000a9e0: 0020 0065 0069 006e 0020 004a 0050 0045  . .e.i.n. .J.P.E
-0000a9f0: 0047 0020 006b 006f 006e 0076 0065 0072  .G. .k.o.n.v.e.r
-0000aa00: 0074 0069 0065 0072 0065 006e 003f 0800  .t.i.e.r.e.n.?..
-0000aa10: 0000 0006 0000 0025 576f 756c 6420 796f  .......%Would yo
-0000aa20: 7520 6c69 6b65 2074 6f20 636f 6e76 6572  u like to conver
-0000aa30: 7420 6974 2074 6f20 4a50 4547 3f07 0000  t it to JPEG?...
-0000aa40: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
-0000aa50: 6c01 0300 0000 3a00 4d00 f600 6300 6800  l.....:.M...c.h.
-0000aa60: 7400 6500 6e00 2000 5300 6900 6500 2000  t.e.n. .S.i.e. .
-0000aa70: 6400 6900 6500 2000 4700 7200 f600 df00  d.i.e. .G.r.....
-0000aa80: 6500 2000 e400 6e00 6400 6500 7200 6e00  e. ...n.d.e.r.n.
-0000aa90: 3f08 0000 0000 0600 0000 1c57 6f75 6c64  ?..........Would
-0000aaa0: 2079 6f75 206c 696b 6520 746f 2072 6573   you like to res
-0000aab0: 697a 6520 6974 3f07 0000 000f 5570 6c6f  ize it?.....Uplo
-0000aac0: 6164 6572 5461 6273 416c 6c01 0300 0000  aderTabsAll.....
-0000aad0: 4400 4d00 f600 6300 6800 7400 6500 6e00  D.M...c.h.t.e.n.
-0000aae0: 2000 5300 6900 6500 2000 6500 7300 2000   .S.i.e. .e.s. .
-0000aaf0: 7400 7200 6f00 7400 7a00 6400 6500 6d00  t.r.o.t.z.d.e.m.
-0000ab00: 2000 6800 6f00 6300 6800 6c00 6100 6400   .h.o.c.h.l.a.d.
-0000ab10: 6500 6e00 3f08 0000 0000 0600 0000 2357  e.n.?.........#W
-0000ab20: 6f75 6c64 2079 6f75 206c 696b 6520 746f  ould you like to
-0000ab30: 2075 706c 6f61 6420 6974 2061 6e79 7761   upload it anywa
-0000ab40: 793f 0700 0000 0f55 706c 6f61 6465 7254  y?.....UploaderT
-0000ab50: 6162 7341 6c6c 0103 0000 005e 0044 0061  absAll.....^.D.a
-0000ab60: 0073 0020 0042 0072 006f 0077 0073 0065  .s. .B.r.o.w.s.e
-0000ab70: 0072 0066 0065 006e 0073 0074 0065 0072  .r.f.e.n.s.t.e.r
-0000ab80: 0020 006b 0061 006e 006e 0020 006e 0075  . .k.a.n.n. .n.u
-0000ab90: 006e 0020 0067 0065 0073 0063 0068 006c  .n. .g.e.s.c.h.l
-0000aba0: 006f 0073 0073 0065 006e 0020 0077 0065  .o.s.s.e.n. .w.e
-0000abb0: 0072 0064 0065 006e 002e 0800 0000 0006  .r.d.e.n........
-0000abc0: 0000 0026 596f 7520 6d61 7920 6e6f 7720  ...&You may now 
-0000abd0: 636c 6f73 6520 7468 6973 2062 726f 7773  close this brows
-0000abe0: 6572 2077 696e 646f 772e 0700 0000 0f55  er window......U
-0000abf0: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
-0000ac00: 0000 001e 003c 004d 0065 0068 0072 0066  .....<.M.e.h.r.f
-0000ac10: 0061 0063 0068 0077 0065 0072 0074 0065  .a.c.h.w.e.r.t.e
-0000ac20: 003e 0800 0000 0006 0000 0011 3c6d 756c  .>..........<mul
-0000ac30: 7469 706c 6520 7661 6c75 6573 3e07 0000  tiple values>...
-0000ac40: 0007 5769 6467 6574 7301 0300 0000 1400  ..Widgets.......
-0000ac50: 3c00 6d00 6500 6800 7200 6600 6100 6300  <.m.e.h.r.f.a.c.
-0000ac60: 6800 3e08 0000 0000 0600 0000 0a3c 6d75  h.>..........<mu
-0000ac70: 6c74 6970 6c65 3e07 0000 0007 5769 6467  ltiple>.....Widg
-0000ac80: 6574 7301 0300 0000 0a00 3c00 6e00 6500  ets.......<.n.e.
-0000ac90: 7500 3e08 0000 0000 0600 0000 053c 6e65  u.>..........<ne
-0000aca0: 773e 0700 0000 0757 6964 6765 7473 0188  w>.....Widgets..
-0000acb0: 0000 0002 0101                           ......
+00009900: 0000 1c00 4800 6500 7200 7300 7400 6500  ....H.e.r.s.t.e.
+00009910: 6c00 6c00 6500 7200 6e00 6100 6d00 6508  l.l.e.r.n.a.m.e.
+00009920: 0000 0000 0600 0000 0c4d 616b 6572 2773  .........Maker's
+00009930: 206e 616d 6507 0000 000c 5465 6368 6e69   name.....Techni
+00009940: 6361 6c54 6162 0103 0000 0016 004d 0061  calTab.......M.a
+00009950: 0078 002e 0020 0042 006c 0065 006e 0064  .x... .B.l.e.n.d
+00009960: 0065 0800 0000 0006 0000 000c 4d61 7820  .e..........Max 
+00009970: 6170 6572 7475 7265 0700 0000 0c54 6563  aperture.....Tec
+00009980: 686e 6963 616c 5461 6201 0300 0000 2600  hnicalTab.....&.
+00009990: 4d00 6100 7800 6900 6d00 6100 6c00 6500  M.a.x.i.m.a.l.e.
+000099a0: 2000 4200 7200 6500 6e00 6e00 7700 6500   .B.r.e.n.n.w.e.
+000099b0: 6900 7400 6508 0000 0000 0600 0000 144d  i.t.e..........M
+000099c0: 6178 696d 756d 2066 6f63 616c 206c 656e  aximum focal len
+000099d0: 6774 6807 0000 000c 5465 6368 6e69 6361  gth.....Technica
+000099e0: 6c54 6162 0103 0000 0026 004d 0069 006e  lTab.....&.M.i.n
+000099f0: 0069 006d 0061 006c 0065 0020 0042 0072  .i.m.a.l.e. .B.r
+00009a00: 0065 006e 006e 0077 0065 0069 0074 0065  .e.n.n.w.e.i.t.e
+00009a10: 0800 0000 0006 0000 0014 4d69 6e69 6d75  ..........Minimu
+00009a20: 6d20 666f 6361 6c20 6c65 6e67 7468 0700  m focal length..
+00009a30: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
+00009a40: 0300 0000 1400 4d00 6f00 6400 6500 6c00  ......M.o.d.e.l.
+00009a50: 6c00 6e00 6100 6d00 6508 0000 0000 0600  l.n.a.m.e.......
+00009a60: 0000 0a4d 6f64 656c 206e 616d 6507 0000  ...Model name...
+00009a70: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
+00009a80: 0000 0012 0056 0065 0072 00e4 006e 0064  .....V.e.r...n.d
+00009a90: 0065 0072 0074 0800 0000 0006 0000 0008  .e.r.t..........
+00009aa0: 4d6f 6469 6669 6564 0700 0000 0c54 6563  Modified.....Tec
+00009ab0: 686e 6963 616c 5461 6201 0300 0000 1600  hnicalTab.......
+00009ac0: 4100 7500 7300 7200 6900 6300 6800 7400  A.u.s.r.i.c.h.t.
+00009ad0: 7500 6e00 6708 0000 0000 0600 0000 0b4f  u.n.g..........O
+00009ae0: 7269 656e 7461 7469 6f6e 0700 0000 0c54  rientation.....T
+00009af0: 6563 686e 6963 616c 5461 6201 0300 0000  echnicalTab.....
+00009b00: 0c00 4100 6e00 6400 6500 7200 6508 0000  ..A.n.d.e.r.e...
+00009b10: 0000 0600 0000 054f 7468 6572 0700 0000  .......Other....
+00009b20: 0c54 6563 686e 6963 616c 5461 6201 0300  .TechnicalTab...
+00009b30: 0000 3400 5000 6800 6f00 7400 6900 6e00  ..4.P.h.o.t.i.n.
+00009b40: 6900 3a00 2000 4b00 6100 6d00 6500 7200  i.:. .K.a.m.e.r.
+00009b50: 6100 2000 6400 6500 6600 6900 6e00 6900  a. .d.e.f.i.n.i.
+00009b60: 6500 7200 6500 6e08 0000 0000 0600 0000  e.r.e.n.........
+00009b70: 1650 686f 7469 6e69 3a20 6465 6669 6e65  .Photini: define
+00009b80: 2063 616d 6572 6107 0000 000c 5465 6368   camera.....Tech
+00009b90: 6e69 6361 6c54 6162 0103 0000 0032 0050  nicalTab.....2.P
+00009ba0: 0068 006f 0074 0069 006e 0069 003a 0020  .h.o.t.i.n.i.:. 
+00009bb0: 004c 0069 006e 0073 0065 0020 0064 0065  .L.i.n.s.e. .d.e
+00009bc0: 0066 0069 006e 0069 0065 0072 0065 006e  .f.i.n.i.e.r.e.n
+00009bd0: 0800 0000 0006 0000 0014 5068 6f74 696e  ..........Photin
+00009be0: 693a 2064 6566 696e 6520 6c65 6e73 0700  i: define lens..
+00009bf0: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
+00009c00: 0300 0000 1600 4700 6500 6e00 6100 7500  ......G.e.n.a.u.
+00009c10: 6900 6700 6b00 6500 6900 7408 0000 0000  i.g.k.e.i.t.....
+00009c20: 0600 0000 0950 7265 6369 7369 6f6e 0700  .....Precision..
+00009c30: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
+00009c40: 0300 0000 3800 2200 7b00 6300 6100 6d00  ....8.".{.c.a.m.
+00009c50: 6500 7200 6100 5f00 6f00 7200 5f00 6c00  e.r.a._.o.r._.l.
+00009c60: 6500 6e00 7300 7d00 2200 2000 6500 6e00  e.n.s.}.". .e.n.
+00009c70: 7400 6600 6500 7200 6e00 6500 6e08 0000  t.f.e.r.n.e.n...
+00009c80: 0000 0600 0000 1952 656d 6f76 6520 227b  .......Remove "{
+00009c90: 6361 6d65 7261 5f6f 725f 6c65 6e73 7d22  camera_or_lens}"
+00009ca0: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
+00009cb0: 6201 0300 0000 1800 5300 6500 7200 6900  b.......S.e.r.i.
+00009cc0: 6500 6e00 6e00 7500 6d00 6d00 6500 7208  e.n.n.u.m.m.e.r.
+00009cd0: 0000 0000 0600 0000 0d53 6572 6961 6c20  .........Serial 
+00009ce0: 6e75 6d62 6572 0700 0000 0c54 6563 686e  number.....Techn
+00009cf0: 6963 616c 5461 6201 0300 0000 1600 4100  icalTab.......A.
+00009d00: 7500 6600 6700 6500 6e00 6f00 6d00 6d00  u.f.g.e.n.o.m.m.
+00009d10: 6500 6e08 0000 0000 0600 0000 0554 616b  e.n..........Tak
+00009d20: 656e 0700 0000 0c54 6563 686e 6963 616c  en.....Technical
+00009d30: 5461 6201 0300 0000 4600 4200 6c00 6500  Tab.....F.B.l.e.
+00009d40: 6e00 6400 6500 2000 7500 6e00 6400 2000  n.d.e. .u.n.d. .
+00009d50: 4200 7200 6500 6e00 6e00 7700 6500 6900  B.r.e.n.n.w.e.i.
+00009d60: 7400 6500 2000 6100 6b00 7400 7500 6100  t.e. .a.k.t.u.a.
+00009d70: 6c00 6900 7300 6900 6500 7200 6500 6e08  l.i.s.i.e.r.e.n.
+00009d80: 0000 0000 0600 0000 1e55 7064 6174 6520  .........Update 
+00009d90: 6170 6572 7475 7265 2026 2066 6f63 616c  aperture & focal
+00009da0: 206c 656e 6774 6807 0000 000c 5465 6368   length.....Tech
+00009db0: 6e69 6361 6c54 6162 0103 0000 0006 006d  nicalTab.......m
+00009dc0: 0061 0078 0800 0000 0006 0000 0003 6d61  .a.x..........ma
+00009dd0: 7807 0000 000c 5465 6368 6e69 6361 6c54  x.....TechnicalT
+00009de0: 6162 0103 0000 0006 006d 0069 006e 0800  ab.......m.i.n..
+00009df0: 0000 0006 0000 0003 6d69 6e07 0000 000c  ........min.....
+00009e00: 5465 6368 6e69 6361 6c54 6162 0103 0000  TechnicalTab....
+00009e10: 000c 006e 006f 0072 006d 0061 006c 0800  ...n.o.r.m.a.l..
+00009e20: 0000 0006 0000 0006 6e6f 726d 616c 0700  ........normal..
+00009e30: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
+00009e40: 0300 0000 2a00 6c00 6900 6e00 6b00 7300  ....*.l.i.n.k.s.
+00009e50: 2d00 7200 6500 6300 6800 7400 7300 2000  -.r.e.c.h.t.s. .
+00009e60: 7300 7000 6900 6500 6700 6500 6c00 6e08  s.p.i.e.g.e.l.n.
+00009e70: 0000 0000 0600 0000 1572 6566 6c65 6374  .........reflect
+00009e80: 206c 6566 7420 746f 2072 6967 6874 0700   left to right..
+00009e90: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
+00009ea0: 0300 0000 4000 6c00 6900 6e00 6b00 7300  ....@.l.i.n.k.s.
+00009eb0: 2000 6f00 6200 6500 6e00 2d00 7200 6500   .o.b.e.n.-.r.e.
+00009ec0: 6300 6800 7400 7300 2000 7500 6e00 7400  c.h.t.s. .u.n.t.
+00009ed0: 6500 6e00 2000 7300 7000 6900 6500 6700  e.n. .s.p.i.e.g.
+00009ee0: 6500 6c00 6e08 0000 0000 0600 0000 2072  e.l.n......... r
+00009ef0: 6566 6c65 6374 2074 6f70 206c 6566 7420  eflect top left 
+00009f00: 746f 2062 6f74 746f 6d20 7269 6768 7407  to bottom right.
+00009f10: 0000 000c 5465 6368 6e69 6361 6c54 6162  ....TechnicalTab
+00009f20: 0103 0000 0040 0072 0065 0063 0068 0074  .....@.r.e.c.h.t
+00009f30: 0073 0020 006f 0062 0065 006e 002d 006c  .s. .o.b.e.n.-.l
+00009f40: 0069 006e 006b 0073 0020 0075 006e 0074  .i.n.k.s. .u.n.t
+00009f50: 0065 006e 0020 0073 0070 0069 0065 0067  .e.n. .s.p.i.e.g
+00009f60: 0065 006c 006e 0800 0000 0006 0000 0020  .e.l.n......... 
+00009f70: 7265 666c 6563 7420 746f 7020 7269 6768  reflect top righ
+00009f80: 7420 746f 2062 6f74 746f 6d20 6c65 6674  t to bottom left
+00009f90: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
+00009fa0: 6201 0300 0000 2600 6f00 6200 6500 6e00  b.....&.o.b.e.n.
+00009fb0: 2d00 7500 6e00 7400 6500 6e00 2000 7300  -.u.n.t.e.n. .s.
+00009fc0: 7000 6900 6500 6700 6500 6c00 6e08 0000  p.i.e.g.e.l.n...
+00009fd0: 0000 0600 0000 1572 6566 6c65 6374 2074  .......reflect t
+00009fe0: 6f70 2074 6f20 626f 7474 6f6d 0700 0000  op to bottom....
+00009ff0: 0c54 6563 686e 6963 616c 5461 6201 0300  .TechnicalTab...
+0000a000: 0000 3e00 3900 3000 2000 4700 7200 6100  ..>.9.0. .G.r.a.
+0000a010: 6400 2000 6900 6d00 2000 5500 6800 7200  d. .i.m. .U.h.r.
+0000a020: 7a00 6500 6900 6700 6500 7200 7300 6900  z.e.i.g.e.r.s.i.
+0000a030: 6e00 6e00 2000 6400 7200 6500 6800 6500  n.n. .d.r.e.h.e.
+0000a040: 6e08 0000 0000 0600 0000 0c72 6f74 6174  n..........rotat
+0000a050: 6520 2b39 30c2 b007 0000 000c 5465 6368  e +90.......Tech
+0000a060: 6e69 6361 6c54 6162 0103 0000 0044 0039  nicalTab.....D.9
+0000a070: 0030 0020 0047 0072 0061 0064 0020 0067  .0. .G.r.a.d. .g
+0000a080: 0065 0067 0065 006e 0020 0055 0068 0072  .e.g.e.n. .U.h.r
+0000a090: 007a 0065 0069 0067 0065 0072 0073 0069  .z.e.i.g.e.r.s.i
+0000a0a0: 006e 006e 0020 0064 0072 0065 0068 0065  .n.n. .d.r.e.h.e
+0000a0b0: 006e 0800 0000 0006 0000 000c 726f 7461  .n..........rota
+0000a0c0: 7465 202d 3930 c2b0 0700 0000 0c54 6563  te -90.......Tec
+0000a0d0: 686e 6963 616c 5461 6201 0300 0000 4000  hnicalTab.....@.
+0000a0e0: 3100 3800 3000 2000 4700 7200 6100 6400  1.8.0. .G.r.a.d.
+0000a0f0: 2000 6900 6d00 2000 5500 6800 7200 7a00   .i.m. .U.h.r.z.
+0000a100: 6500 6900 6700 6500 7200 7300 6900 6e00  e.i.g.e.r.s.i.n.
+0000a110: 6e00 2000 6400 7200 6500 6800 6500 6e08  n. .d.r.e.h.e.n.
+0000a120: 0000 0000 0600 0000 0c72 6f74 6174 6520  .........rotate 
+0000a130: 3138 30c2 b007 0000 000c 5465 6368 6e69  180.......Techni
+0000a140: 6361 6c54 6162 0103 0000 0026 005a 0075  calTab.....&.Z.u
+0000a150: 0020 0041 006c 0062 0065 006e 0020 0068  . .A.l.b.e.n. .h
+0000a160: 0069 006e 007a 0075 0066 00fc 0067 0065  .i.n.z.u.f...g.e
+0000a170: 006e 0800 0000 0006 0000 000d 4164 6420  .n..........Add 
+0000a180: 746f 2061 6c62 756d 7307 0000 000f 5570  to albums.....Up
+0000a190: 6c6f 6164 6572 5461 6273 416c 6c01 0300  loaderTabsAll...
+0000a1a0: 0000 3000 4700 6500 6e00 6500 6800 6d00  ..0.G.e.n.e.h.m.
+0000a1b0: 6900 6700 7500 6e00 6700 2000 6500 7200  i.g.u.n.g. .e.r.
+0000a1c0: 6600 6f00 7200 6400 6500 7200 6c00 6900  f.o.r.d.e.r.l.i.
+0000a1d0: 6300 6808 0000 0000 0600 0000 1641 7574  c.h..........Aut
+0000a1e0: 686f 7269 7361 7469 6f6e 2072 6571 7569  horisation requi
+0000a1f0: 7265 6407 0000 000f 5570 6c6f 6164 6572  red.....Uploader
+0000a200: 5461 6273 416c 6c01 0300 0000 2200 4600  TabsAll.....".F.
+0000a210: 6500 6e00 7300 7400 6500 7200 2000 7300  e.n.s.t.e.r. .s.
+0000a220: 6300 6800 6c00 6900 6500 df00 6500 6e08  c.h.l.i.e...e.n.
+0000a230: 0000 0000 0600 0000 0c43 6c6f 7365 2077  .........Close w
+0000a240: 696e 646f 7707 0000 000f 5570 6c6f 6164  indow.....Upload
+0000a250: 6572 5461 6273 416c 6c01 0300 0000 4600  erTabsAll.....F.
+0000a260: 4200 6500 6500 6e00 6400 6500 6e00 2000  B.e.e.n.d.e.n. .
+0000a270: 7700 6900 7200 6400 2000 6400 6100 7300  w.i.r.d. .d.a.s.
+0000a280: 2000 4800 6f00 6300 6800 6c00 6100 6400   .H.o.c.h.l.a.d.
+0000a290: 6500 6e00 2000 7300 7400 6f00 7000 7000  e.n. .s.t.o.p.p.
+0000a2a0: 6500 6e00 2e08 0000 0000 0600 0000 2643  e.n...........&C
+0000a2b0: 6c6f 7369 6e67 206e 6f77 2077 696c 6c20  losing now will 
+0000a2c0: 7465 726d 696e 6174 6520 7468 6520 7570  terminate the up
+0000a2d0: 6c6f 6164 2e07 0000 000f 5570 6c6f 6164  load......Upload
+0000a2e0: 6572 5461 6273 416c 6c01 0300 0000 2a00  erTabsAll.....*.
+0000a2f0: 4e00 6500 7500 6500 7300 2000 4100 6c00  N.e.u.e.s. .A.l.
+0000a300: 6200 7500 6d00 2000 6500 7200 7300 7400  b.u.m. .e.r.s.t.
+0000a310: 6500 6c00 6c00 6500 6e08 0000 0000 0600  e.l.l.e.n.......
+0000a320: 0000 1043 7265 6174 6520 6e65 7720 616c  ...Create new al
+0000a330: 6275 6d07 0000 000f 5570 6c6f 6164 6572  bum.....Uploader
+0000a340: 5461 6273 416c 6c01 0300 0000 ca00 4400  TabsAll.......D.
+0000a350: 6900 6500 2000 4400 6100 7400 6500 6900  i.e. .D.a.t.e.i.
+0000a360: 2020 1e00 7b00 6600 6900 6c00 6500 5f00    ..{.f.i.l.e._.
+0000a370: 6e00 6100 6d00 6500 7d20 1c00 2000 6800  n.a.m.e.} .. .h.
+0000a380: 6100 7400 2000 7b00 7300 6900 7a00 6500  a.t. .{.s.i.z.e.
+0000a390: 7d00 2000 4200 7900 7400 6500 7300 2000  }. .B.y.t.e.s. .
+0000a3a0: 7500 6e00 6400 2000 fc00 6200 6500 7200  u.n.d. ...b.e.r.
+0000a3b0: 7300 6300 6800 7200 6500 6900 7400 6500  s.c.h.r.e.i.t.e.
+0000a3c0: 7400 2000 7b00 7300 6500 7200 7600 6900  t. .{.s.e.r.v.i.
+0000a3d0: 6300 6500 7d00 2000 4200 6500 6700 7200  c.e.}. .B.e.g.r.
+0000a3e0: 6500 6e00 7a00 7500 6e00 6700 2000 7600  e.n.z.u.n.g. .v.
+0000a3f0: 6f00 6e00 2000 7b00 6d00 6100 7800 5f00  o.n. .{.m.a.x._.
+0000a400: 7300 6900 7a00 6500 7d00 2000 4200 7900  s.i.z.e.}. .B.y.
+0000a410: 7400 6500 7300 2e08 0000 0000 0600 0000  t.e.s...........
+0000a420: 5646 696c 6520 227b 6669 6c65 5f6e 616d  VFile "{file_nam
+0000a430: 657d 2220 6861 7320 7b73 697a 657d 2062  e}" has {size} b
+0000a440: 7974 6573 2061 6e64 2065 7863 6565 6473  ytes and exceeds
+0000a450: 207b 7365 7276 6963 657d 2773 206c 696d   {service}'s lim
+0000a460: 6974 206f 6620 7b6d 6178 5f73 697a 657d  it of {max_size}
+0000a470: 2062 7974 6573 2e07 0000 000f 5570 6c6f   bytes......Uplo
+0000a480: 6164 6572 5461 6273 416c 6c01 0300 0000  aderTabsAll.....
+0000a490: ca00 4400 6100 7400 6500 6900 2020 1e00  ..D.a.t.e.i.  ..
+0000a4a0: 7b00 6600 6900 6c00 6500 5f00 6e00 6100  {.f.i.l.e._.n.a.
+0000a4b0: 6d00 6500 7d20 1c00 2000 6800 6100 7400  m.e.} .. .h.a.t.
+0000a4c0: 2000 7b00 7300 6900 7a00 6500 7d00 2000   .{.s.i.z.e.}. .
+0000a4d0: 5000 6900 7800 6500 6c00 2000 7500 6e00  P.i.x.e.l. .u.n.
+0000a4e0: 6400 2000 fc00 6200 6500 7200 7300 6300  d. ...b.e.r.s.c.
+0000a4f0: 6800 7200 6500 6900 7400 6500 7400 2000  h.r.e.i.t.e.t. .
+0000a500: 6400 6900 6500 2000 4700 7200 6500 6e00  d.i.e. .G.r.e.n.
+0000a510: 7a00 6500 2000 7600 6f00 6e00 2000 7b00  z.e. .v.o.n. .{.
+0000a520: 6d00 6100 7800 5f00 7300 6900 7a00 6500  m.a.x._.s.i.z.e.
+0000a530: 7d00 2000 5000 6900 7800 6500 6c00 2000  }. .P.i.x.e.l. .
+0000a540: 7600 6f00 6e00 2000 7b00 7300 6500 7200  v.o.n. .{.s.e.r.
+0000a550: 7600 6900 6300 6500 7d00 2e08 0000 0000  v.i.c.e.}.......
+0000a560: 0600 0000 5846 696c 6520 227b 6669 6c65  ....XFile "{file
+0000a570: 5f6e 616d 657d 2220 6861 7320 7b73 697a  _name}" has {siz
+0000a580: 657d 2070 6978 656c 7320 616e 6420 6578  e} pixels and ex
+0000a590: 6365 6564 7320 7b73 6572 7669 6365 7d27  ceeds {service}'
+0000a5a0: 7320 6c69 6d69 7420 6f66 207b 6d61 785f  s limit of {max_
+0000a5b0: 7369 7a65 7d20 7069 7865 6c73 2e07 0000  size} pixels....
+0000a5c0: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
+0000a5d0: 6c01 0300 0000 d000 4400 6100 7400 6500  l.......D.a.t.e.
+0000a5e0: 6900 2020 1e00 7b00 6600 6900 6c00 6500  i.  ..{.f.i.l.e.
+0000a5f0: 5f00 6e00 6100 6d00 6500 7d20 1c00 2000  _.n.a.m.e.} .. .
+0000a600: 6900 7300 7400 2000 6900 6d00 2000 4600  i.s.t. .i.m. .F.
+0000a610: 6f00 7200 6d00 6100 7400 2020 1e00 7b00  o.r.m.a.t.  ..{.
+0000a620: 6600 6900 6c00 6500 5f00 7400 7900 7000  f.i.l.e._.t.y.p.
+0000a630: 6500 7d20 1c00 2c00 2000 6400 6100 7300  e.} ..,. .d.a.s.
+0000a640: 2000 7b00 7300 6500 7200 7600 6900 6300   .{.s.e.r.v.i.c.
+0000a650: 6500 7d00 2000 6d00 f600 6700 6c00 6900  e.}. .m...g.l.i.
+0000a660: 6300 6800 6500 7200 7700 6500 6900 7300  c.h.e.r.w.e.i.s.
+0000a670: 6500 2000 6e00 6900 6300 6800 7400 2000  e. .n.i.c.h.t. .
+0000a680: 6b00 6f00 7200 7200 6500 6b00 7400 2000  k.o.r.r.e.k.t. .
+0000a690: 7600 6500 7200 6100 7200 6200 6500 6900  v.e.r.a.r.b.e.i.
+0000a6a0: 7400 6500 7400 2e08 0000 0000 0600 0000  t.e.t...........
+0000a6b0: 5646 696c 6520 227b 6669 6c65 5f6e 616d  VFile "{file_nam
+0000a6c0: 657d 2220 6973 206f 6620 7479 7065 2022  e}" is of type "
+0000a6d0: 7b66 696c 655f 7479 7065 7d22 2c20 7768  {file_type}", wh
+0000a6e0: 6963 6820 7b73 6572 7669 6365 7d20 6d61  ich {service} ma
+0000a6f0: 7920 6e6f 7420 6861 6e64 6c65 2063 6f72  y not handle cor
+0000a700: 7265 6374 6c79 2e07 0000 000f 5570 6c6f  rectly......Uplo
+0000a710: 6164 6572 5461 6273 416c 6c01 0300 0000  aderTabsAll.....
+0000a720: 6200 4800 6f00 6300 6800 6c00 6100 6400  b.H.o.c.h.l.a.d.
+0000a730: 6500 6e00 2000 6400 6500 7200 2000 4400  e.n. .d.e.r. .D.
+0000a740: 6100 7400 6500 6900 2020 1e00 7b00 6600  a.t.e.i.  ..{.f.
+0000a750: 6900 6c00 6500 5f00 6e00 6100 6d00 6500  i.l.e._.n.a.m.e.
+0000a760: 7d20 1c00 2000 6600 6500 6800 6c00 6700  } .. .f.e.h.l.g.
+0000a770: 6500 7300 6300 6800 6c00 6100 6700 6500  e.s.c.h.l.a.g.e.
+0000a780: 6e00 2e08 0000 0000 0600 0000 2146 696c  n...........!Fil
+0000a790: 6520 227b 6669 6c65 5f6e 616d 657d 2220  e "{file_name}" 
+0000a7a0: 7570 6c6f 6164 2066 6169 6c65 642e 0700  upload failed...
+0000a7b0: 0000 0f55 706c 6f61 6465 7254 6162 7341  ...UploaderTabsA
+0000a7c0: 6c6c 0103 0000 001c 0044 0061 0074 0065  ll.......D.a.t.e
+0000a7d0: 0069 0020 007a 0075 0020 0067 0072 006f  .i. .z.u. .g.r.o
+0000a7e0: 00df 002e 0800 0000 0006 0000 000f 4669  ..............Fi
+0000a7f0: 6c65 2074 6f6f 206c 6172 6765 2e07 0000  le too large....
+0000a800: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
+0000a810: 6c01 0300 0000 ba00 4400 6100 7400 6500  l.......D.a.t.e.
+0000a820: 6900 2000 7b00 6600 6900 6c00 6500 5f00  i. .{.f.i.l.e._.
+0000a830: 6e00 6100 6d00 6500 7d00 2000 7700 7500  n.a.m.e.}. .w.u.
+0000a840: 7200 6400 6500 2000 6200 6500 7200 6500  r.d.e. .b.e.r.e.
+0000a850: 6900 7400 7300 2000 6100 7500 6600 2000  i.t.s. .a.u.f. .
+0000a860: 7b00 7300 6500 7200 7600 6900 6300 6500  {.s.e.r.v.i.c.e.
+0000a870: 7d00 2000 6800 6f00 6300 6800 6700 6500  }. .h.o.c.h.g.e.
+0000a880: 6c00 6100 6400 6500 6e00 2e00 2000 5700  l.a.d.e.n... .W.
+0000a890: 6900 6500 2000 6d00 f600 6300 6800 7400  i.e. .m...c.h.t.
+0000a8a0: 6500 6e00 2000 5300 6900 6500 2000 7300  e.n. .S.i.e. .s.
+0000a8b0: 6900 6500 2000 6100 6b00 7400 7500 6100  i.e. .a.k.t.u.a.
+0000a8c0: 6c00 6900 7300 6900 6500 7200 6500 6e00  l.i.s.i.e.r.e.n.
+0000a8d0: 3f08 0000 0000 0600 0000 5946 696c 6520  ?.........YFile 
+0000a8e0: 7b66 696c 655f 6e61 6d65 7d20 6861 7320  {file_name} has 
+0000a8f0: 616c 7265 6164 7920 6265 656e 2075 706c  already been upl
+0000a900: 6f61 6465 6420 746f 207b 7365 7276 6963  oaded to {servic
+0000a910: 657d 2e20 486f 7720 776f 756c 6420 796f  e}. How would yo
+0000a920: 7520 6c69 6b65 2074 6f20 7570 6461 7465  u like to update
+0000a930: 2069 743f 0700 0000 0f55 706c 6f61 6465   it?.....Uploade
+0000a940: 7254 6162 7341 6c6c 0103 0000 0032 0049  rTabsAll.....2.I
+0000a950: 006e 006b 006f 006d 0070 0061 0074 0069  .n.k.o.m.p.a.t.i
+0000a960: 0062 006c 0065 0073 0020 0042 0069 006c  .b.l.e.s. .B.i.l
+0000a970: 0064 0066 006f 0072 006d 0061 0074 002e  .d.f.o.r.m.a.t..
+0000a980: 0800 0000 0006 0000 0018 496e 636f 6d70  ..........Incomp
+0000a990: 6174 6962 6c65 2069 6d61 6765 2074 7970  atible image typ
+0000a9a0: 652e 0700 0000 0f55 706c 6f61 6465 7254  e......UploaderT
+0000a9b0: 6162 7341 6c6c 0103 0000 0010 0041 006e  absAll.......A.n
+0000a9c0: 006d 0065 006c 0064 0065 006e 0800 0000  .m.e.l.d.e.n....
+0000a9d0: 0006 0000 0006 4c6f 6720 696e 0700 0000  ......Log in....
+0000a9e0: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
+0000a9f0: 0103 0000 0010 0041 0062 006d 0065 006c  .......A.b.m.e.l
+0000aa00: 0064 0065 006e 0800 0000 0006 0000 0007  .d.e.n..........
+0000aa10: 4c6f 6720 6f75 7407 0000 000f 5570 6c6f  Log out.....Uplo
+0000aa20: 6164 6572 5461 6273 416c 6c01 0300 0000  aderTabsAll.....
+0000aa30: 4600 4100 6e00 6700 6500 6d00 6500 6c00  F.A.n.g.e.m.e.l.
+0000aa40: 6400 6500 7400 2000 6100 6c00 7300 2000  d.e.t. .a.l.s. .
+0000aa50: 7b00 7500 7300 6500 7200 7d00 2000 6100  {.u.s.e.r.}. .a.
+0000aa60: 7500 6600 2000 7b00 7300 6500 7200 7600  u.f. .{.s.e.r.v.
+0000aa70: 6900 6300 6500 7d08 0000 0000 0600 0000  i.c.e.}.........
+0000aa80: 204c 6f67 6765 6420 696e 2061 7320 7b75   Logged in as {u
+0000aa90: 7365 727d 206f 6e20 7b73 6572 7669 6365  ser} on {service
+0000aaa0: 7d07 0000 000f 5570 6c6f 6164 6572 5461  }.....UploaderTa
+0000aab0: 6273 416c 6c01 0300 0000 2a00 4b00 6500  bsAll.....*.K.e.
+0000aac0: 6900 6e00 2000 4200 6900 6c00 6400 2000  i.n. .B.i.l.d. .
+0000aad0: 6800 6f00 6300 6800 6700 6500 6c00 6100  h.o.c.h.g.e.l.a.
+0000aae0: 6400 6500 6e08 0000 0000 0600 0000 0f4e  d.e.n..........N
+0000aaf0: 6f20 696d 6167 6520 7570 6c6f 6164 0700  o image upload..
+0000ab00: 0000 0f55 706c 6f61 6465 7254 6162 7341  ...UploaderTabsA
+0000ab10: 6c6c 0103 0000 0018 004b 0065 0069 006e  ll.......K.e.i.n
+0000ab20: 0020 0054 0072 0065 0066 0066 0065 0072  . .T.r.e.f.f.e.r
+0000ab30: 0800 0000 0006 0000 0008 4e6f 206d 6174  ..........No mat
+0000ab40: 6368 0700 0000 0f55 706c 6f61 6465 7254  ch.....UploaderT
+0000ab50: 6162 7341 6c6c 0103 0000 003c 004e 0069  absAll.....<.N.i
+0000ab60: 0063 0068 0074 0020 0061 006e 0067 0065  .c.h.t. .a.n.g.e
+0000ab70: 006d 0065 006c 0064 0065 0074 0020 0062  .m.e.l.d.e.t. .b
+0000ab80: 0065 0069 0020 007b 0073 0065 0072 0076  .e.i. .{.s.e.r.v
+0000ab90: 0069 0063 0065 007d 0800 0000 0006 0000  .i.c.e.}........
+0000aba0: 001a 4e6f 7420 6c6f 6767 6564 2069 6e20  ..Not logged in 
+0000abb0: 746f 207b 7365 7276 6963 657d 0700 0000  to {service}....
+0000abc0: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
+0000abd0: 0103 0000 0022 0050 0068 006f 0074 0069  .....".P.h.o.t.i
+0000abe0: 006e 0069 003a 0020 007a 0075 006c 0061  .n.i.:. .z.u.l.a
+0000abf0: 0073 0073 0065 006e 0800 0000 0006 0000  .s.s.e.n........
+0000ac00: 0012 5068 6f74 696e 693a 2061 7574 686f  ..Photini: autho
+0000ac10: 7269 7365 0700 0000 0f55 706c 6f61 6465  rise.....Uploade
+0000ac20: 7254 6162 7341 6c6c 0103 0000 0034 0050  rTabsAll.....4.P
+0000ac30: 0068 006f 0074 0069 006e 0069 003a 0020  .h.o.t.i.n.i.:. 
+0000ac40: 0069 006e 006b 006f 006d 0070 0061 0074  .i.n.k.o.m.p.a.t
+0000ac50: 0069 0062 006c 0065 0072 0020 0054 0079  .i.b.l.e.r. .T.y
+0000ac60: 0070 0800 0000 0006 0000 001a 5068 6f74  .p..........Phot
+0000ac70: 696e 693a 2069 6e63 6f6d 7061 7469 626c  ini: incompatibl
+0000ac80: 6520 7479 7065 0700 0000 0f55 706c 6f61  e type.....Uploa
+0000ac90: 6465 7254 6162 7341 6c6c 0103 0000 0020  derTabsAll..... 
+0000aca0: 0050 0068 006f 0074 0069 006e 0069 003a  .P.h.o.t.i.n.i.:
+0000acb0: 0020 007a 0075 0020 0067 0072 006f 00df  . .z.u. .g.r.o..
+0000acc0: 0800 0000 0006 0000 0012 5068 6f74 696e  ..........Photin
+0000acd0: 693a 2074 6f6f 206c 6172 6765 0700 0000  i: too large....
+0000ace0: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
+0000acf0: 0103 0000 003c 0050 0068 006f 0074 0069  .....<.P.h.o.t.i
+0000ad00: 006e 0069 003a 0020 0046 0065 0068 006c  .n.i.:. .F.e.h.l
+0000ad10: 0065 0072 0020 0062 0065 0069 006d 0020  .e.r. .b.e.i.m. 
+0000ad20: 0048 006f 0063 0068 006c 0061 0064 0065  .H.o.c.h.l.a.d.e
+0000ad30: 006e 0800 0000 0006 0000 0015 5068 6f74  .n..........Phot
+0000ad40: 696e 693a 2075 706c 6f61 6420 6572 726f  ini: upload erro
+0000ad50: 7207 0000 000f 5570 6c6f 6164 6572 5461  r.....UploaderTa
+0000ad60: 6273 416c 6c01 0300 0000 3000 5000 6800  bsAll.....0.P.h.
+0000ad70: 6f00 7400 6900 6e00 6900 3a00 2000 4800  o.t.i.n.i.:. .H.
+0000ad80: 6f00 6300 6800 6c00 6100 6400 6500 6e00  o.c.h.l.a.d.e.n.
+0000ad90: 2000 6c00 e400 7500 6600 7408 0000 0000   .l...u.f.t.....
+0000ada0: 0600 0000 1b50 686f 7469 6e69 3a20 7570  .....Photini: up
+0000adb0: 6c6f 6164 2069 6e20 7072 6f67 7265 7373  load in progress
+0000adc0: 0700 0000 0f55 706c 6f61 6465 7254 6162  .....UploaderTab
+0000add0: 7341 6c6c 0103 0000 00ce 0042 0069 0074  sAll.......B.i.t
+0000ade0: 0074 0065 0020 0076 0065 0072 0077 0065  .t.e. .v.e.r.w.e
+0000adf0: 006e 0064 0065 006e 0020 0053 0069 0065  .n.d.e.n. .S.i.e
+0000ae00: 0020 0049 0068 0072 0065 006e 0020 0057  . .I.h.r.e.n. .W
+0000ae10: 0065 0062 0062 0072 006f 0077 0073 0065  .e.b.b.r.o.w.s.e
+0000ae20: 0072 002c 0020 0075 006d 0020 0050 0068  .r.,. .u.m. .P.h
+0000ae30: 006f 0074 0069 006e 0069 0020 007a 0075  .o.t.i.n.i. .z.u
+0000ae40: 0020 0061 0075 0074 006f 0072 0069 0073  . .a.u.t.o.r.i.s
+0000ae50: 0069 0065 0072 0065 006e 002c 0020 0075  .i.e.r.e.n.,. .u
+0000ae60: 006e 0064 0020 0073 0063 0068 006c 0069  .n.d. .s.c.h.l.i
+0000ae70: 0065 00df 0065 006e 0020 0053 0069 0065  .e...e.n. .S.i.e
+0000ae80: 0020 0064 0061 006e 006e 0020 0064 0069  . .d.a.n.n. .d.i
+0000ae90: 0065 0073 0065 006e 0020 0044 0069 0061  .e.s.e.n. .D.i.a
+0000aea0: 006c 006f 0067 002e 0800 0000 0006 0000  .l.o.g..........
+0000aeb0: 004d 506c 6561 7365 2075 7365 2079 6f75  .MPlease use you
+0000aec0: 7220 7765 6220 6272 6f77 7365 7220 746f  r web browser to
+0000aed0: 2061 7574 686f 7269 7365 2050 686f 7469   authorise Photi
+0000aee0: 6e69 2c20 616e 6420 7468 656e 2063 6c6f  ni, and then clo
+0000aef0: 7365 2074 6869 7320 6469 616c 6f67 2e07  se this dialog..
+0000af00: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
+0000af10: 416c 6c01 0300 0000 1600 4600 6f00 7200  All.......F.o.r.
+0000af20: 7400 7300 6300 6800 7200 6900 7400 7408  t.s.c.h.r.i.t.t.
+0000af30: 0000 0000 0600 0000 0850 726f 6772 6573  .........Progres
+0000af40: 7307 0000 000f 5570 6c6f 6164 6572 5461  s.....UploaderTa
+0000af50: 6273 416c 6c01 0300 0000 1a00 4200 6900  bsAll.......B.i.
+0000af60: 6c00 6400 2000 6500 7200 7300 6500 7400  l.d. .e.r.s.e.t.
+0000af70: 7a00 6500 6e08 0000 0000 0600 0000 0d52  z.e.n..........R
+0000af80: 6570 6c61 6365 2069 6d61 6765 0700 0000  eplace image....
+0000af90: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
+0000afa0: 0103 0000 001c 0050 0068 006f 0074 006f  .......P.h.o.t.o
+0000afb0: 0020 0065 0072 0073 0065 0074 007a 0065  . .e.r.s.e.t.z.e
+0000afc0: 006e 0800 0000 0006 0000 000d 5265 706c  .n..........Repl
+0000afd0: 6163 6520 7068 6f74 6f07 0000 000f 5570  ace photo.....Up
+0000afe0: 6c6f 6164 6572 5461 6273 416c 6c01 0300  loaderTabsAll...
+0000aff0: 0000 1c00 4200 6900 6c00 6400 2000 6100  ....B.i.l.d. .a.
+0000b000: 7500 7300 7700 e400 6800 6c00 6500 6e08  u.s.w...h.l.e.n.
+0000b010: 0000 0000 0600 0000 0f53 656c 6563 7420  .........Select 
+0000b020: 616e 2069 6d61 6765 0700 0000 0f55 706c  an image.....Upl
+0000b030: 6f61 6465 7254 6162 7341 6c6c 0103 0000  oaderTabsAll....
+0000b040: 0018 00dc 0062 0065 0072 0073 0070 0072  .....b.e.r.s.p.r
+0000b050: 0069 006e 0067 0065 006e 0800 0000 0006  .i.n.g.e.n......
+0000b060: 0000 0004 536b 6970 0700 0000 0f55 706c  ....Skip.....Upl
+0000b070: 6f61 6465 7254 6162 7341 6c6c 0103 0000  oaderTabsAll....
+0000b080: 0022 0048 006f 0063 0068 006c 0061 0064  .".H.o.c.h.l.a.d
+0000b090: 0065 006e 0020 0073 0074 0061 0072 0074  .e.n. .s.t.a.r.t
+0000b0a0: 0065 006e 0800 0000 0006 0000 000c 5374  .e.n..........St
+0000b0b0: 6172 7420 7570 6c6f 6164 0700 0000 0f55  art upload.....U
+0000b0c0: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
+0000b0d0: 0000 0022 0048 006f 0063 0068 006c 0061  ...".H.o.c.h.l.a
+0000b0e0: 0064 0065 006e 0020 0073 0074 006f 0070  .d.e.n. .s.t.o.p
+0000b0f0: 0070 0065 006e 0800 0000 0006 0000 000b  .p.e.n..........
+0000b100: 5374 6f70 2075 706c 6f61 6407 0000 000f  Stop upload.....
+0000b110: 5570 6c6f 6164 6572 5461 6273 416c 6c01  UploaderTabsAll.
+0000b120: 0300 0000 3200 4100 6c00 7300 2000 6e00  ....2.A.l.s. .n.
+0000b130: 6500 7500 6500 7300 2000 5000 6800 6f00  e.u.e.s. .P.h.o.
+0000b140: 7400 6f00 2000 6800 6f00 6300 6800 6c00  t.o. .h.o.c.h.l.
+0000b150: 6100 6400 6500 6e08 0000 0000 0600 0000  a.d.e.n.........
+0000b160: 1355 706c 6f61 6420 6173 206e 6577 2070  .Upload as new p
+0000b170: 686f 746f 0700 0000 0f55 706c 6f61 6465  hoto.....Uploade
+0000b180: 7254 6162 7341 6c6c 0103 0000 005a 0048  rTabsAll.....Z.H
+0000b190: 006f 0063 0068 006c 0061 0064 0065 006e  .o.c.h.l.a.d.e.n
+0000b1a0: 0020 006e 0061 0063 0068 0020 007b 0073  . .n.a.c.h. .{.s
+0000b1b0: 0065 0072 0076 0069 0063 0065 007d 0020  .e.r.v.i.c.e.}. 
+0000b1c0: 0077 0075 0072 0064 0065 0020 006e 0069  .w.u.r.d.e. .n.i
+0000b1d0: 0063 0068 0074 0020 0062 0065 0065 006e  .c.h.t. .b.e.e.n
+0000b1e0: 0064 0065 0074 002e 0800 0000 0006 0000  .d.e.t..........
+0000b1f0: 0025 5570 6c6f 6164 2074 6f20 7b73 6572  .%Upload to {ser
+0000b200: 7669 6365 7d20 6861 7320 6e6f 7420 6669  vice} has not fi
+0000b210: 6e69 7368 6564 2e07 0000 000f 5570 6c6f  nished......Uplo
+0000b220: 6164 6572 5461 6273 416c 6c01 0300 0000  aderTabsAll.....
+0000b230: 6800 5700 6500 6c00 6300 6800 6500 2000  h.W.e.l.c.h.e. .
+0000b240: 4200 6900 6c00 6400 6400 6100 7400 6500  B.i.l.d.d.a.t.e.
+0000b250: 6900 2000 7000 6100 7300 7300 7400 2000  i. .p.a.s.s.t. .
+0000b260: 7a00 7500 2000 6400 6900 6500 7300 6500  z.u. .d.i.e.s.e.
+0000b270: 6d00 2000 4200 6900 6c00 6400 2000 6100  m. .B.i.l.d. .a.
+0000b280: 7500 6600 2000 7b00 7300 6500 7200 7600  u.f. .{.s.e.r.v.
+0000b290: 6900 6300 6500 7d00 3f08 0000 0000 0600  i.c.e.}.?.......
+0000b2a0: 0000 3357 6869 6368 2069 6d61 6765 2066  ..3Which image f
+0000b2b0: 696c 6520 6d61 7463 6865 7320 7468 6973  ile matches this
+0000b2c0: 2070 6963 7475 7265 206f 6e20 7b73 6572   picture on {ser
+0000b2d0: 7669 6365 7d3f 0700 0000 0f55 706c 6f61  vice}?.....Uploa
+0000b2e0: 6465 7254 6162 7341 6c6c 0103 0000 0050  derTabsAll.....P
+0000b2f0: 004d 00f6 0063 0068 0074 0065 006e 0020  .M...c.h.t.e.n. 
+0000b300: 0053 0069 0065 0020 0065 0073 0020 0069  .S.i.e. .e.s. .i
+0000b310: 006e 0020 0065 0069 006e 0020 004a 0050  .n. .e.i.n. .J.P
+0000b320: 0045 0047 0020 006b 006f 006e 0076 0065  .E.G. .k.o.n.v.e
+0000b330: 0072 0074 0069 0065 0072 0065 006e 003f  .r.t.i.e.r.e.n.?
+0000b340: 0800 0000 0006 0000 0025 576f 756c 6420  .........%Would 
+0000b350: 796f 7520 6c69 6b65 2074 6f20 636f 6e76  you like to conv
+0000b360: 6572 7420 6974 2074 6f20 4a50 4547 3f07  ert it to JPEG?.
+0000b370: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
+0000b380: 416c 6c01 0300 0000 3a00 4d00 f600 6300  All.....:.M...c.
+0000b390: 6800 7400 6500 6e00 2000 5300 6900 6500  h.t.e.n. .S.i.e.
+0000b3a0: 2000 6400 6900 6500 2000 4700 7200 f600   .d.i.e. .G.r...
+0000b3b0: df00 6500 2000 e400 6e00 6400 6500 7200  ..e. ...n.d.e.r.
+0000b3c0: 6e00 3f08 0000 0000 0600 0000 1c57 6f75  n.?..........Wou
+0000b3d0: 6c64 2079 6f75 206c 696b 6520 746f 2072  ld you like to r
+0000b3e0: 6573 697a 6520 6974 3f07 0000 000f 5570  esize it?.....Up
+0000b3f0: 6c6f 6164 6572 5461 6273 416c 6c01 0300  loaderTabsAll...
+0000b400: 0000 4400 4d00 f600 6300 6800 7400 6500  ..D.M...c.h.t.e.
+0000b410: 6e00 2000 5300 6900 6500 2000 6500 7300  n. .S.i.e. .e.s.
+0000b420: 2000 7400 7200 6f00 7400 7a00 6400 6500   .t.r.o.t.z.d.e.
+0000b430: 6d00 2000 6800 6f00 6300 6800 6c00 6100  m. .h.o.c.h.l.a.
+0000b440: 6400 6500 6e00 3f08 0000 0000 0600 0000  d.e.n.?.........
+0000b450: 2357 6f75 6c64 2079 6f75 206c 696b 6520  #Would you like 
+0000b460: 746f 2075 706c 6f61 6420 6974 2061 6e79  to upload it any
+0000b470: 7761 793f 0700 0000 0f55 706c 6f61 6465  way?.....Uploade
+0000b480: 7254 6162 7341 6c6c 0103 0000 005e 0044  rTabsAll.....^.D
+0000b490: 0061 0073 0020 0042 0072 006f 0077 0073  .a.s. .B.r.o.w.s
+0000b4a0: 0065 0072 0066 0065 006e 0073 0074 0065  .e.r.f.e.n.s.t.e
+0000b4b0: 0072 0020 006b 0061 006e 006e 0020 006e  .r. .k.a.n.n. .n
+0000b4c0: 0075 006e 0020 0067 0065 0073 0063 0068  .u.n. .g.e.s.c.h
+0000b4d0: 006c 006f 0073 0073 0065 006e 0020 0077  .l.o.s.s.e.n. .w
+0000b4e0: 0065 0072 0064 0065 006e 002e 0800 0000  .e.r.d.e.n......
+0000b4f0: 0006 0000 0026 596f 7520 6d61 7920 6e6f  .....&You may no
+0000b500: 7720 636c 6f73 6520 7468 6973 2062 726f  w close this bro
+0000b510: 7773 6572 2077 696e 646f 772e 0700 0000  wser window.....
+0000b520: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
+0000b530: 0103 0000 001e 003c 004d 0065 0068 0072  .......<.M.e.h.r
+0000b540: 0066 0061 0063 0068 0077 0065 0072 0074  .f.a.c.h.w.e.r.t
+0000b550: 0065 003e 0800 0000 0006 0000 0011 3c6d  .e.>..........<m
+0000b560: 756c 7469 706c 6520 7661 6c75 6573 3e07  ultiple values>.
+0000b570: 0000 0007 5769 6467 6574 7301 0300 0000  ....Widgets.....
+0000b580: 1400 3c00 6d00 6500 6800 7200 6600 6100  ..<.m.e.h.r.f.a.
+0000b590: 6300 6800 3e08 0000 0000 0600 0000 0a3c  c.h.>..........<
+0000b5a0: 6d75 6c74 6970 6c65 3e07 0000 0007 5769  multiple>.....Wi
+0000b5b0: 6467 6574 7301 0300 0000 0a00 3c00 6e00  dgets.......<.n.
+0000b5c0: 6500 7500 3e08 0000 0000 0600 0000 053c  e.u.>..........<
+0000b5d0: 6e65 773e 0700 0000 0757 6964 6765 7473  new>.....Widgets
+0000b5e0: 0188 0000 0002 0101                      ........
```

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.en.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.en.qm`

 * *Files 4% similar despite different names*

```diff
@@ -1,1796 +1,1821 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0265 6e42 0000 0d80 0000 5a6c  .....enB......Zl
-00000020: 0000 3e78 0000 7388 0000 567a 0000 73fe  ..>x..s...Vz..s.
-00000030: 0000 569e 0004 a0b9 0000 00d1 0004 a0b9  ..V.............
-00000040: 0000 346d 0004 bda9 0000 2cdb 0004 d025  ..4m......,....%
-00000050: 0000 2e5d 0004 ec30 0000 2eaf 0005 4835  ...]...0......H5
-00000060: 0000 0532 0005 4835 0000 3cf1 0005 4835  ...2..H5..<...H5
-00000070: 0000 4bad 0005 8c04 0000 3023 0005 9625  ..K.......0#...%
-00000080: 0000 4d2b 0005 97c5 0000 1647 0005 a200  ..M+.......G....
-00000090: 0000 5fa2 0007 c4af 0000 1e0f 0012 2b0e  .._...........+.
-000000a0: 0000 2c20 001c da4d 0000 27fd 001c dbdd  .., ...M..'.....
-000000b0: 0000 5d10 0024 12d5 0000 1d1c 002c f63e  ..]..$.......,.>
-000000c0: 0000 0b08 002d 8634 0000 46fc 002f a5f5  .....-.4..F../..
-000000d0: 0000 3575 0037 171b 0000 46ca 003b f105  ..5u.7....F..;..
-000000e0: 0000 0d31 0040 e4ce 0000 61d0 0043 4cae  ...1.@....a..CL.
-000000f0: 0000 626d 0047 c4e3 0000 5e31 004b 87d4  ..bm.G....^1.K..
-00000100: 0000 43fa 004d 5005 0000 4262 0056 aec2  ..C..MP...Bb.V..
-00000110: 0000 4581 0056 aec2 0000 54b6 0056 f6af  ..E..V....T..V..
-00000120: 0000 154d 005a 81be 0000 5615 005b 0b25  ...M.Z....V..[.%
-00000130: 0000 16e4 005b 0b25 0000 27d8 005b 0b25  .....[.%..'..[.%
-00000140: 0000 4751 0060 1085 0000 45d7 0067 aad3  ..GQ.`....E..g..
-00000150: 0000 2e7d 0069 a403 0000 1b47 0069 a403  ...}.i.....G.i..
-00000160: 0000 2ecf 006c c199 0000 1319 0071 0769  .....l.......q.i
-00000170: 0000 325b 0077 0ebc 0000 4f8f 0094 cf02  ..2[.w....O.....
-00000180: 0000 55e7 00a2 1470 0000 5831 00a3 85ee  ..U....p..X1....
-00000190: 0000 0408 00b8 6470 0000 57d7 00bd d20e  ......dp..W.....
-000001a0: 0000 5ae7 00c0 dd34 0000 2488 00c6 1d14  ..Z....4..$.....
-000001b0: 0000 5cb1 00c6 6470 0000 5804 00d1 9ab5  ..\...dp..X.....
-000001c0: 0000 5dc2 00d7 0cb9 0000 1c2e 00dc 0fc4  ..].............
-000001d0: 0000 486a 00ec 29c4 0000 460f 00f2 f2c8  ..Hj..)...F.....
-000001e0: 0000 1458 0106 6074 0000 28bf 0113 87c5  ...X..`t..(.....
-000001f0: 0000 5548 011d e755 0000 2419 0126 bda5  ..UH...U..$..&..
-00000200: 0000 359d 0145 eb79 0000 197b 015e eb2f  ..5..E.y...{.^./
-00000210: 0000 6149 015f 0dad 0000 1935 0163 c933  ..aI._.....5.c.3
-00000220: 0000 0fea 016a 032e 0000 373d 0173 8fc8  .....j....7=.s..
-00000230: 0000 5ce4 0180 6a59 0000 2d42 018e d47e  ..\...jY..-B...~
-00000240: 0000 0904 018f 97f8 0000 5401 01be 34b7  ..........T...4.
-00000250: 0000 5335 01c1 faa5 0000 136a 01c1 faa5  ..S5.......j....
-00000260: 0000 4896 01c5 f5cd 0000 5943 01ca 84a1  ..H.......YC....
-00000270: 0000 406e 01d2 e96e 0000 2ef5 01d8 cd24  ..@n...n.......$
-00000280: 0000 1e31 01e4 e113 0000 585e 01f7 4f45  ...1......X^..OE
-00000290: 0000 35f7 01fc 7925 0000 2c8e 01fd 69a5  ..5...y%..,...i.
-000002a0: 0000 0e1c 0201 ff63 0000 50a2 0232 05d5  .......c..P..2..
-000002b0: 0000 229c 0249 c9ae 0000 5e70 026d bc14  .."..I....^p.m..
-000002c0: 0000 5fca 0277 2b35 0000 1d9a 0286 e00e  .._..w+5........
-000002d0: 0000 093c 0296 5357 0000 2bd6 0298 5c09  ...<..SW..+...\.
-000002e0: 0000 337f 029f e98c 0000 41e7 02c8 9fa3  ..3.......A.....
-000002f0: 0000 115e 02cf fca5 0000 19c7 02d6 0815  ...^............
-00000300: 0000 5f6f 02f3 9dc3 0000 41b3 02f9 c4c5  .._o......A.....
-00000310: 0000 1486 02f9 c4c5 0000 2699 02f9 c4c5  ..........&.....
-00000320: 0000 44fb 0302 20f5 0000 296c 0305 1aa9  ..D... ...)l....
-00000330: 0000 24e5 030c 9764 0000 2fc7 0334 c2be  ..$....d../..4..
-00000340: 0000 3ab3 0354 44bd 0000 1ad6 0359 7694  ..:..TD......Yv.
-00000350: 0000 5c42 035a 4e6e 0000 3995 037d 2417  ..\B.ZNn..9..}$.
-00000360: 0000 58c9 037d 9c24 0000 45a6 037f eb99  ..X..}.$..E.....
-00000370: 0000 3621 0380 b55f 0000 6029 0391 ff0e  ..6!..._..`)....
-00000380: 0000 02eb 039a 6ece 0000 5bdc 03b0 bf25  ......n...[....%
-00000390: 0000 0068 03b0 bf25 0000 3fe7 03b4 664e  ...h...%..?...fN
-000003a0: 0000 6247 03b5 83a3 0000 43ca 03e2 d39e  ..bG......C.....
-000003b0: 0000 0776 03e6 8545 0000 3e22 03ef 1f79  ...v...E..>"...y
-000003c0: 0000 1a8f 03f1 1a05 0000 539f 03ff d948  ..........S....H
-000003d0: 0000 529d 0409 59a5 0000 3d6c 040e 9e79  ..R...Y...=l...y
-000003e0: 0000 2711 041f dd3e 0000 49ba 0442 4dfe  ..'....>..I..BM.
-000003f0: 0000 3fba 0447 966e 0000 4efb 044c 1eee  ..?..G.n..N..L..
-00000400: 0000 5a6d 0457 019e 0000 0384 0459 8f63  ..Zm.W.......Y.c
-00000410: 0000 306b 045f e8c9 0000 0d90 0460 e588  ..0k._.......`..
-00000420: 0000 2d09 0498 3c81 0000 5174 04ab 7ea5  ..-...<...Qt..~.
-00000430: 0000 299a 04c8 4039 0000 13bd 04c8 4039  ..)...@9......@9
-00000440: 0000 25a8 04d0 e082 0000 55ad 04d2 fa22  ..%.......U...."
-00000450: 0000 13e1 04d3 9ff4 0000 1838 04f5 7367  ...........8..sg
-00000460: 0000 151e 0515 8cbe 0000 4ca0 051a 65f5  ..........L...e.
-00000470: 0000 5d84 0520 62a4 0000 3f10 0528 4ac0  ..].. b...?..(J.
-00000480: 0000 291a 052d 4d3c 0000 12b4 0530 af74  ..)..-M<.....0.t
-00000490: 0000 4776 0531 a702 0000 20d9 0535 96fe  ..Gv.1.... ..5..
-000004a0: 0000 5c18 0537 8957 0000 1130 053b 7b05  ..\..7.W...0.;{.
-000004b0: 0000 14f8 053b 7b05 0000 26e9 053e 782d  .....;{...&..>x-
-000004c0: 0000 21e5 0544 794d 0000 21b0 055f 746e  ..!..DyM..!.._tn
-000004d0: 0000 5b2c 0565 06e3 0000 0693 0577 76ec  ..[,.e.......wv.
-000004e0: 0000 52ca 057b 92f3 0000 1595 057b 92f3  ..R..{.......{..
-000004f0: 0000 4666 0588 b047 0000 0d08 058b e05e  ..Ff...G.......^
-00000500: 0000 057c 058f dfb3 0000 3dff 059b 8898  ...|......=.....
-00000510: 0000 409c 05a0 71ff 0000 5253 05a3 3419  ..@...q...RS..4.
-00000520: 0000 3f3a 05a6 17ae 0000 436a 05a6 c895  ..?:......Cj....
-00000530: 0000 210b 05a9 c6ae 0000 3ec0 05ab 3502  ..!.......>...5.
-00000540: 0000 4aa8 05ab 8bc4 0000 05a1 05ac 8de5  ..J.............
-00000550: 0000 14ab 05af caf4 0000 5461 05b3 f92e  ..........Ta....
-00000560: 0000 2ad5 05b9 6619 0000 0e49 05d3 4c4e  ..*...f....I..LN
-00000570: 0000 3f8c 05dd d675 0000 348e 05e9 9749  ..?....u..4....I
-00000580: 0000 4637 05fe 219e 0000 548a 0602 a46e  ..F7..!...T....n
-00000590: 0000 4a37 0618 f51e 0000 39e7 0626 dcc9  ..J7......9..&..
-000005a0: 0000 2131 0627 7c75 0000 215a 063b cf25  ..!1.'|u..!Z.;.%
-000005b0: 0000 1b15 0647 6c6e 0000 1f07 064f 4f8e  .....Gln.....OO.
-000005c0: 0000 38d0 0653 24e5 0000 4303 065a 7e13  ..8..S$...C..Z~.
-000005d0: 0000 24bd 0667 a1fe 0000 4522 066a 3ba3  ..$..g....E".j;.
-000005e0: 0000 1054 067b 0603 0000 2f3a 067c 1595  ...T.{..../:.|..
-000005f0: 0000 1de8 068d 7d90 0000 400e 068f 2045  ......}...@... E
-00000600: 0000 2313 0698 3c81 0000 05c6 069d bc4e  ..#...<........N
-00000610: 0000 0a21 06a3 1c7f 0000 47cb 06a5 c6b5  ...!......G.....
-00000620: 0000 4bd0 06b7 eb69 0000 1734 06ba eeff  ..K....i...4....
-00000630: 0000 6189 06c3 25ee 0000 3815 06c3 2be7  ..a...%...8...+.
-00000640: 0000 30ba 06c9 55b9 0000 2671 06c9 b805  ..0...U...&q....
-00000650: 0000 50cf 06ce 697e 0000 1fa7 06d4 e879  ..P...i~.......y
-00000660: 0000 19f6 06e7 88c7 0000 2aa9 06ea 1312  ..........*.....
-00000670: 0000 204f 06f1 acb5 0000 4042 0706 6093  .. O......@B..`.
-00000680: 0000 3e98 0717 352e 0000 4c21 071b d822  ..>...5...L!..."
-00000690: 0000 5df8 0725 0ed3 0000 1f7c 072a 02b3  ..]..%.....|.*..
-000006a0: 0000 1eab 072b 5bf1 0000 54dc 073b 0713  .....+[...T..;..
-000006b0: 0000 1fe9 073e 8aae 0000 18a2 0740 7b19  .....>.......@{.
-000006c0: 0000 1ba2 0745 d72e 0000 621a 0747 58b5  .....E....b..GX.
-000006d0: 0000 18fe 0752 93ae 0000 011a 0756 937c  .....R.......V.|
-000006e0: 0000 56c2 0761 5de5 0000 0e7d 0773 020e  ..V..a]....}.s..
-000006f0: 0000 59f1 0778 9733 0000 5513 077c e91e  ..Y..x.3..U..|..
-00000700: 0000 1d72 077d e8e5 0000 3546 0783 2294  ...r.}....5F..".
-00000710: 0000 0f74 078c 0ba4 0000 0d67 0790 c8f5  ...t.......g....
-00000720: 0000 1570 0791 9109 0000 2577 0799 f1c5  ...p......%w....
-00000730: 0000 42a6 079d a354 0000 5ffa 07a1 d6cb  ..B....T.._.....
-00000740: 0000 2ff1 07ab 8e03 0000 0000 07b4 0f05  ../.............
-00000750: 0000 3da4 07c3 bd54 0000 5760 07c9 d658  ..=....T..W`...X
-00000760: 0000 4c77 07e0 1a4f 0000 1a50 07ee 2434  ..Lw...O...P..$4
-00000770: 0000 4f59 07f6 6e0f 0000 5b5f 0812 7098  ..OY..n...[_..p.
-00000780: 0000 40c1 0842 126e 0000 2f5d 0843 f97e  ..@..B.n../].C.~
-00000790: 0000 0bad 0847 159e 0000 58f9 084e b2f5  .....G....X..N..
-000007a0: 0000 2942 0876 6c3e 0000 0179 088b 0b9e  ..)B.vl>...y....
-000007b0: 0000 3ba8 089b d2f1 0000 4fda 08a4 2089  ..;.......O... .
-000007c0: 0000 4335 08ad 8b6e 0000 3a50 08ae abbe  ..C5...n..:P....
-000007d0: 0000 0148 08bc 210e 0000 0747 08bd 8ce8  ...H..!....G....
-000007e0: 0000 221a 08f0 ac75 0000 1084 08fb ecd3  .."....u........
-000007f0: 0000 2e04 08ff ed5f 0000 1794 0907 6914  ......._......i.
-00000800: 0000 40f3 090d 6f19 0000 0c6b 091d 05f0  ..@...o....k....
-00000810: 0000 3dcc 0920 f035 0000 3c98 0923 8a14  ..=.. .5..<..#..
-00000820: 0000 588f 092a 03d5 0000 0027 092c eb99  ..X..*.....'.,..
-00000830: 0000 08c9 0938 bd9e 0000 3503 0941 e34c  .....8....5..A.L
-00000840: 0000 0f14 0949 9184 0000 4155 0949 b384  .....I....AU.I..
-00000850: 0000 3200 094d 67fe 0000 1394 094d 67fe  ..2..Mg......Mg.
-00000860: 0000 2524 094d 67fe 0000 439f 094d 67fe  ..%$.Mg...C..Mg.
-00000870: 0000 4919 095e 89d3 0000 5ee1 0968 7d7d  ..I..^....^..h}}
-00000880: 0000 14d1 0968 7d7d 0000 18d1 0968 7d7d  .....h}}.....h}}
-00000890: 0000 26c0 096d 01e5 0000 0555 096f 9788  ..&..m.....U.o..
-000008a0: 0000 53cc 0974 a647 0000 2b48 0977 0c94  ..S..t.G..+H.w..
-000008b0: 0000 4bf9 097c 1775 0000 1dc1 0987 b01e  ..K..|.u........
-000008c0: 0000 42dc 09c2 2cce 0000 4ad1 09ca a91e  ..B...,...J.....
-000008d0: 0000 393a 09ee 202e 0000 0a8f 09f5 9023  ..9:.. ........#
-000008e0: 0000 285d 0a0d 74f2 0000 0617 0a0d 74f2  ..(]..t.......t.
-000008f0: 0000 2f8e 0a3b 8333 0000 048b 0a69 66c9  ../..;.3.....if.
-00000900: 0000 1cf7 0a6c 5bd9 0000 00f4 0a6c 5bd9  .....l[......l[.
-00000910: 0000 34bb 0a73 2a51 0000 1b6f 0a76 0292  ..4..s*Q...o.v..
-00000920: 0000 472a 0a7f ce9e 0000 6060 0a89 b649  ..G*......``...I
-00000930: 0000 142a 0a8b 8b22 0000 34df 0a8b d95e  ...*..."..4....^
-00000940: 0000 1cb7 0a99 6ff8 0000 563b 0ab7 5d54  ......o...V;..]T
-00000950: 0000 0508 0ac3 dd9f 0000 441f 0ac7 826e  ..........D....n
-00000960: 0000 03c1 0acd eec7 0000 244b 0ad6 d87e  ..........$K...~
-00000970: 0000 0230 0ae9 b7f5 0000 1222 0aea 9594  ...0......."....
-00000980: 0000 10b8 0afb 86b9 0000 2bac 0b0c 7643  ..........+...vC
-00000990: 0000 35cc 0b0c 8953 0000 1871 0b16 9077  ..5....S...q...w
-000009a0: 0000 04cf 0b1c 6fee 0000 008f 0b31 6541  ......o......1eA
-000009b0: 0000 070f 0b32 f535 0000 2890 0b4d 2eee  .....2.5..(..M..
-000009c0: 0000 36c2 0b52 aea4 0000 2241 0b55 9355  ..6..R...."A.U.U
-000009d0: 0000 5d4e 0b69 37c9 0000 33d6 0b6f 5c75  ..]N.i7...3..o\u
-000009e0: 0000 5372 0b70 d229 0000 1707 0b7b 2ca5  ..Sr.p.).....{,.
-000009f0: 0000 0cb2 0b81 700e 0000 3646 0b82 249e  ......p...6F..$.
-00000a00: 0000 034a 0b8a 2614 0000 161f 0b8a 9d0e  ...J..&.........
-00000a10: 0000 4ccb 0ba0 757f 0000 60a9 0ba0 9785  ..L...u...`.....
-00000a20: 0000 235f 0ba0 c9de 0000 5583 0ba3 fc0c  ..#_......U.....
-00000a30: 0000 2085 0ba4 08e7 0000 20af 0bbf 620d  .. ....... ...b.
-00000a40: 0000 0650 0bc0 05e4 0000 1693 0bc0 93e3  ...P............
-00000a50: 0000 4b80 0be2 cc85 0000 479e 0be4 0395  ..K.......G.....
-00000a60: 0000 5436 0bf0 2bfe 0000 01ba 0bf0 453e  ..T6..+.......E>
-00000a70: 0000 0fae 0c13 2b8e 0000 1f36 0c1a b9a5  ......+....6....
-00000a80: 0000 2b7e 0c20 4f43 0000 3e4d 0c25 7849  ..+~. OC..>M.%xI
-00000a90: 0000 3293 0c27 e76f 0000 6100 0c28 b745  ..2..'.o..a..(.E
-00000aa0: 0000 4fb3 0c29 84a3 0000 1d48 0c35 9b9e  ..O..).....H.5..
-00000ab0: 0000 341c 0c4c 8c75 0000 44d3 0c4f 0f0e  ..4..L.u..D..O..
-00000ac0: 0000 4d4e 0c5d e1c2 0000 1190 0c5e 6fb4  ..MN.].......^o.
-00000ad0: 0000 2183 0c7d 7095 0000 1288 0c80 8aa3  ..!..}p.........
-00000ae0: 0000 1c8d 0c80 8aa3 0000 3043 0c93 93be  ..........0C....
-00000af0: 0000 315f 0c94 ba43 0000 06d2 0ca0 d5c3  ..1_...C........
-00000b00: 0000 0f42 0cbb 0173 0000 3096 0cc2 0d7e  ...B...s..0....~
-00000b10: 0000 519b 0cca 0285 0000 254f 0cce 648d  ..Q.......%O..d.
-00000b20: 0000 5c6d 0cd8 f02d 0000 05eb 0d04 cb1e  ..\m...-........
-00000b30: 0000 1ed9 0d0e 50f8 0000 48ed 0d0e 6da3  ......P...H...m.
-00000b40: 0000 0cdd 0d19 6c99 0000 25fe 0d34 07f1  ......l...%..4..
-00000b50: 0000 0ee2 0d34 6913 0000 4220 0d36 9b85  .....4i...B .6..
-00000b60: 0000 3230 0d49 166e 0000 48c1 0d86 3e6e  ..20.I.n..H...>n
-00000b70: 0000 30de 0d8c 40ce 0000 3f61 0d8f b523  ..0...@...?a...#
-00000b80: 0000 15b9 0d8f b523 0000 2743 0d8f c4f3  .......#..'C....
-00000b90: 0000 1405 0d8f c4f3 0000 264a 0d96 5b13  ..........&J..[.
-00000ba0: 0000 1026 0d96 f824 0000 10e4 0da7 df9e  ...&...$........
-00000bb0: 0000 4943 0db0 6493 0000 25ce 0dba 6f39  ..IC..d...%...o9
-00000bc0: 0000 3325 0dc9 1a88 0000 1253 0dd7 f89b  ..3%.......S....
-00000bd0: 0000 2e2f 0e03 0de0 0000 11ed 0e03 0de0  .../............
-00000be0: 0000 23e2 0e0b 4344 0000 5229 0e0c 2965  ..#...CD..R)..)e
-00000bf0: 0000 23a9 0e10 6e3e 0000 4816 0e14 c055  ..#...n>..H....U
-00000c00: 0000 2dd8 0e2c 0f2e 0000 4553 0e31 45cf  ..-..,....ES.1E.
-00000c10: 0000 5039 0e39 c321 0000 31d0 0e6e 2258  ..P9.9.!..1..n"X
-00000c20: 0000 5136 0e6e 4858 0000 50f8 0e6f 36c5  ..Q6.nHX..P..o6.
-00000c30: 0000 4c4b 0e95 28b5 0000 0dc0 0e97 bcb5  ..LK..(.........
-00000c40: 0000 0dee 0e9c a374 0000 571f 0e9e 60ae  .......t..W...`.
-00000c50: 0000 2a3d 0ea2 ec1e 0000 4e6f 0ea3 b08e  ..*=......No....
-00000c60: 0000 028c 0eaf 6fc3 0000 3cc8 0eb6 b7de  ......o...<.....
-00000c70: 0000 4dec 0ebe c4c3 0000 4123 0ec1 ac3f  ..M.......A#...?
-00000c80: 0000 28ed 0ed2 6f37 0000 52f5 0ed2 862e  ..(...o7..R.....
-00000c90: 0000 37bf 0edb 53e1 0000 15f1 0edb 53e1  ..7...S.......S.
-00000ca0: 0000 277d 0edd a743 0000 0eb2 0edf 208d  ..'}...C...... .
-00000cb0: 0000 57a1 0eeb 97ce 0000 386e 0eed da75  ..W.......8n...u
-00000cc0: 0000 51fb 0eee 44a4 0000 56e9 0ef1 01de  ..Q...D...V.....
-00000cd0: 0000 2d6b 0ef6 09ee 0000 0449 0f05 000c  ..-k.......I....
-00000ce0: 0000 1669 0f16 93ca 0000 2835 0f31 815c  ...i......(5.1.\
-00000cf0: 0000 22d7 0f33 2495 0000 1765 0f48 89e2  .."..3$....e.H..
-00000d00: 0000 3d12 0f59 715e 0000 5977 0f62 0773  ..=..Yq^..Yw.b.s
-00000d10: 0000 2014 0f64 7a39 0000 3d47 0f66 4e29  .. ..dz9..=G.fN)
-00000d20: 0000 44a5 0f6f e836 0000 500e 0f74 5d8e  ..D..o.6..P..t].
-00000d30: 0000 3b2e 0f82 a059 0000 468c 0f8f 1b8e  ..;....Y..F.....
-00000d40: 0000 11bf 0f9a 906e 0000 29d0 0f9d 6ca9  .......n..)...l.
-00000d50: 0000 12e5 0fa8 b309 0000 32dc 0fa9 1015  ..........2.....
-00000d60: 0000 5f0d 0fb1 d16f 0000 5f3e 0fb6 b24e  .._....o.._>...N
-00000d70: 0000 3c41 0fd4 15de 0000 2271 0fd4 15de  ..<A......"q....
-00000d80: 0000 4188 0fe8 0889 0000 2c60 0fef 5405  ..A.......,`..T.
-00000d90: 0000 16bb 0fef 5405 0000 27ad 6900 0062  ......T...'.i..b
-00000da0: 8e03 ffff ffff 0800 0000 0006 0000 0008  ................
-00000db0: 2641 6464 7265 7373 0700 0000 0a41 6464  &Address.....Add
-00000dc0: 7265 7373 5461 6201 03ff ffff ff08 0000  ressTab.........
-00000dd0: 0000 0600 0000 2241 6464 7265 7373 206c  ......"Address l
-00000de0: 6f6f 6b75 7020 706f 7765 7265 6420 6279  ookup powered by
-00000df0: 204f 7065 6e43 6167 6507 0000 000a 4164   OpenCage.....Ad
-00000e00: 6472 6573 7354 6162 0103 ffff ffff 0800  dressTab........
-00000e10: 0000 0006 0000 0008 416c 7469 7475 6465  ........Altitude
-00000e20: 0700 0000 0a41 6464 7265 7373 5461 6201  .....AddressTab.
-00000e30: 03ff ffff ff08 0000 0000 0600 0000 2341  ..............#A
-00000e40: 6c74 6974 7564 6520 6f66 2074 6865 206c  ltitude of the l
-00000e50: 6f63 6174 696f 6e20 696e 206d 6574 7265  ocation in metre
-00000e60: 732e 0700 0000 0a41 6464 7265 7373 5461  s......AddressTa
-00000e70: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00000e80: 0443 6974 7907 0000 000a 4164 6472 6573  .City.....Addres
-00000e90: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
-00000ea0: 0000 0007 436f 756e 7472 7907 0000 000a  ....Country.....
-00000eb0: 4164 6472 6573 7354 6162 0103 ffff ffff  AddressTab......
-00000ec0: 0800 0000 0006 0000 000f 4465 6c65 7465  ..........Delete
-00000ed0: 206c 6f63 6174 696f 6e07 0000 000a 4164   location.....Ad
-00000ee0: 6472 6573 7354 6162 0103 ffff ffff 0800  dressTab........
-00000ef0: 0000 0006 0000 0012 4475 706c 6963 6174  ........Duplicat
-00000f00: 6520 6c6f 6361 7469 6f6e 0700 0000 0a41  e location.....A
-00000f10: 6464 7265 7373 5461 6201 03ff ffff ff08  ddressTab.......
-00000f20: 0000 0000 0600 0000 2245 6e74 6572 2061  ........"Enter a
-00000f30: 2066 756c 6c20 6e61 6d65 206f 6620 7468   full name of th
-00000f40: 6520 6c6f 6361 7469 6f6e 2e07 0000 000a  e location......
-00000f50: 4164 6472 6573 7354 6162 0103 ffff ffff  AddressTab......
-00000f60: 0800 0000 0006 0000 0057 456e 7465 7220  .........WEnter 
-00000f70: 676c 6f62 616c 6c79 2075 6e69 7175 6520  globally unique 
-00000f80: 6964 656e 7469 6669 6572 2873 2920 6f66  identifier(s) of
-00000f90: 2074 6865 206c 6f63 6174 696f 6e2e 2053   the location. S
-00000fa0: 6570 6172 6174 6520 7468 656d 2077 6974  eparate them wit
-00000fb0: 6820 223b 2220 6368 6172 6163 7465 7273  h ";" characters
-00000fc0: 2e07 0000 000a 4164 6472 6573 7354 6162  ......AddressTab
-00000fd0: 0103 ffff ffff 0800 0000 0006 0000 003d  ...............=
-00000fe0: 456e 7465 7220 7468 6520 3220 6f72 2033  Enter the 2 or 3
-00000ff0: 206c 6574 7465 7220 4953 4f20 3331 3636   letter ISO 3166
-00001000: 2063 6f75 6e74 7279 2063 6f64 6520 6f66   country code of
-00001010: 2074 6865 2063 6f75 6e74 7279 2e07 0000   the country....
-00001020: 000a 4164 6472 6573 7354 6162 0103 ffff  ..AddressTab....
-00001030: ffff 0800 0000 0006 0000 0040 456e 7465  ...........@Ente
-00001040: 7220 7468 6520 6465 7461 696c 7320 6162  r the details ab
-00001050: 6f75 7420 6120 6c6f 6361 7469 6f6e 2077  out a location w
-00001060: 6865 7265 2074 6869 7320 696d 6167 6520  here this image 
-00001070: 7761 7320 6372 6561 7465 642e 0700 0000  was created.....
-00001080: 0a41 6464 7265 7373 5461 6201 03ff ffff  .AddressTab.....
-00001090: ff08 0000 0000 0600 0000 4045 6e74 6572  ..........@Enter
-000010a0: 2074 6865 2064 6574 6169 6c73 2061 626f   the details abo
-000010b0: 7574 2061 206c 6f63 6174 696f 6e20 7768  ut a location wh
-000010c0: 6963 6820 6973 2073 686f 776e 2069 6e20  ich is shown in 
-000010d0: 7468 6973 2069 6d61 6765 2e07 0000 000a  this image......
-000010e0: 4164 6472 6573 7354 6162 0103 ffff ffff  AddressTab......
-000010f0: 0800 0000 0006 0000 001b 456e 7465 7220  ..........Enter 
-00001100: 7468 6520 6e61 6d65 206f 6620 7468 6520  the name of the 
-00001110: 6369 7479 2e07 0000 000a 4164 6472 6573  city......Addres
-00001120: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
-00001130: 0000 001e 456e 7465 7220 7468 6520 6e61  ....Enter the na
-00001140: 6d65 206f 6620 7468 6520 636f 756e 7472  me of the countr
-00001150: 792e 0700 0000 0a41 6464 7265 7373 5461  y......AddressTa
-00001160: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00001170: 2845 6e74 6572 2074 6865 206e 616d 6520  (Enter the name 
-00001180: 6f66 2074 6865 2070 726f 7669 6e63 6520  of the province 
-00001190: 6f72 2073 7461 7465 2e07 0000 000a 4164  or state......Ad
-000011a0: 6472 6573 7354 6162 0103 ffff ffff 0800  dressTab........
-000011b0: 0000 0006 0000 0022 456e 7465 7220 7468  ......."Enter th
-000011c0: 6520 6e61 6d65 206f 6620 7468 6520 7375  e name of the su
-000011d0: 626c 6f63 6174 696f 6e2e 0700 0000 0a41  blocation......A
-000011e0: 6464 7265 7373 5461 6201 03ff ffff ff08  ddressTab.......
-000011f0: 0000 0000 0600 0000 2345 6e74 6572 2074  ........#Enter t
-00001200: 6865 206e 616d 6520 6f66 2074 6865 2077  he name of the w
-00001210: 6f72 6c64 2072 6567 696f 6e2e 0700 0000  orld region.....
-00001220: 0a41 6464 7265 7373 5461 6201 03ff ffff  .AddressTab.....
-00001230: ff08 0000 0000 0600 0000 2547 656f 6461  ..........%Geoda
-00001240: 7461 20c2 a920 4f70 656e 5374 7265 6574  ta .. OpenStreet
-00001250: 4d61 7020 636f 6e74 7269 6275 746f 7273  Map contributors
-00001260: 0700 0000 0a41 6464 7265 7373 5461 6201  .....AddressTab.
-00001270: 03ff ffff ff08 0000 0000 0600 0000 1a47  ...............G
-00001280: 6574 2061 6464 7265 7373 2066 726f 6d20  et address from 
-00001290: 6c61 742c 206c 6f6e 6707 0000 000a 4164  lat, long.....Ad
-000012a0: 6472 6573 7354 6162 0103 ffff ffff 0800  dressTab........
-000012b0: 0000 0006 0000 000b 4c6f 6361 7469 6f6e  ........Location
-000012c0: 2049 4407 0000 000a 4164 6472 6573 7354   ID.....AddressT
-000012d0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-000012e0: 0004 4e61 6d65 0700 0000 0a41 6464 7265  ..Name.....Addre
-000012f0: 7373 5461 6201 03ff ffff ff08 0000 0000  ssTab...........
-00001300: 0600 0000 0850 726f 7669 6e63 6507 0000  .....Province...
-00001310: 000a 4164 6472 6573 7354 6162 0103 ffff  ..AddressTab....
-00001320: ffff 0800 0000 0006 0000 0006 5265 6769  ............Regi
-00001330: 6f6e 0700 0000 0a41 6464 7265 7373 5461  on.....AddressTa
-00001340: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00001350: 0653 7472 6565 7407 0000 000a 4164 6472  .Street.....Addr
-00001360: 6573 7354 6162 0103 ffff ffff 0800 0000  essTab..........
-00001370: 0006 0000 0006 6361 6d65 7261 0700 0000  ......camera....
-00001380: 0a41 6464 7265 7373 5461 6201 03ff ffff  .AddressTab.....
-00001390: ff08 0000 0000 0600 0000 0d73 7562 6a65  ...........subje
-000013a0: 6374 207b 6964 787d 0700 0000 0a41 6464  ct {idx}.....Add
-000013b0: 7265 7373 5461 6201 03ff ffff ff08 0000  ressTab.........
-000013c0: 0000 0600 0000 1d50 686f 7469 6e69 2070  .......Photini p
-000013d0: 686f 746f 206d 6574 6164 6174 6120 6564  hoto metadata ed
-000013e0: 6974 6f72 0700 0000 0743 4c49 4865 6c70  itor.....CLIHelp
-000013f0: 0103 ffff ffff 0800 0000 0006 0000 0027  ...............'
-00001400: 5573 6167 653a 2025 7072 6f67 205b 6f70  Usage: %prog [op
-00001410: 7469 6f6e 735d 205b 6669 6c65 5f6e 616d  tions] [file_nam
-00001420: 652c 202e 2e2e 5d07 0000 0007 434c 4948  e, ...].....CLIH
-00001430: 656c 7001 03ff ffff ff08 0000 0000 0600  elp.............
-00001440: 0000 2369 6e63 7265 6173 6520 6e75 6d62  ..#increase numb
-00001450: 6572 206f 6620 6c6f 6767 696e 6720 6d65  er of logging me
-00001460: 7373 6167 6573 0700 0000 0743 4c49 4865  ssages.....CLIHe
-00001470: 6c70 0103 ffff ffff 0800 0000 0006 0000  lp..............
-00001480: 0021 7465 7374 206e 6577 2066 6561 7475  .!test new featu
-00001490: 7265 7320 6f72 2041 5049 2076 6572 7369  res or API versi
-000014a0: 6f6e 7307 0000 0007 434c 4948 656c 7001  ons.....CLIHelp.
-000014b0: 03ff ffff ff08 0000 0000 0600 0000 1526  ...............&
-000014c0: 4465 7363 7269 7074 6976 6520 6d65 7461  Descriptive meta
-000014d0: 6461 7461 0700 0000 0e44 6573 6372 6970  data.....Descrip
-000014e0: 7469 7665 5461 6201 03ff ffff ff08 0000  tiveTab.........
-000014f0: 0000 0600 0000 0c3c 6661 766f 7572 6974  .......<favourit
-00001500: 6573 3e07 0000 000e 4465 7363 7269 7074  es>.....Descript
-00001510: 6976 6554 6162 0103 ffff ffff 0800 0000  iveTab..........
-00001520: 0006 0000 0130 4120 6d6f 7265 2064 6574  .....0A more det
-00001530: 6169 6c65 6420 7465 7874 7561 6c20 6465  ailed textual de
-00001540: 7363 7269 7074 696f 6e20 6f66 2074 6865  scription of the
-00001550: 2070 7572 706f 7365 2061 6e64 206d 6561   purpose and mea
-00001560: 6e69 6e67 206f 6620 616e 2069 6d61 6765  ning of an image
-00001570: 2074 6861 7420 656c 6162 6f72 6174 6573   that elaborates
-00001580: 206f 6e20 7468 6520 696e 666f 726d 6174   on the informat
-00001590: 696f 6e20 7072 6f76 6964 6564 2062 7920  ion provided by 
-000015a0: 7468 6520 416c 7420 5465 7874 2028 4163  the Alt Text (Ac
-000015b0: 6365 7373 6962 696c 6974 7929 2070 726f  cessibility) pro
-000015c0: 7065 7274 792e 2054 6869 7320 7072 6f70  perty. This prop
-000015d0: 6572 7479 2064 6f65 7320 6e6f 7420 6861  erty does not ha
-000015e0: 7665 2061 2063 6861 7261 6374 6572 206c  ve a character l
-000015f0: 696d 6974 6174 696f 6e20 616e 6420 6973  imitation and is
-00001600: 206e 6f74 2072 6571 7569 7265 6420 6966   not required if
-00001610: 2074 6865 2041 6c74 2054 6578 7420 2841   the Alt Text (A
-00001620: 6363 6573 7369 6269 6c69 7479 2920 6669  ccessibility) fi
-00001630: 656c 6420 7375 6666 6963 6965 6e74 6c79  eld sufficiently
-00001640: 2064 6573 6372 6962 6573 2074 6865 2069   describes the i
-00001650: 6d61 6765 2e2e 0700 0000 0e44 6573 6372  mage.......Descr
-00001660: 6970 7469 7665 5461 6201 03ff ffff ff08  iptiveTab.......
-00001670: 0000 0000 0600 0000 1841 6c74 2054 6578  .........Alt Tex
-00001680: 7420 2841 6363 6573 7369 6269 6c69 7479  t (Accessibility
-00001690: 2907 0000 000e 4465 7363 7269 7074 6976  ).....Descriptiv
-000016a0: 6554 6162 0103 ffff ffff 0800 0000 0006  eTab............
-000016b0: 0000 0015 4465 7363 7269 7074 696f 6e20  ....Description 
-000016c0: 2f20 4361 7074 696f 6e07 0000 000e 4465  / Caption.....De
-000016d0: 7363 7269 7074 6976 6554 6162 0103 ffff  scriptiveTab....
-000016e0: ffff 0800 0000 0006 0000 00c2 456e 7465  ............Ente
-000016f0: 7220 6120 2263 6170 7469 6f6e 2220 6465  r a "caption" de
-00001700: 7363 7269 6269 6e67 2074 6865 2077 686f  scribing the who
-00001710: 2c20 7768 6174 2c20 616e 6420 7768 7920  , what, and why 
-00001720: 6f66 2077 6861 7420 6973 2068 6170 7065  of what is happe
-00001730: 6e69 6e67 2069 6e20 7468 6973 2069 6d61  ning in this ima
-00001740: 6765 2c20 7468 6973 206d 6967 6874 2069  ge, this might i
-00001750: 6e63 6c75 6465 206e 616d 6573 206f 6620  nclude names of 
-00001760: 7065 6f70 6c65 2c20 616e 642f 6f72 2074  people, and/or t
-00001770: 6865 6972 2072 6f6c 6520 696e 2074 6865  heir role in the
-00001780: 2061 6374 696f 6e20 7468 6174 2069 7320   action that is 
-00001790: 7461 6b69 6e67 2070 6c61 6365 2077 6974  taking place wit
-000017a0: 6869 6e20 7468 6520 696d 6167 652e 0700  hin the image...
-000017b0: 0000 0e44 6573 6372 6970 7469 7665 5461  ...DescriptiveTa
-000017c0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-000017d0: 4b45 6e74 6572 2061 2062 7269 6566 2070  KEnter a brief p
-000017e0: 7562 6c69 7368 6162 6c65 2073 796e 6f70  ublishable synop
-000017f0: 7369 7320 6f72 2073 756d 6d61 7279 206f  sis or summary o
-00001800: 6620 7468 6520 636f 6e74 656e 7473 206f  f the contents o
-00001810: 6620 7468 6520 696d 6167 652e 0700 0000  f the image.....
-00001820: 0e44 6573 6372 6970 7469 7665 5461 6201  .DescriptiveTab.
-00001830: 03ff ffff ff08 0000 0000 0600 0000 5645  ..............VE
-00001840: 6e74 6572 2061 2073 686f 7274 2076 6572  nter a short ver
-00001850: 6261 6c20 616e 6420 6875 6d61 6e20 7265  bal and human re
-00001860: 6164 6162 6c65 206e 616d 6520 666f 7220  adable name for 
-00001870: 7468 6520 696d 6167 652c 2074 6869 7320  the image, this 
-00001880: 6d61 7920 6265 2074 6865 2066 696c 6520  may be the file 
-00001890: 6e61 6d65 2e07 0000 000e 4465 7363 7269  name......Descri
-000018a0: 7074 6976 6554 6162 0103 ffff ffff 0800  ptiveTab........
-000018b0: 0000 0006 0000 0082 456e 7465 7220 616e  ........Enter an
-000018c0: 7920 6e75 6d62 6572 206f 6620 6b65 7977  y number of keyw
-000018d0: 6f72 6473 2c20 7465 726d 7320 6f72 2070  ords, terms or p
-000018e0: 6872 6173 6573 2075 7365 6420 746f 2065  hrases used to e
-000018f0: 7870 7265 7373 2074 6865 2073 7562 6a65  xpress the subje
-00001900: 6374 206d 6174 7465 7220 696e 2074 6865  ct matter in the
-00001910: 2069 6d61 6765 2e20 5365 7061 7261 7465   image. Separate
-00001920: 2074 6865 6d20 7769 7468 2022 3b22 2063   them with ";" c
-00001930: 6861 7261 6374 6572 732e 0700 0000 0e44  haracters......D
-00001940: 6573 6372 6970 7469 7665 5461 6201 03ff  escriptiveTab...
-00001950: ffff ff08 0000 0000 0600 0000 9b45 6e74  .............Ent
-00001960: 6572 2074 6578 7420 6465 7363 7269 6269  er text describi
-00001970: 6e67 2074 6865 2061 7070 6561 7261 6e63  ng the appearanc
-00001980: 6520 6f66 2074 6865 2069 6d61 6765 2066  e of the image f
-00001990: 726f 6d20 6120 7669 7375 616c 2070 6572  rom a visual per
-000019a0: 7370 6563 7469 7665 2c20 666f 6375 7369  spective, focusi
-000019b0: 6e67 206f 6e20 6465 7461 696c 7320 7468  ng on details th
-000019c0: 6174 2061 7265 2072 656c 6576 616e 7420  at are relevant 
-000019d0: 746f 2074 6865 2070 7572 706f 7365 2061  to the purpose a
-000019e0: 6e64 206d 6561 6e69 6e67 206f 6620 7468  nd meaning of th
-000019f0: 6520 696d 6167 652e 0700 0000 0e44 6573  e image......Des
-00001a00: 6372 6970 7469 7665 5461 6201 03ff ffff  criptiveTab.....
-00001a10: ff08 0000 0000 0600 0000 2445 7874 656e  ..........$Exten
-00001a20: 6465 6420 4465 7363 7269 7074 696f 6e20  ded Description 
-00001a30: 2841 6363 6573 7369 6269 6c69 7479 2907  (Accessibility).
-00001a40: 0000 000e 4465 7363 7269 7074 6976 6554  ....DescriptiveT
-00001a50: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00001a60: 0008 4865 6164 6c69 6e65 0700 0000 0e44  ..Headline.....D
-00001a70: 6573 6372 6970 7469 7665 5461 6201 03ff  escriptiveTab...
-00001a80: ffff ff08 0000 0000 0600 0000 084b 6579  .............Key
-00001a90: 776f 7264 7307 0000 000e 4465 7363 7269  words.....Descri
-00001aa0: 7074 6976 6554 6162 0103 ffff ffff 0800  ptiveTab........
-00001ab0: 0000 0006 0000 0006 5261 7469 6e67 0700  ........Rating..
-00001ac0: 0000 0e44 6573 6372 6970 7469 7665 5461  ...DescriptiveTa
-00001ad0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00001ae0: 1354 6974 6c65 202f 204f 626a 6563 7420  .Title / Object 
-00001af0: 4e61 6d65 0700 0000 0e44 6573 6372 6970  Name.....Descrip
-00001b00: 7469 7665 5461 6201 03ff ffff ff08 0000  tiveTab.........
-00001b10: 0000 0600 0000 0672 656a 6563 7407 0000  .......reject...
-00001b20: 000e 4465 7363 7269 7074 6976 6554 6162  ..DescriptiveTab
-00001b30: 0103 ffff ffff 0800 0000 0006 0000 000f  ................
-00001b40: 2877 6865 6e20 706f 7373 6962 6c65 2907  (when possible).
-00001b50: 0000 000c 4564 6974 5365 7474 696e 6773  ....EditSettings
-00001b60: 0103 ffff ffff 0800 0000 0006 0000 000d  ................
-00001b70: 416c 7761 7973 2063 7265 6174 6507 0000  Always create...
-00001b80: 000c 4564 6974 5365 7474 696e 6773 0103  ..EditSettings..
-00001b90: ffff ffff 0800 0000 0006 0000 000d 416c  ..............Al
-00001ba0: 7761 7973 2064 656c 6574 6507 0000 000c  ways delete.....
-00001bb0: 4564 6974 5365 7474 696e 6773 0103 ffff  EditSettings....
-00001bc0: ffff 0800 0000 0006 0000 000c 416c 7761  ............Alwa
-00001bd0: 7973 2077 7269 7465 0700 0000 0c45 6469  ys write.....Edi
-00001be0: 7453 6574 7469 6e67 7301 03ff ffff ff08  tSettings.......
-00001bf0: 0000 0000 0600 0000 1343 7265 6174 6520  .........Create 
-00001c00: 6966 206e 6563 6573 7361 7279 0700 0000  if necessary....
-00001c10: 0c45 6469 7453 6574 7469 6e67 7301 03ff  .EditSettings...
-00001c20: ffff ff08 0000 0000 0600 0000 1444 656c  .............Del
-00001c30: 6574 6520 7768 656e 2070 6f73 7369 626c  ete when possibl
-00001c40: 6507 0000 000c 4564 6974 5365 7474 696e  e.....EditSettin
-00001c50: 6773 0103 ffff ffff 0800 0000 0006 0000  gs..............
-00001c60: 000f 4669 6c65 2074 696d 6573 7461 6d70  ..File timestamp
-00001c70: 7307 0000 000c 4564 6974 5365 7474 696e  s.....EditSettin
-00001c80: 6773 0103 ffff ffff 0800 0000 0006 0000  gs..............
-00001c90: 0011 4950 5443 2d49 494d 206d 6574 6164  ..IPTC-IIM metad
-00001ca0: 6174 6107 0000 000c 4564 6974 5365 7474  ata.....EditSett
-00001cb0: 696e 6773 0103 ffff ffff 0800 0000 0006  ings............
-00001cc0: 0000 000d 4b65 6570 206f 7269 6769 6e61  ....Keep origina
-00001cd0: 6c07 0000 000c 4564 6974 5365 7474 696e  l.....EditSettin
-00001ce0: 6773 0103 ffff ffff 0800 0000 0006 0000  gs..............
-00001cf0: 0011 5068 6f74 696e 693a 2073 6574 7469  ..Photini: setti
-00001d00: 6e67 7307 0000 000c 4564 6974 5365 7474  ngs.....EditSett
-00001d10: 696e 6773 0103 ffff ffff 0800 0000 0006  ings............
-00001d20: 0000 0019 5365 7420 746f 2077 6865 6e20  ....Set to when 
-00001d30: 6669 6c65 2069 7320 7361 7665 6407 0000  file is saved...
-00001d40: 000c 4564 6974 5365 7474 696e 6773 0103  ..EditSettings..
-00001d50: ffff ffff 0800 0000 0006 0000 001b 5365  ..............Se
-00001d60: 7420 746f 2077 6865 6e20 7068 6f74 6f20  t to when photo 
-00001d70: 7761 7320 7461 6b65 6e07 0000 000c 4564  was taken.....Ed
-00001d80: 6974 5365 7474 696e 6773 0103 ffff ffff  itSettings......
-00001d90: 0800 0000 0006 0000 001b 5368 6f77 2049  ..........Show I
-00001da0: 5054 432d 4949 4d20 6c65 6e67 7468 206c  PTC-IIM length l
-00001db0: 696d 6974 7307 0000 000c 4564 6974 5365  imits.....EditSe
-00001dc0: 7474 696e 6773 0103 ffff ffff 0800 0000  ttings..........
-00001dd0: 0006 0000 000d 5369 6465 6361 7220 6669  ......Sidecar fi
-00001de0: 6c65 7307 0000 000c 4564 6974 5365 7474  les.....EditSett
-00001df0: 696e 6773 0103 ffff ffff 0800 0000 0006  ings............
-00001e00: 0000 000f 5772 6974 6520 6966 2065 7869  ....Write if exi
-00001e10: 7374 7307 0000 000c 4564 6974 5365 7474  sts.....EditSett
-00001e20: 696e 6773 0103 ffff ffff 0800 0000 0006  ings............
-00001e30: 0000 0013 5772 6974 6520 746f 2069 6d61  ....Write to ima
-00001e40: 6765 2066 696c 6507 0000 000c 4564 6974  ge file.....Edit
-00001e50: 5365 7474 696e 6773 0103 ffff ffff 0800  Settings........
-00001e60: 0000 0006 0000 000e 2646 6c69 636b 7220  ........&Flickr 
-00001e70: 7570 6c6f 6164 0700 0000 0946 6c69 636b  upload.....Flick
-00001e80: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
-00001e90: 0000 002e 416c 6275 6d20 7769 6c6c 2062  ....Album will b
-00001ea0: 6520 6372 6561 7465 6420 7768 656e 2070  e created when p
-00001eb0: 686f 746f 7320 6172 6520 7570 6c6f 6164  hotos are upload
-00001ec0: 6564 0700 0000 0946 6c69 636b 7254 6162  ed.....FlickrTab
-00001ed0: 0103 ffff ffff 0800 0000 0006 0000 0010  ................
-00001ee0: 416c 6c6f 7720 636f 6d6d 656e 7469 6e67  Allow commenting
-00001ef0: 0700 0000 0946 6c69 636b 7254 6162 0103  .....FlickrTab..
-00001f00: ffff ffff 0800 0000 0006 0000 0014 416c  ..............Al
-00001f10: 6c6f 7720 7461 6773 2061 6e64 206e 6f74  low tags and not
-00001f20: 6573 0700 0000 0946 6c69 636b 7254 6162  es.....FlickrTab
-00001f30: 0103 ffff ffff 0800 0000 0006 0000 0011  ................
-00001f40: 416e 7920 466c 6963 6b72 206d 656d 6265  Any Flickr membe
-00001f50: 7207 0000 0009 466c 6963 6b72 5461 6201  r.....FlickrTab.
-00001f60: 03ff ffff ff08 0000 0000 0600 0000 1041  ...............A
-00001f70: 7274 2f49 6c6c 7573 7472 6174 696f 6e07  rt/Illustration.
-00001f80: 0000 0009 466c 6963 6b72 5461 6201 03ff  ....FlickrTab...
-00001f90: ffff ff08 0000 0000 0600 0000 1743 6861  .............Cha
-00001fa0: 6e67 6520 616c 6275 6d20 6d65 6d62 6572  nge album member
-00001fb0: 7368 6970 0700 0000 0946 6c69 636b 7254  ship.....FlickrT
-00001fc0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00001fd0: 0013 4368 616e 6765 2063 6f6e 7465 6e74  ..Change content
-00001fe0: 2074 7970 6507 0000 0009 466c 6963 6b72   type.....Flickr
-00001ff0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00002000: 0000 1743 6861 6e67 6520 6869 6465 2066  ...Change hide f
-00002010: 726f 6d20 7365 6172 6368 0700 0000 0946  rom search.....F
-00002020: 6c69 636b 7254 6162 0103 ffff ffff 0800  lickrTab........
-00002030: 0000 0006 0000 000e 4368 616e 6765 206c  ........Change l
-00002040: 6963 656e 6365 0700 0000 0946 6c69 636b  icence.....Flick
-00002050: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
-00002060: 0000 0013 4368 616e 6765 2073 6166 6574  ....Change safet
-00002070: 7920 6c65 7665 6c07 0000 0009 466c 6963  y level.....Flic
-00002080: 6b72 5461 6201 03ff ffff ff08 0000 0000  krTab...........
-00002090: 0600 0000 1643 6861 6e67 6520 7669 6577  .....Change view
-000020a0: 696e 6720 7072 6976 6163 7907 0000 0009  ing privacy.....
+00000010: a700 0000 0565 6e5f 4742 4200 000d c800  .....en_GBB.....
+00000020: 0000 6800 0057 3a00 0000 6d00 0057 5c00  ..h..W:...m..W\.
+00000030: 0000 7300 0059 6200 0002 6d00 0000 0000  ..s..Yb...m.....
+00000040: 0002 6d00 003f dc00 0027 3d00 0050 7600  ..m..?...'=..Pv.
+00000050: 005a 6c00 003e f300 0073 8800 0057 7e00  .Zl..>...s...W~.
+00000060: 0073 fe00 0057 a200 00cf 4f00 0059 8400  .s...W....O..Y..
+00000070: 04a0 b900 0000 f200 04a0 b900 0034 e800  .............4..
+00000080: 04bd a900 002d 5600 04d0 2500 002e d800  .....-V...%.....
+00000090: 04ec 3000 002f 2a00 0548 3500 0005 5300  ..0../*..H5...S.
+000000a0: 0548 3500 003d 6c00 0548 3500 004c 4900  .H5..=l..H5..LI.
+000000b0: 058c 0400 0030 9e00 0596 2500 004d c700  .....0....%..M..
+000000c0: 0597 c500 0016 c200 05a2 0000 0060 ec00  .............`..
+000000d0: 07c4 af00 001e 8a00 122b 0e00 002c 9b00  .........+...,..
+000000e0: 1cda 4d00 0028 7800 1cdb dd00 005e 5a00  ..M..(x......^Z.
+000000f0: 2412 d500 001d 9700 2cf6 3e00 000b 2900  $.......,.>...).
+00000100: 2d86 3400 0047 9800 2fa5 f500 0035 f000  -.4..G../....5..
+00000110: 3717 1b00 0047 6600 3bf1 0500 000d 5200  7....Gf.;.....R.
+00000120: 40e4 ce00 0063 1a00 434c ae00 0063 b700  @....c..CL...c..
+00000130: 47c4 e300 005f 7b00 4b87 d400 0044 9600  G...._{.K....D..
+00000140: 4d50 0500 0042 fe00 56ae c200 0046 1d00  MP...B..V....F..
+00000150: 56ae c200 0055 7600 56f6 af00 0015 c800  V....Uv.V.......
+00000160: 5a81 be00 0056 d500 5b0b 2500 0017 5f00  Z....V..[.%..._.
+00000170: 5b0b 2500 0028 5300 5b0b 2500 0047 ed00  [.%..(S.[.%..G..
+00000180: 6010 8500 0046 7300 67aa d300 002e f800  `....Fs.g.......
+00000190: 69a4 0300 001b c200 69a4 0300 002f 4a00  i.......i..../J.
+000001a0: 6cc1 9900 0013 9400 7107 6900 0032 d600  l.......q.i..2..
+000001b0: 770e bc00 0050 2b00 94cf 0200 0056 a700  w....P+......V..
+000001c0: a214 7000 0059 3500 a385 ee00 0004 2900  ..p..Y5.......).
+000001d0: b33d c200 000f 0300 b864 7000 0058 db00  .=.......dp..X..
+000001e0: bdd2 0e00 005c 3100 c0dd 3400 0025 0300  .....\1...4..%..
+000001f0: c61d 1400 005d fb00 c664 7000 0059 0800  .....]...dp..Y..
+00000200: d19a b500 005f 0c00 d70c b900 001c a900  ....._..........
+00000210: dc0f c400 0049 0600 ec29 c400 0046 ab00  .....I...)...F..
+00000220: f2f2 c800 0014 d301 0660 7400 0029 3a01  .........`t..):.
+00000230: 1387 c500 0056 0801 1de7 5500 0024 9401  .....V....U..$..
+00000240: 26bd a500 0036 1801 45eb 7900 0019 f601  &....6..E.y.....
+00000250: 5eeb 2f00 0062 9301 5f0d ad00 0019 b001  ^./..b.._.......
+00000260: 63c9 3300 0010 3801 6a03 2e00 0037 b801  c.3...8.j....7..
+00000270: 738f c800 005e 2e01 806a 5900 002d bd01  s....^...jY..-..
+00000280: 8ed4 7e00 0009 2501 8f97 f800 0054 c101  ..~...%......T..
+00000290: be34 b700 0053 f501 c1fa a500 0013 e501  .4...S..........
+000002a0: c1fa a500 0049 3201 c5f5 cd00 005a 8d01  .....I2......Z..
+000002b0: ca84 a100 0041 0a01 d2e9 6e00 002f 7001  .....A....n../p.
+000002c0: d8cd 2400 001e ac01 e4e1 1300 0059 a801  ..$..........Y..
+000002d0: f74f 4500 0036 7201 fc79 2500 002d 0901  .OE..6r..y%..-..
+000002e0: fd69 a500 000e 3d02 01ff 6300 0051 6202  .i....=...c..Qb.
+000002f0: 3205 d500 0023 1702 49c9 ae00 005f ba02  2....#..I...._..
+00000300: 6dbc 1400 0061 1402 772b 3500 001e 1502  m....a..w+5.....
+00000310: 86e0 0e00 0009 5d02 9653 5700 002c 5102  ......]..SW..,Q.
+00000320: 985c 0900 0033 fa02 9fe9 8c00 0042 8302  .\...3.......B..
+00000330: c89f a300 0011 d902 cffc a500 001a 4202  ..............B.
+00000340: d608 1500 0060 b902 f39d c300 0042 4f02  .....`.......BO.
+00000350: f9c4 c500 0015 0102 f9c4 c500 0027 1402  .............'..
+00000360: f9c4 c500 0045 9703 0220 f500 0029 e703  .....E... ...)..
+00000370: 051a a900 0025 6003 0c97 6400 0030 4203  .....%`...d..0B.
+00000380: 34c2 be00 003b 2e03 5444 bd00 001b 5103  4....;..TD....Q.
+00000390: 5976 9400 005d 8c03 5a4e 6e00 003a 1003  Yv...]..ZNn..:..
+000003a0: 7d24 1700 005a 1303 7d9c 2400 0046 4203  }$...Z..}.$..FB.
+000003b0: 7feb 9900 0036 9c03 80b5 5f00 0061 7303  .....6...._..as.
+000003c0: 91ff 0e00 0003 0c03 9a6e ce00 005d 2603  .........n...]&.
+000003d0: b0bf 2500 0000 8903 b0bf 2500 0040 8303  ..%.......%..@..
+000003e0: b466 4e00 0063 9103 b583 a300 0044 6603  .fN..c.......Df.
+000003f0: e2d3 9e00 0007 9703 e685 4500 003e 9d03  ..........E..>..
+00000400: ef1f 7900 001b 0a03 f11a 0500 0054 5f03  ..y..........T_.
+00000410: ffd9 4800 0053 5d04 0959 a500 003d e704  ..H..S]..Y...=..
+00000420: 0e9e 7900 0027 8c04 1fdd 3e00 004a 5604  ..y..'....>..JV.
+00000430: 424d fe00 0040 5604 4796 6e00 004f 9704  BM...@V.G.n..O..
+00000440: 4c1e ee00 005b b704 4cdd 2500 0011 0604  L....[..L.%.....
+00000450: 5701 9e00 0003 a504 598f 6300 0030 e604  W.......Y.c..0..
+00000460: 5fe8 c900 000d b104 60e5 8800 002d 8404  _.......`....-..
+00000470: 91a3 6e00 002b 5004 983c 8100 0052 3404  ..n..+P..<...R4.
+00000480: ab7e a500 002a 1504 c840 3900 0014 3804  .~...*...@9...8.
+00000490: c840 3900 0026 2304 d0e0 8200 0056 6d04  .@9..&#......Vm.
+000004a0: d2fa 2200 0014 5c04 d39f f400 0018 b304  .."...\.........
+000004b0: f573 6700 0015 9905 158c be00 004d 3c05  .sg..........M<.
+000004c0: 1a65 f500 005e ce05 2062 a400 003f 8b05  .e...^.. b...?..
+000004d0: 284a c000 0029 9505 2d4d 3c00 0013 2f05  (J...)..-M<.../.
+000004e0: 30af 7400 0048 1205 31a7 0200 0021 5405  0.t..H..1....!T.
+000004f0: 3596 fe00 005d 6205 3789 5700 0011 ab05  5....]b.7.W.....
+00000500: 3b7b 0500 0015 7305 3b7b 0500 0027 6405  ;{....s.;{...'d.
+00000510: 3e78 2d00 0022 6005 4479 4d00 0022 2b05  >x-.."`.DyM.."+.
+00000520: 5f74 6e00 005c 7605 6506 e300 0006 b405  _tn..\v.e.......
+00000530: 7776 ec00 0053 8a05 7b92 f300 0016 1005  wv...S..{.......
+00000540: 7b92 f300 0047 0205 88b0 4700 000d 2905  {....G....G...).
+00000550: 8be0 5e00 0005 9d05 8fdf b300 003e 7a05  ..^..........>z.
+00000560: 9b88 9800 0041 3805 a071 ff00 0053 1305  .....A8..q...S..
+00000570: a334 1900 003f b505 a617 ae00 0044 0605  .4...?.......D..
+00000580: a6c8 9500 0021 8605 a9c6 ae00 003f 3b05  .....!.......?;.
+00000590: ab35 0200 004b 4405 ab8b c400 0005 c205  .5...KD.........
+000005a0: ac8d e500 0015 2605 afca f400 0055 2105  ......&......U!.
+000005b0: b966 1900 000e 6a05 d34c 4e00 0040 2805  .f....j..LN..@(.
+000005c0: ddd6 7500 0035 0905 e997 4900 0046 d305  ..u..5....I..F..
+000005d0: fe21 9e00 0055 4a06 02a4 6e00 004a d306  .!...UJ...n..J..
+000005e0: 18f5 1e00 003a 6206 26dc c900 0021 ac06  .....:b.&....!..
+000005f0: 277c 7500 0021 d506 3bcf 2500 001b 9006  '|u..!..;.%.....
+00000600: 476c 6e00 001f 8206 4f4f 8e00 0039 4b06  Gln.....OO...9K.
+00000610: 5324 e500 0043 9f06 5a7e 1300 0025 3806  S$...C..Z~...%8.
+00000620: 67a1 fe00 0045 be06 6a3b a300 0010 a206  g....E..j;......
+00000630: 7b06 0300 002f b506 7c15 9500 001e 6306  {..../..|.....c.
+00000640: 8d7d 9000 0040 aa06 8f20 4500 0023 8e06  .}...@... E..#..
+00000650: 983c 8100 0005 e706 9dbc 4e00 000a 4206  .<........N...B.
+00000660: a31c 7f00 0048 6706 a5c6 b500 004c 6c06  .....Hg......Ll.
+00000670: b7eb 6900 0017 af06 baee ff00 0062 d306  ..i..........b..
+00000680: c325 ee00 0038 9006 c32b e700 0031 3506  .%...8...+...15.
+00000690: c955 b900 0026 ec06 c9b8 0500 0051 8f06  .U...&.......Q..
+000006a0: ce69 7e00 0020 2206 d4e8 7900 001a 7106  .i~.. "...y...q.
+000006b0: e788 c700 002b 2406 ea13 1200 0020 ca06  .....+$...... ..
+000006c0: f1ac b500 0040 de07 0660 9300 003f 1307  .....@...`...?..
+000006d0: 1735 2e00 004c bd07 1bd8 2200 005f 4207  .5...L....".._B.
+000006e0: 250e d300 001f f707 2a02 b300 001f 2607  %.......*.....&.
+000006f0: 2b5b f100 0055 9c07 3b07 1300 0020 6407  +[...U..;.... d.
+00000700: 3e8a ae00 0019 1d07 407b 1900 001c 1d07  >.......@{......
+00000710: 45d7 2e00 0063 6407 4758 b500 0019 7907  E....cd.GX....y.
+00000720: 5293 ae00 0001 3b07 5693 7c00 0057 c607  R.....;.V.|..W..
+00000730: 615d e500 000e 9e07 7302 0e00 005b 3b07  a]......s....[;.
+00000740: 7897 3300 0055 d307 7ce9 1e00 001d ed07  x.3..U..|.......
+00000750: 7de8 e500 0035 c107 8322 9400 000f c207  }....5..."......
+00000760: 8c0b a400 000d 8807 90c8 f500 0015 eb07  ................
+00000770: 9191 0900 0025 f207 99f1 c500 0043 4207  .....%.......CB.
+00000780: 9da3 5400 0061 4407 a1d6 cb00 0030 6c07  ..T..aD......0l.
+00000790: ab8e 0300 0000 2107 b40f 0500 003e 1f07  ......!......>..
+000007a0: c3bd 5400 0058 6407 c9d6 5800 004d 1307  ..T..Xd...X..M..
+000007b0: e01a 4f00 001a cb07 ee24 3400 004f f507  ..O......$4..O..
+000007c0: f66e 0f00 005c a908 1270 9800 0041 5d08  .n...\...p...A].
+000007d0: 4212 6e00 002f d808 43f9 7e00 000b ce08  B.n../..C.~.....
+000007e0: 4715 9e00 005a 4308 4eb2 f500 0029 bd08  G....ZC.N....)..
+000007f0: 766c 3e00 0001 9a08 8b0b 9e00 003c 2308  vl>..........<#.
+00000800: 9bd2 f100 0050 9a08 a420 8900 0043 d108  .....P... ...C..
+00000810: ad8b 6e00 003a cb08 aeab be00 0001 6908  ..n..:........i.
+00000820: bc21 0e00 0007 6808 bd8c e800 0022 9508  .!....h......"..
+00000830: f0ac 7500 0010 d208 fbec d300 002e 7f08  ..u.............
+00000840: ffed 5f00 0018 0f09 0769 1400 0041 8f09  .._......i...A..
+00000850: 0d6f 1900 000c 8c09 1d05 f000 003e 4709  .o...........>G.
+00000860: 20f0 3500 003d 1309 238a 1400 0059 d909   .5..=..#....Y..
+00000870: 2a03 d500 0000 4809 2ceb 9900 0008 ea09  *.....H.,.......
+00000880: 38bd 9e00 0035 7e09 41e3 4c00 000f 6209  8....5~.A.L...b.
+00000890: 4991 8400 0041 f109 49b3 8400 0032 7b09  I....A..I....2{.
+000008a0: 4d67 fe00 0014 0f09 4d67 fe00 0025 9f09  Mg......Mg...%..
+000008b0: 4d67 fe00 0044 3b09 4d67 fe00 0049 b509  Mg...D;.Mg...I..
+000008c0: 5e89 d300 0060 2b09 687d 7d00 0015 4c09  ^....`+.h}}...L.
+000008d0: 687d 7d00 0019 4c09 687d 7d00 0027 3b09  h}}...L.h}}..';.
+000008e0: 6d01 e500 0005 7609 6f97 8800 0054 8c09  m.....v.o....T..
+000008f0: 74a6 4700 002b c309 770c 9400 004c 9509  t.G..+..w....L..
+00000900: 7c17 7500 001e 3c09 87b0 1e00 0043 7809  |.u...<......Cx.
+00000910: c22c ce00 004b 6d09 caa9 1e00 0039 b509  .,...Km......9..
+00000920: ee20 2e00 000a b009 f590 2300 0028 d80a  . ........#..(..
+00000930: 0d74 f200 0006 380a 0d74 f200 0030 090a  .t....8..t...0..
+00000940: 3b83 3300 0004 ac0a 6966 c900 001d 720a  ;.3.....if....r.
+00000950: 6c5b d900 0001 150a 6c5b d900 0035 360a  l[......l[...56.
+00000960: 732a 5100 001b ea0a 7602 9200 0047 c60a  s*Q.....v....G..
+00000970: 7fce 9e00 0061 aa0a 89b6 4900 0014 a50a  .....a....I.....
+00000980: 8b8b 2200 0035 5a0a 8bd9 5e00 001d 320a  .."..5Z...^...2.
+00000990: 996f f800 0056 fb0a b75d 5400 0005 290a  .o...V...]T...).
+000009a0: c3dd 9f00 0044 bb0a c782 6e00 0003 e20a  .....D....n.....
+000009b0: cdee c700 0024 c60a d6d8 7e00 0002 510a  .....$....~...Q.
+000009c0: e9b7 f500 0012 9d0a ea95 9400 0011 330a  ..............3.
+000009d0: fb86 b900 002c 270b 0c76 4300 0036 470b  .....,'..vC..6G.
+000009e0: 0c89 5300 0018 ec0b 1690 7700 0004 f00b  ..S.......w.....
+000009f0: 1c6f ee00 0000 b00b 3165 4100 0007 300b  .o......1eA...0.
+00000a00: 32f5 3500 0029 0b0b 4d2e ee00 0037 3d0b  2.5..)..M....7=.
+00000a10: 52ae a400 0022 bc0b 5593 5500 005e 980b  R...."..U.U..^..
+00000a20: 6937 c900 0034 510b 6f5c 7500 0054 320b  i7...4Q.o\u..T2.
+00000a30: 70d2 2900 0017 820b 7b2c a500 000c d30b  p.).....{,......
+00000a40: 8170 0e00 0036 c10b 8224 9e00 0003 6b0b  .p...6...$....k.
+00000a50: 8a26 1400 0016 9a0b 8a9d 0e00 004d 670b  .&...........Mg.
+00000a60: a075 7f00 0061 f30b a097 8500 0023 da0b  .u...a.......#..
+00000a70: a0c9 de00 0056 430b a3fc 0c00 0021 000b  .....VC......!..
+00000a80: a408 e700 0021 2a0b bf62 0d00 0006 710b  .....!*..b....q.
+00000a90: c005 e400 0017 0e0b c093 e300 004c 1c0b  .............L..
+00000aa0: e2cc 8500 0048 3a0b e403 9500 0054 f60b  .....H:......T..
+00000ab0: f02b fe00 0001 db0b f045 3e00 000f fc0c  .+.......E>.....
+00000ac0: 132b 8e00 001f b10c 1ab9 a500 002b f90c  .+...........+..
+00000ad0: 204f 4300 003e c80c 2578 4900 0033 0e0c   OC..>..%xI..3..
+00000ae0: 27e7 6f00 0062 4a0c 28b7 4500 0050 4f0c  '.o..bJ.(.E..PO.
+00000af0: 2984 a300 001d c30c 359b 9e00 0034 970c  ).......5....4..
+00000b00: 4c8c 7500 0045 6f0c 4f0f 0e00 004d ea0c  L.u..Eo.O....M..
+00000b10: 5de1 c200 0012 0b0c 5e6f b400 0021 fe0c  ].......^o...!..
+00000b20: 7d70 9500 0013 030c 808a a300 001d 080c  }p..............
+00000b30: 808a a300 0030 be0c 9393 be00 0031 da0c  .....0.......1..
+00000b40: 94ba 4300 0006 f30c a0d5 c300 000f 900c  ..C.............
+00000b50: bb01 7300 0031 110c c20d 7e00 0052 5b0c  ..s..1....~..R[.
+00000b60: ca02 8500 0025 ca0c ce64 8d00 005d b70c  .....%...d...]..
+00000b70: d8f0 2d00 0006 0c0d 04cb 1e00 001f 540d  ..-...........T.
+00000b80: 0e50 f800 0049 890d 0e6d a300 000c fe0d  .P...I...m......
+00000b90: 196c 9900 0026 790d 3407 f100 000f 300d  .l...&y.4.....0.
+00000ba0: 3469 1300 0042 bc0d 369b 8500 0032 ab0d  4i...B..6....2..
+00000bb0: 4916 6e00 0049 5d0d 863e 6e00 0031 590d  I.n..I]..>n..1Y.
+00000bc0: 8c40 ce00 003f fd0d 8fb5 2300 0016 340d  .@...?....#...4.
+00000bd0: 8fb5 2300 0027 be0d 8fc4 f300 0014 800d  ..#..'..........
+00000be0: 8fc4 f300 0026 c50d 965b 1300 0010 740d  .....&...[....t.
+00000bf0: 96f8 2400 0011 5f0d a7df 9e00 0049 df0d  ..$..._......I..
+00000c00: b064 9300 0026 490d ba6f 3900 0033 a00d  .d...&I..o9..3..
+00000c10: c91a 8800 0012 ce0d d7f8 9b00 002e aa0e  ................
+00000c20: 030d e000 0012 680e 030d e000 0024 5d0e  ......h......$].
+00000c30: 0b43 4400 0052 e90e 0c29 6500 0024 240e  .CD..R...)e..$$.
+00000c40: 106e 3e00 0048 b20e 14c0 5500 002e 530e  .n>..H....U...S.
+00000c50: 2c0f 2e00 0045 ef0e 3145 cf00 0050 f90e  ,....E..1E...P..
+00000c60: 39c3 2100 0032 4b0e 6e22 5800 0051 f60e  9.!..2K.n"X..Q..
+00000c70: 6e48 5800 0051 b80e 6f36 c500 004c e70e  nHX..Q..o6...L..
+00000c80: 9528 b500 000d e10e 97bc b500 000e 0f0e  .(..............
+00000c90: 9ca3 7400 0058 230e 9e60 ae00 002a b80e  ..t..X#..`...*..
+00000ca0: a2ec 1e00 004f 0b0e a3b0 8e00 0002 ad0e  .....O..........
+00000cb0: af6f c300 003d 430e b6b7 de00 004e 880e  .o...=C......N..
+00000cc0: bec4 c300 0041 bf0e c1ac 3f00 0029 680e  .....A....?..)h.
+00000cd0: d26f 3700 0053 b50e d286 2e00 0038 3a0e  .o7..S.......8:.
+00000ce0: db53 e100 0016 6c0e db53 e100 0027 f80e  .S....l..S...'..
+00000cf0: dda7 4300 000e d30e df20 8d00 0058 a50e  ..C...... ...X..
+00000d00: eb97 ce00 0038 e90e edda 7500 0052 bb0e  .....8....u..R..
+00000d10: ee44 a400 0057 ed0e f101 de00 002d e60e  .D...W.......-..
+00000d20: f609 ee00 0004 6a0f 0500 0c00 0016 e40f  ......j.........
+00000d30: 1693 ca00 0028 b00f 3181 5c00 0023 520f  .....(..1.\..#R.
+00000d40: 3324 9500 0017 e00f 4889 e200 003d 8d0f  3$......H....=..
+00000d50: 5971 5e00 005a c10f 6207 7300 0020 8f0f  Yq^..Z..b.s.. ..
+00000d60: 647a 3900 003d c20f 664e 2900 0045 410f  dz9..=..fN)..EA.
+00000d70: 6fe8 3600 0050 ce0f 745d 8e00 003b a90f  o.6..P..t]...;..
+00000d80: 82a0 5900 0047 280f 8f1b 8e00 0012 3a0f  ..Y..G(.......:.
+00000d90: 9a90 6e00 002a 4b0f 9d6c a900 0013 600f  ..n..*K..l....`.
+00000da0: a8b3 0900 0033 570f a910 1500 0060 570f  .....3W......`W.
+00000db0: b1d1 6f00 0060 880f b6b2 4e00 003c bc0f  ..o..`....N..<..
+00000dc0: d415 de00 0022 ec0f d415 de00 0042 240f  .....".......B$.
+00000dd0: e808 8900 002c db0f ef54 0500 0017 360f  .....,...T....6.
+00000de0: ef54 0500 0028 2869 0000 63d8 03ff ffff  .T...((i..c.....
+00000df0: ff08 0000 0000 0600 0000 0220 6d07 0000  ........... m...
+00000e00: 000a 4164 6472 6573 7354 6162 0103 ffff  ..AddressTab....
+00000e10: ffff 0800 0000 0006 0000 0008 2641 6464  ............&Add
+00000e20: 7265 7373 0700 0000 0a41 6464 7265 7373  ress.....Address
+00000e30: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00000e40: 0000 2241 6464 7265 7373 206c 6f6f 6b75  .."Address looku
+00000e50: 7020 706f 7765 7265 6420 6279 204f 7065  p powered by Ope
+00000e60: 6e43 6167 6507 0000 000a 4164 6472 6573  nCage.....Addres
+00000e70: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
+00000e80: 0000 0008 416c 7469 7475 6465 0700 0000  ....Altitude....
+00000e90: 0a41 6464 7265 7373 5461 6201 03ff ffff  .AddressTab.....
+00000ea0: ff08 0000 0000 0600 0000 2341 6c74 6974  ..........#Altit
+00000eb0: 7564 6520 6f66 2074 6865 206c 6f63 6174  ude of the locat
+00000ec0: 696f 6e20 696e 206d 6574 7265 732e 0700  ion in metres...
+00000ed0: 0000 0a41 6464 7265 7373 5461 6201 03ff  ...AddressTab...
+00000ee0: ffff ff08 0000 0000 0600 0000 0443 6974  .............Cit
+00000ef0: 7907 0000 000a 4164 6472 6573 7354 6162  y.....AddressTab
+00000f00: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
+00000f10: 436f 756e 7472 7907 0000 000a 4164 6472  Country.....Addr
+00000f20: 6573 7354 6162 0103 ffff ffff 0800 0000  essTab..........
+00000f30: 0006 0000 000f 4465 6c65 7465 206c 6f63  ......Delete loc
+00000f40: 6174 696f 6e07 0000 000a 4164 6472 6573  ation.....Addres
+00000f50: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
+00000f60: 0000 0012 4475 706c 6963 6174 6520 6c6f  ....Duplicate lo
+00000f70: 6361 7469 6f6e 0700 0000 0a41 6464 7265  cation.....Addre
+00000f80: 7373 5461 6201 03ff ffff ff08 0000 0000  ssTab...........
+00000f90: 0600 0000 2245 6e74 6572 2061 2066 756c  ...."Enter a ful
+00000fa0: 6c20 6e61 6d65 206f 6620 7468 6520 6c6f  l name of the lo
+00000fb0: 6361 7469 6f6e 2e07 0000 000a 4164 6472  cation......Addr
+00000fc0: 6573 7354 6162 0103 ffff ffff 0800 0000  essTab..........
+00000fd0: 0006 0000 0057 456e 7465 7220 676c 6f62  .....WEnter glob
+00000fe0: 616c 6c79 2075 6e69 7175 6520 6964 656e  ally unique iden
+00000ff0: 7469 6669 6572 2873 2920 6f66 2074 6865  tifier(s) of the
+00001000: 206c 6f63 6174 696f 6e2e 2053 6570 6172   location. Separ
+00001010: 6174 6520 7468 656d 2077 6974 6820 223b  ate them with ";
+00001020: 2220 6368 6172 6163 7465 7273 2e07 0000  " characters....
+00001030: 000a 4164 6472 6573 7354 6162 0103 ffff  ..AddressTab....
+00001040: ffff 0800 0000 0006 0000 003d 456e 7465  ...........=Ente
+00001050: 7220 7468 6520 3220 6f72 2033 206c 6574  r the 2 or 3 let
+00001060: 7465 7220 4953 4f20 3331 3636 2063 6f75  ter ISO 3166 cou
+00001070: 6e74 7279 2063 6f64 6520 6f66 2074 6865  ntry code of the
+00001080: 2063 6f75 6e74 7279 2e07 0000 000a 4164   country......Ad
+00001090: 6472 6573 7354 6162 0103 ffff ffff 0800  dressTab........
+000010a0: 0000 0006 0000 0040 456e 7465 7220 7468  .......@Enter th
+000010b0: 6520 6465 7461 696c 7320 6162 6f75 7420  e details about 
+000010c0: 6120 6c6f 6361 7469 6f6e 2077 6865 7265  a location where
+000010d0: 2074 6869 7320 696d 6167 6520 7761 7320   this image was 
+000010e0: 6372 6561 7465 642e 0700 0000 0a41 6464  created......Add
+000010f0: 7265 7373 5461 6201 03ff ffff ff08 0000  ressTab.........
+00001100: 0000 0600 0000 4045 6e74 6572 2074 6865  ......@Enter the
+00001110: 2064 6574 6169 6c73 2061 626f 7574 2061   details about a
+00001120: 206c 6f63 6174 696f 6e20 7768 6963 6820   location which 
+00001130: 6973 2073 686f 776e 2069 6e20 7468 6973  is shown in this
+00001140: 2069 6d61 6765 2e07 0000 000a 4164 6472   image......Addr
+00001150: 6573 7354 6162 0103 ffff ffff 0800 0000  essTab..........
+00001160: 0006 0000 001b 456e 7465 7220 7468 6520  ......Enter the 
+00001170: 6e61 6d65 206f 6620 7468 6520 6369 7479  name of the city
+00001180: 2e07 0000 000a 4164 6472 6573 7354 6162  ......AddressTab
+00001190: 0103 ffff ffff 0800 0000 0006 0000 001e  ................
+000011a0: 456e 7465 7220 7468 6520 6e61 6d65 206f  Enter the name o
+000011b0: 6620 7468 6520 636f 756e 7472 792e 0700  f the country...
+000011c0: 0000 0a41 6464 7265 7373 5461 6201 03ff  ...AddressTab...
+000011d0: ffff ff08 0000 0000 0600 0000 2845 6e74  ............(Ent
+000011e0: 6572 2074 6865 206e 616d 6520 6f66 2074  er the name of t
+000011f0: 6865 2070 726f 7669 6e63 6520 6f72 2073  he province or s
+00001200: 7461 7465 2e07 0000 000a 4164 6472 6573  tate......Addres
+00001210: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
+00001220: 0000 0022 456e 7465 7220 7468 6520 6e61  ..."Enter the na
+00001230: 6d65 206f 6620 7468 6520 7375 626c 6f63  me of the subloc
+00001240: 6174 696f 6e2e 0700 0000 0a41 6464 7265  ation......Addre
+00001250: 7373 5461 6201 03ff ffff ff08 0000 0000  ssTab...........
+00001260: 0600 0000 2345 6e74 6572 2074 6865 206e  ....#Enter the n
+00001270: 616d 6520 6f66 2074 6865 2077 6f72 6c64  ame of the world
+00001280: 2072 6567 696f 6e2e 0700 0000 0a41 6464   region......Add
+00001290: 7265 7373 5461 6201 03ff ffff ff08 0000  ressTab.........
+000012a0: 0000 0600 0000 2547 656f 6461 7461 20c2  ......%Geodata .
+000012b0: a920 4f70 656e 5374 7265 6574 4d61 7020  . OpenStreetMap 
+000012c0: 636f 6e74 7269 6275 746f 7273 0700 0000  contributors....
+000012d0: 0a41 6464 7265 7373 5461 6201 03ff ffff  .AddressTab.....
+000012e0: ff08 0000 0000 0600 0000 1a47 6574 2061  ...........Get a
+000012f0: 6464 7265 7373 2066 726f 6d20 6c61 742c  ddress from lat,
+00001300: 206c 6f6e 6707 0000 000a 4164 6472 6573   long.....Addres
+00001310: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
+00001320: 0000 000b 4c6f 6361 7469 6f6e 2049 4407  ....Location ID.
+00001330: 0000 000a 4164 6472 6573 7354 6162 0103  ....AddressTab..
+00001340: ffff ffff 0800 0000 0006 0000 0004 4e61  ..............Na
+00001350: 6d65 0700 0000 0a41 6464 7265 7373 5461  me.....AddressTa
+00001360: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00001370: 0850 726f 7669 6e63 6507 0000 000a 4164  .Province.....Ad
+00001380: 6472 6573 7354 6162 0103 ffff ffff 0800  dressTab........
+00001390: 0000 0006 0000 0006 5265 6769 6f6e 0700  ........Region..
+000013a0: 0000 0a41 6464 7265 7373 5461 6201 03ff  ...AddressTab...
+000013b0: ffff ff08 0000 0000 0600 0000 0653 7472  .............Str
+000013c0: 6565 7407 0000 000a 4164 6472 6573 7354  eet.....AddressT
+000013d0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+000013e0: 0006 6361 6d65 7261 0700 0000 0a41 6464  ..camera.....Add
+000013f0: 7265 7373 5461 6201 03ff ffff ff08 0000  ressTab.........
+00001400: 0000 0600 0000 0d73 7562 6a65 6374 207b  .......subject {
+00001410: 6964 787d 0700 0000 0a41 6464 7265 7373  idx}.....Address
+00001420: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00001430: 0000 1d50 686f 7469 6e69 2070 686f 746f  ...Photini photo
+00001440: 206d 6574 6164 6174 6120 6564 6974 6f72   metadata editor
+00001450: 0700 0000 0743 4c49 4865 6c70 0103 ffff  .....CLIHelp....
+00001460: ffff 0800 0000 0006 0000 0027 5573 6167  ...........'Usag
+00001470: 653a 2025 7072 6f67 205b 6f70 7469 6f6e  e: %prog [option
+00001480: 735d 205b 6669 6c65 5f6e 616d 652c 202e  s] [file_name, .
+00001490: 2e2e 5d07 0000 0007 434c 4948 656c 7001  ..].....CLIHelp.
+000014a0: 03ff ffff ff08 0000 0000 0600 0000 2369  ..............#i
+000014b0: 6e63 7265 6173 6520 6e75 6d62 6572 206f  ncrease number o
+000014c0: 6620 6c6f 6767 696e 6720 6d65 7373 6167  f logging messag
+000014d0: 6573 0700 0000 0743 4c49 4865 6c70 0103  es.....CLIHelp..
+000014e0: ffff ffff 0800 0000 0006 0000 0021 7465  .............!te
+000014f0: 7374 206e 6577 2066 6561 7475 7265 7320  st new features 
+00001500: 6f72 2041 5049 2076 6572 7369 6f6e 7307  or API versions.
+00001510: 0000 0007 434c 4948 656c 7001 03ff ffff  ....CLIHelp.....
+00001520: ff08 0000 0000 0600 0000 1526 4465 7363  ...........&Desc
+00001530: 7269 7074 6976 6520 6d65 7461 6461 7461  riptive metadata
+00001540: 0700 0000 0e44 6573 6372 6970 7469 7665  .....Descriptive
+00001550: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00001560: 0000 0c3c 6661 766f 7572 6974 6573 3e07  ...<favourites>.
+00001570: 0000 000e 4465 7363 7269 7074 6976 6554  ....DescriptiveT
+00001580: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00001590: 0130 4120 6d6f 7265 2064 6574 6169 6c65  .0A more detaile
+000015a0: 6420 7465 7874 7561 6c20 6465 7363 7269  d textual descri
+000015b0: 7074 696f 6e20 6f66 2074 6865 2070 7572  ption of the pur
+000015c0: 706f 7365 2061 6e64 206d 6561 6e69 6e67  pose and meaning
+000015d0: 206f 6620 616e 2069 6d61 6765 2074 6861   of an image tha
+000015e0: 7420 656c 6162 6f72 6174 6573 206f 6e20  t elaborates on 
+000015f0: 7468 6520 696e 666f 726d 6174 696f 6e20  the information 
+00001600: 7072 6f76 6964 6564 2062 7920 7468 6520  provided by the 
+00001610: 416c 7420 5465 7874 2028 4163 6365 7373  Alt Text (Access
+00001620: 6962 696c 6974 7929 2070 726f 7065 7274  ibility) propert
+00001630: 792e 2054 6869 7320 7072 6f70 6572 7479  y. This property
+00001640: 2064 6f65 7320 6e6f 7420 6861 7665 2061   does not have a
+00001650: 2063 6861 7261 6374 6572 206c 696d 6974   character limit
+00001660: 6174 696f 6e20 616e 6420 6973 206e 6f74  ation and is not
+00001670: 2072 6571 7569 7265 6420 6966 2074 6865   required if the
+00001680: 2041 6c74 2054 6578 7420 2841 6363 6573   Alt Text (Acces
+00001690: 7369 6269 6c69 7479 2920 6669 656c 6420  sibility) field 
+000016a0: 7375 6666 6963 6965 6e74 6c79 2064 6573  sufficiently des
+000016b0: 6372 6962 6573 2074 6865 2069 6d61 6765  cribes the image
+000016c0: 2e2e 0700 0000 0e44 6573 6372 6970 7469  .......Descripti
+000016d0: 7665 5461 6201 03ff ffff ff08 0000 0000  veTab...........
+000016e0: 0600 0000 1841 6c74 2054 6578 7420 2841  .....Alt Text (A
+000016f0: 6363 6573 7369 6269 6c69 7479 2907 0000  ccessibility)...
+00001700: 000e 4465 7363 7269 7074 6976 6554 6162  ..DescriptiveTab
+00001710: 0103 ffff ffff 0800 0000 0006 0000 0015  ................
+00001720: 4465 7363 7269 7074 696f 6e20 2f20 4361  Description / Ca
+00001730: 7074 696f 6e07 0000 000e 4465 7363 7269  ption.....Descri
+00001740: 7074 6976 6554 6162 0103 ffff ffff 0800  ptiveTab........
+00001750: 0000 0006 0000 00c2 456e 7465 7220 6120  ........Enter a 
+00001760: 2263 6170 7469 6f6e 2220 6465 7363 7269  "caption" descri
+00001770: 6269 6e67 2074 6865 2077 686f 2c20 7768  bing the who, wh
+00001780: 6174 2c20 616e 6420 7768 7920 6f66 2077  at, and why of w
+00001790: 6861 7420 6973 2068 6170 7065 6e69 6e67  hat is happening
+000017a0: 2069 6e20 7468 6973 2069 6d61 6765 2c20   in this image, 
+000017b0: 7468 6973 206d 6967 6874 2069 6e63 6c75  this might inclu
+000017c0: 6465 206e 616d 6573 206f 6620 7065 6f70  de names of peop
+000017d0: 6c65 2c20 616e 642f 6f72 2074 6865 6972  le, and/or their
+000017e0: 2072 6f6c 6520 696e 2074 6865 2061 6374   role in the act
+000017f0: 696f 6e20 7468 6174 2069 7320 7461 6b69  ion that is taki
+00001800: 6e67 2070 6c61 6365 2077 6974 6869 6e20  ng place within 
+00001810: 7468 6520 696d 6167 652e 0700 0000 0e44  the image......D
+00001820: 6573 6372 6970 7469 7665 5461 6201 03ff  escriptiveTab...
+00001830: ffff ff08 0000 0000 0600 0000 4b45 6e74  ............KEnt
+00001840: 6572 2061 2062 7269 6566 2070 7562 6c69  er a brief publi
+00001850: 7368 6162 6c65 2073 796e 6f70 7369 7320  shable synopsis 
+00001860: 6f72 2073 756d 6d61 7279 206f 6620 7468  or summary of th
+00001870: 6520 636f 6e74 656e 7473 206f 6620 7468  e contents of th
+00001880: 6520 696d 6167 652e 0700 0000 0e44 6573  e image......Des
+00001890: 6372 6970 7469 7665 5461 6201 03ff ffff  criptiveTab.....
+000018a0: ff08 0000 0000 0600 0000 5645 6e74 6572  ..........VEnter
+000018b0: 2061 2073 686f 7274 2076 6572 6261 6c20   a short verbal 
+000018c0: 616e 6420 6875 6d61 6e20 7265 6164 6162  and human readab
+000018d0: 6c65 206e 616d 6520 666f 7220 7468 6520  le name for the 
+000018e0: 696d 6167 652c 2074 6869 7320 6d61 7920  image, this may 
+000018f0: 6265 2074 6865 2066 696c 6520 6e61 6d65  be the file name
+00001900: 2e07 0000 000e 4465 7363 7269 7074 6976  ......Descriptiv
+00001910: 6554 6162 0103 ffff ffff 0800 0000 0006  eTab............
+00001920: 0000 0082 456e 7465 7220 616e 7920 6e75  ....Enter any nu
+00001930: 6d62 6572 206f 6620 6b65 7977 6f72 6473  mber of keywords
+00001940: 2c20 7465 726d 7320 6f72 2070 6872 6173  , terms or phras
+00001950: 6573 2075 7365 6420 746f 2065 7870 7265  es used to expre
+00001960: 7373 2074 6865 2073 7562 6a65 6374 206d  ss the subject m
+00001970: 6174 7465 7220 696e 2074 6865 2069 6d61  atter in the ima
+00001980: 6765 2e20 5365 7061 7261 7465 2074 6865  ge. Separate the
+00001990: 6d20 7769 7468 2022 3b22 2063 6861 7261  m with ";" chara
+000019a0: 6374 6572 732e 0700 0000 0e44 6573 6372  cters......Descr
+000019b0: 6970 7469 7665 5461 6201 03ff ffff ff08  iptiveTab.......
+000019c0: 0000 0000 0600 0000 9b45 6e74 6572 2074  .........Enter t
+000019d0: 6578 7420 6465 7363 7269 6269 6e67 2074  ext describing t
+000019e0: 6865 2061 7070 6561 7261 6e63 6520 6f66  he appearance of
+000019f0: 2074 6865 2069 6d61 6765 2066 726f 6d20   the image from 
+00001a00: 6120 7669 7375 616c 2070 6572 7370 6563  a visual perspec
+00001a10: 7469 7665 2c20 666f 6375 7369 6e67 206f  tive, focusing o
+00001a20: 6e20 6465 7461 696c 7320 7468 6174 2061  n details that a
+00001a30: 7265 2072 656c 6576 616e 7420 746f 2074  re relevant to t
+00001a40: 6865 2070 7572 706f 7365 2061 6e64 206d  he purpose and m
+00001a50: 6561 6e69 6e67 206f 6620 7468 6520 696d  eaning of the im
+00001a60: 6167 652e 0700 0000 0e44 6573 6372 6970  age......Descrip
+00001a70: 7469 7665 5461 6201 03ff ffff ff08 0000  tiveTab.........
+00001a80: 0000 0600 0000 2445 7874 656e 6465 6420  ......$Extended 
+00001a90: 4465 7363 7269 7074 696f 6e20 2841 6363  Description (Acc
+00001aa0: 6573 7369 6269 6c69 7479 2907 0000 000e  essibility).....
+00001ab0: 4465 7363 7269 7074 6976 6554 6162 0103  DescriptiveTab..
+00001ac0: ffff ffff 0800 0000 0006 0000 0008 4865  ..............He
+00001ad0: 6164 6c69 6e65 0700 0000 0e44 6573 6372  adline.....Descr
+00001ae0: 6970 7469 7665 5461 6201 03ff ffff ff08  iptiveTab.......
+00001af0: 0000 0000 0600 0000 084b 6579 776f 7264  .........Keyword
+00001b00: 7307 0000 000e 4465 7363 7269 7074 6976  s.....Descriptiv
+00001b10: 6554 6162 0103 ffff ffff 0800 0000 0006  eTab............
+00001b20: 0000 0006 5261 7469 6e67 0700 0000 0e44  ....Rating.....D
+00001b30: 6573 6372 6970 7469 7665 5461 6201 03ff  escriptiveTab...
+00001b40: ffff ff08 0000 0000 0600 0000 1354 6974  .............Tit
+00001b50: 6c65 202f 204f 626a 6563 7420 4e61 6d65  le / Object Name
+00001b60: 0700 0000 0e44 6573 6372 6970 7469 7665  .....Descriptive
+00001b70: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00001b80: 0000 0672 656a 6563 7407 0000 000e 4465  ...reject.....De
+00001b90: 7363 7269 7074 6976 6554 6162 0103 ffff  scriptiveTab....
+00001ba0: ffff 0800 0000 0006 0000 000f 2877 6865  ............(whe
+00001bb0: 6e20 706f 7373 6962 6c65 2907 0000 000c  n possible).....
+00001bc0: 4564 6974 5365 7474 696e 6773 0103 ffff  EditSettings....
+00001bd0: ffff 0800 0000 0006 0000 000d 416c 7761  ............Alwa
+00001be0: 7973 2063 7265 6174 6507 0000 000c 4564  ys create.....Ed
+00001bf0: 6974 5365 7474 696e 6773 0103 ffff ffff  itSettings......
+00001c00: 0800 0000 0006 0000 000d 416c 7761 7973  ..........Always
+00001c10: 2064 656c 6574 6507 0000 000c 4564 6974   delete.....Edit
+00001c20: 5365 7474 696e 6773 0103 ffff ffff 0800  Settings........
+00001c30: 0000 0006 0000 000c 416c 7761 7973 2077  ........Always w
+00001c40: 7269 7465 0700 0000 0c45 6469 7453 6574  rite.....EditSet
+00001c50: 7469 6e67 7301 03ff ffff ff08 0000 0000  tings...........
+00001c60: 0600 0000 1343 7265 6174 6520 6966 206e  .....Create if n
+00001c70: 6563 6573 7361 7279 0700 0000 0c45 6469  ecessary.....Edi
+00001c80: 7453 6574 7469 6e67 7301 03ff ffff ff08  tSettings.......
+00001c90: 0000 0000 0600 0000 1444 656c 6574 6520  .........Delete 
+00001ca0: 7768 656e 2070 6f73 7369 626c 6507 0000  when possible...
+00001cb0: 000c 4564 6974 5365 7474 696e 6773 0103  ..EditSettings..
+00001cc0: ffff ffff 0800 0000 0006 0000 000f 4669  ..............Fi
+00001cd0: 6c65 2074 696d 6573 7461 6d70 7307 0000  le timestamps...
+00001ce0: 000c 4564 6974 5365 7474 696e 6773 0103  ..EditSettings..
+00001cf0: ffff ffff 0800 0000 0006 0000 000c 4750  ..............GP
+00001d00: 5820 696d 706f 7274 6572 0700 0000 0c45  X importer.....E
+00001d10: 6469 7453 6574 7469 6e67 7301 03ff ffff  ditSettings.....
+00001d20: ff08 0000 0000 0600 0000 1149 5054 432d  ...........IPTC-
+00001d30: 4949 4d20 6d65 7461 6461 7461 0700 0000  IIM metadata....
+00001d40: 0c45 6469 7453 6574 7469 6e67 7301 03ff  .EditSettings...
+00001d50: ffff ff08 0000 0000 0600 0000 0d4b 6565  .............Kee
+00001d60: 7020 6f72 6967 696e 616c 0700 0000 0c45  p original.....E
+00001d70: 6469 7453 6574 7469 6e67 7301 03ff ffff  ditSettings.....
+00001d80: ff08 0000 0000 0600 0000 1150 686f 7469  ...........Photi
+00001d90: 6e69 3a20 7365 7474 696e 6773 0700 0000  ni: settings....
+00001da0: 0c45 6469 7453 6574 7469 6e67 7301 03ff  .EditSettings...
+00001db0: ffff ff08 0000 0000 0600 0000 1953 6574  .............Set
+00001dc0: 2074 6f20 7768 656e 2066 696c 6520 6973   to when file is
+00001dd0: 2073 6176 6564 0700 0000 0c45 6469 7453   saved.....EditS
+00001de0: 6574 7469 6e67 7301 03ff ffff ff08 0000  ettings.........
+00001df0: 0000 0600 0000 1b53 6574 2074 6f20 7768  .......Set to wh
+00001e00: 656e 2070 686f 746f 2077 6173 2074 616b  en photo was tak
+00001e10: 656e 0700 0000 0c45 6469 7453 6574 7469  en.....EditSetti
+00001e20: 6e67 7301 03ff ffff ff08 0000 0000 0600  ngs.............
+00001e30: 0000 1b53 686f 7720 4950 5443 2d49 494d  ...Show IPTC-IIM
+00001e40: 206c 656e 6774 6820 6c69 6d69 7473 0700   length limits..
+00001e50: 0000 0c45 6469 7453 6574 7469 6e67 7301  ...EditSettings.
+00001e60: 03ff ffff ff08 0000 0000 0600 0000 0d53  ...............S
+00001e70: 6964 6563 6172 2066 696c 6573 0700 0000  idecar files....
+00001e80: 0c45 6469 7453 6574 7469 6e67 7301 03ff  .EditSettings...
+00001e90: ffff ff08 0000 0000 0600 0000 0f57 7269  .............Wri
+00001ea0: 7465 2069 6620 6578 6973 7473 0700 0000  te if exists....
+00001eb0: 0c45 6469 7453 6574 7469 6e67 7301 03ff  .EditSettings...
+00001ec0: ffff ff08 0000 0000 0600 0000 1357 7269  .............Wri
+00001ed0: 7465 2074 6f20 696d 6167 6520 6669 6c65  te to image file
+00001ee0: 0700 0000 0c45 6469 7453 6574 7469 6e67  .....EditSetting
+00001ef0: 7301 03ff ffff ff08 0000 0000 0600 0000  s...............
+00001f00: 0c73 6574 2061 6c74 6974 7564 6507 0000  .set altitude...
+00001f10: 000c 4564 6974 5365 7474 696e 6773 0103  ..EditSettings..
+00001f20: ffff ffff 0800 0000 0006 0000 000e 2646  ..............&F
+00001f30: 6c69 636b 7220 7570 6c6f 6164 0700 0000  lickr upload....
+00001f40: 0946 6c69 636b 7254 6162 0103 ffff ffff  .FlickrTab......
+00001f50: 0800 0000 0006 0000 002e 416c 6275 6d20  ..........Album 
+00001f60: 7769 6c6c 2062 6520 6372 6561 7465 6420  will be created 
+00001f70: 7768 656e 2070 686f 746f 7320 6172 6520  when photos are 
+00001f80: 7570 6c6f 6164 6564 0700 0000 0946 6c69  uploaded.....Fli
+00001f90: 636b 7254 6162 0103 ffff ffff 0800 0000  ckrTab..........
+00001fa0: 0006 0000 0010 416c 6c6f 7720 636f 6d6d  ......Allow comm
+00001fb0: 656e 7469 6e67 0700 0000 0946 6c69 636b  enting.....Flick
+00001fc0: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
+00001fd0: 0000 0014 416c 6c6f 7720 7461 6773 2061  ....Allow tags a
+00001fe0: 6e64 206e 6f74 6573 0700 0000 0946 6c69  nd notes.....Fli
+00001ff0: 636b 7254 6162 0103 ffff ffff 0800 0000  ckrTab..........
+00002000: 0006 0000 0011 416e 7920 466c 6963 6b72  ......Any Flickr
+00002010: 206d 656d 6265 7207 0000 0009 466c 6963   member.....Flic
+00002020: 6b72 5461 6201 03ff ffff ff08 0000 0000  krTab...........
+00002030: 0600 0000 1041 7274 2f49 6c6c 7573 7472  .....Art/Illustr
+00002040: 6174 696f 6e07 0000 0009 466c 6963 6b72  ation.....Flickr
+00002050: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00002060: 0000 1743 6861 6e67 6520 616c 6275 6d20  ...Change album 
+00002070: 6d65 6d62 6572 7368 6970 0700 0000 0946  membership.....F
+00002080: 6c69 636b 7254 6162 0103 ffff ffff 0800  lickrTab........
+00002090: 0000 0006 0000 0013 4368 616e 6765 2063  ........Change c
+000020a0: 6f6e 7465 6e74 2074 7970 6507 0000 0009  ontent type.....
 000020b0: 466c 6963 6b72 5461 6201 03ff ffff ff08  FlickrTab.......
-000020c0: 0000 0000 0600 0000 3343 6861 6e67 6520  ........3Change 
-000020d0: 7768 6f20 6361 6e20 636f 6d6d 656e 7420  who can comment 
-000020e0: 6f72 2074 6167 2028 616e 6420 7669 6577  or tag (and view
-000020f0: 696e 6720 7072 6976 6163 7929 0700 0000  ing privacy)....
-00002100: 0946 6c69 636b 7254 6162 0103 ffff ffff  .FlickrTab......
-00002110: 0800 0000 0006 0000 000c 436f 6e74 656e  ..........Conten
-00002120: 7420 7479 7065 0700 0000 0946 6c69 636b  t type.....Flick
-00002130: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
-00002140: 0000 000b 4465 7363 7269 7074 696f 6e07  ....Description.
-00002150: 0000 0009 466c 6963 6b72 5461 6201 03ff  ....FlickrTab...
-00002160: ffff ff08 0000 0000 0600 0000 0646 616d  .............Fam
-00002170: 696c 7907 0000 0009 466c 6963 6b72 5461  ily.....FlickrTa
-00002180: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00002190: 0646 6c69 636b 7207 0000 0009 466c 6963  .Flickr.....Flic
-000021a0: 6b72 5461 6201 03ff ffff ff08 0000 0000  krTab...........
-000021b0: 0600 0000 0746 7269 656e 6473 0700 0000  .....Friends....
-000021c0: 0946 6c69 636b 7254 6162 0103 ffff ffff  .FlickrTab......
-000021d0: 0800 0000 0006 0000 0010 4672 6965 6e64  ..........Friend
-000021e0: 7320 2620 6661 6d69 6c79 0700 0000 0946  s & family.....F
-000021f0: 6c69 636b 7254 6162 0103 ffff ffff 0800  lickrTab........
-00002200: 0000 0006 0000 0010 4869 6465 2066 726f  ........Hide fro
-00002210: 6d20 7365 6172 6368 0700 0000 0946 6c69  m search.....Fli
-00002220: 636b 7254 6162 0103 ffff ffff 0800 0000  ckrTab..........
-00002230: 0006 0000 0007 4c69 6365 6e63 6507 0000  ......Licence...
-00002240: 0009 466c 6963 6b72 5461 6201 03ff ffff  ..FlickrTab.....
-00002250: ff08 0000 0000 0600 0000 084d 6f64 6572  ...........Moder
-00002260: 6174 6507 0000 0009 466c 6963 6b72 5461  ate.....FlickrTa
-00002270: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00002280: 094e 6577 2061 6c62 756d 0700 0000 0946  .New album.....F
-00002290: 6c69 636b 7254 6162 0103 ffff ffff 0800  lickrTab........
-000022a0: 0000 0006 0000 0008 4f6e 6c79 2079 6f75  ........Only you
+000020c0: 0000 0000 0600 0000 1743 6861 6e67 6520  .........Change 
+000020d0: 6869 6465 2066 726f 6d20 7365 6172 6368  hide from search
+000020e0: 0700 0000 0946 6c69 636b 7254 6162 0103  .....FlickrTab..
+000020f0: ffff ffff 0800 0000 0006 0000 000e 4368  ..............Ch
+00002100: 616e 6765 206c 6963 656e 6365 0700 0000  ange licence....
+00002110: 0946 6c69 636b 7254 6162 0103 ffff ffff  .FlickrTab......
+00002120: 0800 0000 0006 0000 0013 4368 616e 6765  ..........Change
+00002130: 2073 6166 6574 7920 6c65 7665 6c07 0000   safety level...
+00002140: 0009 466c 6963 6b72 5461 6201 03ff ffff  ..FlickrTab.....
+00002150: ff08 0000 0000 0600 0000 1643 6861 6e67  ...........Chang
+00002160: 6520 7669 6577 696e 6720 7072 6976 6163  e viewing privac
+00002170: 7907 0000 0009 466c 6963 6b72 5461 6201  y.....FlickrTab.
+00002180: 03ff ffff ff08 0000 0000 0600 0000 3343  ..............3C
+00002190: 6861 6e67 6520 7768 6f20 6361 6e20 636f  hange who can co
+000021a0: 6d6d 656e 7420 6f72 2074 6167 2028 616e  mment or tag (an
+000021b0: 6420 7669 6577 696e 6720 7072 6976 6163  d viewing privac
+000021c0: 7929 0700 0000 0946 6c69 636b 7254 6162  y).....FlickrTab
+000021d0: 0103 ffff ffff 0800 0000 0006 0000 000c  ................
+000021e0: 436f 6e74 656e 7420 7479 7065 0700 0000  Content type....
+000021f0: 0946 6c69 636b 7254 6162 0103 ffff ffff  .FlickrTab......
+00002200: 0800 0000 0006 0000 000b 4465 7363 7269  ..........Descri
+00002210: 7074 696f 6e07 0000 0009 466c 6963 6b72  ption.....Flickr
+00002220: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00002230: 0000 0646 616d 696c 7907 0000 0009 466c  ...Family.....Fl
+00002240: 6963 6b72 5461 6201 03ff ffff ff08 0000  ickrTab.........
+00002250: 0000 0600 0000 0646 6c69 636b 7207 0000  .......Flickr...
+00002260: 0009 466c 6963 6b72 5461 6201 03ff ffff  ..FlickrTab.....
+00002270: ff08 0000 0000 0600 0000 0746 7269 656e  ...........Frien
+00002280: 6473 0700 0000 0946 6c69 636b 7254 6162  ds.....FlickrTab
+00002290: 0103 ffff ffff 0800 0000 0006 0000 0010  ................
+000022a0: 4672 6965 6e64 7320 2620 6661 6d69 6c79  Friends & family
 000022b0: 0700 0000 0946 6c69 636b 7254 6162 0103  .....FlickrTab..
-000022c0: ffff ffff 0800 0000 0006 0000 0011 5065  ..............Pe
-000022d0: 6f70 6c65 2079 6f75 2066 6f6c 6c6f 7707  ople you follow.
-000022e0: 0000 0009 466c 6963 6b72 5461 6201 03ff  ....FlickrTab...
-000022f0: ffff ff08 0000 0000 0600 0000 0550 686f  .............Pho
-00002300: 746f 0700 0000 0946 6c69 636b 7254 6162  to.....FlickrTab
-00002310: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
-00002320: 5072 6976 6174 6507 0000 0009 466c 6963  Private.....Flic
-00002330: 6b72 5461 6201 03ff ffff ff08 0000 0000  krTab...........
-00002340: 0600 0000 0650 7562 6c69 6307 0000 0009  .....Public.....
-00002350: 466c 6963 6b72 5461 6201 03ff ffff ff08  FlickrTab.......
-00002360: 0000 0000 0600 0000 1a52 6570 6c61 6365  .........Replace
-00002370: 2069 6d61 6765 2072 6567 696f 6e20 6e6f   image region no
-00002380: 7465 7307 0000 0009 466c 6963 6b72 5461  tes.....FlickrTa
-00002390: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-000023a0: 1052 6570 6c61 6365 206d 6574 6164 6174  .Replace metadat
-000023b0: 6107 0000 0009 466c 6963 6b72 5461 6201  a.....FlickrTab.
-000023c0: 03ff ffff ff08 0000 0000 0600 0000 0a52  ...............R
-000023d0: 6573 7472 6963 7465 6407 0000 0009 466c  estricted.....Fl
-000023e0: 6963 6b72 5461 6201 03ff ffff ff08 0000  ickrTab.........
-000023f0: 0000 0600 0000 0453 6166 6507 0000 0009  .......Safe.....
-00002400: 466c 6963 6b72 5461 6201 03ff ffff ff08  FlickrTab.......
-00002410: 0000 0000 0600 0000 0c53 6166 6574 7920  .........Safety 
-00002420: 6c65 7665 6c07 0000 0009 466c 6963 6b72  level.....Flickr
-00002430: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00002440: 0000 0a53 6372 6565 6e73 686f 7407 0000  ...Screenshot...
-00002450: 0009 466c 6963 6b72 5461 6201 03ff ffff  ..FlickrTab.....
-00002460: ff08 0000 0000 0600 0000 0b53 796e 6368  ...........Synch
-00002470: 726f 6e69 7365 0700 0000 0946 6c69 636b  ronise.....Flick
-00002480: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
-00002490: 0000 0005 5469 746c 6507 0000 0009 466c  ....Title.....Fl
-000024a0: 6963 6b72 5461 6201 03ff ffff ff08 0000  ickrTab.........
-000024b0: 0000 0600 0000 0f56 6965 7769 6e67 2070  .......Viewing p
-000024c0: 7269 7661 6379 0700 0000 0946 6c69 636b  rivacy.....Flick
-000024d0: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
-000024e0: 0000 0013 5669 7274 7561 6c20 5068 6f74  ....Virtual Phot
-000024f0: 6f67 7261 7068 7907 0000 0009 466c 6963  ography.....Flic
-00002500: 6b72 5461 6201 03ff ffff ff08 0000 0000  krTab...........
-00002510: 0600 0000 0b41 6c62 756d 2074 6974 6c65  .....Album title
-00002520: 0700 0000 0f47 6f6f 676c 6550 686f 746f  .....GooglePhoto
-00002530: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
-00002540: 0000 0080 4669 6c65 2022 7b66 696c 655f  ....File "{file_
-00002550: 6e61 6d65 7d22 2069 7320 6f76 6572 2032  name}" is over 2
-00002560: 35c2 a04d 422e 2052 656d 656d 6265 7220  5..MB. Remember 
-00002570: 7468 6174 2050 686f 7469 6e69 2075 706c  that Photini upl
-00002580: 6f61 6473 2063 6f75 6e74 2074 6f77 6172  oads count towar
-00002590: 6473 2073 746f 7261 6765 2069 6e20 796f  ds storage in yo
-000025a0: 7572 2047 6f6f 676c 6520 4163 636f 756e  ur Google Accoun
-000025b0: 742e 2055 706c 6f61 6420 6974 2061 6e79  t. Upload it any
-000025c0: 7761 793f 0700 0000 0f47 6f6f 676c 6550  way?.....GoogleP
-000025d0: 686f 746f 7354 6162 0103 ffff ffff 0800  hotosTab........
-000025e0: 0000 0006 0000 0015 476f 6f67 6c65 2026  ........Google &
-000025f0: 5068 6f74 6f73 2075 706c 6f61 6407 0000  Photos upload...
-00002600: 000f 476f 6f67 6c65 5068 6f74 6f73 5461  ..GooglePhotosTa
-00002610: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00002620: 0d47 6f6f 676c 6520 5068 6f74 6f73 0700  .Google Photos..
-00002630: 0000 0f47 6f6f 676c 6550 686f 746f 7354  ...GooglePhotosT
-00002640: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00002650: 000b 4c61 7267 6520 6669 6c65 2e07 0000  ..Large file....
-00002660: 000f 476f 6f67 6c65 5068 6f74 6f73 5461  ..GooglePhotosTa
-00002670: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00002680: 094e 6577 2061 6c62 756d 0700 0000 0f47  .New album.....G
+000022c0: ffff ffff 0800 0000 0006 0000 0010 4869  ..............Hi
+000022d0: 6465 2066 726f 6d20 7365 6172 6368 0700  de from search..
+000022e0: 0000 0946 6c69 636b 7254 6162 0103 ffff  ...FlickrTab....
+000022f0: ffff 0800 0000 0006 0000 0007 4c69 6365  ............Lice
+00002300: 6e63 6507 0000 0009 466c 6963 6b72 5461  nce.....FlickrTa
+00002310: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00002320: 084d 6f64 6572 6174 6507 0000 0009 466c  .Moderate.....Fl
+00002330: 6963 6b72 5461 6201 03ff ffff ff08 0000  ickrTab.........
+00002340: 0000 0600 0000 094e 6577 2061 6c62 756d  .......New album
+00002350: 0700 0000 0946 6c69 636b 7254 6162 0103  .....FlickrTab..
+00002360: ffff ffff 0800 0000 0006 0000 0008 4f6e  ..............On
+00002370: 6c79 2079 6f75 0700 0000 0946 6c69 636b  ly you.....Flick
+00002380: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
+00002390: 0000 0011 5065 6f70 6c65 2079 6f75 2066  ....People you f
+000023a0: 6f6c 6c6f 7707 0000 0009 466c 6963 6b72  ollow.....Flickr
+000023b0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+000023c0: 0000 0550 686f 746f 0700 0000 0946 6c69  ...Photo.....Fli
+000023d0: 636b 7254 6162 0103 ffff ffff 0800 0000  ckrTab..........
+000023e0: 0006 0000 0007 5072 6976 6174 6507 0000  ......Private...
+000023f0: 0009 466c 6963 6b72 5461 6201 03ff ffff  ..FlickrTab.....
+00002400: ff08 0000 0000 0600 0000 0650 7562 6c69  ...........Publi
+00002410: 6307 0000 0009 466c 6963 6b72 5461 6201  c.....FlickrTab.
+00002420: 03ff ffff ff08 0000 0000 0600 0000 1a52  ...............R
+00002430: 6570 6c61 6365 2069 6d61 6765 2072 6567  eplace image reg
+00002440: 696f 6e20 6e6f 7465 7307 0000 0009 466c  ion notes.....Fl
+00002450: 6963 6b72 5461 6201 03ff ffff ff08 0000  ickrTab.........
+00002460: 0000 0600 0000 1052 6570 6c61 6365 206d  .......Replace m
+00002470: 6574 6164 6174 6107 0000 0009 466c 6963  etadata.....Flic
+00002480: 6b72 5461 6201 03ff ffff ff08 0000 0000  krTab...........
+00002490: 0600 0000 0a52 6573 7472 6963 7465 6407  .....Restricted.
+000024a0: 0000 0009 466c 6963 6b72 5461 6201 03ff  ....FlickrTab...
+000024b0: ffff ff08 0000 0000 0600 0000 0453 6166  .............Saf
+000024c0: 6507 0000 0009 466c 6963 6b72 5461 6201  e.....FlickrTab.
+000024d0: 03ff ffff ff08 0000 0000 0600 0000 0c53  ...............S
+000024e0: 6166 6574 7920 6c65 7665 6c07 0000 0009  afety level.....
+000024f0: 466c 6963 6b72 5461 6201 03ff ffff ff08  FlickrTab.......
+00002500: 0000 0000 0600 0000 0a53 6372 6565 6e73  .........Screens
+00002510: 686f 7407 0000 0009 466c 6963 6b72 5461  hot.....FlickrTa
+00002520: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00002530: 0b53 796e 6368 726f 6e69 7365 0700 0000  .Synchronise....
+00002540: 0946 6c69 636b 7254 6162 0103 ffff ffff  .FlickrTab......
+00002550: 0800 0000 0006 0000 0005 5469 746c 6507  ..........Title.
+00002560: 0000 0009 466c 6963 6b72 5461 6201 03ff  ....FlickrTab...
+00002570: ffff ff08 0000 0000 0600 0000 0f56 6965  .............Vie
+00002580: 7769 6e67 2070 7269 7661 6379 0700 0000  wing privacy....
+00002590: 0946 6c69 636b 7254 6162 0103 ffff ffff  .FlickrTab......
+000025a0: 0800 0000 0006 0000 0013 5669 7274 7561  ..........Virtua
+000025b0: 6c20 5068 6f74 6f67 7261 7068 7907 0000  l Photography...
+000025c0: 0009 466c 6963 6b72 5461 6201 03ff ffff  ..FlickrTab.....
+000025d0: ff08 0000 0000 0600 0000 0b41 6c62 756d  ...........Album
+000025e0: 2074 6974 6c65 0700 0000 0f47 6f6f 676c   title.....Googl
+000025f0: 6550 686f 746f 7354 6162 0103 ffff ffff  ePhotosTab......
+00002600: 0800 0000 0006 0000 0080 4669 6c65 2022  ..........File "
+00002610: 7b66 696c 655f 6e61 6d65 7d22 2069 7320  {file_name}" is 
+00002620: 6f76 6572 2032 35c2 a04d 422e 2052 656d  over 25..MB. Rem
+00002630: 656d 6265 7220 7468 6174 2050 686f 7469  ember that Photi
+00002640: 6e69 2075 706c 6f61 6473 2063 6f75 6e74  ni uploads count
+00002650: 2074 6f77 6172 6473 2073 746f 7261 6765   towards storage
+00002660: 2069 6e20 796f 7572 2047 6f6f 676c 6520   in your Google 
+00002670: 4163 636f 756e 742e 2055 706c 6f61 6420  Account. Upload 
+00002680: 6974 2061 6e79 7761 793f 0700 0000 0f47  it anyway?.....G
 00002690: 6f6f 676c 6550 686f 746f 7354 6162 0103  ooglePhotosTab..
-000026a0: ffff ffff 0800 0000 0006 0000 0013 5068  ..............Ph
-000026b0: 6f74 696e 693a 206c 6172 6765 2066 696c  otini: large fil
-000026c0: 6507 0000 000f 476f 6f67 6c65 5068 6f74  e.....GooglePhot
-000026d0: 6f73 5461 6201 03ff ffff ff08 0000 0000  osTab...........
-000026e0: 0600 0000 2250 6c65 6173 6520 656e 7465  ...."Please ente
-000026f0: 7220 6120 7469 746c 6520 666f 7220 7468  r a title for th
-00002700: 6520 616c 6275 6d07 0000 000f 476f 6f67  e album.....Goog
-00002710: 6c65 5068 6f74 6f73 5461 6201 03ff ffff  lePhotosTab.....
-00002720: ff08 0000 0000 0600 0000 2c47 5058 2066  ..........,GPX f
-00002730: 696c 6573 2028 2a2e 6770 7820 2a2e 4750  iles (*.gpx *.GP
-00002740: 5820 2a2e 4770 7829 3b3b 416c 6c20 6669  X *.Gpx);;All fi
-00002750: 6c65 7320 282a 2907 0000 000b 4770 7849  les (*).....GpxI
-00002760: 6d70 6f72 7465 7201 03ff ffff ff08 0000  mporter.........
-00002770: 0000 0600 0000 0f49 6d70 6f72 7420 4750  .......Import GP
-00002780: 5820 6669 6c65 0700 0000 0b47 7078 496d  X file.....GpxIm
-00002790: 706f 7274 6572 0103 0000 0014 0043 006c  porter.......C.l
-000027a0: 006f 0073 0065 0020 0066 0069 006c 0065  .o.s.e. .f.i.l.e
-000027b0: 0300 0000 1600 4300 6c00 6f00 7300 6500  ......C.l.o.s.e.
-000027c0: 2000 6600 6900 6c00 6500 7308 0000 0000   .f.i.l.e.s.....
-000027d0: 0600 0000 0d43 6c6f 7365 2066 696c 6528  .....Close file(
-000027e0: 7329 0700 0000 0949 6d61 6765 4c69 7374  s).....ImageList
-000027f0: 0103 ffff ffff 0800 0000 0006 0000 0021  ...............!
-00002800: 446f 2079 6f75 2077 616e 7420 746f 2073  Do you want to s
-00002810: 6176 6520 796f 7572 2063 6861 6e67 6573  ave your changes
-00002820: 3f07 0000 0009 496d 6167 654c 6973 7401  ?.....ImageList.
-00002830: 03ff ffff ff08 0000 0000 0600 0000 2949  ..............)I
-00002840: 6d61 6765 7320 287b 307d 293b 3b56 6964  mages ({0});;Vid
-00002850: 656f 7320 287b 317d 293b 3b41 6c6c 2066  eos ({1});;All f
-00002860: 696c 6573 2028 2a29 0700 0000 0949 6d61  iles (*).....Ima
-00002870: 6765 4c69 7374 0103 ffff ffff 0800 0000  geList..........
-00002880: 0006 0000 0021 4d65 7461 6461 7461 2064  .....!Metadata d
-00002890: 6966 6665 7265 6e63 6573 3a20 7b66 696c  ifferences: {fil
-000028a0: 655f 6e61 6d65 7d07 0000 0009 496d 6167  e_name}.....Imag
-000028b0: 654c 6973 7401 03ff ffff ff08 0000 0000  eList...........
-000028c0: 0600 0000 144e 6f20 7468 756d 626e 6169  .....No thumbnai
-000028d0: 6c20 696e 2066 696c 6507 0000 0009 496d  l in file.....Im
-000028e0: 6167 654c 6973 7401 03ff ffff ff08 0000  ageList.........
-000028f0: 0000 0600 0000 0a4f 7065 6e20 6669 6c65  .......Open file
-00002900: 7307 0000 0009 496d 6167 654c 6973 7401  s.....ImageList.
-00002910: 03ff ffff ff08 0000 0000 0600 0000 1550  ...............P
-00002920: 686f 7469 6e69 3a20 756e 7361 7665 6420  hotini: unsaved 
-00002930: 6461 7461 0700 0000 0949 6d61 6765 4c69  data.....ImageLi
-00002940: 7374 0103 0000 0028 0052 0065 0067 0065  st.....(.R.e.g.e
-00002950: 006e 0065 0072 0061 0074 0065 0020 0074  .n.e.r.a.t.e. .t
-00002960: 0068 0075 006d 0062 006e 0061 0069 006c  .h.u.m.b.n.a.i.l
-00002970: 0300 0000 2a00 5200 6500 6700 6500 6e00  ....*.R.e.g.e.n.
-00002980: 6500 7200 6100 7400 6500 2000 7400 6800  e.r.a.t.e. .t.h.
-00002990: 7500 6d00 6200 6e00 6100 6900 6c00 7308  u.m.b.n.a.i.l.s.
-000029a0: 0000 0000 0600 0000 1752 6567 656e 6572  .........Regener
-000029b0: 6174 6520 7468 756d 626e 6169 6c28 7329  ate thumbnail(s)
-000029c0: 0700 0000 0949 6d61 6765 4c69 7374 0103  .....ImageList..
-000029d0: 0000 0016 0052 0065 006c 006f 0061 0064  .....R.e.l.o.a.d
-000029e0: 0020 0066 0069 006c 0065 0300 0000 1800  . .f.i.l.e......
-000029f0: 5200 6500 6c00 6f00 6100 6400 2000 6600  R.e.l.o.a.d. .f.
-00002a00: 6900 6c00 6500 7308 0000 0000 0600 0000  i.l.e.s.........
-00002a10: 0e52 656c 6f61 6420 6669 6c65 2873 2907  .Reload file(s).
-00002a20: 0000 0009 496d 6167 654c 6973 7401 03ff  ....ImageList...
-00002a30: ffff ff08 0000 0000 0600 0000 0c53 6176  .............Sav
-00002a40: 6520 6368 616e 6765 7307 0000 0009 496d  e changes.....Im
-00002a50: 6167 654c 6973 7401 03ff ffff ff08 0000  ageList.........
-00002a60: 0000 0600 0000 2253 6f6d 6520 696d 6167  ......"Some imag
-00002a70: 6573 2068 6176 6520 756e 7361 7665 6420  es have unsaved 
-00002a80: 6d65 7461 6461 7461 2e07 0000 0009 496d  metadata......Im
-00002a90: 6167 654c 6973 7401 03ff ffff ff08 0000  ageList.........
-00002aa0: 0000 0600 0000 0753 6f72 7420 6279 0700  .......Sort by..
-00002ab0: 0000 0949 6d61 6765 4c69 7374 0103 ffff  ...ImageList....
-00002ac0: ffff 0800 0000 0006 0000 000e 5468 756d  ............Thum
-00002ad0: 626e 6169 6c20 7369 7a65 0700 0000 0949  bnail size.....I
-00002ae0: 6d61 6765 4c69 7374 0103 ffff ffff 0800  mageList........
-00002af0: 0000 0006 0000 000c 5669 6577 2063 6861  ........View cha
-00002b00: 6e67 6573 0700 0000 0949 6d61 6765 4c69  nges.....ImageLi
-00002b10: 7374 0103 ffff ffff 0800 0000 0006 0000  st..............
-00002b20: 000a 6461 7465 2074 616b 656e 0700 0000  ..date taken....
-00002b30: 0949 6d61 6765 4c69 7374 0103 ffff ffff  .ImageList......
-00002b40: 0800 0000 0006 0000 0009 6669 6c65 206e  ..........file n
-00002b50: 616d 6507 0000 0009 496d 6167 654c 6973  ame.....ImageLis
-00002b60: 7401 03ff ffff ff08 0000 0000 0600 0000  t...............
-00002b70: 096e 6577 2076 616c 7565 0700 0000 0949  .new value.....I
-00002b80: 6d61 6765 4c69 7374 0103 ffff ffff 0800  mageList........
-00002b90: 0000 0006 0000 0009 6f6c 6420 7661 6c75  ........old valu
-00002ba0: 6507 0000 0009 496d 6167 654c 6973 7401  e.....ImageList.
-00002bb0: 03ff ffff ff08 0000 0000 0600 0000 0475  ...............u
-00002bc0: 6e64 6f07 0000 0009 496d 6167 654c 6973  ndo.....ImageLis
-00002bd0: 7401 0300 0000 2000 2500 6e00 2000 6600  t..... .%.n. .f.
-00002be0: 6900 6c00 6500 2000 7300 6500 6c00 6500  i.l.e. .s.e.l.e.
-00002bf0: 6300 7400 6500 6403 0000 0022 0025 006e  c.t.e.d....".%.n
-00002c00: 0020 0066 0069 006c 0065 0073 0020 0073  . .f.i.l.e.s. .s
-00002c10: 0065 006c 0065 0063 0074 0065 0064 0800  .e.l.e.c.t.e.d..
-00002c20: 0000 0006 0000 0013 256e 2066 696c 6528  ........%n file(
-00002c30: 7329 2073 656c 6563 7465 6407 0000 000b  s) selected.....
-00002c40: 496d 706f 7274 6572 5461 6201 03ff ffff  ImporterTab.....
-00002c50: ff08 0000 0000 0600 0000 0e26 496d 706f  ...........&Impo
-00002c60: 7274 2070 686f 746f 7307 0000 000b 496d  rt photos.....Im
-00002c70: 706f 7274 6572 5461 6201 03ff ffff ff08  porterTab.......
-00002c80: 0000 0000 0600 0000 0e3c 6164 6420 6120  .........<add a 
-00002c90: 666f 6c64 6572 3e07 0000 000b 496d 706f  folder>.....Impo
-00002ca0: 7274 6572 5461 6201 03ff ffff ff08 0000  rterTab.........
-00002cb0: 0000 0600 0000 0f3c 7365 6c65 6374 2073  .......<select s
-00002cc0: 6f75 7263 653e 0700 0000 0b49 6d70 6f72  ource>.....Impor
-00002cd0: 7465 7254 6162 0103 ffff ffff 0800 0000  terTab..........
-00002ce0: 0006 0000 0026 436c 6f73 696e 6720 6e6f  .....&Closing no
-00002cf0: 7720 7769 6c6c 2074 6572 6d69 6e61 7465  w will terminate
-00002d00: 2074 6865 2069 6d70 6f72 742e 0700 0000   the import.....
-00002d10: 0b49 6d70 6f72 7465 7254 6162 0103 ffff  .ImporterTab....
-00002d20: ffff 0800 0000 0006 0000 000b 436f 7079  ............Copy
-00002d30: 2070 686f 746f 7307 0000 000b 496d 706f   photos.....Impo
-00002d40: 7274 6572 5461 6201 03ff ffff ff08 0000  rterTab.........
-00002d50: 0000 0600 0000 2249 6d70 6f72 7469 6e67  ......"Importing
-00002d60: 2070 686f 746f 7320 6861 7320 6e6f 7420   photos has not 
-00002d70: 6669 6e69 7368 6564 2e07 0000 000b 496d  finished......Im
-00002d80: 706f 7274 6572 5461 6201 03ff ffff ff08  porterTab.......
-00002d90: 0000 0000 0600 0000 0b4d 6f76 6520 7068  .........Move ph
-00002da0: 6f74 6f73 0700 0000 0b49 6d70 6f72 7465  otos.....Importe
-00002db0: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
-00002dc0: 0000 001b 5068 6f74 696e 693a 2069 6d70  ....Photini: imp
-00002dd0: 6f72 7420 696e 2070 726f 6772 6573 7307  ort in progress.
-00002de0: 0000 000b 496d 706f 7274 6572 5461 6201  ....ImporterTab.
-00002df0: 03ff ffff ff08 0000 0000 0600 0000 1652  ...............R
-00002e00: 656d 6f76 6520 227b 736f 7572 6365 5f6e  emove "{source_n
-00002e10: 616d 657d 2207 0000 000b 496d 706f 7274  ame}".....Import
-00002e20: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
-00002e30: 0600 0000 0a53 656c 6563 7420 616c 6c07  .....Select all.
+000026a0: ffff ffff 0800 0000 0006 0000 0015 476f  ..............Go
+000026b0: 6f67 6c65 2026 5068 6f74 6f73 2075 706c  ogle &Photos upl
+000026c0: 6f61 6407 0000 000f 476f 6f67 6c65 5068  oad.....GooglePh
+000026d0: 6f74 6f73 5461 6201 03ff ffff ff08 0000  otosTab.........
+000026e0: 0000 0600 0000 0d47 6f6f 676c 6520 5068  .......Google Ph
+000026f0: 6f74 6f73 0700 0000 0f47 6f6f 676c 6550  otos.....GoogleP
+00002700: 686f 746f 7354 6162 0103 ffff ffff 0800  hotosTab........
+00002710: 0000 0006 0000 000b 4c61 7267 6520 6669  ........Large fi
+00002720: 6c65 2e07 0000 000f 476f 6f67 6c65 5068  le......GooglePh
+00002730: 6f74 6f73 5461 6201 03ff ffff ff08 0000  otosTab.........
+00002740: 0000 0600 0000 094e 6577 2061 6c62 756d  .......New album
+00002750: 0700 0000 0f47 6f6f 676c 6550 686f 746f  .....GooglePhoto
+00002760: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
+00002770: 0000 0013 5068 6f74 696e 693a 206c 6172  ....Photini: lar
+00002780: 6765 2066 696c 6507 0000 000f 476f 6f67  ge file.....Goog
+00002790: 6c65 5068 6f74 6f73 5461 6201 03ff ffff  lePhotosTab.....
+000027a0: ff08 0000 0000 0600 0000 2250 6c65 6173  .........."Pleas
+000027b0: 6520 656e 7465 7220 6120 7469 746c 6520  e enter a title 
+000027c0: 666f 7220 7468 6520 616c 6275 6d07 0000  for the album...
+000027d0: 000f 476f 6f67 6c65 5068 6f74 6f73 5461  ..GooglePhotosTa
+000027e0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+000027f0: 2c47 5058 2066 696c 6573 2028 2a2e 6770  ,GPX files (*.gp
+00002800: 7820 2a2e 4750 5820 2a2e 4770 7829 3b3b  x *.GPX *.Gpx);;
+00002810: 416c 6c20 6669 6c65 7320 282a 2907 0000  All files (*)...
+00002820: 000b 4770 7849 6d70 6f72 7465 7201 03ff  ..GpxImporter...
+00002830: ffff ff08 0000 0000 0600 0000 0f49 6d70  .............Imp
+00002840: 6f72 7420 4750 5820 6669 6c65 0700 0000  ort GPX file....
+00002850: 0b47 7078 496d 706f 7274 6572 0103 0000  .GpxImporter....
+00002860: 0014 0043 006c 006f 0073 0065 0020 0066  ...C.l.o.s.e. .f
+00002870: 0069 006c 0065 0300 0000 1600 4300 6c00  .i.l.e......C.l.
+00002880: 6f00 7300 6500 2000 6600 6900 6c00 6500  o.s.e. .f.i.l.e.
+00002890: 7308 0000 0000 0600 0000 0d43 6c6f 7365  s..........Close
+000028a0: 2066 696c 6528 7329 0700 0000 0949 6d61   file(s).....Ima
+000028b0: 6765 4c69 7374 0103 ffff ffff 0800 0000  geList..........
+000028c0: 0006 0000 0021 446f 2079 6f75 2077 616e  .....!Do you wan
+000028d0: 7420 746f 2073 6176 6520 796f 7572 2063  t to save your c
+000028e0: 6861 6e67 6573 3f07 0000 0009 496d 6167  hanges?.....Imag
+000028f0: 654c 6973 7401 03ff ffff ff08 0000 0000  eList...........
+00002900: 0600 0000 2949 6d61 6765 7320 287b 307d  ....)Images ({0}
+00002910: 293b 3b56 6964 656f 7320 287b 317d 293b  );;Videos ({1});
+00002920: 3b41 6c6c 2066 696c 6573 2028 2a29 0700  ;All files (*)..
+00002930: 0000 0949 6d61 6765 4c69 7374 0103 ffff  ...ImageList....
+00002940: ffff 0800 0000 0006 0000 0021 4d65 7461  ...........!Meta
+00002950: 6461 7461 2064 6966 6665 7265 6e63 6573  data differences
+00002960: 3a20 7b66 696c 655f 6e61 6d65 7d07 0000  : {file_name}...
+00002970: 0009 496d 6167 654c 6973 7401 03ff ffff  ..ImageList.....
+00002980: ff08 0000 0000 0600 0000 144e 6f20 7468  ...........No th
+00002990: 756d 626e 6169 6c20 696e 2066 696c 6507  umbnail in file.
+000029a0: 0000 0009 496d 6167 654c 6973 7401 03ff  ....ImageList...
+000029b0: ffff ff08 0000 0000 0600 0000 0a4f 7065  .............Ope
+000029c0: 6e20 6669 6c65 7307 0000 0009 496d 6167  n files.....Imag
+000029d0: 654c 6973 7401 03ff ffff ff08 0000 0000  eList...........
+000029e0: 0600 0000 1550 686f 7469 6e69 3a20 756e  .....Photini: un
+000029f0: 7361 7665 6420 6461 7461 0700 0000 0949  saved data.....I
+00002a00: 6d61 6765 4c69 7374 0103 0000 0028 0052  mageList.....(.R
+00002a10: 0065 0067 0065 006e 0065 0072 0061 0074  .e.g.e.n.e.r.a.t
+00002a20: 0065 0020 0074 0068 0075 006d 0062 006e  .e. .t.h.u.m.b.n
+00002a30: 0061 0069 006c 0300 0000 2a00 5200 6500  .a.i.l....*.R.e.
+00002a40: 6700 6500 6e00 6500 7200 6100 7400 6500  g.e.n.e.r.a.t.e.
+00002a50: 2000 7400 6800 7500 6d00 6200 6e00 6100   .t.h.u.m.b.n.a.
+00002a60: 6900 6c00 7308 0000 0000 0600 0000 1752  i.l.s..........R
+00002a70: 6567 656e 6572 6174 6520 7468 756d 626e  egenerate thumbn
+00002a80: 6169 6c28 7329 0700 0000 0949 6d61 6765  ail(s).....Image
+00002a90: 4c69 7374 0103 0000 0016 0052 0065 006c  List.......R.e.l
+00002aa0: 006f 0061 0064 0020 0066 0069 006c 0065  .o.a.d. .f.i.l.e
+00002ab0: 0300 0000 1800 5200 6500 6c00 6f00 6100  ......R.e.l.o.a.
+00002ac0: 6400 2000 6600 6900 6c00 6500 7308 0000  d. .f.i.l.e.s...
+00002ad0: 0000 0600 0000 0e52 656c 6f61 6420 6669  .......Reload fi
+00002ae0: 6c65 2873 2907 0000 0009 496d 6167 654c  le(s).....ImageL
+00002af0: 6973 7401 03ff ffff ff08 0000 0000 0600  ist.............
+00002b00: 0000 0c53 6176 6520 6368 616e 6765 7307  ...Save changes.
+00002b10: 0000 0009 496d 6167 654c 6973 7401 03ff  ....ImageList...
+00002b20: ffff ff08 0000 0000 0600 0000 2253 6f6d  ............"Som
+00002b30: 6520 696d 6167 6573 2068 6176 6520 756e  e images have un
+00002b40: 7361 7665 6420 6d65 7461 6461 7461 2e07  saved metadata..
+00002b50: 0000 0009 496d 6167 654c 6973 7401 03ff  ....ImageList...
+00002b60: ffff ff08 0000 0000 0600 0000 0753 6f72  .............Sor
+00002b70: 7420 6279 0700 0000 0949 6d61 6765 4c69  t by.....ImageLi
+00002b80: 7374 0103 ffff ffff 0800 0000 0006 0000  st..............
+00002b90: 000e 5468 756d 626e 6169 6c20 7369 7a65  ..Thumbnail size
+00002ba0: 0700 0000 0949 6d61 6765 4c69 7374 0103  .....ImageList..
+00002bb0: ffff ffff 0800 0000 0006 0000 000c 5669  ..............Vi
+00002bc0: 6577 2063 6861 6e67 6573 0700 0000 0949  ew changes.....I
+00002bd0: 6d61 6765 4c69 7374 0103 ffff ffff 0800  mageList........
+00002be0: 0000 0006 0000 000a 6461 7465 2074 616b  ........date tak
+00002bf0: 656e 0700 0000 0949 6d61 6765 4c69 7374  en.....ImageList
+00002c00: 0103 ffff ffff 0800 0000 0006 0000 0009  ................
+00002c10: 6669 6c65 206e 616d 6507 0000 0009 496d  file name.....Im
+00002c20: 6167 654c 6973 7401 03ff ffff ff08 0000  ageList.........
+00002c30: 0000 0600 0000 096e 6577 2076 616c 7565  .......new value
+00002c40: 0700 0000 0949 6d61 6765 4c69 7374 0103  .....ImageList..
+00002c50: ffff ffff 0800 0000 0006 0000 0009 6f6c  ..............ol
+00002c60: 6420 7661 6c75 6507 0000 0009 496d 6167  d value.....Imag
+00002c70: 654c 6973 7401 03ff ffff ff08 0000 0000  eList...........
+00002c80: 0600 0000 0475 6e64 6f07 0000 0009 496d  .....undo.....Im
+00002c90: 6167 654c 6973 7401 0300 0000 2000 2500  ageList..... .%.
+00002ca0: 6e00 2000 6600 6900 6c00 6500 2000 7300  n. .f.i.l.e. .s.
+00002cb0: 6500 6c00 6500 6300 7400 6500 6403 0000  e.l.e.c.t.e.d...
+00002cc0: 0022 0025 006e 0020 0066 0069 006c 0065  .".%.n. .f.i.l.e
+00002cd0: 0073 0020 0073 0065 006c 0065 0063 0074  .s. .s.e.l.e.c.t
+00002ce0: 0065 0064 0800 0000 0006 0000 0013 256e  .e.d..........%n
+00002cf0: 2066 696c 6528 7329 2073 656c 6563 7465   file(s) selecte
+00002d00: 6407 0000 000b 496d 706f 7274 6572 5461  d.....ImporterTa
+00002d10: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00002d20: 0e26 496d 706f 7274 2070 686f 746f 7307  .&Import photos.
+00002d30: 0000 000b 496d 706f 7274 6572 5461 6201  ....ImporterTab.
+00002d40: 03ff ffff ff08 0000 0000 0600 0000 0e3c  ...............<
+00002d50: 6164 6420 6120 666f 6c64 6572 3e07 0000  add a folder>...
+00002d60: 000b 496d 706f 7274 6572 5461 6201 03ff  ..ImporterTab...
+00002d70: ffff ff08 0000 0000 0600 0000 0f3c 7365  .............<se
+00002d80: 6c65 6374 2073 6f75 7263 653e 0700 0000  lect source>....
+00002d90: 0b49 6d70 6f72 7465 7254 6162 0103 ffff  .ImporterTab....
+00002da0: ffff 0800 0000 0006 0000 0026 436c 6f73  ...........&Clos
+00002db0: 696e 6720 6e6f 7720 7769 6c6c 2074 6572  ing now will ter
+00002dc0: 6d69 6e61 7465 2074 6865 2069 6d70 6f72  minate the impor
+00002dd0: 742e 0700 0000 0b49 6d70 6f72 7465 7254  t......ImporterT
+00002de0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00002df0: 000b 436f 7079 2070 686f 746f 7307 0000  ..Copy photos...
+00002e00: 000b 496d 706f 7274 6572 5461 6201 03ff  ..ImporterTab...
+00002e10: ffff ff08 0000 0000 0600 0000 2249 6d70  ............"Imp
+00002e20: 6f72 7469 6e67 2070 686f 746f 7320 6861  orting photos ha
+00002e30: 7320 6e6f 7420 6669 6e69 7368 6564 2e07  s not finished..
 00002e40: 0000 000b 496d 706f 7274 6572 5461 6201  ....ImporterTab.
-00002e50: 03ff ffff ff08 0000 0000 0600 0000 0a53  ...............S
-00002e60: 656c 6563 7420 6e65 7707 0000 000b 496d  elect new.....Im
-00002e70: 706f 7274 6572 5461 6201 03ff ffff ff08  porterTab.......
-00002e80: 0000 0000 0600 0000 1253 656c 6563 7420  .........Select 
-00002e90: 726f 6f74 2066 6f6c 6465 7207 0000 000b  root folder.....
-00002ea0: 496d 706f 7274 6572 5461 6201 03ff ffff  ImporterTab.....
-00002eb0: ff08 0000 0000 0600 0000 0653 6f75 7263  ...........Sourc
-00002ec0: 6507 0000 000b 496d 706f 7274 6572 5461  e.....ImporterTa
-00002ed0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00002ee0: 0953 746f 7020 636f 7079 0700 0000 0b49  .Stop copy.....I
-00002ef0: 6d70 6f72 7465 7254 6162 0103 ffff ffff  mporterTab......
-00002f00: 0800 0000 0006 0000 0009 5374 6f70 206d  ..........Stop m
-00002f10: 6f76 6507 0000 000b 496d 706f 7274 6572  ove.....Importer
-00002f20: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00002f30: 0000 0d54 6172 6765 7420 666f 726d 6174  ...Target format
-00002f40: 0700 0000 0b49 6d70 6f72 7465 7254 6162  .....ImporterTab
-00002f50: 0103 ffff ffff 0800 0000 0006 0000 0015  ................
-00002f60: 6361 6d65 7261 3a20 7b63 616d 6572 615f  camera: {camera_
-00002f70: 6e61 6d65 7d07 0000 000b 496d 706f 7274  name}.....Import
-00002f80: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
-00002f90: 0600 0000 1566 6f6c 6465 723a 207b 666f  .....folder: {fo
-00002fa0: 6c64 6572 5f6e 616d 657d 0700 0000 0b49  lder_name}.....I
-00002fb0: 6d70 6f72 7465 7254 6162 0103 ffff ffff  mporterTab......
-00002fc0: 0800 0000 0006 0000 0007 7265 6672 6573  ..........refres
-00002fd0: 6807 0000 000b 496d 706f 7274 6572 5461  h.....ImporterTa
-00002fe0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00002ff0: 1026 4970 6572 6e69 7479 2075 706c 6f61  .&Ipernity uploa
-00003000: 6407 0000 000b 4970 6572 6e69 7479 5461  d.....IpernityTa
-00003010: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00003020: 0b41 7474 7269 6275 7469 6f6e 0700 0000  .Attribution....
-00003030: 0b49 7065 726e 6974 7954 6162 0103 ffff  .IpernityTab....
-00003040: ffff 0800 0000 0006 0000 001b 4174 7472  ............Attr
-00003050: 6962 7574 696f 6e20 2b20 6e6f 2064 6572  ibution + no der
-00003060: 6976 6174 6976 6507 0000 000b 4970 6572  ivative.....Iper
-00003070: 6e69 7479 5461 6201 03ff ffff ff08 0000  nityTab.........
-00003080: 0000 0600 0000 1c41 7474 7269 6275 7469  .......Attributi
-00003090: 6f6e 202b 206e 6f6e 2063 6f6d 6d65 7263  on + non commerc
-000030a0: 6961 6c07 0000 000b 4970 6572 6e69 7479  ial.....Ipernity
-000030b0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-000030c0: 0000 2c41 7474 7269 6275 7469 6f6e 202b  ..,Attribution +
-000030d0: 206e 6f6e 2063 6f6d 6d65 7263 6961 6c20   non commercial 
-000030e0: 2b20 6e6f 2064 6572 6976 6174 6976 6507  + no derivative.
-000030f0: 0000 000b 4970 6572 6e69 7479 5461 6201  ....IpernityTab.
-00003100: 03ff ffff ff08 0000 0000 0600 0000 2a41  ..............*A
-00003110: 7474 7269 6275 7469 6f6e 202b 206e 6f6e  ttribution + non
-00003120: 2063 6f6d 6d65 7263 6961 6c20 2b20 7368   commercial + sh
-00003130: 6172 6520 616c 696b 6507 0000 000b 4970  are alike.....Ip
-00003140: 6572 6e69 7479 5461 6201 03ff ffff ff08  ernityTab.......
-00003150: 0000 0000 0600 0000 1941 7474 7269 6275  .........Attribu
-00003160: 7469 6f6e 202b 2073 6861 7265 2061 6c69  tion + share ali
-00003170: 6b65 0700 0000 0b49 7065 726e 6974 7954  ke.....IpernityT
-00003180: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00003190: 0017 4368 616e 6765 2061 6c62 756d 206d  ..Change album m
-000031a0: 656d 6265 7273 6869 7007 0000 000b 4970  embership.....Ip
-000031b0: 6572 6e69 7479 5461 6201 03ff ffff ff08  ernityTab.......
-000031c0: 0000 0000 0600 0000 1243 6861 6e67 6520  .........Change 
-000031d0: 7468 6520 6c69 6365 6e63 6507 0000 000b  the licence.....
-000031e0: 4970 6572 6e69 7479 5461 6201 03ff ffff  IpernityTab.....
-000031f0: ff08 0000 0000 0600 0000 1d43 6861 6e67  ...........Chang
-00003200: 6520 7768 6f20 6361 6e20 636f 6d6d 656e  e who can commen
-00003210: 7420 6f72 2074 6167 0700 0000 0b49 7065  t or tag.....Ipe
-00003220: 726e 6974 7954 6162 0103 ffff ffff 0800  rnityTab........
-00003230: 0000 0006 0000 0015 4368 616e 6765 2077  ........Change w
-00003240: 686f 2063 616e 2073 6565 2069 7407 0000  ho can see it...
-00003250: 000b 4970 6572 6e69 7479 5461 6201 03ff  ..IpernityTab...
-00003260: ffff ff08 0000 0000 0600 0000 0843 6f6e  .............Con
-00003270: 7461 6374 7307 0000 000b 4970 6572 6e69  tacts.....Iperni
-00003280: 7479 5461 6201 03ff ffff ff08 0000 0000  tyTab...........
-00003290: 0600 0000 1f43 6f70 7972 6967 6874 2028  .....Copyright (
-000032a0: 616c 6c20 7269 6768 7473 2072 6573 6572  all rights reser
-000032b0: 7665 6429 0700 0000 0b49 7065 726e 6974  ved).....Ipernit
-000032c0: 7954 6162 0103 ffff ffff 0800 0000 0006  yTab............
-000032d0: 0000 000b 4465 7363 7269 7074 696f 6e07  ....Description.
-000032e0: 0000 000b 4970 6572 6e69 7479 5461 6201  ....IpernityTab.
-000032f0: 03ff ffff ff08 0000 0000 0600 0000 0845  ...............E
-00003300: 7665 7279 6f6e 6507 0000 000b 4970 6572  veryone.....Iper
-00003310: 6e69 7479 5461 6201 03ff ffff ff08 0000  nityTab.........
-00003320: 0000 0600 0000 1145 7665 7279 6f6e 6520  .......Everyone 
-00003330: 2870 7562 6c69 6329 0700 0000 0b49 7065  (public).....Ipe
-00003340: 726e 6974 7954 6162 0103 ffff ffff 0800  rnityTab........
-00003350: 0000 0006 0000 0006 4661 6d69 6c79 0700  ........Family..
-00003360: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
-00003370: ffff ffff 0800 0000 0006 0000 0010 4661  ..............Fa
-00003380: 6d69 6c79 2026 2066 7269 656e 6473 0700  mily & friends..
-00003390: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
-000033a0: ffff ffff 0800 0000 0006 0000 002c 4672  .............,Fr
-000033b0: 6565 2075 7365 2028 636f 7079 7269 6768  ee use (copyrigh
-000033c0: 7420 7375 7272 656e 6465 7265 642c 206e  t surrendered, n
-000033d0: 6f20 6c69 6365 6e63 6529 0700 0000 0b49  o licence).....I
-000033e0: 7065 726e 6974 7954 6162 0103 ffff ffff  pernityTab......
-000033f0: 0800 0000 0006 0000 0007 4672 6965 6e64  ..........Friend
-00003400: 7307 0000 000b 4970 6572 6e69 7479 5461  s.....IpernityTa
-00003410: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00003420: 0849 7065 726e 6974 7907 0000 000b 4970  .Ipernity.....Ip
-00003430: 6572 6e69 7479 5461 6201 03ff ffff ff08  ernityTab.......
-00003440: 0000 0000 0600 0000 074c 6963 656e 6365  .........Licence
-00003450: 0700 0000 0b49 7065 726e 6974 7954 6162  .....IpernityTab
-00003460: 0103 ffff ffff 0800 0000 0006 0000 0009  ................
-00003470: 4e65 7720 616c 6275 6d07 0000 000b 4970  New album.....Ip
-00003480: 6572 6e69 7479 5461 6201 03ff ffff ff08  ernityTab.......
-00003490: 0000 0000 0600 0000 084f 6e6c 7920 796f  .........Only yo
-000034a0: 7507 0000 000b 4970 6572 6e69 7479 5461  u.....IpernityTa
-000034b0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-000034c0: 124f 6e6c 7920 796f 7520 2870 7269 7661  .Only you (priva
-000034d0: 7465 2907 0000 000b 4970 6572 6e69 7479  te).....Ipernity
-000034e0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-000034f0: 0000 1a52 6570 6c61 6365 2069 6d61 6765  ...Replace image
-00003500: 2072 6567 696f 6e20 6e6f 7465 7307 0000   region notes...
-00003510: 000b 4970 6572 6e69 7479 5461 6201 03ff  ..IpernityTab...
-00003520: ffff ff08 0000 0000 0600 0000 1052 6570  .............Rep
-00003530: 6c61 6365 206d 6574 6164 6174 6107 0000  lace metadata...
-00003540: 000b 4970 6572 6e69 7479 5461 6201 03ff  ..IpernityTab...
-00003550: ffff ff08 0000 0000 0600 0000 0b53 796e  .............Syn
-00003560: 6368 726f 6e69 7365 0700 0000 0b49 7065  chronise.....Ipe
-00003570: 726e 6974 7954 6162 0103 ffff ffff 0800  rnityTab........
-00003580: 0000 0006 0000 0005 5469 746c 6507 0000  ........Title...
-00003590: 000b 4970 6572 6e69 7479 5461 6201 03ff  ..IpernityTab...
-000035a0: ffff ff08 0000 0000 0600 0000 1857 686f  .............Who
-000035b0: 2063 616e 2063 6f6d 6d65 6e74 206f 6e20   can comment on 
-000035c0: 616c 6275 6d07 0000 000b 4970 6572 6e69  album.....Iperni
-000035d0: 7479 5461 6201 03ff ffff ff08 0000 0000  tyTab...........
-000035e0: 0600 0000 0857 686f 2063 616e 3a07 0000  .....Who can:...
-000035f0: 000b 4970 6572 6e69 7479 5461 6201 03ff  ..IpernityTab...
-00003600: ffff ff08 0000 0000 0600 0000 1361 6464  .............add
-00003610: 206b 6579 776f 7264 732c 206e 6f74 6573   keywords, notes
-00003620: 0700 0000 0b49 7065 726e 6974 7954 6162  .....IpernityTab
-00003630: 0103 ffff ffff 0800 0000 0006 0000 000f  ................
-00003640: 6964 656e 7469 6679 2070 656f 706c 6507  identify people.
-00003650: 0000 000b 4970 6572 6e69 7479 5461 6201  ....IpernityTab.
-00003660: 03ff ffff ff08 0000 0000 0600 0000 0e70  ...............p
-00003670: 6f73 7420 6120 636f 6d6d 656e 7407 0000  ost a comment...
-00003680: 000b 4970 6572 6e69 7479 5461 6201 03ff  ..IpernityTab...
-00003690: ffff ff08 0000 0000 0600 0000 0d73 6565  .............see
-000036a0: 2074 6865 2070 686f 746f 0700 0000 0b49   the photo.....I
-000036b0: 7065 726e 6974 7954 6162 0103 ffff ffff  pernityTab......
-000036c0: 0800 0000 0006 0000 0006 4c61 6e67 3a20  ..........Lang: 
-000036d0: 0700 0000 0d4c 616e 6741 6c74 5769 6467  .....LangAltWidg
-000036e0: 6574 0103 ffff ffff 0800 0000 0006 0000  et..............
-000036f0: 0008 4c61 6e67 7561 6765 0700 0000 0d4c  ..Language.....L
-00003700: 616e 6741 6c74 5769 6467 6574 0103 ffff  angAltWidget....
-00003710: ffff 0800 0000 0006 0000 000c 4e65 7720  ............New 
-00003720: 6c61 6e67 7561 6765 0700 0000 0d4c 616e  language.....Lan
-00003730: 6741 6c74 5769 6467 6574 0103 ffff ffff  gAltWidget......
-00003740: 0800 0000 0006 0000 0014 5365 7420 6465  ..........Set de
-00003750: 6661 756c 7420 6c61 6e67 7561 6765 0700  fault language..
-00003760: 0000 0d4c 616e 6741 6c74 5769 6467 6574  ...LangAltWidget
-00003770: 0103 ffff ffff 0800 0000 0006 0000 004b  ...............K
-00003780: 5768 6174 206c 616e 6775 6167 6520 6973  What language is
-00003790: 2074 6865 2063 7572 7265 6e74 2074 6578   the current tex
-000037a0: 7420 696e 3f20 506c 6561 7365 2065 6e74  t in? Please ent
-000037b0: 6572 2061 6e20 5246 4333 3036 3620 6c61  er an RFC3066 la
-000037c0: 6e67 7561 6765 2074 6167 2e07 0000 000d  nguage tag......
-000037d0: 4c61 6e67 416c 7457 6964 6765 7401 03ff  LangAltWidget...
-000037e0: ffff ff08 0000 0000 0600 0000 4a57 6861  ............JWha
-000037f0: 7420 6c61 6e67 7561 6765 2077 6f75 6c64  t language would
-00003800: 2079 6f75 206c 696b 6520 746f 2061 6464   you like to add
-00003810: 3f20 506c 6561 7365 2065 6e74 6572 2061  ? Please enter a
-00003820: 6e20 5246 4333 3036 3620 6c61 6e67 7561  n RFC3066 langua
-00003830: 6765 2074 6167 2e07 0000 000d 4c61 6e67  ge tag......Lang
-00003840: 416c 7457 6964 6765 7401 03ff ffff ff08  AltWidget.......
-00003850: 0000 0000 0600 0000 094c 6174 2c20 6c6f  .........Lat, lo
-00003860: 6e67 0700 0000 0e4c 6174 4c6f 6e67 4469  ng.....LatLongDi
-00003870: 7370 6c61 7901 03ff ffff ff08 0000 0000  splay...........
-00003880: 0600 0000 504c 6174 6974 7564 6520 616e  ....PLatitude an
-00003890: 6420 6c6f 6e67 6974 7564 6520 2869 6e20  d longitude (in 
-000038a0: 6465 6772 6565 7329 2061 7320 7477 6f20  degrees) as two 
-000038b0: 6465 6369 6d61 6c20 6e75 6d62 6572 7320  decimal numbers 
-000038c0: 7365 7061 7261 7465 6420 6279 2061 2063  separated by a c
-000038d0: 6f6d 6d61 2e07 0000 000e 4c61 744c 6f6e  omma......LatLon
-000038e0: 6744 6973 706c 6179 0103 ffff ffff 0800  gDisplay........
-000038f0: 0000 0006 0000 0015 5068 6f74 696e 6920  ........Photini 
-00003900: 6572 726f 7220 6c6f 6767 696e 6707 0000  error logging...
-00003910: 000c 4c6f 6767 6572 5769 6e64 6f77 0103  ..LoggerWindow..
-00003920: ffff ffff 0800 0000 0006 0000 000d 5361  ..............Sa
-00003930: 7665 206c 6f67 2066 696c 6507 0000 000c  ve log file.....
-00003940: 4c6f 6767 6572 5769 6e64 6f77 0103 ffff  LoggerWindow....
-00003950: ffff 0800 0000 0006 0000 000b 4d61 7020  ............Map 
-00003960: 2826 4269 6e67 2907 0000 000a 4d61 7054  (&Bing).....MapT
-00003970: 6162 4269 6e67 0103 ffff ffff 0800 0000  abBing..........
-00003980: 0006 0000 002b 5365 6172 6368 2061 6e64  .....+Search and
-00003990: 2061 6c74 6974 7564 6520 6c6f 6f6b 7570   altitude lookup
-000039a0: 2070 726f 7669 6465 6420 6279 2042 696e   provided by Bin
-000039b0: 6707 0000 000a 4d61 7054 6162 4269 6e67  g.....MapTabBing
-000039c0: 0103 ffff ffff 0800 0000 0006 0000 0021  ...............!
-000039d0: 5365 7276 6572 206f 7665 726c 6f61 642c  Server overload,
-000039e0: 2070 6c65 6173 6520 7472 7920 6167 6169   please try agai
-000039f0: 6e07 0000 000a 4d61 7054 6162 4269 6e67  n.....MapTabBing
-00003a00: 0103 ffff ffff 0800 0000 0006 0000 000d  ................
-00003a10: 4d61 7020 2826 476f 6f67 6c65 2907 0000  Map (&Google)...
-00003a20: 000c 4d61 7054 6162 476f 6f67 6c65 0103  ..MapTabGoogle..
-00003a30: ffff ffff 0800 0000 0006 0000 002c 5365  .............,Se
-00003a40: 6172 6368 2061 6e64 2061 6c74 6974 7564  arch and altitud
-00003a50: 6520 6c6f 6f6b 7570 2070 6f77 6572 6564  e lookup powered
-00003a60: 2062 7920 476f 6f67 6c65 0700 0000 0c4d   by Google.....M
-00003a70: 6170 5461 6247 6f6f 676c 6501 03ff ffff  apTabGoogle.....
-00003a80: ff08 0000 0000 0600 0000 0d4d 6170 2028  ...........Map (
-00003a90: 264d 6170 626f 7829 0700 0000 0c4d 6170  &Mapbox).....Map
-00003aa0: 5461 624d 6170 626f 7801 03ff ffff ff08  TabMapbox.......
-00003ab0: 0000 0000 0600 0000 1853 6561 7263 6820  .........Search 
-00003ac0: 706f 7765 7265 6420 6279 204d 6170 626f  powered by Mapbo
-00003ad0: 7807 0000 000c 4d61 7054 6162 4d61 7062  x.....MapTabMapb
-00003ae0: 6f78 0103 ffff ffff 0800 0000 0006 0000  ox..............
-00003af0: 000d 4162 6f75 7420 5068 6f74 696e 6907  ..About Photini.
-00003b00: 0000 0007 4d65 6e75 4261 7201 03ff ffff  ....MenuBar.....
-00003b10: ff08 0000 0000 0600 0000 5141 6e20 6561  ..........QAn ea
-00003b20: 7379 2074 6f20 7573 6520 6469 6769 7461  sy to use digita
-00003b30: 6c20 7068 6f74 6f67 7261 7068 206d 6574  l photograph met
-00003b40: 6164 6174 6120 2845 7869 662c 2049 5054  adata (Exif, IPT
-00003b50: 432c 2058 4d50 2920 6564 6974 696e 6720  C, XMP) editing 
-00003b60: 6170 706c 6963 6174 696f 6e2e 0700 0000  application.....
-00003b70: 074d 656e 7542 6172 0103 ffff ffff 0800  .MenuBar........
-00003b80: 0000 0006 0000 0010 4368 6563 6b20 666f  ........Check fo
-00003b90: 7220 7570 6461 7465 0700 0000 074d 656e  r update.....Men
-00003ba0: 7542 6172 0103 ffff ffff 0800 0000 0006  uBar............
-00003bb0: 0000 000f 436c 6f73 6520 616c 6c20 6669  ....Close all fi
-00003bc0: 6c65 7307 0000 0007 4d65 6e75 4261 7201  les.....MenuBar.
-00003bd0: 03ff ffff ff08 0000 0000 0600 0000 1245  ...............E
-00003be0: 6e61 626c 6520 7370 656c 6c20 6368 6563  nable spell chec
-00003bf0: 6b07 0000 0007 4d65 6e75 4261 7201 03ff  k.....MenuBar...
-00003c00: ffff ff08 0000 0000 0600 0000 0446 696c  .............Fil
-00003c10: 6507 0000 0007 4d65 6e75 4261 7201 03ff  e.....MenuBar...
-00003c20: ffff ff08 0000 0000 0600 0000 1646 6978  .............Fix
-00003c30: 206d 6973 7369 6e67 2074 6875 6d62 6e61   missing thumbna
-00003c40: 696c 7307 0000 0007 4d65 6e75 4261 7201  ils.....MenuBar.
-00003c50: 03ff ffff ff08 0000 0000 0600 0000 0448  ...............H
-00003c60: 656c 7007 0000 0007 4d65 6e75 4261 7201  elp.....MenuBar.
-00003c70: 03ff ffff ff08 0000 0000 0600 0000 0a4f  ...............O
-00003c80: 7065 6e20 6669 6c65 7307 0000 0007 4d65  pen files.....Me
+00002e50: 03ff ffff ff08 0000 0000 0600 0000 0b4d  ...............M
+00002e60: 6f76 6520 7068 6f74 6f73 0700 0000 0b49  ove photos.....I
+00002e70: 6d70 6f72 7465 7254 6162 0103 ffff ffff  mporterTab......
+00002e80: 0800 0000 0006 0000 001b 5068 6f74 696e  ..........Photin
+00002e90: 693a 2069 6d70 6f72 7420 696e 2070 726f  i: import in pro
+00002ea0: 6772 6573 7307 0000 000b 496d 706f 7274  gress.....Import
+00002eb0: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
+00002ec0: 0600 0000 1652 656d 6f76 6520 227b 736f  .....Remove "{so
+00002ed0: 7572 6365 5f6e 616d 657d 2207 0000 000b  urce_name}".....
+00002ee0: 496d 706f 7274 6572 5461 6201 03ff ffff  ImporterTab.....
+00002ef0: ff08 0000 0000 0600 0000 0a53 656c 6563  ...........Selec
+00002f00: 7420 616c 6c07 0000 000b 496d 706f 7274  t all.....Import
+00002f10: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
+00002f20: 0600 0000 0a53 656c 6563 7420 6e65 7707  .....Select new.
+00002f30: 0000 000b 496d 706f 7274 6572 5461 6201  ....ImporterTab.
+00002f40: 03ff ffff ff08 0000 0000 0600 0000 1253  ...............S
+00002f50: 656c 6563 7420 726f 6f74 2066 6f6c 6465  elect root folde
+00002f60: 7207 0000 000b 496d 706f 7274 6572 5461  r.....ImporterTa
+00002f70: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00002f80: 0653 6f75 7263 6507 0000 000b 496d 706f  .Source.....Impo
+00002f90: 7274 6572 5461 6201 03ff ffff ff08 0000  rterTab.........
+00002fa0: 0000 0600 0000 0953 746f 7020 636f 7079  .......Stop copy
+00002fb0: 0700 0000 0b49 6d70 6f72 7465 7254 6162  .....ImporterTab
+00002fc0: 0103 ffff ffff 0800 0000 0006 0000 0009  ................
+00002fd0: 5374 6f70 206d 6f76 6507 0000 000b 496d  Stop move.....Im
+00002fe0: 706f 7274 6572 5461 6201 03ff ffff ff08  porterTab.......
+00002ff0: 0000 0000 0600 0000 0d54 6172 6765 7420  .........Target 
+00003000: 666f 726d 6174 0700 0000 0b49 6d70 6f72  format.....Impor
+00003010: 7465 7254 6162 0103 ffff ffff 0800 0000  terTab..........
+00003020: 0006 0000 0015 6361 6d65 7261 3a20 7b63  ......camera: {c
+00003030: 616d 6572 615f 6e61 6d65 7d07 0000 000b  amera_name}.....
+00003040: 496d 706f 7274 6572 5461 6201 03ff ffff  ImporterTab.....
+00003050: ff08 0000 0000 0600 0000 1566 6f6c 6465  ...........folde
+00003060: 723a 207b 666f 6c64 6572 5f6e 616d 657d  r: {folder_name}
+00003070: 0700 0000 0b49 6d70 6f72 7465 7254 6162  .....ImporterTab
+00003080: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
+00003090: 7265 6672 6573 6807 0000 000b 496d 706f  refresh.....Impo
+000030a0: 7274 6572 5461 6201 03ff ffff ff08 0000  rterTab.........
+000030b0: 0000 0600 0000 1026 4970 6572 6e69 7479  .......&Ipernity
+000030c0: 2075 706c 6f61 6407 0000 000b 4970 6572   upload.....Iper
+000030d0: 6e69 7479 5461 6201 03ff ffff ff08 0000  nityTab.........
+000030e0: 0000 0600 0000 0b41 7474 7269 6275 7469  .......Attributi
+000030f0: 6f6e 0700 0000 0b49 7065 726e 6974 7954  on.....IpernityT
+00003100: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00003110: 001b 4174 7472 6962 7574 696f 6e20 2b20  ..Attribution + 
+00003120: 6e6f 2064 6572 6976 6174 6976 6507 0000  no derivative...
+00003130: 000b 4970 6572 6e69 7479 5461 6201 03ff  ..IpernityTab...
+00003140: ffff ff08 0000 0000 0600 0000 1c41 7474  .............Att
+00003150: 7269 6275 7469 6f6e 202b 206e 6f6e 2063  ribution + non c
+00003160: 6f6d 6d65 7263 6961 6c07 0000 000b 4970  ommercial.....Ip
+00003170: 6572 6e69 7479 5461 6201 03ff ffff ff08  ernityTab.......
+00003180: 0000 0000 0600 0000 2c41 7474 7269 6275  ........,Attribu
+00003190: 7469 6f6e 202b 206e 6f6e 2063 6f6d 6d65  tion + non comme
+000031a0: 7263 6961 6c20 2b20 6e6f 2064 6572 6976  rcial + no deriv
+000031b0: 6174 6976 6507 0000 000b 4970 6572 6e69  ative.....Iperni
+000031c0: 7479 5461 6201 03ff ffff ff08 0000 0000  tyTab...........
+000031d0: 0600 0000 2a41 7474 7269 6275 7469 6f6e  ....*Attribution
+000031e0: 202b 206e 6f6e 2063 6f6d 6d65 7263 6961   + non commercia
+000031f0: 6c20 2b20 7368 6172 6520 616c 696b 6507  l + share alike.
+00003200: 0000 000b 4970 6572 6e69 7479 5461 6201  ....IpernityTab.
+00003210: 03ff ffff ff08 0000 0000 0600 0000 1941  ...............A
+00003220: 7474 7269 6275 7469 6f6e 202b 2073 6861  ttribution + sha
+00003230: 7265 2061 6c69 6b65 0700 0000 0b49 7065  re alike.....Ipe
+00003240: 726e 6974 7954 6162 0103 ffff ffff 0800  rnityTab........
+00003250: 0000 0006 0000 0017 4368 616e 6765 2061  ........Change a
+00003260: 6c62 756d 206d 656d 6265 7273 6869 7007  lbum membership.
+00003270: 0000 000b 4970 6572 6e69 7479 5461 6201  ....IpernityTab.
+00003280: 03ff ffff ff08 0000 0000 0600 0000 1243  ...............C
+00003290: 6861 6e67 6520 7468 6520 6c69 6365 6e63  hange the licenc
+000032a0: 6507 0000 000b 4970 6572 6e69 7479 5461  e.....IpernityTa
+000032b0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+000032c0: 1d43 6861 6e67 6520 7768 6f20 6361 6e20  .Change who can 
+000032d0: 636f 6d6d 656e 7420 6f72 2074 6167 0700  comment or tag..
+000032e0: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
+000032f0: ffff ffff 0800 0000 0006 0000 0015 4368  ..............Ch
+00003300: 616e 6765 2077 686f 2063 616e 2073 6565  ange who can see
+00003310: 2069 7407 0000 000b 4970 6572 6e69 7479   it.....Ipernity
+00003320: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00003330: 0000 0843 6f6e 7461 6374 7307 0000 000b  ...Contacts.....
+00003340: 4970 6572 6e69 7479 5461 6201 03ff ffff  IpernityTab.....
+00003350: ff08 0000 0000 0600 0000 1f43 6f70 7972  ...........Copyr
+00003360: 6967 6874 2028 616c 6c20 7269 6768 7473  ight (all rights
+00003370: 2072 6573 6572 7665 6429 0700 0000 0b49   reserved).....I
+00003380: 7065 726e 6974 7954 6162 0103 ffff ffff  pernityTab......
+00003390: 0800 0000 0006 0000 000b 4465 7363 7269  ..........Descri
+000033a0: 7074 696f 6e07 0000 000b 4970 6572 6e69  ption.....Iperni
+000033b0: 7479 5461 6201 03ff ffff ff08 0000 0000  tyTab...........
+000033c0: 0600 0000 0845 7665 7279 6f6e 6507 0000  .....Everyone...
+000033d0: 000b 4970 6572 6e69 7479 5461 6201 03ff  ..IpernityTab...
+000033e0: ffff ff08 0000 0000 0600 0000 1145 7665  .............Eve
+000033f0: 7279 6f6e 6520 2870 7562 6c69 6329 0700  ryone (public)..
+00003400: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
+00003410: ffff ffff 0800 0000 0006 0000 0006 4661  ..............Fa
+00003420: 6d69 6c79 0700 0000 0b49 7065 726e 6974  mily.....Ipernit
+00003430: 7954 6162 0103 ffff ffff 0800 0000 0006  yTab............
+00003440: 0000 0010 4661 6d69 6c79 2026 2066 7269  ....Family & fri
+00003450: 656e 6473 0700 0000 0b49 7065 726e 6974  ends.....Ipernit
+00003460: 7954 6162 0103 ffff ffff 0800 0000 0006  yTab............
+00003470: 0000 002c 4672 6565 2075 7365 2028 636f  ...,Free use (co
+00003480: 7079 7269 6768 7420 7375 7272 656e 6465  pyright surrende
+00003490: 7265 642c 206e 6f20 6c69 6365 6e63 6529  red, no licence)
+000034a0: 0700 0000 0b49 7065 726e 6974 7954 6162  .....IpernityTab
+000034b0: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
+000034c0: 4672 6965 6e64 7307 0000 000b 4970 6572  Friends.....Iper
+000034d0: 6e69 7479 5461 6201 03ff ffff ff08 0000  nityTab.........
+000034e0: 0000 0600 0000 0849 7065 726e 6974 7907  .......Ipernity.
+000034f0: 0000 000b 4970 6572 6e69 7479 5461 6201  ....IpernityTab.
+00003500: 03ff ffff ff08 0000 0000 0600 0000 074c  ...............L
+00003510: 6963 656e 6365 0700 0000 0b49 7065 726e  icence.....Ipern
+00003520: 6974 7954 6162 0103 ffff ffff 0800 0000  ityTab..........
+00003530: 0006 0000 0009 4e65 7720 616c 6275 6d07  ......New album.
+00003540: 0000 000b 4970 6572 6e69 7479 5461 6201  ....IpernityTab.
+00003550: 03ff ffff ff08 0000 0000 0600 0000 084f  ...............O
+00003560: 6e6c 7920 796f 7507 0000 000b 4970 6572  nly you.....Iper
+00003570: 6e69 7479 5461 6201 03ff ffff ff08 0000  nityTab.........
+00003580: 0000 0600 0000 124f 6e6c 7920 796f 7520  .......Only you 
+00003590: 2870 7269 7661 7465 2907 0000 000b 4970  (private).....Ip
+000035a0: 6572 6e69 7479 5461 6201 03ff ffff ff08  ernityTab.......
+000035b0: 0000 0000 0600 0000 1a52 6570 6c61 6365  .........Replace
+000035c0: 2069 6d61 6765 2072 6567 696f 6e20 6e6f   image region no
+000035d0: 7465 7307 0000 000b 4970 6572 6e69 7479  tes.....Ipernity
+000035e0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+000035f0: 0000 1052 6570 6c61 6365 206d 6574 6164  ...Replace metad
+00003600: 6174 6107 0000 000b 4970 6572 6e69 7479  ata.....Ipernity
+00003610: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00003620: 0000 0b53 796e 6368 726f 6e69 7365 0700  ...Synchronise..
+00003630: 0000 0b49 7065 726e 6974 7954 6162 0103  ...IpernityTab..
+00003640: ffff ffff 0800 0000 0006 0000 0005 5469  ..............Ti
+00003650: 746c 6507 0000 000b 4970 6572 6e69 7479  tle.....Ipernity
+00003660: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00003670: 0000 1857 686f 2063 616e 2063 6f6d 6d65  ...Who can comme
+00003680: 6e74 206f 6e20 616c 6275 6d07 0000 000b  nt on album.....
+00003690: 4970 6572 6e69 7479 5461 6201 03ff ffff  IpernityTab.....
+000036a0: ff08 0000 0000 0600 0000 0857 686f 2063  ...........Who c
+000036b0: 616e 3a07 0000 000b 4970 6572 6e69 7479  an:.....Ipernity
+000036c0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+000036d0: 0000 1361 6464 206b 6579 776f 7264 732c  ...add keywords,
+000036e0: 206e 6f74 6573 0700 0000 0b49 7065 726e   notes.....Ipern
+000036f0: 6974 7954 6162 0103 ffff ffff 0800 0000  ityTab..........
+00003700: 0006 0000 000f 6964 656e 7469 6679 2070  ......identify p
+00003710: 656f 706c 6507 0000 000b 4970 6572 6e69  eople.....Iperni
+00003720: 7479 5461 6201 03ff ffff ff08 0000 0000  tyTab...........
+00003730: 0600 0000 0e70 6f73 7420 6120 636f 6d6d  .....post a comm
+00003740: 656e 7407 0000 000b 4970 6572 6e69 7479  ent.....Ipernity
+00003750: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00003760: 0000 0d73 6565 2074 6865 2070 686f 746f  ...see the photo
+00003770: 0700 0000 0b49 7065 726e 6974 7954 6162  .....IpernityTab
+00003780: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
+00003790: 4c61 6e67 3a20 0700 0000 0d4c 616e 6741  Lang: .....LangA
+000037a0: 6c74 5769 6467 6574 0103 ffff ffff 0800  ltWidget........
+000037b0: 0000 0006 0000 0008 4c61 6e67 7561 6765  ........Language
+000037c0: 0700 0000 0d4c 616e 6741 6c74 5769 6467  .....LangAltWidg
+000037d0: 6574 0103 ffff ffff 0800 0000 0006 0000  et..............
+000037e0: 000c 4e65 7720 6c61 6e67 7561 6765 0700  ..New language..
+000037f0: 0000 0d4c 616e 6741 6c74 5769 6467 6574  ...LangAltWidget
+00003800: 0103 ffff ffff 0800 0000 0006 0000 0014  ................
+00003810: 5365 7420 6465 6661 756c 7420 6c61 6e67  Set default lang
+00003820: 7561 6765 0700 0000 0d4c 616e 6741 6c74  uage.....LangAlt
+00003830: 5769 6467 6574 0103 ffff ffff 0800 0000  Widget..........
+00003840: 0006 0000 004b 5768 6174 206c 616e 6775  .....KWhat langu
+00003850: 6167 6520 6973 2074 6865 2063 7572 7265  age is the curre
+00003860: 6e74 2074 6578 7420 696e 3f20 506c 6561  nt text in? Plea
+00003870: 7365 2065 6e74 6572 2061 6e20 5246 4333  se enter an RFC3
+00003880: 3036 3620 6c61 6e67 7561 6765 2074 6167  066 language tag
+00003890: 2e07 0000 000d 4c61 6e67 416c 7457 6964  ......LangAltWid
+000038a0: 6765 7401 03ff ffff ff08 0000 0000 0600  get.............
+000038b0: 0000 4a57 6861 7420 6c61 6e67 7561 6765  ..JWhat language
+000038c0: 2077 6f75 6c64 2079 6f75 206c 696b 6520   would you like 
+000038d0: 746f 2061 6464 3f20 506c 6561 7365 2065  to add? Please e
+000038e0: 6e74 6572 2061 6e20 5246 4333 3036 3620  nter an RFC3066 
+000038f0: 6c61 6e67 7561 6765 2074 6167 2e07 0000  language tag....
+00003900: 000d 4c61 6e67 416c 7457 6964 6765 7401  ..LangAltWidget.
+00003910: 03ff ffff ff08 0000 0000 0600 0000 094c  ...............L
+00003920: 6174 2c20 6c6f 6e67 0700 0000 0e4c 6174  at, long.....Lat
+00003930: 4c6f 6e67 4469 7370 6c61 7901 03ff ffff  LongDisplay.....
+00003940: ff08 0000 0000 0600 0000 504c 6174 6974  ..........PLatit
+00003950: 7564 6520 616e 6420 6c6f 6e67 6974 7564  ude and longitud
+00003960: 6520 2869 6e20 6465 6772 6565 7329 2061  e (in degrees) a
+00003970: 7320 7477 6f20 6465 6369 6d61 6c20 6e75  s two decimal nu
+00003980: 6d62 6572 7320 7365 7061 7261 7465 6420  mbers separated 
+00003990: 6279 2061 2073 7061 6365 2e07 0000 000e  by a space......
+000039a0: 4c61 744c 6f6e 6744 6973 706c 6179 0103  LatLongDisplay..
+000039b0: ffff ffff 0800 0000 0006 0000 0015 5068  ..............Ph
+000039c0: 6f74 696e 6920 6572 726f 7220 6c6f 6767  otini error logg
+000039d0: 696e 6707 0000 000c 4c6f 6767 6572 5769  ing.....LoggerWi
+000039e0: 6e64 6f77 0103 ffff ffff 0800 0000 0006  ndow............
+000039f0: 0000 000d 5361 7665 206c 6f67 2066 696c  ....Save log fil
+00003a00: 6507 0000 000c 4c6f 6767 6572 5769 6e64  e.....LoggerWind
+00003a10: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
+00003a20: 000b 4d61 7020 2826 4269 6e67 2907 0000  ..Map (&Bing)...
+00003a30: 000a 4d61 7054 6162 4269 6e67 0103 ffff  ..MapTabBing....
+00003a40: ffff 0800 0000 0006 0000 002b 5365 6172  ...........+Sear
+00003a50: 6368 2061 6e64 2061 6c74 6974 7564 6520  ch and altitude 
+00003a60: 6c6f 6f6b 7570 2070 726f 7669 6465 6420  lookup provided 
+00003a70: 6279 2042 696e 6707 0000 000a 4d61 7054  by Bing.....MapT
+00003a80: 6162 4269 6e67 0103 ffff ffff 0800 0000  abBing..........
+00003a90: 0006 0000 0021 5365 7276 6572 206f 7665  .....!Server ove
+00003aa0: 726c 6f61 642c 2070 6c65 6173 6520 7472  rload, please tr
+00003ab0: 7920 6167 6169 6e07 0000 000a 4d61 7054  y again.....MapT
+00003ac0: 6162 4269 6e67 0103 ffff ffff 0800 0000  abBing..........
+00003ad0: 0006 0000 000d 4d61 7020 2826 476f 6f67  ......Map (&Goog
+00003ae0: 6c65 2907 0000 000c 4d61 7054 6162 476f  le).....MapTabGo
+00003af0: 6f67 6c65 0103 ffff ffff 0800 0000 0006  ogle............
+00003b00: 0000 002c 5365 6172 6368 2061 6e64 2061  ...,Search and a
+00003b10: 6c74 6974 7564 6520 6c6f 6f6b 7570 2070  ltitude lookup p
+00003b20: 6f77 6572 6564 2062 7920 476f 6f67 6c65  owered by Google
+00003b30: 0700 0000 0c4d 6170 5461 6247 6f6f 676c  .....MapTabGoogl
+00003b40: 6501 03ff ffff ff08 0000 0000 0600 0000  e...............
+00003b50: 0d4d 6170 2028 264d 6170 626f 7829 0700  .Map (&Mapbox)..
+00003b60: 0000 0c4d 6170 5461 624d 6170 626f 7801  ...MapTabMapbox.
+00003b70: 03ff ffff ff08 0000 0000 0600 0000 1853  ...............S
+00003b80: 6561 7263 6820 706f 7765 7265 6420 6279  earch powered by
+00003b90: 204d 6170 626f 7807 0000 000c 4d61 7054   Mapbox.....MapT
+00003ba0: 6162 4d61 7062 6f78 0103 ffff ffff 0800  abMapbox........
+00003bb0: 0000 0006 0000 000d 4162 6f75 7420 5068  ........About Ph
+00003bc0: 6f74 696e 6907 0000 0007 4d65 6e75 4261  otini.....MenuBa
+00003bd0: 7201 03ff ffff ff08 0000 0000 0600 0000  r...............
+00003be0: 5141 6e20 6561 7379 2074 6f20 7573 6520  QAn easy to use 
+00003bf0: 6469 6769 7461 6c20 7068 6f74 6f67 7261  digital photogra
+00003c00: 7068 206d 6574 6164 6174 6120 2845 7869  ph metadata (Exi
+00003c10: 662c 2049 5054 432c 2058 4d50 2920 6564  f, IPTC, XMP) ed
+00003c20: 6974 696e 6720 6170 706c 6963 6174 696f  iting applicatio
+00003c30: 6e2e 0700 0000 074d 656e 7542 6172 0103  n......MenuBar..
+00003c40: ffff ffff 0800 0000 0006 0000 0010 4368  ..............Ch
+00003c50: 6563 6b20 666f 7220 7570 6461 7465 0700  eck for update..
+00003c60: 0000 074d 656e 7542 6172 0103 ffff ffff  ...MenuBar......
+00003c70: 0800 0000 0006 0000 000f 436c 6f73 6520  ..........Close 
+00003c80: 616c 6c20 6669 6c65 7307 0000 0007 4d65  all files.....Me
 00003c90: 6e75 4261 7201 03ff ffff ff08 0000 0000  nuBar...........
-00003ca0: 0600 0000 294f 7065 6e20 736f 7572 6365  ....)Open source
-00003cb0: 2070 6163 6b61 6765 2061 7661 696c 6162   package availab
-00003cc0: 6c65 2066 726f 6d20 7b75 726c 7d2e 0700  le from {url}...
-00003cd0: 0000 074d 656e 7542 6172 0103 ffff ffff  ...MenuBar......
-00003ce0: 0800 0000 0006 0000 0007 4f70 7469 6f6e  ..........Option
-00003cf0: 7307 0000 0007 4d65 6e75 4261 7201 03ff  s.....MenuBar...
-00003d00: ffff ff08 0000 0000 0600 0000 1550 686f  .............Pho
-00003d10: 7469 6e69 2064 6f63 756d 656e 7461 7469  tini documentati
-00003d20: 6f6e 0700 0000 074d 656e 7542 6172 0103  on.....MenuBar..
-00003d30: ffff ffff 0800 0000 0006 0000 001d 5068  ..............Ph
-00003d40: 6f74 696e 6920 7068 6f74 6f20 6d65 7461  otini photo meta
-00003d50: 6461 7461 2065 6469 746f 7207 0000 0007  data editor.....
-00003d60: 4d65 6e75 4261 7201 03ff ffff ff08 0000  MenuBar.........
-00003d70: 0000 0600 0000 0e50 686f 7469 6e69 3a20  .......Photini: 
-00003d80: 6162 6f75 7407 0000 0007 4d65 6e75 4261  about.....MenuBa
-00003d90: 7201 03ff ffff ff08 0000 0000 0600 0000  r...............
-00003da0: 1650 686f 7469 6e69 3a20 7665 7273 696f  .Photini: versio
-00003db0: 6e20 6368 6563 6b07 0000 0007 4d65 6e75  n check.....Menu
+00003ca0: 0600 0000 1245 6e61 626c 6520 7370 656c  .....Enable spel
+00003cb0: 6c20 6368 6563 6b07 0000 0007 4d65 6e75  l check.....Menu
+00003cc0: 4261 7201 03ff ffff ff08 0000 0000 0600  Bar.............
+00003cd0: 0000 0446 696c 6507 0000 0007 4d65 6e75  ...File.....Menu
+00003ce0: 4261 7201 03ff ffff ff08 0000 0000 0600  Bar.............
+00003cf0: 0000 1646 6978 206d 6973 7369 6e67 2074  ...Fix missing t
+00003d00: 6875 6d62 6e61 696c 7307 0000 0007 4d65  humbnails.....Me
+00003d10: 6e75 4261 7201 03ff ffff ff08 0000 0000  nuBar...........
+00003d20: 0600 0000 0448 656c 7007 0000 0007 4d65  .....Help.....Me
+00003d30: 6e75 4261 7201 03ff ffff ff08 0000 0000  nuBar...........
+00003d40: 0600 0000 0a4f 7065 6e20 6669 6c65 7307  .....Open files.
+00003d50: 0000 0007 4d65 6e75 4261 7201 03ff ffff  ....MenuBar.....
+00003d60: ff08 0000 0000 0600 0000 294f 7065 6e20  ..........)Open 
+00003d70: 736f 7572 6365 2070 6163 6b61 6765 2061  source package a
+00003d80: 7661 696c 6162 6c65 2066 726f 6d20 7b75  vailable from {u
+00003d90: 726c 7d2e 0700 0000 074d 656e 7542 6172  rl}......MenuBar
+00003da0: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
+00003db0: 4f70 7469 6f6e 7307 0000 0007 4d65 6e75  Options.....Menu
 00003dc0: 4261 7201 03ff ffff ff08 0000 0000 0600  Bar.............
-00003dd0: 0000 0451 7569 7407 0000 0007 4d65 6e75  ...Quit.....Menu
-00003de0: 4261 7201 03ff ffff ff08 0000 0000 0600  Bar.............
-00003df0: 0000 0c53 6176 6520 6368 616e 6765 7307  ...Save changes.
-00003e00: 0000 0007 4d65 6e75 4261 7201 03ff ffff  ....MenuBar.....
-00003e10: ff08 0000 0000 0600 0000 0f53 656c 6563  ...........Selec
-00003e20: 7465 6420 696d 6167 6573 0700 0000 074d  ted images.....M
-00003e30: 656e 7542 6172 0103 ffff ffff 0800 0000  enuBar..........
-00003e40: 0006 0000 0008 5365 7474 696e 6773 0700  ......Settings..
-00003e50: 0000 074d 656e 7542 6172 0103 ffff ffff  ...MenuBar......
-00003e60: 0800 0000 0006 0000 0008 5370 656c 6c69  ..........Spelli
-00003e70: 6e67 0700 0000 074d 656e 7542 6172 0103  ng.....MenuBar..
-00003e80: ffff ffff 0800 0000 0006 0000 0065 5468  .............eTh
-00003e90: 6973 2070 726f 6772 616d 2069 7320 7265  is program is re
-00003ea0: 6c65 6173 6564 2077 6974 6820 6120 474e  leased with a GN
-00003eb0: 5520 4765 6e65 7261 6c20 5075 626c 6963  U General Public
-00003ec0: 204c 6963 656e 7365 2e20 466f 7220 6465   License. For de
-00003ed0: 7461 696c 7320 636c 6963 6b20 7468 6520  tails click the 
-00003ee0: 227b 6465 7461 696c 737d 2220 6275 7474  "{details}" butt
-00003ef0: 6f6e 2e07 0000 0007 4d65 6e75 4261 7201  on......MenuBar.
-00003f00: 03ff ffff ff08 0000 0000 0600 0000 5559  ..............UY
-00003f10: 6f75 2061 7265 2063 7572 7265 6e74 6c79  ou are currently
-00003f20: 2072 756e 6e69 6e67 2050 686f 7469 6e69   running Photini
-00003f30: 2076 6572 7369 6f6e 207b 7665 7273 696f   version {versio
-00003f40: 6e7d 2e20 5468 6520 6c61 7465 7374 2072  n}. The latest r
-00003f50: 656c 6561 7365 2069 7320 7b72 656c 6561  elease is {relea
-00003f60: 7365 7d2e 0700 0000 074d 656e 7542 6172  se}......MenuBar
-00003f70: 0103 ffff ffff 0800 0000 0006 0000 0013  ................
-00003f80: 264f 776e 6572 7368 6970 206d 6574 6164  &Ownership metad
-00003f90: 6174 6107 0000 0008 4f77 6e65 7254 6162  ata.....OwnerTab
-00003fa0: 0103 ffff ffff 0800 0000 0006 0000 0013  ................
-00003fb0: 416c 6c20 7269 6768 7473 2072 6573 6572  All rights reser
-00003fc0: 7665 6407 0000 0008 4f77 6e65 7254 6162  ved.....OwnerTab
-00003fd0: 0103 ffff ffff 0800 0000 0006 0000 000e  ................
-00003fe0: 4170 706c 7920 7465 6d70 6c61 7465 0700  Apply template..
-00003ff0: 0000 084f 776e 6572 5461 6201 03ff ffff  ...OwnerTab.....
-00004000: ff08 0000 0000 0600 0000 1b41 7474 7269  ...........Attri
-00004010: 6275 7469 6f6e 2034 2e30 2028 4343 2042  bution 4.0 (CC B
-00004020: 5920 342e 3029 0700 0000 084f 776e 6572  Y 4.0).....Owner
-00004030: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00004040: 0000 2c41 7474 7269 6275 7469 6f6e 2d4e  ..,Attribution-N
-00004050: 6f44 6572 6976 6174 6976 6573 2034 2e30  oDerivatives 4.0
-00004060: 2028 4343 2042 592d 4e44 2034 2e30 2907   (CC BY-ND 4.0).
-00004070: 0000 0008 4f77 6e65 7254 6162 0103 ffff  ....OwnerTab....
-00004080: ffff 0800 0000 0006 0000 002c 4174 7472  ...........,Attr
-00004090: 6962 7574 696f 6e2d 4e6f 6e43 6f6d 6d65  ibution-NonComme
-000040a0: 7263 6961 6c20 342e 3020 2843 4320 4259  rcial 4.0 (CC BY
-000040b0: 2d4e 4320 342e 3029 0700 0000 084f 776e  -NC 4.0).....Own
-000040c0: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
-000040d0: 0600 0000 3d41 7474 7269 6275 7469 6f6e  ....=Attribution
-000040e0: 2d4e 6f6e 436f 6d6d 6572 6369 616c 2d4e  -NonCommercial-N
-000040f0: 6f44 6572 6976 6174 6976 6573 2034 2e30  oDerivatives 4.0
-00004100: 2028 4343 2042 592d 4e43 2d4e 4420 342e   (CC BY-NC-ND 4.
-00004110: 3029 0700 0000 084f 776e 6572 5461 6201  0).....OwnerTab.
-00004120: 03ff ffff ff08 0000 0000 0600 0000 3a41  ..............:A
-00004130: 7474 7269 6275 7469 6f6e 2d4e 6f6e 436f  ttribution-NonCo
-00004140: 6d6d 6572 6369 616c 2d53 6861 7265 416c  mmercial-ShareAl
-00004150: 696b 6520 342e 3020 2843 4320 4259 2d4e  ike 4.0 (CC BY-N
-00004160: 432d 5341 2034 2e30 2907 0000 0008 4f77  C-SA 4.0).....Ow
-00004170: 6e65 7254 6162 0103 ffff ffff 0800 0000  nerTab..........
-00004180: 0006 0000 0029 4174 7472 6962 7574 696f  .....)Attributio
-00004190: 6e2d 5368 6172 6541 6c69 6b65 2034 2e30  n-ShareAlike 4.0
-000041a0: 2028 4343 2042 592d 5341 2034 2e30 2907   (CC BY-SA 4.0).
-000041b0: 0000 0008 4f77 6e65 7254 6162 0103 ffff  ....OwnerTab....
-000041c0: ffff 0800 0000 0006 0000 0034 4343 3020  ...........4CC0 
-000041d0: 312e 3020 556e 6976 6572 7361 6c20 2843  1.0 Universal (C
-000041e0: 4330 2031 2e30 2920 5075 626c 6963 2044  C0 1.0) Public D
-000041f0: 6f6d 6169 6e20 4465 6469 6361 7469 6f6e  omain Dedication
-00004200: 0700 0000 084f 776e 6572 5461 6201 03ff  .....OwnerTab...
-00004210: ffff ff08 0000 0000 0600 0000 0443 6974  .............Cit
-00004220: 7907 0000 0008 4f77 6e65 7254 6162 0103  y.....OwnerTab..
-00004230: ffff ffff 0800 0000 0006 0000 0010 436f  ..............Co
-00004240: 7079 7269 6768 7420 4e6f 7469 6365 0700  pyright Notice..
-00004250: 0000 084f 776e 6572 5461 6201 03ff ffff  ...OwnerTab.....
-00004260: ff08 0000 0000 0600 0000 0743 6f75 6e74  ...........Count
-00004270: 7279 0700 0000 084f 776e 6572 5461 6201  ry.....OwnerTab.
-00004280: 03ff ffff ff08 0000 0000 0600 0000 0743  ...............C
-00004290: 7265 6174 6f72 0700 0000 084f 776e 6572  reator.....Owner
-000042a0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-000042b0: 0000 2643 7265 6174 6f72 202f 204c 6963  ..&Creator / Lic
-000042c0: 656e 736f 7220 436f 6e74 6163 7420 496e  ensor Contact In
-000042d0: 666f 726d 6174 696f 6e07 0000 0008 4f77  formation.....Ow
-000042e0: 6e65 7254 6162 0103 ffff ffff 0800 0000  nerTab..........
-000042f0: 0006 0000 0012 4372 6561 746f 7227 7320  ......Creator's 
-00004300: 4a6f 6274 6974 6c65 0700 0000 084f 776e  Jobtitle.....Own
-00004310: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
-00004320: 0600 0000 0b43 7265 6469 7420 4c69 6e65  .....Credit Line
-00004330: 0700 0000 084f 776e 6572 5461 6201 03ff  .....OwnerTab...
-00004340: ffff ff08 0000 0000 0600 0000 1244 6566  .............Def
-00004350: 696e 6520 6e65 7720 6c69 6365 6e63 6507  ine new licence.
-00004360: 0000 0008 4f77 6e65 7254 6162 0103 ffff  ....OwnerTab....
-00004370: ffff 0800 0000 0006 0000 000e 4465 7461  ............Deta
-00004380: 696c 2041 6464 7265 7373 0700 0000 084f  il Address.....O
-00004390: 776e 6572 5461 6201 03ff ffff ff08 0000  wnerTab.........
-000043a0: 0000 0600 0000 0d45 6469 7420 7465 6d70  .......Edit temp
-000043b0: 6c61 7465 0700 0000 084f 776e 6572 5461  late.....OwnerTa
-000043c0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-000043d0: 0845 6d61 696c 2873 2907 0000 0008 4f77  .Email(s).....Ow
-000043e0: 6e65 7254 6162 0103 ffff ffff 0800 0000  nerTab..........
-000043f0: 0006 0000 005f 456e 7465 7220 6120 6e6f  ....._Enter a no
-00004400: 7469 6365 206f 6e20 7468 6520 6375 7272  tice on the curr
-00004410: 656e 7420 6f77 6e65 7220 6f66 2074 6865  ent owner of the
-00004420: 2063 6f70 7972 6967 6874 2066 6f72 2074   copyright for t
-00004430: 6869 7320 696d 6167 652c 2073 7563 6820  his image, such 
-00004440: 6173 2022 c2a9 3230 3038 204a 616e 6520  as "..2008 Jane 
-00004450: 446f 6522 2e07 0000 0008 4f77 6e65 7254  Doe"......OwnerT
-00004460: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00004470: 005e 456e 7465 7220 6164 6472 6573 7320  .^Enter address 
-00004480: 6465 7461 696c 2028 652e 672e 2066 6c61  detail (e.g. fla
-00004490: 7420 6e75 6d62 6572 206f 7220 726f 6f6d  t number or room
-000044a0: 206e 756d 6265 7229 2066 6f72 2074 6865   number) for the
-000044b0: 2070 6572 736f 6e20 7468 6174 2063 7265   person that cre
-000044c0: 6174 6564 2074 6869 7320 696d 6167 652e  ated this image.
-000044d0: 0700 0000 084f 776e 6572 5461 6201 03ff  .....OwnerTab...
-000044e0: ffff ff08 0000 0000 0600 0000 6545 6e74  ............eEnt
-000044f0: 6572 2069 6e66 6f72 6d61 7469 6f6e 2061  er information a
-00004500: 626f 7574 2065 6d62 6172 676f 6573 2c20  bout embargoes, 
-00004510: 6f72 206f 7468 6572 2072 6573 7472 6963  or other restric
-00004520: 7469 6f6e 7320 6e6f 7420 636f 7665 7265  tions not covere
-00004530: 6420 6279 2074 6865 2052 6967 6874 7320  d by the Rights 
-00004540: 5573 6167 6520 5465 726d 7320 6669 656c  Usage Terms fiel
-00004550: 642e 0700 0000 084f 776e 6572 5461 6201  d......OwnerTab.
-00004560: 03ff ffff ff08 0000 0000 0600 0000 3945  ..............9E
-00004570: 6e74 6572 2069 6e73 7472 7563 7469 6f6e  nter instruction
-00004580: 7320 6f6e 2068 6f77 2074 6869 7320 696d  s on how this im
-00004590: 6167 6520 6361 6e20 6c65 6761 6c6c 7920  age can legally 
-000045a0: 6265 2075 7365 642e 0700 0000 084f 776e  be used......Own
-000045b0: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
-000045c0: 0600 0000 3c45 6e74 6572 2073 7472 6565  ....<Enter stree
-000045d0: 7420 6164 6472 6573 7320 666f 7220 7468  t address for th
-000045e0: 6520 7065 7273 6f6e 2074 6861 7420 6372  e person that cr
-000045f0: 6561 7465 6420 7468 6973 2069 6d61 6765  eated this image
-00004600: 2e07 0000 0008 4f77 6e65 7254 6162 0103  ......OwnerTab..
-00004610: ffff ffff 0800 0000 0006 0000 0045 456e  .............EEn
-00004620: 7465 7220 7468 6520 6369 7479 2066 6f72  ter the city for
-00004630: 2074 6865 2061 6464 7265 7373 206f 6620   the address of 
-00004640: 7468 6520 7065 7273 6f6e 2074 6861 7420  the person that 
-00004650: 6372 6561 7465 6420 7468 6973 2069 6d61  created this ima
-00004660: 6765 2e07 0000 0008 4f77 6e65 7254 6162  ge......OwnerTab
-00004670: 0103 ffff ffff 0800 0000 0006 0000 004d  ...............M
-00004680: 456e 7465 7220 7468 6520 636f 756e 7472  Enter the countr
-00004690: 7920 6e61 6d65 2066 6f72 2074 6865 2061  y name for the a
-000046a0: 6464 7265 7373 206f 6620 7468 6520 7065  ddress of the pe
-000046b0: 7273 6f6e 2074 6861 7420 6372 6561 7465  rson that create
-000046c0: 6420 7468 6973 2069 6d61 6765 2e07 0000  d this image....
-000046d0: 0008 4f77 6e65 7254 6162 0103 ffff ffff  ..OwnerTab......
-000046e0: 0800 0000 0006 0000 003e 456e 7465 7220  .........>Enter 
-000046f0: 7468 6520 6a6f 6220 7469 746c 6520 6f66  the job title of
-00004700: 2074 6865 2070 6572 736f 6e20 6c69 7374   the person list
-00004710: 6564 2069 6e20 7468 6520 4372 6561 746f  ed in the Creato
-00004720: 7220 6669 656c 642e 0700 0000 084f 776e  r field......Own
-00004730: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
-00004740: 0600 0000 3545 6e74 6572 2074 6865 206e  ....5Enter the n
-00004750: 616d 6520 6f66 2074 6865 2070 6572 736f  ame of the perso
-00004760: 6e20 7468 6174 2063 7265 6174 6564 2074  n that created t
-00004770: 6869 7320 696d 6167 652e 0700 0000 084f  his image......O
-00004780: 776e 6572 5461 6201 03ff ffff ff08 0000  wnerTab.........
-00004790: 0000 0600 0000 4c45 6e74 6572 2074 6865  ......LEnter the
-000047a0: 2070 6f73 7461 6c20 636f 6465 2066 6f72   postal code for
-000047b0: 2074 6865 2061 6464 7265 7373 206f 6620   the address of 
-000047c0: 7468 6520 7065 7273 6f6e 2074 6861 7420  the person that 
-000047d0: 6372 6561 7465 6420 7468 6973 2069 6d61  created this ima
-000047e0: 6765 2e07 0000 0008 4f77 6e65 7254 6162  ge......OwnerTab
-000047f0: 0103 ffff ffff 0800 0000 0006 0000 0046  ...............F
-00004800: 456e 7465 7220 7468 6520 7374 6174 6520  Enter the state 
-00004810: 666f 7220 7468 6520 6164 6472 6573 7320  for the address 
-00004820: 6f66 2074 6865 2070 6572 736f 6e20 7468  of the person th
-00004830: 6174 2063 7265 6174 6564 2074 6869 7320  at created this 
-00004840: 696d 6167 652e 0700 0000 084f 776e 6572  image......Owner
-00004850: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00004860: 0000 5e45 6e74 6572 2074 6865 2077 6f72  ..^Enter the wor
-00004870: 6b20 5765 6220 5552 4c20 666f 7220 7468  k Web URL for th
-00004880: 6520 7065 7273 6f6e 2074 6861 7420 6372  e person that cr
-00004890: 6561 7465 6420 7468 6973 2069 6d61 6765  eated this image
-000048a0: 2c20 7375 6368 2061 7320 6874 7470 3a2f  , such as http:/
-000048b0: 2f77 7777 2e64 6f6d 6169 6e2e 636f 6d2f  /www.domain.com/
-000048c0: 2e07 0000 0008 4f77 6e65 7254 6162 0103  ......OwnerTab..
-000048d0: ffff ffff 0800 0000 0006 0000 005d 456e  .............]En
-000048e0: 7465 7220 7468 6520 776f 726b 2065 6d61  ter the work ema
-000048f0: 696c 2061 6464 7265 7373 2066 6f72 2074  il address for t
-00004900: 6865 2070 6572 736f 6e20 7468 6174 2063  he person that c
-00004910: 7265 6174 6564 2074 6869 7320 696d 6167  reated this imag
-00004920: 652c 2073 7563 6820 6173 206e 616d 6540  e, such as name@
-00004930: 646f 6d61 696e 2e63 6f6d 2e07 0000 0008  domain.com......
-00004940: 4f77 6e65 7254 6162 0103 ffff ffff 0800  OwnerTab........
-00004950: 0000 0006 0000 007c 456e 7465 7220 7468  .......|Enter th
-00004960: 6520 776f 726b 2070 686f 6e65 206e 756d  e work phone num
-00004970: 6265 7220 666f 7220 7468 6520 7065 7273  ber for the pers
-00004980: 6f6e 2074 6861 7420 6372 6561 7465 6420  on that created 
-00004990: 7468 6973 2069 6d61 6765 2c20 7573 696e  this image, usin
-000049a0: 6720 7468 6520 696e 7465 726e 6174 696f  g the internatio
-000049b0: 6e61 6c20 666f 726d 6174 2c20 7375 6368  nal format, such
-000049c0: 2061 7320 2b31 2028 3132 3329 2034 3536   as +1 (123) 456
-000049d0: 3738 392e 0700 0000 084f 776e 6572 5461  789......OwnerTa
-000049e0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-000049f0: 3a45 6e74 6572 2077 686f 2073 686f 756c  :Enter who shoul
-00004a00: 6420 6265 2063 7265 6469 7465 6420 7768  d be credited wh
-00004a10: 656e 2074 6869 7320 696d 6167 6520 6973  en this image is
-00004a20: 2070 7562 6c69 7368 6564 2e07 0000 0008   published......
-00004a30: 4f77 6e65 7254 6162 0103 ffff ffff 0800  OwnerTab........
-00004a40: 0000 0006 0000 0013 496e 6974 6961 6c69  ........Initiali
-00004a50: 7365 2074 656d 706c 6174 6507 0000 0008  se template.....
-00004a60: 4f77 6e65 7254 6162 0103 ffff ffff 0800  OwnerTab........
-00004a70: 0000 0006 0000 000c 496e 7374 7275 6374  ........Instruct
-00004a80: 696f 6e73 0700 0000 084f 776e 6572 5461  ions.....OwnerTa
-00004a90: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00004aa0: 044e 616d 6507 0000 0008 4f77 6e65 7254  .Name.....OwnerT
-00004ab0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00004ac0: 0018 4f70 656e 206c 696e 6b20 746f 2022  ..Open link to "
-00004ad0: 7b6c 6963 656e 6365 7d22 0700 0000 084f  {licence}".....O
-00004ae0: 776e 6572 5461 6201 03ff ffff ff08 0000  wnerTab.........
-00004af0: 0000 0600 0000 0850 686f 6e65 2873 2907  .......Phone(s).
-00004b00: 0000 0008 4f77 6e65 7254 6162 0103 ffff  ....OwnerTab....
-00004b10: ffff 0800 0000 0006 0000 001b 5068 6f74  ............Phot
-00004b20: 696e 693a 206f 776e 6572 7368 6970 2074  ini: ownership t
-00004b30: 656d 706c 6174 6507 0000 0008 4f77 6e65  emplate.....Owne
-00004b40: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
-00004b50: 0000 000b 506f 7374 616c 2043 6f64 6507  ....Postal Code.
-00004b60: 0000 0008 4f77 6e65 7254 6162 0103 ffff  ....OwnerTab....
-00004b70: ffff 0800 0000 0006 0000 0016 5075 626c  ............Publ
-00004b80: 6963 2044 6f6d 6169 6e20 4d61 726b 2031  ic Domain Mark 1
-00004b90: 2e30 0700 0000 084f 776e 6572 5461 6201  .0.....OwnerTab.
-00004ba0: 03ff ffff ff08 0000 0000 0600 0000 0652  ...............R
-00004bb0: 6967 6874 7307 0000 0008 4f77 6e65 7254  ights.....OwnerT
-00004bc0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00004bd0: 000e 5374 6174 652f 5072 6f76 696e 6365  ..State/Province
-00004be0: 0700 0000 084f 776e 6572 5461 6201 03ff  .....OwnerTab...
-00004bf0: ffff ff08 0000 0000 0600 0000 0e53 7472  .............Str
-00004c00: 6565 7420 4164 6472 6573 7307 0000 0008  eet Address.....
-00004c10: 4f77 6e65 7254 6162 0103 ffff ffff 0800  OwnerTab........
-00004c20: 0000 0006 0000 0003 5552 4c07 0000 0008  ........URL.....
-00004c30: 4f77 6e65 7254 6162 0103 ffff ffff 0800  OwnerTab........
-00004c40: 0000 0006 0000 000b 5573 6167 6520 5465  ........Usage Te
-00004c50: 726d 7307 0000 0008 4f77 6e65 7254 6162  rms.....OwnerTab
-00004c60: 0103 ffff ffff 0800 0000 0006 0000 0033  ...............3
-00004c70: 5573 6520 2559 2074 6f20 696e 7365 7274  Use %Y to insert
-00004c80: 2074 6865 2079 6561 7220 7468 6520 7068   the year the ph
-00004c90: 6f74 6f67 7261 7068 2077 6173 2074 616b  otograph was tak
-00004ca0: 656e 2e07 0000 0008 4f77 6e65 7254 6162  en......OwnerTab
-00004cb0: 0103 ffff ffff 0800 0000 0006 0000 000d  ................
-00004cc0: 5765 6220 5374 6174 656d 656e 7407 0000  Web Statement...
-00004cd0: 0008 4f77 6e65 7254 6162 0103 ffff ffff  ..OwnerTab......
-00004ce0: 0800 0000 0006 0000 000a 5765 6220 5552  ..........Web UR
-00004cf0: 4c28 7329 0700 0000 084f 776e 6572 5461  L(s).....OwnerTa
-00004d00: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00004d10: 0c3c 6e65 7720 7365 6172 6368 3e07 0000  .<new search>...
-00004d20: 000a 5068 6f74 696e 694d 6170 0103 ffff  ..PhotiniMap....
-00004d30: ffff 0800 0000 0006 0000 000f 3c72 6570  ............<rep
-00004d40: 6561 7420 7365 6172 6368 3e07 0000 000a  eat search>.....
-00004d50: 5068 6f74 696e 694d 6170 0103 ffff ffff  PhotiniMap......
-00004d60: 0800 0000 0006 0000 000e 3c77 6964 656e  ..........<widen
-00004d70: 2073 6561 7263 683e 0700 0000 0a50 686f   search>.....Pho
-00004d80: 7469 6e69 4d61 7001 03ff ffff ff08 0000  tiniMap.........
-00004d90: 0000 0600 0000 0841 6c74 6974 7564 6507  .......Altitude.
-00004da0: 0000 000a 5068 6f74 696e 694d 6170 0103  ....PhotiniMap..
-00004db0: ffff ffff 0800 0000 0006 0000 0015 4765  ..............Ge
-00004dc0: 7420 616c 7469 7475 6465 2066 726f 6d20  t altitude from 
-00004dd0: 6d61 7007 0000 000a 5068 6f74 696e 694d  map.....PhotiniM
-00004de0: 6170 0103 ffff ffff 0800 0000 0006 0000  ap..............
-00004df0: 000d 4c6f 6164 2047 5058 2066 696c 6507  ..Load GPX file.
-00004e00: 0000 000a 5068 6f74 696e 694d 6170 0103  ....PhotiniMap..
-00004e10: ffff ffff 0800 0000 0006 0000 000f 5265  ..............Re
-00004e20: 6d6f 7665 2047 5058 2064 6174 6107 0000  move GPX data...
-00004e30: 000a 5068 6f74 696e 694d 6170 0103 ffff  ..PhotiniMap....
-00004e40: ffff 0800 0000 0006 0000 0006 5365 6172  ............Sear
-00004e50: 6368 0700 0000 0a50 686f 7469 6e69 4d61  ch.....PhotiniMa
-00004e60: 7001 03ff ffff ff08 0000 0000 0600 0000  p...............
-00004e70: 1353 6574 2063 6f6f 7264 7320 6672 6f6d  .Set coords from
-00004e80: 2047 5058 0700 0000 0a50 686f 7469 6e69   GPX.....Photini
-00004e90: 4d61 7001 03ff ffff ff08 0000 0000 0600  Map.............
-00004ea0: 0000 1026 5069 7865 6c66 6564 2075 706c  ...&Pixelfed upl
-00004eb0: 6f61 6407 0000 000b 5069 7865 6c66 6564  oad.....Pixelfed
-00004ec0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00004ed0: 0000 1241 6464 2074 6f20 636f 6c6c 6563  ...Add to collec
-00004ee0: 7469 6f6e 7307 0000 000b 5069 7865 6c66  tions.....Pixelf
-00004ef0: 6564 5461 6201 03ff ffff ff08 0000 0000  edTab...........
-00004f00: 0600 0000 1341 6c6c 2052 6967 6874 7320  .....All Rights 
-00004f10: 5265 7365 7276 6564 0700 0000 0b50 6978  Reserved.....Pix
-00004f20: 656c 6665 6454 6162 0103 ffff ffff 0800  elfedTab........
-00004f30: 0000 0006 0000 000b 4174 7472 6962 7574  ........Attribut
-00004f40: 696f 6e07 0000 000b 5069 7865 6c66 6564  ion.....Pixelfed
-00004f50: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00004f60: 0000 1441 7474 7269 6275 7469 6f6e 2d4e  ...Attribution-N
-00004f70: 6f44 6572 6976 7307 0000 000b 5069 7865  oDerivs.....Pixe
-00004f80: 6c66 6564 5461 6201 03ff ffff ff08 0000  lfedTab.........
-00004f90: 0000 0600 0000 1941 7474 7269 6275 7469  .......Attributi
-00004fa0: 6f6e 2d4e 6f6e 436f 6d6d 6572 6369 616c  on-NonCommercial
-00004fb0: 0700 0000 0b50 6978 656c 6665 6454 6162  .....PixelfedTab
-00004fc0: 0103 ffff ffff 0800 0000 0006 0000 0022  ..............."
-00004fd0: 4174 7472 6962 7574 696f 6e2d 4e6f 6e43  Attribution-NonC
-00004fe0: 6f6d 6d65 7263 6961 6c2d 4e6f 4465 7269  ommercial-NoDeri
-00004ff0: 7673 0700 0000 0b50 6978 656c 6665 6454  vs.....PixelfedT
-00005000: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00005010: 0024 4174 7472 6962 7574 696f 6e2d 4e6f  .$Attribution-No
-00005020: 6e43 6f6d 6d65 7263 6961 6c2d 5368 6172  nCommercial-Shar
-00005030: 6541 6c69 6b65 0700 0000 0b50 6978 656c  eAlike.....Pixel
-00005040: 6665 6454 6162 0103 ffff ffff 0800 0000  fedTab..........
-00005050: 0006 0000 0016 4174 7472 6962 7574 696f  ......Attributio
-00005060: 6e2d 5368 6172 6541 6c69 6b65 0700 0000  n-ShareAlike....
-00005070: 0b50 6978 656c 6665 6454 6162 0103 ffff  .PixelfedTab....
-00005080: ffff 0800 0000 0006 0000 0007 4361 7074  ............Capt
-00005090: 696f 6e07 0000 000b 5069 7865 6c66 6564  ion.....Pixelfed
-000050a0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-000050b0: 0000 1243 686f 6f73 6520 616e 2069 6e73  ...Choose an ins
-000050c0: 7461 6e63 6507 0000 000b 5069 7865 6c66  tance.....Pixelf
-000050d0: 6564 5461 6201 03ff ffff ff08 0000 0000  edTab...........
-000050e0: 0600 0000 1543 6f6c 6c65 6374 696f 6e20  .....Collection 
-000050f0: 7669 7369 6269 6c69 7479 0700 0000 0b50  visibility.....P
-00005100: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
-00005110: 0800 0000 0006 0000 0015 4372 6561 7465  ..........Create
-00005120: 206e 6577 2063 6f6c 6c65 6374 696f 6e07   new collection.
-00005130: 0000 000b 5069 7865 6c66 6564 5461 6201  ....PixelfedTab.
-00005140: 03ff ffff ff08 0000 0000 0600 0000 0b44  ...............D
-00005150: 6573 6372 6970 7469 6f6e 0700 0000 0b50  escription.....P
-00005160: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
-00005170: 0800 0000 0006 0000 0010 4469 7361 626c  ..........Disabl
-00005180: 6520 636f 6d6d 656e 7473 0700 0000 0b50  e comments.....P
-00005190: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
-000051a0: 0800 0000 0006 0000 0005 4472 6166 7407  ..........Draft.
-000051b0: 0000 000b 5069 7865 6c66 6564 5461 6201  ....PixelfedTab.
-000051c0: 03ff ffff ff08 0000 0000 0600 0000 6646  ..............fF
-000051d0: 696c 6520 227b 6669 6c65 5f6e 616d 657d  ile "{file_name}
-000051e0: 2220 646f 6573 206e 6f74 2068 6176 6520  " does not have 
-000051f0: 616e 7920 2261 6c74 2074 6578 7422 2066  any "alt text" f
-00005200: 6f72 2061 6363 6573 7369 6269 6c69 7479  or accessibility
-00005210: 2e20 576f 756c 6420 796f 7520 6c69 6b65  . Would you like
-00005220: 2074 6f20 7570 6c6f 6164 2069 7420 616e   to upload it an
-00005230: 7977 6179 3f07 0000 000b 5069 7865 6c66  yway?.....Pixelf
-00005240: 6564 5461 6201 03ff ffff ff08 0000 0000  edTab...........
-00005250: 0600 0000 0e46 6f6c 6c6f 7765 7273 206f  .....Followers o
-00005260: 6e6c 7907 0000 000b 5069 7865 6c66 6564  nly.....Pixelfed
-00005270: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00005280: 0000 0847 656e 6572 6174 6507 0000 000b  ...Generate.....
-00005290: 5069 7865 6c66 6564 5461 6201 03ff ffff  PixelfedTab.....
-000052a0: ff08 0000 0000 0600 0000 074c 6963 656e  ...........Licen
-000052b0: 6365 0700 0000 0b50 6978 656c 6665 6454  ce.....PixelfedT
-000052c0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-000052d0: 0011 4d69 7373 696e 6720 616c 7420 7465  ..Missing alt te
-000052e0: 7874 2e07 0000 000b 5069 7865 6c66 6564  xt......Pixelfed
-000052f0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00005300: 0000 0e4e 6577 2063 6f6c 6c65 6374 696f  ...New collectio
-00005310: 6e07 0000 000b 5069 7865 6c66 6564 5461  n.....PixelfedTa
-00005320: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00005330: 054f 7468 6572 0700 0000 0b50 6978 656c  .Other.....Pixel
-00005340: 6665 6454 6162 0103 ffff ffff 0800 0000  fedTab..........
-00005350: 0006 0000 0011 5068 6f74 696e 693a 2061  ......Photini: a
-00005360: 6c74 2074 6578 7407 0000 000b 5069 7865  lt text.....Pixe
-00005370: 6c66 6564 5461 6201 03ff ffff ff08 0000  lfedTab.........
-00005380: 0000 0600 0000 1850 686f 7469 6e69 3a20  .......Photini: 
-00005390: 6368 6f6f 7365 2069 6e73 7461 6e63 6507  choose instance.
-000053a0: 0000 000b 5069 7865 6c66 6564 5461 6201  ....PixelfedTab.
-000053b0: 03ff ffff ff08 0000 0000 0600 0000 0850  ...............P
-000053c0: 6978 656c 6665 6407 0000 000b 5069 7865  ixelfed.....Pixe
-000053d0: 6c66 6564 5461 6201 03ff ffff ff08 0000  lfedTab.........
-000053e0: 0000 0600 0000 0f50 6f73 7420 7669 7369  .......Post visi
-000053f0: 6269 6c69 7479 0700 0000 0b50 6978 656c  bility.....Pixel
-00005400: 6665 6454 6162 0103 ffff ffff 0800 0000  fedTab..........
-00005410: 0006 0000 0006 5075 626c 6963 0700 0000  ......Public....
-00005420: 0b50 6978 656c 6665 6454 6162 0103 ffff  .PixelfedTab....
-00005430: ffff 0800 0000 0006 0000 001e 5075 626c  ............Publ
-00005440: 6963 2044 6f6d 6169 6e20 4465 6469 6361  ic Domain Dedica
-00005450: 7469 6f6e 2028 4343 3029 0700 0000 0b50  tion (CC0).....P
-00005460: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
-00005470: 0800 0000 0006 0000 0012 5075 626c 6963  ..........Public
-00005480: 2044 6f6d 6169 6e20 576f 726b 0700 0000   Domain Work....
-00005490: 0b50 6978 656c 6665 6454 6162 0103 ffff  .PixelfedTab....
-000054a0: ffff 0800 0000 0006 0000 000e 5365 6e73  ............Sens
-000054b0: 6974 6976 6520 706f 7374 0700 0000 0b50  itive post.....P
-000054c0: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
-000054d0: 0800 0000 0006 0000 0007 5370 6f69 6c65  ..........Spoile
-000054e0: 7207 0000 000b 5069 7865 6c66 6564 5461  r.....PixelfedTa
-000054f0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00005500: 0554 6974 6c65 0700 0000 0b50 6978 656c  .Title.....Pixel
-00005510: 6665 6454 6162 0103 ffff ffff 0800 0000  fedTab..........
-00005520: 0006 0000 0008 556e 6c69 7374 6564 0700  ......Unlisted..
-00005530: 0000 0b50 6978 656c 6665 6454 6162 0103  ...PixelfedTab..
-00005540: ffff ffff 0800 0000 0006 0000 000d 5570  ..............Up
-00005550: 6461 7465 2072 656d 6f74 6507 0000 000b  date remote.....
-00005560: 5069 7865 6c66 6564 5461 6201 03ff ffff  PixelfedTab.....
-00005570: ff08 0000 0000 0600 0000 2b57 6869 6368  ..........+Which
-00005580: 2050 6978 656c 6665 6420 696e 7374 616e   Pixelfed instan
-00005590: 6365 2068 6f73 7473 2079 6f75 7220 6163  ce hosts your ac
-000055a0: 636f 756e 743f 0700 0000 0b50 6978 656c  count?.....Pixel
-000055b0: 6665 6454 6162 0103 ffff ffff 0800 0000  fedTab..........
-000055c0: 0006 0000 0035 4120 7069 7865 6c20 6f66  .....5A pixel of
-000055d0: 2061 2064 6967 6974 616c 2069 6d61 6765   a digital image
-000055e0: 2073 6574 7469 6e67 2061 6e20 6162 736f   setting an abso
-000055f0: 6c75 7465 2076 616c 7565 2e07 0000 000a  lute value......
-00005600: 5265 6769 6f6e 7354 6162 0103 ffff ffff  RegionsTab......
-00005610: 0800 0000 0006 0000 000d 426f 756e 6461  ..........Bounda
-00005620: 7279 2075 6e69 7407 0000 000a 5265 6769  ry unit.....Regi
-00005630: 6f6e 7354 6162 0103 ffff ffff 0800 0000  onsTab..........
-00005640: 0006 0000 000c 436f 6e74 656e 7420 7479  ......Content ty
-00005650: 7065 0700 0000 0a52 6567 696f 6e73 5461  pe.....RegionsTa
-00005660: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00005670: 0d44 656c 6574 6520 7265 6769 6f6e 0700  .Delete region..
-00005680: 0000 0a52 6567 696f 6e73 5461 6201 03ff  ...RegionsTab...
-00005690: ffff ff08 0000 0000 0600 0000 0d44 656c  .............Del
-000056a0: 6574 6520 7665 7274 6578 0700 0000 0a52  ete vertex.....R
-000056b0: 6567 696f 6e73 5461 6201 03ff ffff ff08  egionsTab.......
-000056c0: 0000 0000 0600 0000 0b44 6573 6372 6970  .........Descrip
-000056d0: 7469 6f6e 0700 0000 0a52 6567 696f 6e73  tion.....Regions
-000056e0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-000056f0: 0000 5845 6e74 6572 2061 2022 6361 7074  ..XEnter a "capt
-00005700: 696f 6e22 2064 6573 6372 6962 696e 6720  ion" describing 
-00005710: 7468 6520 7768 6f2c 2077 6861 742c 2061  the who, what, a
-00005720: 6e64 2077 6879 206f 6620 7768 6174 2069  nd why of what i
-00005730: 7320 6861 7070 656e 696e 6720 696e 2074  s happening in t
-00005740: 6869 7320 7265 6769 6f6e 2e07 0000 000a  his region......
-00005750: 5265 6769 6f6e 7354 6162 0103 ffff ffff  RegionsTab......
-00005760: 0800 0000 0006 0000 005e 456e 7465 7220  .........^Enter 
-00005770: 7468 6520 6e61 6d65 7320 6f66 2070 656f  the names of peo
-00005780: 706c 6520 7368 6f77 6e20 696e 2074 6869  ple shown in thi
-00005790: 7320 7265 6769 6f6e 2e20 5365 7061 7261  s region. Separa
-000057a0: 7465 206d 756c 7469 706c 6520 656e 7472  te multiple entr
-000057b0: 6965 7320 7769 7468 2022 3b22 2063 6861  ies with ";" cha
-000057c0: 7261 6374 6572 732e 0700 0000 0a52 6567  racters......Reg
-000057d0: 696f 6e73 5461 6201 03ff ffff ff08 0000  ionsTab.........
-000057e0: 0000 0600 0000 5246 7265 652d 7465 7874  ......RFree-text
-000057f0: 206e 616d 6520 6f66 2074 6865 2072 6567   name of the reg
-00005800: 696f 6e2e 2053 686f 756c 6420 6265 2075  ion. Should be u
-00005810: 6e69 7175 6520 616d 6f6e 6720 616c 6c20  nique among all 
-00005820: 5265 6769 6f6e 204e 616d 6573 206f 6620  Region Names of 
-00005830: 616e 2069 6d61 6765 2e07 0000 000a 5265  an image......Re
-00005840: 6769 6f6e 7354 6162 0103 ffff ffff 0800  gionsTab........
-00005850: 0000 0006 0000 000a 4964 656e 7469 6669  ........Identifi
-00005860: 6572 0700 0000 0a52 6567 696f 6e73 5461  er.....RegionsTa
-00005870: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00005880: 9049 6465 6e74 6966 6965 7220 6f66 2074  .Identifier of t
-00005890: 6865 2072 6567 696f 6e2e 204d 7573 7420  he region. Must 
-000058a0: 6265 2075 6e69 7175 6520 616d 6f6e 6720  be unique among 
-000058b0: 616c 6c20 5265 6769 6f6e 2049 6465 6e74  all Region Ident
-000058c0: 6966 6965 7273 206f 6620 616e 2069 6d61  ifiers of an ima
-000058d0: 6765 2e20 446f 6573 206e 6f74 2068 6176  ge. Does not hav
-000058e0: 6520 746f 2062 6520 756e 6971 7565 2062  e to be unique b
-000058f0: 6579 6f6e 6420 7468 6520 6d65 7461 6461  eyond the metada
-00005900: 7461 206f 6620 7468 6973 2069 6d61 6765  ta of this image
-00005910: 2e07 0000 000a 5265 6769 6f6e 7354 6162  ......RegionsTab
-00005920: 0103 ffff ffff 0800 0000 0006 0000 000e  ................
-00005930: 496d 6167 6520 2652 6567 696f 6e73 0700  Image &Regions..
-00005940: 0000 0a52 6567 696f 6e73 5461 6201 03ff  ...RegionsTab...
-00005950: ffff ff08 0000 0000 0600 0000 044e 616d  .............Nam
-00005960: 6507 0000 000a 5265 6769 6f6e 7354 6162  e.....RegionsTab
-00005970: 0103 ffff ffff 0800 0000 0006 0000 000a  ................
-00005980: 4e65 7720 6369 7263 6c65 0700 0000 0a52  New circle.....R
-00005990: 6567 696f 6e73 5461 6201 03ff ffff ff08  egionsTab.......
-000059a0: 0000 0000 0600 0000 094e 6577 2070 6f69  .........New poi
-000059b0: 6e74 0700 0000 0a52 6567 696f 6e73 5461  nt.....RegionsTa
-000059c0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-000059d0: 0b4e 6577 2070 6f6c 7967 6f6e 0700 0000  .New polygon....
-000059e0: 0a52 6567 696f 6e73 5461 6201 03ff ffff  .RegionsTab.....
-000059f0: ff08 0000 0000 0600 0000 0d4e 6577 2072  ...........New r
-00005a00: 6563 7461 6e67 6c65 0700 0000 0a52 6567  ectangle.....Reg
-00005a10: 696f 6e73 5461 6201 03ff ffff ff08 0000  ionsTab.........
-00005a20: 0000 0600 0000 0a4e 6577 2076 6572 7465  .......New verte
-00005a30: 7807 0000 000a 5265 6769 6f6e 7354 6162  x.....RegionsTab
-00005a40: 0103 ffff ffff 0800 0000 0006 0000 000c  ................
-00005a50: 5065 7273 6f6e 2073 686f 776e 0700 0000  Person shown....
-00005a60: 0a52 6567 696f 6e73 5461 6201 03ff ffff  .RegionsTab.....
-00005a70: ff08 0000 0000 0600 0000 4152 656c 6174  ..........ARelat
-00005a80: 6976 6520 7061 7274 206f 6620 7468 6520  ive part of the 
-00005a90: 7369 7a65 206f 6620 616e 2069 6d61 6765  size of an image
-00005aa0: 2061 6c6f 6e67 2074 6865 2078 2d20 6f72   along the x- or
-00005ab0: 2074 6865 2079 2d61 7869 732e 0700 0000   the y-axis.....
-00005ac0: 0a52 6567 696f 6e73 5461 6201 03ff ffff  .RegionsTab.....
-00005ad0: ff08 0000 0000 0600 0000 0452 6f6c 6507  ...........Role.
-00005ae0: 0000 000a 5265 6769 6f6e 7354 6162 0103  ....RegionsTab..
-00005af0: ffff ffff 0800 0000 0006 0000 007f 526f  ..............Ro
-00005b00: 6c65 206f 6620 7468 6973 2072 6567 696f  le of this regio
-00005b10: 6e20 616d 6f6e 6720 616c 6c20 7265 6769  n among all regi
-00005b20: 6f6e 7320 6f66 2074 6869 7320 696d 6167  ons of this imag
-00005b30: 6520 6f72 206f 6620 6f74 6865 7220 696d  e or of other im
-00005b40: 6167 6573 2e20 5468 6520 7661 6c75 6520  ages. The value 
-00005b50: 5348 4f55 4c44 2062 6520 7461 6b65 6e20  SHOULD be taken 
-00005b60: 6672 6f6d 2061 2043 6f6e 7472 6f6c 6c65  from a Controlle
-00005b70: 6420 566f 6361 6275 6c61 7279 2e07 0000  d Vocabulary....
-00005b80: 000a 5265 6769 6f6e 7354 6162 0103 ffff  ..RegionsTab....
-00005b90: ffff 0800 0000 0006 0000 0064 5468 6520  ...........dThe 
-00005ba0: 496d 6167 6520 5265 6769 6f6e 2053 7472  Image Region Str
-00005bb0: 7563 7475 7265 2069 6e63 6c75 6465 7320  ucture includes 
-00005bc0: 6f70 7469 6f6e 616c 6c79 2061 6e79 206d  optionally any m
-00005bd0: 6574 6164 6174 6120 7072 6f70 6572 7479  etadata property
-00005be0: 2077 6869 6368 2069 7320 7265 6c61 7465   which is relate
-00005bf0: 6420 746f 2074 6865 2072 6567 696f 6e2e  d to the region.
-00005c00: 0700 0000 0a52 6567 696f 6e73 5461 6201  .....RegionsTab.
-00005c10: 03ff ffff ff08 0000 0000 0600 0000 6d54  ..............mT
-00005c20: 6865 2073 656d 616e 7469 6320 7479 7065  he semantic type
-00005c30: 206f 6620 7768 6174 2069 7320 7368 6f77   of what is show
-00005c40: 6e20 696e 7369 6465 2074 6865 2072 6567  n inside the reg
-00005c50: 696f 6e2e 2054 6865 2076 616c 7565 2053  ion. The value S
-00005c60: 484f 554c 4420 6265 2074 616b 656e 2066  HOULD be taken f
-00005c70: 726f 6d20 6120 436f 6e74 726f 6c6c 6564  rom a Controlled
-00005c80: 2056 6f63 6162 756c 6172 792e 0700 0000   Vocabulary.....
-00005c90: 0a52 6567 696f 6e73 5461 6201 03ff ffff  .RegionsTab.....
-00005ca0: ff08 0000 0000 0600 0000 3f55 6e69 7420  ..........?Unit 
-00005cb0: 7573 6564 2066 6f72 206d 6561 7375 7269  used for measuri
-00005cc0: 6e67 2064 696d 656e 7369 6f6e 7320 6f66  ng dimensions of
-00005cd0: 2074 6865 2062 6f75 6e64 6172 7920 6f66   the boundary of
-00005ce0: 2061 2072 6567 696f 6e2e 0700 0000 0a52   a region......R
-00005cf0: 6567 696f 6e73 5461 6201 03ff ffff ff08  egionsTab.......
-00005d00: 0000 0000 0600 0000 1755 6e72 6561 6461  .........Unreada
-00005d10: 626c 6520 696d 6167 6520 666f 726d 6174  ble image format
-00005d20: 0700 0000 0a52 6567 696f 6e73 5461 6201  .....RegionsTab.
-00005d30: 03ff ffff ff08 0000 0000 0600 0000 0570  ...............p
-00005d40: 6978 656c 0700 0000 0a52 6567 696f 6e73  ixel.....Regions
-00005d50: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00005d60: 0000 0872 656c 6174 6976 6507 0000 000a  ...relative.....
-00005d70: 5265 6769 6f6e 7354 6162 0103 ffff ffff  RegionsTab......
-00005d80: 0800 0000 0006 0000 0013 2654 6563 686e  ..........&Techn
-00005d90: 6963 616c 206d 6574 6164 6174 6107 0000  ical metadata...
-00005da0: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
-00005db0: ffff ffff 0800 0000 0006 0000 000a 3335  ..............35
-00005dc0: 6d6d 2065 7175 6976 0700 0000 0c54 6563  mm equiv.....Tec
-00005dd0: 686e 6963 616c 5461 6201 03ff ffff ff08  hnicalTab.......
-00005de0: 0000 0000 0600 0000 4841 646a 7573 7420  ........HAdjust 
-00005df0: 696d 6167 6520 6170 6572 7475 7265 2061  image aperture a
-00005e00: 6e64 2066 6f63 616c 206c 656e 6774 6820  nd focal length 
-00005e10: 746f 2061 6772 6565 2077 6974 6820 6c65  to agree with le
-00005e20: 6e73 2073 7065 6369 6669 6361 7469 6f6e  ns specification
-00005e30: 3f07 0000 000c 5465 6368 6e69 6361 6c54  ?.....TechnicalT
-00005e40: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00005e50: 000c 4164 6a75 7374 2074 696d 6573 0700  ..Adjust times..
-00005e60: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
-00005e70: 03ff ffff ff08 0000 0000 0600 0000 0841  ...............A
-00005e80: 7065 7274 7572 6507 0000 000c 5465 6368  perture.....Tech
-00005e90: 6e69 6361 6c54 6162 0103 ffff ffff 0800  nicalTab........
-00005ea0: 0000 0006 0000 001d 4170 6572 7475 7265  ........Aperture
-00005eb0: 2061 7420 6d61 782e 2066 6f63 616c 206c   at max. focal l
-00005ec0: 656e 6774 6807 0000 000c 5465 6368 6e69  ength.....Techni
-00005ed0: 6361 6c54 6162 0103 ffff ffff 0800 0000  calTab..........
-00005ee0: 0006 0000 001d 4170 6572 7475 7265 2061  ......Aperture a
-00005ef0: 7420 6d69 6e2e 2066 6f63 616c 206c 656e  t min. focal len
-00005f00: 6774 6807 0000 000c 5465 6368 6e69 6361  gth.....Technica
-00005f10: 6c54 6162 0103 ffff ffff 0800 0000 0006  lTab............
-00005f20: 0000 0006 4361 6d65 7261 0700 0000 0c54  ....Camera.....T
-00005f30: 6563 686e 6963 616c 5461 6201 03ff ffff  echnicalTab.....
-00005f40: ff08 0000 0000 0600 0000 3f43 6861 6e67  ..........?Chang
-00005f50: 696e 6720 6d61 6b65 7220 6e61 6d65 2077  ing maker name w
-00005f60: 696c 6c20 696e 7661 6c69 6461 7465 2045  ill invalidate E
-00005f70: 7869 6620 6d61 6b65 726e 6f74 6520 696e  xif makernote in
-00005f80: 666f 726d 6174 696f 6e2e 0700 0000 0c54  formation......T
-00005f90: 6563 686e 6963 616c 5461 6201 03ff ffff  echnicalTab.....
-00005fa0: ff08 0000 0000 0600 0000 0d44 6174 6520  ...........Date 
-00005fb0: 616e 6420 7469 6d65 0700 0000 0c54 6563  and time.....Tec
-00005fc0: 686e 6963 616c 5461 6201 03ff ffff ff08  hnicalTab.......
-00005fd0: 0000 0000 0600 0000 0944 6967 6974 6973  .........Digitis
-00005fe0: 6564 0700 0000 0c54 6563 686e 6963 616c  ed.....Technical
-00005ff0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00006000: 0000 2944 6f20 796f 7520 7761 6e74 2074  ..)Do you want t
-00006010: 6f20 6465 6c65 7465 2074 6865 2045 7869  o delete the Exi
-00006020: 6620 6d61 6b65 726e 6f74 653f 0700 0000  f makernote?....
-00006030: 0c54 6563 686e 6963 616c 5461 6201 03ff  .TechnicalTab...
-00006040: ffff ff08 0000 0000 0600 0000 0c46 6f63  .............Foc
-00006050: 616c 206c 656e 6774 6807 0000 000c 5465  al length.....Te
-00006060: 6368 6e69 6361 6c54 6162 0103 ffff ffff  chnicalTab......
-00006070: 0800 0000 0006 0000 000a 4c65 6e73 206d  ..........Lens m
-00006080: 6f64 656c 0700 0000 0c54 6563 686e 6963  odel.....Technic
-00006090: 616c 5461 6201 03ff ffff ff08 0000 0000  alTab...........
-000060a0: 0600 0000 1f4c 696e 6b20 2764 6967 6974  .....Link 'digit
-000060b0: 6973 6564 2720 616e 6420 276d 6f64 6966  ised' and 'modif
-000060c0: 6965 6427 0700 0000 0c54 6563 686e 6963  ied'.....Technic
-000060d0: 616c 5461 6201 03ff ffff ff08 0000 0000  alTab...........
-000060e0: 0600 0000 1c4c 696e 6b20 2774 616b 656e  .....Link 'taken
-000060f0: 2720 616e 6420 2764 6967 6974 6973 6564  ' and 'digitised
-00006100: 2707 0000 000c 5465 6368 6e69 6361 6c54  '.....TechnicalT
-00006110: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00006120: 000c 4d61 6b65 7227 7320 6e61 6d65 0700  ..Maker's name..
-00006130: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
-00006140: 03ff ffff ff08 0000 0000 0600 0000 0c4d  ...............M
-00006150: 6178 2061 7065 7274 7572 6507 0000 000c  ax aperture.....
-00006160: 5465 6368 6e69 6361 6c54 6162 0103 ffff  TechnicalTab....
-00006170: ffff 0800 0000 0006 0000 0014 4d61 7869  ............Maxi
-00006180: 6d75 6d20 666f 6361 6c20 6c65 6e67 7468  mum focal length
-00006190: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
-000061a0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-000061b0: 144d 696e 696d 756d 2066 6f63 616c 206c  .Minimum focal l
-000061c0: 656e 6774 6807 0000 000c 5465 6368 6e69  ength.....Techni
-000061d0: 6361 6c54 6162 0103 ffff ffff 0800 0000  calTab..........
-000061e0: 0006 0000 000a 4d6f 6465 6c20 6e61 6d65  ......Model name
-000061f0: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
-00006200: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00006210: 084d 6f64 6966 6965 6407 0000 000c 5465  .Modified.....Te
-00006220: 6368 6e69 6361 6c54 6162 0103 ffff ffff  chnicalTab......
-00006230: 0800 0000 0006 0000 000b 4f72 6965 6e74  ..........Orient
-00006240: 6174 696f 6e07 0000 000c 5465 6368 6e69  ation.....Techni
-00006250: 6361 6c54 6162 0103 ffff ffff 0800 0000  calTab..........
-00006260: 0006 0000 0005 4f74 6865 7207 0000 000c  ......Other.....
-00006270: 5465 6368 6e69 6361 6c54 6162 0103 ffff  TechnicalTab....
-00006280: ffff 0800 0000 0006 0000 0016 5068 6f74  ............Phot
-00006290: 696e 693a 2064 6566 696e 6520 6361 6d65  ini: define came
-000062a0: 7261 0700 0000 0c54 6563 686e 6963 616c  ra.....Technical
-000062b0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-000062c0: 0000 1450 686f 7469 6e69 3a20 6465 6669  ...Photini: defi
-000062d0: 6e65 206c 656e 7307 0000 000c 5465 6368  ne lens.....Tech
-000062e0: 6e69 6361 6c54 6162 0103 ffff ffff 0800  nicalTab........
-000062f0: 0000 0006 0000 001a 5068 6f74 696e 693a  ........Photini:
-00006300: 206d 616b 6572 206e 616d 6520 6368 616e   maker name chan
-00006310: 6765 0700 0000 0c54 6563 686e 6963 616c  ge.....Technical
-00006320: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
-00006330: 0000 0950 7265 6369 7369 6f6e 0700 0000  ...Precision....
-00006340: 0c54 6563 686e 6963 616c 5461 6201 03ff  .TechnicalTab...
-00006350: ffff ff08 0000 0000 0600 0000 1952 656d  .............Rem
-00006360: 6f76 6520 227b 6361 6d65 7261 5f6f 725f  ove "{camera_or_
-00006370: 6c65 6e73 7d22 0700 0000 0c54 6563 686e  lens}".....Techn
+00003dd0: 0000 1550 686f 7469 6e69 2064 6f63 756d  ...Photini docum
+00003de0: 656e 7461 7469 6f6e 0700 0000 074d 656e  entation.....Men
+00003df0: 7542 6172 0103 ffff ffff 0800 0000 0006  uBar............
+00003e00: 0000 001d 5068 6f74 696e 6920 7068 6f74  ....Photini phot
+00003e10: 6f20 6d65 7461 6461 7461 2065 6469 746f  o metadata edito
+00003e20: 7207 0000 0007 4d65 6e75 4261 7201 03ff  r.....MenuBar...
+00003e30: ffff ff08 0000 0000 0600 0000 0e50 686f  .............Pho
+00003e40: 7469 6e69 3a20 6162 6f75 7407 0000 0007  tini: about.....
+00003e50: 4d65 6e75 4261 7201 03ff ffff ff08 0000  MenuBar.........
+00003e60: 0000 0600 0000 1650 686f 7469 6e69 3a20  .......Photini: 
+00003e70: 7665 7273 696f 6e20 6368 6563 6b07 0000  version check...
+00003e80: 0007 4d65 6e75 4261 7201 03ff ffff ff08  ..MenuBar.......
+00003e90: 0000 0000 0600 0000 0451 7569 7407 0000  .........Quit...
+00003ea0: 0007 4d65 6e75 4261 7201 03ff ffff ff08  ..MenuBar.......
+00003eb0: 0000 0000 0600 0000 0c53 6176 6520 6368  .........Save ch
+00003ec0: 616e 6765 7307 0000 0007 4d65 6e75 4261  anges.....MenuBa
+00003ed0: 7201 03ff ffff ff08 0000 0000 0600 0000  r...............
+00003ee0: 0f53 656c 6563 7465 6420 696d 6167 6573  .Selected images
+00003ef0: 0700 0000 074d 656e 7542 6172 0103 ffff  .....MenuBar....
+00003f00: ffff 0800 0000 0006 0000 0008 5365 7474  ............Sett
+00003f10: 696e 6773 0700 0000 074d 656e 7542 6172  ings.....MenuBar
+00003f20: 0103 ffff ffff 0800 0000 0006 0000 0008  ................
+00003f30: 5370 656c 6c69 6e67 0700 0000 074d 656e  Spelling.....Men
+00003f40: 7542 6172 0103 ffff ffff 0800 0000 0006  uBar............
+00003f50: 0000 0065 5468 6973 2070 726f 6772 616d  ...eThis program
+00003f60: 2069 7320 7265 6c65 6173 6564 2077 6974   is released wit
+00003f70: 6820 6120 474e 5520 4765 6e65 7261 6c20  h a GNU General 
+00003f80: 5075 626c 6963 204c 6963 656e 7365 2e20  Public License. 
+00003f90: 466f 7220 6465 7461 696c 7320 636c 6963  For details clic
+00003fa0: 6b20 7468 6520 227b 6465 7461 696c 737d  k the "{details}
+00003fb0: 2220 6275 7474 6f6e 2e07 0000 0007 4d65  " button......Me
+00003fc0: 6e75 4261 7201 03ff ffff ff08 0000 0000  nuBar...........
+00003fd0: 0600 0000 5559 6f75 2061 7265 2063 7572  ....UYou are cur
+00003fe0: 7265 6e74 6c79 2072 756e 6e69 6e67 2050  rently running P
+00003ff0: 686f 7469 6e69 2076 6572 7369 6f6e 207b  hotini version {
+00004000: 7665 7273 696f 6e7d 2e20 5468 6520 6c61  version}. The la
+00004010: 7465 7374 2072 656c 6561 7365 2069 7320  test release is 
+00004020: 7b72 656c 6561 7365 7d2e 0700 0000 074d  {release}......M
+00004030: 656e 7542 6172 0103 ffff ffff 0800 0000  enuBar..........
+00004040: 0006 0000 0013 264f 776e 6572 7368 6970  ......&Ownership
+00004050: 206d 6574 6164 6174 6107 0000 0008 4f77   metadata.....Ow
+00004060: 6e65 7254 6162 0103 ffff ffff 0800 0000  nerTab..........
+00004070: 0006 0000 0013 416c 6c20 7269 6768 7473  ......All rights
+00004080: 2072 6573 6572 7665 6407 0000 0008 4f77   reserved.....Ow
+00004090: 6e65 7254 6162 0103 ffff ffff 0800 0000  nerTab..........
+000040a0: 0006 0000 000e 4170 706c 7920 7465 6d70  ......Apply temp
+000040b0: 6c61 7465 0700 0000 084f 776e 6572 5461  late.....OwnerTa
+000040c0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+000040d0: 1b41 7474 7269 6275 7469 6f6e 2034 2e30  .Attribution 4.0
+000040e0: 2028 4343 2042 5920 342e 3029 0700 0000   (CC BY 4.0)....
+000040f0: 084f 776e 6572 5461 6201 03ff ffff ff08  .OwnerTab.......
+00004100: 0000 0000 0600 0000 2c41 7474 7269 6275  ........,Attribu
+00004110: 7469 6f6e 2d4e 6f44 6572 6976 6174 6976  tion-NoDerivativ
+00004120: 6573 2034 2e30 2028 4343 2042 592d 4e44  es 4.0 (CC BY-ND
+00004130: 2034 2e30 2907 0000 0008 4f77 6e65 7254   4.0).....OwnerT
+00004140: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00004150: 002c 4174 7472 6962 7574 696f 6e2d 4e6f  .,Attribution-No
+00004160: 6e43 6f6d 6d65 7263 6961 6c20 342e 3020  nCommercial 4.0 
+00004170: 2843 4320 4259 2d4e 4320 342e 3029 0700  (CC BY-NC 4.0)..
+00004180: 0000 084f 776e 6572 5461 6201 03ff ffff  ...OwnerTab.....
+00004190: ff08 0000 0000 0600 0000 3d41 7474 7269  ..........=Attri
+000041a0: 6275 7469 6f6e 2d4e 6f6e 436f 6d6d 6572  bution-NonCommer
+000041b0: 6369 616c 2d4e 6f44 6572 6976 6174 6976  cial-NoDerivativ
+000041c0: 6573 2034 2e30 2028 4343 2042 592d 4e43  es 4.0 (CC BY-NC
+000041d0: 2d4e 4420 342e 3029 0700 0000 084f 776e  -ND 4.0).....Own
+000041e0: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
+000041f0: 0600 0000 3a41 7474 7269 6275 7469 6f6e  ....:Attribution
+00004200: 2d4e 6f6e 436f 6d6d 6572 6369 616c 2d53  -NonCommercial-S
+00004210: 6861 7265 416c 696b 6520 342e 3020 2843  hareAlike 4.0 (C
+00004220: 4320 4259 2d4e 432d 5341 2034 2e30 2907  C BY-NC-SA 4.0).
+00004230: 0000 0008 4f77 6e65 7254 6162 0103 ffff  ....OwnerTab....
+00004240: ffff 0800 0000 0006 0000 0029 4174 7472  ...........)Attr
+00004250: 6962 7574 696f 6e2d 5368 6172 6541 6c69  ibution-ShareAli
+00004260: 6b65 2034 2e30 2028 4343 2042 592d 5341  ke 4.0 (CC BY-SA
+00004270: 2034 2e30 2907 0000 0008 4f77 6e65 7254   4.0).....OwnerT
+00004280: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00004290: 0034 4343 3020 312e 3020 556e 6976 6572  .4CC0 1.0 Univer
+000042a0: 7361 6c20 2843 4330 2031 2e30 2920 5075  sal (CC0 1.0) Pu
+000042b0: 626c 6963 2044 6f6d 6169 6e20 4465 6469  blic Domain Dedi
+000042c0: 6361 7469 6f6e 0700 0000 084f 776e 6572  cation.....Owner
+000042d0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+000042e0: 0000 0443 6974 7907 0000 0008 4f77 6e65  ...City.....Owne
+000042f0: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
+00004300: 0000 0010 436f 7079 7269 6768 7420 4e6f  ....Copyright No
+00004310: 7469 6365 0700 0000 084f 776e 6572 5461  tice.....OwnerTa
+00004320: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00004330: 0743 6f75 6e74 7279 0700 0000 084f 776e  .Country.....Own
+00004340: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
+00004350: 0600 0000 0743 7265 6174 6f72 0700 0000  .....Creator....
+00004360: 084f 776e 6572 5461 6201 03ff ffff ff08  .OwnerTab.......
+00004370: 0000 0000 0600 0000 2643 7265 6174 6f72  ........&Creator
+00004380: 202f 204c 6963 656e 736f 7220 436f 6e74   / Licensor Cont
+00004390: 6163 7420 496e 666f 726d 6174 696f 6e07  act Information.
+000043a0: 0000 0008 4f77 6e65 7254 6162 0103 ffff  ....OwnerTab....
+000043b0: ffff 0800 0000 0006 0000 0012 4372 6561  ............Crea
+000043c0: 746f 7227 7320 4a6f 6274 6974 6c65 0700  tor's Jobtitle..
+000043d0: 0000 084f 776e 6572 5461 6201 03ff ffff  ...OwnerTab.....
+000043e0: ff08 0000 0000 0600 0000 0b43 7265 6469  ...........Credi
+000043f0: 7420 4c69 6e65 0700 0000 084f 776e 6572  t Line.....Owner
+00004400: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00004410: 0000 1244 6566 696e 6520 6e65 7720 6c69  ...Define new li
+00004420: 6365 6e63 6507 0000 0008 4f77 6e65 7254  cence.....OwnerT
+00004430: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00004440: 000e 4465 7461 696c 2041 6464 7265 7373  ..Detail Address
+00004450: 0700 0000 084f 776e 6572 5461 6201 03ff  .....OwnerTab...
+00004460: ffff ff08 0000 0000 0600 0000 0d45 6469  .............Edi
+00004470: 7420 7465 6d70 6c61 7465 0700 0000 084f  t template.....O
+00004480: 776e 6572 5461 6201 03ff ffff ff08 0000  wnerTab.........
+00004490: 0000 0600 0000 0845 6d61 696c 2873 2907  .......Email(s).
+000044a0: 0000 0008 4f77 6e65 7254 6162 0103 ffff  ....OwnerTab....
+000044b0: ffff 0800 0000 0006 0000 005f 456e 7465  ..........._Ente
+000044c0: 7220 6120 6e6f 7469 6365 206f 6e20 7468  r a notice on th
+000044d0: 6520 6375 7272 656e 7420 6f77 6e65 7220  e current owner 
+000044e0: 6f66 2074 6865 2063 6f70 7972 6967 6874  of the copyright
+000044f0: 2066 6f72 2074 6869 7320 696d 6167 652c   for this image,
+00004500: 2073 7563 6820 6173 2022 c2a9 3230 3038   such as "..2008
+00004510: 204a 616e 6520 446f 6522 2e07 0000 0008   Jane Doe"......
+00004520: 4f77 6e65 7254 6162 0103 ffff ffff 0800  OwnerTab........
+00004530: 0000 0006 0000 005e 456e 7465 7220 6164  .......^Enter ad
+00004540: 6472 6573 7320 6465 7461 696c 2028 652e  dress detail (e.
+00004550: 672e 2066 6c61 7420 6e75 6d62 6572 206f  g. flat number o
+00004560: 7220 726f 6f6d 206e 756d 6265 7229 2066  r room number) f
+00004570: 6f72 2074 6865 2070 6572 736f 6e20 7468  or the person th
+00004580: 6174 2063 7265 6174 6564 2074 6869 7320  at created this 
+00004590: 696d 6167 652e 0700 0000 084f 776e 6572  image......Owner
+000045a0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+000045b0: 0000 6545 6e74 6572 2069 6e66 6f72 6d61  ..eEnter informa
+000045c0: 7469 6f6e 2061 626f 7574 2065 6d62 6172  tion about embar
+000045d0: 676f 6573 2c20 6f72 206f 7468 6572 2072  goes, or other r
+000045e0: 6573 7472 6963 7469 6f6e 7320 6e6f 7420  estrictions not 
+000045f0: 636f 7665 7265 6420 6279 2074 6865 2052  covered by the R
+00004600: 6967 6874 7320 5573 6167 6520 5465 726d  ights Usage Term
+00004610: 7320 6669 656c 642e 0700 0000 084f 776e  s field......Own
+00004620: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
+00004630: 0600 0000 3945 6e74 6572 2069 6e73 7472  ....9Enter instr
+00004640: 7563 7469 6f6e 7320 6f6e 2068 6f77 2074  uctions on how t
+00004650: 6869 7320 696d 6167 6520 6361 6e20 6c65  his image can le
+00004660: 6761 6c6c 7920 6265 2075 7365 642e 0700  gally be used...
+00004670: 0000 084f 776e 6572 5461 6201 03ff ffff  ...OwnerTab.....
+00004680: ff08 0000 0000 0600 0000 3c45 6e74 6572  ..........<Enter
+00004690: 2073 7472 6565 7420 6164 6472 6573 7320   street address 
+000046a0: 666f 7220 7468 6520 7065 7273 6f6e 2074  for the person t
+000046b0: 6861 7420 6372 6561 7465 6420 7468 6973  hat created this
+000046c0: 2069 6d61 6765 2e07 0000 0008 4f77 6e65   image......Owne
+000046d0: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
+000046e0: 0000 0045 456e 7465 7220 7468 6520 6369  ...EEnter the ci
+000046f0: 7479 2066 6f72 2074 6865 2061 6464 7265  ty for the addre
+00004700: 7373 206f 6620 7468 6520 7065 7273 6f6e  ss of the person
+00004710: 2074 6861 7420 6372 6561 7465 6420 7468   that created th
+00004720: 6973 2069 6d61 6765 2e07 0000 0008 4f77  is image......Ow
+00004730: 6e65 7254 6162 0103 ffff ffff 0800 0000  nerTab..........
+00004740: 0006 0000 004d 456e 7465 7220 7468 6520  .....MEnter the 
+00004750: 636f 756e 7472 7920 6e61 6d65 2066 6f72  country name for
+00004760: 2074 6865 2061 6464 7265 7373 206f 6620   the address of 
+00004770: 7468 6520 7065 7273 6f6e 2074 6861 7420  the person that 
+00004780: 6372 6561 7465 6420 7468 6973 2069 6d61  created this ima
+00004790: 6765 2e07 0000 0008 4f77 6e65 7254 6162  ge......OwnerTab
+000047a0: 0103 ffff ffff 0800 0000 0006 0000 003e  ...............>
+000047b0: 456e 7465 7220 7468 6520 6a6f 6220 7469  Enter the job ti
+000047c0: 746c 6520 6f66 2074 6865 2070 6572 736f  tle of the perso
+000047d0: 6e20 6c69 7374 6564 2069 6e20 7468 6520  n listed in the 
+000047e0: 4372 6561 746f 7220 6669 656c 642e 0700  Creator field...
+000047f0: 0000 084f 776e 6572 5461 6201 03ff ffff  ...OwnerTab.....
+00004800: ff08 0000 0000 0600 0000 3545 6e74 6572  ..........5Enter
+00004810: 2074 6865 206e 616d 6520 6f66 2074 6865   the name of the
+00004820: 2070 6572 736f 6e20 7468 6174 2063 7265   person that cre
+00004830: 6174 6564 2074 6869 7320 696d 6167 652e  ated this image.
+00004840: 0700 0000 084f 776e 6572 5461 6201 03ff  .....OwnerTab...
+00004850: ffff ff08 0000 0000 0600 0000 4c45 6e74  ............LEnt
+00004860: 6572 2074 6865 2070 6f73 7461 6c20 636f  er the postal co
+00004870: 6465 2066 6f72 2074 6865 2061 6464 7265  de for the addre
+00004880: 7373 206f 6620 7468 6520 7065 7273 6f6e  ss of the person
+00004890: 2074 6861 7420 6372 6561 7465 6420 7468   that created th
+000048a0: 6973 2069 6d61 6765 2e07 0000 0008 4f77  is image......Ow
+000048b0: 6e65 7254 6162 0103 ffff ffff 0800 0000  nerTab..........
+000048c0: 0006 0000 0046 456e 7465 7220 7468 6520  .....FEnter the 
+000048d0: 7374 6174 6520 666f 7220 7468 6520 6164  state for the ad
+000048e0: 6472 6573 7320 6f66 2074 6865 2070 6572  dress of the per
+000048f0: 736f 6e20 7468 6174 2063 7265 6174 6564  son that created
+00004900: 2074 6869 7320 696d 6167 652e 0700 0000   this image.....
+00004910: 084f 776e 6572 5461 6201 03ff ffff ff08  .OwnerTab.......
+00004920: 0000 0000 0600 0000 5e45 6e74 6572 2074  ........^Enter t
+00004930: 6865 2077 6f72 6b20 5765 6220 5552 4c20  he work Web URL 
+00004940: 666f 7220 7468 6520 7065 7273 6f6e 2074  for the person t
+00004950: 6861 7420 6372 6561 7465 6420 7468 6973  hat created this
+00004960: 2069 6d61 6765 2c20 7375 6368 2061 7320   image, such as 
+00004970: 6874 7470 3a2f 2f77 7777 2e64 6f6d 6169  http://www.domai
+00004980: 6e2e 636f 6d2f 2e07 0000 0008 4f77 6e65  n.com/......Owne
+00004990: 7254 6162 0103 ffff ffff 0800 0000 0006  rTab............
+000049a0: 0000 005d 456e 7465 7220 7468 6520 776f  ...]Enter the wo
+000049b0: 726b 2065 6d61 696c 2061 6464 7265 7373  rk email address
+000049c0: 2066 6f72 2074 6865 2070 6572 736f 6e20   for the person 
+000049d0: 7468 6174 2063 7265 6174 6564 2074 6869  that created thi
+000049e0: 7320 696d 6167 652c 2073 7563 6820 6173  s image, such as
+000049f0: 206e 616d 6540 646f 6d61 696e 2e63 6f6d   name@domain.com
+00004a00: 2e07 0000 0008 4f77 6e65 7254 6162 0103  ......OwnerTab..
+00004a10: ffff ffff 0800 0000 0006 0000 007c 456e  .............|En
+00004a20: 7465 7220 7468 6520 776f 726b 2070 686f  ter the work pho
+00004a30: 6e65 206e 756d 6265 7220 666f 7220 7468  ne number for th
+00004a40: 6520 7065 7273 6f6e 2074 6861 7420 6372  e person that cr
+00004a50: 6561 7465 6420 7468 6973 2069 6d61 6765  eated this image
+00004a60: 2c20 7573 696e 6720 7468 6520 696e 7465  , using the inte
+00004a70: 726e 6174 696f 6e61 6c20 666f 726d 6174  rnational format
+00004a80: 2c20 7375 6368 2061 7320 2b31 2028 3132  , such as +1 (12
+00004a90: 3329 2034 3536 3738 392e 0700 0000 084f  3) 456789......O
+00004aa0: 776e 6572 5461 6201 03ff ffff ff08 0000  wnerTab.........
+00004ab0: 0000 0600 0000 3a45 6e74 6572 2077 686f  ......:Enter who
+00004ac0: 2073 686f 756c 6420 6265 2063 7265 6469   should be credi
+00004ad0: 7465 6420 7768 656e 2074 6869 7320 696d  ted when this im
+00004ae0: 6167 6520 6973 2070 7562 6c69 7368 6564  age is published
+00004af0: 2e07 0000 0008 4f77 6e65 7254 6162 0103  ......OwnerTab..
+00004b00: ffff ffff 0800 0000 0006 0000 0013 496e  ..............In
+00004b10: 6974 6961 6c69 7365 2074 656d 706c 6174  itialise templat
+00004b20: 6507 0000 0008 4f77 6e65 7254 6162 0103  e.....OwnerTab..
+00004b30: ffff ffff 0800 0000 0006 0000 000c 496e  ..............In
+00004b40: 7374 7275 6374 696f 6e73 0700 0000 084f  structions.....O
+00004b50: 776e 6572 5461 6201 03ff ffff ff08 0000  wnerTab.........
+00004b60: 0000 0600 0000 044e 616d 6507 0000 0008  .......Name.....
+00004b70: 4f77 6e65 7254 6162 0103 ffff ffff 0800  OwnerTab........
+00004b80: 0000 0006 0000 0018 4f70 656e 206c 696e  ........Open lin
+00004b90: 6b20 746f 2022 7b6c 6963 656e 6365 7d22  k to "{licence}"
+00004ba0: 0700 0000 084f 776e 6572 5461 6201 03ff  .....OwnerTab...
+00004bb0: ffff ff08 0000 0000 0600 0000 0850 686f  .............Pho
+00004bc0: 6e65 2873 2907 0000 0008 4f77 6e65 7254  ne(s).....OwnerT
+00004bd0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00004be0: 001b 5068 6f74 696e 693a 206f 776e 6572  ..Photini: owner
+00004bf0: 7368 6970 2074 656d 706c 6174 6507 0000  ship template...
+00004c00: 0008 4f77 6e65 7254 6162 0103 ffff ffff  ..OwnerTab......
+00004c10: 0800 0000 0006 0000 000b 506f 7374 616c  ..........Postal
+00004c20: 2043 6f64 6507 0000 0008 4f77 6e65 7254   Code.....OwnerT
+00004c30: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00004c40: 0016 5075 626c 6963 2044 6f6d 6169 6e20  ..Public Domain 
+00004c50: 4d61 726b 2031 2e30 0700 0000 084f 776e  Mark 1.0.....Own
+00004c60: 6572 5461 6201 03ff ffff ff08 0000 0000  erTab...........
+00004c70: 0600 0000 0652 6967 6874 7307 0000 0008  .....Rights.....
+00004c80: 4f77 6e65 7254 6162 0103 ffff ffff 0800  OwnerTab........
+00004c90: 0000 0006 0000 000e 5374 6174 652f 5072  ........State/Pr
+00004ca0: 6f76 696e 6365 0700 0000 084f 776e 6572  ovince.....Owner
+00004cb0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00004cc0: 0000 0e53 7472 6565 7420 4164 6472 6573  ...Street Addres
+00004cd0: 7307 0000 0008 4f77 6e65 7254 6162 0103  s.....OwnerTab..
+00004ce0: ffff ffff 0800 0000 0006 0000 0003 5552  ..............UR
+00004cf0: 4c07 0000 0008 4f77 6e65 7254 6162 0103  L.....OwnerTab..
+00004d00: ffff ffff 0800 0000 0006 0000 000b 5573  ..............Us
+00004d10: 6167 6520 5465 726d 7307 0000 0008 4f77  age Terms.....Ow
+00004d20: 6e65 7254 6162 0103 ffff ffff 0800 0000  nerTab..........
+00004d30: 0006 0000 0033 5573 6520 2559 2074 6f20  .....3Use %Y to 
+00004d40: 696e 7365 7274 2074 6865 2079 6561 7220  insert the year 
+00004d50: 7468 6520 7068 6f74 6f67 7261 7068 2077  the photograph w
+00004d60: 6173 2074 616b 656e 2e07 0000 0008 4f77  as taken......Ow
+00004d70: 6e65 7254 6162 0103 ffff ffff 0800 0000  nerTab..........
+00004d80: 0006 0000 000d 5765 6220 5374 6174 656d  ......Web Statem
+00004d90: 656e 7407 0000 0008 4f77 6e65 7254 6162  ent.....OwnerTab
+00004da0: 0103 ffff ffff 0800 0000 0006 0000 000a  ................
+00004db0: 5765 6220 5552 4c28 7329 0700 0000 084f  Web URL(s).....O
+00004dc0: 776e 6572 5461 6201 03ff ffff ff08 0000  wnerTab.........
+00004dd0: 0000 0600 0000 0220 6d07 0000 000a 5068  ....... m.....Ph
+00004de0: 6f74 696e 694d 6170 0103 ffff ffff 0800  otiniMap........
+00004df0: 0000 0006 0000 000c 3c6e 6577 2073 6561  ........<new sea
+00004e00: 7263 683e 0700 0000 0a50 686f 7469 6e69  rch>.....Photini
+00004e10: 4d61 7001 03ff ffff ff08 0000 0000 0600  Map.............
+00004e20: 0000 0f3c 7265 7065 6174 2073 6561 7263  ...<repeat searc
+00004e30: 683e 0700 0000 0a50 686f 7469 6e69 4d61  h>.....PhotiniMa
+00004e40: 7001 03ff ffff ff08 0000 0000 0600 0000  p...............
+00004e50: 0e3c 7769 6465 6e20 7365 6172 6368 3e07  .<widen search>.
+00004e60: 0000 000a 5068 6f74 696e 694d 6170 0103  ....PhotiniMap..
+00004e70: ffff ffff 0800 0000 0006 0000 0008 416c  ..............Al
+00004e80: 7469 7475 6465 0700 0000 0a50 686f 7469  titude.....Photi
+00004e90: 6e69 4d61 7001 03ff ffff ff08 0000 0000  niMap...........
+00004ea0: 0600 0000 1547 6574 2061 6c74 6974 7564  .....Get altitud
+00004eb0: 6520 6672 6f6d 206d 6170 0700 0000 0a50  e from map.....P
+00004ec0: 686f 7469 6e69 4d61 7001 03ff ffff ff08  hotiniMap.......
+00004ed0: 0000 0000 0600 0000 0d4c 6f61 6420 4750  .........Load GP
+00004ee0: 5820 6669 6c65 0700 0000 0a50 686f 7469  X file.....Photi
+00004ef0: 6e69 4d61 7001 03ff ffff ff08 0000 0000  niMap...........
+00004f00: 0600 0000 0f52 656d 6f76 6520 4750 5820  .....Remove GPX 
+00004f10: 6461 7461 0700 0000 0a50 686f 7469 6e69  data.....Photini
+00004f20: 4d61 7001 03ff ffff ff08 0000 0000 0600  Map.............
+00004f30: 0000 0653 6561 7263 6807 0000 000a 5068  ...Search.....Ph
+00004f40: 6f74 696e 694d 6170 0103 ffff ffff 0800  otiniMap........
+00004f50: 0000 0006 0000 0013 5365 7420 636f 6f72  ........Set coor
+00004f60: 6473 2066 726f 6d20 4750 5807 0000 000a  ds from GPX.....
+00004f70: 5068 6f74 696e 694d 6170 0103 ffff ffff  PhotiniMap......
+00004f80: 0800 0000 0006 0000 0010 2650 6978 656c  ..........&Pixel
+00004f90: 6665 6420 7570 6c6f 6164 0700 0000 0b50  fed upload.....P
+00004fa0: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
+00004fb0: 0800 0000 0006 0000 0012 4164 6420 746f  ..........Add to
+00004fc0: 2063 6f6c 6c65 6374 696f 6e73 0700 0000   collections....
+00004fd0: 0b50 6978 656c 6665 6454 6162 0103 ffff  .PixelfedTab....
+00004fe0: ffff 0800 0000 0006 0000 0013 416c 6c20  ............All 
+00004ff0: 5269 6768 7473 2052 6573 6572 7665 6407  Rights Reserved.
+00005000: 0000 000b 5069 7865 6c66 6564 5461 6201  ....PixelfedTab.
+00005010: 03ff ffff ff08 0000 0000 0600 0000 0b41  ...............A
+00005020: 7474 7269 6275 7469 6f6e 0700 0000 0b50  ttribution.....P
+00005030: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
+00005040: 0800 0000 0006 0000 0014 4174 7472 6962  ..........Attrib
+00005050: 7574 696f 6e2d 4e6f 4465 7269 7673 0700  ution-NoDerivs..
+00005060: 0000 0b50 6978 656c 6665 6454 6162 0103  ...PixelfedTab..
+00005070: ffff ffff 0800 0000 0006 0000 0019 4174  ..............At
+00005080: 7472 6962 7574 696f 6e2d 4e6f 6e43 6f6d  tribution-NonCom
+00005090: 6d65 7263 6961 6c07 0000 000b 5069 7865  mercial.....Pixe
+000050a0: 6c66 6564 5461 6201 03ff ffff ff08 0000  lfedTab.........
+000050b0: 0000 0600 0000 2241 7474 7269 6275 7469  ......"Attributi
+000050c0: 6f6e 2d4e 6f6e 436f 6d6d 6572 6369 616c  on-NonCommercial
+000050d0: 2d4e 6f44 6572 6976 7307 0000 000b 5069  -NoDerivs.....Pi
+000050e0: 7865 6c66 6564 5461 6201 03ff ffff ff08  xelfedTab.......
+000050f0: 0000 0000 0600 0000 2441 7474 7269 6275  ........$Attribu
+00005100: 7469 6f6e 2d4e 6f6e 436f 6d6d 6572 6369  tion-NonCommerci
+00005110: 616c 2d53 6861 7265 416c 696b 6507 0000  al-ShareAlike...
+00005120: 000b 5069 7865 6c66 6564 5461 6201 03ff  ..PixelfedTab...
+00005130: ffff ff08 0000 0000 0600 0000 1641 7474  .............Att
+00005140: 7269 6275 7469 6f6e 2d53 6861 7265 416c  ribution-ShareAl
+00005150: 696b 6507 0000 000b 5069 7865 6c66 6564  ike.....Pixelfed
+00005160: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00005170: 0000 0743 6170 7469 6f6e 0700 0000 0b50  ...Caption.....P
+00005180: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
+00005190: 0800 0000 0006 0000 0012 4368 6f6f 7365  ..........Choose
+000051a0: 2061 6e20 696e 7374 616e 6365 0700 0000   an instance....
+000051b0: 0b50 6978 656c 6665 6454 6162 0103 ffff  .PixelfedTab....
+000051c0: ffff 0800 0000 0006 0000 0015 436f 6c6c  ............Coll
+000051d0: 6563 7469 6f6e 2076 6973 6962 696c 6974  ection visibilit
+000051e0: 7907 0000 000b 5069 7865 6c66 6564 5461  y.....PixelfedTa
+000051f0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00005200: 1543 7265 6174 6520 6e65 7720 636f 6c6c  .Create new coll
+00005210: 6563 7469 6f6e 0700 0000 0b50 6978 656c  ection.....Pixel
+00005220: 6665 6454 6162 0103 ffff ffff 0800 0000  fedTab..........
+00005230: 0006 0000 000b 4465 7363 7269 7074 696f  ......Descriptio
+00005240: 6e07 0000 000b 5069 7865 6c66 6564 5461  n.....PixelfedTa
+00005250: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00005260: 1044 6973 6162 6c65 2063 6f6d 6d65 6e74  .Disable comment
+00005270: 7307 0000 000b 5069 7865 6c66 6564 5461  s.....PixelfedTa
+00005280: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00005290: 0544 7261 6674 0700 0000 0b50 6978 656c  .Draft.....Pixel
+000052a0: 6665 6454 6162 0103 ffff ffff 0800 0000  fedTab..........
+000052b0: 0006 0000 0066 4669 6c65 2022 7b66 696c  .....fFile "{fil
+000052c0: 655f 6e61 6d65 7d22 2064 6f65 7320 6e6f  e_name}" does no
+000052d0: 7420 6861 7665 2061 6e79 2022 616c 7420  t have any "alt 
+000052e0: 7465 7874 2220 666f 7220 6163 6365 7373  text" for access
+000052f0: 6962 696c 6974 792e 2057 6f75 6c64 2079  ibility. Would y
+00005300: 6f75 206c 696b 6520 746f 2075 706c 6f61  ou like to uploa
+00005310: 6420 6974 2061 6e79 7761 793f 0700 0000  d it anyway?....
+00005320: 0b50 6978 656c 6665 6454 6162 0103 ffff  .PixelfedTab....
+00005330: ffff 0800 0000 0006 0000 000e 466f 6c6c  ............Foll
+00005340: 6f77 6572 7320 6f6e 6c79 0700 0000 0b50  owers only.....P
+00005350: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
+00005360: 0800 0000 0006 0000 0008 4765 6e65 7261  ..........Genera
+00005370: 7465 0700 0000 0b50 6978 656c 6665 6454  te.....PixelfedT
+00005380: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00005390: 0007 4c69 6365 6e63 6507 0000 000b 5069  ..Licence.....Pi
+000053a0: 7865 6c66 6564 5461 6201 03ff ffff ff08  xelfedTab.......
+000053b0: 0000 0000 0600 0000 114d 6973 7369 6e67  .........Missing
+000053c0: 2061 6c74 2074 6578 742e 0700 0000 0b50   alt text......P
+000053d0: 6978 656c 6665 6454 6162 0103 ffff ffff  ixelfedTab......
+000053e0: 0800 0000 0006 0000 000e 4e65 7720 636f  ..........New co
+000053f0: 6c6c 6563 7469 6f6e 0700 0000 0b50 6978  llection.....Pix
+00005400: 656c 6665 6454 6162 0103 ffff ffff 0800  elfedTab........
+00005410: 0000 0006 0000 0005 4f74 6865 7207 0000  ........Other...
+00005420: 000b 5069 7865 6c66 6564 5461 6201 03ff  ..PixelfedTab...
+00005430: ffff ff08 0000 0000 0600 0000 1150 686f  .............Pho
+00005440: 7469 6e69 3a20 616c 7420 7465 7874 0700  tini: alt text..
+00005450: 0000 0b50 6978 656c 6665 6454 6162 0103  ...PixelfedTab..
+00005460: ffff ffff 0800 0000 0006 0000 0018 5068  ..............Ph
+00005470: 6f74 696e 693a 2063 686f 6f73 6520 696e  otini: choose in
+00005480: 7374 616e 6365 0700 0000 0b50 6978 656c  stance.....Pixel
+00005490: 6665 6454 6162 0103 ffff ffff 0800 0000  fedTab..........
+000054a0: 0006 0000 0008 5069 7865 6c66 6564 0700  ......Pixelfed..
+000054b0: 0000 0b50 6978 656c 6665 6454 6162 0103  ...PixelfedTab..
+000054c0: ffff ffff 0800 0000 0006 0000 000f 506f  ..............Po
+000054d0: 7374 2076 6973 6962 696c 6974 7907 0000  st visibility...
+000054e0: 000b 5069 7865 6c66 6564 5461 6201 03ff  ..PixelfedTab...
+000054f0: ffff ff08 0000 0000 0600 0000 0650 7562  .............Pub
+00005500: 6c69 6307 0000 000b 5069 7865 6c66 6564  lic.....Pixelfed
+00005510: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00005520: 0000 1e50 7562 6c69 6320 446f 6d61 696e  ...Public Domain
+00005530: 2044 6564 6963 6174 696f 6e20 2843 4330   Dedication (CC0
+00005540: 2907 0000 000b 5069 7865 6c66 6564 5461  ).....PixelfedTa
+00005550: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00005560: 1250 7562 6c69 6320 446f 6d61 696e 2057  .Public Domain W
+00005570: 6f72 6b07 0000 000b 5069 7865 6c66 6564  ork.....Pixelfed
+00005580: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00005590: 0000 0e53 656e 7369 7469 7665 2070 6f73  ...Sensitive pos
+000055a0: 7407 0000 000b 5069 7865 6c66 6564 5461  t.....PixelfedTa
+000055b0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+000055c0: 0753 706f 696c 6572 0700 0000 0b50 6978  .Spoiler.....Pix
+000055d0: 656c 6665 6454 6162 0103 ffff ffff 0800  elfedTab........
+000055e0: 0000 0006 0000 0005 5469 746c 6507 0000  ........Title...
+000055f0: 000b 5069 7865 6c66 6564 5461 6201 03ff  ..PixelfedTab...
+00005600: ffff ff08 0000 0000 0600 0000 0855 6e6c  .............Unl
+00005610: 6973 7465 6407 0000 000b 5069 7865 6c66  isted.....Pixelf
+00005620: 6564 5461 6201 03ff ffff ff08 0000 0000  edTab...........
+00005630: 0600 0000 0d55 7064 6174 6520 7265 6d6f  .....Update remo
+00005640: 7465 0700 0000 0b50 6978 656c 6665 6454  te.....PixelfedT
+00005650: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00005660: 002b 5768 6963 6820 5069 7865 6c66 6564  .+Which Pixelfed
+00005670: 2069 6e73 7461 6e63 6520 686f 7374 7320   instance hosts 
+00005680: 796f 7572 2061 6363 6f75 6e74 3f07 0000  your account?...
+00005690: 000b 5069 7865 6c66 6564 5461 6201 03ff  ..PixelfedTab...
+000056a0: ffff ff08 0000 0000 0600 0000 3541 2070  ............5A p
+000056b0: 6978 656c 206f 6620 6120 6469 6769 7461  ixel of a digita
+000056c0: 6c20 696d 6167 6520 7365 7474 696e 6720  l image setting 
+000056d0: 616e 2061 6273 6f6c 7574 6520 7661 6c75  an absolute valu
+000056e0: 652e 0700 0000 0a52 6567 696f 6e73 5461  e......RegionsTa
+000056f0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00005700: 0d42 6f75 6e64 6172 7920 756e 6974 0700  .Boundary unit..
+00005710: 0000 0a52 6567 696f 6e73 5461 6201 03ff  ...RegionsTab...
+00005720: ffff ff08 0000 0000 0600 0000 0c43 6f6e  .............Con
+00005730: 7465 6e74 2074 7970 6507 0000 000a 5265  tent type.....Re
+00005740: 6769 6f6e 7354 6162 0103 ffff ffff 0800  gionsTab........
+00005750: 0000 0006 0000 000d 4465 6c65 7465 2072  ........Delete r
+00005760: 6567 696f 6e07 0000 000a 5265 6769 6f6e  egion.....Region
+00005770: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
+00005780: 0000 000d 4465 6c65 7465 2076 6572 7465  ....Delete verte
+00005790: 7807 0000 000a 5265 6769 6f6e 7354 6162  x.....RegionsTab
+000057a0: 0103 ffff ffff 0800 0000 0006 0000 000b  ................
+000057b0: 4465 7363 7269 7074 696f 6e07 0000 000a  Description.....
+000057c0: 5265 6769 6f6e 7354 6162 0103 ffff ffff  RegionsTab......
+000057d0: 0800 0000 0006 0000 0058 456e 7465 7220  .........XEnter 
+000057e0: 6120 2263 6170 7469 6f6e 2220 6465 7363  a "caption" desc
+000057f0: 7269 6269 6e67 2074 6865 2077 686f 2c20  ribing the who, 
+00005800: 7768 6174 2c20 616e 6420 7768 7920 6f66  what, and why of
+00005810: 2077 6861 7420 6973 2068 6170 7065 6e69   what is happeni
+00005820: 6e67 2069 6e20 7468 6973 2072 6567 696f  ng in this regio
+00005830: 6e2e 0700 0000 0a52 6567 696f 6e73 5461  n......RegionsTa
+00005840: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00005850: 5e45 6e74 6572 2074 6865 206e 616d 6573  ^Enter the names
+00005860: 206f 6620 7065 6f70 6c65 2073 686f 776e   of people shown
+00005870: 2069 6e20 7468 6973 2072 6567 696f 6e2e   in this region.
+00005880: 2053 6570 6172 6174 6520 6d75 6c74 6970   Separate multip
+00005890: 6c65 2065 6e74 7269 6573 2077 6974 6820  le entries with 
+000058a0: 223b 2220 6368 6172 6163 7465 7273 2e07  ";" characters..
+000058b0: 0000 000a 5265 6769 6f6e 7354 6162 0103  ....RegionsTab..
+000058c0: ffff ffff 0800 0000 0006 0000 0052 4672  .............RFr
+000058d0: 6565 2d74 6578 7420 6e61 6d65 206f 6620  ee-text name of 
+000058e0: 7468 6520 7265 6769 6f6e 2e20 5368 6f75  the region. Shou
+000058f0: 6c64 2062 6520 756e 6971 7565 2061 6d6f  ld be unique amo
+00005900: 6e67 2061 6c6c 2052 6567 696f 6e20 4e61  ng all Region Na
+00005910: 6d65 7320 6f66 2061 6e20 696d 6167 652e  mes of an image.
+00005920: 0700 0000 0a52 6567 696f 6e73 5461 6201  .....RegionsTab.
+00005930: 03ff ffff ff08 0000 0000 0600 0000 0a49  ...............I
+00005940: 6465 6e74 6966 6965 7207 0000 000a 5265  dentifier.....Re
+00005950: 6769 6f6e 7354 6162 0103 ffff ffff 0800  gionsTab........
+00005960: 0000 0006 0000 0090 4964 656e 7469 6669  ........Identifi
+00005970: 6572 206f 6620 7468 6520 7265 6769 6f6e  er of the region
+00005980: 2e20 4d75 7374 2062 6520 756e 6971 7565  . Must be unique
+00005990: 2061 6d6f 6e67 2061 6c6c 2052 6567 696f   among all Regio
+000059a0: 6e20 4964 656e 7469 6669 6572 7320 6f66  n Identifiers of
+000059b0: 2061 6e20 696d 6167 652e 2044 6f65 7320   an image. Does 
+000059c0: 6e6f 7420 6861 7665 2074 6f20 6265 2075  not have to be u
+000059d0: 6e69 7175 6520 6265 796f 6e64 2074 6865  nique beyond the
+000059e0: 206d 6574 6164 6174 6120 6f66 2074 6869   metadata of thi
+000059f0: 7320 696d 6167 652e 0700 0000 0a52 6567  s image......Reg
+00005a00: 696f 6e73 5461 6201 03ff ffff ff08 0000  ionsTab.........
+00005a10: 0000 0600 0000 0e49 6d61 6765 2026 5265  .......Image &Re
+00005a20: 6769 6f6e 7307 0000 000a 5265 6769 6f6e  gions.....Region
+00005a30: 7354 6162 0103 ffff ffff 0800 0000 0006  sTab............
+00005a40: 0000 0004 4e61 6d65 0700 0000 0a52 6567  ....Name.....Reg
+00005a50: 696f 6e73 5461 6201 03ff ffff ff08 0000  ionsTab.........
+00005a60: 0000 0600 0000 0a4e 6577 2063 6972 636c  .......New circl
+00005a70: 6507 0000 000a 5265 6769 6f6e 7354 6162  e.....RegionsTab
+00005a80: 0103 ffff ffff 0800 0000 0006 0000 0009  ................
+00005a90: 4e65 7720 706f 696e 7407 0000 000a 5265  New point.....Re
+00005aa0: 6769 6f6e 7354 6162 0103 ffff ffff 0800  gionsTab........
+00005ab0: 0000 0006 0000 000b 4e65 7720 706f 6c79  ........New poly
+00005ac0: 676f 6e07 0000 000a 5265 6769 6f6e 7354  gon.....RegionsT
+00005ad0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00005ae0: 000d 4e65 7720 7265 6374 616e 676c 6507  ..New rectangle.
+00005af0: 0000 000a 5265 6769 6f6e 7354 6162 0103  ....RegionsTab..
+00005b00: ffff ffff 0800 0000 0006 0000 000a 4e65  ..............Ne
+00005b10: 7720 7665 7274 6578 0700 0000 0a52 6567  w vertex.....Reg
+00005b20: 696f 6e73 5461 6201 03ff ffff ff08 0000  ionsTab.........
+00005b30: 0000 0600 0000 0c50 6572 736f 6e20 7368  .......Person sh
+00005b40: 6f77 6e07 0000 000a 5265 6769 6f6e 7354  own.....RegionsT
+00005b50: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00005b60: 0041 5265 6c61 7469 7665 2070 6172 7420  .ARelative part 
+00005b70: 6f66 2074 6865 2073 697a 6520 6f66 2061  of the size of a
+00005b80: 6e20 696d 6167 6520 616c 6f6e 6720 7468  n image along th
+00005b90: 6520 782d 206f 7220 7468 6520 792d 6178  e x- or the y-ax
+00005ba0: 6973 2e07 0000 000a 5265 6769 6f6e 7354  is......RegionsT
+00005bb0: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00005bc0: 0004 526f 6c65 0700 0000 0a52 6567 696f  ..Role.....Regio
+00005bd0: 6e73 5461 6201 03ff ffff ff08 0000 0000  nsTab...........
+00005be0: 0600 0000 7f52 6f6c 6520 6f66 2074 6869  .....Role of thi
+00005bf0: 7320 7265 6769 6f6e 2061 6d6f 6e67 2061  s region among a
+00005c00: 6c6c 2072 6567 696f 6e73 206f 6620 7468  ll regions of th
+00005c10: 6973 2069 6d61 6765 206f 7220 6f66 206f  is image or of o
+00005c20: 7468 6572 2069 6d61 6765 732e 2054 6865  ther images. The
+00005c30: 2076 616c 7565 2053 484f 554c 4420 6265   value SHOULD be
+00005c40: 2074 616b 656e 2066 726f 6d20 6120 436f   taken from a Co
+00005c50: 6e74 726f 6c6c 6564 2056 6f63 6162 756c  ntrolled Vocabul
+00005c60: 6172 792e 0700 0000 0a52 6567 696f 6e73  ary......Regions
+00005c70: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00005c80: 0000 6454 6865 2049 6d61 6765 2052 6567  ..dThe Image Reg
+00005c90: 696f 6e20 5374 7275 6374 7572 6520 696e  ion Structure in
+00005ca0: 636c 7564 6573 206f 7074 696f 6e61 6c6c  cludes optionall
+00005cb0: 7920 616e 7920 6d65 7461 6461 7461 2070  y any metadata p
+00005cc0: 726f 7065 7274 7920 7768 6963 6820 6973  roperty which is
+00005cd0: 2072 656c 6174 6564 2074 6f20 7468 6520   related to the 
+00005ce0: 7265 6769 6f6e 2e07 0000 000a 5265 6769  region......Regi
+00005cf0: 6f6e 7354 6162 0103 ffff ffff 0800 0000  onsTab..........
+00005d00: 0006 0000 006d 5468 6520 7365 6d61 6e74  .....mThe semant
+00005d10: 6963 2074 7970 6520 6f66 2077 6861 7420  ic type of what 
+00005d20: 6973 2073 686f 776e 2069 6e73 6964 6520  is shown inside 
+00005d30: 7468 6520 7265 6769 6f6e 2e20 5468 6520  the region. The 
+00005d40: 7661 6c75 6520 5348 4f55 4c44 2062 6520  value SHOULD be 
+00005d50: 7461 6b65 6e20 6672 6f6d 2061 2043 6f6e  taken from a Con
+00005d60: 7472 6f6c 6c65 6420 566f 6361 6275 6c61  trolled Vocabula
+00005d70: 7279 2e07 0000 000a 5265 6769 6f6e 7354  ry......RegionsT
+00005d80: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+00005d90: 003f 556e 6974 2075 7365 6420 666f 7220  .?Unit used for 
+00005da0: 6d65 6173 7572 696e 6720 6469 6d65 6e73  measuring dimens
+00005db0: 696f 6e73 206f 6620 7468 6520 626f 756e  ions of the boun
+00005dc0: 6461 7279 206f 6620 6120 7265 6769 6f6e  dary of a region
+00005dd0: 2e07 0000 000a 5265 6769 6f6e 7354 6162  ......RegionsTab
+00005de0: 0103 ffff ffff 0800 0000 0006 0000 0017  ................
+00005df0: 556e 7265 6164 6162 6c65 2069 6d61 6765  Unreadable image
+00005e00: 2066 6f72 6d61 7407 0000 000a 5265 6769   format.....Regi
+00005e10: 6f6e 7354 6162 0103 ffff ffff 0800 0000  onsTab..........
+00005e20: 0006 0000 0005 7069 7865 6c07 0000 000a  ......pixel.....
+00005e30: 5265 6769 6f6e 7354 6162 0103 ffff ffff  RegionsTab......
+00005e40: 0800 0000 0006 0000 0008 7265 6c61 7469  ..........relati
+00005e50: 7665 0700 0000 0a52 6567 696f 6e73 5461  ve.....RegionsTa
+00005e60: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00005e70: 0320 6d6d 0700 0000 0c54 6563 686e 6963  . mm.....Technic
+00005e80: 616c 5461 6201 03ff ffff ff08 0000 0000  alTab...........
+00005e90: 0600 0000 1326 5465 6368 6e69 6361 6c20  .....&Technical 
+00005ea0: 6d65 7461 6461 7461 0700 0000 0c54 6563  metadata.....Tec
+00005eb0: 686e 6963 616c 5461 6201 03ff ffff ff08  hnicalTab.......
+00005ec0: 0000 0000 0600 0000 0a33 356d 6d20 6571  .........35mm eq
+00005ed0: 7569 7607 0000 000c 5465 6368 6e69 6361  uiv.....Technica
+00005ee0: 6c54 6162 0103 ffff ffff 0800 0000 0006  lTab............
+00005ef0: 0000 0048 4164 6a75 7374 2069 6d61 6765  ...HAdjust image
+00005f00: 2061 7065 7274 7572 6520 616e 6420 666f   aperture and fo
+00005f10: 6361 6c20 6c65 6e67 7468 2074 6f20 6167  cal length to ag
+00005f20: 7265 6520 7769 7468 206c 656e 7320 7370  ree with lens sp
+00005f30: 6563 6966 6963 6174 696f 6e3f 0700 0000  ecification?....
+00005f40: 0c54 6563 686e 6963 616c 5461 6201 03ff  .TechnicalTab...
+00005f50: ffff ff08 0000 0000 0600 0000 0c41 646a  .............Adj
+00005f60: 7573 7420 7469 6d65 7307 0000 000c 5465  ust times.....Te
+00005f70: 6368 6e69 6361 6c54 6162 0103 ffff ffff  chnicalTab......
+00005f80: 0800 0000 0006 0000 0008 4170 6572 7475  ..........Apertu
+00005f90: 7265 0700 0000 0c54 6563 686e 6963 616c  re.....Technical
+00005fa0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00005fb0: 0000 1d41 7065 7274 7572 6520 6174 206d  ...Aperture at m
+00005fc0: 6178 2e20 666f 6361 6c20 6c65 6e67 7468  ax. focal length
+00005fd0: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
+00005fe0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00005ff0: 1d41 7065 7274 7572 6520 6174 206d 696e  .Aperture at min
+00006000: 2e20 666f 6361 6c20 6c65 6e67 7468 0700  . focal length..
+00006010: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
+00006020: 03ff ffff ff08 0000 0000 0600 0000 0643  ...............C
+00006030: 616d 6572 6107 0000 000c 5465 6368 6e69  amera.....Techni
+00006040: 6361 6c54 6162 0103 ffff ffff 0800 0000  calTab..........
+00006050: 0006 0000 003f 4368 616e 6769 6e67 206d  .....?Changing m
+00006060: 616b 6572 206e 616d 6520 7769 6c6c 2069  aker name will i
+00006070: 6e76 616c 6964 6174 6520 4578 6966 206d  nvalidate Exif m
+00006080: 616b 6572 6e6f 7465 2069 6e66 6f72 6d61  akernote informa
+00006090: 7469 6f6e 2e07 0000 000c 5465 6368 6e69  tion......Techni
+000060a0: 6361 6c54 6162 0103 ffff ffff 0800 0000  calTab..........
+000060b0: 0006 0000 000d 4461 7465 2061 6e64 2074  ......Date and t
+000060c0: 696d 6507 0000 000c 5465 6368 6e69 6361  ime.....Technica
+000060d0: 6c54 6162 0103 ffff ffff 0800 0000 0006  lTab............
+000060e0: 0000 0009 4469 6769 7469 7365 6407 0000  ....Digitised...
+000060f0: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
+00006100: ffff ffff 0800 0000 0006 0000 0029 446f  .............)Do
+00006110: 2079 6f75 2077 616e 7420 746f 2064 656c   you want to del
+00006120: 6574 6520 7468 6520 4578 6966 206d 616b  ete the Exif mak
+00006130: 6572 6e6f 7465 3f07 0000 000c 5465 6368  ernote?.....Tech
+00006140: 6e69 6361 6c54 6162 0103 ffff ffff 0800  nicalTab........
+00006150: 0000 0006 0000 000c 466f 6361 6c20 6c65  ........Focal le
+00006160: 6e67 7468 0700 0000 0c54 6563 686e 6963  ngth.....Technic
+00006170: 616c 5461 6201 03ff ffff ff08 0000 0000  alTab...........
+00006180: 0600 0000 0a4c 656e 7320 6d6f 6465 6c07  .....Lens model.
+00006190: 0000 000c 5465 6368 6e69 6361 6c54 6162  ....TechnicalTab
+000061a0: 0103 ffff ffff 0800 0000 0006 0000 001f  ................
+000061b0: 4c69 6e6b 2027 6469 6769 7469 7365 6427  Link 'digitised'
+000061c0: 2061 6e64 2027 6d6f 6469 6669 6564 2707   and 'modified'.
+000061d0: 0000 000c 5465 6368 6e69 6361 6c54 6162  ....TechnicalTab
+000061e0: 0103 ffff ffff 0800 0000 0006 0000 001c  ................
+000061f0: 4c69 6e6b 2027 7461 6b65 6e27 2061 6e64  Link 'taken' and
+00006200: 2027 6469 6769 7469 7365 6427 0700 0000   'digitised'....
+00006210: 0c54 6563 686e 6963 616c 5461 6201 03ff  .TechnicalTab...
+00006220: ffff ff08 0000 0000 0600 0000 0c4d 616b  .............Mak
+00006230: 6572 2773 206e 616d 6507 0000 000c 5465  er's name.....Te
+00006240: 6368 6e69 6361 6c54 6162 0103 ffff ffff  chnicalTab......
+00006250: 0800 0000 0006 0000 000c 4d61 7820 6170  ..........Max ap
+00006260: 6572 7475 7265 0700 0000 0c54 6563 686e  erture.....Techn
+00006270: 6963 616c 5461 6201 03ff ffff ff08 0000  icalTab.........
+00006280: 0000 0600 0000 144d 6178 696d 756d 2066  .......Maximum f
+00006290: 6f63 616c 206c 656e 6774 6807 0000 000c  ocal length.....
+000062a0: 5465 6368 6e69 6361 6c54 6162 0103 ffff  TechnicalTab....
+000062b0: ffff 0800 0000 0006 0000 0014 4d69 6e69  ............Mini
+000062c0: 6d75 6d20 666f 6361 6c20 6c65 6e67 7468  mum focal length
+000062d0: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
+000062e0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+000062f0: 0a4d 6f64 656c 206e 616d 6507 0000 000c  .Model name.....
+00006300: 5465 6368 6e69 6361 6c54 6162 0103 ffff  TechnicalTab....
+00006310: ffff 0800 0000 0006 0000 0008 4d6f 6469  ............Modi
+00006320: 6669 6564 0700 0000 0c54 6563 686e 6963  fied.....Technic
+00006330: 616c 5461 6201 03ff ffff ff08 0000 0000  alTab...........
+00006340: 0600 0000 0b4f 7269 656e 7461 7469 6f6e  .....Orientation
+00006350: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
+00006360: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+00006370: 054f 7468 6572 0700 0000 0c54 6563 686e  .Other.....Techn
 00006380: 6963 616c 5461 6201 03ff ffff ff08 0000  icalTab.........
-00006390: 0000 0600 0000 0d53 6572 6961 6c20 6e75  .......Serial nu
-000063a0: 6d62 6572 0700 0000 0c54 6563 686e 6963  mber.....Technic
-000063b0: 616c 5461 6201 03ff ffff ff08 0000 0000  alTab...........
-000063c0: 0600 0000 0554 616b 656e 0700 0000 0c54  .....Taken.....T
-000063d0: 6563 686e 6963 616c 5461 6201 03ff ffff  echnicalTab.....
-000063e0: ff08 0000 0000 0600 0000 1e55 7064 6174  ...........Updat
-000063f0: 6520 6170 6572 7475 7265 2026 2066 6f63  e aperture & foc
-00006400: 616c 206c 656e 6774 6807 0000 000c 5465  al length.....Te
-00006410: 6368 6e69 6361 6c54 6162 0103 ffff ffff  chnicalTab......
-00006420: 0800 0000 0006 0000 0003 6d61 7807 0000  ..........max...
-00006430: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
-00006440: ffff ffff 0800 0000 0006 0000 0003 6d69  ..............mi
-00006450: 6e07 0000 000c 5465 6368 6e69 6361 6c54  n.....TechnicalT
-00006460: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
-00006470: 0006 6e6f 726d 616c 0700 0000 0c54 6563  ..normal.....Tec
-00006480: 686e 6963 616c 5461 6201 03ff ffff ff08  hnicalTab.......
-00006490: 0000 0000 0600 0000 1572 6566 6c65 6374  .........reflect
-000064a0: 206c 6566 7420 746f 2072 6967 6874 0700   left to right..
-000064b0: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
-000064c0: 03ff ffff ff08 0000 0000 0600 0000 2072  .............. r
-000064d0: 6566 6c65 6374 2074 6f70 206c 6566 7420  eflect top left 
-000064e0: 746f 2062 6f74 746f 6d20 7269 6768 7407  to bottom right.
-000064f0: 0000 000c 5465 6368 6e69 6361 6c54 6162  ....TechnicalTab
-00006500: 0103 ffff ffff 0800 0000 0006 0000 0020  ............... 
-00006510: 7265 666c 6563 7420 746f 7020 7269 6768  reflect top righ
-00006520: 7420 746f 2062 6f74 746f 6d20 6c65 6674  t to bottom left
-00006530: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
-00006540: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-00006550: 1572 6566 6c65 6374 2074 6f70 2074 6f20  .reflect top to 
-00006560: 626f 7474 6f6d 0700 0000 0c54 6563 686e  bottom.....Techn
-00006570: 6963 616c 5461 6201 03ff ffff ff08 0000  icalTab.........
-00006580: 0000 0600 0000 0c72 6f74 6174 6520 2b39  .......rotate +9
-00006590: 30c2 b007 0000 000c 5465 6368 6e69 6361  0.......Technica
-000065a0: 6c54 6162 0103 ffff ffff 0800 0000 0006  lTab............
-000065b0: 0000 000c 726f 7461 7465 202d 3930 c2b0  ....rotate -90..
-000065c0: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
-000065d0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
-000065e0: 0c72 6f74 6174 6520 3138 30c2 b007 0000  .rotate 180.....
-000065f0: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
-00006600: ffff ffff 0800 0000 0006 0000 000d 4164  ..............Ad
-00006610: 6420 746f 2061 6c62 756d 7307 0000 000f  d to albums.....
-00006620: 5570 6c6f 6164 6572 5461 6273 416c 6c01  UploaderTabsAll.
-00006630: 03ff ffff ff08 0000 0000 0600 0000 1641  ...............A
-00006640: 7574 686f 7269 7361 7469 6f6e 2072 6571  uthorisation req
-00006650: 7569 7265 6407 0000 000f 5570 6c6f 6164  uired.....Upload
-00006660: 6572 5461 6273 416c 6c01 03ff ffff ff08  erTabsAll.......
-00006670: 0000 0000 0600 0000 0c43 6c6f 7365 2077  .........Close w
-00006680: 696e 646f 7707 0000 000f 5570 6c6f 6164  indow.....Upload
-00006690: 6572 5461 6273 416c 6c01 03ff ffff ff08  erTabsAll.......
-000066a0: 0000 0000 0600 0000 2643 6c6f 7369 6e67  ........&Closing
-000066b0: 206e 6f77 2077 696c 6c20 7465 726d 696e   now will termin
-000066c0: 6174 6520 7468 6520 7570 6c6f 6164 2e07  ate the upload..
-000066d0: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
-000066e0: 416c 6c01 03ff ffff ff08 0000 0000 0600  All.............
-000066f0: 0000 1043 7265 6174 6520 6e65 7720 616c  ...Create new al
-00006700: 6275 6d07 0000 000f 5570 6c6f 6164 6572  bum.....Uploader
-00006710: 5461 6273 416c 6c01 03ff ffff ff08 0000  TabsAll.........
-00006720: 0000 0600 0000 5646 696c 6520 227b 6669  ......VFile "{fi
-00006730: 6c65 5f6e 616d 657d 2220 6861 7320 7b73  le_name}" has {s
-00006740: 697a 657d 2062 7974 6573 2061 6e64 2065  ize} bytes and e
-00006750: 7863 6565 6473 207b 7365 7276 6963 657d  xceeds {service}
-00006760: 2773 206c 696d 6974 206f 6620 7b6d 6178  's limit of {max
-00006770: 5f73 697a 657d 2062 7974 6573 2e07 0000  _size} bytes....
-00006780: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
-00006790: 6c01 03ff ffff ff08 0000 0000 0600 0000  l...............
-000067a0: 5846 696c 6520 227b 6669 6c65 5f6e 616d  XFile "{file_nam
-000067b0: 657d 2220 6861 7320 7b73 697a 657d 2070  e}" has {size} p
-000067c0: 6978 656c 7320 616e 6420 6578 6365 6564  ixels and exceed
-000067d0: 7320 7b73 6572 7669 6365 7d27 7320 6c69  s {service}'s li
-000067e0: 6d69 7420 6f66 207b 6d61 785f 7369 7a65  mit of {max_size
-000067f0: 7d20 7069 7865 6c73 2e07 0000 000f 5570  } pixels......Up
-00006800: 6c6f 6164 6572 5461 6273 416c 6c01 03ff  loaderTabsAll...
-00006810: ffff ff08 0000 0000 0600 0000 5646 696c  ............VFil
-00006820: 6520 227b 6669 6c65 5f6e 616d 657d 2220  e "{file_name}" 
-00006830: 6973 206f 6620 7479 7065 2022 7b66 696c  is of type "{fil
-00006840: 655f 7479 7065 7d22 2c20 7768 6963 6820  e_type}", which 
-00006850: 7b73 6572 7669 6365 7d20 6d61 7920 6e6f  {service} may no
-00006860: 7420 6861 6e64 6c65 2063 6f72 7265 6374  t handle correct
-00006870: 6c79 2e07 0000 000f 5570 6c6f 6164 6572  ly......Uploader
-00006880: 5461 6273 416c 6c01 03ff ffff ff08 0000  TabsAll.........
-00006890: 0000 0600 0000 2146 696c 6520 227b 6669  ......!File "{fi
-000068a0: 6c65 5f6e 616d 657d 2220 7570 6c6f 6164  le_name}" upload
-000068b0: 2066 6169 6c65 642e 0700 0000 0f55 706c   failed......Upl
-000068c0: 6f61 6465 7254 6162 7341 6c6c 0103 ffff  oaderTabsAll....
-000068d0: ffff 0800 0000 0006 0000 000f 4669 6c65  ............File
-000068e0: 2074 6f6f 206c 6172 6765 2e07 0000 000f   too large......
-000068f0: 5570 6c6f 6164 6572 5461 6273 416c 6c01  UploaderTabsAll.
-00006900: 03ff ffff ff08 0000 0000 0600 0000 5946  ..............YF
-00006910: 696c 6520 7b66 696c 655f 6e61 6d65 7d20  ile {file_name} 
-00006920: 6861 7320 616c 7265 6164 7920 6265 656e  has already been
-00006930: 2075 706c 6f61 6465 6420 746f 207b 7365   uploaded to {se
-00006940: 7276 6963 657d 2e20 486f 7720 776f 756c  rvice}. How woul
-00006950: 6420 796f 7520 6c69 6b65 2074 6f20 7570  d you like to up
-00006960: 6461 7465 2069 743f 0700 0000 0f55 706c  date it?.....Upl
-00006970: 6f61 6465 7254 6162 7341 6c6c 0103 ffff  oaderTabsAll....
-00006980: ffff 0800 0000 0006 0000 0018 496e 636f  ............Inco
-00006990: 6d70 6174 6962 6c65 2069 6d61 6765 2074  mpatible image t
-000069a0: 7970 652e 0700 0000 0f55 706c 6f61 6465  ype......Uploade
-000069b0: 7254 6162 7341 6c6c 0103 ffff ffff 0800  rTabsAll........
-000069c0: 0000 0006 0000 0006 4c6f 6720 696e 0700  ........Log in..
-000069d0: 0000 0f55 706c 6f61 6465 7254 6162 7341  ...UploaderTabsA
-000069e0: 6c6c 0103 ffff ffff 0800 0000 0006 0000  ll..............
-000069f0: 0007 4c6f 6720 6f75 7407 0000 000f 5570  ..Log out.....Up
-00006a00: 6c6f 6164 6572 5461 6273 416c 6c01 03ff  loaderTabsAll...
-00006a10: ffff ff08 0000 0000 0600 0000 204c 6f67  ............ Log
-00006a20: 6765 6420 696e 2061 7320 7b75 7365 727d  ged in as {user}
-00006a30: 206f 6e20 7b73 6572 7669 6365 7d07 0000   on {service}...
-00006a40: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
-00006a50: 6c01 03ff ffff ff08 0000 0000 0600 0000  l...............
-00006a60: 0f4e 6f20 696d 6167 6520 7570 6c6f 6164  .No image upload
-00006a70: 0700 0000 0f55 706c 6f61 6465 7254 6162  .....UploaderTab
-00006a80: 7341 6c6c 0103 ffff ffff 0800 0000 0006  sAll............
-00006a90: 0000 0008 4e6f 206d 6174 6368 0700 0000  ....No match....
-00006aa0: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
-00006ab0: 0103 ffff ffff 0800 0000 0006 0000 001a  ................
-00006ac0: 4e6f 7420 6c6f 6767 6564 2069 6e20 746f  Not logged in to
-00006ad0: 207b 7365 7276 6963 657d 0700 0000 0f55   {service}.....U
-00006ae0: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
-00006af0: ffff ffff 0800 0000 0006 0000 0012 5068  ..............Ph
-00006b00: 6f74 696e 693a 2061 7574 686f 7269 7365  otini: authorise
-00006b10: 0700 0000 0f55 706c 6f61 6465 7254 6162  .....UploaderTab
-00006b20: 7341 6c6c 0103 ffff ffff 0800 0000 0006  sAll............
-00006b30: 0000 001a 5068 6f74 696e 693a 2069 6e63  ....Photini: inc
-00006b40: 6f6d 7061 7469 626c 6520 7479 7065 0700  ompatible type..
-00006b50: 0000 0f55 706c 6f61 6465 7254 6162 7341  ...UploaderTabsA
-00006b60: 6c6c 0103 ffff ffff 0800 0000 0006 0000  ll..............
-00006b70: 0012 5068 6f74 696e 693a 2074 6f6f 206c  ..Photini: too l
-00006b80: 6172 6765 0700 0000 0f55 706c 6f61 6465  arge.....Uploade
-00006b90: 7254 6162 7341 6c6c 0103 ffff ffff 0800  rTabsAll........
-00006ba0: 0000 0006 0000 0015 5068 6f74 696e 693a  ........Photini:
-00006bb0: 2075 706c 6f61 6420 6572 726f 7207 0000   upload error...
-00006bc0: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
-00006bd0: 6c01 03ff ffff ff08 0000 0000 0600 0000  l...............
-00006be0: 1b50 686f 7469 6e69 3a20 7570 6c6f 6164  .Photini: upload
-00006bf0: 2069 6e20 7072 6f67 7265 7373 0700 0000   in progress....
-00006c00: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
-00006c10: 0103 ffff ffff 0800 0000 0006 0000 004d  ...............M
-00006c20: 506c 6561 7365 2075 7365 2079 6f75 7220  Please use your 
-00006c30: 7765 6220 6272 6f77 7365 7220 746f 2061  web browser to a
-00006c40: 7574 686f 7269 7365 2050 686f 7469 6e69  uthorise Photini
-00006c50: 2c20 616e 6420 7468 656e 2063 6c6f 7365  , and then close
-00006c60: 2074 6869 7320 6469 616c 6f67 2e07 0000   this dialog....
-00006c70: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
-00006c80: 6c01 03ff ffff ff08 0000 0000 0600 0000  l...............
-00006c90: 0850 726f 6772 6573 7307 0000 000f 5570  .Progress.....Up
-00006ca0: 6c6f 6164 6572 5461 6273 416c 6c01 03ff  loaderTabsAll...
-00006cb0: ffff ff08 0000 0000 0600 0000 0d52 6570  .............Rep
-00006cc0: 6c61 6365 2069 6d61 6765 0700 0000 0f55  lace image.....U
-00006cd0: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
-00006ce0: ffff ffff 0800 0000 0006 0000 000d 5265  ..............Re
-00006cf0: 706c 6163 6520 7068 6f74 6f07 0000 000f  place photo.....
-00006d00: 5570 6c6f 6164 6572 5461 6273 416c 6c01  UploaderTabsAll.
-00006d10: 03ff ffff ff08 0000 0000 0600 0000 0f53  ...............S
-00006d20: 656c 6563 7420 616e 2069 6d61 6765 0700  elect an image..
-00006d30: 0000 0f55 706c 6f61 6465 7254 6162 7341  ...UploaderTabsA
-00006d40: 6c6c 0103 ffff ffff 0800 0000 0006 0000  ll..............
-00006d50: 0004 536b 6970 0700 0000 0f55 706c 6f61  ..Skip.....Uploa
-00006d60: 6465 7254 6162 7341 6c6c 0103 ffff ffff  derTabsAll......
-00006d70: 0800 0000 0006 0000 000c 5374 6172 7420  ..........Start 
-00006d80: 7570 6c6f 6164 0700 0000 0f55 706c 6f61  upload.....Uploa
-00006d90: 6465 7254 6162 7341 6c6c 0103 ffff ffff  derTabsAll......
-00006da0: 0800 0000 0006 0000 000b 5374 6f70 2075  ..........Stop u
-00006db0: 706c 6f61 6407 0000 000f 5570 6c6f 6164  pload.....Upload
-00006dc0: 6572 5461 6273 416c 6c01 03ff ffff ff08  erTabsAll.......
-00006dd0: 0000 0000 0600 0000 1355 706c 6f61 6420  .........Upload 
-00006de0: 6173 206e 6577 2070 686f 746f 0700 0000  as new photo....
-00006df0: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
-00006e00: 0103 ffff ffff 0800 0000 0006 0000 0025  ...............%
-00006e10: 5570 6c6f 6164 2074 6f20 7b73 6572 7669  Upload to {servi
-00006e20: 6365 7d20 6861 7320 6e6f 7420 6669 6e69  ce} has not fini
-00006e30: 7368 6564 2e07 0000 000f 5570 6c6f 6164  shed......Upload
-00006e40: 6572 5461 6273 416c 6c01 03ff ffff ff08  erTabsAll.......
-00006e50: 0000 0000 0600 0000 3357 6869 6368 2069  ........3Which i
-00006e60: 6d61 6765 2066 696c 6520 6d61 7463 6865  mage file matche
-00006e70: 7320 7468 6973 2070 6963 7475 7265 206f  s this picture o
-00006e80: 6e20 7b73 6572 7669 6365 7d3f 0700 0000  n {service}?....
-00006e90: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
-00006ea0: 0103 ffff ffff 0800 0000 0006 0000 0025  ...............%
-00006eb0: 576f 756c 6420 796f 7520 6c69 6b65 2074  Would you like t
-00006ec0: 6f20 636f 6e76 6572 7420 6974 2074 6f20  o convert it to 
-00006ed0: 4a50 4547 3f07 0000 000f 5570 6c6f 6164  JPEG?.....Upload
-00006ee0: 6572 5461 6273 416c 6c01 03ff ffff ff08  erTabsAll.......
-00006ef0: 0000 0000 0600 0000 1c57 6f75 6c64 2079  .........Would y
-00006f00: 6f75 206c 696b 6520 746f 2072 6573 697a  ou like to resiz
-00006f10: 6520 6974 3f07 0000 000f 5570 6c6f 6164  e it?.....Upload
-00006f20: 6572 5461 6273 416c 6c01 03ff ffff ff08  erTabsAll.......
-00006f30: 0000 0000 0600 0000 2357 6f75 6c64 2079  ........#Would y
-00006f40: 6f75 206c 696b 6520 746f 2075 706c 6f61  ou like to uploa
-00006f50: 6420 6974 2061 6e79 7761 793f 0700 0000  d it anyway?....
-00006f60: 0f55 706c 6f61 6465 7254 6162 7341 6c6c  .UploaderTabsAll
-00006f70: 0103 ffff ffff 0800 0000 0006 0000 0026  ...............&
-00006f80: 596f 7520 6d61 7920 6e6f 7720 636c 6f73  You may now clos
-00006f90: 6520 7468 6973 2062 726f 7773 6572 2077  e this browser w
-00006fa0: 696e 646f 772e 0700 0000 0f55 706c 6f61  indow......Uploa
-00006fb0: 6465 7254 6162 7341 6c6c 0103 ffff ffff  derTabsAll......
-00006fc0: 0800 0000 0006 0000 0011 3c6d 756c 7469  ..........<multi
-00006fd0: 706c 6520 7661 6c75 6573 3e07 0000 0007  ple values>.....
-00006fe0: 5769 6467 6574 7301 03ff ffff ff08 0000  Widgets.........
-00006ff0: 0000 0600 0000 0a3c 6d75 6c74 6970 6c65  .......<multiple
-00007000: 3e07 0000 0007 5769 6467 6574 7301 03ff  >.....Widgets...
-00007010: ffff ff08 0000 0000 0600 0000 053c 6e65  .............<ne
-00007020: 773e 0700 0000 0757 6964 6765 7473 0188  w>.....Widgets..
-00007030: 0000 0002 0101                           ......
+00006390: 0000 0600 0000 1650 686f 7469 6e69 3a20  .......Photini: 
+000063a0: 6465 6669 6e65 2063 616d 6572 6107 0000  define camera...
+000063b0: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
+000063c0: ffff ffff 0800 0000 0006 0000 0014 5068  ..............Ph
+000063d0: 6f74 696e 693a 2064 6566 696e 6520 6c65  otini: define le
+000063e0: 6e73 0700 0000 0c54 6563 686e 6963 616c  ns.....Technical
+000063f0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00006400: 0000 1a50 686f 7469 6e69 3a20 6d61 6b65  ...Photini: make
+00006410: 7220 6e61 6d65 2063 6861 6e67 6507 0000  r name change...
+00006420: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
+00006430: ffff ffff 0800 0000 0006 0000 0009 5072  ..............Pr
+00006440: 6563 6973 696f 6e07 0000 000c 5465 6368  ecision.....Tech
+00006450: 6e69 6361 6c54 6162 0103 ffff ffff 0800  nicalTab........
+00006460: 0000 0006 0000 0019 5265 6d6f 7665 2022  ........Remove "
+00006470: 7b63 616d 6572 615f 6f72 5f6c 656e 737d  {camera_or_lens}
+00006480: 2207 0000 000c 5465 6368 6e69 6361 6c54  ".....TechnicalT
+00006490: 6162 0103 ffff ffff 0800 0000 0006 0000  ab..............
+000064a0: 000d 5365 7269 616c 206e 756d 6265 7207  ..Serial number.
+000064b0: 0000 000c 5465 6368 6e69 6361 6c54 6162  ....TechnicalTab
+000064c0: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
+000064d0: 5461 6b65 6e07 0000 000c 5465 6368 6e69  Taken.....Techni
+000064e0: 6361 6c54 6162 0103 ffff ffff 0800 0000  calTab..........
+000064f0: 0006 0000 001e 5570 6461 7465 2061 7065  ......Update ape
+00006500: 7274 7572 6520 2620 666f 6361 6c20 6c65  rture & focal le
+00006510: 6e67 7468 0700 0000 0c54 6563 686e 6963  ngth.....Technic
+00006520: 616c 5461 6201 03ff ffff ff08 0000 0000  alTab...........
+00006530: 0600 0000 0168 0700 0000 0c54 6563 686e  .....h.....Techn
+00006540: 6963 616c 5461 6201 03ff ffff ff08 0000  icalTab.........
+00006550: 0000 0600 0000 016d 0700 0000 0c54 6563  .......m.....Tec
+00006560: 686e 6963 616c 5461 6201 03ff ffff ff08  hnicalTab.......
+00006570: 0000 0000 0600 0000 036d 6178 0700 0000  .........max....
+00006580: 0c54 6563 686e 6963 616c 5461 6201 03ff  .TechnicalTab...
+00006590: ffff ff08 0000 0000 0600 0000 036d 696e  .............min
+000065a0: 0700 0000 0c54 6563 686e 6963 616c 5461  .....TechnicalTa
+000065b0: 6201 03ff ffff ff08 0000 0000 0600 0000  b...............
+000065c0: 066e 6f72 6d61 6c07 0000 000c 5465 6368  .normal.....Tech
+000065d0: 6e69 6361 6c54 6162 0103 ffff ffff 0800  nicalTab........
+000065e0: 0000 0006 0000 0015 7265 666c 6563 7420  ........reflect 
+000065f0: 6c65 6674 2074 6f20 7269 6768 7407 0000  left to right...
+00006600: 000c 5465 6368 6e69 6361 6c54 6162 0103  ..TechnicalTab..
+00006610: ffff ffff 0800 0000 0006 0000 0020 7265  ............. re
+00006620: 666c 6563 7420 746f 7020 6c65 6674 2074  flect top left t
+00006630: 6f20 626f 7474 6f6d 2072 6967 6874 0700  o bottom right..
+00006640: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
+00006650: 03ff ffff ff08 0000 0000 0600 0000 2072  .............. r
+00006660: 6566 6c65 6374 2074 6f70 2072 6967 6874  eflect top right
+00006670: 2074 6f20 626f 7474 6f6d 206c 6566 7407   to bottom left.
+00006680: 0000 000c 5465 6368 6e69 6361 6c54 6162  ....TechnicalTab
+00006690: 0103 ffff ffff 0800 0000 0006 0000 0015  ................
+000066a0: 7265 666c 6563 7420 746f 7020 746f 2062  reflect top to b
+000066b0: 6f74 746f 6d07 0000 000c 5465 6368 6e69  ottom.....Techni
+000066c0: 6361 6c54 6162 0103 ffff ffff 0800 0000  calTab..........
+000066d0: 0006 0000 000c 726f 7461 7465 202b 3930  ......rotate +90
+000066e0: c2b0 0700 0000 0c54 6563 686e 6963 616c  .......Technical
+000066f0: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+00006700: 0000 0c72 6f74 6174 6520 2d39 30c2 b007  ...rotate -90...
+00006710: 0000 000c 5465 6368 6e69 6361 6c54 6162  ....TechnicalTab
+00006720: 0103 ffff ffff 0800 0000 0006 0000 000c  ................
+00006730: 726f 7461 7465 2031 3830 c2b0 0700 0000  rotate 180......
+00006740: 0c54 6563 686e 6963 616c 5461 6201 03ff  .TechnicalTab...
+00006750: ffff ff08 0000 0000 0600 0000 0173 0700  .............s..
+00006760: 0000 0c54 6563 686e 6963 616c 5461 6201  ...TechnicalTab.
+00006770: 03ff ffff ff08 0000 0000 0600 0000 03c6  ................
+00006780: 922f 0700 0000 0c54 6563 686e 6963 616c  ./.....Technical
+00006790: 5461 6201 03ff ffff ff08 0000 0000 0600  Tab.............
+000067a0: 0000 0d41 6464 2074 6f20 616c 6275 6d73  ...Add to albums
+000067b0: 0700 0000 0f55 706c 6f61 6465 7254 6162  .....UploaderTab
+000067c0: 7341 6c6c 0103 ffff ffff 0800 0000 0006  sAll............
+000067d0: 0000 0016 4175 7468 6f72 6973 6174 696f  ....Authorisatio
+000067e0: 6e20 7265 7175 6972 6564 0700 0000 0f55  n required.....U
+000067f0: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
+00006800: ffff ffff 0800 0000 0006 0000 000c 436c  ..............Cl
+00006810: 6f73 6520 7769 6e64 6f77 0700 0000 0f55  ose window.....U
+00006820: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
+00006830: ffff ffff 0800 0000 0006 0000 0026 436c  .............&Cl
+00006840: 6f73 696e 6720 6e6f 7720 7769 6c6c 2074  osing now will t
+00006850: 6572 6d69 6e61 7465 2074 6865 2075 706c  erminate the upl
+00006860: 6f61 642e 0700 0000 0f55 706c 6f61 6465  oad......Uploade
+00006870: 7254 6162 7341 6c6c 0103 ffff ffff 0800  rTabsAll........
+00006880: 0000 0006 0000 0010 4372 6561 7465 206e  ........Create n
+00006890: 6577 2061 6c62 756d 0700 0000 0f55 706c  ew album.....Upl
+000068a0: 6f61 6465 7254 6162 7341 6c6c 0103 ffff  oaderTabsAll....
+000068b0: ffff 0800 0000 0006 0000 0056 4669 6c65  ...........VFile
+000068c0: 2022 7b66 696c 655f 6e61 6d65 7d22 2068   "{file_name}" h
+000068d0: 6173 207b 7369 7a65 7d20 6279 7465 7320  as {size} bytes 
+000068e0: 616e 6420 6578 6365 6564 7320 7b73 6572  and exceeds {ser
+000068f0: 7669 6365 7d27 7320 6c69 6d69 7420 6f66  vice}'s limit of
+00006900: 207b 6d61 785f 7369 7a65 7d20 6279 7465   {max_size} byte
+00006910: 732e 0700 0000 0f55 706c 6f61 6465 7254  s......UploaderT
+00006920: 6162 7341 6c6c 0103 ffff ffff 0800 0000  absAll..........
+00006930: 0006 0000 0058 4669 6c65 2022 7b66 696c  .....XFile "{fil
+00006940: 655f 6e61 6d65 7d22 2068 6173 207b 7369  e_name}" has {si
+00006950: 7a65 7d20 7069 7865 6c73 2061 6e64 2065  ze} pixels and e
+00006960: 7863 6565 6473 207b 7365 7276 6963 657d  xceeds {service}
+00006970: 2773 206c 696d 6974 206f 6620 7b6d 6178  's limit of {max
+00006980: 5f73 697a 657d 2070 6978 656c 732e 0700  _size} pixels...
+00006990: 0000 0f55 706c 6f61 6465 7254 6162 7341  ...UploaderTabsA
+000069a0: 6c6c 0103 ffff ffff 0800 0000 0006 0000  ll..............
+000069b0: 0056 4669 6c65 2022 7b66 696c 655f 6e61  .VFile "{file_na
+000069c0: 6d65 7d22 2069 7320 6f66 2074 7970 6520  me}" is of type 
+000069d0: 227b 6669 6c65 5f74 7970 657d 222c 2077  "{file_type}", w
+000069e0: 6869 6368 207b 7365 7276 6963 657d 206d  hich {service} m
+000069f0: 6179 206e 6f74 2068 616e 646c 6520 636f  ay not handle co
+00006a00: 7272 6563 746c 792e 0700 0000 0f55 706c  rrectly......Upl
+00006a10: 6f61 6465 7254 6162 7341 6c6c 0103 ffff  oaderTabsAll....
+00006a20: ffff 0800 0000 0006 0000 0021 4669 6c65  ...........!File
+00006a30: 2022 7b66 696c 655f 6e61 6d65 7d22 2075   "{file_name}" u
+00006a40: 706c 6f61 6420 6661 696c 6564 2e07 0000  pload failed....
+00006a50: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
+00006a60: 6c01 03ff ffff ff08 0000 0000 0600 0000  l...............
+00006a70: 0f46 696c 6520 746f 6f20 6c61 7267 652e  .File too large.
+00006a80: 0700 0000 0f55 706c 6f61 6465 7254 6162  .....UploaderTab
+00006a90: 7341 6c6c 0103 ffff ffff 0800 0000 0006  sAll............
+00006aa0: 0000 0059 4669 6c65 207b 6669 6c65 5f6e  ...YFile {file_n
+00006ab0: 616d 657d 2068 6173 2061 6c72 6561 6479  ame} has already
+00006ac0: 2062 6565 6e20 7570 6c6f 6164 6564 2074   been uploaded t
+00006ad0: 6f20 7b73 6572 7669 6365 7d2e 2048 6f77  o {service}. How
+00006ae0: 2077 6f75 6c64 2079 6f75 206c 696b 6520   would you like 
+00006af0: 746f 2075 7064 6174 6520 6974 3f07 0000  to update it?...
+00006b00: 000f 5570 6c6f 6164 6572 5461 6273 416c  ..UploaderTabsAl
+00006b10: 6c01 03ff ffff ff08 0000 0000 0600 0000  l...............
+00006b20: 1849 6e63 6f6d 7061 7469 626c 6520 696d  .Incompatible im
+00006b30: 6167 6520 7479 7065 2e07 0000 000f 5570  age type......Up
+00006b40: 6c6f 6164 6572 5461 6273 416c 6c01 03ff  loaderTabsAll...
+00006b50: ffff ff08 0000 0000 0600 0000 064c 6f67  .............Log
+00006b60: 2069 6e07 0000 000f 5570 6c6f 6164 6572   in.....Uploader
+00006b70: 5461 6273 416c 6c01 03ff ffff ff08 0000  TabsAll.........
+00006b80: 0000 0600 0000 074c 6f67 206f 7574 0700  .......Log out..
+00006b90: 0000 0f55 706c 6f61 6465 7254 6162 7341  ...UploaderTabsA
+00006ba0: 6c6c 0103 ffff ffff 0800 0000 0006 0000  ll..............
+00006bb0: 0020 4c6f 6767 6564 2069 6e20 6173 207b  . Logged in as {
+00006bc0: 7573 6572 7d20 6f6e 207b 7365 7276 6963  user} on {servic
+00006bd0: 657d 0700 0000 0f55 706c 6f61 6465 7254  e}.....UploaderT
+00006be0: 6162 7341 6c6c 0103 ffff ffff 0800 0000  absAll..........
+00006bf0: 0006 0000 000f 4e6f 2069 6d61 6765 2075  ......No image u
+00006c00: 706c 6f61 6407 0000 000f 5570 6c6f 6164  pload.....Upload
+00006c10: 6572 5461 6273 416c 6c01 03ff ffff ff08  erTabsAll.......
+00006c20: 0000 0000 0600 0000 084e 6f20 6d61 7463  .........No matc
+00006c30: 6807 0000 000f 5570 6c6f 6164 6572 5461  h.....UploaderTa
+00006c40: 6273 416c 6c01 03ff ffff ff08 0000 0000  bsAll...........
+00006c50: 0600 0000 1a4e 6f74 206c 6f67 6765 6420  .....Not logged 
+00006c60: 696e 2074 6f20 7b73 6572 7669 6365 7d07  in to {service}.
+00006c70: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
+00006c80: 416c 6c01 03ff ffff ff08 0000 0000 0600  All.............
+00006c90: 0000 1250 686f 7469 6e69 3a20 6175 7468  ...Photini: auth
+00006ca0: 6f72 6973 6507 0000 000f 5570 6c6f 6164  orise.....Upload
+00006cb0: 6572 5461 6273 416c 6c01 03ff ffff ff08  erTabsAll.......
+00006cc0: 0000 0000 0600 0000 1a50 686f 7469 6e69  .........Photini
+00006cd0: 3a20 696e 636f 6d70 6174 6962 6c65 2074  : incompatible t
+00006ce0: 7970 6507 0000 000f 5570 6c6f 6164 6572  ype.....Uploader
+00006cf0: 5461 6273 416c 6c01 03ff ffff ff08 0000  TabsAll.........
+00006d00: 0000 0600 0000 1250 686f 7469 6e69 3a20  .......Photini: 
+00006d10: 746f 6f20 6c61 7267 6507 0000 000f 5570  too large.....Up
+00006d20: 6c6f 6164 6572 5461 6273 416c 6c01 03ff  loaderTabsAll...
+00006d30: ffff ff08 0000 0000 0600 0000 1550 686f  .............Pho
+00006d40: 7469 6e69 3a20 7570 6c6f 6164 2065 7272  tini: upload err
+00006d50: 6f72 0700 0000 0f55 706c 6f61 6465 7254  or.....UploaderT
+00006d60: 6162 7341 6c6c 0103 ffff ffff 0800 0000  absAll..........
+00006d70: 0006 0000 001b 5068 6f74 696e 693a 2075  ......Photini: u
+00006d80: 706c 6f61 6420 696e 2070 726f 6772 6573  pload in progres
+00006d90: 7307 0000 000f 5570 6c6f 6164 6572 5461  s.....UploaderTa
+00006da0: 6273 416c 6c01 03ff ffff ff08 0000 0000  bsAll...........
+00006db0: 0600 0000 4d50 6c65 6173 6520 7573 6520  ....MPlease use 
+00006dc0: 796f 7572 2077 6562 2062 726f 7773 6572  your web browser
+00006dd0: 2074 6f20 6175 7468 6f72 6973 6520 5068   to authorise Ph
+00006de0: 6f74 696e 692c 2061 6e64 2074 6865 6e20  otini, and then 
+00006df0: 636c 6f73 6520 7468 6973 2064 6961 6c6f  close this dialo
+00006e00: 672e 0700 0000 0f55 706c 6f61 6465 7254  g......UploaderT
+00006e10: 6162 7341 6c6c 0103 ffff ffff 0800 0000  absAll..........
+00006e20: 0006 0000 0008 5072 6f67 7265 7373 0700  ......Progress..
+00006e30: 0000 0f55 706c 6f61 6465 7254 6162 7341  ...UploaderTabsA
+00006e40: 6c6c 0103 ffff ffff 0800 0000 0006 0000  ll..............
+00006e50: 000d 5265 706c 6163 6520 696d 6167 6507  ..Replace image.
+00006e60: 0000 000f 5570 6c6f 6164 6572 5461 6273  ....UploaderTabs
+00006e70: 416c 6c01 03ff ffff ff08 0000 0000 0600  All.............
+00006e80: 0000 0d52 6570 6c61 6365 2070 686f 746f  ...Replace photo
+00006e90: 0700 0000 0f55 706c 6f61 6465 7254 6162  .....UploaderTab
+00006ea0: 7341 6c6c 0103 ffff ffff 0800 0000 0006  sAll............
+00006eb0: 0000 000f 5365 6c65 6374 2061 6e20 696d  ....Select an im
+00006ec0: 6167 6507 0000 000f 5570 6c6f 6164 6572  age.....Uploader
+00006ed0: 5461 6273 416c 6c01 03ff ffff ff08 0000  TabsAll.........
+00006ee0: 0000 0600 0000 0453 6b69 7007 0000 000f  .......Skip.....
+00006ef0: 5570 6c6f 6164 6572 5461 6273 416c 6c01  UploaderTabsAll.
+00006f00: 03ff ffff ff08 0000 0000 0600 0000 0c53  ...............S
+00006f10: 7461 7274 2075 706c 6f61 6407 0000 000f  tart upload.....
+00006f20: 5570 6c6f 6164 6572 5461 6273 416c 6c01  UploaderTabsAll.
+00006f30: 03ff ffff ff08 0000 0000 0600 0000 0b53  ...............S
+00006f40: 746f 7020 7570 6c6f 6164 0700 0000 0f55  top upload.....U
+00006f50: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
+00006f60: ffff ffff 0800 0000 0006 0000 0013 5570  ..............Up
+00006f70: 6c6f 6164 2061 7320 6e65 7720 7068 6f74  load as new phot
+00006f80: 6f07 0000 000f 5570 6c6f 6164 6572 5461  o.....UploaderTa
+00006f90: 6273 416c 6c01 03ff ffff ff08 0000 0000  bsAll...........
+00006fa0: 0600 0000 2555 706c 6f61 6420 746f 207b  ....%Upload to {
+00006fb0: 7365 7276 6963 657d 2068 6173 206e 6f74  service} has not
+00006fc0: 2066 696e 6973 6865 642e 0700 0000 0f55   finished......U
+00006fd0: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
+00006fe0: ffff ffff 0800 0000 0006 0000 0033 5768  .............3Wh
+00006ff0: 6963 6820 696d 6167 6520 6669 6c65 206d  ich image file m
+00007000: 6174 6368 6573 2074 6869 7320 7069 6374  atches this pict
+00007010: 7572 6520 6f6e 207b 7365 7276 6963 657d  ure on {service}
+00007020: 3f07 0000 000f 5570 6c6f 6164 6572 5461  ?.....UploaderTa
+00007030: 6273 416c 6c01 03ff ffff ff08 0000 0000  bsAll...........
+00007040: 0600 0000 2557 6f75 6c64 2079 6f75 206c  ....%Would you l
+00007050: 696b 6520 746f 2063 6f6e 7665 7274 2069  ike to convert i
+00007060: 7420 746f 204a 5045 473f 0700 0000 0f55  t to JPEG?.....U
+00007070: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
+00007080: ffff ffff 0800 0000 0006 0000 001c 576f  ..............Wo
+00007090: 756c 6420 796f 7520 6c69 6b65 2074 6f20  uld you like to 
+000070a0: 7265 7369 7a65 2069 743f 0700 0000 0f55  resize it?.....U
+000070b0: 706c 6f61 6465 7254 6162 7341 6c6c 0103  ploaderTabsAll..
+000070c0: ffff ffff 0800 0000 0006 0000 0023 576f  .............#Wo
+000070d0: 756c 6420 796f 7520 6c69 6b65 2074 6f20  uld you like to 
+000070e0: 7570 6c6f 6164 2069 7420 616e 7977 6179  upload it anyway
+000070f0: 3f07 0000 000f 5570 6c6f 6164 6572 5461  ?.....UploaderTa
+00007100: 6273 416c 6c01 03ff ffff ff08 0000 0000  bsAll...........
+00007110: 0600 0000 2659 6f75 206d 6179 206e 6f77  ....&You may now
+00007120: 2063 6c6f 7365 2074 6869 7320 6272 6f77   close this brow
+00007130: 7365 7220 7769 6e64 6f77 2e07 0000 000f  ser window......
+00007140: 5570 6c6f 6164 6572 5461 6273 416c 6c01  UploaderTabsAll.
+00007150: 03ff ffff ff08 0000 0000 0600 0000 113c  ...............<
+00007160: 6d75 6c74 6970 6c65 2076 616c 7565 733e  multiple values>
+00007170: 0700 0000 0757 6964 6765 7473 0103 ffff  .....Widgets....
+00007180: ffff 0800 0000 0006 0000 000a 3c6d 756c  ............<mul
+00007190: 7469 706c 653e 0700 0000 0757 6964 6765  tiple>.....Widge
+000071a0: 7473 0103 ffff ffff 0800 0000 0006 0000  ts..............
+000071b0: 0005 3c6e 6577 3e07 0000 0007 5769 6467  ..<new>.....Widg
+000071c0: 6574 7301 8800 0000 0201 01              ets........
```

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.es.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.es.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.fr.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.fr.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.it.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.it.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.ko.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.ko.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.nb.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.nb.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/lang/photini.pl.qm` & `Photini-2023.5.0/src/photini/data/lang/photini.pl.qm`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/linux/photini.desktop` & `Photini-2023.5.0/src/photini/data/linux/photini.desktop`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/map_pin_grey.png` & `Photini-2023.5.0/src/photini/data/map_pin_grey.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/map_pin_red.png` & `Photini-2023.5.0/src/photini/data/map_pin_red.png`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/mapboxmap/script.js` & `Photini-2023.5.0/src/photini/data/mapboxmap/script.js`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/data/windows/install_shortcuts.vbs` & `Photini-2023.5.0/src/photini/data/windows/install_shortcuts.vbs`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/descriptive.py` & `Photini-2023.5.0/src/photini/descriptive.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/editor.py` & `Photini-2023.5.0/src/photini/editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,14 +537,15 @@
         app.installTranslator(translator)
         translator = QtCore.QTranslator(parent=app)
     # parse remaining arguments
     version = 'Photini ' + __version__ + ', build ' + build
     version += '\n  Python ' + sys.version
     version += '\n  ' + exiv2_version
     version += '\n  ' + qt_version
+    version += ', locale ' + locale.bcp47Name()
     if spelling_version:
         version += '\n  ' + spelling_version
     if ffmpeg_version:
         version += '\n  ' + ffmpeg_version
     version += '\n  available styles: {}'.format(
         ', '.join(QtWidgets.QStyleFactory.keys()))
     version += '\n  using style: {}'.format(
```

### Comparing `Photini-2023.4.0.2/src/photini/editsettings.py` & `Photini-2023.5.0/src/photini/editsettings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# -*- coding: utf-8 -*-
 #  Photini - a simple photo metadata editor.
 #  http://github.com/jim-easterbrook/Photini
-#  Copyright (C) 2012-22  Jim Easterbrook  jim@jim-easterbrook.me.uk
+#  Copyright (C) 2012-23  Jim Easterbrook  jim@jim-easterbrook.me.uk
 #
 #  This program is free software: you can redistribute it and/or
 #  modify it under the terms of the GNU General Public License as
 #  published by the Free Software Foundation, either version 3 of the
 #  License, or (at your option) any later version.
 #
 #  This program is distributed in the hope that it will be useful,
@@ -25,15 +24,16 @@
 logger = logging.getLogger(__name__)
 translate = QtCore.QCoreApplication.translate
 
 
 class EditSettings(QtWidgets.QDialog):
     def __init__(self, *arg, **kw):
         super(EditSettings, self).__init__(*arg, **kw)
-        self.config_store = QtWidgets.QApplication.instance().config_store
+        self.app = QtWidgets.QApplication.instance()
+        self.config_store = self.app.config_store
         self.setWindowTitle(translate('EditSettings', 'Photini: settings'))
         self.setLayout(QtWidgets.QVBoxLayout())
         # main dialog area
         scroll_area = QtWidgets.QScrollArea()
         self.layout().addWidget(scroll_area)
         panel = QtWidgets.QWidget()
         layout = FormLayout()
@@ -125,14 +125,22 @@
         self.time_taken.setChecked(keep_time=='taken')
         panel.layout().addRow('', self.time_taken)
         button = QtWidgets.QRadioButton(
             translate('EditSettings', 'Set to when file is saved'))
         button_group.addButton(button)
         button.setChecked(keep_time=='now')
         panel.layout().addRow('', button)
+        # import GPX altitude
+        if self.app.gpx_importer:
+            self.gpx_altitude = QtWidgets.QCheckBox(
+                translate('EditSettings', 'set altitude'))
+            self.gpx_altitude.setChecked(
+                self.config_store.get('map', 'gpx_altitude', True))
+            panel.layout().addRow(
+                translate('EditSettings', 'GPX importer'), self.gpx_altitude)
         # add panel to scroll area after its size is known
         scroll_area.setWidget(panel)
 
     @QtSlot()
     @catch_all
     def new_write_if(self):
         if_mode = self.write_if.isChecked()
@@ -168,8 +176,11 @@
         if self.keep_time.isChecked():
             keep_time = 'keep'
         elif self.time_taken.isChecked():
             keep_time = 'taken'
         else:
             keep_time = 'now'
         self.config_store.set('files', 'preserve_timestamps', keep_time)
+        if self.app.gpx_importer:
+            self.config_store.set(
+                'map', 'gpx_altitude', self.gpx_altitude.isChecked())
         return self.accept()
```

### Comparing `Photini-2023.4.0.2/src/photini/exiv2.py` & `Photini-2023.5.0/src/photini/exiv2.py`

 * *Files 2% similar despite different names*

```diff
@@ -284,20 +284,35 @@
             logger.exception(ex)
             return None
 
     def set_exif_thumbnail_from_buffer(self, buffer):
         thumb = exiv2.ExifThumb(self._exifData)
         thumb.setJpegThumbnail(buffer)
 
-    def get_exif_comment(self, tag, value):
+    def get_exif_comment(self, tag, datum):
+        type_id = datum.typeId()
+        if type_id == exiv2.TypeId.undefined:
+            value = datum.value(exiv2.TypeId.comment)
+            data = memoryview(value.data())
+            charset = value.charsetId()
+        else:
+            value = datum.value(exiv2.TypeId.undefined)
+            data = bytearray(len(value))
+            value.copy(data, exiv2.ByteOrder.invalidByteOrder)
+            if data[:5] == b'ASCII':
+                charset = exiv2.CharsetId.ascii
+            elif data[:3] == b'JIS':
+                charset = exiv2.CharsetId.jis
+            elif data[:7] == b'UNICODE':
+                charset = exiv2.CharsetId.unicode
+            else:
+                charset = exiv2.CharsetId.undefined
         # ignore Exiv2's comment decoding, Python is better at unicode
-        data = memoryview(value.data())
         if not any(data):
             return None
-        charset = value.charsetId()
         raw_value = data[8:]
         if charset == exiv2.CharsetId.ascii:
             encodings = ('ascii',)
         elif charset == exiv2.CharsetId.jis:
             # Exif standard says JIS X208-1990, but doesn't say what encoding
             encodings = ('iso2022_jp', 'euc_jp', 'shift_jis', 'cp932')
         elif charset == exiv2.CharsetId.unicode:
@@ -348,20 +363,19 @@
                    'Exif.Image.XPTitle', 'Exif.Image.XPComment',
                    'Exif.Image.XPAuthor', 'Exif.Image.XPKeywords',
                    'Exif.Image.XPSubject', 'Exif.NikonLd1.LensIDNumber',
                    'Exif.NikonLd2.LensIDNumber',
                    'Exif.NikonLd3.LensIDNumber', 'Exif.Pentax.ModelID'):
             # use Exiv2's "interpreted string"
             return datum._print()
-        type_id = datum.typeId()
         if tag in ('Exif.Photo.UserComment',
                    'Exif.GPSInfo.GPSProcessingMethod'):
-            value = datum.value(exiv2.TypeId.comment)
-            return self.get_exif_comment(tag, value)
+            return self.get_exif_comment(tag, datum)
         value = datum.value()
+        type_id = datum.typeId()
         if type_id == exiv2.TypeId.asciiString:
             return value.toString()
         if type_id in (exiv2.TypeId.unsignedByte, exiv2.TypeId.undefined):
             result = bytearray(value.size())
             value.copy(result, exiv2.ByteOrder.invalidByteOrder)
             return result
         if type_id not in (
@@ -530,14 +544,17 @@
         type_id = key.defaultTypeId()
         if type_id == exiv2.TypeId.unsignedByte:
             value = exiv2.DataValue(
                 value, exiv2.ByteOrder.invalidByteOrder, type_id)
         elif type_id == exiv2.TypeId.asciiString:
             value = exiv2.AsciiValue(value)
         elif type_id == exiv2.TypeId.comment:
+            # only comment value Photini writes is GPS processing method
+            # which is certain to be ASCII
+            value = 'charset=Ascii ' + value
             value = exiv2.CommentValue(value)
         elif type_id == exiv2.TypeId.unsignedShort:
             value = exiv2.UShortValue(value)
         elif type_id == exiv2.TypeId.unsignedLong:
             value = exiv2.ULongValue(value)
         elif type_id == exiv2.TypeId.unsignedRational:
             if isinstance(value, (list, tuple)):
```

### Comparing `Photini-2023.4.0.2/src/photini/ffmpeg.py` & `Photini-2023.5.0/src/photini/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/flickr.py` & `Photini-2023.5.0/src/photini/flickr.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/googlemap.py` & `Photini-2023.5.0/src/photini/googlemap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/googlephotos.py` & `Photini-2023.5.0/src/photini/googlephotos.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/gpximporter.py` & `Photini-2023.5.0/src/photini/gpximporter.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/imagelist.py` & `Photini-2023.5.0/src/photini/imagelist.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/importer.py` & `Photini-2023.5.0/src/photini/importer.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/ipernity.py` & `Photini-2023.5.0/src/photini/ipernity.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/loggerwindow.py` & `Photini-2023.5.0/src/photini/loggerwindow.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/mapboxmap.py` & `Photini-2023.5.0/src/photini/mapboxmap.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/metadata.py` & `Photini-2023.5.0/src/photini/metadata.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/ownership.py` & `Photini-2023.5.0/src/photini/ownership.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/photinimap.py` & `Photini-2023.5.0/src/photini/photinimap.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,16 @@
         self.widgets['latlon'].new_value.connect(self.new_latlon)
         left_side.addWidget(self.widgets['latlon'], 0, 1)
         # altitude
         label = QtWidgets.QLabel(translate('PhotiniMap', 'Altitude'))
         label.setAlignment(Qt.AlignmentFlag.AlignRight)
         left_side.addWidget(label, 1, 0)
         self.widgets['alt'] = DoubleSpinBox('exif:GPSAltitude')
-        self.widgets['alt'].set_suffix(' m')
+        self.widgets['alt'].set_suffix(
+            translate('PhotiniMap', ' m', 'metres altitude'))
         self.widgets['alt'].new_value.connect(self.new_value)
         left_side.addWidget(self.widgets['alt'], 1, 1)
         if hasattr(self.geocoder, 'get_altitude'):
             self.widgets['get_altitude'] = QtWidgets.QPushButton(
                 translate('PhotiniMap', 'Get altitude from map'))
             self.widgets['get_altitude'].clicked.connect(self.get_altitude)
             left_side.addWidget(self.widgets['get_altitude'], 2, 1)
@@ -532,14 +533,15 @@
         self.widgets['clear_gpx'].setEnabled(
             bool(self.app.gpx_importer.display_points))
 
     @QtSlot()
     @catch_all
     def set_from_gpx(self):
         selected_images = self.app.image_list.get_selected_images()
+        set_altitude = self.app.config_store.get('map', 'gpx_altitude', True)
         changed = False
         for image in selected_images:
             if not image.metadata.date_taken:
                 continue
             utc_time = image.metadata.date_taken.to_utc()
             utc_time = utc_time.replace(tzinfo=timezone.utc)
             candidates = self.app.gpx_importer.get_locations_at(utc_time)
@@ -548,15 +550,18 @@
             nearest = candidates[0]
             for c in candidates[1:]:
                 if abs(c.time - utc_time) < abs(nearest.time - utc_time):
                     nearest = c
             gps = dict(image.metadata.gps_info)
             gps['exif:GPSLatitude'] = nearest.latitude
             gps['exif:GPSLongitude'] = nearest.longitude
-            gps['exif:GPSAltitude'] = nearest.elevation
+            if set_altitude and nearest.elevation is not None:
+                gps['exif:GPSAltitude'] = round(nearest.elevation, 1)
+            else:
+                gps['exif:GPSAltitude'] = None
             gps['method'] = 'GPS'
             image.metadata.gps_info = gps
             changed = True
         if changed:
             self.update_display(selected_images)
 
     @QtSlot()
@@ -630,15 +635,15 @@
 
     @catch_all
     def marker_click(self, marker_id):
         self.app.image_list.select_images(self.marker_info[marker_id]['images'])
 
     @catch_all
     def marker_drag(self, lat, lng):
-        self.widgets['latlon'].set_value('{:.6f}, {:.6f}'.format(lat, lng))
+        self.widgets['latlon'].set_value((lat, lng))
 
     @catch_all
     def marker_drag_end(self, lat, lng, marker_id):
         info = self.marker_info[marker_id]
         for image in info['images']:
             gps = dict(image.metadata.gps_info)
             gps['exif:GPSLatitude'] = lat
```

### Comparing `Photini-2023.4.0.2/src/photini/pixelfed.py` & `Photini-2023.5.0/src/photini/pixelfed.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/pyqt.py` & `Photini-2023.5.0/src/photini/pyqt.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/regions.py` & `Photini-2023.5.0/src/photini/regions.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/scripts.py` & `Photini-2023.5.0/src/photini/scripts.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ##  along with this program.  If not, see
 ##  <http://www.gnu.org/licenses/>.
 
 import importlib
 import logging
 from optparse import OptionParser
 import os
+import platform
 import site
 import subprocess
 import sys
 
 import pkg_resources
 
 from photini.configstore import BaseConfigStore
@@ -34,15 +35,18 @@
 
 def configure(argv=None):
     # get config
     config = BaseConfigStore('editor')
     install_extras = []
     ## Qt library choice is complicated
     print('Which Qt package would you like to use?')
-    packages = ['PyQt5', 'PyQt6', 'PySide2', 'PySide6']
+    packages = ['PyQt5', 'PySide2']
+    if platform.system() != 'Windows' or platform.release() not in ('7', '8'):
+        # Qt6 is not available for Windows < 10
+        packages += ['PyQt6', 'PySide6']
     # get installed Qt packages
     installed = []
     choices = {}
     default = None
     n = 0
     for package in packages:
         # run separate python interpreter for each to avoid interactions
```

### Comparing `Photini-2023.4.0.2/src/photini/spelling.py` & `Photini-2023.5.0/src/photini/spelling.py`

 * *Files identical despite different names*

### Comparing `Photini-2023.4.0.2/src/photini/technical.py` & `Photini-2023.5.0/src/photini/technical.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,33 +310,38 @@
         return QtGui.QValidator.State.Invalid, text, pos
 
     @catch_all
     def valueFromText(self, text):
         if not text.strip():
             return 0
         hours, sep, minutes = text.partition(':')
-        hours = int(hours)
+        hours, OK = self.locale().toInt(hours)
+        if not OK:
+            return 0
         if minutes:
+            minutes, OK = self.locale().toInt(minutes)
+            if not OK:
+                minutes = 0
             minutes = int(15.0 * round(float(minutes) / 15.0))
             if hours < 0:
                 minutes = -minutes
         else:
             minutes = 0
         return (hours * 60) + minutes
 
     @catch_all
     def textFromValue(self, value):
         if value is None:
             return ''
         if value < 0:
-            sign = '-'
+            sign = self.locale().negativeSign()
             value = -value
         else:
-            sign = '+'
-        return '{}{:02d}:{:02d}'.format(sign, value // 60, value % 60)
+            sign = self.locale().positiveSign()
+        return sign + QtCore.QTime(value // 60, value % 60).toString('hh:mm')
 
 
 class PrecisionSlider(Slider):
     value_changed = QtSignal(int)
 
     def __init__(self, *arg, **kw):
         super(PrecisionSlider, self).__init__(*arg, **kw)
@@ -430,15 +435,21 @@
         self.app = QtWidgets.QApplication.instance()
         self.setLayout(QtWidgets.QHBoxLayout())
         self.layout().setContentsMargins(0, 0, 0, 0)
         spacing = self.layout().spacing()
         self.layout().setSpacing(0)
         # offset value
         self.offset = QtWidgets.QTimeEdit()
-        self.offset.setDisplayFormat("'h:'hh 'm:'mm 's:'ss")
+        self.offset.setDisplayFormat("'{}:'HH' {}:'mm' {}:'ss".format(
+            translate('TechnicalTab', 'h',
+                      'single letter abbreviation of "hours"'),
+            translate('TechnicalTab', 'm',
+                      'single letter abbreviation of "minutes"'),
+            translate('TechnicalTab', 's',
+                      'single letter abbreviation of "seconds"')))
         self.layout().addWidget(self.offset)
         self.layout().addSpacing(spacing)
         # time zone
         self.time_zone = TimeZoneWidget('time_zone')
         self.time_zone.set_value(None)
         self.layout().addWidget(self.time_zone)
         self.layout().addSpacing(spacing)
@@ -597,18 +608,20 @@
                 ('max_fl', translate('TechnicalTab', 'Maximum focal length')),
                 ('max_fl_fn',
                  translate('TechnicalTab', 'Aperture at max. focal length')),
                 ):
             self.lens_spec[key] = DoubleSpinBox(key)
             self.lens_spec[key].setMinimum(0.0)
             if key.endswith('_fn'):
-                self.lens_spec[key].set_prefix('ƒ/')
+                self.lens_spec[key].set_prefix(translate(
+                    'TechnicalTab', 'ƒ/', 'lens aperture'))
             else:
                 self.lens_spec[key].setSingleStep(1.0)
-                self.lens_spec[key].set_suffix(' mm')
+                self.lens_spec[key].set_suffix(translate(
+                    'TechnicalTab', ' mm', 'millimetres focal length'))
             self.panel.layout().addRow(label, self.lens_spec[key])
 
     def get_value(self):
         lens_model = super(NewLensDialog, self).get_value()
         min_fl = self.lens_spec['min_fl'].get_value() or 0
         max_fl = self.lens_spec['max_fl'].get_value() or min_fl
         min_fl_fn = self.lens_spec['min_fl_fn'].get_value() or 0
@@ -713,29 +726,32 @@
             width_for_text(self.widgets['lens_model'], 'x' * 30))
         self.widgets['lens_model'].new_value.connect(self._new_value)
         other_group.layout().addRow(translate('TechnicalTab', 'Lens model'),
                                     self.widgets['lens_model'])
         # focal length
         self.widgets['focal_length'] = DoubleSpinBox('focal_length')
         self.widgets['focal_length'].setMinimum(0.0)
-        self.widgets['focal_length'].set_suffix(' mm')
+        self.widgets['focal_length'].set_suffix(translate(
+            'TechnicalTab', ' mm', 'millimetres focal length'))
         self.widgets['focal_length'].new_value.connect(self._new_value)
         other_group.layout().addRow(translate('TechnicalTab', 'Focal length'),
                                     self.widgets['focal_length'])
         # 35mm equivalent focal length
         self.widgets['focal_length_35'] = IntSpinBox('focal_length_35')
         self.widgets['focal_length_35'].setMinimum(0)
-        self.widgets['focal_length_35'].set_suffix(' mm')
+        self.widgets['focal_length_35'].set_suffix(translate(
+            'TechnicalTab', ' mm', 'millimetres focal length'))
         self.widgets['focal_length_35'].new_value.connect(self._new_value)
         other_group.layout().addRow(translate('TechnicalTab', '35mm equiv'),
                                     self.widgets['focal_length_35'])
         # aperture
         self.widgets['aperture'] = DoubleSpinBox('aperture')
         self.widgets['aperture'].setMinimum(0.0)
-        self.widgets['aperture'].set_prefix('ƒ/')
+        self.widgets['aperture'].set_prefix(translate(
+            'TechnicalTab', 'ƒ/', 'lens aperture'))
         self.widgets['aperture'].new_value.connect(self._new_value)
         other_group.layout().addRow(translate('TechnicalTab', 'Aperture'),
                                     self.widgets['aperture'])
         self.layout().addWidget(other_group, stretch=1)
         # disable until an image is selected
         self.setEnabled(False)
```

### Comparing `Photini-2023.4.0.2/src/photini/types.py` & `Photini-2023.5.0/src/photini/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,15 @@
             tz_offset = None
         # extract sub seconds
         if not sub_sec_string:
             match = cls._subsec_re.match(unparsed)
             if match:
                 unparsed, sub_sec_string = match.groups()
         if sub_sec_string:
+            sub_sec_string = sub_sec_string.strip()
             microsecond = int((sub_sec_string + '000000')[:6])
         else:
             microsecond = 0
             precision = 6
         # extract time
         match = cls._time_re.match(unparsed)
         if match:
@@ -293,15 +294,15 @@
     _fmt_elements = ('%Y', '-%m', '-%d', 'T%H', ':%M', ':%S', '.%f')
 
     def to_ISO_8601(self, precision=None, time_zone=True):
         if precision is None:
             precision = self['precision']
         fmt = ''.join(self._fmt_elements[:precision])
         datetime_string = self['datetime'].strftime(fmt)
-        if precision > 6:
+        if precision > 6 and datetime_string[-3:] == '000':
             # truncate subsecond to 3 digits
             datetime_string = datetime_string[:-3]
         if precision > 3 and time_zone and self['tz_offset'] is not None:
             # add time zone
             minutes = self['tz_offset']
             if minutes >= 0:
                 datetime_string += '+'
@@ -865,22 +866,24 @@
     # https://developer.adobe.com/xmp/docs/XMPNamespaces/XMPDataTypes/#language-alternative
 
     DEFAULT = 'x-default'
 
     def __init__(self, value=None, default_lang=None, strip=True):
         if isinstance(value, str):
             value = {self.DEFAULT: value}
+        elif isinstance(value, MD_LangAlt):
+            default_lang = default_lang or value.default_lang
         value = value or {}
         if strip:
             value = dict((k, v.strip()) for (k, v) in value.items())
         value = dict((k, v) for (k, v) in value.items() if v)
         if default_lang:
             self.default_lang = default_lang
-        elif isinstance(value, MD_LangAlt):
-            self.default_lang = value.default_lang
+            if self.DEFAULT in value and self.default_lang not in value:
+                value[self.default_lang] = value[self.DEFAULT]
         else:
             self.default_lang = self.identify_default(value)
         if self.default_lang != self.DEFAULT and self.DEFAULT in value:
             del value[self.DEFAULT]
         super(MD_LangAlt, self).__init__(value)
 
     @classmethod
@@ -1363,22 +1366,30 @@
                     pstv)
         degrees, minutes, seconds = numbers
         degrees = int(degrees)
         minutes = float(minutes + (seconds / 60))
         return '{:d},{:.8f}'.format(degrees, minutes), pstv
 
     def contains(self, this, other):
-        return abs(float(other) - float(this)) < 0.0000001
+        if other is None:
+            return False
+        return abs(float(other) - float(this)) < 0.0000005
 
     def compact_form(self):
         return round(float(self), 6)
 
     def __str__(self):
         return '{:.6f}'.format(float(self))
 
+    def __eq__(self, other):
+        return self.contains(self, other)
+
+    def __ne__(self, other):
+        return not self.contains(self, other)
+
 
 class MD_Latitude(MD_Coordinate):
     def to_exif(self):
         numbers, pstv = self.to_exif_part()
         return numbers, ('S', 'N')[pstv]
 
     def to_xmp(self):
@@ -1484,14 +1495,23 @@
                 result.append(self[k] and self[k].to_xmp())
         return result
 
     def __bool__(self):
         return any(self[k] for k in ('exif:GPSLatitude', 'exif:GPSLongitude',
                                      'exif:GPSAltitude'))
 
+    def __eq__(self, other):
+        return not self.__ne__(other)
+
+    def __ne__(self, other):
+        if not isinstance(other, MD_GPSinfo):
+            other = MD_GPSinfo(other)
+        return any(self[k] != other[k] for k in (
+            'exif:GPSLatitude', 'exif:GPSLongitude', 'exif:GPSAltitude'))
+
 
 class MD_Aperture(MD_Rational):
     # store FNumber and APEX aperture as fractions
     # only FNumber is presented to the user, either is computed if missing
     @classmethod
     def from_exiv2(cls, file_value, tag):
         if not any(file_value):
```

### Comparing `Photini-2023.4.0.2/src/photini/uploader.py` & `Photini-2023.5.0/src/photini/uploader.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,15 +380,14 @@
 class AlbumList(QtWidgets.QWidget):
     def __init__(self, *arg, max_selected=0, **kw):
         super(AlbumList, self).__init__(*arg, **kw)
         self.setLayout(QtWidgets.QVBoxLayout())
         self.layout().setSpacing(0)
         self.layout().setSizeConstraint(
             QtWidgets.QLayout.SizeConstraint.SetMinAndMaxSize)
-        self.setAutoFillBackground(False)
         self.album_widgets = []
         self.max_selected = max_selected
         self.checked_widgets = []
 
     def add_album(self, album, index=-1):
         widget = QtWidgets.QCheckBox(album['title'].replace('&', '&&'))
         if album['description']:
@@ -488,15 +487,14 @@
         group = QtWidgets.QGroupBox()
         group.setMinimumWidth(width_for_text(group, 'x' * 23))
         group.setLayout(QtWidgets.QVBoxLayout())
         label = label or translate('UploaderTabsAll', 'Add to albums')
         group.layout().addWidget(QtWidgets.QLabel(label))
         scrollarea = QtWidgets.QScrollArea()
         scrollarea.setFrameStyle(scrollarea.Shape.NoFrame)
-        scrollarea.setStyleSheet("QScrollArea {background-color: transparent}")
         self.widget['albums'] = AlbumList(max_selected=max_selected)
         scrollarea.setWidget(self.widget['albums'])
         group.layout().addWidget(scrollarea)
         column.addWidget(group, 0, 0)
         return column
 
     @QtSlot()
```

### Comparing `Photini-2023.4.0.2/src/photini/widgets.py` & `Photini-2023.5.0/src/photini/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 ##  along with this program.  If not, see
 ##  <http://www.gnu.org/licenses/>.
 
 import logging
 import re
 
 from photini.pyqt import *
+from photini.pyqt import qt_version_info
 from photini.types import MD_LangAlt
 
 logger = logging.getLogger(__name__)
 translate = QtCore.QCoreApplication.translate
 
 
 class WidgetMixin(object):
@@ -377,15 +378,19 @@
             self.setPlaceholderText('')
         if not value:
             self.clear()
         else:
             self.setPlainText(str(value))
 
     def get_value(self):
-        return self.toPlainText()
+        if qt_version_info < (5, 9):
+            return self.toPlainText()
+        value = self.document().toRawText()
+        value = value.replace('\u2029', '\n')
+        return value
 
     def set_multiple(self, choices=[]):
         self._is_multiple = True
         self.choices = list(choices)
         self.setPlaceholderText(self.multiple_values)
         self.clear()
 
@@ -829,18 +834,18 @@
         self.lat_validator = QtGui.QDoubleValidator(
             -90.0, 90.0, 20, parent=self)
         self.lng_validator = QtGui.QDoubleValidator(
             -180.0, 180.0, 20, parent=self)
         self.setButtonSymbols(self.ButtonSymbols.NoButtons)
         self.label = QtWidgets.QLabel(translate('LatLongDisplay', 'Lat, long'))
         self.label.setAlignment(Qt.AlignmentFlag.AlignRight)
-        self.setFixedWidth(width_for_text(self, '8' * 23))
+        self.setFixedWidth(width_for_text(self, '8' * 22))
         self.setToolTip('<p>{}</p>'.format(translate(
             'LatLongDisplay', 'Latitude and longitude (in degrees) as two'
-            ' decimal numbers separated by a comma.')))
+            ' decimal numbers separated by a space.')))
 
     @catch_all
     def focusOutEvent(self, event):
         self.emit_value()
         super(LatLongDisplay, self).focusOutEvent(event)
 
     @catch_all
@@ -870,67 +875,78 @@
     def stepEnabled(self):
         return self.StepEnabledFlag.StepNone
 
     @catch_all
     def validate(self, text, pos):
         if not text:
             return QtGui.QValidator.State.Acceptable, text, pos
-        parts = [x.strip() for x in text.split(',')]
+        parts = text.split()
         if len(parts) > 2:
             return QtGui.QValidator.State.Invalid, text, pos
         result = self.lat_validator.validate(parts[0], pos)[0]
         if result != QtGui.QValidator.State.Invalid and len(parts) > 1:
             lng_result = self.lng_validator.validate(parts[1], pos)[0]
             if lng_result == QtGui.QValidator.State.Invalid:
                 result = lng_result
             elif result == QtGui.QValidator.State.Acceptable:
                 result = lng_result
         return result, text, pos
 
     @catch_all
     def fixup(self, value):
-        value = value.split(',')
-        if len(value) != 2 or not all(value):
+        value = self.text_to_value(value)
+        if len(value) != 2:
             return
-        value = [float(x) for x in value]
         value[0] = min(max(value[0], -90.0), 90.0)
         value[1] = ((value[1] + 180.0) % 360.0) - 180.0
-        self.lineEdit().setText('{:f}, {:f}'.format(*value))
+        self.lineEdit().setText(self.value_to_text(value))
+
+    def text_to_value(self, text):
+        value = [self.locale().toDouble(x) for x in text.split()]
+        if not all(x[1] for x in value):
+            # float conversion failed
+            return []
+        return [x[0] for x in value]
+
+    def value_to_text(self, value):
+        return ' '.join(self.locale().toString(float(x), 'f', 6) for x in value)
 
     def get_value(self):
-        value = self.text() or None
-        if value and self.hasAcceptableInput():
-            value = [float(x) for x in value.split(',')]
+        value = self.text_to_value(self.text())
+        if len(value) != 2:
+            return None
         return value
 
     def get_value_dict(self):
         if self.is_multiple():
             return {}
         return dict(zip(self._key, self.get_value() or (None, None)))
 
     def set_value(self, value):
         self.set_not_multiple()
         if not value:
             self.clear()
         else:
-            self.lineEdit().setText(str(value))
+            if not isinstance(value, str):
+                value = self.value_to_text(value)
+            self.lineEdit().setText(value)
 
     def set_value_list(self, values):
         choices = set()
         if not values:
             self.setEnabled(False)
             self.set_value(None)
             return
         self.setEnabled(True)
         for value in values:
             if value:
                 lat = value['exif:GPSLatitude']
                 lon = value['exif:GPSLongitude']
                 if lat and lon:
-                    choices.add('{}, {}'.format(lat, lon))
+                    choices.add(self.value_to_text((lat, lon)))
                     continue
             choices.add(None)
         if len(choices) > 1:
             self.set_multiple(choices=[x for x in choices if x])
         else:
             self.set_value(choices and choices.pop())
 
@@ -967,8 +983,12 @@
     def fixup(self, text):
         if not self.fix_up():
             super(DoubleSpinBox, self).fixup(text)
 
     @catch_all
     def textFromValue(self, value):
         # don't use QDoubleSpinBox's fixed number of decimals
-        return str(round(float(value), self.decimals()))
+        decimals = self.decimals()
+        value = round(float(value), decimals)
+        while decimals > 1 and round(value, decimals - 1) == value:
+            decimals -= 1
+        return self.locale().toString(value, 'f', decimals)
```

