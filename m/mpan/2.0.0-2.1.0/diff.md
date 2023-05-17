# Comparing `tmp/mpan-2.0.0.tar.gz` & `tmp/mpan-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpan-2.0.0.tar", max compression
+gzip compressed data, was "mpan-2.1.0.tar", max compression
```

## Comparing `mpan-2.0.0.tar` & `mpan-2.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1065 2021-05-06 10:54:19.467420 mpan-2.0.0/LICENSE
--rw-r--r--   0        0        0      794 2022-04-01 14:27:34.943103 mpan-2.0.0/README.md
--rw-r--r--   0        0        0       81 2022-01-05 17:42:21.645722 mpan-2.0.0/mpan/__init__.py
--rw-r--r--   0        0        0      522 2022-01-05 17:42:21.645722 mpan-2.0.0/mpan/common.py
--rw-r--r--   0        0        0    13811 2022-08-25 08:44:16.632722 mpan-2.0.0/mpan/data.py
--rw-r--r--   0        0        0     1203 2022-08-25 08:44:16.632722 mpan-2.0.0/mpan/distributor.py
--rw-r--r--   0        0        0       44 2022-01-05 17:42:21.645722 mpan-2.0.0/mpan/exceptions.py
--rw-r--r--   0        0        0      161 2022-01-05 17:42:21.645722 mpan-2.0.0/mpan/generation/faker.py
--rw-r--r--   0        0        0      713 2022-08-25 08:44:16.636721 mpan-2.0.0/mpan/generation/helpers.py
--rw-r--r--   0        0        0      225 2022-01-05 17:42:21.645722 mpan-2.0.0/mpan/generation/mimesis.py
--rw-r--r--   0        0        0      205 2022-01-05 17:42:21.645722 mpan-2.0.0/mpan/helpers.py
--rw-r--r--   0        0        0     1196 2022-01-05 17:42:21.645722 mpan-2.0.0/mpan/meter_time_switch_code.py
--rw-r--r--   0        0        0     3679 2022-08-05 13:02:15.759820 mpan-2.0.0/mpan/mpan.py
--rw-r--r--   0        0        0     1287 2022-01-05 17:42:21.645722 mpan-2.0.0/mpan/profile_class.py
--rw-r--r--   0        0        0     1606 2022-08-25 08:45:48.908781 mpan-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1634 2022-09-20 09:48:56.212898 mpan-2.0.0/setup.py
--rw-r--r--   0        0        0     1672 2022-09-20 09:48:56.213118 mpan-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-16 12:09:51.485029 mpan-2.1.0/LICENSE
+-rw-r--r--   0        0        0      794 2023-05-16 12:09:51.485029 mpan-2.1.0/README.md
+-rw-r--r--   0        0        0       81 2023-05-16 12:09:51.485029 mpan-2.1.0/mpan/__init__.py
+-rw-r--r--   0        0        0      522 2023-05-16 15:44:15.429802 mpan-2.1.0/mpan/common.py
+-rw-r--r--   0        0        0    13811 2023-05-16 15:44:22.769802 mpan-2.1.0/mpan/data.py
+-rw-r--r--   0        0        0     1202 2023-05-17 15:57:03.372616 mpan-2.1.0/mpan/distributor.py
+-rw-r--r--   0        0        0       44 2023-05-16 12:09:51.485029 mpan-2.1.0/mpan/exceptions.py
+-rw-r--r--   0        0        0      161 2023-05-16 12:09:51.485029 mpan-2.1.0/mpan/generation/faker.py
+-rw-r--r--   0        0        0      712 2023-05-17 15:57:03.372616 mpan-2.1.0/mpan/generation/helpers.py
+-rw-r--r--   0        0        0      225 2023-05-16 12:09:51.485029 mpan-2.1.0/mpan/generation/mimesis.py
+-rw-r--r--   0        0        0      205 2023-05-16 15:44:39.116334 mpan-2.1.0/mpan/helpers.py
+-rw-r--r--   0        0        0     1195 2023-05-17 15:57:03.372616 mpan-2.1.0/mpan/meter_time_switch_code.py
+-rw-r--r--   0        0        0     3683 2023-05-17 15:57:03.372616 mpan-2.1.0/mpan/mpan.py
+-rw-r--r--   0        0        0     1286 2023-05-17 15:57:03.372616 mpan-2.1.0/mpan/profile_class.py
+-rw-r--r--   0        0        0     1604 2023-05-17 15:57:03.372616 mpan-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1634 2023-05-17 15:59:45.231145 mpan-2.1.0/setup.py
+-rw-r--r--   0        0        0     1672 2023-05-17 15:59:45.231352 mpan-2.1.0/PKG-INFO
```

### Comparing `mpan-2.0.0/LICENSE` & `mpan-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpan-2.0.0/README.md` & `mpan-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mpan-2.0.0/mpan/common.py` & `mpan-2.1.0/mpan/common.py`

 * *Files identical despite different names*

### Comparing `mpan-2.0.0/mpan/data.py` & `mpan-2.1.0/mpan/data.py`

 * *Files identical despite different names*

### Comparing `mpan-2.0.0/mpan/distributor.py` & `mpan-2.1.0/mpan/distributor.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
     @property
     def participant_id(self) -> str:
         return ID_LOOKUP[self.identifier]["id"]
 
     @property
     def gsp_group_ids(self) -> List[str]:
