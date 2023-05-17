# Comparing `tmp/huntflow_api_client-0.0.2.tar.gz` & `tmp/huntflow_api_client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huntflow_api_client-0.0.2.tar", max compression
+gzip compressed data, was "huntflow_api_client-0.0.4.tar", last modified: Wed May 17 11:20:29 2023, max compression
```

## Comparing `huntflow_api_client-0.0.2.tar` & `huntflow_api_client-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,86 @@
--rw-r--r--   0        0        0     1065 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/LICENSE
--rw-r--r--   0        0        0      488 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/README.md
--rw-r--r--   0        0        0       76 2023-04-28 13:36:59.459770 huntflow_api_client-0.0.2/huntflow_api_client/__init__.py
--rw-r--r--   0        0        0     6250 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/api.py
--rw-r--r--   0        0        0        0 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/entities/__init__.py
--rw-r--r--   0        0        0      955 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/entities/base.py
--rw-r--r--   0        0        0     1483 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/entities/tags.py
--rw-r--r--   0        0        0      187 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/errors.py
--rw-r--r--   0        0        0        0 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/__init__.py
--rw-r--r--   0        0        0      196 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/common.py
--rw-r--r--   0        0        0        0 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/request/__init__.py
--rw-r--r--   0        0        0      298 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/request/tags.py
--rw-r--r--   0        0        0        0 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/response/__init__.py
--rw-r--r--   0        0        0      313 2023-04-28 13:36:40.455608 huntflow_api_client-0.0.2/huntflow_api_client/models/response/tags.py
--rw-r--r--   0        0        0       53 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/__init__.py
--rw-r--r--   0        0        0     1871 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/locker.py
--rw-r--r--   0        0        0     5186 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/proxy.py
--rw-r--r--   0        0        0      730 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/storage.py
--rw-r--r--   0        0        0      562 2023-04-28 13:36:40.459608 huntflow_api_client-0.0.2/huntflow_api_client/tokens/token.py
--rw-r--r--   0        0        0     1328 2023-04-28 13:36:59.463770 huntflow_api_client-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1175 1970-01-01 00:00:00.000000 huntflow_api_client-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/LICENSE
+-rw-r--r--   0        0        0      488 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/README.md
+-rw-r--r--   0        0        0       76 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/huntflow_api_client/__init__.py
+-rw-r--r--   0        0        0     5578 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/huntflow_api_client/api.py
+-rw-r--r--   0        0        0        0 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/huntflow_api_client/entities/__init__.py
+-rw-r--r--   0        0        0     1760 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/huntflow_api_client/entities/account_vacancy_request.py
+-rw-r--r--   0        0        0     1434 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/huntflow_api_client/entities/accounts.py
+-rw-r--r--   0        0        0     2903 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/huntflow_api_client/entities/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      730 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/huntflow_api_client/entities/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0     8317 2023-05-17 11:20:10.702725 huntflow_api_client-0.0.4/huntflow_api_client/entities/applicants.py
+-rw-r--r--   0        0        0      941 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/base.py
+-rw-r--r--   0        0        0     2651 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/coworkers.py
+-rw-r--r--   0        0        0     3002 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/dictionaries.py
+-rw-r--r--   0        0        0     2538 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/divisions.py
+-rw-r--r--   0        0        0     6720 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/production_calendars.py
+-rw-r--r--   0        0        0      713 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/rejection_reason.py
+-rw-r--r--   0        0        0     2456 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/tags.py
+-rw-r--r--   0        0        0     9379 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/vacancies.py
+-rw-r--r--   0        0        0     2918 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/vacancy_requests.py
+-rw-r--r--   0        0        0     1789 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/entities/webhooks.py
+-rw-r--r--   0        0        0      553 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/errors/__init__.py
+-rw-r--r--   0        0        0     1127 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/errors/errors.py
+-rw-r--r--   0        0        0     3732 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/errors/handlers.py
+-rw-r--r--   0        0        0      361 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/errors/response_hooks.py
+-rw-r--r--   0        0        0        0 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/__init__.py
+-rw-r--r--   0        0        0     6501 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/common.py
+-rw-r--r--   0        0        0     2145 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/consts.py
+-rw-r--r--   0        0        0        0 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/__init__.py
+-rw-r--r--   0        0        0     3614 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/applicant_on_vacancy.py
+-rw-r--r--   0        0        0     6196 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/applicants.py
+-rw-r--r--   0        0        0     1492 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/dictionaries.py
+-rw-r--r--   0        0        0      691 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/divisions.py
+-rw-r--r--   0        0        0      921 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/production_calendars.py
+-rw-r--r--   0        0        0      259 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/tags.py
+-rw-r--r--   0        0        0     3123 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/vacancies.py
+-rw-r--r--   0        0        0     1407 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/vacancy_requests.py
+-rw-r--r--   0        0        0      482 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/request/webhooks.py
+-rw-r--r--   0        0        0        0 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/__init__.py
+-rw-r--r--   0        0        0     2102 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/account_vacancy_request.py
+-rw-r--r--   0        0        0     1595 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/accounts.py
+-rw-r--r--   0        0        0     1054 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/applicant_on_vacancy.py
+-rw-r--r--   0        0        0      773 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/applicant_on_vacancy_status.py
+-rw-r--r--   0        0        0    12930 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/applicants.py
+-rw-r--r--   0        0        0     1262 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/coworkers.py
+-rw-r--r--   0        0        0     2261 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/dictionaries.py
+-rw-r--r--   0        0        0     1507 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/divisions.py
+-rw-r--r--   0        0        0      330 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/offers.py
+-rw-r--r--   0        0        0     1525 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/production_calendars.py
+-rw-r--r--   0        0        0      476 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/rejection_reason.py
+-rw-r--r--   0        0        0      781 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/survey.py
+-rw-r--r--   0        0        0      241 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/tags.py
+-rw-r--r--   0        0        0     6182 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/vacancies.py
+-rw-r--r--   0        0        0     2973 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/vacancy_requests.py
+-rw-r--r--   0        0        0      719 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/models/response/webhooks.py
+-rw-r--r--   0        0        0       53 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/tokens/__init__.py
+-rw-r--r--   0        0        0     1871 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/tokens/locker.py
+-rw-r--r--   0        0        0     5186 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/tokens/proxy.py
+-rw-r--r--   0        0        0      730 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/tokens/storage.py
+-rw-r--r--   0        0        0      548 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/huntflow_api_client/tokens/token.py
+-rw-r--r--   0        0        0     1354 2023-05-17 11:20:29.290877 huntflow_api_client-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     4744 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/api.py
+-rw-r--r--   0        0        0       79 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/conftest.py
+-rw-r--r--   0        0        0      176 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/fixtures/server.py
+-rw-r--r--   0        0        0      856 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/fixtures/tokens.py
+-rw-r--r--   0        0        0        0 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/__init__.py
+-rw-r--r--   0        0        0     3161 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_account_divisions.py
+-rw-r--r--   0        0        0     2590 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_account_tags.py
+-rw-r--r--   0        0        0     3782 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_account_vacancy_request.py
+-rw-r--r--   0        0        0     2279 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_accounts.py
+-rw-r--r--   0        0        0     3614 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_applicant_on_vacancy.py
+-rw-r--r--   0        0        0     1214 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_applicant_on_vacancy_statuses.py
+-rw-r--r--   0        0        0    16569 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_applicants.py
+-rw-r--r--   0        0        0     2815 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_coworkers.py
+-rw-r--r--   0        0        0     4417 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_dictionaries.py
+-rw-r--r--   0        0        0     7692 2023-05-17 11:20:10.706725 huntflow_api_client-0.0.4/tests/test_entities/test_production_calendar.py
+-rw-r--r--   0        0        0     1039 2023-05-17 11:20:10.710725 huntflow_api_client-0.0.4/tests/test_entities/test_rejection_reasons.py
+-rw-r--r--   0        0        0    14337 2023-05-17 11:20:10.710725 huntflow_api_client-0.0.4/tests/test_entities/test_vacancies.py
+-rw-r--r--   0        0        0     4266 2023-05-17 11:20:10.710725 huntflow_api_client-0.0.4/tests/test_entities/test_vacancy_request.py
+-rw-r--r--   0        0        0     2534 2023-05-17 11:20:10.710725 huntflow_api_client-0.0.4/tests/test_entities/test_webhooks.py
+-rw-r--r--   0        0        0        0 2023-05-17 11:20:10.710725 huntflow_api_client-0.0.4/tests/test_errors/__init__.py
+-rw-r--r--   0        0        0     8007 2023-05-17 11:20:10.710725 huntflow_api_client-0.0.4/tests/test_errors/test_error_handlers.py
+-rw-r--r--   0        0        0        0 2023-05-17 11:20:10.710725 huntflow_api_client-0.0.4/tests/test_tokens/__init__.py
+-rw-r--r--   0        0        0     5630 2023-05-17 11:20:10.710725 huntflow_api_client-0.0.4/tests/test_tokens/test_access_token.py
+-rw-r--r--   0        0        0     1973 2023-05-17 11:20:10.710725 huntflow_api_client-0.0.4/tests/test_tokens/test_huntflow_token_proxy.py
+-rw-r--r--   0        0        0      824 1970-01-01 00:00:00.000000 huntflow_api_client-0.0.4/PKG-INFO
```

### Comparing `huntflow_api_client-0.0.2/LICENSE` & `huntflow_api_client-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.2/huntflow_api_client/api.py` & `huntflow_api_client-0.0.4/huntflow_api_client/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import logging
 from typing import Optional
 
 import httpx
 
