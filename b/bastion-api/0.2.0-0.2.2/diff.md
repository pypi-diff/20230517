# Comparing `tmp/bastion_api-0.2.0.tar.gz` & `tmp/bastion_api-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bastion_api-0.2.0.tar", max compression
+gzip compressed data, was "bastion_api-0.2.2.tar", max compression
```

## Comparing `bastion_api-0.2.0.tar` & `bastion_api-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,24 @@
--rw-r--r--   0        0        0      178 2023-04-10 12:05:00.739901 bastion_api-0.2.0/LICENSE
--rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 bastion_api-0.2.0/README.md
--rw-r--r--   0        0        0      311 2023-05-16 14:24:38.151875 bastion_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-16 09:32:45.417575 bastion_api-0.2.0/src/bastion_api/__init__.py
--rw-r--r--   0        0        0    33823 2023-05-16 14:23:37.488493 bastion_api-0.2.0/src/bastion_api/bastion.py
--rw-r--r--   0        0        0        0 2023-05-16 13:17:30.854465 bastion_api-0.2.0/src/bastion_api/dto/__init__.py
--rw-r--r--   0        0        0      173 2023-05-16 13:58:25.251623 bastion_api-0.2.0/src/bastion_api/dto/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      532 2023-05-16 13:58:25.255623 bastion_api-0.2.0/src/bastion_api/dto/__pycache__/config.cpython-310.pyc
--rw-r--r--   0        0        0      212 2023-05-16 11:36:00.337034 bastion_api-0.2.0/src/bastion_api/dto/config.py
--rw-r--r--   0        0        0      957 2023-05-16 14:23:37.380494 bastion_api-0.2.0/src/bastion_api/dto/device_dto.py
--rw-r--r--   0        0        0     2960 2023-05-16 14:20:20.754482 bastion_api-0.2.0/src/bastion_api/dto/old_dto.py
--rw-r--r--   0        0        0     1449 2023-05-16 13:27:28.275950 bastion_api-0.2.0/src/bastion_api/dto/organization_dto.py
--rw-r--r--   0        0        0     8747 2023-05-16 14:20:20.770482 bastion_api-0.2.0/src/bastion_api/dto/pass_dto.py
--rw-r--r--   0        0        0     2898 2023-05-16 13:27:28.295950 bastion_api-0.2.0/src/bastion_api/dto/person_dto.py
--rw-r--r--   0        0        0     2558 2023-05-16 14:17:31.752162 bastion_api-0.2.0/src/bastion_api/dto/points_dto.py
--rw-r--r--   0        0        0     4916 2023-05-16 14:20:20.766482 bastion_api-0.2.0/src/bastion_api/dto/support.py
--rw-r--r--   0        0        0      875 2023-05-16 12:44:48.791816 bastion_api-0.2.0/src/bastion_api/handlers.py
--rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 bastion_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      178 2023-04-10 12:05:00.739901 bastion_api-0.2.2/LICENSE
+-rw-r--r--   0        0        0      171 2023-04-10 11:56:09.609658 bastion_api-0.2.2/README.md
+-rw-r--r--   0        0        0      311 2023-05-17 12:18:44.392056 bastion_api-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-16 09:32:45.417575 bastion_api-0.2.2/src/bastion_api/__init__.py
+-rw-r--r--   0        0        0    34016 2023-05-17 12:18:28.392213 bastion_api-0.2.2/src/bastion_api/bastion.py
+-rw-r--r--   0        0        0        0 2023-05-16 13:17:30.854465 bastion_api-0.2.2/src/bastion_api/dto/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-16 13:58:25.251623 bastion_api-0.2.2/src/bastion_api/dto/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      536 2023-05-17 12:02:03.938377 bastion_api-0.2.2/src/bastion_api/dto/__pycache__/config.cpython-310.pyc
+-rw-r--r--   0        0        0      899 2023-05-17 12:02:03.910378 bastion_api-0.2.2/src/bastion_api/dto/__pycache__/device_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     1098 2023-05-17 12:02:03.910378 bastion_api-0.2.2/src/bastion_api/dto/__pycache__/organization_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     5532 2023-05-17 12:03:24.517481 bastion_api-0.2.2/src/bastion_api/dto/__pycache__/pass_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     1979 2023-05-17 12:02:03.914378 bastion_api-0.2.2/src/bastion_api/dto/__pycache__/person_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     2270 2023-05-17 12:02:03.914378 bastion_api-0.2.2/src/bastion_api/dto/__pycache__/points_dto.cpython-310.pyc
+-rw-r--r--   0        0        0     4478 2023-05-17 12:02:03.922378 bastion_api-0.2.2/src/bastion_api/dto/__pycache__/support.cpython-310.pyc
+-rw-r--r--   0        0        0      216 2023-05-17 12:02:03.646381 bastion_api-0.2.2/src/bastion_api/dto/config.py
+-rw-r--r--   0        0        0      957 2023-05-16 14:23:37.380494 bastion_api-0.2.2/src/bastion_api/dto/device_dto.py
+-rw-r--r--   0        0        0     2960 2023-05-16 14:20:20.754482 bastion_api-0.2.2/src/bastion_api/dto/old_dto.py
+-rw-r--r--   0        0        0     1449 2023-05-16 13:27:28.275950 bastion_api-0.2.2/src/bastion_api/dto/organization_dto.py
+-rw-r--r--   0        0        0     8775 2023-05-17 12:03:24.337483 bastion_api-0.2.2/src/bastion_api/dto/pass_dto.py
+-rw-r--r--   0        0        0     2898 2023-05-16 13:27:28.295950 bastion_api-0.2.2/src/bastion_api/dto/person_dto.py
+-rw-r--r--   0        0        0     2558 2023-05-16 14:17:31.752162 bastion_api-0.2.2/src/bastion_api/dto/points_dto.py
+-rw-r--r--   0        0        0     4916 2023-05-17 12:18:28.396213 bastion_api-0.2.2/src/bastion_api/dto/support.py
+-rw-r--r--   0        0        0      994 2023-05-17 12:18:28.360214 bastion_api-0.2.2/src/bastion_api/handlers.py
+-rw-r--r--   0        0        0      537 1970-01-01 00:00:00.000000 bastion_api-0.2.2/PKG-INFO
```

### Comparing `bastion_api-0.2.0/src/bastion_api/bastion.py` & `bastion_api-0.2.2/src/bastion_api/bastion.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,31 @@
-from typing import List, Dict
+from typing import Dict, List
 from datetime import datetime as dt, timedelta as td
