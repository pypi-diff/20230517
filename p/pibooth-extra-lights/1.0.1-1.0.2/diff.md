# Comparing `tmp/pibooth_extra_lights-1.0.1.tar.gz` & `tmp/pibooth_extra_lights-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pibooth_extra_lights-1.0.1.tar", last modified: Sun Oct 11 17:36:44 2020, max compression
+gzip compressed data, was "pibooth_extra_lights-1.0.2.tar", last modified: Wed May 17 05:15:29 2023, max compression
```

## Comparing `pibooth_extra_lights-1.0.1.tar` & `pibooth_extra_lights-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-11 17:36:44.404745 pibooth_extra_lights-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (116)     4019 2020-10-11 17:36:44.404745 pibooth_extra_lights-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2384 2020-10-11 17:35:34.000000 pibooth_extra_lights-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-11 17:36:44.404745 pibooth_extra_lights-1.0.1/pibooth_extra_lights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4019 2020-10-11 17:36:44.000000 pibooth_extra_lights-1.0.1/pibooth_extra_lights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      352 2020-10-11 17:36:44.000000 pibooth_extra_lights-1.0.1/pibooth_extra_lights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-11 17:36:44.000000 pibooth_extra_lights-1.0.1/pibooth_extra_lights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       55 2020-10-11 17:36:44.000000 pibooth_extra_lights-1.0.1/pibooth_extra_lights.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-11 17:36:44.000000 pibooth_extra_lights-1.0.1/pibooth_extra_lights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)       15 2020-10-11 17:36:44.000000 pibooth_extra_lights-1.0.1/pibooth_extra_lights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       21 2020-10-11 17:36:44.000000 pibooth_extra_lights-1.0.1/pibooth_extra_lights.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1858 2020-10-11 17:35:34.000000 pibooth_extra_lights-1.0.1/pibooth_extra_lights.py
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-10-11 17:36:44.404745 pibooth_extra_lights-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1933 2020-10-11 17:35:34.000000 pibooth_extra_lights-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:15:29.808874 pibooth_extra_lights-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34502 2023-05-17 05:14:56.000000 pibooth_extra_lights-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-17 05:15:29.808874 pibooth_extra_lights-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-17 05:14:56.000000 pibooth_extra_lights-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 05:15:29.808874 pibooth_extra_lights-1.0.2/pibooth_extra_lights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-05-17 05:15:29.000000 pibooth_extra_lights-1.0.2/pibooth_extra_lights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-17 05:15:29.000000 pibooth_extra_lights-1.0.2/pibooth_extra_lights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:15:29.000000 pibooth_extra_lights-1.0.2/pibooth_extra_lights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-17 05:15:29.000000 pibooth_extra_lights-1.0.2/pibooth_extra_lights.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 05:15:29.000000 pibooth_extra_lights-1.0.2/pibooth_extra_lights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-17 05:15:29.000000 pibooth_extra_lights-1.0.2/pibooth_extra_lights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-17 05:15:29.000000 pibooth_extra_lights-1.0.2/pibooth_extra_lights.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-17 05:14:56.000000 pibooth_extra_lights-1.0.2/pibooth_extra_lights.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 05:15:29.808874 pibooth_extra_lights-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-17 05:14:56.000000 pibooth_extra_lights-1.0.2/setup.py
```

### Comparing `pibooth_extra_lights-1.0.1/README.rst` & `pibooth_extra_lights-1.0.2/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -31,48 +31,57 @@
 .. code-block:: ini
 
     [CONTROLS]
 
     # Physical GPIO OUT pin to light a LED at pibooth startup (list of pins accepted)
     startup_led_pin = 29
 
+    # If True, startup LED is lighting by setting pin(s) to HIGH else by setting to LOW
+    startup_led_active_high = True
+
     # Physical GPIO OUT pin to light a LED during the entire capture sequence (list of pins accepted)
     preview_led_pin = 31
 
+    # If True, preview LED is lighting by setting pin(s) to HIGH else by setting to LOW
+    preview_led_active_high = True
+
     # Physical GPIO OUT pin to light a LED when the capture is taken (list of pins accepted)
     flash_led_pin = 33
 
+    # If True, flash LED is lighting by setting pin(s) to HIGH else by setting to LOW
+    flash_led_active_high = True
+
 .. note:: Edit the configuration by running the command ``pibooth --config``.
 
 States description
 ------------------
 
