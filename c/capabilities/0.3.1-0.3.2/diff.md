# Comparing `tmp/capabilities-0.3.1.tar.gz` & `tmp/capabilities-0.3.2.tar.gz`

## Comparing `capabilities-0.3.1.tar` & `capabilities-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.1/setup.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/__about__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/__init__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/__main__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/cli.py
--rw-r--r--   0        0        0     1285 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/config.py
--rw-r--r--   0        0        0    16987 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/core.py
--rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/dec.py
--rw-r--r--   0        0        0    15162 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/example.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/__init__.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/hf.py
--rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/loader.py
--rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/nomic_index.py
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/oai.py
--rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/search_index.py
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/simple_vector_index.py
--rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/types.py
--rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/search/util.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/util/__init__.py
--rw-r--r--   0        0        0     8767 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/util/config.py
--rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 capabilities-0.3.1/capabilities/util/misc.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/cheese.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/leansearch.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/readme.txt
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/tesla10k.py
--rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/data/apple10k.pdf
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/data/sample.md
--rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/data/sample.pdf
--rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.1/examples/data/tesla10k.txt
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_dec.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_document_loader.py
--rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_search.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_search_util.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_tutorial1.py
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/test_vector_idx.py
--rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
--rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
--rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.1/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.1/README.md
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 capabilities-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 capabilities-0.3.2/setup.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 capabilities-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/__about__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/__init__.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/__main__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/cli.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/config.py
+-rw-r--r--   0        0        0    16987 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/core.py
+-rw-r--r--   0        0        0     8071 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/dec.py
+-rw-r--r--   0        0        0    15162 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/example.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/__init__.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/hf.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/loader.py
+-rw-r--r--   0        0        0     6082 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/nomic_index.py
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/oai.py
+-rw-r--r--   0        0        0    12426 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/search_index.py
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/simple_vector_index.py
+-rw-r--r--   0        0        0     7076 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/types.py
+-rw-r--r--   0        0        0     5313 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/search/util.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/util/__init__.py
+-rw-r--r--   0        0        0     9213 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/util/config.py
+-rw-r--r--   0        0        0     6628 2020-02-02 00:00:00.000000 capabilities-0.3.2/capabilities/util/misc.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/cheese.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/leansearch.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/readme.txt
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/tesla10k.py
+-rw-r--r--   0        0        0   840980 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/data/apple10k.pdf
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/data/sample.md
+-rw-r--r--   0        0        0     7945 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/data/sample.pdf
+-rw-r--r--   0        0        0   157134 2020-02-02 00:00:00.000000 capabilities-0.3.2/examples/data/tesla10k.txt
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_dec.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_document_loader.py
+-rw-r--r--   0        0        0     2841 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_search.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_search_util.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_tutorial1.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/test_vector_idx.py
+-rw-r--r--   0        0        0   353564 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0   353563 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt
+-rw-r--r--   0        0        0   353565 2020-02-02 00:00:00.000000 capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt
+-rw-r--r--   0        0        0     1802 2020-02-02 00:00:00.000000 capabilities-0.3.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 capabilities-0.3.2/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 capabilities-0.3.2/README.md
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 capabilities-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    14287 2020-02-02 00:00:00.000000 capabilities-0.3.2/PKG-INFO
```

### Comparing `capabilities-0.3.1/.github/workflows/python-publish.yml` & `capabilities-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/cli.py` & `capabilities-0.3.2/capabilities/cli.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/config.py` & `capabilities-0.3.2/capabilities/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 from dataclasses import dataclass
 import os
 from typing import Optional
 import pydantic
 from pathlib import Path
 from rich import print
 import sys
-
+import logging
 from capabilities.util.config import SecretPersist, get_app_config_dir
 
-CONFIG_DIR = get_app_config_dir("capabilities")
+
+logger = logging.getLogger(__name__)
 
 
 class Config(pydantic.BaseSettings, SecretPersist):
     api_key: Optional[pydantic.SecretStr] = pydantic.Field(default=None, is_secret=True)
     api_url: str = "https://api.blazon.ai"
 
+    config_dir: Path = pydantic.Field(
+        default_factory=lambda: get_app_config_dir("capabilities")
+    )
+
     @property