-
-from aiohttp import ClientResponse, ClientSession
 from pydantic import BaseModel
+from aiohttp import ClientResponse, ClientSession
 from loguru import logger
 
-
-from src.bastion_api.dto.config import BastionConfig
 from src.bastion_api.dto.device_dto import DeviceDto
 from src.bastion_api.dto.organization_dto import OrgDto, DepartDto
 from src.bastion_api.dto.pass_dto import CardEventDto, CardDto, AttendanceDto, PassDto, MatValuePassDto, CarPassDto
 from src.bastion_api.dto.person_dto import PersonDto
 from src.bastion_api.dto.points_dto import EntryPointDto, AccessLevelDto, ControlAreaDto, AccessPointDto
 from src.bastion_api.dto.support import DictValDto, PassBriefDto
-
-from src.bastion_api.handlers import BastionIntegrationError
+from src.bastion_api.handlers import BastionIntegrationError, _handle_response
+from src.bastion_api.dto.config import IntegrationConfig
 
 
 class Bastion:
     session: ClientSession
+    config: BaseModel
     bastion_servers: []
     _code_for_url: str = ""
+    config: IntegrationConfig
 
-    def __init__(self, bastion_config: BastionConfig):
-        self.config = bastion_config
-        self.session = ClientSession()
-
-    async def _send_noods(self, method: str, url: str, data: BaseModel | None | Dict = None) -> ClientResponse:
+    async def _wrap_response(self, method: str, url: str, data: BaseModel | None | Dict = None) -> ClientResponse:
         logger.warning(url)
         if self.session:
             async with self.session.request(method.upper(),
                                             url=f"http://{self.config.iks_host}:{self.config.iks_port}{url}",
                                             json=data.dict() if isinstance(data, BaseModel) else data if isinstance(
                                                 data, Dict) else None) as response:
                 await response.read()
@@ -44,119 +39,116 @@
                         cook["expires"] = (dt.now() + td(days=1)).strftime("%a, %d %b %Y %H:%M:%S GMT")
                     self.session.cookie_jar.update_cookies(response.cookies)
                 if response.status != 200:
                     raise BastionIntegrationError(message=f"Bad response status:  {response.status}")
 
         return response
 
-    async def _handle_response(self, response, dto):
-        model_list = []
-        for info in response:
-            model_list.append(dto(**info))
-        return model_list
+    # ________________________________________________________________________________________________________
 
-    async def init(self, search_servers: str = None):
-        """Указываем сервер бастиона для работы.
-                Если указан None - будут использованы все найденные сервера
-                Необходима авторизация за оператора"""
+    async def connect_to_bastion_iks(self, search_servers: str = None):
+        """Функция осуществляет подключение к Бастион ИКС согласно файлу конфигурации"""
 
-        response = await(await self._send_noods(method="POST", url="/api/Login",
-                                                data={"opername": f"{self.config.iks_operator_login}",
-                                                      "password": f"{self.config.iks_operator_password}"})).text()
+        response = await(await self._wrap_response(method="POST", url="/api/Login",
+                                                   data={"opername": f"{self.config.iks_operator_login}",
+                                                         "password": f"{self.config.iks_operator_password}"})).text()
         if "info" in self.config.log:
             logger.info(response)
 
-        self.bastion_servers = (await (await self._send_noods(method="GET", url="/api/GetServers")).json())
+        self.bastion_servers = (await (await self._wrap_response(method="GET", url="/api/GetServers")).json())
         if search_servers:
             if search_servers.lower() in self.bastion_servers.servers_code:
                 self.bastion_servers.servers_code = search_servers.lower()
             else:
                 raise BastionIntegrationError(message="Some server not found")
 
         for server_code in (
                 self.bastion_servers if self.bastion_servers.__class__ == "list" else [
                     self.bastion_servers]):
             self._code_for_url = self._code_for_url + f"srvCode={server_code}&"
 
     # ________________________________________________________________________________________________________
 
     async def logout(self):
-        await self._send_noods(method="POST", url="/api/LogOff")
+        await self._wrap_response(method="POST", url="/api/LogOff")
 
     # ________________________________________________________________________________________________________
 
     async def get_version(self) -> str:
         """Метод, возвращающий строку с версией модуля"""
-        response = await (await self._send_noods(method="GET", url="/api/GetVersion")).text()
+        response = await (await self._wrap_response(method="GET", url="/api/GetVersion")).text()
         if "info" in self.config.log:
             logger.info(response)
         return response
 
     async def check_connection(self) -> str:
         """Метод предназначен для проверки связи с одним или несколькими серверами."""
-        response = await (await self._send_noods(method="GET", url=f"/api/CheckConnection?{self._code_for_url}")).text()
+        response = await (
+            await self._wrap_response(method="GET", url=f"/api/CheckConnection?{self._code_for_url}")).text()
         if "info" in self.config.log:
             logger.info(response)
         return response
 
     # ________________________________________________________________________________________________________
 
     async def get_entity_points(self) -> List[EntryPointDto]:
         """Метод, предназначенный для получения информации о точках прохода"""
-        response = await (await self._send_noods(method="GET", url=f"/api/GetEntryPoints?{self._code_for_url}")).json()
-        model_list = await self._handle_response(response, EntryPointDto)
+        response = await (
+            await self._wrap_response(method="GET", url=f"/api/GetEntryPoints?{self._code_for_url}")).json()
+        model_list = await _handle_response(response, EntryPointDto)
         if "info" in self.config.log:
             logger.info(response)
         return model_list
 
     async def get_access_level(self) -> List[AccessLevelDto]:
         """Метод, предназначенный для получения информации об уровнях доступа"""
