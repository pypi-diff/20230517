# Comparing `tmp/robot_package-1.0.0.tar.gz` & `tmp/robot_package-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot_package-1.0.0.tar", last modified: Wed May 17 15:50:12 2023, max compression
+gzip compressed data, was "robot_package-1.0.1.tar", last modified: Wed May 17 16:05:19 2023, max compression
```

## Comparing `robot_package-1.0.0.tar` & `robot_package-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 15:50:12.220525 robot_package-1.0.0/
--rw-rw-rw-   0        0        0       98 2023-05-17 15:50:12.220525 robot_package-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 15:50:12.189652 robot_package-1.0.0/robot_package/
--rw-rw-rw-   0        0        0   189440 2023-05-02 08:00:58.000000 robot_package-1.0.0/robot_package/jaco2.pyd
-drwxrwxrwx   0        0        0        0 2023-05-17 15:50:12.220525 robot_package-1.0.0/robot_package.egg-info/
--rw-rw-rw-   0        0        0       98 2023-05-17 15:50:12.000000 robot_package-1.0.0/robot_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-17 15:50:12.000000 robot_package-1.0.0/robot_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 15:50:12.000000 robot_package-1.0.0/robot_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 15:50:12.000000 robot_package-1.0.0/robot_package.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       14 2023-05-17 15:50:12.000000 robot_package-1.0.0/robot_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 15:50:12.220525 robot_package-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      290 2023-05-17 15:49:43.000000 robot_package-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-17 16:05:19.679691 robot_package-1.0.1/
+-rw-rw-rw-   0        0        0       98 2023-05-17 16:05:19.671655 robot_package-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-17 16:05:19.655656 robot_package-1.0.1/robot_package/
+-rw-rw-rw-   0        0        0   189440 2023-05-02 08:00:58.000000 robot_package-1.0.1/robot_package/jaco2.pyd
+drwxrwxrwx   0        0        0        0 2023-05-17 16:05:19.671655 robot_package-1.0.1/robot_package.egg-info/
+-rw-rw-rw-   0        0        0       98 2023-05-17 16:05:19.000000 robot_package-1.0.1/robot_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-17 16:05:19.000000 robot_package-1.0.1/robot_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-17 16:05:19.000000 robot_package-1.0.1/robot_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-17 15:50:12.000000 robot_package-1.0.1/robot_package.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       14 2023-05-17 16:05:19.000000 robot_package-1.0.1/robot_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-17 16:05:19.679691 robot_package-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      290 2023-05-17 16:05:06.000000 robot_package-1.0.1/setup.py
```