-
         now = date.today()
 
         r = []
         for gsp_id, (started, stopped) in GSP_IDS[self.participant_id]:
             if now > started:
                 if not stopped or stopped > now:
                     r.append(gsp_id)
```

### Comparing `mpan-2.0.0/mpan/generation/helpers.py` & `mpan-2.1.0/mpan/generation/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 
 from ..data import ID_LOOKUP
 from ..mpan import MPAN
 from ..profile_class import ProfileClass
 
 
 def generate() -> str:
-
     profile_class = random.choice(tuple(ProfileClass.DESCRIPTIONS.keys()))
 
     mtc = random.randint(100, 999)
 
     llfc_options = string.ascii_uppercase + string.digits
     llfc = "".join([random.choice(llfc_options) for _ in range(3)])
```

### Comparing `mpan-2.0.0/mpan/meter_time_switch_code.py` & `mpan-2.1.0/mpan/meter_time_switch_code.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         try:
             return 0 < int(self.identifier) < 1000
         except ValueError:
             return False
 
     @property
     def description(self) -> Optional[str]:
-
         if not self.identifier:
             return None
 
         try:
             value = int(self.identifier)
         except ValueError:
             return None
```

### Comparing `mpan-2.0.0/mpan/mpan.py` & `mpan-2.1.0/mpan/mpan.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 from .distributor import Distributor
 from .exceptions import InvalidMPANError
 from .meter_time_switch_code import MeterTimeSwitchCode
 from .profile_class import ProfileClass
 
 
 class MPAN:
-
     RE_SHORT = re.compile(r"^((\d\d)(\d{8})\d\d(\d))$")
     RE_LONG = re.compile(
         r"^((\d\d)(\d\d\d)([A-Z0-9]{3}))((\d\d)(\d{8})\d\d(\d))$"
     )
 
     # 11 is deliberately missing as-per the rules for the validation algorithm.
     PRIMES = [3, 5, 7, 13, 17, 19, 23, 29, 31, 37, 41, 43]
 
     def __init__(self, raw_string: str) -> None:
-
         self.top_line = None
         self.profile_class = None
         self.meter_time_switch_code = None
         self.line_loss_factor_class = None
         self.core = None
         self.distributor = None
         self.identifier = None
@@ -51,15 +49,15 @@
     def __str__(self) -> str:
         return self._raw
 
     def __repr__(self):
         return str(self)
 
     def __eq__(self, other):
-        if not isinstance(other, MPAN):
+        if not isinstance(other, (MPAN, str)):
             return False
         return str(self) == str(other)
 
     @property
     def is_short(self) -> bool:
         return self.profile_class is None
 