-    def secrets_file(self) -> Path:
-        return CONFIG_DIR / "secrets.json"
+    def secrets_file(self) -> Optional[Path]:
+        if self.config_dir.exists():
+            return self.config_dir / "secrets.json"
+        else:
+            return None
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
         env_prefix = "CAPABILITIES_"
         secret_postfix = lambda self: self.api_url
```

### Comparing `capabilities-0.3.1/capabilities/core.py` & `capabilities-0.3.2/capabilities/core.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/dec.py` & `capabilities-0.3.2/capabilities/dec.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/example.py` & `capabilities-0.3.2/capabilities/example.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/search/hf.py` & `capabilities-0.3.2/capabilities/search/hf.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/search/loader.py` & `capabilities-0.3.2/capabilities/search/loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/search/nomic_index.py` & `capabilities-0.3.2/capabilities/search/nomic_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/search/oai.py` & `capabilities-0.3.2/capabilities/search/oai.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/search/search_index.py` & `capabilities-0.3.2/capabilities/search/search_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/search/simple_vector_index.py` & `capabilities-0.3.2/capabilities/search/simple_vector_index.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/search/types.py` & `capabilities-0.3.2/capabilities/search/types.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/search/util.py` & `capabilities-0.3.2/capabilities/search/util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/capabilities/util/config.py` & `capabilities-0.3.2/capabilities/util/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import functools
 import json
 import logging
 import sys
 from typing import Any, Optional, Union
 from pathlib import Path
 import os
 import subprocess
@@ -69,30 +70,36 @@
         return Path(git_root)
     logger.debug(
         f"{cwd} is not in a git repository and no pyproject.toml could be found."
     )
     return None
 
 
+@functools.cache
 def get_app_config_dir(app_name: str) -> Path:
     """Get the path to the application directory.
 
     The implementation is based on https://click.palletsprojects.com/en/8.1.x/api/#click.get_app_dir
     """
     if sys.platform == "win32":
         p = Path(os.environ.get("APPDATA", "~/.config"))
     elif sys.platform == "linux":
         p = Path(os.environ.get("XDG_CONFIG_HOME", "~/.config"))
     elif sys.platform == "darwin":  # macos
         # [todo] "~/Library/Application Support" or "~/Library/Preferences"?
         p = Path("~") / "Library" / "Application Support"
     else:
         p = Path(os.environ.get("XDG_CONFIG_HOME", "~/.config"))
-    p = p.expanduser().resolve() / app_name
-    p.mkdir(exist_ok=True)
+    p = p.expanduser().resolve()
+    # [todo](ed) user may not be able to create directories
+    p = p / app_name
+    try:
+        p.mkdir(exist_ok=True)
+    except Exception:
+        pass
     return p
 
 
 def get_app_cache_dir(app_name: str) -> Path:
     """Returns the path that ths OS wants you to use to place application-specific caching files."""
     if sys.platform == "win32":
         p = Path(os.environ.get("LOCALAPPDATA", "~/.cache"))
@@ -102,15 +109,18 @@
         p = Path("~/Library/Caches")
     else:
         logger.warning(
             f"Unrecognised platform: {sys.platform}, user cache is defaulting to a tmpdir."
         )
         p = Path(tempfile.gettempdir())
     p = p.expanduser().resolve() / app_name
-    p.mkdir(exist_ok=True)
+    try:
+        p.mkdir(exist_ok=True)
+    except Exception:
+        pass
     return p
 
 
 def persist_config(p: Path, key: Union[str, tuple[str, ...]], value: Any):
     if p.exists():
         root = json.loads(p.read_text())
     else:
