# Comparing `tmp/skellyai-0.1.3.tar.gz` & `tmp/skellyai-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skellyai-0.1.3.tar", last modified: Tue May 16 20:00:50 2023, max compression
+gzip compressed data, was "dist/skellyai-0.1.4.tar", last modified: Tue May 16 23:24:36 2023, max compression
```

## Comparing `skellyai-0.1.3.tar` & `skellyai-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-16 20:00:50.374425 skellyai-0.1.3/
--rw-r--r--   0 bennicholl   (501) staff       (20)      455 2023-05-16 20:00:50.374136 skellyai-0.1.3/PKG-INFO
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-16 20:00:50.371166 skellyai-0.1.3/code/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.3/code/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)       45 2023-05-16 19:50:21.000000 skellyai-0.1.3/code/label_gen.py
--rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-05-16 20:00:50.374559 skellyai-0.1.3/setup.cfg
--rw-r--r--   0 bennicholl   (501) staff       (20)      698 2023-05-16 20:00:25.000000 skellyai-0.1.3/setup.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-16 20:00:50.373545 skellyai-0.1.3/skellyai.egg-info/
--rw-r--r--   0 bennicholl   (501) staff       (20)      455 2023-05-16 20:00:50.000000 skellyai-0.1.3/skellyai.egg-info/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)      202 2023-05-16 20:00:50.000000 skellyai-0.1.3/skellyai.egg-info/SOURCES.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-05-16 20:00:50.000000 skellyai-0.1.3/skellyai.egg-info/dependency_links.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-05-16 20:00:50.000000 skellyai-0.1.3/skellyai.egg-info/requires.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        5 2023-05-16 20:00:50.000000 skellyai-0.1.3/skellyai.egg-info/top_level.txt
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-16 23:24:36.008228 skellyai-0.1.4/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-05-16 23:24:36.007565 skellyai-0.1.4/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-05-16 23:24:36.008400 skellyai-0.1.4/setup.cfg
+-rw-r--r--   0 bennicholl   (501) staff       (20)      654 2023-05-16 23:24:18.000000 skellyai-0.1.4/setup.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-16 23:24:36.004243 skellyai-0.1.4/skellyai/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.4/skellyai/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)      705 2023-05-16 17:53:34.000000 skellyai-0.1.4/skellyai/label_gen.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-05-16 23:24:36.007032 skellyai-0.1.4/skellyai.egg-info/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)      210 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/SOURCES.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/dependency_links.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/requires.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        9 2023-05-16 23:24:35.000000 skellyai-0.1.4/skellyai.egg-info/top_level.txt
```

### Comparing `skellyai-0.1.3/setup.py` & `skellyai-0.1.4/setup.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1 +1 @@
-from setuptools import setupsetup(    name='skellyai',    version='0.1.3',        description='generated labeled data',    url='https://github.com/shuds13/pyexample',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['code'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
+from setuptools import setupsetup(    name='skellyai',    version='0.1.4',        description='generated labeled data',    author='Ben Nicholl',    author_email='ben.nicholl66@gmail.com',    license='BSD 2-clause',    packages=['skellyai'],    install_requires=[                      'pandas==1.4.4',                      'sagemaker==2.155.0'                      ],    classifiers=[        'Development Status :: 1 - Planning',        'Intended Audience :: Science/Research',        'License :: OSI Approved :: BSD License',          'Operating System :: POSIX :: Linux',                "Programming Language :: Python :: 3"    ],)
```

