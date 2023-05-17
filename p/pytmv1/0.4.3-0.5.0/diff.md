# Comparing `tmp/pytmv1-0.4.3.tar.gz` & `tmp/pytmv1-0.5.0.tar.gz`

## Comparing `pytmv1-0.4.3.tar` & `pytmv1-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.4.3/.coveragerc
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.4.3/tox.ini
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/__about__.py
--rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/__init__.py
--rwxr-xr-x   0        0        0    26132 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/caller.py
--rwxr-xr-x   0        0        0    10922 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/core.py
--rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/exceptions.py
--rwxr-xr-x   0        0        0      662 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/logger.py
--rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/mapper.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/py.typed
--rwxr-xr-x   0        0        0     3916 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/results.py
--rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/model/__init__.py
--rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/model/commons.py
--rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/model/enums.py
--rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/model/requests.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.4.3/src/pytmv1/model/responses.py
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.4.3/.gitignore
--rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.4.3/LICENSE.txt
--rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.4.3/README.md
--rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.4.3/PKG-INFO
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 pytmv1-0.5.0/.coveragerc
+-rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 pytmv1-0.5.0/tox.ini
+-rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/__about__.py
+-rwxr-xr-x   0        0        0     3504 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/__init__.py
+-rwxr-xr-x   0        0        0    26298 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/caller.py
+-rwxr-xr-x   0        0        0    10916 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/core.py
+-rwxr-xr-x   0        0        0     1479 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/exceptions.py
+-rwxr-xr-x   0        0        0     3967 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/mapper.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/py.typed
+-rwxr-xr-x   0        0        0     3910 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/results.py
+-rwxr-xr-x   0        0        0     3183 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/__init__.py
+-rw-r--r--   0        0        0     6141 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/commons.py
+-rw-r--r--   0        0        0     4770 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/enums.py
+-rwxr-xr-x   0        0        0     1816 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/requests.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pytmv1-0.5.0/src/pytmv1/model/responses.py
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 pytmv1-0.5.0/.gitignore
+-rwxr-xr-x   0        0        0    11540 2020-02-02 00:00:00.000000 pytmv1-0.5.0/LICENSE.txt
+-rwxr-xr-x   0        0        0    14766 2020-02-02 00:00:00.000000 pytmv1-0.5.0/README.md
+-rwxr-xr-x   0        0        0     1932 2020-02-02 00:00:00.000000 pytmv1-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 pytmv1-0.5.0/PKG-INFO
```

### Comparing `pytmv1-0.4.3/src/pytmv1/__init__.py` & `pytmv1-0.5.0/src/pytmv1/__init__.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/src/pytmv1/caller.py` & `pytmv1-0.5.0/src/pytmv1/caller.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
+import logging
 from functools import lru_cache
 from logging import Logger
 from typing import Callable, Optional, Type, Union
 
-from . import logger, utils
+from . import utils
 from .core import DEFAULT_POLL_TIME, Core
 from .model.commons import (
     Endpoint,
     ExceptionObject,
     SaeAlert,
     SuspiciousObject,
     TiAlert,
@@ -42,15 +43,15 @@
     SandboxAnalysisResultResp,
     SandboxSubmissionStatusResp,
     SandboxSuspiciousListResp,
     SubmitFileToSandboxResp,
 )
 from .results import MultiResult, Result
 