-from huntflow_api_client.errors import (
-    InvalidAccessTokenError,
-    InvalidRefreshTokenError,
-    TokenExpiredError,
-)
+from huntflow_api_client.errors.errors import InvalidAccessTokenError, TokenExpiredError
+from huntflow_api_client.errors.response_hooks import raise_for_status
 from huntflow_api_client.tokens.proxy import AbstractTokenProxy, DummyHuntflowTokenProxy
 from huntflow_api_client.tokens.token import ApiToken
 
 logger = logging.getLogger(__name__)
 
 
 class HuntflowAPI:
@@ -45,14 +42,15 @@
         self.base_url = base_url
 
         self._autorefresh_tokens = auto_refresh_tokens
 
     @property
     def http_client(self) -> httpx.AsyncClient:
         http_client = httpx.AsyncClient(base_url=self.base_url)
+        http_client.event_hooks["response"] = [raise_for_status]
         return http_client
 
     async def request(  # type: ignore[no-untyped-def]
         self,
         method: str,
         path: str,
         *,
@@ -106,31 +104,16 @@
                 data=data,
                 files=files,
                 json=json,
                 params=params,
                 headers=headers,
                 timeout=timeout,
             )
-            await self._raise_token_expired(response)
-        return response
 
-    async def _raise_token_expired(self, response: httpx.Response) -> None:
-        if response.status_code != 401:
-            return
-        if not hasattr(response, "_content"):
-            await response.aread()
-        data = response.json()
-        try:
-            msg = data["errors"][0]["detail"]
-        except KeyError:
-            msg = None
-        if msg == "token_expired":
-            raise TokenExpiredError()
-        if msg == "Invalid access token":
-            raise InvalidAccessTokenError()
+        return response
 
     async def _run_token_refresh(self) -> None:
         # Why do we have to check if token was changed?
         # Consider the situation:
         # * we send 4 requests at the same time
         # * 3 of the 4 are returned with 401 token_expired errors
         # * 1 of the 4 is still waiting for response