-        response = await (await self._send_noods(method="GET", url=f"/api/GetAccessLevels?{self._code_for_url}")).json()
-        model_list = await self._handle_response(response, AccessLevelDto)
+        response = await (
+            await self._wrap_response(method="GET", url=f"/api/GetAccessLevels?{self._code_for_url}")).json()
+        model_list = await _handle_response(response, AccessLevelDto)
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     # ________________________________________________________________________________________________________
 
     async def get_dict_value(self, category: int = "") -> List[DictValDto]:
         """Метод предназначен для запроса списка словарных значений с фильтрацией
         по категории.
         category = Категория словарных значений, информацию о которых требуется получить
         """
-        response = await (await self._send_noods(method="GET", url=f"/api/GetDictVals?{self._code_for_url}"
-                                                                   f"category={category}")).json()
-        model_list = await self._handle_response(response, DictValDto)
+        response = await (await self._wrap_response(method="GET", url=f"/api/GetDictVals?{self._code_for_url}"
+                                                                      f"category={category}")).json()
+        model_list = await _handle_response(response, DictValDto)
         if "info" in self.config.log:
             logger.info(response)
-        return response
+        return model_list
 
     async def get_card_events(self, card_info: CardDto) -> List[CardEventDto]:
         """Метод предназначен для получения списка событий, произошедших с конкретной картой доступа"""
 
-        response = await(await self._send_noods(method="GET",
-                                                url=f"/api/GetCardEvents?{self._code_for_url}"
-                                                    f"cardCode={card_info.card_code}&"
-                                                    f"dateFrom={card_info.date_from}&"
-                                                    f"dateTo={card_info.date_to}")).json()
-        model_list = await self._handle_response(response, CardEventDto)
+        response = await(await self._wrap_response(method="GET",
+                                                   url=f"/api/GetCardEvents?{self._code_for_url}"
+                                                       f"cardCode={card_info.card_code}&"
+                                                       f"dateFrom={card_info.date_from}&"
+                                                       f"dateTo={card_info.date_to}")).json()
+        model_list = await _handle_response(response, CardEventDto)
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def get_attendance(self, card_info: CardDto) -> List[AttendanceDto]:
         """Метод предназначен для получения списка посещений с конкретной картой доступа,
          либо со всеми катами доступа с сервера"""
 
-        response = await (await self._send_noods(method="GET",
-                                                 url=f"/api/GetAttendance?{self._code_for_url}"
-                                                     f"cardCode={card_info.card_code}&"
-                                                     f"dateFrom={card_info.date_from}&"
-                                                     f"dateTo={card_info.date_to}")).json()
-        model_list = await self._handle_response(response, AttendanceDto)
+        response = await (await self._wrap_response(method="GET",
+                                                    url=f"/api/GetAttendance?{self._code_for_url}"
+                                                        f"cardCode={card_info.card_code}&"
+                                                        f"dateFrom={card_info.date_from}&"
+                                                        f"dateTo={card_info.date_to}")).json()
+        model_list = await _handle_response(response, AttendanceDto)
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     # ________________________________________________________________________________________________________
 
     async def create_or_update_pass(self, new_pass_card: PassDto.NewPassPerson, use_access_level: bool = ''):