-log: Logger = logger.get_logger(__name__)
+log: Logger = logging.getLogger(__name__)
 
 
 def client(
     name: str,
     token: str,
     url: str,
     pool_connections: int = 1,
@@ -343,15 +344,21 @@
         :rtype: Result[NoContentResp]:
         """
         return self._core.send(
             NoContentResp,
             Api.EDIT_ALERT_STATUS.value.format(alert_id),
             HttpMethod.PATCH,
             json={"investigationStatus": status},
-            headers={"If-Match": '"' + if_match + '"'},
+            headers={
+                "If-Match": (
+                    if_match
+                    if if_match.startswith('"')
+                    else '"' + if_match + '"'
+                )
+            },
         )
 
     def enable_account(self, *accounts: AccountTask) -> MultiResult[MultiResp]:
         """Allows the user to sign in to new application and browser sessions.
 
         :param accounts: Account(s) to enable.
         :type accounts: Tuple[AccountTask, ...]
```

### Comparing `pytmv1-0.4.3/src/pytmv1/core.py` & `pytmv1-0.5.0/src/pytmv1/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
+import logging
 import re
 import time
 from logging import Logger
 from typing import Any, Callable, Dict, List, Type
 from urllib.parse import SplitResult, urlsplit
 
 from bs4 import BeautifulSoup
 from pydantic import AnyHttpUrl, parse_obj_as
 from requests import PreparedRequest, Request, Response
 from requests.adapters import HTTPAdapter
 
-from . import logger
 from .__about__ import __version__
 from .exceptions import (
     ParseModelError,
     ServerHtmlError,
     ServerJsonError,
     ServerMultiJsonError,
     ServerTextError,
@@ -49,15 +49,15 @@
 
 USERAGENT_SUFFIX: str = "PyTMV1"
 API_VERSION: str = "v3.0"
 DEFAULT_POLL_TIME: float = 1800
 CONNECT_TIMEOUT: int = 5
 READ_TIMEOUT: int = 30
 
-log: Logger = logger.get_logger(__name__)
+log: Logger = logging.getLogger(__name__)
 
 
 class Core:
     def __init__(
         self,
         appname: str,
         token: str,
```

### Comparing `pytmv1-0.4.3/src/pytmv1/exceptions.py` & `pytmv1-0.5.0/src/pytmv1/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/src/pytmv1/mapper.py` & `pytmv1-0.5.0/src/pytmv1/mapper.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/src/pytmv1/results.py` & `pytmv1-0.5.0/src/pytmv1/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
+import logging
 import time
 from dataclasses import dataclass, field
 from enum import Enum
 from functools import wraps
 from logging import Logger
 from typing import Any, Callable, Generic, List, Optional, TypeVar
 
 from pydantic import ValidationError
 from requests import RequestException
 
-from . import logger
 from .exceptions import ServerCustError, ServerJsonError, ServerMultiJsonError
 from .model.commons import Error, MsError
 from .model.responses import MR, R
 
 E = TypeVar("E", bound=Error)
 F = TypeVar("F", bound=Callable[..., Any])
 
-log: Logger = logger.get_logger(__name__)
+log: Logger = logging.getLogger(__name__)
 
 
 def multi_result(func: F) -> Callable[..., MultiResult[MR]]:
     @wraps(func)
     def _multi_result(*args: Any, **kwargs: Any) -> MultiResult[MR]:
         obj: MR | Exception = _wrapper(func, *args, **kwargs)
         return (
```

### Comparing `pytmv1-0.4.3/src/pytmv1/utils.py` & `pytmv1-0.5.0/src/pytmv1/utils.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/src/pytmv1/model/commons.py` & `pytmv1-0.5.0/src/pytmv1/model/commons.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/src/pytmv1/model/enums.py` & `pytmv1-0.5.0/src/pytmv1/model/enums.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/src/pytmv1/model/requests.py` & `pytmv1-0.5.0/src/pytmv1/model/requests.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/src/pytmv1/model/responses.py` & `pytmv1-0.5.0/src/pytmv1/model/responses.py`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/LICENSE.txt` & `pytmv1-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/README.md` & `pytmv1-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/pyproject.toml` & `pytmv1-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytmv1-0.4.3/PKG-INFO` & `pytmv1-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytmv1
-Version: 0.4.3
+Version: 0.5.0
 Summary: Python library for Trend Micro Vision One
 Project-URL: Source, https://github.com/TrendATI/pytmv1
 Project-URL: Issues, https://github.com/TrendATI/pytmv1/issues
 Author-email: Thomas Legros <thomas_legros@trendmicro.com>
 Maintainer-email: TrendATI <ati-integration@trendmicro.com>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