-Here is the `pibooth state sequence <https://github.com/pibooth/pibooth#states-and-lights-management>`_
+Here is the `pibooth state sequence <https://pibooth.readthedocs.io/en/latest/sources/plugins/plugins.html#influencing-states>`_
 updated with the lights activated by this plugin:
 
-.. image:: https://raw.githubusercontent.com/pibooth/pibooth-extra-lights/master/templates/state_sequence.png
+.. image:: https://raw.githubusercontent.com/pibooth/pibooth-extra-lights/master/docs/images/state_sequence.png
    :align: center
    :alt: State sequence
 
 Circuit diagram
 ---------------
 
 Here is the diagram for hardware connections.
 
-.. image:: https://raw.githubusercontent.com/pibooth/pibooth-extra-lights/master/templates/sketch.png
+.. image:: https://raw.githubusercontent.com/pibooth/pibooth-extra-lights/master/docs/images/sketch.png
    :align: center
    :alt: Electronic sketch
 
 .. --- Links ------------------------------------------------------------------
 
 .. _`pibooth`: https://pypi.org/project/pibooth
 
-.. |PythonVersions| image:: https://img.shields.io/badge/python-2.7+ / 3.6+-red.svg
+.. |PythonVersions| image:: https://img.shields.io/badge/python-3.6+-red.svg
    :target: https://www.python.org/downloads
-   :alt: Python 2.7+/3.6+
+   :alt: Python 3.6+
 
 .. |PypiPackage| image:: https://badge.fury.io/py/pibooth-extra-lights.svg
    :target: https://pypi.org/project/pibooth-extra-lights
    :alt: PyPi package
 
 .. |Downloads| image:: https://img.shields.io/pypi/dm/pibooth-extra-lights?color=purple
    :target: https://pypi.org/project/pibooth-extra-lights
```

### Comparing `pibooth_extra_lights-1.0.1/setup.py` & `pibooth_extra_lights-1.0.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,55 +5,53 @@
 from io import open
 import os.path as osp
 from setuptools import setup
 
 
 HERE = osp.abspath(osp.dirname(__file__))
 sys.path.insert(0, HERE)
-import pibooth_extra_lights as plugin
+import pibooth_extra_lights as plugin  # nopep8 : import shall be done after adding setup to paths
 
 
 def main():
     setup(
         name=plugin.__name__,
         version=plugin.__version__,
         description=plugin.__doc__,
         long_description=open(osp.join(HERE, 'README.rst'), encoding='utf-8').read(),
         long_description_content_type='text/x-rst',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
             'Environment :: Other Environment',
             'Intended Audience :: Developers',
             'Intended Audience :: End Users/Desktop',
-            'License :: OSI Approved :: MIT License',
+            'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
             'Operating System :: POSIX :: Linux',
-            'Programming Language :: Python :: 2.7',
-            'Programming Language :: Python :: 3.4',
-            'Programming Language :: Python :: 3.5',
+            'Programming Language :: Python :: 3.6',
+            'Programming Language :: Python :: 3.7',
+            'Programming Language :: Python :: 3.8',
+            'Programming Language :: Python :: 3.9',
             'Natural Language :: English',
             'Topic :: Multimedia :: Graphics :: Capture :: Digital Camera',
         ],
         author="Vincent Verdeil, Antoine Rousseaux",
         url="https://github.com/pibooth/pibooth-extra-lights",
         download_url="https://github.com/pibooth/pibooth-extra-lights/archive/{}.tar.gz".format(plugin.__version__),
-        license='MIT license',
+        license='GPLv3',
         platforms=['unix', 'linux'],
         keywords=[
             'Raspberry Pi',
             'camera',
             'photobooth'
         ],
         py_modules=['pibooth_extra_lights'],
+        python_requires=">=3.6",
         install_requires=[
             'pibooth>=2.0.0',
         ],
-        options={
-            'bdist_wheel':
-                {'universal': True}
-        },
         zip_safe=False,  # Don't install the lib as an .egg zipfile
         entry_points={'pibooth': ["pibooth_extra_lights = pibooth_extra_lights"]},
     )
 
 
 if __name__ == '__main__':
     main()
```