@@ -171,338 +163,343 @@
                                  По умолчанию значение флага – false,
                                   в этом случае используются данные поля EntryPoints модели Pass.
                                   стр. 29 документации пп 5.14
         """
         if not new_pass_card.entryPoints and not new_pass_card.accessLevels:
             raise BastionIntegrationError(message="Please input access level or entry points")
 
-        response = await (await self._send_noods(method="PUT",
-                                                 url=f"/api/PutPass?{self._code_for_url}"
-                                                     f"useAccessLevelsInsteadOfEntryPoints={use_access_level}",
-                                                 data=new_pass_card)).text()
+        response = await (await self._wrap_response(method="PUT",
+                                                    url=f"/api/PutPass?{self._code_for_url}"
+                                                        f"useAccessLevelsInsteadOfEntryPoints={use_access_level}",
+                                                    data=new_pass_card)).text()
         if "info" in self.config.log:
             logger.info(response)
         return response
 
     async def return_pass_for_card(self, _pass: PassDto.ReturnPassForCardCode, ) -> str:
         """Метод предназначен для создания или редактирования КД,
          а также для создания/редактирования заявки на пропуск"""
 
-        response = await (await self._send_noods(method="PUT",
-                                                 url=f"/api/PutPass?{self._code_for_url}"
-                                                     f"useAccessLevelsInsteadOfEntryPoints=",
-                                                 data=_pass)).text()
+        response = await (await self._wrap_response(method="PUT",
+                                                    url=f"/api/PutPass?{self._code_for_url}"
+                                                        f"useAccessLevelsInsteadOfEntryPoints=",
+                                                    data=_pass)).text()
         if "info" in self.config.log:
             logger.info(response)
         return response
 
     async def get_pass(self, get_pass_info: PassDto.ReturnPass) -> List[PassDto]:
         """Метод предназначен для получения списка пропусков
         с фильтрацией по их статусу и типу с сервера"""
-        response = await (await self._send_noods(method="GET",
-                                                 url=f"/api/GetPasses?{self._code_for_url}"
-                                                     f"cardStatus={get_pass_info.card_status}&"
-                                                     f"passType={get_pass_info.pass_type}&"
-                                                     f"withoutPhoto={get_pass_info.without_photo}&"
-                                                     f"startFrom={get_pass_info.start_numer}&"
-                                                     f"maxCount={get_pass_info.max_count}")).json()
-        model_list = await self._handle_response(response, PassDto)
+        response = await (await self._wrap_response(method="GET",
+                                                    url=f"/api/GetPasses?{self._code_for_url}"
+                                                        f"cardStatus={get_pass_info.card_status}&"
+                                                        f"passType={get_pass_info.pass_type}&"
+                                                        f"withoutPhoto={get_pass_info.without_photo}&"
+                                                        f"startFrom={get_pass_info.start_numer}&"
+                                                        f"maxCount={get_pass_info.max_count}")).json()
+        model_list = await _handle_response(response, PassDto)
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def get_passes_by_person(self, person_info: PersonDto, without_photo: bool) -> List[PassDto]:
         """Метод предназначен для получения списка пропусков любых статусов"""
 
-        response = await (await self._send_noods(method="GET",  # Dont change url parameters
-                                                 url=f"/api/GetPassesByPerson?{self._code_for_url}"
-                                                     f"name={person_info.name}&"
-                                                     f"firstname={person_info.firstName}&"
-                                                     f"secondname={person_info.secondName}&"
-                                                     f"birthDate={person_info.birthDate}&"
-                                                     f"withoutPhoto={without_photo}")).json()
+        response = await (await self._wrap_response(method="GET",  # Dont change url parameters
+                                                    url=f"/api/GetPassesByPerson?{self._code_for_url}"
+                                                        f"name={person_info.name}&"
+                                                        f"firstname={person_info.firstName}&"
+                                                        f"secondname={person_info.secondName}&"
+                                                        f"birthDate={person_info.birthDate}&"
+                                                        f"withoutPhoto={without_photo}")).json()
 
-        model_list = await self._handle_response(response, PassDto)
+        model_list = await _handle_response(response, PassDto)
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def get_pass_by_card(self, card_code: str, without_photo: bool = "") -> List[PassDto]:
         """Метод предназначен для получения списка пропусков любых статусов, по которым когда-либо выдавалась карта
         without_photo: bool - true если фотографии возвращать не нужно"""
-        response = await (await self._send_noods(method="GET",
-                                                 url=f"/api/GetPassesByCardCode?{self._code_for_url}"
-                                                     f"cardCode={card_code}&"
-                                                     f"withoutPhoto={without_photo}")).json()
-        model_list = await self._handle_response(response, PassDto)
+        response = await (await self._wrap_response(method="GET",
+                                                    url=f"/api/GetPassesByCardCode?{self._code_for_url}"
+                                                        f"cardCode={card_code}&"
+                                                        f"withoutPhoto={without_photo}")).json()
+        model_list = await _handle_response(response, PassDto)
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def get_pass_count(self, card_status: int = "", pass_type: int = "") -> str:
         """Метод предназначен для получения общего количества пропусков"""
-        response = await (await self._send_noods(method="GET",
-                                                 url=f"/api/GetPassCount?{self._code_for_url}"
-                                                     f"cardStatus={card_status}&"
-                                                     f"passType={pass_type}")).text()
+        response = await (await self._wrap_response(method="GET",
+                                                    url=f"/api/GetPassCount?{self._code_for_url}"
+                                                        f"cardStatus={card_status}&"
+                                                        f"passType={pass_type}")).text()
 
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def block_pass(self, card_code: str, block_reason: str) -> str:
         """Метод предназначен для блокировки КД"""
-        response = await (await self._send_noods(method="GET",
-                                                 url=f"/api/BlockPass?{self._code_for_url}"
-                                                     f"cardCode={card_code}&"
-                                                     f"blockReason={block_reason}")).text()
+        response = await (await self._wrap_response(method="GET",
+                                                    url=f"/api/BlockPass?{self._code_for_url}"
+                                                        f"cardCode={card_code}&"
+                                                        f"blockReason={block_reason}")).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def unblock_pass(self, card_code: str) -> str:
         """Метод предназначен для разблокировки КД"""
-        response = await (await self._send_noods(method="GET", url=f"/api/UnblockPass?{self._code_for_url}"
-                                                                   f"cardCode={card_code}")).text()
+        response = await (await self._wrap_response(method="GET", url=f"/api/UnblockPass?{self._code_for_url}"
+                                                                      f"cardCode={card_code}")).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def archive_pass(self, card_code: str) -> str:
         """Метод предназначен для переноса в архив карты доступа"""
-        response = await (await self._send_noods(method="GET", url=f"/api/ReturnPass?{self._code_for_url}"
-                                                                   f"cardCode={card_code}")).text()
+        response = await (await self._wrap_response(method="GET", url=f"/api/ReturnPass?{self._code_for_url}"
+                                                                      f"cardCode={card_code}")).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def issue_pass(self, person_info: PersonDto, pass_type: int, card_code: str) -> str:
         """Метод предназначен для выдачи КД по ранее созданной заявке на пропуск"""
-        response = await (await self._send_noods(method="GET",
-                                                 url=f"/api/IssuePass?{self._code_for_url}"
-                                                     f"name={person_info.name}&"
-                                                     f"firstname={person_info.firstName}&"
-                                                     f"secondname={person_info.secondName}&"
-                                                     f"birthDate={person_info.birthDate}&"
-                                                     f"passType={pass_type}&"
-                                                     f"cardCode={card_code}")).text()
+        response = await (await self._wrap_response(method="GET",
+                                                    url=f"/api/IssuePass?{self._code_for_url}"
+                                                        f"name={person_info.name}&"
+                                                        f"firstname={person_info.firstName}&"
+                                                        f"secondname={person_info.secondName}&"
+                                                        f"birthDate={person_info.birthDate}&"
+                                                        f"passType={pass_type}&"
+                                                        f"cardCode={card_code}")).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>  <srvN> – код сервера, а <resultN> – результат выполнения операции.
 
     async def get_material_pass_by_pass(self, pass_id: int) -> str:
         """Метод предназначен для выдачи материального пропуска по ранее созданной заявке на сервере"""
         response = await (
-            await self._send_noods(method="GET", url=f"/api/IssueMVPass?{self._code_for_url}passid={pass_id}")).json()
+            await self._wrap_response(method="GET",
+                                      url=f"/api/IssueMVPass?{self._code_for_url}passid={pass_id}")).json()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def ban_material_pass(self, pass_id: int) -> str:
         """Метод предназначен для изъятия материального пропуска на сервере"""
-        response = await (await self._send_noods(method="GET",
-                                                 url=f"/api/WithdrawMVPass?{self._code_for_url}passid={pass_id}")).json()
+        response = await (await self._wrap_response(method="GET",
+                                                    url=f"/api/WithdrawMVPass?{self._code_for_url}passid={pass_id}")).json()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     # ________________________________________________________________________________________________________
 
     async def get_organisation(self, org_filter: str = "") -> List[OrgDto]:
         """Метод предназначен для получения списка организаций"""
-        response = await (await self._send_noods(method="GET", url=f"/api/GetOrgs?{self._code_for_url}"
-                                                                   f"filter={org_filter}")).json()
-        model_list = await self._handle_response(response, OrgDto)
+        response = await (await self._wrap_response(method="GET", url=f"/api/GetOrgs?{self._code_for_url}"
+                                                                      f"filter={org_filter}")).json()
+        model_list = await _handle_response(response, OrgDto)
 
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def create_organization(self, organization: OrgDto) -> str:
         """Метод предназначен для добавления организации """
         response = await (
-            await self._send_noods(method="PUT", url=f"/api/PutOrg?{self._code_for_url}", data=organization)).text()
+            await self._wrap_response(method="PUT", url=f"/api/PutOrg?{self._code_for_url}", data=organization)).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def update_organization(self, organization: OrgDto, organization_new_name: str) -> str:
         """Метод предназначен для переименования организации на всех серверах, добавленных в схему интеграции, либо на одном сервере, код которого передан в качестве входного параметра."""
-        response = await (await self._send_noods(method="POST",
-                                                 url=f"/api/UpdateOrg?{self._code_for_url}"
-                                                     f"orgNewName={organization_new_name}",
-                                                 data=organization)).text()
+        response = await (await self._wrap_response(method="POST",
+                                                    url=f"/api/UpdateOrg?{self._code_for_url}"
+                                                        f"orgNewName={organization_new_name}",
+                                                    data=organization)).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def delete_organization(self, organization: OrgDto) -> str:
         """Метод предназначен для удаления организации (вместе со всеми дочерними организациями и подразделениями) на всех серверах, добавленных в схему интеграции, либо на одном сервере, код которого передан в качестве входного параметра."""
         response = await (
-            await self._send_noods(method="POST", url=f"/api/DeleteOrg?{self._code_for_url}", data=organization)).text()
+            await self._wrap_response(method="POST", url=f"/api/DeleteOrg?{self._code_for_url}",
+                                      data=organization)).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     # ________________________________________________________________________________________________________
 
     async def get_department(self, department_name: str = "") -> List[DepartDto]:
         """Метод предназначен для получения списка подразделений (всех, либо принадлежащих организации, имя которой передано в качестве входного параметра)"""
-        response = await (await self._send_noods(method="GET",
-                                                 url=f"/api/GetDeparts?{self._code_for_url}parentOrgName={department_name}")).json()
-        model_list = await self._handle_response(response, DepartDto)
+        response = await (await self._wrap_response(method="GET",
+                                                    url=f"/api/GetDeparts?{self._code_for_url}parentOrgName={department_name}")).json()
+        model_list = await _handle_response(response, DepartDto)
 
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def create_department(self, department: DepartDto) -> str:
         """Метод предназначен для добавления подразделения"""
         response = await (
-            await self._send_noods(method="PUT", url=f"/api/PutDepart?{self._code_for_url}", data=department)).text()
+            await self._wrap_response(method="PUT", url=f"/api/PutDepart?{self._code_for_url}", data=department)).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def update_department(self, department: DepartDto, new_department_name: str) -> str:
         """Метод предназначен для переименования подразделения"""
-        response = await (await self._send_noods(method="POST",
-                                                 url=f"/api/UpdateDepart?{self._code_for_url}departNewName={new_department_name}",
-                                                 data=department)).text()
+        response = await (await self._wrap_response(method="POST",
+                                                    url=f"/api/UpdateDepart?{self._code_for_url}departNewName={new_department_name}",
+                                                    data=department)).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def delete_department(self, department: DepartDto) -> str:
         """Метод предназначен для удаления подразделения"""
-        response = await (await self._send_noods(method="POST", url=f"/api/DeleteDepart?{self._code_for_url}",
-                                                 data=department)).text()
+        response = await (await self._wrap_response(method="POST", url=f"/api/DeleteDepart?{self._code_for_url}",
+                                                    data=department)).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     # ________________________________________________________________________________________________________
 
     async def put_material_pass(self, mat_value: MatValuePassDto, claim: bool = "", ) -> str:
         """Метод предназначен для создания или редактирования материального пропуска, а также для создания/редактирования заявки на материальный пропуск
         claim - Флаг, определяющий, будет создан выданный материальный пропуск, либо же будет создана заявка на пропуск
             """
         response = await (
-            await self._send_noods(method="PUT", url=f"/api/PutMVPass?{self._code_for_url}issuePass={claim}",
-                                   data=mat_value)).text()
+            await self._wrap_response(method="PUT", url=f"/api/PutMVPass?{self._code_for_url}issuePass={claim}",
+                                      data=mat_value)).text()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def get_material_pass(self, status: int = "") -> List[MatValuePassDto]:
         """Метод предназначен для получения списка материальных пропусков с фильтрацией по их статусу с сервера
         status: int - Статус возвращаемых материальных пропусков. Значение параметра может быть пустым, в этом случае будут возвращены пропуска с любым статусом
         """
-        response = await(await self._send_noods(method="GET",
-                                                url=f"/api/GetMVPasses?{self._code_for_url}status={status}")).json()
-        model_list = await self._handle_response(response, MatValuePassDto)
+        response = await(await self._wrap_response(method="GET",
+                                                   url=f"/api/GetMVPasses?{self._code_for_url}status={status}")).json()
+        model_list = await _handle_response(response, MatValuePassDto)
 
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def get_material_pass_by_person(self, pass_dto: PassBriefDto) -> List[MatValuePassDto]:
         """Метод предназначен для получения списка материальных пропусков с фильтрацией по персональному пропуску с сервера, код которого передан в качестве входного параметра"""
 
         response = await (
-            await self._send_noods(method="POST", url=f"/api/GetMVPassesByPersonPass?{self._code_for_url}",
-                                   data=pass_dto)).json()
+            await self._wrap_response(method="POST", url=f"/api/GetMVPassesByPersonPass?{self._code_for_url}",
+                                      data=pass_dto)).json()
 
-        model_list = await self._handle_response(response, MatValuePassDto)
+        model_list = await _handle_response(response, MatValuePassDto)
 
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     # ________________________________________________________________________________________________________
 
     async def put_car_pass(self, car_pass: CarPassDto, claim: bool = "") -> str:
         """Метод предназначен для создания или редактирования транспортного пропуска, а также для создания/редактирования заявки на транспортный пропуск"""
         response = await (
-            await self._send_noods(method="PUT", url=f"/api/PutCarPass?{self._code_for_url}issuePass={claim}",
-                                   data=car_pass)).json()
+            await self._wrap_response(method="PUT", url=f"/api/PutCarPass?{self._code_for_url}issuePass={claim}",
+                                      data=car_pass)).json()
 
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def get_car_pass(self, status: int = "") -> List[CarPassDto]:
         """Метод предназначен для получения списка транспортных пропусков с фильтрацией по их статусу
         status: int - Статус возвращаемых транспортных пропусков. Значение параметра может быть пустым, в этом случае будут возвращены пропуска с любым статусом"""
 
         response = await (
-            await self._send_noods(method="GET", url=f"/api/GetCarPasses?{self._code_for_url}status={status}")).json()
+            await self._wrap_response(method="GET",
+                                      url=f"/api/GetCarPasses?{self._code_for_url}status={status}")).json()
 
-        model_list = await self._handle_response(response, CarPassDto)
+        model_list = await _handle_response(response, CarPassDto)
 
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def get_car_pass_by_person_pass(self, pass_dto: PassBriefDto) -> List[CarPassDto]:
         """Метод предназначен для получения списка транспортных пропусков с фильтрацией по персональному пропуску"""
 
         response = await (
-            await self._send_noods(method="POST", url=f"/api/GetCarPassesByPersonPass?{self._code_for_url}",
-                                   data=pass_dto)).json()
+            await self._wrap_response(method="POST", url=f"/api/GetCarPassesByPersonPass?{self._code_for_url}",
+                                      data=pass_dto)).json()
 
-        model_list = await self._handle_response(response, CarPassDto)
+        model_list = await _handle_response(response, CarPassDto)
 
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def get_car_pass_by_claim(self, pass_id: int) -> str:
         """Метод предназначен для выдачи транспортного пропуска по ранее созданной заявке"""
         response = await (
-            await self._send_noods(method="GET", url=f"/api/IssueCarPass?{self._code_for_url}passid={pass_id}")).json()
+            await self._wrap_response(method="GET",
+                                      url=f"/api/IssueCarPass?{self._code_for_url}passid={pass_id}")).json()
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     async def banned_car_pass(self, pass_id: int) -> str:
         """Метод предназначен для изъятия транспортного пропуска на сервере, код которого передан в качестве входного параметра."""
-        response = await (await self._send_noods(method="GET",
-                                                 url=f"/api/WithdrawCarPass?{self._code_for_url}passid={pass_id}")).json()
+        response = await (await self._wrap_response(method="GET",
+                                                    url=f"/api/WithdrawCarPass?{self._code_for_url}passid={pass_id}")).json()
 
         if "info" in self.config.log:
             logger.info(response)
         return response  # Метод возвращает строку в следующем формате: <srvN>:<resultN>
 
     # ________________________________________________________________________________________________________
 
     async def get_devices(self, driver_id: int = "", device_type: int = "") -> List[DeviceDto]:
         """Метод предназначен для получения набора устройств, добавленных в систему на сервере
         driver_id: int - Код типа драйвера, устройства которого необходимо получить. Значение параметра может быть пустым, в таком случае будут возвращены устройства всех драйверов
         device_type: int - Код типа устройства. В случае передачи непустого значения параметра будут возвращены устройства только данного типа. Значение параметра может быть пустым."""
-        response = await ((await self._send_noods(method="GET",
-                                                  url=f"/api/GetDevices?{self._code_for_url}driverId={driver_id}&deviceType={device_type}"))).json()
+        response = await ((await self._wrap_response(method="GET",
+                                                     url=f"/api/GetDevices?{self._code_for_url}driverId={driver_id}&deviceType={device_type}"))).json()
 
-        model_list = await self._handle_response(response, DeviceDto)
+        model_list = await _handle_response(response, DeviceDto)
 
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def get_control_area(self) -> List[ControlAreaDto]:
         """Метод, предназначенный для получения информации об областях контроля"""
         response = await (
-            await self._send_noods(method="GET", url=f"/api/GetControlAreas?{self._code_for_url}")).json()
-        model_list = await self._handle_response(response, ControlAreaDto)
+            await self._wrap_response(method="GET", url=f"/api/GetControlAreas?{self._code_for_url}")).json()
+        model_list = await _handle_response(response, ControlAreaDto)
 
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
 
     async def get_access_point(self) -> List[AccessPointDto]:
         """Метод, предназначенный для получения информации об точках доступа"""
-        response = await (await self._send_noods(method="GET", url=f"/api/GetAccessPoints?{self._code_for_url}")).json()
-        model_list = await self._handle_response(response, AccessPointDto)
+        response = await (
+            await self._wrap_response(method="GET", url=f"/api/GetAccessPoints?{self._code_for_url}")).json()
+        model_list = await _handle_response(response, AccessPointDto)
 
         if "info" in self.config.log:
             logger.info(model_list)
         return model_list
```

### Comparing `bastion_api-0.2.0/src/bastion_api/dto/__pycache__/config.cpython-310.pyc` & `bastion_api-0.2.2/src/bastion_api/dto/__pycache__/config.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue May 16 11:36:00 2023 UTC, .py size: 212 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-00000000: 6f0d 0d0a 0000 0000 a06a 6364 d400 0000  o........jcd....
+00000000: 6f0d 0d0a 0000 0000 3bc2 6464 d800 0000  o.......;.dd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2000 0000 6400  .....@...s ...d.
 00000030: 6401 6c00 6d01 5a01 0100 4700 6402 6403  d.l.m.Z...G.d.d.
 00000040: 8400 6403 6501 8303 5a02 6404 5300 2905  ..d.e...Z.d.S.).
 00000050: e900 0000 0029 01da 0942 6173 654d 6f64  .....)...BaseMod
 00000060: 656c 6300 0000 0000 0000 0000 0000 0000  elc.............
 00000070: 0000 0003 0000 0040 0000 0073 3a00 0000  .......@...s:...
 00000080: 6500 5a01 6400 5a02 5500 6503 6504 6401  e.Z.d.Z.U.e.e.d.
 00000090: 3c00 6505 6504 6402 3c00 6503 6504 6403  <.e.e.d.<.e.e.d.
 000000a0: 3c00 6503 6504 6404 3c00 6506 6503 1900  <.e.e.d.<.e.e...
-000000b0: 6504 6405 3c00 6406 5300 2907 da0d 4261  e.d.<.d.S.)...Ba
-000000c0: 7374 696f 6e43 6f6e 6669 67da 0869 6b73  stionConfig..iks
-000000d0: 5f68 6f73 74da 0869 6b73 5f70 6f72 74da  _host..iks_port.
-000000e0: 1269 6b73 5f6f 7065 7261 746f 725f 6c6f  .iks_operator_lo
-000000f0: 6769 6eda 1569 6b73 5f6f 7065 7261 746f  gin..iks_operato
-00000100: 725f 7061 7373 776f 7264 da03 6c6f 674e  r_password..logN
-00000110: 2907 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-00000120: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-00000130: 6e61 6d65 5f5f da03 7374 72da 0f5f 5f61  name__..str..__a
-00000140: 6e6e 6f74 6174 696f 6e73 5f5f da03 696e  nnotations__..in
-00000150: 74da 046c 6973 74a9 0072 1000 0000 7210  t..list..r....r.
-00000160: 0000 00fa 4e2f 686f 6d65 2f64 6d69 7472  ....N/home/dmitr
-00000170: 792f 5079 6368 6172 6d50 726f 6a65 6374  y/PycharmProject
-00000180: 732f 4261 7374 696f 6e5f 696e 7465 6772  s/Bastion_integr
-00000190: 6174 696f 6e2f 7372 632f 6261 7374 696f  ation/src/bastio
-000001a0: 6e5f 6170 692f 6474 6f2f 636f 6e66 6967  n_api/dto/config
-000001b0: 2e70 7972 0300 0000 0400 0000 730c 0000  .pyr........s...
-000001c0: 000a 0008 0108 0108 0108 0110 0172 0300  .............r..
-000001d0: 0000 4e29 03da 0870 7964 616e 7469 6372  ..N)...pydanticr
-000001e0: 0200 0000 7203 0000 0072 1000 0000 7210  ....r....r....r.
-000001f0: 0000 0072 1000 0000 7211 0000 00da 083c  ...r....r......<
-00000200: 6d6f 6475 6c65 3e01 0000 0073 0400 0000  module>....s....
-00000210: 0c00 1403                                ....
+000000b0: 6504 6405 3c00 6406 5300 2907 da11 496e  e.d.<.d.S.)...In
+000000c0: 7465 6772 6174 696f 6e43 6f6e 6669 67da  tegrationConfig.
+000000d0: 0869 6b73 5f68 6f73 74da 0869 6b73 5f70  .iks_host..iks_p
+000000e0: 6f72 74da 1269 6b73 5f6f 7065 7261 746f  ort..iks_operato
+000000f0: 725f 6c6f 6769 6eda 1569 6b73 5f6f 7065  r_login..iks_ope
+00000100: 7261 746f 725f 7061 7373 776f 7264 da03  rator_password..
+00000110: 6c6f 674e 2907 da08 5f5f 6e61 6d65 5f5f  logN)...__name__
+00000120: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000130: 7175 616c 6e61 6d65 5f5f da03 7374 72da  qualname__..str.
+00000140: 0f5f 5f61 6e6e 6f74 6174 696f 6e73 5f5f  .__annotations__
+00000150: da03 696e 74da 046c 6973 74a9 0072 1000  ..int..list..r..
+00000160: 0000 7210 0000 00fa 4e2f 686f 6d65 2f64  ..r.....N/home/d
+00000170: 6d69 7472 792f 5079 6368 6172 6d50 726f  mitry/PycharmPro
+00000180: 6a65 6374 732f 4261 7374 696f 6e5f 696e  jects/Bastion_in
+00000190: 7465 6772 6174 696f 6e2f 7372 632f 6261  tegration/src/ba
+000001a0: 7374 696f 6e5f 6170 692f 6474 6f2f 636f  stion_api/dto/co
+000001b0: 6e66 6967 2e70 7972 0300 0000 0400 0000  nfig.pyr........
+000001c0: 730c 0000 000a 0008 0108 0108 0108 0110  s...............
+000001d0: 0172 0300 0000 4e29 03da 0870 7964 616e  .r....N)...pydan
+000001e0: 7469 6372 0200 0000 7203 0000 0072 1000  ticr....r....r..
+000001f0: 0000 7210 0000 0072 1000 0000 7211 0000  ..r....r....r...
+00000200: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+00000210: 0400 0000 0c00 1403                      ........
```

### Comparing `bastion_api-0.2.0/src/bastion_api/dto/device_dto.py` & `bastion_api-0.2.2/src/bastion_api/dto/device_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.0/src/bastion_api/dto/old_dto.py` & `bastion_api-0.2.2/src/bastion_api/dto/old_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.0/src/bastion_api/dto/organization_dto.py` & `bastion_api-0.2.2/src/bastion_api/dto/organization_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.0/src/bastion_api/dto/pass_dto.py` & `bastion_api-0.2.2/src/bastion_api/dto/pass_dto.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,21 +28,21 @@
         """return_pass_for_card"""
         cardCode: str = ""  # Код карты доступа (может быть пустым в том случае если объект представляет набор данных заявки на пропуск)
         personData: PersonDto  # Набор персональных данных пропуска
         pincode: int  # Pin-код пропуска
         passCat: str  # Категория пропуска
 
 
-class ReturnPass(BaseModel):
-    """get_pass"""
-    card_status: int = ""  # Статус возвращаемых пропусков. Значение параметра может быть пустым, в этом случае будут возвращены пропуска с любым статусом
-    pass_type: int = ""  # Тип возвращаемых пропусков. Значение параметра может быть пустым, в этом случае будут возвращены пропуска всех типов (Постоянный - 1, Временный - 2, Разовый - 4)
-    without_photo: bool = ""  # Флаг, определяющий, нужно ли возвращать фотографии владельцев пропусков (true если фотографии возвращать не нужно).
-    start_numer: int = ""  # Порядковый номер, начиная с которого будут возвращены пропуска (постраничный вывод). Значение параметра может быть пустым, в этом случае будут возвращаться пропуска начиная с первого
-    max_count: int = ""  # Максимальное количество пропусков, которое будет возвращено методом (постраничный вывод). Значение параметра может быть пустым, в этом случае количество возвращаемых пропусков ограничиваться не будет
+    class ReturnPass(BaseModel):
+        """get_pass"""
+        card_status: int = ""  # Статус возвращаемых пропусков. Значение параметра может быть пустым, в этом случае будут возвращены пропуска с любым статусом
+        pass_type: int = ""  # Тип возвращаемых пропусков. Значение параметра может быть пустым, в этом случае будут возвращены пропуска всех типов (Постоянный - 1, Временный - 2, Разовый - 4)
+        without_photo: bool = ""  # Флаг, определяющий, нужно ли возвращать фотографии владельцев пропусков (true если фотографии возвращать не нужно).
+        start_numer: int = ""  # Порядковый номер, начиная с которого будут возвращены пропуска (постраничный вывод). Значение параметра может быть пустым, в этом случае будут возвращаться пропуска начиная с первого
+        max_count: int = ""  # Максимальное количество пропусков, которое будет возвращено методом (постраничный вывод). Значение параметра может быть пустым, в этом случае количество возвращаемых пропусков ограничиваться не будет
 
 
 
 class GetPassByPersonDto(BaseModel):
     """Тип Pass представляет краткий набор данных персонального пропуска или заявки на пропуск.
     get_material_pass_by_person
     get_car_pass_by_person_pass