@@ -146,22 +129,15 @@
         if await self._token_proxy.is_updated():
             return
         if not await self._token_proxy.lock_for_update():
             return
         try:
             refresh_data = await self._token_proxy.get_refresh_data()
             async with self.http_client as client:
-                response = await client.post(
-                    "/token/refresh",
-                    json=refresh_data,
-                )
-                if response.status_code == 404:
-                    raise InvalidRefreshTokenError()
-
-                response.raise_for_status()
+                response = await client.post("/token/refresh", json=refresh_data)
             await self._token_proxy.update(response.json())
         finally:
             await self._token_proxy.release_lock()
 
     async def _autorefresh_token_request(self, *args: str, **kwargs: str) -> httpx.Response:
         try:
             response = await self._request(*args, **kwargs)
```

### Comparing `huntflow_api_client-0.0.2/huntflow_api_client/entities/base.py` & `huntflow_api_client-0.0.4/huntflow_api_client/entities/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     @abc.abstractmethod
     async def get(self, *args, **kwargs):  # type: ignore
         pass
 
 
 class ListEntityMixin(abc.ABC):
     @abc.abstractmethod
-    async def list(self, *args, **kwargs):  # type: ignore  # noqa: A003
+    async def list(self, *args, **kwargs):  # type: ignore
         pass
 
 
 class CreateEntityMixin(abc.ABC):
     @abc.abstractmethod
     async def create(self, *args, **kwargs):  # type: ignore
         pass
```

### Comparing `huntflow_api_client-0.0.2/huntflow_api_client/tokens/locker.py` & `huntflow_api_client-0.0.4/huntflow_api_client/tokens/locker.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.2/huntflow_api_client/tokens/proxy.py` & `huntflow_api_client-0.0.4/huntflow_api_client/tokens/proxy.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.2/huntflow_api_client/tokens/storage.py` & `huntflow_api_client-0.0.4/huntflow_api_client/tokens/storage.py`

 * *Files identical despite different names*

### Comparing `huntflow_api_client-0.0.2/huntflow_api_client/tokens/token.py` & `huntflow_api_client-0.0.4/huntflow_api_client/tokens/token.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     last_refresh_timestamp: Optional[float] = 0.0
 
     @classmethod
     def from_dict(cls, dict_: Dict[str, Any]) -> "ApiToken":
         attrs = {field.name for field in fields(cls)}
         return cls(**{k: v for k, v in dict_.items() if k in attrs})
 
-    def dict(self) -> Dict[str, Any]:  # noqa: A003
+    def dict(self) -> Dict[str, Any]:
         return asdict(self)
```