@@ -200,48 +210,53 @@
     ```
 
     Now, when you call `persist_secret`, it will save it in a different slot determined by
     `secret_postfix`. So now `get_secret`'s return value will depend on whether mode is dev or prod.
 
     """
 
-    def _get_secret_prelude(self, key: str):
+    def _get_secret_prelude(self, key: str) -> tuple[Optional[Path], str]:
         assert isinstance(self, BaseSettings)
         fields = getattr(self, "__fields__")
         assert key in fields
         field = fields[key]
         assert issubclass(SecretStr, field.annotation)
         extra = field.field_info.extra
         assert extra.get(
             "is_secret", False
         ), "please add the 'is_secret=True' kwarg to Field constructor"
         cfg = getattr(self, "__config__")
-        secrets_file = getattr(self, "secrets_file")
+        secrets_file = getattr(self, "secrets_file", None)
+        if secrets_file is not None:
+            secrets_file = Path(secrets_file)
         secret_postfix = getattr(cfg, "secret_postfix", None)
         if secret_postfix is None:
             secret_postfix = "default"
         elif secret_postfix in fields:
             secret_postfix = getattr(self, secret_postfix)
             assert isinstance(secret_postfix, str)
         elif callable(secret_postfix):
             secret_postfix = secret_postfix(self)
         else:
             raise ValueError(f"secret_postfix {secret_postfix} not found")
         return secrets_file, secret_postfix
 
     def persist_secret(self, key: str, secret: str):
         file, postfix = self._get_secret_prelude(key)
-        logger.debug(f"Saving secret {key} for {postfix} to {file}")
-        persist_config(file, (key, postfix), secret)
+        if file is not None:
+            logger.debug(f"Saving secret {key} for {postfix} to {file}")
+            persist_config(file, (key, postfix), secret)
         setattr(self, key, SecretStr(secret))
 
     def get_secret(self, key: str) -> Optional[str]:
         file, postfix = self._get_secret_prelude(key)
         secret: Optional[SecretStr] = getattr(self, key, None)
         if secret is None:
+            if file is None:
+                return None
             try:
                 value = get_config(file, (key, postfix))
                 if value is None:
                     logger.debug(f"{key} for {postfix} was invalidated")
                     return None
             except LookupError:
                 logger.debug(f"no {key} for {postfix} found in {file}")
@@ -249,9 +264,10 @@
             setattr(self, key, SecretStr(value))
             return value
         else:
             return secret.get_secret_value()
 
     def invalidate_secret(self, key: str):
         file, postfix = self._get_secret_prelude(key)
-        persist_config(file, (key, postfix), None)
+        if file is not None:
+            persist_config(file, (key, postfix), None)
         setattr(self, key, None)
```

### Comparing `capabilities-0.3.1/capabilities/util/misc.py` & `capabilities-0.3.2/capabilities/util/misc.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/examples/cheese.py` & `capabilities-0.3.2/examples/cheese.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/examples/leansearch.py` & `capabilities-0.3.2/examples/leansearch.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/examples/tesla10k.py` & `capabilities-0.3.2/examples/tesla10k.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/examples/data/apple10k.pdf` & `capabilities-0.3.2/examples/data/apple10k.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/examples/data/sample.md` & `capabilities-0.3.2/examples/data/sample.md`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/examples/data/sample.pdf` & `capabilities-0.3.2/examples/data/sample.pdf`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/examples/data/tesla10k.txt` & `capabilities-0.3.2/examples/data/tesla10k.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/test_dec.py` & `capabilities-0.3.2/tests/test_dec.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/test_document_loader.py` & `capabilities-0.3.2/tests/test_document_loader.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/test_search.py` & `capabilities-0.3.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/test_search_util.py` & `capabilities-0.3.2/tests/test_search_util.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/test_tutorial1.py` & `capabilities-0.3.2/tests/test_tutorial1.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/test_vector_idx.py` & `capabilities-0.3.2/tests/test_vector_idx.py`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt` & `capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/NomicIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/NomicIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt` & `capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/SearchIndex-openai/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt` & `capabilities-0.3.2/tests/snapshots/test_search/test_search_e2e/SearchIndex-sentence-transformersall-MiniLM-L6-v2/r0.txt`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/.gitignore` & `capabilities-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/LICENSE` & `capabilities-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/pyproject.toml` & `capabilities-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `capabilities-0.3.1/PKG-INFO` & `capabilities-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: capabilities
-Version: 0.3.1
+Version: 0.3.2
 Summary: Build trusted, faster, and more powerful applications with the Blazon Capabilities API.
 Author-email: Blazon AI <support@blazon.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