```

### Comparing `bastion_api-0.2.0/src/bastion_api/dto/person_dto.py` & `bastion_api-0.2.2/src/bastion_api/dto/person_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.0/src/bastion_api/dto/points_dto.py` & `bastion_api-0.2.2/src/bastion_api/dto/points_dto.py`

 * *Files identical despite different names*

### Comparing `bastion_api-0.2.0/src/bastion_api/dto/support.py` & `bastion_api-0.2.2/src/bastion_api/dto/support.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-
 from pydantic import BaseModel
 
+
 class DictValDto(BaseModel):
     """Тип DictVal представляет данные словарного значения. Используется в методе запроса словарных
         значений GetDictVals"""
     category: int  # Категория словарного значения
     value: str  # Текст словарного значения
 
 
-
-
 class TimeIntervalDto(BaseModel):
     """Объект типа TimeInterval представляет собой временной промежуток, фигурирующий в уровне
 доступа, привязанному к пропуску в СКУД АПК «Бастион-2». Объект типа TimeInterval является
 полем в типе данных Pass, использующемся в методе создания/редактирования пропуска/заявки
 на пропуск PutPass и в методе получения коллекции пропусков GetPasses"""
     timeStart: str  # Время начала действия пропуска в течение дня HH:MM:SS
     timeEnd: str  # Время окончания действия пропуска в течение дня HH:MM:SS