@@ -113,15 +111,14 @@
     def _parse_short(self, m: re.Match) -> None:
         self.core = m.group(1)
         self.distributor = Distributor(m.group(2))
         self.identifier = m.group(3)
         self.checksum = m.group(4)
 
     def _parse_long(self, m: re.Match) -> None:
-
         self.top_line = m.group(1)
         self.profile_class = ProfileClass(m.group(2))
         self.meter_time_switch_code = MeterTimeSwitchCode(m.group(3))
         self.line_loss_factor_class = m.group(4)
 
         self.core = m.group(5)
         self.distributor = Distributor(m.group(6))
```

### Comparing `mpan-2.0.0/mpan/profile_class.py` & `mpan-2.1.0/mpan/profile_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Optional
 
 from .common import Subsection
 
 
 class ProfileClass(Subsection):
-
     DESCRIPTIONS = {
         "00": "Half-hourly supply (import and export)",
         "01": "Domestic unrestricted",
         "02": "Domestic Economy meter of two or more rates",
         "03": "Non-domestic unrestricted",
         "04": "Non-domestic Economy 7",
         "05": (
```

### Comparing `mpan-2.0.0/pyproject.toml` & `mpan-2.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mpan"
-version = "2.0.0"
+version = "2.1.0"
 description = "A parsing library for the UK's MPAN energy standard"
 authors = ["Limejump Developers <opensource@limejump.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/limejump/mpan"
 repository = "https://github.com/limejump/mpan"
 documentation = "https://github.com/limejump/mpan"
@@ -21,15 +21,15 @@
 
 [tool.poetry.extras]
 faker = ["Faker"]
 mimesis = ["mimesis"]
 
 
 [tool.poetry.dev-dependencies]
-black = "^20.8b1"
+black = "^23.0"
 isort = "^5.7.0"
 flake8 = "^3.8.4"
 freezegun = "^1.2.1"
 ipython = "^7.20.0"
 mkdocs = "^1.2.3"
 mkdocs-techdocs-core = "^0.2.2"
 pre-commit = "^2.10.0"
```

### Comparing `mpan-2.0.0/setup.py` & `mpan-2.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['coverage[toml]>=6.2,<7.0']
 
 extras_require = \
 {'faker': ['Faker>=10.0.0,<11.0.0'], 'mimesis': ['mimesis>=5.1.0,<6.0.0']}
 
 setup_kwargs = {
     'name': 'mpan',
-    'version': '2.0.0',
+    'version': '2.1.0',
     'description': "A parsing library for the UK's MPAN energy standard",
     'long_description': "[![Limejump logo](https://raw.githubusercontent.com/limejump/mpan/master/docs/logo.png)](https://limejump.com/)\n\n\n# mpan\n\n[![PyPI](https://img.shields.io/pypi/pyversions/mpan)](https://pypi.org/project/mpan)\n[![PyPI](https://img.shields.io/pypi/wheel/mpan)](https://pypi.org/project/mpan)\n[![License](https://img.shields.io/pypi/l/mpan)](https://mit-license.org/)\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n![100% Coverage](https://img.shields.io/badge/coverage-100%25-4ec820.svg)\n\nA library to help you parse the UK energy industry's MPAN number format.\n\n## Links\n\n* [Official documentation](https://limejump.github.io/mpan/)\n* [Wikipedia article on the MPAN standard](https://en.wikipedia.org/wiki/Meter_Point_Administration_Number)\n",
     'author': 'Limejump Developers',
     'author_email': 'opensource@limejump.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/limejump/mpan',
```

### Comparing `mpan-2.0.0/PKG-INFO` & `mpan-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpan
-Version: 2.0.0
+Version: 2.1.0
 Summary: A parsing library for the UK's MPAN energy standard
 Home-page: https://github.com/limejump/mpan
 License: MIT
 Author: Limejump Developers
 Author-email: opensource@limejump.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