@@ -62,20 +60,22 @@
     carYear: int = None  # Год выпуска
     carColorStr: str = None  # Цвет
     carWeight: str = None  # Вес
     carVolume: str = None  # Версия
     carOwnerStr: str = None  # Владелец
     carTypeStr: str = None  # Тип
 
+
 class PersonBriefDto(BaseModel):
     """представляет собой краткий набор данных персоны"""
     name: str
     firstName: str = None
     secondName: str = None
     birthDate: str = None
 
+
 class PassBriefDto(BaseModel):
     """Тип Pass представляет краткий набор данных персонального пропуска или заявки на пропуск."""
     CardCode: str
     PersonData: PersonBriefDto
     PassType: int
     CardStatus: int
```

### Comparing `bastion_api-0.2.0/src/bastion_api/handlers.py` & `bastion_api-0.2.2/src/bastion_api/handlers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from pydantic import BaseModel
+
 
 
 class BastionIntegrationError(Exception):
     error_type: str = "C"
     default_class: int = 999
     default_subclass: int = 999
     context: Dict[str, str | int] = None
@@ -27,7 +27,12 @@
             "code": f"{self.error_type}-{self.default_class}-{self.default_subclass}",
             "class": self.default_class,
             "subclass": self.default_subclass,
             "comment": self.message
         }
 
 
+async def _handle_response(response, dto):
+    model_list = []
+    for info in response:
+        model_list.append(dto(**info))
+    return model_list
```

### Comparing `bastion_api-0.2.0/PKG-INFO` & `bastion_api-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bastion-api
-Version: 0.2.0
+Version: 0.2.2
 Summary: Модуль интеграции с API Бастоин ИКС
 Author: Mrkorogod
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

